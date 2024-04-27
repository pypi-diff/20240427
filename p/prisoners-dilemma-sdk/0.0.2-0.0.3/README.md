# Comparing `tmp/prisoners_dilemma_sdk-0.0.2.tar.gz` & `tmp/prisoners_dilemma_sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prisoners_dilemma_sdk-0.0.2.tar", last modified: Sat Apr 27 16:05:19 2024, max compression
+gzip compressed data, was "prisoners_dilemma_sdk-0.0.3.tar", last modified: Sat Apr 27 16:21:58 2024, max compression
```

## Comparing `prisoners_dilemma_sdk-0.0.2.tar` & `prisoners_dilemma_sdk-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:05:19.345687 prisoners_dilemma_sdk-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-27 16:05:19.345687 prisoners_dilemma_sdk-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-27 16:05:16.000000 prisoners_dilemma_sdk-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:05:19.345687 prisoners_dilemma_sdk-0.0.2/prisoners_dilemma_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 16:05:16.000000 prisoners_dilemma_sdk-0.0.2/prisoners_dilemma_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-27 16:05:16.000000 prisoners_dilemma_sdk-0.0.2/prisoners_dilemma_sdk/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:05:19.345687 prisoners_dilemma_sdk-0.0.2/prisoners_dilemma_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-27 16:05:19.000000 prisoners_dilemma_sdk-0.0.2/prisoners_dilemma_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-27 16:05:19.000000 prisoners_dilemma_sdk-0.0.2/prisoners_dilemma_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:05:19.000000 prisoners_dilemma_sdk-0.0.2/prisoners_dilemma_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 16:05:19.000000 prisoners_dilemma_sdk-0.0.2/prisoners_dilemma_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 16:05:19.345687 prisoners_dilemma_sdk-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-27 16:05:16.000000 prisoners_dilemma_sdk-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:21:58.587647 prisoners_dilemma_sdk-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-27 16:21:58.587647 prisoners_dilemma_sdk-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-27 16:21:55.000000 prisoners_dilemma_sdk-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:21:58.587647 prisoners_dilemma_sdk-0.0.3/prisoners_dilemma_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 16:21:55.000000 prisoners_dilemma_sdk-0.0.3/prisoners_dilemma_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-27 16:21:55.000000 prisoners_dilemma_sdk-0.0.3/prisoners_dilemma_sdk/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:21:58.587647 prisoners_dilemma_sdk-0.0.3/prisoners_dilemma_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-27 16:21:58.000000 prisoners_dilemma_sdk-0.0.3/prisoners_dilemma_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-27 16:21:58.000000 prisoners_dilemma_sdk-0.0.3/prisoners_dilemma_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:21:58.000000 prisoners_dilemma_sdk-0.0.3/prisoners_dilemma_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 16:21:58.000000 prisoners_dilemma_sdk-0.0.3/prisoners_dilemma_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 16:21:58.587647 prisoners_dilemma_sdk-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-27 16:21:55.000000 prisoners_dilemma_sdk-0.0.3/setup.py
```

### Comparing `prisoners_dilemma_sdk-0.0.2/PKG-INFO` & `prisoners_dilemma_sdk-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prisoners-dilemma-sdk
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://github.com/youssef-attai/prisoners-dilemma-sdk
 Author: Youssef Atta'i
 Author-email: youssefjattai@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/youssef-attai/prisoners-dilemma-sdk
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `prisoners_dilemma_sdk-0.0.2/prisoners_dilemma_sdk.egg-info/PKG-INFO` & `prisoners_dilemma_sdk-0.0.3/prisoners_dilemma_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prisoners-dilemma-sdk
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://github.com/youssef-attai/prisoners-dilemma-sdk
 Author: Youssef Atta'i
 Author-email: youssefjattai@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/youssef-attai/prisoners-dilemma-sdk
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `prisoners_dilemma_sdk-0.0.2/setup.py` & `prisoners_dilemma_sdk-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 NAME = "prisoners-dilemma-sdk"
 
 INSTALL_REQUIRES = []
 
 
 setuptools.setup(
```

