# Comparing `tmp/datafusion_stubs-0.0.2.tar.gz` & `tmp/datafusion_stubs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafusion_stubs-0.0.2.tar", last modified: Sat Apr 27 16:55:14 2024, max compression
+gzip compressed data, was "datafusion_stubs-0.0.3.tar", last modified: Sat Apr 27 17:25:12 2024, max compression
```

## Comparing `datafusion_stubs-0.0.2.tar` & `datafusion_stubs-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,19 @@
-drwxrwxr-x   0 reda      (1000) reda      (1000)        0 2024-04-27 16:55:14.765754 datafusion_stubs-0.0.2/
--rw-rw-r--   0 reda      (1000) reda      (1000)    11357 2024-04-27 12:54:42.000000 datafusion_stubs-0.0.2/LICENSE
--rw-rw-r--   0 reda      (1000) reda      (1000)      809 2024-04-27 16:55:14.765754 datafusion_stubs-0.0.2/PKG-INFO
--rw-rw-r--   0 reda      (1000) reda      (1000)      406 2024-04-27 16:36:20.000000 datafusion_stubs-0.0.2/README.md
-drwxrwxr-x   0 reda      (1000) reda      (1000)        0 2024-04-27 16:55:14.765754 datafusion_stubs-0.0.2/datafusion_stubs.egg-info/
--rw-rw-r--   0 reda      (1000) reda      (1000)      809 2024-04-27 16:55:14.000000 datafusion_stubs-0.0.2/datafusion_stubs.egg-info/PKG-INFO
--rw-rw-r--   0 reda      (1000) reda      (1000)      196 2024-04-27 16:55:14.000000 datafusion_stubs-0.0.2/datafusion_stubs.egg-info/SOURCES.txt
--rw-rw-r--   0 reda      (1000) reda      (1000)        1 2024-04-27 16:55:14.000000 datafusion_stubs-0.0.2/datafusion_stubs.egg-info/dependency_links.txt
--rw-rw-r--   0 reda      (1000) reda      (1000)       17 2024-04-27 16:55:14.000000 datafusion_stubs-0.0.2/datafusion_stubs.egg-info/top_level.txt
--rw-rw-r--   0 reda      (1000) reda      (1000)      501 2024-04-27 16:55:14.765754 datafusion_stubs-0.0.2/setup.cfg
--rw-rw-r--   0 reda      (1000) reda      (1000)      107 2024-04-27 15:19:50.000000 datafusion_stubs-0.0.2/setup.py
+drwxrwxr-x   0 reda      (1000) reda      (1000)        0 2024-04-27 17:25:12.641801 datafusion_stubs-0.0.3/
+-rw-rw-r--   0 reda      (1000) reda      (1000)    11357 2024-04-27 12:54:42.000000 datafusion_stubs-0.0.3/LICENSE
+-rw-r--r--   0 reda      (1000) reda      (1000)      789 2024-04-27 17:25:12.637802 datafusion_stubs-0.0.3/PKG-INFO
+-rw-rw-r--   0 reda      (1000) reda      (1000)      406 2024-04-27 16:36:20.000000 datafusion_stubs-0.0.3/README.md
+drwxrwxr-x   0 reda      (1000) reda      (1000)        0 2024-04-27 17:25:12.637802 datafusion_stubs-0.0.3/datafusion-stubs/
+-rw-rw-r--   0 reda      (1000) reda      (1000)     1196 2024-04-27 14:29:18.000000 datafusion_stubs-0.0.3/datafusion-stubs/__init__.pyi
+-rw-rw-r--   0 reda      (1000) reda      (1000)      729 2024-04-27 12:54:53.000000 datafusion_stubs-0.0.3/datafusion-stubs/common.pyi
+-rw-rw-r--   0 reda      (1000) reda      (1000)     3597 2024-04-27 12:54:53.000000 datafusion_stubs-0.0.3/datafusion-stubs/expr.pyi
+-rw-rw-r--   0 reda      (1000) reda      (1000)    13450 2024-04-27 15:19:50.000000 datafusion_stubs-0.0.3/datafusion-stubs/functions.pyi
+-rw-rw-r--   0 reda      (1000) reda      (1000)      272 2024-04-27 13:12:08.000000 datafusion_stubs-0.0.3/datafusion-stubs/object_store.pyi
+-rw-rw-r--   0 reda      (1000) reda      (1000)        0 2024-04-27 12:54:53.000000 datafusion_stubs-0.0.3/datafusion-stubs/py.typed
+-rw-rw-r--   0 reda      (1000) reda      (1000)      242 2024-04-27 12:54:53.000000 datafusion_stubs-0.0.3/datafusion-stubs/substrait.pyi
+drwxrwxr-x   0 reda      (1000) reda      (1000)        0 2024-04-27 17:25:12.637802 datafusion_stubs-0.0.3/datafusion_stubs.egg-info/
+-rw-r--r--   0 reda      (1000) reda      (1000)      789 2024-04-27 17:25:12.000000 datafusion_stubs-0.0.3/datafusion_stubs.egg-info/PKG-INFO
+-rw-rw-r--   0 reda      (1000) reda      (1000)      402 2024-04-27 17:25:12.000000 datafusion_stubs-0.0.3/datafusion_stubs.egg-info/SOURCES.txt
+-rw-rw-r--   0 reda      (1000) reda      (1000)        1 2024-04-27 17:25:12.000000 datafusion_stubs-0.0.3/datafusion_stubs.egg-info/dependency_links.txt
+-rw-rw-r--   0 reda      (1000) reda      (1000)       17 2024-04-27 17:25:12.000000 datafusion_stubs-0.0.3/datafusion_stubs.egg-info/top_level.txt
+-rw-rw-r--   0 reda      (1000) reda      (1000)      555 2024-04-27 17:25:12.641801 datafusion_stubs-0.0.3/setup.cfg
+-rw-rw-r--   0 reda      (1000) reda      (1000)      107 2024-04-27 17:22:23.000000 datafusion_stubs-0.0.3/setup.py
```

### Comparing `datafusion_stubs-0.0.2/LICENSE` & `datafusion_stubs-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datafusion_stubs-0.0.2/PKG-INFO` & `datafusion_stubs-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: datafusion_stubs
-Version: 0.0.2
+Version: 0.0.3
 Summary: PEP 561 type stubs for Apache DataFusion Python Bindings
 Home-page: https://github.com/3ok/datafusion-stubs
 Author: Reda Bouaida
 Author-email: reda.bouaida@outlook.com
 License: Apache-2.0
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # datafusion-stubs
 
 **Note: This project is still in very early work-in-progress (WIP) stage.**
@@ -23,9 +22,7 @@
 This packages aims to provide type stubs for [DataFusion Python bindings](https://github.com/apache/datafusion-python).
 
 ## Install
 
 ```shell
 $ pip install datafusion-stubs
 ```
-
-
```

### Comparing `datafusion_stubs-0.0.2/datafusion_stubs.egg-info/PKG-INFO` & `datafusion_stubs-0.0.3/datafusion_stubs.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: datafusion-stubs
-Version: 0.0.2
+Version: 0.0.3
 Summary: PEP 561 type stubs for Apache DataFusion Python Bindings
 Home-page: https://github.com/3ok/datafusion-stubs
 Author: Reda Bouaida
 Author-email: reda.bouaida@outlook.com
 License: Apache-2.0
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # datafusion-stubs
 
 **Note: This project is still in very early work-in-progress (WIP) stage.**
@@ -23,9 +22,7 @@
 This packages aims to provide type stubs for [DataFusion Python bindings](https://github.com/apache/datafusion-python).
 
 ## Install
 
 ```shell
 $ pip install datafusion-stubs
 ```
-
-
```

