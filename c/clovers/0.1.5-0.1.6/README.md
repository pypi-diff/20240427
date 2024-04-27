# Comparing `tmp/clovers-0.1.5.tar.gz` & `tmp/clovers-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clovers-0.1.5.tar", max compression
+gzip compressed data, was "clovers-0.1.6.tar", max compression
```

## Comparing `clovers-0.1.5.tar` & `clovers-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2975 2024-04-25 16:17:20.354668 clovers-0.1.5/clovers/__init__.py
--rw-r--r--   0        0        0     3250 2024-04-25 15:57:07.509856 clovers-0.1.5/clovers/core/adapter.py
--rw-r--r--   0        0        0      582 2024-04-15 03:01:44.120813 clovers-0.1.5/clovers/core/config.py
--rw-r--r--   0        0        0       57 2024-04-25 15:35:33.878533 clovers-0.1.5/clovers/core/logger.py
--rw-r--r--   0        0        0     6815 2024-04-25 15:57:43.990068 clovers-0.1.5/clovers/core/plugin.py
--rw-r--r--   0        0        0     2774 2024-04-15 02:23:00.885679 clovers-0.1.5/clovers/utils/library.py
--rw-r--r--   0        0        0    10961 2024-04-16 04:46:17.581644 clovers-0.1.5/clovers/utils/linecard.py
--rw-r--r--   0        0        0     1884 2024-04-15 08:48:00.582248 clovers-0.1.5/clovers/utils/tools.py
--rw-r--r--   0        0        0     1086 2024-04-15 03:18:25.255783 clovers-0.1.5/LICENSE
--rw-r--r--   0        0        0      645 2024-04-25 14:38:39.377101 clovers-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    10284 2024-04-23 16:13:55.973406 clovers-0.1.5/README.md
--rw-r--r--   0        0        0    10627 1970-01-01 00:00:00.000000 clovers-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     2975 2024-04-26 12:12:23.702750 clovers-0.1.6/clovers/__init__.py
+-rw-r--r--   0        0        0     3250 2024-04-26 12:12:23.702750 clovers-0.1.6/clovers/core/adapter.py
+-rw-r--r--   0        0        0      582 2024-04-26 12:12:23.703249 clovers-0.1.6/clovers/core/config.py
+-rw-r--r--   0        0        0       57 2024-04-26 12:12:23.703249 clovers-0.1.6/clovers/core/logger.py
+-rw-r--r--   0        0        0     6820 2024-04-26 12:19:20.500935 clovers-0.1.6/clovers/core/plugin.py
+-rw-r--r--   0        0        0     2774 2024-04-26 12:12:23.704249 clovers-0.1.6/clovers/utils/library.py
+-rw-r--r--   0        0        0    10961 2024-04-26 12:12:23.704249 clovers-0.1.6/clovers/utils/linecard.py
+-rw-r--r--   0        0        0     1884 2024-04-26 12:12:23.704749 clovers-0.1.6/clovers/utils/tools.py
+-rw-r--r--   0        0        0     1086 2024-04-26 12:12:23.701749 clovers-0.1.6/LICENSE
+-rw-r--r--   0        0        0      645 2024-04-26 12:21:42.779928 clovers-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    10284 2024-04-26 12:12:23.702250 clovers-0.1.6/README.md
+-rw-r--r--   0        0        0    10627 1970-01-01 00:00:00.000000 clovers-0.1.6/PKG-INFO
```

### Comparing `clovers-0.1.5/clovers/__init__.py` & `clovers-0.1.6/clovers/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.5/clovers/core/adapter.py` & `clovers-0.1.6/clovers/core/adapter.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.5/clovers/core/config.py` & `clovers-0.1.6/clovers/core/config.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.5/clovers/core/plugin.py` & `clovers-0.1.6/clovers/core/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,25 +57,24 @@
         self.temp_handles: dict[str, tuple[float, Handle]] = {}
         self.startup_tasklist: list[Coroutine] = []
         self.shutdown_tasklist: list[Coroutine] = []
         self.build_event: Callable | None = build_event
         self.build_result: Callable | None = build_result
 
     def handle_warpper(self, func: Callable[..., Coroutine]):
-        if build_event := self.build_event:
-            func = lambda e: func(build_event(e))
-        if build_result := self.build_result:
+        middle_func = lambda e: func(build_event(e))if (build_event := self.build_event) else func
 
+        if build_result := self.build_result:
             async def wrapper(event):
-                if result := await func(event):
+                if result := await middle_func(event):
                     return build_result(result)
 
             return wrapper
         else:
-            return lambda e: func(e)
+            return middle_func
 
     def commands_register(self, commands: PluginCommands, key: int):
         if not commands:
             self.command_dict.setdefault("", set()).add(key)
         elif isinstance(commands, set):
             for command in commands:
                 self.command_dict.setdefault(command, set()).add(key)
```

### Comparing `clovers-0.1.5/clovers/utils/library.py` & `clovers-0.1.6/clovers/utils/library.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.5/clovers/utils/linecard.py` & `clovers-0.1.6/clovers/utils/linecard.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.5/clovers/utils/tools.py` & `clovers-0.1.6/clovers/utils/tools.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.5/LICENSE` & `clovers-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `clovers-0.1.5/pyproject.toml` & `clovers-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clovers"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["KarisAya <1048827424@qq.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 toml = "^0.10.2"
```

### Comparing `clovers-0.1.5/README.md` & `clovers-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `clovers-0.1.5/PKG-INFO` & `clovers-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clovers
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

