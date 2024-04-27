# Comparing `tmp/tremolo-0.0.504.tar.gz` & `tmp/tremolo-0.0.505.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/tux/tremolo/dist/.tmp-3of1j8yj/tremolo-0.0.504.tar", last modified: Thu Apr 11 07:59:52 2024, max compression
+gzip compressed data, was "/home/tux/tremolo/dist/.tmp-aqsy59ri/tremolo-0.0.505.tar", last modified: Sat Apr 27 01:17:23 2024, max compression
```

## Comparing `tremolo-0.0.504.tar` & `tremolo-0.0.505.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-11 07:59:52.000000 tremolo-0.0.504/
--rw-r--r--   0 tux       (1000) users      (100)     1063 2024-02-01 14:00:19.000000 tremolo-0.0.504/LICENSE.txt
--rw-r--r--   0 tux       (1000) users      (100)       63 2024-03-16 12:09:02.000000 tremolo-0.0.504/MANIFEST.in
--rw-r--r--   0 tux       (1000) users      (100)     6473 2024-04-11 07:59:52.000000 tremolo-0.0.504/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)     5683 2024-02-01 14:00:19.000000 tremolo-0.0.504/README.md
--rw-r--r--   0 tux       (1000) users      (100)     1016 2024-03-16 12:09:02.000000 tremolo-0.0.504/pyproject.toml
--rw-r--r--   0 tux       (1000) users      (100)       38 2024-04-11 07:59:52.000000 tremolo-0.0.504/setup.cfg
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-11 07:59:52.000000 tremolo-0.0.504/tremolo/
--rw-r--r--   0 tux       (1000) users      (100)      308 2024-04-11 07:58:51.000000 tremolo-0.0.504/tremolo/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)     7213 2024-02-05 09:58:51.000000 tremolo-0.0.504/tremolo/__main__.py
--rw-r--r--   0 tux       (1000) users      (100)     2674 2024-02-20 23:07:43.000000 tremolo-0.0.504/tremolo/asgi_lifespan.py
--rw-r--r--   0 tux       (1000) users      (100)     9917 2024-04-11 02:23:44.000000 tremolo-0.0.504/tremolo/asgi_server.py
--rw-r--r--   0 tux       (1000) users      (100)      681 2024-02-01 14:00:19.000000 tremolo-0.0.504/tremolo/exceptions.py
--rw-r--r--   0 tux       (1000) users      (100)     1139 2024-02-01 14:00:19.000000 tremolo-0.0.504/tremolo/handlers.py
--rw-r--r--   0 tux       (1000) users      (100)    11708 2024-03-27 21:22:49.000000 tremolo-0.0.504/tremolo/http_server.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-11 07:59:52.000000 tremolo-0.0.504/tremolo/lib/
--rw-r--r--   0 tux       (1000) users      (100)        0 2024-02-01 14:00:19.000000 tremolo-0.0.504/tremolo/lib/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)      603 2024-02-01 14:00:19.000000 tremolo-0.0.504/tremolo/lib/connections.py
--rw-r--r--   0 tux       (1000) users      (100)      671 2024-02-05 09:57:05.000000 tremolo-0.0.504/tremolo/lib/contexts.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-11 07:59:52.000000 tremolo-0.0.504/tremolo/lib/h1parser/
--rw-r--r--   0 tux       (1000) users      (100)       52 2024-02-01 14:00:19.000000 tremolo-0.0.504/tremolo/lib/h1parser/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)     6075 2024-04-11 07:58:51.000000 tremolo-0.0.504/tremolo/lib/h1parser/parse_header.py
--rw-r--r--   0 tux       (1000) users      (100)     2084 2024-02-01 14:00:19.000000 tremolo-0.0.504/tremolo/lib/http_exception.py
--rw-r--r--   0 tux       (1000) users      (100)    18457 2024-04-11 07:58:51.000000 tremolo-0.0.504/tremolo/lib/http_protocol.py
--rw-r--r--   0 tux       (1000) users      (100)    12797 2024-03-08 01:51:43.000000 tremolo-0.0.504/tremolo/lib/http_request.py
--rw-r--r--   0 tux       (1000) users      (100)    15760 2024-04-04 21:42:22.000000 tremolo-0.0.504/tremolo/lib/http_response.py
--rw-r--r--   0 tux       (1000) users      (100)     1896 2024-02-01 14:00:19.000000 tremolo-0.0.504/tremolo/lib/locks.py
--rw-r--r--   0 tux       (1000) users      (100)      919 2024-03-05 03:41:31.000000 tremolo-0.0.504/tremolo/lib/pools.py
--rw-r--r--   0 tux       (1000) users      (100)     1170 2024-02-25 01:31:07.000000 tremolo-0.0.504/tremolo/lib/queue.py
--rw-r--r--   0 tux       (1000) users      (100)     1199 2024-03-08 01:52:01.000000 tremolo-0.0.504/tremolo/lib/request.py
--rw-r--r--   0 tux       (1000) users      (100)     1460 2024-04-01 02:53:44.000000 tremolo-0.0.504/tremolo/lib/response.py
--rw-r--r--   0 tux       (1000) users      (100)      534 2024-02-01 14:00:19.000000 tremolo-0.0.504/tremolo/lib/tasks.py
--rw-r--r--   0 tux       (1000) users      (100)     6064 2024-02-01 14:00:19.000000 tremolo-0.0.504/tremolo/lib/websocket.py
--rw-r--r--   0 tux       (1000) users      (100)    28028 2024-04-04 22:17:18.000000 tremolo-0.0.504/tremolo/tremolo.py
--rw-r--r--   0 tux       (1000) users      (100)     1095 2024-04-04 21:42:22.000000 tremolo-0.0.504/tremolo/utils.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-11 07:59:52.000000 tremolo-0.0.504/tremolo.egg-info/
--rw-r--r--   0 tux       (1000) users      (100)     6473 2024-04-11 07:59:52.000000 tremolo-0.0.504/tremolo.egg-info/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)      778 2024-04-11 07:59:52.000000 tremolo-0.0.504/tremolo.egg-info/SOURCES.txt
--rw-r--r--   0 tux       (1000) users      (100)        1 2024-04-11 07:59:52.000000 tremolo-0.0.504/tremolo.egg-info/dependency_links.txt
--rw-r--r--   0 tux       (1000) users      (100)        8 2024-04-11 07:59:52.000000 tremolo-0.0.504/tremolo.egg-info/top_level.txt
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-27 01:17:23.000000 tremolo-0.0.505/
+-rw-r--r--   0 tux       (1000) users      (100)     1063 2024-02-01 14:00:19.000000 tremolo-0.0.505/LICENSE.txt
+-rw-r--r--   0 tux       (1000) users      (100)       63 2024-03-16 12:09:02.000000 tremolo-0.0.505/MANIFEST.in
+-rw-r--r--   0 tux       (1000) users      (100)     6473 2024-04-27 01:17:23.000000 tremolo-0.0.505/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)     5683 2024-02-01 14:00:19.000000 tremolo-0.0.505/README.md
+-rw-r--r--   0 tux       (1000) users      (100)     1016 2024-03-16 12:09:02.000000 tremolo-0.0.505/pyproject.toml
+-rw-r--r--   0 tux       (1000) users      (100)       38 2024-04-27 01:17:23.000000 tremolo-0.0.505/setup.cfg
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-27 01:17:23.000000 tremolo-0.0.505/tremolo/
+-rw-r--r--   0 tux       (1000) users      (100)      308 2024-04-27 01:16:14.000000 tremolo-0.0.505/tremolo/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)     7213 2024-02-05 09:58:51.000000 tremolo-0.0.505/tremolo/__main__.py
+-rw-r--r--   0 tux       (1000) users      (100)     2674 2024-02-20 23:07:43.000000 tremolo-0.0.505/tremolo/asgi_lifespan.py
+-rw-r--r--   0 tux       (1000) users      (100)     9921 2024-04-26 23:42:43.000000 tremolo-0.0.505/tremolo/asgi_server.py
+-rw-r--r--   0 tux       (1000) users      (100)      681 2024-02-01 14:00:19.000000 tremolo-0.0.505/tremolo/exceptions.py
+-rw-r--r--   0 tux       (1000) users      (100)     1139 2024-02-01 14:00:19.000000 tremolo-0.0.505/tremolo/handlers.py
+-rw-r--r--   0 tux       (1000) users      (100)    11708 2024-03-27 21:22:49.000000 tremolo-0.0.505/tremolo/http_server.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-27 01:17:23.000000 tremolo-0.0.505/tremolo/lib/
+-rw-r--r--   0 tux       (1000) users      (100)        0 2024-02-01 14:00:19.000000 tremolo-0.0.505/tremolo/lib/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)      603 2024-02-01 14:00:19.000000 tremolo-0.0.505/tremolo/lib/connections.py
+-rw-r--r--   0 tux       (1000) users      (100)      671 2024-02-05 09:57:05.000000 tremolo-0.0.505/tremolo/lib/contexts.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-27 01:17:23.000000 tremolo-0.0.505/tremolo/lib/h1parser/
+-rw-r--r--   0 tux       (1000) users      (100)       52 2024-02-01 14:00:19.000000 tremolo-0.0.505/tremolo/lib/h1parser/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)     6075 2024-04-11 07:58:51.000000 tremolo-0.0.505/tremolo/lib/h1parser/parse_header.py
+-rw-r--r--   0 tux       (1000) users      (100)     2084 2024-02-01 14:00:19.000000 tremolo-0.0.505/tremolo/lib/http_exception.py
+-rw-r--r--   0 tux       (1000) users      (100)    18427 2024-04-26 23:47:45.000000 tremolo-0.0.505/tremolo/lib/http_protocol.py
+-rw-r--r--   0 tux       (1000) users      (100)    13054 2024-04-27 01:01:06.000000 tremolo-0.0.505/tremolo/lib/http_request.py
+-rw-r--r--   0 tux       (1000) users      (100)    15760 2024-04-04 21:42:22.000000 tremolo-0.0.505/tremolo/lib/http_response.py
+-rw-r--r--   0 tux       (1000) users      (100)     1896 2024-02-01 14:00:19.000000 tremolo-0.0.505/tremolo/lib/locks.py
+-rw-r--r--   0 tux       (1000) users      (100)      919 2024-03-05 03:41:31.000000 tremolo-0.0.505/tremolo/lib/pools.py
+-rw-r--r--   0 tux       (1000) users      (100)     1170 2024-02-25 01:31:07.000000 tremolo-0.0.505/tremolo/lib/queue.py
+-rw-r--r--   0 tux       (1000) users      (100)     1322 2024-04-26 23:08:31.000000 tremolo-0.0.505/tremolo/lib/request.py
+-rw-r--r--   0 tux       (1000) users      (100)     1460 2024-04-01 02:53:44.000000 tremolo-0.0.505/tremolo/lib/response.py
+-rw-r--r--   0 tux       (1000) users      (100)      534 2024-02-01 14:00:19.000000 tremolo-0.0.505/tremolo/lib/tasks.py
+-rw-r--r--   0 tux       (1000) users      (100)     6064 2024-02-01 14:00:19.000000 tremolo-0.0.505/tremolo/lib/websocket.py
+-rw-r--r--   0 tux       (1000) users      (100)    28028 2024-04-04 22:17:18.000000 tremolo-0.0.505/tremolo/tremolo.py
+-rw-r--r--   0 tux       (1000) users      (100)     1095 2024-04-04 21:42:22.000000 tremolo-0.0.505/tremolo/utils.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-27 01:17:23.000000 tremolo-0.0.505/tremolo.egg-info/
+-rw-r--r--   0 tux       (1000) users      (100)     6473 2024-04-27 01:17:23.000000 tremolo-0.0.505/tremolo.egg-info/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)      778 2024-04-27 01:17:23.000000 tremolo-0.0.505/tremolo.egg-info/SOURCES.txt
+-rw-r--r--   0 tux       (1000) users      (100)        1 2024-04-27 01:17:23.000000 tremolo-0.0.505/tremolo.egg-info/dependency_links.txt
+-rw-r--r--   0 tux       (1000) users      (100)        8 2024-04-27 01:17:23.000000 tremolo-0.0.505/tremolo.egg-info/top_level.txt
```

### Comparing `tremolo-0.0.504/LICENSE.txt` & `tremolo-0.0.505/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.504/PKG-INFO` & `tremolo-0.0.505/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.504
+Version: 0.0.505
 Summary: Tremolo is a stream-oriented, asynchronous, programmable HTTP server written in pure Python. It can also serve as an ASGI server.
 Author-email: nggit <contact@anggit.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/nggit/tremolo
 Project-URL: Source, https://github.com/nggit/tremolo
 Project-URL: Funding, https://github.com/sponsors/nggit
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tremolo-0.0.504/README.md` & `tremolo-0.0.505/README.md`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.504/pyproject.toml` & `tremolo-0.0.505/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.504/tremolo/__main__.py` & `tremolo-0.0.505/tremolo/__main__.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.504/tremolo/asgi_lifespan.py` & `tremolo-0.0.505/tremolo/asgi_lifespan.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.504/tremolo/asgi_server.py` & `tremolo-0.0.505/tremolo/asgi_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
             data = await self._read.__anext__()
 
             return {
                 'type': 'http.request',
                 'body': data,
                 'more_body': (
                     (data != b'' and self.request.content_length == -1) or
-                    self.request.body_size < self.request.content_length
+                    self.request.body_consumed < self.request.content_length
                 )
             }
         except (asyncio.CancelledError, Exception) as exc:
             if not (self._read is None or self.request is None or
                     isinstance(exc, StopAsyncIteration)):
                 self.print_exception(exc)
```

### Comparing `tremolo-0.0.504/tremolo/exceptions.py` & `tremolo-0.0.505/tremolo/exceptions.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.504/tremolo/handlers.py` & `tremolo-0.0.505/tremolo/handlers.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.504/tremolo/http_server.py` & `tremolo-0.0.505/tremolo/http_server.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.504/tremolo/lib/connections.py` & `tremolo-0.0.505/tremolo/lib/connections.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.504/tremolo/lib/contexts.py` & `tremolo-0.0.505/tremolo/lib/contexts.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.504/tremolo/lib/h1parser/parse_header.py` & `tremolo-0.0.505/tremolo/lib/h1parser/parse_header.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.504/tremolo/lib/http_exception.py` & `tremolo-0.0.505/tremolo/lib/http_exception.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.504/tremolo/lib/http_protocol.py` & `tremolo-0.0.505/tremolo/lib/http_protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,14 @@
             self,
             data,
             queue=None,
             transport=None,
             rate=1048576,
             buffer_size=16 * 1024
             ):
-        data_size = len(data)
         mv = memoryview(data)
 
         while mv and queue is not None:
             queue.put_nowait(mv[:buffer_size].tobytes())
             queue_size = queue.qsize()
 
             if queue_size > self.options['max_queue_size']:
@@ -131,15 +130,15 @@
             mv = mv[buffer_size:]
 
         if transport is not None and self.request is not None:
             if self.request.upgraded:
                 transport.resume_reading()
                 return
 
-            self.request.body_size += data_size
+            self.request.body_size += len(data)
 
             if (b'content-length' in self.request.headers and
                     self.request.body_size >= self.request.content_length and
                     queue is not None):
                 queue.put_nowait(None)
             elif self.request.body_size < self.options['client_max_body_size']:
                 transport.resume_reading()
```

### Comparing `tremolo-0.0.504/tremolo/lib/http_request.py` & `tremolo-0.0.505/tremolo/lib/http_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,18 +143,15 @@
 
     async def body(self, raw=False):
         async for data in self.stream(raw=raw):
             self._body.extend(data)
 
         return self._body
 
-    def read(self, size=None):
-        if size is None:
-            return self.stream()
-
+    def read(self, size=-1):
         return self.recv(size=size, raw=False)
 
     def eof(self):
         return self._eof and self._read_buf == b''
 
     async def recv(self, size=-1, raw=True):
         if size == 0 or self.eof():
@@ -246,15 +243,20 @@
                         del buf[:chunk_size + i + 4]
         else:
             if (self.content_length >
                     self.protocol.options['client_max_body_size']):
                 raise PayloadTooLarge
 
             async for data in super().recv():
-                yield data
+                if -1 < self.content_length < self.body_consumed:
+                    # pipelining is not yet supported on a request with a body
+                    self.protocol.logger.info('Content-Length mismatch')
+                    yield data[:self.content_length - self.body_consumed]
+                else:
+                    yield data
 
         self._eof = True
 
     @property
     def upgraded(self):
         return self._upgraded
```

### Comparing `tremolo-0.0.504/tremolo/lib/http_response.py` & `tremolo-0.0.505/tremolo/lib/http_response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.504/tremolo/lib/locks.py` & `tremolo-0.0.505/tremolo/lib/locks.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.504/tremolo/lib/pools.py` & `tremolo-0.0.505/tremolo/lib/pools.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.504/tremolo/lib/queue.py` & `tremolo-0.0.505/tremolo/lib/queue.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.504/tremolo/lib/request.py` & `tremolo-0.0.505/tremolo/lib/request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Copyright (c) 2023 nggit
 
 import asyncio
 
 
 class Request:
-    __slots__ = ('protocol', 'body_size')
+    __slots__ = ('protocol', 'body_size', 'body_consumed')
 
     def __init__(self, protocol):
         self.protocol = protocol
         self.body_size = 0
+        self.body_consumed = 0
 
     @property
     def context(self):
         return self.protocol.context
 
     @property
     def ctx(self):
@@ -20,14 +21,15 @@
 
     @property
     def transport(self):
         return self.protocol.transport
 
     def clear_body(self):
         self.body_size = 0
+        self.body_consumed = 0
 
     async def recv(self):
         while self.protocol.queue[0] is not None:
             task = self.protocol.loop.create_task(
                 self.protocol.queue[0].get()
             )
             timer = self.protocol.loop.call_at(
@@ -44,8 +46,9 @@
                 raise TimeoutError('recv timeout') from exc
             finally:
                 timer.cancel()
 
             if data is None:
                 break
 
+            self.body_consumed += len(data)
             yield data
```

### Comparing `tremolo-0.0.504/tremolo/lib/response.py` & `tremolo-0.0.505/tremolo/lib/response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.504/tremolo/lib/tasks.py` & `tremolo-0.0.505/tremolo/lib/tasks.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.504/tremolo/lib/websocket.py` & `tremolo-0.0.505/tremolo/lib/websocket.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.504/tremolo/tremolo.py` & `tremolo-0.0.505/tremolo/tremolo.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.504/tremolo/utils.py` & `tremolo-0.0.505/tremolo/utils.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.504/tremolo.egg-info/PKG-INFO` & `tremolo-0.0.505/tremolo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.504
+Version: 0.0.505
 Summary: Tremolo is a stream-oriented, asynchronous, programmable HTTP server written in pure Python. It can also serve as an ASGI server.
 Author-email: nggit <contact@anggit.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/nggit/tremolo
 Project-URL: Source, https://github.com/nggit/tremolo
 Project-URL: Funding, https://github.com/sponsors/nggit
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tremolo-0.0.504/tremolo.egg-info/SOURCES.txt` & `tremolo-0.0.505/tremolo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

