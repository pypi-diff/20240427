# Comparing `tmp/dynamicwebsite-1.0.1.tar.gz` & `tmp/dynamicwebsite-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamicwebsite-1.0.1.tar", last modified: Mon Apr 22 17:53:54 2024, max compression
+gzip compressed data, was "dynamicwebsite-1.0.2.tar", last modified: Sat Apr 27 15:27:11 2024, max compression
```

## Comparing `dynamicwebsite-1.0.1.tar` & `dynamicwebsite-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:53:54.385927 dynamicwebsite-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-22 17:53:54.385927 dynamicwebsite-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-22 17:53:47.000000 dynamicwebsite-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:53:54.385927 dynamicwebsite-1.0.1/dynamicWebsite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-22 17:53:54.000000 dynamicwebsite-1.0.1/dynamicWebsite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-22 17:53:54.000000 dynamicwebsite-1.0.1/dynamicWebsite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 17:53:54.000000 dynamicwebsite-1.0.1/dynamicWebsite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-22 17:53:54.000000 dynamicwebsite-1.0.1/dynamicWebsite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-22 17:53:54.000000 dynamicwebsite-1.0.1/dynamicWebsite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20556 2024-04-22 17:53:47.000000 dynamicwebsite-1.0.1/dynamicWebsite.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-22 17:53:47.000000 dynamicwebsite-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 17:53:54.385927 dynamicwebsite-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:27:11.032208 dynamicwebsite-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-27 15:27:11.032208 dynamicwebsite-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-27 15:27:06.000000 dynamicwebsite-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:27:11.032208 dynamicwebsite-1.0.2/dynamicWebsite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-27 15:27:11.000000 dynamicwebsite-1.0.2/dynamicWebsite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-27 15:27:11.000000 dynamicwebsite-1.0.2/dynamicWebsite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 15:27:11.000000 dynamicwebsite-1.0.2/dynamicWebsite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-27 15:27:11.000000 dynamicwebsite-1.0.2/dynamicWebsite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-27 15:27:11.000000 dynamicwebsite-1.0.2/dynamicWebsite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20570 2024-04-27 15:27:06.000000 dynamicwebsite-1.0.2/dynamicWebsite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-27 15:27:06.000000 dynamicwebsite-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 15:27:11.032208 dynamicwebsite-1.0.2/setup.cfg
```

### Comparing `dynamicwebsite-1.0.1/PKG-INFO` & `dynamicwebsite-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: dynamicWebsite
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple way to host web server bundled with websocket to send and receive live data, from client to server, and pass live HTML changes from server to client without having to refresh the page.
 Author-email: Bhindi <bhaskarpanja93@gmail.com>, riyapuri0710 <riyapuri0710@gmail.com>
 Project-URL: Homepage, https://github.com/BhaskarPanja93/dynamicWebsite
 Keywords: website,dynamic website,update website,live website,change website,websocket
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: randomisedString
 Requires-Dist: cryptography
 Requires-Dist: Flask
 
-# dynamicWebsite v1.0.1
+# dynamicWebsite v1.0.2
 
 ```pip install dynamicWebsite --upgrade```
 
 ###### <br>A simple way to host web server bundled with websocket to send and receive live data, from client to server, and pass live HTML changes from server to client without having to refresh the page."
 
 <br>To install: 
 ```
```

### Comparing `dynamicwebsite-1.0.1/README.md` & `dynamicwebsite-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# dynamicWebsite v1.0.1
+# dynamicWebsite v1.0.2
 
 ```pip install dynamicWebsite --upgrade```
 
 ###### <br>A simple way to host web server bundled with websocket to send and receive live data, from client to server, and pass live HTML changes from server to client without having to refresh the page."
 
 <br>To install: 
 ```
```

### Comparing `dynamicwebsite-1.0.1/dynamicWebsite.egg-info/PKG-INFO` & `dynamicwebsite-1.0.2/dynamicWebsite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: dynamicWebsite
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple way to host web server bundled with websocket to send and receive live data, from client to server, and pass live HTML changes from server to client without having to refresh the page.
 Author-email: Bhindi <bhaskarpanja93@gmail.com>, riyapuri0710 <riyapuri0710@gmail.com>
 Project-URL: Homepage, https://github.com/BhaskarPanja93/dynamicWebsite
 Keywords: website,dynamic website,update website,live website,change website,websocket
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: randomisedString
 Requires-Dist: cryptography
 Requires-Dist: Flask
 
-# dynamicWebsite v1.0.1
+# dynamicWebsite v1.0.2
 
 ```pip install dynamicWebsite --upgrade```
 
 ###### <br>A simple way to host web server bundled with websocket to send and receive live data, from client to server, and pass live HTML changes from server to client without having to refresh the page."
 
 <br>To install: 
 ```
```

### Comparing `dynamicwebsite-1.0.1/dynamicWebsite.py` & `dynamicwebsite-1.0.2/dynamicWebsite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 __packagename__ = "dynamicWebsite"
 
 
 def updatePackage():
     from time import sleep
     from json import loads
     import http.client
@@ -126,15 +126,15 @@
         Read from a request context environ object into current cookie object and return itself
         :param requestObj: the request context to read from
         :return:
         """
         self.remoteAddress = requestObj.remote_addr
         self.UA = requestObj.user_agent.string
         self.hostURL = requestObj.host
-        self.delim = requestObj.headers.get("DELIM")
+        self.delim = requestObj.headers.get("DELIM") or self.delim
         return self
 
     def readAnotherCookie(self, cookie: Cookie) -> Cookie:
         """
         Read from a different cookie object into current cookie object and return itself
         :param cookie: another cookie object of self type
         :return:
```

### Comparing `dynamicwebsite-1.0.1/pyproject.toml` & `dynamicwebsite-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dynamicWebsite"
-version = "1.0.1"
+version = "1.0.2"
 description = "A simple way to host web server bundled with websocket to send and receive live data, from client to server, and pass live HTML changes from server to client without having to refresh the page."
 
 readme = "README.md"
 authors = [{ name = "Bhindi", email = "bhaskarpanja93@gmail.com" },
            { name = "riyapuri0710", email = "riyapuri0710@gmail.com" }]
 
 classifiers = [
```

