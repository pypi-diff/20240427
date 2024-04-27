# Comparing `tmp/datafusion_stubs-0.0.1.tar.gz` & `tmp/datafusion_stubs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafusion_stubs-0.0.1.tar", last modified: Sat Apr 27 16:43:15 2024, max compression
+gzip compressed data, was "datafusion_stubs-0.0.2.tar", last modified: Sat Apr 27 16:55:14 2024, max compression
```

## Comparing `datafusion_stubs-0.0.1.tar` & `datafusion_stubs-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 reda      (1000) reda      (1000)        0 2024-04-27 16:43:15.914250 datafusion_stubs-0.0.1/
--rw-rw-r--   0 reda      (1000) reda      (1000)    11357 2024-04-27 12:54:42.000000 datafusion_stubs-0.0.1/LICENSE
--rw-rw-r--   0 reda      (1000) reda      (1000)      809 2024-04-27 16:43:15.914250 datafusion_stubs-0.0.1/PKG-INFO
--rw-rw-r--   0 reda      (1000) reda      (1000)      406 2024-04-27 16:36:20.000000 datafusion_stubs-0.0.1/README.md
-drwxrwxr-x   0 reda      (1000) reda      (1000)        0 2024-04-27 16:43:15.914250 datafusion_stubs-0.0.1/datafusion_stubs.egg-info/
--rw-rw-r--   0 reda      (1000) reda      (1000)      809 2024-04-27 16:43:15.000000 datafusion_stubs-0.0.1/datafusion_stubs.egg-info/PKG-INFO
--rw-rw-r--   0 reda      (1000) reda      (1000)      196 2024-04-27 16:43:15.000000 datafusion_stubs-0.0.1/datafusion_stubs.egg-info/SOURCES.txt
--rw-rw-r--   0 reda      (1000) reda      (1000)        1 2024-04-27 16:43:15.000000 datafusion_stubs-0.0.1/datafusion_stubs.egg-info/dependency_links.txt
--rw-rw-r--   0 reda      (1000) reda      (1000)       17 2024-04-27 16:43:15.000000 datafusion_stubs-0.0.1/datafusion_stubs.egg-info/top_level.txt
--rw-rw-r--   0 reda      (1000) reda      (1000)      501 2024-04-27 16:43:15.914250 datafusion_stubs-0.0.1/setup.cfg
--rw-rw-r--   0 reda      (1000) reda      (1000)      107 2024-04-27 15:19:50.000000 datafusion_stubs-0.0.1/setup.py
+drwxrwxr-x   0 reda      (1000) reda      (1000)        0 2024-04-27 16:55:14.765754 datafusion_stubs-0.0.2/
+-rw-rw-r--   0 reda      (1000) reda      (1000)    11357 2024-04-27 12:54:42.000000 datafusion_stubs-0.0.2/LICENSE
+-rw-rw-r--   0 reda      (1000) reda      (1000)      809 2024-04-27 16:55:14.765754 datafusion_stubs-0.0.2/PKG-INFO
+-rw-rw-r--   0 reda      (1000) reda      (1000)      406 2024-04-27 16:36:20.000000 datafusion_stubs-0.0.2/README.md
+drwxrwxr-x   0 reda      (1000) reda      (1000)        0 2024-04-27 16:55:14.765754 datafusion_stubs-0.0.2/datafusion_stubs.egg-info/
+-rw-rw-r--   0 reda      (1000) reda      (1000)      809 2024-04-27 16:55:14.000000 datafusion_stubs-0.0.2/datafusion_stubs.egg-info/PKG-INFO
+-rw-rw-r--   0 reda      (1000) reda      (1000)      196 2024-04-27 16:55:14.000000 datafusion_stubs-0.0.2/datafusion_stubs.egg-info/SOURCES.txt
+-rw-rw-r--   0 reda      (1000) reda      (1000)        1 2024-04-27 16:55:14.000000 datafusion_stubs-0.0.2/datafusion_stubs.egg-info/dependency_links.txt
+-rw-rw-r--   0 reda      (1000) reda      (1000)       17 2024-04-27 16:55:14.000000 datafusion_stubs-0.0.2/datafusion_stubs.egg-info/top_level.txt
+-rw-rw-r--   0 reda      (1000) reda      (1000)      501 2024-04-27 16:55:14.765754 datafusion_stubs-0.0.2/setup.cfg
+-rw-rw-r--   0 reda      (1000) reda      (1000)      107 2024-04-27 15:19:50.000000 datafusion_stubs-0.0.2/setup.py
```

### Comparing `datafusion_stubs-0.0.1/LICENSE` & `datafusion_stubs-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datafusion_stubs-0.0.1/PKG-INFO` & `datafusion_stubs-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafusion_stubs
-Version: 0.0.1
+Version: 0.0.2
 Summary: PEP 561 type stubs for Apache DataFusion Python Bindings
 Home-page: https://github.com/3ok/datafusion-stubs
 Author: Reda Bouaida
 Author-email: reda.bouaida@outlook.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `datafusion_stubs-0.0.1/datafusion_stubs.egg-info/PKG-INFO` & `datafusion_stubs-0.0.2/datafusion_stubs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafusion-stubs
-Version: 0.0.1
+Version: 0.0.2
 Summary: PEP 561 type stubs for Apache DataFusion Python Bindings
 Home-page: https://github.com/3ok/datafusion-stubs
 Author: Reda Bouaida
 Author-email: reda.bouaida@outlook.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

