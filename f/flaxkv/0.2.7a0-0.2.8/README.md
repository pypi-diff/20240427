# Comparing `tmp/flaxkv-0.2.7a0.tar.gz` & `tmp/flaxkv-0.2.8.tar.gz`

## Comparing `flaxkv-0.2.7a0.tar` & `flaxkv-0.2.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 flaxkv-0.2.7a0/flaxkv/__init__.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 flaxkv-0.2.7a0/flaxkv/__main__.py
--rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 flaxkv-0.2.7a0/flaxkv/_sqlite.py
--rw-r--r--   0        0        0    37792 2020-02-02 00:00:00.000000 flaxkv-0.2.7a0/flaxkv/core.py
--rw-r--r--   0        0        0     3471 2020-02-02 00:00:00.000000 flaxkv-0.2.7a0/flaxkv/decorators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flaxkv-0.2.7a0/flaxkv/exceptions.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 flaxkv-0.2.7a0/flaxkv/helper.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 flaxkv-0.2.7a0/flaxkv/log.py
--rw-r--r--   0        0        0    11823 2020-02-02 00:00:00.000000 flaxkv-0.2.7a0/flaxkv/manager.py
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 flaxkv-0.2.7a0/flaxkv/pack.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 flaxkv-0.2.7a0/flaxkv/serve/__init__.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 flaxkv-0.2.7a0/flaxkv/serve/app.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 flaxkv-0.2.7a0/flaxkv/serve/interface.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 flaxkv-0.2.7a0/flaxkv/serve/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flaxkv-0.2.7a0/flaxkv/serve/pub_sub.py
--rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 flaxkv-0.2.7a0/flaxkv/serve/route.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 flaxkv-0.2.7a0/.gitignore
--rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 flaxkv-0.2.7a0/LICENSE
--rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 flaxkv-0.2.7a0/README.md
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 flaxkv-0.2.7a0/pyproject.toml
--rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 flaxkv-0.2.7a0/PKG-INFO
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 flaxkv-0.2.8/flaxkv/__init__.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 flaxkv-0.2.8/flaxkv/__main__.py
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 flaxkv-0.2.8/flaxkv/_sqlite.py
+-rw-r--r--   0        0        0    38876 2020-02-02 00:00:00.000000 flaxkv-0.2.8/flaxkv/core.py
+-rw-r--r--   0        0        0     3471 2020-02-02 00:00:00.000000 flaxkv-0.2.8/flaxkv/decorators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flaxkv-0.2.8/flaxkv/exceptions.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 flaxkv-0.2.8/flaxkv/helper.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 flaxkv-0.2.8/flaxkv/log.py
+-rw-r--r--   0        0        0    11909 2020-02-02 00:00:00.000000 flaxkv-0.2.8/flaxkv/manager.py
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 flaxkv-0.2.8/flaxkv/pack.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 flaxkv-0.2.8/flaxkv/serve/__init__.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 flaxkv-0.2.8/flaxkv/serve/app.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 flaxkv-0.2.8/flaxkv/serve/interface.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 flaxkv-0.2.8/flaxkv/serve/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flaxkv-0.2.8/flaxkv/serve/pub_sub.py
+-rw-r--r--   0        0        0    12199 2020-02-02 00:00:00.000000 flaxkv-0.2.8/flaxkv/serve/route.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 flaxkv-0.2.8/.gitignore
+-rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 flaxkv-0.2.8/LICENSE
+-rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 flaxkv-0.2.8/README.md
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 flaxkv-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 flaxkv-0.2.8/PKG-INFO
```

### Comparing `flaxkv-0.2.7a0/flaxkv/__init__.py` & `flaxkv-0.2.8/flaxkv/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 
 from __future__ import annotations
 
 import re
 
 from .core import LevelDBDict, LMDBDict, RemoteDBDict
 
-__version__ = "0.2.7-alpha"
+__version__ = "0.2.8"
 
 __all__ = [
     "FlaxKV",
+    "Flaxkv",
     "dbdict",
     "dictdb",
     "LMDBDict",
     "LevelDBDict",
     "RemoteDBDict",
 ]
 
@@ -75,7 +76,8 @@
 
     else:
         raise ValueError(f"Unsupported DB type {backend}.")
 
 
 dbdict = FlaxKV
 dictdb = FlaxKV
+Flaxkv = FlaxKV
```

### Comparing `flaxkv-0.2.7a0/flaxkv/__main__.py` & `flaxkv-0.2.8/flaxkv/__main__.py`

 * *Files identical despite different names*

### Comparing `flaxkv-0.2.7a0/flaxkv/_sqlite.py` & `flaxkv-0.2.8/flaxkv/_sqlite.py`

 * *Files identical despite different names*

### Comparing `flaxkv-0.2.7a0/flaxkv/core.py` & `flaxkv-0.2.8/flaxkv/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -406,14 +406,25 @@
         self._last_set_time = time.time()
         # Trigger immediate write if buffer size exceeds MAX_BUFFER_SIZE
         if self._buffered_count >= self.MAX_BUFFER_SIZE:
             self._logger.debug("Trigger immediate write")
             self._buffered_count = 0
             self.write_immediately()
 
+    def from_dict(self, d: dict, clear=False):
+        """
+        Updates the buffer with the given dictionary.
+
+        Args:
+            d (dict): A dictionary of key-value pairs to update.
+        """
+        if clear:
+            self.clear(wait=True)
+        self.update(d)
+
     # @class_measure_time()
     def _write_buffer_to_db(
         self,
         current_write_num: int,
     ):
         """
         Writes the current buffer to the database.
@@ -827,31 +838,41 @@
     """
     A dictionary-like class that stores key-value pairs in an LMDB database.
     Type:
         key: int, float, bool, str, tuple
         value: int, float, bool, str, list, dict, and np.ndarray,
     """
 
+    _instances = {}
+
+    def __new__(cls, db_name: str, root_path: str, rebuild=False, **kwargs):
+        name = db_name + str(root_path)
+        if name not in cls._instances:
+            cls._instances[name] = super().__new__(cls)
+        return cls._instances[name]
+
     def __init__(
         self,
         db_name: str,
         root_path: str = './',
         map_size=1024**3,
         rebuild=False,
         **kwargs,
     ):
-        super().__init__(
-            "lmdb",
-            root_path,
-            db_name,
-            max_dbs=1,
-            map_size=map_size,
-            rebuild=rebuild,
-            **kwargs,
-        )
+        if not hasattr(self, '_initialized'):
+            super().__init__(
+                "lmdb",
+                root_path,
+                db_name,
+                max_dbs=1,
+                map_size=map_size,
+                rebuild=rebuild,
+                **kwargs,
+            )
+            self._initialized = True
 
     def _iter_db_view(self, view, include_key=True, include_value=True):
         """
         Iterates over the items in the database view.
 
         Args:
             view: The database view to iterate over.
@@ -895,22 +916,33 @@
     """
     A dictionary-like class that stores key-value pairs in a LevelDB database.
     Type:
         key: int, float, bool, str, tuple
         value: int, float, bool, str, list, dict and np.ndarray,
     """
 
+    _instances = {}
+
+    def __new__(cls, db_name: str, root_path: str, rebuild=False, **kwargs):
+        name = db_name + str(root_path)
+        if name not in cls._instances:
+            cls._instances[name] = super().__new__(cls)
+        return cls._instances[name]
+
     def __init__(self, db_name: str, root_path: str, rebuild=False, **kwargs):
-        super().__init__(
-            "leveldb",
-            root_path_or_url=root_path,
-            db_name=db_name,
-            rebuild=rebuild,
-            **kwargs,
-        )
+        if not hasattr(self, '_initialized'):
+            super().__init__(
+                "leveldb",
+                root_path_or_url=root_path,
+                db_name=db_name,
+                rebuild=rebuild,
+                **kwargs,
+            )
+
+            self._initialized = True
 
     def _iter_db_view(self, view, include_key=True, include_value=True):
         """
         Iterates over the items in the database view.
 
         Args:
             view: The database view to iterate over.
```

### Comparing `flaxkv-0.2.7a0/flaxkv/decorators.py` & `flaxkv-0.2.8/flaxkv/decorators.py`

 * *Files identical despite different names*

### Comparing `flaxkv-0.2.7a0/flaxkv/helper.py` & `flaxkv-0.2.8/flaxkv/helper.py`

 * *Files identical despite different names*

### Comparing `flaxkv-0.2.7a0/flaxkv/log.py` & `flaxkv-0.2.8/flaxkv/log.py`

 * *Files identical despite different names*

### Comparing `flaxkv-0.2.7a0/flaxkv/manager.py` & `flaxkv-0.2.8/flaxkv/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,23 +19,30 @@
 import os
 import re
 import shutil
 import threading
 import time
 import traceback
 from pathlib import Path
+from typing import Dict, Literal
 from uuid import uuid4
 
 import msgspec
 from loguru import logger
 
 from .decorators import retry
 from .pack import decode, decode_key, encode
 
 
+class StructUpdateData(msgspec.Struct):
+    type: str
+    data: Dict[bytes, bytes]
+    time: float
+
+
 class DBManager:
     def __init__(
         self, db_type: str, root_path_or_url: str, db_name: str, rebuild=False, **kwargs
     ):
         """
         Initializes the database manager.
 
@@ -234,15 +241,14 @@
 
     @retry(
         max_retries=3,
         delay=0.2,
         backoff=2,
     )
     def attach_db(self, event: threading.Event):
-        from .serve.interface import StructUpdateData
 
         with self.client.stream(
             "POST",
             f"/connect",
             json={
                 "db_name": self.db_name,
                 "backend": self._backend,
```

### Comparing `flaxkv-0.2.7a0/flaxkv/pack.py` & `flaxkv-0.2.8/flaxkv/pack.py`

 * *Files identical despite different names*

### Comparing `flaxkv-0.2.7a0/flaxkv/serve/__init__.py` & `flaxkv-0.2.8/flaxkv/serve/__init__.py`

 * *Files identical despite different names*

### Comparing `flaxkv-0.2.7a0/flaxkv/serve/app.py` & `flaxkv-0.2.8/flaxkv/serve/app.py`

 * *Files identical despite different names*

### Comparing `flaxkv-0.2.7a0/flaxkv/serve/interface.py` & `flaxkv-0.2.8/flaxkv/serve/interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,13 +51,7 @@
     keys: List[bytes]
 
 
 class StructDeleteBatchData(msgspec.Struct):
     keys: List[bytes]
     client_id: str
     time: float
-
-
-class StructUpdateData(msgspec.Struct):
-    type: str
-    data: Dict[bytes, bytes]
-    time: float
```

### Comparing `flaxkv-0.2.7a0/flaxkv/serve/manager.py` & `flaxkv-0.2.8/flaxkv/serve/manager.py`

 * *Files identical despite different names*

### Comparing `flaxkv-0.2.7a0/flaxkv/serve/route.py` & `flaxkv-0.2.8/flaxkv/serve/route.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,17 +105,17 @@
         print(f"Current subscribers: {_db_manager.subscribers.keys()}")
 
         if db is None:
             _db_manager.set_db(
                 db_name=data.db_name, backend=data.backend, rebuild=data.rebuild
             )
         elif data.rebuild:
-            db.destroy()
+            db.clear(wait=True)
             _db_manager.set_db(
-                db_name=data.db_name, backend=data.backend, rebuild=False
+                db_name=data.db_name, backend=data.backend, rebuild=data.rebuild
             )
 
         async def stream(client: dict) -> AsyncGenerator:
             try:
                 chunk_size = 1024 * 1024
                 while True:
                     done, pending = await asyncio.wait(
```

### Comparing `flaxkv-0.2.7a0/.gitignore` & `flaxkv-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `flaxkv-0.2.7a0/LICENSE` & `flaxkv-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `flaxkv-0.2.7a0/README.md` & `flaxkv-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `flaxkv-0.2.7a0/pyproject.toml` & `flaxkv-0.2.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -46,30 +46,30 @@
 
 [project.optional-dependencies]
 test = [
     "litestar>=2.5.0",
     "pytest",
     "pytest-aiohttp",
     "uvicorn",
-    "httpx",
+    "httpx[http2]",
     "pandas",
     "hypercorn",
     "uvloop; sys_platform == 'linux'",
 ]
 
 server = [
     "uvicorn",
     "hypercorn",
     "uvloop; sys_platform == 'linux'",
     "litestar>=2.5.0",
-    "httpx",
+    "httpx[http2]",
 ]
 
 client = [
-    "httpx",
+    "httpx[http2]",
 ]
 
 
 [project.scripts]
 flaxkv = "flaxkv.__main__:main"
 
 [tool.hatch.version]
```

### Comparing `flaxkv-0.2.7a0/PKG-INFO` & `flaxkv-0.2.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: flaxkv
-Version: 0.2.7a0
+Version: 0.2.8
 Summary: A high-performance dictionary database.
 Project-URL: Homepage, https://github.com/KenyonY/flaxkv
 Project-URL: Documentation, https://github.com/KenyonY/flaxkv#flaxkv
 Project-URL: Issues, https://github.com/KenyonY/flaxkv/issues
 Project-URL: Source, https://github.com/KenyonY/flaxkv
 Author-email: "K.Y" <beidongjiedeguang@gmail.com>
 License-File: LICENSE
@@ -24,23 +24,23 @@
 Requires-Dist: plyvel-ci>=1.5.0; sys_platform == 'win32'
 Requires-Dist: plyvel>=1.5.0; sys_platform == 'linux'
 Requires-Dist: psutil
 Requires-Dist: pytz
 Requires-Dist: rich
 Requires-Dist: typing-extensions>=4.7.1; python_version < '3.11'
 Provides-Extra: client
-Requires-Dist: httpx; extra == 'client'
+Requires-Dist: httpx[http2]; extra == 'client'
 Provides-Extra: server
-Requires-Dist: httpx; extra == 'server'
+Requires-Dist: httpx[http2]; extra == 'server'
 Requires-Dist: hypercorn; extra == 'server'
 Requires-Dist: litestar>=2.5.0; extra == 'server'
 Requires-Dist: uvicorn; extra == 'server'
 Requires-Dist: uvloop; (sys_platform == 'linux') and extra == 'server'
 Provides-Extra: test
-Requires-Dist: httpx; extra == 'test'
+Requires-Dist: httpx[http2]; extra == 'test'
 Requires-Dist: hypercorn; extra == 'test'
 Requires-Dist: litestar>=2.5.0; extra == 'test'
 Requires-Dist: pandas; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-aiohttp; extra == 'test'
 Requires-Dist: uvicorn; extra == 'test'
 Requires-Dist: uvloop; (sys_platform == 'linux') and extra == 'test'
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flaxkv Version: 0.2.7a0 Summary: A high-performance
+Metadata-Version: 2.3 Name: flaxkv Version: 0.2.8 Summary: A high-performance
 dictionary database. Project-URL: Homepage, https://github.com/KenyonY/flaxkv
 Project-URL: Documentation, https://github.com/KenyonY/flaxkv#flaxkv Project-
 URL: Issues, https://github.com/KenyonY/flaxkv/issues Project-URL: Source,
 https://github.com/KenyonY/flaxkv Author-email: "K.Y"
 gmail.com> License-File: LICENSE Keywords: Machine
 Learning,NLP,leveldb,lmdb,on-disk dict,persistent-storage Classifier:
 Development Status :: 5 - Production/Stable Classifier: Operating System :: OS
@@ -10,24 +10,24 @@
 >=3.8 Requires-Dist: fire Requires-Dist: lmdb>=1.4.1 Requires-Dist:
 loguru>=0.7.0 Requires-Dist: msgpack Requires-Dist: msgspec>=0.18.4 Requires-
 Dist: numpy Requires-Dist: orjson>=3.9 Requires-Dist: plyvel-ci>=1.5.0;
 sys_platform == 'darwin' Requires-Dist: plyvel-ci>=1.5.0; sys_platform ==
 'win32' Requires-Dist: plyvel>=1.5.0; sys_platform == 'linux' Requires-Dist:
 psutil Requires-Dist: pytz Requires-Dist: rich Requires-Dist: typing-
 extensions>=4.7.1; python_version < '3.11' Provides-Extra: client Requires-
-Dist: httpx; extra == 'client' Provides-Extra: server Requires-Dist: httpx;
-extra == 'server' Requires-Dist: hypercorn; extra == 'server' Requires-Dist:
-litestar>=2.5.0; extra == 'server' Requires-Dist: uvicorn; extra == 'server'
-Requires-Dist: uvloop; (sys_platform == 'linux') and extra == 'server'
-Provides-Extra: test Requires-Dist: httpx; extra == 'test' Requires-Dist:
-hypercorn; extra == 'test' Requires-Dist: litestar>=2.5.0; extra == 'test'
-Requires-Dist: pandas; extra == 'test' Requires-Dist: pytest; extra == 'test'
-Requires-Dist: pytest-aiohttp; extra == 'test' Requires-Dist: uvicorn; extra ==
-'test' Requires-Dist: uvloop; (sys_platform == 'linux') and extra == 'test'
-Description-Content-Type: text/markdown
+Dist: httpx[http2]; extra == 'client' Provides-Extra: server Requires-Dist:
+httpx[http2]; extra == 'server' Requires-Dist: hypercorn; extra == 'server'
+Requires-Dist: litestar>=2.5.0; extra == 'server' Requires-Dist: uvicorn; extra
+== 'server' Requires-Dist: uvloop; (sys_platform == 'linux') and extra ==
+'server' Provides-Extra: test Requires-Dist: httpx[http2]; extra == 'test'
+Requires-Dist: hypercorn; extra == 'test' Requires-Dist: litestar>=2.5.0; extra
+== 'test' Requires-Dist: pandas; extra == 'test' Requires-Dist: pytest; extra
+== 'test' Requires-Dist: pytest-aiohttp; extra == 'test' Requires-Dist:
+uvicorn; extra == 'test' Requires-Dist: uvloop; (sys_platform == 'linux') and
+extra == 'test' Description-Content-Type: text/markdown
                                     ************
                               ?ð???² FFllaaxxKKVV ************
                     A high-performance dictionary database.
    _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_R_e_l_e_a_s_e_ _(_l_a_t_e_s_t_ _b_y_ _d_a_t_e_)_]_[_t_e_s_t_s_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_s_]
                         ****** EEnngglliisshh || _?ç_?®_?_?ä_?½_?_?ä_?¸_?­_?æ_?_? ******
 
 The `flaxkv` provides an interface very similar to a dictionary for interacting
```

