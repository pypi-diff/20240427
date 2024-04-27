# Comparing `tmp/cheeseapi-1.1.1.tar.gz` & `tmp/cheeseapi-1.1.2.tar.gz`

## Comparing `cheeseapi-1.1.1.tar` & `cheeseapi-1.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 cheeseapi-1.1.1/CheeseAPI/__init__.py
--rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 cheeseapi-1.1.1/CheeseAPI/app.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 cheeseapi-1.1.1/CheeseAPI/cors.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cheeseapi-1.1.1/CheeseAPI/exception.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 cheeseapi-1.1.1/CheeseAPI/file.py
--rw-r--r--   0        0        0    32439 2020-02-02 00:00:00.000000 cheeseapi-1.1.1/CheeseAPI/handle.py
--rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 cheeseapi-1.1.1/CheeseAPI/protocol.py
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 cheeseapi-1.1.1/CheeseAPI/request.py
--rw-r--r--   0        0        0    17621 2020-02-02 00:00:00.000000 cheeseapi-1.1.1/CheeseAPI/response.py
--rw-r--r--   0        0        0    11152 2020-02-02 00:00:00.000000 cheeseapi-1.1.1/CheeseAPI/route.py
--rw-r--r--   0        0        0    10335 2020-02-02 00:00:00.000000 cheeseapi-1.1.1/CheeseAPI/schedule.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 cheeseapi-1.1.1/CheeseAPI/server.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 cheeseapi-1.1.1/CheeseAPI/signal.py
--rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 cheeseapi-1.1.1/CheeseAPI/text.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 cheeseapi-1.1.1/CheeseAPI/validator.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 cheeseapi-1.1.1/CheeseAPI/websocket.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 cheeseapi-1.1.1/CheeseAPI/workspace.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cheeseapi-1.1.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-1.1.1/LICENSE
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 cheeseapi-1.1.1/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cheeseapi-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     5021 2020-02-02 00:00:00.000000 cheeseapi-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/__init__.py
+-rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/app.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/cors.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/exception.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/file.py
+-rw-r--r--   0        0        0    32439 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/handle.py
+-rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/protocol.py
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/request.py
+-rw-r--r--   0        0        0    17621 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/response.py
+-rw-r--r--   0        0        0    11145 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/route.py
+-rw-r--r--   0        0        0    10335 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/schedule.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/server.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/signal.py
+-rw-r--r--   0        0        0     8509 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/text.py
+-rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/validator.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/websocket.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/workspace.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/LICENSE
+-rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/PKG-INFO
```

### Comparing `cheeseapi-1.1.1/CheeseAPI/app.py` & `cheeseapi-1.1.2/CheeseAPI/app.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.1/CheeseAPI/cors.py` & `cheeseapi-1.1.2/CheeseAPI/cors.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.1/CheeseAPI/exception.py` & `cheeseapi-1.1.2/CheeseAPI/exception.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.1/CheeseAPI/file.py` & `cheeseapi-1.1.2/CheeseAPI/file.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.1/CheeseAPI/handle.py` & `cheeseapi-1.1.2/CheeseAPI/handle.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.1/CheeseAPI/protocol.py` & `cheeseapi-1.1.2/CheeseAPI/protocol.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.1/CheeseAPI/request.py` & `cheeseapi-1.1.2/CheeseAPI/request.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.1/CheeseAPI/response.py` & `cheeseapi-1.1.2/CheeseAPI/response.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.1/CheeseAPI/route.py` & `cheeseapi-1.1.2/CheeseAPI/route.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                 'pattern': r'.+',
                 'type': str,
                 'weight': 0
             }
         ]
         self._node: RouteNode = RouteNode()
 
-    def addPattern(self, key: str, pattern: re.Pattern, type: object | Callable, weight: int):
+    def addPattern(self, key: str, pattern: str, type: object | Callable, weight: int):
         '''
         新增动态路由匹配条件。
 
         - Args
 
             - key: 在动态路由中的key。
```

### Comparing `cheeseapi-1.1.1/CheeseAPI/schedule.py` & `cheeseapi-1.1.2/CheeseAPI/schedule.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.1/CheeseAPI/server.py` & `cheeseapi-1.1.2/CheeseAPI/server.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.1/CheeseAPI/signal.py` & `cheeseapi-1.1.2/CheeseAPI/signal.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.1/CheeseAPI/text.py` & `cheeseapi-1.1.2/CheeseAPI/text.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os, time, traceback
-from typing import TYPE_CHECKING, List, Tuple
+from typing import TYPE_CHECKING, List, Tuple, Any
 
 import setproctitle
 from CheeseLog import ProgressBar, logger
 
 if TYPE_CHECKING:
     from CheeseAPI.app import App
     from CheeseAPI.protocol import HttpProtocol, WebsocketProtocol
@@ -146,14 +146,32 @@
         message += '{:.6f} seconds'.format(timer % 60)
         styledMessage += '<blue>{:.6f}</blue> seconds'.format(timer % 60)
 
         return [
             (message, styledMessage)
         ]
 
+    def validator_requiredMessage(self, scope: str, key: str) -> str:
+        return f'参数{scope}.{key}是必要的'
+
+    def validator_typeMessage(self, scope: str, key: str, expected_type: object) -> str:
+        return f'参数{scope}.{key}无法转换为{expected_type.__name__}'
+
+    def validator_patternMessage(self, scope: str, key: str) -> str:
+        return f'参数{scope}.{key}正则校验错误'
+
+    def validator_minMessage(self, scope: str, key: str, min: object) -> str:
+        return f'参数{scope}.{key}不允许小于{min}'
+
+    def validator_maxMessage(self, scope: str, key: str, max: object) -> str:
+        return f'参数{scope}.{key}不允许大于{max}'
+
+    def validator_enumMessage(self, scope: str, key: str, enum: List[Any]) -> str:
+        return f'参数{scope}.{key}不允许为{enum}之外的值'
+
     @property
     def process_title(self) -> str:
         return self._process_title
 
     @process_title.setter
     def process_title(self, value: str):
         self._process_title = value
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cheeseapi-1.1.1/CheeseAPI/websocket.py` & `cheeseapi-1.1.2/CheeseAPI/websocket.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from CheeseAPI.request import Request
 
 class WebsocketServer:
     async def subprotocol(self, *, request: 'Request', **kwargs) -> str | None:
         ...
```

### Comparing `cheeseapi-1.1.1/LICENSE` & `cheeseapi-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.1/README.md` & `cheeseapi-1.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -51,21 +51,23 @@
 | 文件名 | 备注 |
 | - | - |
 | \_\_init\_\_.py | 公用变量 |
 | model.py | ORM或类 |
 | api.py | API接口 |
 | service.py | 业务逻辑实现 |
 | handle.py | 插槽逻辑 |
+| validator.py | 参数校验 |
 
 一般来说，模块中的文件调用有明显的顺序关系（从顶层到底层）：
 
 ```
-handle.py ---
-            |-> service.py -> model.py -> __init__.py
-api.py ------
+validator.py -> api.py -----|
+                            |-> service.py -> model.py -> __init__.py
+                handle.py --|
+
 ```
 
 ## **使用**
 
 创建一个启动入口文件`app.py`：
 
 ```python
@@ -106,40 +108,46 @@
 (DEBUG) 2024-03-19 14:05:40.350681 > The process 346 stopped
 (ENDING) 2024-03-19 14:05:40.350816 > The server runs for a total of 2 minutes 27.944854 seconds
 (ENDING) 2024-03-19 14:05:40.350849 > The master process 346 stopped
 ```
 
 ## **更多...**
 
-### 1. [**App （主模块）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App.md)
+### 1. [**Demo**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Demo.md)
+
+#### 1.1 [**简单的增删改查 (CRUD)**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/demo/CRUD)
+
+### 2. [**App （主模块）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App.md)
+
+#### 2.1 [**Server （服务器配置）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Server.md)
 
-#### 1.1 [**Server （服务器配置）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Server.md)
+#### 2.2 [**Workspace （工作区配置）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Workspace.md)
 
-#### 1.2 [**Workspace （工作区配置）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Workspace.md)
+#### 2.3 [**Signal （信号插槽）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Signal.md)
 
-#### 1.3 [**Signal （信号插槽）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Signal.md)
+#### 2.4 [**RouteBus （路由总线）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/RouteBus.md)
 
-#### 1.4 [**RouteBus （路由总线）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/RouteBus.md)
+#### 2.5 [**Cors （跨域管理）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Cors.md)
 
-#### 1.5 [**Cors （跨域管理）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Cors.md)
+#### 2.6 [**Scheduler （任务调度者）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Scheduler.md)
 
-#### 1.6 [**Scheduler （任务调度者）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Scheduler.md)
+### 3. [**Request （请求体）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Request.md)
 
-### 2. [**Request （请求体）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Request.md)
+### 4. [**Response （响应体）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Response.md)
 
-### 3. [**Response （响应体）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Response.md)
+### 5. [**Route （路由）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Route.md)
 
-### 4. [**Route （路由）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Route.md)
+### 6. [**Websocket**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Websocket.md)
 
-### 5. [**Websocket**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Websocket.md)
+### 7. [**File （文件）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/File.md)
 
-### 6. [**File （文件）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/File.md)
+### 8. [**Validator （校验器）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Validator.md)
 
-### 7. [**Schedule （任务调度）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Schedule.md)
+### 9. [**Schedule （任务调度）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Schedule.md)
 
-### 8. [**For 开发者**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Developer.md)
+### 10. [**For 开发者**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Developer.md)
 
 ## **可用的插件模块**
 
 ### 1. **[CheeseAPI_Websocket](https://github.com/CheeseUnknown/CheeseAPI_Websocket)**
 
 websocket的升级插件，支持了更多、更便捷的通讯方式。
```

### Comparing `cheeseapi-1.1.1/pyproject.toml` & `cheeseapi-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "CheeseAPI"
-version = "1.1.1"
+version = "1.1.2"
 description = "一款web协程框架。"
 readme = "README.md"
 license-files = { paths = [ "LICENSE" ] }
 authors = [
     { name = "Cheese Unknown", email = "cheese@cheese.ren" }
 ]
 keywords = [ 'API', 'BackEnd' ]
```

### Comparing `cheeseapi-1.1.1/PKG-INFO` & `cheeseapi-1.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: CheeseAPI
-Version: 1.1.1
+Version: 1.1.2
 Summary: 一款web协程框架。
 Project-URL: Source, https://github.com/CheeseUnknown/CheeseAPI
 Author-email: Cheese Unknown <cheese@cheese.ren>
 License-File: LICENSE
 Keywords: API,BackEnd
 Requires-Dist: cheeselog==1.0.*
 Requires-Dist: cheesesignal==1.1.*
@@ -68,21 +68,23 @@
 | 文件名 | 备注 |
 | - | - |
 | \_\_init\_\_.py | 公用变量 |
 | model.py | ORM或类 |
 | api.py | API接口 |
 | service.py | 业务逻辑实现 |
 | handle.py | 插槽逻辑 |
+| validator.py | 参数校验 |
 
 一般来说，模块中的文件调用有明显的顺序关系（从顶层到底层）：
 
 ```
-handle.py ---
-            |-> service.py -> model.py -> __init__.py
-api.py ------
+validator.py -> api.py -----|
+                            |-> service.py -> model.py -> __init__.py
+                handle.py --|
+
 ```
 
 ## **使用**
 
 创建一个启动入口文件`app.py`：
 
 ```python
@@ -123,40 +125,46 @@
 (DEBUG) 2024-03-19 14:05:40.350681 > The process 346 stopped
 (ENDING) 2024-03-19 14:05:40.350816 > The server runs for a total of 2 minutes 27.944854 seconds
 (ENDING) 2024-03-19 14:05:40.350849 > The master process 346 stopped
 ```
 
 ## **更多...**
 
-### 1. [**App （主模块）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App.md)
+### 1. [**Demo**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Demo.md)
+
+#### 1.1 [**简单的增删改查 (CRUD)**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/demo/CRUD)
+
+### 2. [**App （主模块）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App.md)
+
+#### 2.1 [**Server （服务器配置）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Server.md)
 
-#### 1.1 [**Server （服务器配置）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Server.md)
+#### 2.2 [**Workspace （工作区配置）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Workspace.md)
 
-#### 1.2 [**Workspace （工作区配置）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Workspace.md)
+#### 2.3 [**Signal （信号插槽）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Signal.md)
 
-#### 1.3 [**Signal （信号插槽）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Signal.md)
+#### 2.4 [**RouteBus （路由总线）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/RouteBus.md)
 
-#### 1.4 [**RouteBus （路由总线）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/RouteBus.md)
+#### 2.5 [**Cors （跨域管理）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Cors.md)
 
-#### 1.5 [**Cors （跨域管理）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Cors.md)
+#### 2.6 [**Scheduler （任务调度者）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Scheduler.md)
 
-#### 1.6 [**Scheduler （任务调度者）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Scheduler.md)
+### 3. [**Request （请求体）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Request.md)
 
-### 2. [**Request （请求体）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Request.md)
+### 4. [**Response （响应体）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Response.md)
 
-### 3. [**Response （响应体）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Response.md)
+### 5. [**Route （路由）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Route.md)
 
-### 4. [**Route （路由）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Route.md)
+### 6. [**Websocket**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Websocket.md)
 
-### 5. [**Websocket**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Websocket.md)
+### 7. [**File （文件）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/File.md)
 
-### 6. [**File （文件）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/File.md)
+### 8. [**Validator （校验器）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Validator.md)
 
-### 7. [**Schedule （任务调度）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Schedule.md)
+### 9. [**Schedule （任务调度）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Schedule.md)
 
-### 8. [**For 开发者**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Developer.md)
+### 10. [**For 开发者**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Developer.md)
 
 ## **可用的插件模块**
 
 ### 1. **[CheeseAPI_Websocket](https://github.com/CheeseUnknown/CheeseAPI_Websocket)**
 
 websocket的升级插件，支持了更多、更便捷的通讯方式。
```

