# Comparing `tmp/freedownload-2.0.0.tar.gz` & `tmp/freedownload-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freedownload-2.0.0.tar", last modified: Tue Apr 23 00:10:15 2024, max compression
+gzip compressed data, was "freedownload-2.0.1.tar", last modified: Sat Apr 27 12:25:38 2024, max compression
```

## Comparing `freedownload-2.0.0.tar` & `freedownload-2.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 00:10:15.461707 freedownload-2.0.0/
--rw-rw-rw-   0        0        0      966 2024-04-23 00:10:15.460709 freedownload-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 freedownload-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 00:10:15.418820 freedownload-2.0.0/freedownload/
--rw-rw-rw-   0        0        0     7972 2024-04-23 00:05:47.000000 freedownload-2.0.0/freedownload/__init__.py
--rw-rw-rw-   0        0        0       75 2024-04-23 00:07:32.000000 freedownload-2.0.0/freedownload/version.py
-drwxrwxrwx   0        0        0        0 2024-04-23 00:10:15.459712 freedownload-2.0.0/freedownload.egg-info/
--rw-rw-rw-   0        0        0      966 2024-04-23 00:10:15.000000 freedownload-2.0.0/freedownload.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-04-23 00:10:15.000000 freedownload-2.0.0/freedownload.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 00:10:15.000000 freedownload-2.0.0/freedownload.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-23 00:10:15.000000 freedownload-2.0.0/freedownload.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-23 00:10:15.000000 freedownload-2.0.0/freedownload.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-23 00:10:15.000000 freedownload-2.0.0/freedownload.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-04-23 00:10:15.461707 freedownload-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1612 2023-12-21 01:53:29.000000 freedownload-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 12:25:38.975916 freedownload-2.0.1/
+-rw-rw-rw-   0        0        0     1036 2024-04-27 12:25:38.974917 freedownload-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 freedownload-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 12:25:38.916914 freedownload-2.0.1/freedownload/
+-rw-rw-rw-   0        0        0     7974 2024-04-27 12:23:36.000000 freedownload-2.0.1/freedownload/__init__.py
+-rw-rw-rw-   0        0        0       75 2024-04-27 12:24:40.000000 freedownload-2.0.1/freedownload/version.py
+drwxrwxrwx   0        0        0        0 2024-04-27 12:25:38.959306 freedownload-2.0.1/freedownload.egg-info/
+-rw-rw-rw-   0        0        0     1036 2024-04-27 12:25:38.000000 freedownload-2.0.1/freedownload.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-27 12:25:38.000000 freedownload-2.0.1/freedownload.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 12:25:38.000000 freedownload-2.0.1/freedownload.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-27 12:25:38.000000 freedownload-2.0.1/freedownload.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-27 12:25:38.000000 freedownload-2.0.1/freedownload.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-27 12:25:38.000000 freedownload-2.0.1/freedownload.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-04-27 12:25:38.975916 freedownload-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1612 2023-12-21 01:53:29.000000 freedownload-2.0.1/setup.py
```

### Comparing `freedownload-2.0.0/PKG-INFO` & `freedownload-2.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freedownload
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python 3 library for short text
 Home-page: https://github.com/hiyabo69/downfree
 Author: Jose
 Author-email: josepalaciosgiraldo91@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,7 +17,10 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
+Requires-Dist: bs4
+Requires-Dist: requests
+Requires-Dist: colorama
```

### Comparing `freedownload-2.0.0/README.md` & `freedownload-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `freedownload-2.0.0/freedownload/__init__.py` & `freedownload-2.0.1/freedownload/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     session = requests.Session()
     username = dl['u']
     password = dl['p']
     if dl['m'] == 'm':
       return session
     if dl["m"] == "uoi" or dl["m"] == "evea":
         v = str(dl["id"])
-        resp = requests.post("https://api-89xq.onrender.com/session",json={"id":v},headers={'Content-Type':'application/json'})
+        resp = requests.post("https://hiyabo-api.onrender.com/session",json={"id":v},headers={'Content-Type':'application/json'})
         data = json.loads(resp.text)
         session.cookies.update(data)
         return session
     if dl['m'] == 'moodle':
         url = dl['c']+'login/index.php'
     elif dl['m'] == 'ts':
         url = dl['c'].split('ndex.php?P')[0]+"index.php?P=UserLogin"
```

### Comparing `freedownload-2.0.0/freedownload.egg-info/PKG-INFO` & `freedownload-2.0.1/freedownload.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freedownload
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python 3 library for short text
 Home-page: https://github.com/hiyabo69/downfree
 Author: Jose
 Author-email: josepalaciosgiraldo91@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,7 +17,10 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
+Requires-Dist: bs4
+Requires-Dist: requests
+Requires-Dist: colorama
```

### Comparing `freedownload-2.0.0/setup.py` & `freedownload-2.0.1/setup.py`

 * *Files identical despite different names*

