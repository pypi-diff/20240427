# Comparing `tmp/prisoners_dilemma_sdk-0.0.3.tar.gz` & `tmp/prisoners_dilemma_sdk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prisoners_dilemma_sdk-0.0.3.tar", last modified: Sat Apr 27 16:21:58 2024, max compression
+gzip compressed data, was "prisoners_dilemma_sdk-0.0.4.tar", last modified: Sat Apr 27 16:34:11 2024, max compression
```

## Comparing `prisoners_dilemma_sdk-0.0.3.tar` & `prisoners_dilemma_sdk-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:21:58.587647 prisoners_dilemma_sdk-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-27 16:21:58.587647 prisoners_dilemma_sdk-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-27 16:21:55.000000 prisoners_dilemma_sdk-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:21:58.587647 prisoners_dilemma_sdk-0.0.3/prisoners_dilemma_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 16:21:55.000000 prisoners_dilemma_sdk-0.0.3/prisoners_dilemma_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-27 16:21:55.000000 prisoners_dilemma_sdk-0.0.3/prisoners_dilemma_sdk/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:21:58.587647 prisoners_dilemma_sdk-0.0.3/prisoners_dilemma_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-27 16:21:58.000000 prisoners_dilemma_sdk-0.0.3/prisoners_dilemma_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-27 16:21:58.000000 prisoners_dilemma_sdk-0.0.3/prisoners_dilemma_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:21:58.000000 prisoners_dilemma_sdk-0.0.3/prisoners_dilemma_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 16:21:58.000000 prisoners_dilemma_sdk-0.0.3/prisoners_dilemma_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 16:21:58.587647 prisoners_dilemma_sdk-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-27 16:21:55.000000 prisoners_dilemma_sdk-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:34:11.957325 prisoners_dilemma_sdk-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-27 16:34:11.957325 prisoners_dilemma_sdk-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-27 16:34:07.000000 prisoners_dilemma_sdk-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:34:11.957325 prisoners_dilemma_sdk-0.0.4/prisoners_dilemma_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-27 16:34:07.000000 prisoners_dilemma_sdk-0.0.4/prisoners_dilemma_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-27 16:34:07.000000 prisoners_dilemma_sdk-0.0.4/prisoners_dilemma_sdk/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:34:11.957325 prisoners_dilemma_sdk-0.0.4/prisoners_dilemma_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-27 16:34:11.000000 prisoners_dilemma_sdk-0.0.4/prisoners_dilemma_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-27 16:34:11.000000 prisoners_dilemma_sdk-0.0.4/prisoners_dilemma_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:34:11.000000 prisoners_dilemma_sdk-0.0.4/prisoners_dilemma_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 16:34:11.000000 prisoners_dilemma_sdk-0.0.4/prisoners_dilemma_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 16:34:11.957325 prisoners_dilemma_sdk-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-27 16:34:07.000000 prisoners_dilemma_sdk-0.0.4/setup.py
```

### Comparing `prisoners_dilemma_sdk-0.0.3/PKG-INFO` & `prisoners_dilemma_sdk-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prisoners-dilemma-sdk
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/youssef-attai/prisoners-dilemma-sdk
 Author: Youssef Atta'i
 Author-email: youssefjattai@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/youssef-attai/prisoners-dilemma-sdk
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `prisoners_dilemma_sdk-0.0.3/prisoners_dilemma_sdk.egg-info/PKG-INFO` & `prisoners_dilemma_sdk-0.0.4/prisoners_dilemma_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prisoners-dilemma-sdk
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/youssef-attai/prisoners-dilemma-sdk
 Author: Youssef Atta'i
 Author-email: youssefjattai@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/youssef-attai/prisoners-dilemma-sdk
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `prisoners_dilemma_sdk-0.0.3/setup.py` & `prisoners_dilemma_sdk-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 
 NAME = "prisoners-dilemma-sdk"
 
 INSTALL_REQUIRES = []
 
 
 setuptools.setup(
```

