# Comparing `tmp/kaiju_app-0.1.2-py3-none-any.whl.zip` & `tmp/kaiju_app-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 18679 bytes, number of entries: 13
--rw-r--r--  2.0 unx      314 b- defN 24-Apr-25 10:10 kaiju_app/__init__.py
--rw-r--r--  2.0 unx    16625 b- defN 24-Apr-25 10:10 kaiju_app/app.py
--rw-r--r--  2.0 unx     1473 b- defN 24-Apr-25 10:10 kaiju_app/bases.py
--rw-r--r--  2.0 unx     4410 b- defN 24-Apr-25 10:10 kaiju_app/configurator.py
--rw-r--r--  2.0 unx      314 b- defN 24-Apr-25 10:10 kaiju_app/interfaces.py
--rw-r--r--  2.0 unx     9992 b- defN 24-Apr-25 10:10 kaiju_app/loader.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 10:10 kaiju_app/py.typed
--rw-r--r--  2.0 unx    14232 b- defN 24-Apr-25 10:10 kaiju_app/utils.py
--rw-r--r--  2.0 unx     1069 b- defN 24-Apr-25 10:10 kaiju_app-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     5156 b- defN 24-Apr-25 10:10 kaiju_app-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 10:10 kaiju_app-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-Apr-25 10:10 kaiju_app-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1007 b- defN 24-Apr-25 10:10 kaiju_app-0.1.2.dist-info/RECORD
-13 files, 54694 bytes uncompressed, 17015 bytes compressed:  68.9%
+Zip file size: 18776 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      314 b- defN 24-Apr-27 14:25 kaiju_app/__init__.py
+-rw-r--r--  2.0 unx    16952 b- defN 24-Apr-27 14:25 kaiju_app/app.py
+-rw-r--r--  2.0 unx     1473 b- defN 24-Apr-27 14:25 kaiju_app/bases.py
+-rw-r--r--  2.0 unx     4410 b- defN 24-Apr-27 14:25 kaiju_app/configurator.py
+-rw-r--r--  2.0 unx      314 b- defN 24-Apr-27 14:25 kaiju_app/interfaces.py
+-rw-r--r--  2.0 unx     9992 b- defN 24-Apr-27 14:25 kaiju_app/loader.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-27 14:25 kaiju_app/py.typed
+-rw-r--r--  2.0 unx    14232 b- defN 24-Apr-27 14:25 kaiju_app/utils.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-Apr-27 14:25 kaiju_app-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5156 b- defN 24-Apr-27 14:25 kaiju_app-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-27 14:25 kaiju_app-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-Apr-27 14:25 kaiju_app-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1007 b- defN 24-Apr-27 14:25 kaiju_app-0.1.3.dist-info/RECORD
+13 files, 55021 bytes uncompressed, 17112 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: kaiju_app/py.typed
 Comment: 
 
 Filename: kaiju_app/utils.py
 Comment: 
 
-Filename: kaiju_app-0.1.2.dist-info/LICENSE
+Filename: kaiju_app-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_app-0.1.2.dist-info/METADATA
+Filename: kaiju_app-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_app-0.1.2.dist-info/WHEEL
+Filename: kaiju_app-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_app-0.1.2.dist-info/top_level.txt
+Filename: kaiju_app-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_app-0.1.2.dist-info/RECORD
+Filename: kaiju_app-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_app/__init__.py

```diff
@@ -4,8 +4,8 @@
 from kaiju_app.bases import *
 from kaiju_app.configurator import *
 from kaiju_app.loader import *
 
 __python_version__ = "3.12"
 __author__ = "violetblackdev@gmail.com"
 __license__ = "MIT"
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

## kaiju_app/app.py

```diff
@@ -5,15 +5,15 @@
 from contextlib import suppress
 from contextvars import ContextVar
 from dataclasses import MISSING, Field, dataclass, field
 from enum import Enum
 from types import MappingProxyType
 from typing import Any, Awaitable, Callable, Self, TypedDict, TypeVar, final
 
-from kaiju_scheduler import Scheduler, ScheduledTask
+from kaiju_scheduler import Scheduler, ScheduledTask, Server
 from uvlog import Logger
 
 from kaiju_app.bases import Error
 from kaiju_app.utils import State, timeout, Namespace
 
 __all__ = [
     "Application",
@@ -247,20 +247,26 @@
 
     post_init_timeout_s: float = 300.0
     """A post-init task timeout (sec) for ALL the services combined."""
 
     show_inspection_on_start: bool = False
     """Show inspection data in logs after the app start."""
 
+    max_parallel_tasks: int = 128
+    """Max parallel asyncio tasks submitted to the internal application server simultaneously."""
+
     metadata: dict = field(default_factory=dict)
     """Application metadata not used by it directly."""
 
     scheduler: Scheduler = field(init=False)
     """Internal task scheduler."""
 
+    server: Server = field(init=False)
+    """Internal task server."""
+
     optional_services: list[str] = field(default_factory=list)
     """List of optional services not required for the app start."""
 
     services: MappingProxyType[str, Service] = field(init=False, default=MappingProxyType({}))
     """Application services registry."""
 
     namespace: Namespace = field(init=False, default=Namespace())
@@ -273,14 +279,15 @@
     """Mutable mapping of all application services on their names."""
 
     _post_init_task: asyncio.Future | None = field(init=False, default=None)
 
     def __post_init__(self):
         """Initialize."""
         self.scheduler = Scheduler(logger=self.logger.get_child("_scheduler"))
+        self.server = Server(logger=self.logger.get_child("_server"), max_parallel_tasks=self.max_parallel_tasks)
         self.services = MappingProxyType(self._service_map)
         self.namespace = Namespace(self.env, self.name)
 
     def add_services(self, *services: Service) -> None:
         """Add new services to the application.
 
         The loading order must be resolved.
```

## Comparing `kaiju_app-0.1.2.dist-info/LICENSE` & `kaiju_app-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_app-0.1.2.dist-info/METADATA` & `kaiju_app-0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-app
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python modular application and services
 Home-page: https://github.com/violet-black/kaiju-app
 Author: violetblackdev@gmail.com
 License: MIT
 Keywords: application,microservice,asyncio,infrastructure
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

