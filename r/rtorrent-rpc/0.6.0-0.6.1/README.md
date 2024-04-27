# Comparing `tmp/rtorrent_rpc-0.6.0.tar.gz` & `tmp/rtorrent_rpc-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtorrent_rpc-0.6.0.tar", max compression
+gzip compressed data, was "rtorrent_rpc-0.6.1.tar", max compression
```

## Comparing `rtorrent_rpc-0.6.0.tar` & `rtorrent_rpc-0.6.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1084 2024-04-26 15:42:43.509531 rtorrent_rpc-0.6.0/LICENSE
--rw-r--r--   0        0        0     2456 2024-04-26 15:42:43.513531 rtorrent_rpc-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1436 2024-04-26 15:42:43.513531 rtorrent_rpc-0.6.0/readme.md
--rw-r--r--   0        0        0    29423 2024-04-26 15:42:43.513531 rtorrent_rpc-0.6.0/rtorrent_rpc/__init__.py
--rw-r--r--   0        0        0     2327 2024-04-26 15:42:43.513531 rtorrent_rpc-0.6.0/rtorrent_rpc/_jsonrpc/__init__.py
--rw-r--r--   0        0        0     3050 2024-04-26 15:42:43.513531 rtorrent_rpc-0.6.0/rtorrent_rpc/_jsonrpc/transport.py
--rw-r--r--   0        0        0     1235 2024-04-26 15:42:43.513531 rtorrent_rpc-0.6.0/rtorrent_rpc/_scgi.py
--rw-r--r--   0        0        0      803 2024-04-26 15:42:43.513531 rtorrent_rpc-0.6.0/rtorrent_rpc/_transport.py
--rw-r--r--   0        0        0     3694 2024-04-26 15:42:43.513531 rtorrent_rpc-0.6.0/rtorrent_rpc/helper.py
--rw-r--r--   0        0        0        0 2024-04-26 15:42:43.513531 rtorrent_rpc-0.6.0/rtorrent_rpc/py.typed
--rw-r--r--   0        0        0     2403 1970-01-01 00:00:00.000000 rtorrent_rpc-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-04-27 16:18:58.033188 rtorrent_rpc-0.6.1/LICENSE
+-rw-r--r--   0        0        0     2456 2024-04-27 16:18:58.033188 rtorrent_rpc-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1436 2024-04-27 16:18:58.033188 rtorrent_rpc-0.6.1/readme.md
+-rw-r--r--   0        0        0    29525 2024-04-27 16:18:58.033188 rtorrent_rpc-0.6.1/rtorrent_rpc/__init__.py
+-rw-r--r--   0        0        0     2458 2024-04-27 16:18:58.033188 rtorrent_rpc-0.6.1/rtorrent_rpc/_jsonrpc/__init__.py
+-rw-r--r--   0        0        0     3050 2024-04-27 16:18:58.033188 rtorrent_rpc-0.6.1/rtorrent_rpc/_jsonrpc/transport.py
+-rw-r--r--   0        0        0     1235 2024-04-27 16:18:58.033188 rtorrent_rpc-0.6.1/rtorrent_rpc/_scgi.py
+-rw-r--r--   0        0        0      803 2024-04-27 16:18:58.033188 rtorrent_rpc-0.6.1/rtorrent_rpc/_transport.py
+-rw-r--r--   0        0        0     3920 2024-04-27 16:18:58.033188 rtorrent_rpc-0.6.1/rtorrent_rpc/helper.py
+-rw-r--r--   0        0        0        0 2024-04-27 16:18:58.037188 rtorrent_rpc-0.6.1/rtorrent_rpc/py.typed
+-rw-r--r--   0        0        0     2403 1970-01-01 00:00:00.000000 rtorrent_rpc-0.6.1/PKG-INFO
```

### Comparing `rtorrent_rpc-0.6.0/LICENSE` & `rtorrent_rpc-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.0/pyproject.toml` & `rtorrent_rpc-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rtorrent-rpc"
-version = "0.6.0"
+version = "0.6.1"
 description = "Typed rtorrent rpc client"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'readme.md'
 repository = 'https://github.com/trim21/rtorrent-rpc'
 license = 'MIT'
 packages = [{ include = 'rtorrent_rpc' }]
 keywords = ['rtorrent', 'rpc']
```

### Comparing `rtorrent_rpc-0.6.0/readme.md` & `rtorrent_rpc-0.6.1/readme.md`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.0/rtorrent_rpc/__init__.py` & `rtorrent_rpc-0.6.1/rtorrent_rpc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,26 +117,37 @@
 
     If you are using ruTorrent or nginx scgi proxy, http(s) protocol are also supported
 
     .. code-block:: python
 
         rt = RTorrent('http://127.0.0.1')
 
+    by default, ``/RPC2`` path is used.
 
-    Underling ``xmlrpc.client.ServerProxy`` are exposed as instance property ``.rpc``,
-    you can use ``rt.rpc`` for direct rpc call.
 
-    :param address: rtorrent rpc address
-    :param rutorrent_compatibility: compatibility for ruTorrent or flood.
     """
 
     rpc: xmlrpc.client.ServerProxy
+    """
+    Underling ``xmlrpc.client.ServerProxy`` are exposed as instance property ``.rpc``,
+    you can use ``rt.rpc`` for direct rpc call.
+    """
+
     jsonrpc: JSONRpc
+    """
+    a :class:`JSONRpc` instance to send rpc request with json-rpc.
+    """
 
     def __init__(self, address: str, rutorrent_compatibility: bool = True):
+        """
+        Args:
+            address: rtorrent rpc address
+            rutorrent_compatibility: compatibility for ruTorrent or flood.
+        """
+
         u = urllib.parse.urlparse(address)
         if u.scheme == "scgi":
             self.rpc = SCGIServerProxy(address)
         else:
             self.rpc = xmlrpc.client.ServerProxy(address)
 
         self.jsonrpc = JSONRpc(address=address)
@@ -214,36 +225,32 @@
         """get list of info hash for current downloads"""
         return self.rpc.download_list()  # type: ignore
 
     @property
     def system(self) -> _SystemRpc:
         """method call with ``system`` prefix
 
-        Example:
+        .. code-block:: python
 
-            .. code-block:: python
-
-                rt.system.listMethods(...)
+            rt.system.listMethods(...)
         """
         return self.rpc.system  # type: ignore
 
     def system_list_methods(self) -> list[str]:
         """get supported methods"""
         return self.rpc.system.listMethods()  # type: ignore
 
     @property
     def d(self) -> _DownloadRpc:
         """method call with ``d`` prefix
 
-        Example:
-
-            .. code-block:: python
+        .. code-block:: python
 
-                rt.d.save_resume(...)
-                rt.d.open(...)
+            rt.d.save_resume(...)
+            rt.d.open(...)
         """
         return self.rpc.d  # type: ignore
 
     def d_set_torrent_base_directory(self, info_hash: str, directory: str) -> None:
         """change base directory of a download.
 
         you may need to stop/close torrent first.
@@ -267,49 +274,46 @@
         return self.d.custom.set(info_hash, key, value)
 
     def d_get_custom(self, info_hash: str, key: str) -> str:
         """get custom value by key, return empty str if key not set"""
         return self.d.custom(info_hash, key)
 
     def d_tracker_send_scrape(self, info_hash: str, delay: Unknown) -> None:
+        """force announce"""
         self.rpc.d.tracker.send_scrape(info_hash, delay)
 
+    def d_add_tracker(self, info_hash: str, url: str, *, group: int = 0) -> None:
+        """add a tracker to download"""
+        self.rpc.d.tracker.insert(info_hash, group, url)
+
     @property
     def t(self) -> _TrackerRpc:
         """method call with ``t`` prefix
 
-        Example:
+        .. code-block:: python
 
-            .. code-block:: python
-
-                rt.t.is_enabled(...)
+            rt.t.is_enabled(...)
         """
         return self.rpc.t  # type: ignore
 
     def t_enable_tracker(self, info_hash: str, tracker_index: int) -> None:
         """enable a tracker of download"""
         self.rpc.t.is_enabled.set(f"{info_hash}:t{tracker_index}", 1)
 
     def t_disable_tracker(self, info_hash: str, tracker_index: int) -> None:
         """disable a tracker of download"""
         self.rpc.t.is_enabled.set(f"{info_hash}:t{tracker_index}", 0)
 
-    def d_add_tracker(self, info_hash: str, url: str, *, group: int = 0) -> None:
-        """add a tracker to download"""
-        self.rpc.d.tracker.insert(info_hash, group, url)
-
     @property
     def f(self) -> _FileRpc:
         """method call with ``d`` prefix
 
-        Example:
-
-            .. code-block:: python
+        .. code-block:: python
 
-                rt.f.multicall("<info_hash>", "", "f.path=")
+            rt.f.multicall("<info_hash>", "", "f.path=")
         """
         return self.rpc.f  # type: ignore
 
 
 _methods = [
     "system.methodExist",
     "system.methodHelp",
```

### Comparing `rtorrent_rpc-0.6.0/rtorrent_rpc/_jsonrpc/__init__.py` & `rtorrent_rpc-0.6.1/rtorrent_rpc/_jsonrpc/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,19 +48,24 @@
         self.code = code
         self.message = message
         self.data = data
         self.id = id
 
 
 class JSONRpc:
+    """
+    this class is exposed as ``RTorrent(...).jsonrpc``,
+    you do not need to construct it by yourself.
+    """
+
     _id: int
     _lock: threading.Lock
     _transport: Transport
 
-    __slots__ = ("__host", "__port", "_id", "_lock", "_transport")
+    __slots__ = ("_id", "_lock", "_transport")
 
     def __init__(self, address: str):
         url = urlparse(address)
 
         if url.scheme == "scgi":
             self._transport = _SCGITransport(address)
         elif url.scheme in ("http", "https"):
@@ -68,18 +73,19 @@
         else:
             raise ValueError(f"unsupported protocol {url.scheme}")
 
         self._id = 0
         self._lock = threading.Lock()
 
     def call(self, method: str, params: Any = None) -> Any:
+        """send a json-rpc call"""
         with self._lock:
             id = self._id
             # unlikely to have 100w concurrent request...
-            self._id = (self._id + 1) % 1000000
+            self._id = (id + 1) % 1000000
 
         req = _encode_json(
             {"jsonrpc": "2.0", "id": id, "method": method, "params": params}
         )
 
         res = self._transport.request(req, "application/json")
```

### Comparing `rtorrent_rpc-0.6.0/rtorrent_rpc/_jsonrpc/transport.py` & `rtorrent_rpc-0.6.1/rtorrent_rpc/_jsonrpc/transport.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.0/rtorrent_rpc/_scgi.py` & `rtorrent_rpc-0.6.1/rtorrent_rpc/_scgi.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.0/rtorrent_rpc/_transport.py` & `rtorrent_rpc-0.6.1/rtorrent_rpc/_transport.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.0/rtorrent_rpc/helper.py` & `rtorrent_rpc-0.6.1/rtorrent_rpc/helper.py`

 * *Files 15% similar despite different names*

```diff
@@ -57,32 +57,39 @@
     NORMAL = 1
     HIGH = 2
 
 
 def add_fast_resume_file(base_save_path: Path, torrent_content: bytes) -> bytes:
     """update torrent content, add resume data to torrent,
     skip checking file exists on disk.
+
+    Warnings:
+        this may cause rtorrent into a invalid state and causing bugs, use at your own risk.
     """
 
     return __add_resume_file(
         base_save_path, torrent_content, LibTorrentFilePriority.NORMAL
     )
 
 
 def add_completed_resume_file(base_save_path: Path, torrent_content: bytes) -> bytes:
-    """update torrent content, add resume data to torrent."""
+    """update torrent content, add resume data to torrent.
+
+    Warnings:
+        this may cause rtorrent into a invalid state and causing bugs, use at your own risk.
+    """
     return __add_resume_file(
         base_save_path, torrent_content, LibTorrentFilePriority.OFF
     )
 
 
 def __add_resume_file(
     base_save_path: Path,
     torrent_content: bytes,
-    un_complete_file_prop,
+    un_complete_file_prop: int,
 ) -> bytes:
     """
     based on [rtorrent_fast_resume.pl](https://github.com/rakshasa/rtorrent/blob/master/doc/rtorrent_fast_resume.pl)
     """
     data: dict[str, Any] = bencode2.bdecode(torrent_content, str_key=True)
 
     piece_length = data["info"]["piece length"]
```

### Comparing `rtorrent_rpc-0.6.0/PKG-INFO` & `rtorrent_rpc-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtorrent-rpc
-Version: 0.6.0
+Version: 0.6.1
 Summary: Typed rtorrent rpc client
 Home-page: https://github.com/trim21/rtorrent-rpc
 License: MIT
 Keywords: rtorrent,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.8,<4.0
```

