# Comparing `tmp/rate_control-3.0.0.tar.gz` & `tmp/rate_control-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rate_control-3.0.0.tar", max compression
+gzip compressed data, was "rate_control-3.0.1.tar", max compression
```

## Comparing `rate_control-3.0.0.tar` & `rate_control-3.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1101 2024-04-21 05:06:56.403097 rate_control-3.0.0/LICENSE
--rw-r--r--   0        0        0     3822 2024-04-21 05:06:56.403097 rate_control-3.0.0/README.rst
--rw-r--r--   0        0        0     2872 2024-04-21 05:07:01.275188 rate_control-3.0.0/pyproject.toml
--rw-r--r--   0        0        0      582 2024-04-21 05:06:56.403097 rate_control-3.0.0/rate_control/__init__.py
--rw-r--r--   0        0        0     3673 2024-04-21 05:06:56.403097 rate_control-3.0.0/rate_control/_bucket_group.py
--rw-r--r--   0        0        0      267 2024-04-21 05:06:56.403097 rate_control-3.0.0/rate_control/_buckets/__init__.py
--rw-r--r--   0        0        0      344 2024-04-21 05:06:56.403097 rate_control-3.0.0/rate_control/_buckets/_base/__init__.py
--rw-r--r--   0        0        0     2005 2024-04-21 05:06:56.403097 rate_control-3.0.0/rate_control/_buckets/_base/_abc.py
--rw-r--r--   0        0        0     2479 2024-04-21 05:06:56.403097 rate_control-3.0.0/rate_control/_buckets/_base/_base_rate.py
--rw-r--r--   0        0        0      805 2024-04-21 05:06:56.403097 rate_control-3.0.0/rate_control/_buckets/_base/_capacity_updating.py
--rw-r--r--   0        0        0      906 2024-04-21 05:06:56.403097 rate_control-3.0.0/rate_control/_buckets/_base/_token_based.py
--rw-r--r--   0        0        0      977 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_buckets/_base/_windowed.py
--rw-r--r--   0        0        0     1034 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_buckets/_fixed_window_counter.py
--rw-r--r--   0        0        0     1372 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_buckets/_leaky_bucket.py
--rw-r--r--   0        0        0      659 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_buckets/_sliding_window_log.py
--rw-r--r--   0        0        0      179 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_controllers/__init__.py
--rw-r--r--   0        0        0     4972 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_controllers/_abc.py
--rw-r--r--   0        0        0     1088 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_controllers/_rate_limiter.py
--rw-r--r--   0        0        0     8773 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_controllers/_scheduler.py
--rw-r--r--   0        0        0      111 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_enums/__init__.py
--rw-r--r--   0        0        0      262 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_enums/_duration.py
--rw-r--r--   0        0        0      350 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_enums/_priority.py
--rw-r--r--   0        0        0      297 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_errors.py
--rw-r--r--   0        0        0      105 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_helpers/__init__.py
--rw-r--r--   0        0        0      781 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_helpers/_mk_repr.py
--rw-r--r--   0        0        0      472 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_helpers/_protocols.py
--rw-r--r--   0        0        0     1502 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_helpers/_request.py
--rw-r--r--   0        0        0     1709 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_helpers/_validation.py
--rw-r--r--   0        0        0        0 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/py.typed
--rw-r--r--   0        0        0      202 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/queues/__init__.py
--rw-r--r--   0        0        0     1540 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/queues/_abc.py
--rw-r--r--   0        0        0     1336 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/queues/_fifo.py
--rw-r--r--   0        0        0     1311 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/queues/_lifo.py
--rw-r--r--   0        0        0     1658 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/queues/_priority.py
--rw-r--r--   0        0        0     5042 1970-01-01 00:00:00.000000 rate_control-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1101 2024-04-27 08:00:53.067565 rate_control-3.0.1/LICENSE
+-rw-r--r--   0        0        0     3822 2024-04-27 08:00:53.067565 rate_control-3.0.1/README.rst
+-rw-r--r--   0        0        0     2872 2024-04-27 08:00:57.195532 rate_control-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0      582 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/__init__.py
+-rw-r--r--   0        0        0     3673 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_bucket_group.py
+-rw-r--r--   0        0        0      267 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_buckets/__init__.py
+-rw-r--r--   0        0        0      344 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_buckets/_base/__init__.py
+-rw-r--r--   0        0        0     2005 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_buckets/_base/_abc.py
+-rw-r--r--   0        0        0     2479 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_buckets/_base/_base_rate.py
+-rw-r--r--   0        0        0      805 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_buckets/_base/_capacity_updating.py
+-rw-r--r--   0        0        0      906 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_buckets/_base/_token_based.py
+-rw-r--r--   0        0        0      977 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_buckets/_base/_windowed.py
+-rw-r--r--   0        0        0     1034 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_buckets/_fixed_window_counter.py
+-rw-r--r--   0        0        0     1372 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_buckets/_leaky_bucket.py
+-rw-r--r--   0        0        0      659 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_buckets/_sliding_window_log.py
+-rw-r--r--   0        0        0      179 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_controllers/__init__.py
+-rw-r--r--   0        0        0     4987 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_controllers/_abc.py
+-rw-r--r--   0        0        0     1121 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_controllers/_rate_limiter.py
+-rw-r--r--   0        0        0     8791 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_controllers/_scheduler.py
+-rw-r--r--   0        0        0      111 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_enums/__init__.py
+-rw-r--r--   0        0        0      262 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_enums/_duration.py
+-rw-r--r--   0        0        0      350 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_enums/_priority.py
+-rw-r--r--   0        0        0      297 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_errors.py
+-rw-r--r--   0        0        0      105 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_helpers/__init__.py
+-rw-r--r--   0        0        0      781 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_helpers/_mk_repr.py
+-rw-r--r--   0        0        0      472 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_helpers/_protocols.py
+-rw-r--r--   0        0        0     1502 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_helpers/_request.py
+-rw-r--r--   0        0        0     1709 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_helpers/_validation.py
+-rw-r--r--   0        0        0        0 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/py.typed
+-rw-r--r--   0        0        0      202 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/queues/__init__.py
+-rw-r--r--   0        0        0     1540 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/queues/_abc.py
+-rw-r--r--   0        0        0     1336 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/queues/_fifo.py
+-rw-r--r--   0        0        0     1311 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/queues/_lifo.py
+-rw-r--r--   0        0        0     1658 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/queues/_priority.py
+-rw-r--r--   0        0        0     5042 1970-01-01 00:00:00.000000 rate_control-3.0.1/PKG-INFO
```

### Comparing `rate_control-3.0.0/LICENSE` & `rate_control-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.0/README.rst` & `rate_control-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.0/pyproject.toml` & `rate_control-3.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rate-control"
-version = "3.0.0"
+version = "3.0.1"
 description = "Versatile rate controlling in Python"
 authors = ["Corentin Régent <corentin.regent.pro@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/corentin-regent/rate-control"
 repository = "https://github.com/corentin-regent/rate-control"
 documentation = "https://rate-control.readthedocs.io/"
```

### Comparing `rate_control-3.0.0/rate_control/__init__.py` & `rate_control-3.0.1/rate_control/__init__.py`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.0/rate_control/_bucket_group.py` & `rate_control-3.0.1/rate_control/_bucket_group.py`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.0/rate_control/_buckets/_base/_abc.py` & `rate_control-3.0.1/rate_control/_buckets/_base/_abc.py`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.0/rate_control/_buckets/_base/_base_rate.py` & `rate_control-3.0.1/rate_control/_buckets/_base/_base_rate.py`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.0/rate_control/_buckets/_base/_capacity_updating.py` & `rate_control-3.0.1/rate_control/_buckets/_base/_capacity_updating.py`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.0/rate_control/_buckets/_base/_token_based.py` & `rate_control-3.0.1/rate_control/_buckets/_base/_token_based.py`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.0/rate_control/_buckets/_base/_windowed.py` & `rate_control-3.0.1/rate_control/_buckets/_base/_windowed.py`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.0/rate_control/_buckets/_fixed_window_counter.py` & `rate_control-3.0.1/rate_control/_buckets/_fixed_window_counter.py`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.0/rate_control/_buckets/_leaky_bucket.py` & `rate_control-3.0.1/rate_control/_buckets/_leaky_bucket.py`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.0/rate_control/_buckets/_sliding_window_log.py` & `rate_control-3.0.1/rate_control/_buckets/_sliding_window_log.py`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.0/rate_control/_controllers/_abc.py` & `rate_control-3.0.1/rate_control/_controllers/_abc.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         Returns:
             Whether a request for the given amount of tokens can be processed instantly.
         """
         return not self._is_concurrency_limited and (self._bucket is None or self._bucket.can_acquire(tokens))
 
     @asynccontextmanager
     @abstractmethod
-    async def request(self, tokens: float = 1) -> AsyncIterator[None]:
+    async def request(self, tokens: float = 1, **kwargs: Any) -> AsyncIterator[None]:
         """Asynchronous context manager that requests the given amount of tokens before the execution.
 
         Args:
             tokens: The number of tokens required for the request.
                 Defaults to `1`.
         """
         yield  # pragma: no cover
```

### Comparing `rate_control-3.0.0/rate_control/_controllers/_rate_limiter.py` & `rate_control-3.0.1/rate_control/_controllers/_rate_limiter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 __all__ = [
     'RateLimiter',
 ]
 
 import sys
 from contextlib import asynccontextmanager
+from typing import Any
 
 from rate_control._controllers._abc import RateController
 
 if sys.version_info >= (3, 9):
     from collections.abc import AsyncIterator
 else:
     from typing import AsyncIterator
@@ -19,15 +20,15 @@
 
 
 class RateLimiter(RateController):
     """Rate controller that raises an error if a request cannot be fulfilled instantly."""
 
     @asynccontextmanager
     @override
-    async def request(self, tokens: float = 1) -> AsyncIterator[None]:
+    async def request(self, tokens: float = 1, **_: Any) -> AsyncIterator[None]:
         """Context manager that acquires the given amount of tokens while holding concurrency.
 
         Args:
             tokens: The number of tokens to acquire.
                 Defaults to `1`.
 
         Raises:
```

### Comparing `rate_control-3.0.0/rate_control/_controllers/_scheduler.py` & `rate_control-3.0.1/rate_control/_controllers/_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,14 +104,15 @@
     @asynccontextmanager
     @override
     async def request(
         self,
         tokens: float = 1,
         priority: Priority = Priority.NORMAL,
         fill_or_kill: bool = False,
+        **_: Any,
     ) -> AsyncIterator[None]:
         """Asynchronous context manager that schedules the execution of the contained statements.
 
         Waits until all the conditions of token availability and allowed concurrency are met,
         before actually consuming tokens and holding a spot for the concurrency.
 
         Args:
```

### Comparing `rate_control-3.0.0/rate_control/_helpers/_mk_repr.py` & `rate_control-3.0.1/rate_control/_helpers/_mk_repr.py`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.0/rate_control/_helpers/_request.py` & `rate_control-3.0.1/rate_control/_helpers/_request.py`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.0/rate_control/_helpers/_validation.py` & `rate_control-3.0.1/rate_control/_helpers/_validation.py`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.0/rate_control/queues/_abc.py` & `rate_control-3.0.1/rate_control/queues/_abc.py`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.0/rate_control/queues/_fifo.py` & `rate_control-3.0.1/rate_control/queues/_fifo.py`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.0/rate_control/queues/_lifo.py` & `rate_control-3.0.1/rate_control/queues/_lifo.py`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.0/rate_control/queues/_priority.py` & `rate_control-3.0.1/rate_control/queues/_priority.py`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.0/PKG-INFO` & `rate_control-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rate-control
-Version: 3.0.0
+Version: 3.0.1
 Summary: Versatile rate controlling in Python
 Home-page: https://github.com/corentin-regent/rate-control
 License: MIT
 Keywords: async,rate limit,schedule,throttle,token bucket
 Author: Corentin Régent
 Author-email: corentin.regent.pro@gmail.com
 Requires-Python: >=3.8,<4.0
```

