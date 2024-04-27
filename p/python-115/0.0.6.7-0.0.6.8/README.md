# Comparing `tmp/python_115-0.0.6.7.tar.gz` & `tmp/python_115-0.0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.6.7.tar", max compression
+gzip compressed data, was "python_115-0.0.6.8.tar", max compression
```

## Comparing `python_115-0.0.6.7.tar` & `python_115-0.0.6.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.6.7/LICENSE
--rwxr-xr-x   0        0        0   276350 2024-04-25 04:29:48.234079 python_115-0.0.6.7/p115/__init__.py
--rwxr-xr-x   0        0        0      115 2024-04-19 15:21:20.677842 python_115-0.0.6.7/p115/__main__.py
--rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.6.7/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0      336 2024-04-19 15:07:36.047405 python_115-0.0.6.7/p115/cmd/init.py
--rwxr-xr-x   0        0        0     6742 2024-04-21 18:19:00.204183 python_115-0.0.6.7/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     1445 2024-04-20 20:02:42.644715 python_115-0.0.6.7/p115/cmd/qrcode.py
--rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.6.7/p115/exception.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.6.7/p115/py.typed
--rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.6.7/p115/util/__init__.py
--rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.6.7/p115/util/_init_mimetypes.py
--rwxr-xr-x   0        0        0      360 2024-04-22 14:19:39.864074 python_115-0.0.6.7/p115/util/args.py
--rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.6.7/p115/util/cipher.py
--rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.6.7/p115/util/concurrent.py
--rwxr-xr-x   0        0        0    12230 2024-04-25 02:39:02.864829 python_115-0.0.6.7/p115/util/download.py
--rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.6.7/p115/util/file.py
--rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.6.7/p115/util/hash.py
--rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.6.7/p115/util/ignore.py
--rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.6.7/p115/util/iter.py
--rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.6.7/p115/util/path.py
--rwxr-xr-x   0        0        0     1846 2024-04-24 15:33:36.222174 python_115-0.0.6.7/p115/util/property.py
--rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.6.7/p115/util/response.py
--rwxr-xr-x   0        0        0     6150 2024-04-24 16:05:44.697816 python_115-0.0.6.7/p115/util/retry.py
--rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.6.7/p115/util/text.py
--rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.6.7/p115/util/upload.py
--rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.6.7/p115/util/urlopen.py
--rw-r--r--   0        0        0     1272 2024-04-25 04:30:01.791920 python_115-0.0.6.7/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.6.7/readme.md
--rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.6.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.6.8/LICENSE
+-rwxr-xr-x   0        0        0   276387 2024-04-26 05:53:52.784598 python_115-0.0.6.8/p115/__init__.py
+-rwxr-xr-x   0        0        0      210 2024-04-26 14:24:31.454980 python_115-0.0.6.8/p115/__main__.py
+-rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.6.8/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0      336 2024-04-19 15:07:36.047405 python_115-0.0.6.8/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     6742 2024-04-21 18:19:00.204183 python_115-0.0.6.8/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     1445 2024-04-20 20:02:42.644715 python_115-0.0.6.8/p115/cmd/qrcode.py
+-rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.6.8/p115/exception.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.6.8/p115/py.typed
+-rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.6.8/p115/util/__init__.py
+-rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.6.8/p115/util/_init_mimetypes.py
+-rwxr-xr-x   0        0        0      360 2024-04-22 14:19:39.864074 python_115-0.0.6.8/p115/util/args.py
+-rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.6.8/p115/util/cipher.py
+-rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.6.8/p115/util/concurrent.py
+-rwxr-xr-x   0        0        0    12230 2024-04-25 02:39:02.864829 python_115-0.0.6.8/p115/util/download.py
+-rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.6.8/p115/util/file.py
+-rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.6.8/p115/util/hash.py
+-rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.6.8/p115/util/ignore.py
+-rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.6.8/p115/util/iter.py
+-rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.6.8/p115/util/path.py
+-rwxr-xr-x   0        0        0     1846 2024-04-24 15:33:36.222174 python_115-0.0.6.8/p115/util/property.py
+-rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.6.8/p115/util/response.py
+-rwxr-xr-x   0        0        0     6150 2024-04-24 16:05:44.697816 python_115-0.0.6.8/p115/util/retry.py
+-rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.6.8/p115/util/text.py
+-rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.6.8/p115/util/upload.py
+-rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.6.8/p115/util/urlopen.py
+-rw-r--r--   0        0        0     1272 2024-04-26 14:25:30.231597 python_115-0.0.6.8/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.6.8/readme.md
+-rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.6.8/PKG-INFO
```

### Comparing `python_115-0.0.6.7/LICENSE` & `python_115-0.0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.7/p115/__init__.py` & `python_115-0.0.6.8/p115/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from inspect import isawaitable, iscoroutinefunction
 from io import (
     BufferedReader, BytesIO, TextIOWrapper, UnsupportedOperation, DEFAULT_BUFFER_SIZE, 
 )
 from itertools import count
 from json import dumps, loads
 from mimetypes import guess_type
-from os import fsdecode, fspath, fstat, makedirs, scandir, stat, stat_result, PathLike
+from os import fsdecode, fspath, fstat, lstat, makedirs, scandir, stat, stat_result, PathLike
 from os import path as ospath
 from posixpath import join as joinpath, splitext
 from re import compile as re_compile, escape as re_escape
 from shutil import copyfileobj, SameFileError
 from stat import S_IFDIR, S_IFREG
 from threading import Condition, Thread
 from time import sleep, time
@@ -4173,26 +4173,28 @@
     def attr(self, /) -> MappingProxyType:
         return MappingProxyType(self.__dict__)
 
     def download(
         self, 
         /, 
         local_dir: bytes | str | PathLike = "", 
-        pid: Optional[int] = None, 
-        no_root: bool = False, 
         write_mode: Literal["a", "w", "x", "i"] = "a", 
-        **get_url_kwargs, 
-    ):
+        submit: None | bool | Callable[[Callable], Any] = None, 
+        no_root: bool = False, 
+        predicate: Optional[Callable[[P115PathType], bool]] = None, 
+        onerror: None | bool | Callable[[BaseException], Any] = None, 
+    ) -> Iterator[tuple[P115PathType, str, DownloadTask]]:
         return self.fs.download_tree(
             self, 
             local_dir, 
-            pid=pid, 
-            no_root=no_root, 
             write_mode=write_mode, 
-            **get_url_kwargs, 
+            submit=submit, 
+            no_root=no_root, 
+            predicate=predicate, 
+            onerror=onerror, 
         )
 
     def exists(self, /) -> bool:
         return self.fs.exists(self)
 
     @property
     def file_extension(self, /) -> Optional[str]:
@@ -4657,15 +4659,14 @@
         self, 
         id_or_path: IDOrPathType, 
         /, 
         local_path_or_file: bytes | str | PathLike | SupportsWrite[bytes] = "", 
         pid: Optional[int] = None, 
         write_mode: Literal["a", "w", "x", "i"] = "a", 
         submit: bool | Callable[[Callable], Any] = True, 
-        **get_url_kwargs, 
     ) -> Optional[DownloadTask]:
         if not hasattr(local_path_or_file, "write"):
             if not local_path_or_file:
                 local_path_or_file = self.attr(id_or_path, pid)["name"]
             if ospath.lexists(local_path_or_file): # type: ignore
                 if write_mode == "x":
                     raise FileExistsError(
@@ -4674,15 +4675,15 @@
                     )
                 elif write_mode == "i":
                     return None
         kwargs: dict = {"resume": write_mode == "a"}
         if callable(submit):
             kwargs["submit"] = submit
         task = DownloadTask.create_task(
-            lambda: self.get_url(id_or_path, pid, **get_url_kwargs), 
+            lambda: self.get_url(id_or_path, pid), 
             local_path_or_file, 
             headers=lambda: {
                 **self.client.session.headers, 
                 "Cookie": "; ".join(f"{c.name}={c.value}" for c in self.client.session.cookies), 
             }, 
             **kwargs, 
         )
@@ -4695,19 +4696,19 @@
     def download_tree(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         local_dir: bytes | str | PathLike = "", 
         pid: Optional[int] = None, 
         write_mode: Literal["i", "x", "w", "a"] = "a", 
+        submit: None | bool | Callable[[Callable], Any] = None, 
         no_root: bool = False, 
         predicate: Optional[Callable[[P115PathType], bool]] = None, 
         onerror: None | bool | Callable[[BaseException], Any] = None, 
-        **get_url_kwargs, 
-    ) -> Iterator[tuple[P115PathType, DownloadTask]]:
+    ) -> Iterator[tuple[P115PathType, str, DownloadTask]]:
         local_dir = fsdecode(local_dir)
         if local_dir:
             makedirs(local_dir, exist_ok=True)
         attr = self.attr(id_or_path, pid)
         pathes: Iterable[P115PathType]
         if attr["is_directory"]:
             if not no_root:
@@ -4715,45 +4716,57 @@
                 if local_dir:
                     makedirs(local_dir, exist_ok=True)
             pathes = self.scandir(attr["id"])
         else:
             path_class = type(self).path_class
             attr["fs"] = self
             pathes = (path_class(attr),)
+        mode: Literal["i", "x", "w", "a"]
         for subpath in filter(predicate, pathes):
             if subpath["is_directory"]:
                 yield from self.download_tree(
                     subpath["id"], 
                     ospath.join(local_dir, subpath["name"]), 
                     write_mode=write_mode, 
                     no_root=True, 
                     predicate=predicate, 
                     onerror=onerror, 
-                    **get_url_kwargs, 
                 )
             else:
+                mode = write_mode
                 try:
+                    download_path = ospath.join(local_dir, subpath["name"])
+                    remote_size = subpath["size"]
+                    try:
+                        size = lstat(download_path).st_size
+                    except OSError:
+                        pass
+                    else:
+                        if remote_size == size:
+                            continue
+                        elif remote_size < size:
+                            mode = "w"
                     task = self.download(
                         subpath["id"], 
-                        ospath.join(local_dir, subpath["name"]), 
-                        write_mode=write_mode, 
-                        submit=False, 
-                        **get_url_kwargs, 
+                        download_path, 
+                        write_mode=mode, 
+                        submit=False if submit is None else submit, 
                     )
                 except KeyboardInterrupt:
                     raise
                 except BaseException as exc:
                     if onerror is None or onerror is True:
                         raise
                     elif callable(onerror):
                         onerror(exc)
                 else:
                     if task is not None:
-                        yield subpath, task
-                        task.run_wait()
+                        yield subpath, download_path, task
+                        if submit is None:
+                            task.run_wait()
 
     def exists(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> bool:
@@ -5908,35 +5921,14 @@
                                 path_to_id[new_subpath] = subid
                         if subattr["is_directory"]:
                             put(subid)
             if path_to_id is not None and pop_path is not None:
                 for k in tuple(k for k in path_to_id if startswith(k, old_path)):
                     pop_path(k)
 
-    def download(
-        self, 
-        id_or_path: IDOrPathType, 
-        /, 
-        local_path_or_file: bytes | str | PathLike | SupportsWrite[bytes] = "", 
-        pid: Optional[int] = None, 
-        write_mode: Literal["a", "w", "x", "i"] = "a", 
-        submit = None, 
-        use_web_api: bool = True, 
-        **get_url_kwargs, 
-    ) -> Optional[DownloadTask]:
-        return super().download(
-            id_or_path, 
-            local_path_or_file, 
-            pid=pid, 
-            write_mode=write_mode, 
-            submit=submit, 
-            use_web_api=use_web_api, 
-            **get_url_kwargs, 
-        )
-
     def iterdir(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
         refresh: bool = False, 
     ) -> Iterator[AttrDict]:
@@ -6387,39 +6379,36 @@
     def get_url(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: Optional[int] = None, 
         headers: Optional[Mapping] = None, 
         detail: bool = False, 
-        use_web_api: bool = False, 
     ) -> str:
         attr = self.attr(id_or_path, pid)
         if attr["is_directory"]:
             raise IsADirectoryError(errno.EISDIR, f"{attr['path']!r} (id={attr['id']!r}) is a directory")
         return self.client.download_url(
             attr["pickcode"], 
-            use_web_api=use_web_api and attr["size"] < 1024 * 1024 * 115, 
+            use_web_api=attr["is_violation"] and attr["size"] < 1024 * 1024 * 115, 
             detail=detail, 
             headers=headers, 
         )
 
     def get_url_from_pickcode(
         self, 
         /, 
         pickcode: str, 
         headers: Optional[Mapping] = None, 
         detail: bool = False, 
-        use_web_api: bool = False, 
     ) -> str:
         return self.client.download_url(
             pickcode, 
             detail=detail, 
             headers=headers, 
-            use_web_api=use_web_api, 
         )
 
     def is_empty(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None,
```

### Comparing `python_115-0.0.6.7/p115/cmd/iterdir.py` & `python_115-0.0.6.8/p115/cmd/iterdir.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.7/p115/cmd/qrcode.py` & `python_115-0.0.6.8/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.7/p115/util/_init_mimetypes.py` & `python_115-0.0.6.8/p115/util/_init_mimetypes.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.7/p115/util/cipher.py` & `python_115-0.0.6.8/p115/util/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.7/p115/util/concurrent.py` & `python_115-0.0.6.8/p115/util/concurrent.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.7/p115/util/download.py` & `python_115-0.0.6.8/p115/util/download.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.7/p115/util/file.py` & `python_115-0.0.6.8/p115/util/file.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.7/p115/util/hash.py` & `python_115-0.0.6.8/p115/util/hash.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.7/p115/util/ignore.py` & `python_115-0.0.6.8/p115/util/ignore.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.7/p115/util/iter.py` & `python_115-0.0.6.8/p115/util/iter.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.7/p115/util/path.py` & `python_115-0.0.6.8/p115/util/path.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.7/p115/util/property.py` & `python_115-0.0.6.8/p115/util/property.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.7/p115/util/response.py` & `python_115-0.0.6.8/p115/util/response.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.7/p115/util/retry.py` & `python_115-0.0.6.8/p115/util/retry.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.7/p115/util/text.py` & `python_115-0.0.6.8/p115/util/text.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.7/p115/util/urlopen.py` & `python_115-0.0.6.8/p115/util/urlopen.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.7/pyproject.toml` & `python_115-0.0.6.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.6.7"
+version = "0.0.6.8"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["nas", "115"]
```

### Comparing `python_115-0.0.6.7/readme.md` & `python_115-0.0.6.8/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.7/PKG-INFO` & `python_115-0.0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.6.7
+Version: 0.0.6.8
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: nas,115
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

