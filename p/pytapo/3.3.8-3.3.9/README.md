# Comparing `tmp/pytapo-3.3.8.tar.gz` & `tmp/pytapo-3.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytapo-3.3.8.tar", last modified: Wed Nov 15 10:14:48 2023, max compression
+gzip compressed data, was "pytapo-3.3.9.tar", last modified: Wed Nov 15 10:47:40 2023, max compression
```

## Comparing `pytapo-3.3.8.tar` & `pytapo-3.3.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 jnyiri     (501) staff       (20)        0 2023-11-15 10:14:48.286388 pytapo-3.3.8/
--rw-r--r--   0 jnyiri     (501) staff       (20)     1069 2023-04-19 11:02:05.000000 pytapo-3.3.8/LICENSE
--rw-r--r--   0 jnyiri     (501) staff       (20)       16 2023-04-19 11:02:05.000000 pytapo-3.3.8/MANIFEST.in
--rw-r--r--   0 jnyiri     (501) staff       (20)     5533 2023-11-15 10:14:48.286281 pytapo-3.3.8/PKG-INFO
--rw-r--r--   0 jnyiri     (501) staff       (20)     5076 2023-04-19 11:02:05.000000 pytapo-3.3.8/README.md
-drwxr-xr-x   0 jnyiri     (501) staff       (20)        0 2023-11-15 10:14:48.283165 pytapo-3.3.8/pytapo/
--rw-r--r--   0 jnyiri     (501) staff       (20)      747 2023-08-21 10:42:21.000000 pytapo-3.3.8/pytapo/TlsAdapter.py
--rw-r--r--   0 jnyiri     (501) staff       (20)    64215 2023-11-15 10:13:12.000000 pytapo-3.3.8/pytapo/__init__.py
--rw-r--r--   0 jnyiri     (501) staff       (20)      614 2023-08-19 10:23:34.000000 pytapo-3.3.8/pytapo/const.py
-drwxr-xr-x   0 jnyiri     (501) staff       (20)        0 2023-11-15 10:14:48.286054 pytapo-3.3.8/pytapo/media_stream/
--rw-r--r--   0 jnyiri     (501) staff       (20)        0 2023-04-19 11:02:05.000000 pytapo-3.3.8/pytapo/media_stream/__init__.py
--rw-r--r--   0 jnyiri     (501) staff       (20)     1977 2023-04-19 11:02:05.000000 pytapo-3.3.8/pytapo/media_stream/_utils.py
--rw-r--r--   0 jnyiri     (501) staff       (20)     4346 2023-05-04 14:22:22.000000 pytapo-3.3.8/pytapo/media_stream/convert.py
--rw-r--r--   0 jnyiri     (501) staff       (20)     2626 2023-04-19 11:02:05.000000 pytapo-3.3.8/pytapo/media_stream/crypto.py
--rw-r--r--   0 jnyiri     (501) staff       (20)     8467 2023-07-06 15:42:38.000000 pytapo-3.3.8/pytapo/media_stream/downloader.py
--rw-r--r--   0 jnyiri     (501) staff       (20)      607 2023-04-19 11:02:05.000000 pytapo-3.3.8/pytapo/media_stream/error.py
--rw-r--r--   0 jnyiri     (501) staff       (20)     3264 2023-10-06 13:15:15.000000 pytapo-3.3.8/pytapo/media_stream/pes.py
--rw-r--r--   0 jnyiri     (501) staff       (20)      659 2023-04-19 11:02:05.000000 pytapo-3.3.8/pytapo/media_stream/response.py
--rw-r--r--   0 jnyiri     (501) staff       (20)    19229 2023-04-19 11:02:05.000000 pytapo-3.3.8/pytapo/media_stream/session.py
--rw-r--r--   0 jnyiri     (501) staff       (20)     5222 2023-04-19 11:02:05.000000 pytapo-3.3.8/pytapo/media_stream/tsReader.py
--rw-r--r--   0 jnyiri     (501) staff       (20)       25 2023-11-15 10:14:48.000000 pytapo-3.3.8/pytapo/version.py
-drwxr-xr-x   0 jnyiri     (501) staff       (20)        0 2023-11-15 10:14:48.283659 pytapo-3.3.8/pytapo.egg-info/
--rw-r--r--   0 jnyiri     (501) staff       (20)     5533 2023-11-15 10:14:48.000000 pytapo-3.3.8/pytapo.egg-info/PKG-INFO
--rw-r--r--   0 jnyiri     (501) staff       (20)      569 2023-11-15 10:14:48.000000 pytapo-3.3.8/pytapo.egg-info/SOURCES.txt
--rw-r--r--   0 jnyiri     (501) staff       (20)        1 2023-11-15 10:14:48.000000 pytapo-3.3.8/pytapo.egg-info/dependency_links.txt
--rw-r--r--   0 jnyiri     (501) staff       (20)       34 2023-11-15 10:14:48.000000 pytapo-3.3.8/pytapo.egg-info/requires.txt
--rw-r--r--   0 jnyiri     (501) staff       (20)        7 2023-11-15 10:14:48.000000 pytapo-3.3.8/pytapo.egg-info/top_level.txt
--rw-r--r--   0 jnyiri     (501) staff       (20)       38 2023-11-15 10:14:48.286427 pytapo-3.3.8/setup.cfg
--rw-r--r--   0 jnyiri     (501) staff       (20)      778 2023-11-15 10:09:09.000000 pytapo-3.3.8/setup.py
+drwxr-xr-x   0 jnyiri     (501) staff       (20)        0 2023-11-15 10:47:40.646231 pytapo-3.3.9/
+-rw-r--r--   0 jnyiri     (501) staff       (20)     1069 2023-04-19 11:02:05.000000 pytapo-3.3.9/LICENSE
+-rw-r--r--   0 jnyiri     (501) staff       (20)       16 2023-04-19 11:02:05.000000 pytapo-3.3.9/MANIFEST.in
+-rw-r--r--   0 jnyiri     (501) staff       (20)     5533 2023-11-15 10:47:40.646123 pytapo-3.3.9/PKG-INFO
+-rw-r--r--   0 jnyiri     (501) staff       (20)     5076 2023-04-19 11:02:05.000000 pytapo-3.3.9/README.md
+drwxr-xr-x   0 jnyiri     (501) staff       (20)        0 2023-11-15 10:47:40.642946 pytapo-3.3.9/pytapo/
+-rw-r--r--   0 jnyiri     (501) staff       (20)      747 2023-08-21 10:42:21.000000 pytapo-3.3.9/pytapo/TlsAdapter.py
+-rw-r--r--   0 jnyiri     (501) staff       (20)    64538 2023-11-15 10:46:52.000000 pytapo-3.3.9/pytapo/__init__.py
+-rw-r--r--   0 jnyiri     (501) staff       (20)      614 2023-11-15 10:47:28.000000 pytapo-3.3.9/pytapo/const.py
+drwxr-xr-x   0 jnyiri     (501) staff       (20)        0 2023-11-15 10:47:40.645902 pytapo-3.3.9/pytapo/media_stream/
+-rw-r--r--   0 jnyiri     (501) staff       (20)        0 2023-04-19 11:02:05.000000 pytapo-3.3.9/pytapo/media_stream/__init__.py
+-rw-r--r--   0 jnyiri     (501) staff       (20)     1977 2023-04-19 11:02:05.000000 pytapo-3.3.9/pytapo/media_stream/_utils.py
+-rw-r--r--   0 jnyiri     (501) staff       (20)     4346 2023-05-04 14:22:22.000000 pytapo-3.3.9/pytapo/media_stream/convert.py
+-rw-r--r--   0 jnyiri     (501) staff       (20)     2626 2023-04-19 11:02:05.000000 pytapo-3.3.9/pytapo/media_stream/crypto.py
+-rw-r--r--   0 jnyiri     (501) staff       (20)     8467 2023-07-06 15:42:38.000000 pytapo-3.3.9/pytapo/media_stream/downloader.py
+-rw-r--r--   0 jnyiri     (501) staff       (20)      607 2023-04-19 11:02:05.000000 pytapo-3.3.9/pytapo/media_stream/error.py
+-rw-r--r--   0 jnyiri     (501) staff       (20)     3264 2023-10-06 13:15:15.000000 pytapo-3.3.9/pytapo/media_stream/pes.py
+-rw-r--r--   0 jnyiri     (501) staff       (20)      659 2023-04-19 11:02:05.000000 pytapo-3.3.9/pytapo/media_stream/response.py
+-rw-r--r--   0 jnyiri     (501) staff       (20)    19229 2023-04-19 11:02:05.000000 pytapo-3.3.9/pytapo/media_stream/session.py
+-rw-r--r--   0 jnyiri     (501) staff       (20)     5222 2023-04-19 11:02:05.000000 pytapo-3.3.9/pytapo/media_stream/tsReader.py
+-rw-r--r--   0 jnyiri     (501) staff       (20)       25 2023-11-15 10:47:40.000000 pytapo-3.3.9/pytapo/version.py
+drwxr-xr-x   0 jnyiri     (501) staff       (20)        0 2023-11-15 10:47:40.643505 pytapo-3.3.9/pytapo.egg-info/
+-rw-r--r--   0 jnyiri     (501) staff       (20)     5533 2023-11-15 10:47:40.000000 pytapo-3.3.9/pytapo.egg-info/PKG-INFO
+-rw-r--r--   0 jnyiri     (501) staff       (20)      569 2023-11-15 10:47:40.000000 pytapo-3.3.9/pytapo.egg-info/SOURCES.txt
+-rw-r--r--   0 jnyiri     (501) staff       (20)        1 2023-11-15 10:47:40.000000 pytapo-3.3.9/pytapo.egg-info/dependency_links.txt
+-rw-r--r--   0 jnyiri     (501) staff       (20)       34 2023-11-15 10:47:40.000000 pytapo-3.3.9/pytapo.egg-info/requires.txt
+-rw-r--r--   0 jnyiri     (501) staff       (20)        7 2023-11-15 10:47:40.000000 pytapo-3.3.9/pytapo.egg-info/top_level.txt
+-rw-r--r--   0 jnyiri     (501) staff       (20)       38 2023-11-15 10:47:40.646276 pytapo-3.3.9/setup.cfg
+-rw-r--r--   0 jnyiri     (501) staff       (20)      778 2023-11-15 10:47:35.000000 pytapo-3.3.9/setup.py
```

### Comparing `pytapo-3.3.8/LICENSE` & `pytapo-3.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytapo-3.3.8/PKG-INFO` & `pytapo-3.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytapo
-Version: 3.3.8
+Version: 3.3.9
 Summary: Python library for communication with Tapo Cameras
 Home-page: https://github.com/JurajNyiri/pytapo
 Author: Juraj Nyíri
 Author-email: juraj.nyiri@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytapo-3.3.8/README.md` & `pytapo-3.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pytapo-3.3.8/pytapo/TlsAdapter.py` & `pytapo-3.3.9/pytapo/TlsAdapter.py`

 * *Files identical despite different names*

### Comparing `pytapo-3.3.8/pytapo/__init__.py` & `pytapo-3.3.9/pytapo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -488,35 +488,44 @@
             "POST",
             url,
             data=json.dumps(fullRequest),
             headers=self.headers,
             verify=False,
         )
         responseData = res.json()
+        authValid = True
         if (
             self.isSecureConnection()
             and "result" in responseData
             and "response" in responseData["result"]
         ):
             encryptedResponse = responseData["result"]["response"]
             encryptedResponse = base64.b64decode(responseData["result"]["response"])
-            responseJSON = json.loads(self.decryptResponse(encryptedResponse))
+            try:
+                responseJSON = json.loads(self.decryptResponse(encryptedResponse))
+            except Exception as err:
+                if str(err) == "Padding is incorrect.":
+                    authValid = False
+                else:
+                    raise err
         else:
             responseJSON = res.json()
-        if not self.responseIsOK(res, responseJSON):
+        if not authValid or not self.responseIsOK(res, responseJSON):
             #  -40401: Invalid Stok
             if (
-                responseJSON
-                and "error_code" in responseJSON
-                and (
-                    responseJSON["error_code"] == -40401
-                    or responseJSON["error_code"] == -1
+                not authValid
+                or (
+                    responseJSON
+                    and "error_code" in responseJSON
+                    and (
+                        responseJSON["error_code"] == -40401
+                        or responseJSON["error_code"] == -1
+                    )
                 )
-                and loginRetryCount < MAX_LOGIN_RETRIES
-            ):
+            ) and loginRetryCount < MAX_LOGIN_RETRIES:
                 self.refreshStok()
                 return self.performRequest(requestData, loginRetryCount + 1)
             else:
                 raise Exception(
                     "Error: {}, Response: {}".format(
                         self.getErrorMessage(responseJSON["error_code"]),
                         json.dumps(responseJSON),
```

### Comparing `pytapo-3.3.8/pytapo/const.py` & `pytapo-3.3.9/pytapo/const.py`

 * *Files identical despite different names*

### Comparing `pytapo-3.3.8/pytapo/media_stream/_utils.py` & `pytapo-3.3.9/pytapo/media_stream/_utils.py`

 * *Files identical despite different names*

### Comparing `pytapo-3.3.8/pytapo/media_stream/convert.py` & `pytapo-3.3.9/pytapo/media_stream/convert.py`

 * *Files identical despite different names*

### Comparing `pytapo-3.3.8/pytapo/media_stream/crypto.py` & `pytapo-3.3.9/pytapo/media_stream/crypto.py`

 * *Files identical despite different names*

### Comparing `pytapo-3.3.8/pytapo/media_stream/downloader.py` & `pytapo-3.3.9/pytapo/media_stream/downloader.py`

 * *Files identical despite different names*

### Comparing `pytapo-3.3.8/pytapo/media_stream/error.py` & `pytapo-3.3.9/pytapo/media_stream/error.py`

 * *Files identical despite different names*

### Comparing `pytapo-3.3.8/pytapo/media_stream/pes.py` & `pytapo-3.3.9/pytapo/media_stream/pes.py`

 * *Files identical despite different names*

### Comparing `pytapo-3.3.8/pytapo/media_stream/response.py` & `pytapo-3.3.9/pytapo/media_stream/response.py`

 * *Files identical despite different names*

### Comparing `pytapo-3.3.8/pytapo/media_stream/session.py` & `pytapo-3.3.9/pytapo/media_stream/session.py`

 * *Files identical despite different names*

### Comparing `pytapo-3.3.8/pytapo/media_stream/tsReader.py` & `pytapo-3.3.9/pytapo/media_stream/tsReader.py`

 * *Files identical despite different names*

### Comparing `pytapo-3.3.8/pytapo.egg-info/PKG-INFO` & `pytapo-3.3.9/pytapo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytapo
-Version: 3.3.8
+Version: 3.3.9
 Summary: Python library for communication with Tapo Cameras
 Home-page: https://github.com/JurajNyiri/pytapo
 Author: Juraj Nyíri
 Author-email: juraj.nyiri@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytapo-3.3.8/pytapo.egg-info/SOURCES.txt` & `pytapo-3.3.9/pytapo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytapo-3.3.8/setup.py` & `pytapo-3.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytapo",
-    version="3.3.8",
+    version="3.3.9",
     author="Juraj Nyíri",
     author_email="juraj.nyiri@gmail.com",
     description="Python library for communication with Tapo Cameras",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JurajNyiri/pytapo",
```

