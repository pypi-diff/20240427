# Comparing `tmp/kaiju_scheduler-0.1.2-py3-none-any.whl.zip` & `tmp/kaiju_scheduler-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 8794 bytes, number of entries: 10
--rw-r--r--  2.0 unx      236 b- defN 24-Apr-24 18:52 kaiju_scheduler/__init__.py
--rw-r--r--  2.0 unx      267 b- defN 24-Apr-24 18:52 kaiju_scheduler/interfaces.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 18:52 kaiju_scheduler/py.typed
--rw-r--r--  2.0 unx    10734 b- defN 24-Apr-24 18:52 kaiju_scheduler/scheduler.py
--rw-r--r--  2.0 unx     2721 b- defN 24-Apr-24 18:52 kaiju_scheduler/utils.py
--rw-r--r--  2.0 unx     1069 b- defN 24-Apr-24 18:52 kaiju_scheduler-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     4680 b- defN 24-Apr-24 18:52 kaiju_scheduler-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 18:52 kaiju_scheduler-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-Apr-24 18:52 kaiju_scheduler-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      839 b- defN 24-Apr-24 18:52 kaiju_scheduler-0.1.2.dist-info/RECORD
-10 files, 20654 bytes uncompressed, 7350 bytes compressed:  64.4%
+Zip file size: 11404 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      273 b- defN 24-Apr-27 14:18 kaiju_scheduler/__init__.py
+-rw-r--r--  2.0 unx      267 b- defN 24-Apr-27 14:18 kaiju_scheduler/interfaces.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-27 14:18 kaiju_scheduler/py.typed
+-rw-r--r--  2.0 unx    10228 b- defN 24-Apr-27 14:18 kaiju_scheduler/scheduler.py
+-rw-r--r--  2.0 unx    11381 b- defN 24-Apr-27 14:18 kaiju_scheduler/server.py
+-rw-r--r--  2.0 unx     2733 b- defN 24-Apr-27 14:18 kaiju_scheduler/utils.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-Apr-27 14:18 kaiju_scheduler-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5546 b- defN 24-Apr-27 14:18 kaiju_scheduler-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-27 14:18 kaiju_scheduler-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-27 14:18 kaiju_scheduler-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      922 b- defN 24-Apr-27 14:18 kaiju_scheduler-0.1.3.dist-info/RECORD
+11 files, 32527 bytes uncompressed, 9834 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -6,26 +6,29 @@
 
 Filename: kaiju_scheduler/py.typed
 Comment: 
 
 Filename: kaiju_scheduler/scheduler.py
 Comment: 
 
+Filename: kaiju_scheduler/server.py
+Comment: 
+
 Filename: kaiju_scheduler/utils.py
 Comment: 
 
-Filename: kaiju_scheduler-0.1.2.dist-info/LICENSE
+Filename: kaiju_scheduler-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_scheduler-0.1.2.dist-info/METADATA
+Filename: kaiju_scheduler-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_scheduler-0.1.2.dist-info/WHEEL
+Filename: kaiju_scheduler-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_scheduler-0.1.2.dist-info/top_level.txt
+Filename: kaiju_scheduler-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_scheduler-0.1.2.dist-info/RECORD
+Filename: kaiju_scheduler-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_scheduler/__init__.py

```diff
@@ -1,9 +1,10 @@
 """Asynchronous tasks scheduler and executor."""
 
 from kaiju_scheduler.scheduler import *
+from kaiju_scheduler.server import *
 from kaiju_scheduler.utils import *
 
 __python_version__ = "3.8"
 __author__ = "violetblackdev@gmail.com"
 __license__ = "MIT"
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

## kaiju_scheduler/scheduler.py

```diff
@@ -133,26 +133,23 @@
     async def wait(self) -> None:
         """Wait until the current run has finished."""
         await self._idle.wait()
 
     def json_repr(self) -> Dict[str, Any]:
         """Get JSON compatible object state info."""
         return {
-            "cls": "Task",
-            "data": {
-                "name": self.name,
-                "policy": self._policy.value,
-                "enabled": self._enabled,
-                "started": not self._idle.is_set(),
-                "interval_s": self.interval_s,
-                "max_timeout_s": self.max_timeout_s,
-                "retries": self.retries,
-                "retry_interval_s": self.retry_interval_s,
-                "called_at": self._called_at,
-            },
+            "name": self.name,
+            "policy": self._policy.value,
+            "enabled": self._enabled,
+            "started": not self._idle.is_set(),
+            "interval_s": self.interval_s,
+            "max_timeout_s": self.max_timeout_s,
+            "retries": self.retries,
+            "retry_interval_s": self.retry_interval_s,
+            "called_at": self._called_at,
         }
 
     def run(self) -> None:
         self._executed_task = self._scheduler.loop.create_task(self._run(), name=self.name)
 
     def _logger(self, msg: str, /):
         if self._scheduler.logger is not None:
@@ -194,23 +191,17 @@
 
 @dataclass
 class Scheduler:
     """Schedule and execute local asynchronous functions periodically."""
 
     ExecPolicy: ClassVar = ExecPolicy
 
-    min_refresh_rate: ClassVar[float] = 0.1
-    """Minimum allowed refresh rate between cycles in seconds, limits `refresh_rate` value."""
-
     wait_task_timeout_safe_mod: ClassVar[float] = 4.0
     """Timeout modifier for WAIT tasks (to prevent them waiting forever)."""
 
-    refresh_rate: float = min_refresh_rate
-    """Refresh rate for the next cycle."""
-
     logger: Optional[Logger] = None
     """Optional logger instance."""
 
     loop: asyncio.AbstractEventLoop = None  # type: ignore
     """Asyncio loop to use with the scheduler."""
 
     tasks: List[ScheduledTask] = field(init=False, default_factory=list)
@@ -284,23 +275,15 @@
                 _tasks.append(executed_task)
 
         if _tasks:
             await asyncio.wait(_tasks)
 
     def json_repr(self) -> Dict[str, Any]:
         """Get JSON compatible object state info."""
-        return {
-            "cls": "Scheduler",
-            "data": {
-                "started": self._started,
-                "time": self.loop.time(),
-                "refresh_rate": self.refresh_rate,
-                "tasks": [task.json_repr() for task in self.tasks],
-            },
-        }
+        return {"started": self._started, "time": self.loop.time(), "tasks": [task.json_repr() for task in self.tasks]}
 
     async def __aenter__(self) -> "Scheduler":
         await self.start()
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await self.stop()
```

## kaiju_scheduler/utils.py

```diff
@@ -1,13 +1,12 @@
 """Utility classes and functions."""
 
 import asyncio
-from collections.abc import Mapping
 from types import MappingProxyType
-from typing import Any, Awaitable, Callable, Optional, Tuple, Type, TypeVar
+from typing import Any, Awaitable, Callable, Iterable, Mapping, Optional, Tuple, Type, TypeVar
 
 from kaiju_scheduler.interfaces import Logger
 
 __all__ = ["timeout", "retry", "RetryError"]
 
 
 _Item = TypeVar("_Item")
@@ -46,28 +45,28 @@
             loop = self._loop
         task = asyncio.current_task()
         self._handler = loop.call_at(loop.time() + self._timeout, self._cancel_task, task)
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         if exc_type is asyncio.CancelledError:
-            raise asyncio.TimeoutError
+            raise asyncio.TimeoutError("Timeout")
         if self._handler:
             self._handler.cancel()
 
     @staticmethod
     def _cancel_task(task: asyncio.Task):
         task.cancel()
 
 
 async def retry(
     func: Callable[..., Awaitable[Any]],
     retries: int,
-    args: tuple = tuple(),
-    kws: Mapping = MappingProxyType({}),
+    args: Iterable[Any] = tuple(),
+    kws: Mapping[str, Any] = MappingProxyType({}),
     *,
     interval_s: float = 1.0,
     timeout_s: float = 120.0,
     catch_exceptions: Tuple[Type[BaseException], ...] = (TimeoutError, IOError, ConnectionError, RetryError),
     logger: Optional[Logger] = None,
 ):
     """Retry function call
```

## Comparing `kaiju_scheduler-0.1.2.dist-info/LICENSE` & `kaiju_scheduler-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

