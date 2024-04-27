# Comparing `tmp/anycorn-0.17.0.tar.gz` & `tmp/anycorn-0.17.1.tar.gz`

## Comparing `anycorn-0.17.0.tar` & `anycorn-0.17.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 anycorn-0.17.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 anycorn-0.17.0/.readthedocs.yaml
--rw-r--r--   0        0        0    20871 2020-02-02 00:00:00.000000 anycorn-0.17.0/CHANGELOG.rst
--rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 anycorn-0.17.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 anycorn-0.17.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 anycorn-0.17.0/compliance/autobahn/fuzzingclient.json
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 anycorn-0.17.0/compliance/autobahn/summarise.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 anycorn-0.17.0/compliance/autobahn/ws_server.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 anycorn-0.17.0/compliance/h2spec/cert.pem
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 anycorn-0.17.0/compliance/h2spec/http_server.py
--rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 anycorn-0.17.0/compliance/h2spec/key.pem
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/__init__.py
--rw-r--r--   0        0        0    10592 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/__main__.py
--rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/app_wrappers.py
--rw-r--r--   0        0        0    13238 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/config.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/events.py
--rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/lifespan.py
--rw-r--r--   0        0        0     7344 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/logging.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/py.typed
--rw-r--r--   0        0        0     9348 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/run.py
--rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/statsd.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/task_group.py
--rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/tcp_server.py
--rw-r--r--   0        0        0     7128 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/typing.py
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/udp_server.py
--rw-r--r--   0        0        0     6469 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/utils.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/worker_context.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/middleware/__init__.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/middleware/dispatcher.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/middleware/http_to_https.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/middleware/proxy_fix.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/middleware/wsgi.py
--rwxr-xr-x   0        0        0     2769 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/protocol/__init__.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/protocol/events.py
--rwxr-xr-x   0        0        0    11624 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/protocol/h11.py
--rwxr-xr-x   0        0        0    14996 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/protocol/h2.py
--rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/protocol/h3.py
--rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/protocol/http_stream.py
--rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/protocol/quic.py
--rw-r--r--   0        0        0    14902 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/protocol/ws_stream.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/__init__.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/conftest.py
--rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/helpers.py
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/test___main__.py
--rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/test_app_wrappers.py
--rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/test_config.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/test_keep_alive.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/test_lifespan.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/test_logging.py
--rw-r--r--   0        0        0     8390 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/test_sanity.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/test_utils.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/assets/cert.pem
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/assets/config.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/assets/config.toml
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/assets/config_ssl.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/assets/key.pem
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/middleware/__init__.py
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/middleware/test_dispatcher.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/middleware/test_http_to_https.py
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/middleware/test_proxy_fix.py
--rwxr-xr-x   0        0        0    15366 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/protocol/test_h11.py
--rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/protocol/test_h2.py
--rw-r--r--   0        0        0     9873 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/protocol/test_http_stream.py
--rw-r--r--   0        0        0    17121 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/protocol/test_ws_stream.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 anycorn-0.17.0/.gitignore
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 anycorn-0.17.0/LICENSE
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 anycorn-0.17.0/README.md
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 anycorn-0.17.0/pyproject.toml
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 anycorn-0.17.0/PKG-INFO
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 anycorn-0.17.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 anycorn-0.17.1/.readthedocs.yaml
+-rw-r--r--   0        0        0    20871 2020-02-02 00:00:00.000000 anycorn-0.17.1/CHANGELOG.rst
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 anycorn-0.17.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 anycorn-0.17.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 anycorn-0.17.1/compliance/autobahn/fuzzingclient.json
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 anycorn-0.17.1/compliance/autobahn/summarise.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 anycorn-0.17.1/compliance/autobahn/ws_server.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 anycorn-0.17.1/compliance/h2spec/cert.pem
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 anycorn-0.17.1/compliance/h2spec/http_server.py
+-rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 anycorn-0.17.1/compliance/h2spec/key.pem
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/__init__.py
+-rw-r--r--   0        0        0    10592 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/__main__.py
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/app_wrappers.py
+-rw-r--r--   0        0        0    13238 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/config.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/events.py
+-rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/lifespan.py
+-rw-r--r--   0        0        0     7344 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/logging.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/py.typed
+-rw-r--r--   0        0        0     9348 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/run.py
+-rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/statsd.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/task_group.py
+-rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/tcp_server.py
+-rw-r--r--   0        0        0     7128 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/typing.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/udp_server.py
+-rw-r--r--   0        0        0     6469 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/utils.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/worker_context.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/middleware/__init__.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/middleware/dispatcher.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/middleware/http_to_https.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/middleware/proxy_fix.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/middleware/wsgi.py
+-rwxr-xr-x   0        0        0     2769 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/protocol/__init__.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/protocol/events.py
+-rwxr-xr-x   0        0        0    11624 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/protocol/h11.py
+-rwxr-xr-x   0        0        0    14996 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/protocol/h2.py
+-rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/protocol/h3.py
+-rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/protocol/http_stream.py
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/protocol/quic.py
+-rw-r--r--   0        0        0    14902 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/protocol/ws_stream.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/__init__.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/conftest.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/helpers.py
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/test___main__.py
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/test_app_wrappers.py
+-rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/test_config.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/test_keep_alive.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/test_lifespan.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/test_logging.py
+-rw-r--r--   0        0        0     8390 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/test_sanity.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/test_utils.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/assets/cert.pem
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/assets/config.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/assets/config.toml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/assets/config_ssl.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/assets/key.pem
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/middleware/__init__.py
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/middleware/test_dispatcher.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/middleware/test_http_to_https.py
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/middleware/test_proxy_fix.py
+-rwxr-xr-x   0        0        0    15366 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/protocol/test_h11.py
+-rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/protocol/test_h2.py
+-rw-r--r--   0        0        0     9873 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/protocol/test_http_stream.py
+-rw-r--r--   0        0        0    17121 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/protocol/test_ws_stream.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 anycorn-0.17.1/.gitignore
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 anycorn-0.17.1/LICENSE
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 anycorn-0.17.1/README.md
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 anycorn-0.17.1/pyproject.toml
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 anycorn-0.17.1/PKG-INFO
```

### Comparing `anycorn-0.17.0/.pre-commit-config.yaml` & `anycorn-0.17.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/CHANGELOG.rst` & `anycorn-0.17.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/.github/workflows/ci.yml` & `anycorn-0.17.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/.github/workflows/publish.yml` & `anycorn-0.17.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/compliance/autobahn/ws_server.py` & `anycorn-0.17.1/compliance/autobahn/ws_server.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/compliance/h2spec/cert.pem` & `anycorn-0.17.1/compliance/h2spec/cert.pem`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/compliance/h2spec/http_server.py` & `anycorn-0.17.1/compliance/h2spec/http_server.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/compliance/h2spec/key.pem` & `anycorn-0.17.1/compliance/h2spec/key.pem`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/__init__.py` & `anycorn-0.17.1/src/anycorn/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from .config import Config
 from .run import worker_serve
 from .typing import Framework
 from .utils import wrap_app
 
 __all__ = ("Config", "serve")
-__version__ = "0.17.0"
+__version__ = "0.17.1"
 
 
 async def serve(
     app: Framework,
     config: Config,
     *,
     shutdown_trigger: Callable[..., Awaitable[None]] | None = None,
```

### Comparing `anycorn-0.17.0/src/anycorn/__main__.py` & `anycorn-0.17.1/src/anycorn/__main__.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/app_wrappers.py` & `anycorn-0.17.1/src/anycorn/app_wrappers.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/config.py` & `anycorn-0.17.1/src/anycorn/config.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/lifespan.py` & `anycorn-0.17.1/src/anycorn/lifespan.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/logging.py` & `anycorn-0.17.1/src/anycorn/logging.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/run.py` & `anycorn-0.17.1/src/anycorn/run.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/statsd.py` & `anycorn-0.17.1/src/anycorn/statsd.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/task_group.py` & `anycorn-0.17.1/src/anycorn/task_group.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/tcp_server.py` & `anycorn-0.17.1/src/anycorn/tcp_server.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/typing.py` & `anycorn-0.17.1/src/anycorn/typing.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/udp_server.py` & `anycorn-0.17.1/src/anycorn/udp_server.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/utils.py` & `anycorn-0.17.1/src/anycorn/utils.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/worker_context.py` & `anycorn-0.17.1/src/anycorn/worker_context.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/middleware/dispatcher.py` & `anycorn-0.17.1/src/anycorn/middleware/dispatcher.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/middleware/http_to_https.py` & `anycorn-0.17.1/src/anycorn/middleware/http_to_https.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/middleware/proxy_fix.py` & `anycorn-0.17.1/src/anycorn/middleware/proxy_fix.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/middleware/wsgi.py` & `anycorn-0.17.1/src/anycorn/middleware/wsgi.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/protocol/__init__.py` & `anycorn-0.17.1/src/anycorn/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/protocol/events.py` & `anycorn-0.17.1/src/anycorn/protocol/events.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/protocol/h11.py` & `anycorn-0.17.1/src/anycorn/protocol/h11.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/protocol/h2.py` & `anycorn-0.17.1/src/anycorn/protocol/h2.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/protocol/h3.py` & `anycorn-0.17.1/src/anycorn/protocol/h3.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/protocol/http_stream.py` & `anycorn-0.17.1/src/anycorn/protocol/http_stream.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/protocol/quic.py` & `anycorn-0.17.1/src/anycorn/protocol/quic.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/src/anycorn/protocol/ws_stream.py` & `anycorn-0.17.1/src/anycorn/protocol/ws_stream.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/tests/conftest.py` & `anycorn-0.17.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/tests/helpers.py` & `anycorn-0.17.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/tests/test___main__.py` & `anycorn-0.17.1/tests/test___main__.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/tests/test_app_wrappers.py` & `anycorn-0.17.1/tests/test_app_wrappers.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/tests/test_config.py` & `anycorn-0.17.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/tests/test_keep_alive.py` & `anycorn-0.17.1/tests/test_keep_alive.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/tests/test_lifespan.py` & `anycorn-0.17.1/tests/test_lifespan.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/tests/test_logging.py` & `anycorn-0.17.1/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/tests/test_sanity.py` & `anycorn-0.17.1/tests/test_sanity.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/tests/test_utils.py` & `anycorn-0.17.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/tests/assets/cert.pem` & `anycorn-0.17.1/tests/assets/cert.pem`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/tests/assets/key.pem` & `anycorn-0.17.1/tests/assets/key.pem`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/tests/middleware/test_dispatcher.py` & `anycorn-0.17.1/tests/middleware/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/tests/middleware/test_http_to_https.py` & `anycorn-0.17.1/tests/middleware/test_http_to_https.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/tests/middleware/test_proxy_fix.py` & `anycorn-0.17.1/tests/middleware/test_proxy_fix.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/tests/protocol/test_h11.py` & `anycorn-0.17.1/tests/protocol/test_h11.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/tests/protocol/test_h2.py` & `anycorn-0.17.1/tests/protocol/test_h2.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/tests/protocol/test_http_stream.py` & `anycorn-0.17.1/tests/protocol/test_http_stream.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/tests/protocol/test_ws_stream.py` & `anycorn-0.17.1/tests/protocol/test_ws_stream.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/LICENSE` & `anycorn-0.17.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/README.md` & `anycorn-0.17.1/README.md`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.0/pyproject.toml` & `anycorn-0.17.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
 dependencies = [
     "exceptiongroup >= 1.2.0, <2.0; python_version<'3.11'",
     "h11",
     "h2 >=3.1.0",
     "anyio >=4.0, <5.0",
     "priority",
-    "taskgroup >=0.0.0a4; python_version<'3.11'",
     "tomli; python_version<'3.11'",
     "wsproto >=0.14.0",
 ]
 
 [project.optional-dependencies]
 h3 = [
     "aioquic >= 0.9.0, < 1.0",
```

### Comparing `anycorn-0.17.0/PKG-INFO` & `anycorn-0.17.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: anycorn
-Version: 0.17.0
+Version: 0.17.1
 Summary: A fork of Hypercorn that uses AnyIO
 Author-email: Philip Graham Jones <philip.graham.jones@googlemail.com>, David Brochart <david.brochart@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,14 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Requires-Dist: anyio<5.0,>=4.0
 Requires-Dist: exceptiongroup<2.0,>=1.2.0; python_version < '3.11'
 Requires-Dist: h11
 Requires-Dist: h2>=3.1.0
 Requires-Dist: priority
-Requires-Dist: taskgroup>=0.0.0a4; python_version < '3.11'
 Requires-Dist: tomli; python_version < '3.11'
 Requires-Dist: wsproto>=0.14.0
 Provides-Extra: h3
 Requires-Dist: aioquic<1.0,>=0.9.0; extra == 'h3'
 Provides-Extra: test
 Requires-Dist: mock; extra == 'test'
 Requires-Dist: mypy; extra == 'test'
```

