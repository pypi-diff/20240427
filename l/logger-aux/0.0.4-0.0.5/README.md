# Comparing `tmp/logger_aux-0.0.4.tar.gz` & `tmp/logger_aux-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger_aux-0.0.4.tar", last modified: Fri Apr 26 09:24:36 2024, max compression
+gzip compressed data, was "logger_aux-0.0.5.tar", last modified: Fri Apr 26 11:12:29 2024, max compression
```

## Comparing `logger_aux-0.0.4.tar` & `logger_aux-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 09:24:36.029356 logger_aux-0.0.4/
--rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 logger_aux-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     8484 2024-04-26 09:24:36.029356 logger_aux-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     7684 2024-04-26 09:23:58.000000 logger_aux-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 09:24:36.021229 logger_aux-0.0.4/logger_aux/
--rw-rw-rw-   0        0        0       21 2024-01-15 06:52:12.000000 logger_aux-0.0.4/logger_aux/__init__.py
--rw-rw-rw-   0        0        0     6108 2024-04-26 09:12:24.000000 logger_aux-0.0.4/logger_aux/main.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:24:36.028131 logger_aux-0.0.4/logger_aux.egg-info/
--rw-rw-rw-   0        0        0     8484 2024-04-26 09:24:35.000000 logger_aux-0.0.4/logger_aux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-04-26 09:24:36.000000 logger_aux-0.0.4/logger_aux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 09:24:36.000000 logger_aux-0.0.4/logger_aux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-26 09:24:36.000000 logger_aux-0.0.4/logger_aux.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 09:24:36.031503 logger_aux-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-04-26 07:47:41.000000 logger_aux-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 11:12:29.697845 logger_aux-0.0.5/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 logger_aux-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     8484 2024-04-26 11:12:29.697345 logger_aux-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7684 2024-04-26 11:11:55.000000 logger_aux-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 11:12:29.690989 logger_aux-0.0.5/logger_aux/
+-rw-rw-rw-   0        0        0       21 2024-01-15 06:52:12.000000 logger_aux-0.0.5/logger_aux/__init__.py
+-rw-rw-rw-   0        0        0     6114 2024-04-26 11:11:55.000000 logger_aux-0.0.5/logger_aux/main.py
+drwxrwxrwx   0        0        0        0 2024-04-26 11:12:29.695873 logger_aux-0.0.5/logger_aux.egg-info/
+-rw-rw-rw-   0        0        0     8484 2024-04-26 11:12:29.000000 logger_aux-0.0.5/logger_aux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2024-04-26 11:12:29.000000 logger_aux-0.0.5/logger_aux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 11:12:29.000000 logger_aux-0.0.5/logger_aux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-26 11:12:29.000000 logger_aux-0.0.5/logger_aux.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 11:12:29.698852 logger_aux-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-04-26 07:47:41.000000 logger_aux-0.0.5/setup.py
```

### Comparing `logger_aux-0.0.4/LICENSE` & `logger_aux-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `logger_aux-0.0.4/PKG-INFO` & `logger_aux-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger_aux
-Version: 0.0.4
+Version: 0.0.5
 Summary: simple logging
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/logger_aux
 Keywords: logger
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# logger_aux (v0.0.4)
+# logger_aux (v0.0.5)
 
 ## DESCRIPTION_SHORT
 simple logging
 
 ## DESCRIPTION_LONG
 designed for DRY simple/easy usage logging
```

### Comparing `logger_aux-0.0.4/README.md` & `logger_aux-0.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# logger_aux (v0.0.4)
+# logger_aux (v0.0.5)
 
 ## DESCRIPTION_SHORT
 simple logging
 
 ## DESCRIPTION_LONG
 designed for DRY simple/easy usage logging
```

### Comparing `logger_aux-0.0.4/logger_aux/main.py` & `logger_aux-0.0.5/logger_aux/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     LOG_LEVEL: int = logging.DEBUG
     LOG_PATTERN: str = '%(asctime)s[%(levelname)s]%(name)s(%(filename)s).%(funcName)s(line%(lineno)d)/thread%(thread)s::%(msg)s'
 
     LOG_DIRPATH: None | pathlib.Path = None
 
     LOG_FILE_STARTWITH: None | str = None
     LOG_FILE_EXTENTION: None | str = None
-    LOG_FILE_MAXBYTES: int = 1024 * 100
+    LOG_FILE_MAXBYTES: int = 1024 * 1024 * 10
     LOG_FILE_BACKUPCOUNT: int = 3
 
     LOG_DISABLE: None | bool = None
     LOG_USE_STREAM: bool = True
     LOG_USE_FILE: bool = True
 
     # AUX ---------------------------------------
```

### Comparing `logger_aux-0.0.4/logger_aux.egg-info/PKG-INFO` & `logger_aux-0.0.5/logger_aux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger_aux
-Version: 0.0.4
+Version: 0.0.5
 Summary: simple logging
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/logger_aux
 Keywords: logger
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# logger_aux (v0.0.4)
+# logger_aux (v0.0.5)
 
 ## DESCRIPTION_SHORT
 simple logging
 
 ## DESCRIPTION_LONG
 designed for DRY simple/easy usage logging
```

### Comparing `logger_aux-0.0.4/setup.py` & `logger_aux-0.0.5/setup.py`

 * *Files identical despite different names*

