# Comparing `tmp/clovers-0.1.6.tar.gz` & `tmp/clovers-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clovers-0.1.6.tar", max compression
+gzip compressed data, was "clovers-0.1.7.tar", max compression
```

## Comparing `clovers-0.1.6.tar` & `clovers-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2975 2024-04-26 12:12:23.702750 clovers-0.1.6/clovers/__init__.py
--rw-r--r--   0        0        0     3250 2024-04-26 12:12:23.702750 clovers-0.1.6/clovers/core/adapter.py
--rw-r--r--   0        0        0      582 2024-04-26 12:12:23.703249 clovers-0.1.6/clovers/core/config.py
--rw-r--r--   0        0        0       57 2024-04-26 12:12:23.703249 clovers-0.1.6/clovers/core/logger.py
--rw-r--r--   0        0        0     6820 2024-04-26 12:19:20.500935 clovers-0.1.6/clovers/core/plugin.py
--rw-r--r--   0        0        0     2774 2024-04-26 12:12:23.704249 clovers-0.1.6/clovers/utils/library.py
--rw-r--r--   0        0        0    10961 2024-04-26 12:12:23.704249 clovers-0.1.6/clovers/utils/linecard.py
--rw-r--r--   0        0        0     1884 2024-04-26 12:12:23.704749 clovers-0.1.6/clovers/utils/tools.py
--rw-r--r--   0        0        0     1086 2024-04-26 12:12:23.701749 clovers-0.1.6/LICENSE
--rw-r--r--   0        0        0      645 2024-04-26 12:21:42.779928 clovers-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    10284 2024-04-26 12:12:23.702250 clovers-0.1.6/README.md
--rw-r--r--   0        0        0    10627 1970-01-01 00:00:00.000000 clovers-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     3417 2024-04-27 01:16:04.378247 clovers-0.1.7/clovers/__init__.py
+-rw-r--r--   0        0        0     3250 2024-04-26 17:09:52.294168 clovers-0.1.7/clovers/core/adapter.py
+-rw-r--r--   0        0        0      582 2024-04-26 17:09:52.294168 clovers-0.1.7/clovers/core/config.py
+-rw-r--r--   0        0        0       57 2024-04-26 17:09:52.294668 clovers-0.1.7/clovers/core/logger.py
+-rw-r--r--   0        0        0     6820 2024-04-26 17:09:52.294668 clovers-0.1.7/clovers/core/plugin.py
+-rw-r--r--   0        0        0     2774 2024-04-26 17:09:52.295168 clovers-0.1.7/clovers/utils/library.py
+-rw-r--r--   0        0        0    10961 2024-04-26 17:09:52.295668 clovers-0.1.7/clovers/utils/linecard.py
+-rw-r--r--   0        0        0     1884 2024-04-26 17:09:52.295668 clovers-0.1.7/clovers/utils/tools.py
+-rw-r--r--   0        0        0     1086 2024-04-26 17:09:52.292667 clovers-0.1.7/LICENSE
+-rw-r--r--   0        0        0      645 2024-04-26 18:18:26.413628 clovers-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    10284 2024-04-26 17:09:52.293167 clovers-0.1.7/README.md
+-rw-r--r--   0        0        0    10525 1970-01-01 00:00:00.000000 clovers-0.1.7/PKG-INFO
```

### Comparing `clovers-0.1.6/clovers/__init__.py` & `clovers-0.1.7/clovers/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 from collections.abc import Awaitable
-from .core.plugin import Plugin, Event
+from .core.plugin import Plugin, PluginLoader, Event
 from .core.adapter import Adapter
 from .core.logger import logger
 
 
 class Clovers:
     def __init__(self) -> None:
         self.global_adapter: Adapter = Adapter()
@@ -21,17 +21,28 @@
             if data := plugin(command):
                 task_list.extend(adapter.response_safe(plugin.handles[key], event, extra) for key, event in data.items())
             if plugin.temp_check():
                 event = Event(command, [])
                 task_list.extend(adapter.response_safe(handle, event, extra) for _, handle in plugin.temp_handles.values())
         return sum(await asyncio.gather(*task_list)) if task_list else 0
 
+    def load_plugin(self, name: str):
+        if self.wait_for:
+            raise RuntimeError("cannot loading plugin after clovers startup")
+        plugin = PluginLoader.load(name)
+        if plugin is None:
+            logger.error(f"未找到 {name}")
+        elif plugin not in self.plugins:
+            self.plugins.append(plugin)
+            logger.info(f"{name} 加载成功")
+        else:
+            logger.info(f"{name} 已存在")
+
     async def startup(self):
-        task_list = [task for plugin in self.plugins for task in plugin.startup_tasklist]
-        self.wait_for.append(asyncio.gather(*task_list))
+        self.wait_for.extend(asyncio.create_task(task) for plugin in self.plugins for task in plugin.startup_tasklist)
         self.wait_for.extend(task for plugin in self.plugins for task in plugin.shutdown_tasklist)
         # 混合全局方法
         # 过滤没有指令响应任务的插件
         # 检查任务需求的参数是否存在于响应器获取参数方法。
         extra_args_dict: dict[str, set[str]] = {}
         for adapter_key, adapter in self.adapter_dict.items():
             adapter.remix(self.global_adapter)
```

### Comparing `clovers-0.1.6/clovers/core/adapter.py` & `clovers-0.1.7/clovers/core/adapter.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.6/clovers/core/config.py` & `clovers-0.1.7/clovers/core/config.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.6/clovers/core/plugin.py` & `clovers-0.1.7/clovers/core/plugin.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.6/clovers/utils/library.py` & `clovers-0.1.7/clovers/utils/library.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.6/clovers/utils/linecard.py` & `clovers-0.1.7/clovers/utils/linecard.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.6/clovers/utils/tools.py` & `clovers-0.1.7/clovers/utils/tools.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.6/LICENSE` & `clovers-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `clovers-0.1.6/pyproject.toml` & `clovers-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "clovers"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["KarisAya <1048827424@qq.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.12"
 toml = "^0.10.2"
 fonttools = {version = "^4.51.0", optional = true}
 pillow = {version = "^10.3.0", optional = true}
 matplotlib = {version = "^3.8.4", optional = true}
 numpy = {version = "^1.26.4", optional = true}
 httpx = {version = "^0.27.0", optional = true}
```

### Comparing `clovers-0.1.6/README.md` & `clovers-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `clovers-0.1.6/PKG-INFO` & `clovers-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: clovers
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: linecard
 Provides-Extra: tools
 Requires-Dist: fonttools (>=4.51.0,<5.0.0) ; extra == "linecard"
 Requires-Dist: httpx (>=0.27.0,<0.28.0) ; extra == "tools"
 Requires-Dist: matplotlib (>=3.8.4,<4.0.0) ; extra == "linecard"
 Requires-Dist: numpy (>=1.26.4,<2.0.0) ; extra == "tools"
 Requires-Dist: pillow (>=10.3.0,<11.0.0) ; extra == "linecard"
```

