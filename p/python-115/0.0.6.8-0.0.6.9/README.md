# Comparing `tmp/python_115-0.0.6.8.tar.gz` & `tmp/python_115-0.0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.6.8.tar", max compression
+gzip compressed data, was "python_115-0.0.6.9.tar", max compression
```

## Comparing `python_115-0.0.6.8.tar` & `python_115-0.0.6.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.6.8/LICENSE
--rwxr-xr-x   0        0        0   276387 2024-04-26 05:53:52.784598 python_115-0.0.6.8/p115/__init__.py
--rwxr-xr-x   0        0        0      210 2024-04-26 14:24:31.454980 python_115-0.0.6.8/p115/__main__.py
--rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.6.8/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0      336 2024-04-19 15:07:36.047405 python_115-0.0.6.8/p115/cmd/init.py
--rwxr-xr-x   0        0        0     6742 2024-04-21 18:19:00.204183 python_115-0.0.6.8/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     1445 2024-04-20 20:02:42.644715 python_115-0.0.6.8/p115/cmd/qrcode.py
--rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.6.8/p115/exception.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.6.8/p115/py.typed
--rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.6.8/p115/util/__init__.py
--rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.6.8/p115/util/_init_mimetypes.py
--rwxr-xr-x   0        0        0      360 2024-04-22 14:19:39.864074 python_115-0.0.6.8/p115/util/args.py
--rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.6.8/p115/util/cipher.py
--rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.6.8/p115/util/concurrent.py
--rwxr-xr-x   0        0        0    12230 2024-04-25 02:39:02.864829 python_115-0.0.6.8/p115/util/download.py
--rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.6.8/p115/util/file.py
--rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.6.8/p115/util/hash.py
--rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.6.8/p115/util/ignore.py
--rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.6.8/p115/util/iter.py
--rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.6.8/p115/util/path.py
--rwxr-xr-x   0        0        0     1846 2024-04-24 15:33:36.222174 python_115-0.0.6.8/p115/util/property.py
--rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.6.8/p115/util/response.py
--rwxr-xr-x   0        0        0     6150 2024-04-24 16:05:44.697816 python_115-0.0.6.8/p115/util/retry.py
--rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.6.8/p115/util/text.py
--rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.6.8/p115/util/upload.py
--rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.6.8/p115/util/urlopen.py
--rw-r--r--   0        0        0     1272 2024-04-26 14:25:30.231597 python_115-0.0.6.8/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.6.8/readme.md
--rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.6.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.6.9/LICENSE
+-rwxr-xr-x   0        0        0   278288 2024-04-27 06:52:19.943731 python_115-0.0.6.9/p115/__init__.py
+-rwxr-xr-x   0        0        0      115 2024-04-26 14:30:33.715269 python_115-0.0.6.9/p115/__main__.py
+-rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.6.9/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0      336 2024-04-19 15:07:36.047405 python_115-0.0.6.9/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     6742 2024-04-21 18:19:00.204183 python_115-0.0.6.9/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     1445 2024-04-20 20:02:42.644715 python_115-0.0.6.9/p115/cmd/qrcode.py
+-rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.6.9/p115/exception.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.6.9/p115/py.typed
+-rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.6.9/p115/util/__init__.py
+-rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.6.9/p115/util/_init_mimetypes.py
+-rwxr-xr-x   0        0        0      360 2024-04-22 14:19:39.864074 python_115-0.0.6.9/p115/util/args.py
+-rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.6.9/p115/util/cipher.py
+-rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.6.9/p115/util/concurrent.py
+-rwxr-xr-x   0        0        0    12230 2024-04-25 02:39:02.864829 python_115-0.0.6.9/p115/util/download.py
+-rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.6.9/p115/util/file.py
+-rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.6.9/p115/util/hash.py
+-rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.6.9/p115/util/ignore.py
+-rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.6.9/p115/util/iter.py
+-rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.6.9/p115/util/path.py
+-rwxr-xr-x   0        0        0     1846 2024-04-24 15:33:36.222174 python_115-0.0.6.9/p115/util/property.py
+-rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.6.9/p115/util/response.py
+-rwxr-xr-x   0        0        0     6150 2024-04-24 16:05:44.697816 python_115-0.0.6.9/p115/util/retry.py
+-rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.6.9/p115/util/text.py
+-rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.6.9/p115/util/upload.py
+-rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.6.9/p115/util/urlopen.py
+-rw-r--r--   0        0        0     1272 2024-04-27 07:46:40.661926 python_115-0.0.6.9/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.6.9/readme.md
+-rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.6.9/PKG-INFO
```

### Comparing `python_115-0.0.6.8/LICENSE` & `python_115-0.0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.8/p115/__init__.py` & `python_115-0.0.6.9/p115/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -542,14 +542,69 @@
     ) -> dict:
         """获取已登录设备的信息
         GET https://passportapi.115.com/app/1.0/web/9.2/login_log/login_devices
         """
         api = "https://passportapi.115.com/app/1.0/web/9.2/login_log/login_devices"
         return self.request(api, async_=async_, **request_kwargs)
 
+    def login_qrcode_scan(
+        self, 
+        payload: str | dict, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        """扫描二维码，payload 数据取自 `login_qrcode_token` 接口响应
+        GET https://qrcodeapi.115.com/api/2.0/prompt.php
+        payload:
+            - uid: str
+        """
+        api = "https://qrcodeapi.115.com/api/2.0/prompt.php"
+        if isinstance(payload, str):
+            payload = {"uid": payload}
+        return self.request(api, params=payload, async_=async_, **request_kwargs)
+
+    def login_qrcode_scan_confirm(
+        self, 
+        payload: str | dict, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        """确认扫描二维码，payload 数据取自 `login_qrcode_scan` 接口响应
+        GET https://hnqrcodeapi.115.com/api/2.0/slogin.php
+        payload:
+            - key: str
+            - uid: str
+            - client: int = 0
+        """
+        api = "https://hnqrcodeapi.115.com/api/2.0/slogin.php"
+        if isinstance(payload, str):
+            payload = {"key": payload, "uid": payload, "client": 0}
+        return self.request(api, params=payload, async_=async_, **request_kwargs)
+
+    def login_qrcode_scan_cancel(
+        self, 
+        payload: dict, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        """确认扫描二维码，payload 数据取自 `login_qrcode_scan` 接口响应
+        GET https://hnqrcodeapi.115.com/api/2.0/cancel.php
+        payload:
+            - key: str
+            - uid: str
+            - client: int = 0
+        """
+        api = "https://hnqrcodeapi.115.com/api/2.0/cancel.php"
+        if isinstance(payload, str):
+            payload = {"key": payload, "uid": payload, "client": 0}
+        return self.request(api, params=payload, async_=async_, **request_kwargs)
+
     def login_qrcode_status(
         self, 
         payload: dict, 
         /, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
```

### Comparing `python_115-0.0.6.8/p115/cmd/iterdir.py` & `python_115-0.0.6.9/p115/cmd/iterdir.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.8/p115/cmd/qrcode.py` & `python_115-0.0.6.9/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.8/p115/util/_init_mimetypes.py` & `python_115-0.0.6.9/p115/util/_init_mimetypes.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.8/p115/util/cipher.py` & `python_115-0.0.6.9/p115/util/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.8/p115/util/concurrent.py` & `python_115-0.0.6.9/p115/util/concurrent.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.8/p115/util/download.py` & `python_115-0.0.6.9/p115/util/download.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.8/p115/util/file.py` & `python_115-0.0.6.9/p115/util/file.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.8/p115/util/hash.py` & `python_115-0.0.6.9/p115/util/hash.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.8/p115/util/ignore.py` & `python_115-0.0.6.9/p115/util/ignore.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.8/p115/util/iter.py` & `python_115-0.0.6.9/p115/util/iter.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.8/p115/util/path.py` & `python_115-0.0.6.9/p115/util/path.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.8/p115/util/property.py` & `python_115-0.0.6.9/p115/util/property.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.8/p115/util/response.py` & `python_115-0.0.6.9/p115/util/response.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.8/p115/util/retry.py` & `python_115-0.0.6.9/p115/util/retry.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.8/p115/util/text.py` & `python_115-0.0.6.9/p115/util/text.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.8/p115/util/urlopen.py` & `python_115-0.0.6.9/p115/util/urlopen.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.8/pyproject.toml` & `python_115-0.0.6.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.6.8"
+version = "0.0.6.9"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["nas", "115"]
```

### Comparing `python_115-0.0.6.8/readme.md` & `python_115-0.0.6.9/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.8/PKG-INFO` & `python_115-0.0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.6.8
+Version: 0.0.6.9
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: nas,115
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

