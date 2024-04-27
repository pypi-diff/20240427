# Comparing `tmp/prisoners_dilemma_sdk-0.0.5.tar.gz` & `tmp/prisoners_dilemma_sdk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prisoners_dilemma_sdk-0.0.5.tar", last modified: Sat Apr 27 16:40:50 2024, max compression
+gzip compressed data, was "prisoners_dilemma_sdk-0.0.6.tar", last modified: Sat Apr 27 16:51:57 2024, max compression
```

## Comparing `prisoners_dilemma_sdk-0.0.5.tar` & `prisoners_dilemma_sdk-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:40:50.661763 prisoners_dilemma_sdk-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-27 16:40:50.661763 prisoners_dilemma_sdk-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-27 16:40:45.000000 prisoners_dilemma_sdk-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:40:50.661763 prisoners_dilemma_sdk-0.0.5/prisoners_dilemma_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-27 16:40:45.000000 prisoners_dilemma_sdk-0.0.5/prisoners_dilemma_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-27 16:40:45.000000 prisoners_dilemma_sdk-0.0.5/prisoners_dilemma_sdk/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:40:50.661763 prisoners_dilemma_sdk-0.0.5/prisoners_dilemma_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-27 16:40:50.000000 prisoners_dilemma_sdk-0.0.5/prisoners_dilemma_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-27 16:40:50.000000 prisoners_dilemma_sdk-0.0.5/prisoners_dilemma_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:40:50.000000 prisoners_dilemma_sdk-0.0.5/prisoners_dilemma_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 16:40:50.000000 prisoners_dilemma_sdk-0.0.5/prisoners_dilemma_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 16:40:50.661763 prisoners_dilemma_sdk-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-27 16:40:45.000000 prisoners_dilemma_sdk-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:51:57.333250 prisoners_dilemma_sdk-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-27 16:51:57.333250 prisoners_dilemma_sdk-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-27 16:51:54.000000 prisoners_dilemma_sdk-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:51:57.333250 prisoners_dilemma_sdk-0.0.6/prisoners_dilemma_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-27 16:51:54.000000 prisoners_dilemma_sdk-0.0.6/prisoners_dilemma_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-27 16:51:54.000000 prisoners_dilemma_sdk-0.0.6/prisoners_dilemma_sdk/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:51:57.333250 prisoners_dilemma_sdk-0.0.6/prisoners_dilemma_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-27 16:51:57.000000 prisoners_dilemma_sdk-0.0.6/prisoners_dilemma_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-27 16:51:57.000000 prisoners_dilemma_sdk-0.0.6/prisoners_dilemma_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:51:57.000000 prisoners_dilemma_sdk-0.0.6/prisoners_dilemma_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 16:51:57.000000 prisoners_dilemma_sdk-0.0.6/prisoners_dilemma_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 16:51:57.333250 prisoners_dilemma_sdk-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-27 16:51:54.000000 prisoners_dilemma_sdk-0.0.6/setup.py
```

### Comparing `prisoners_dilemma_sdk-0.0.5/PKG-INFO` & `prisoners_dilemma_sdk-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prisoners-dilemma-sdk
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/youssef-attai/prisoners-dilemma-sdk
 Author: Youssef Atta'i
 Author-email: youssefjattai@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/youssef-attai/prisoners-dilemma-sdk
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `prisoners_dilemma_sdk-0.0.5/prisoners_dilemma_sdk.egg-info/PKG-INFO` & `prisoners_dilemma_sdk-0.0.6/prisoners_dilemma_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prisoners-dilemma-sdk
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/youssef-attai/prisoners-dilemma-sdk
 Author: Youssef Atta'i
 Author-email: youssefjattai@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/youssef-attai/prisoners-dilemma-sdk
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `prisoners_dilemma_sdk-0.0.5/setup.py` & `prisoners_dilemma_sdk-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 
 NAME = "prisoners-dilemma-sdk"
 
 INSTALL_REQUIRES = []
 
 
 setuptools.setup(
```

