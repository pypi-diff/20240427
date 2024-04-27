# Comparing `tmp/prisoners_dilemma_sdk-0.0.1.tar.gz` & `tmp/prisoners_dilemma_sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prisoners_dilemma_sdk-0.0.1.tar", last modified: Sat Apr 27 15:36:39 2024, max compression
+gzip compressed data, was "prisoners_dilemma_sdk-0.0.2.tar", last modified: Sat Apr 27 16:05:19 2024, max compression
```

## Comparing `prisoners_dilemma_sdk-0.0.1.tar` & `prisoners_dilemma_sdk-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:36:39.421901 prisoners_dilemma_sdk-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-27 15:36:39.421901 prisoners_dilemma_sdk-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-27 15:36:36.000000 prisoners_dilemma_sdk-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:36:39.421901 prisoners_dilemma_sdk-0.0.1/prisoners_dilemma_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 15:36:36.000000 prisoners_dilemma_sdk-0.0.1/prisoners_dilemma_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-27 15:36:36.000000 prisoners_dilemma_sdk-0.0.1/prisoners_dilemma_sdk/hello.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:36:39.421901 prisoners_dilemma_sdk-0.0.1/prisoners_dilemma_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-27 15:36:39.000000 prisoners_dilemma_sdk-0.0.1/prisoners_dilemma_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-27 15:36:39.000000 prisoners_dilemma_sdk-0.0.1/prisoners_dilemma_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 15:36:39.000000 prisoners_dilemma_sdk-0.0.1/prisoners_dilemma_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 15:36:39.000000 prisoners_dilemma_sdk-0.0.1/prisoners_dilemma_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 15:36:39.421901 prisoners_dilemma_sdk-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-27 15:36:36.000000 prisoners_dilemma_sdk-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:05:19.345687 prisoners_dilemma_sdk-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-27 16:05:19.345687 prisoners_dilemma_sdk-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-27 16:05:16.000000 prisoners_dilemma_sdk-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:05:19.345687 prisoners_dilemma_sdk-0.0.2/prisoners_dilemma_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 16:05:16.000000 prisoners_dilemma_sdk-0.0.2/prisoners_dilemma_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-27 16:05:16.000000 prisoners_dilemma_sdk-0.0.2/prisoners_dilemma_sdk/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:05:19.345687 prisoners_dilemma_sdk-0.0.2/prisoners_dilemma_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-27 16:05:19.000000 prisoners_dilemma_sdk-0.0.2/prisoners_dilemma_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-27 16:05:19.000000 prisoners_dilemma_sdk-0.0.2/prisoners_dilemma_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:05:19.000000 prisoners_dilemma_sdk-0.0.2/prisoners_dilemma_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 16:05:19.000000 prisoners_dilemma_sdk-0.0.2/prisoners_dilemma_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 16:05:19.345687 prisoners_dilemma_sdk-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-27 16:05:16.000000 prisoners_dilemma_sdk-0.0.2/setup.py
```

### Comparing `prisoners_dilemma_sdk-0.0.1/setup.py` & `prisoners_dilemma_sdk-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 NAME = "prisoners-dilemma-sdk"
 
 INSTALL_REQUIRES = []
 
 
 setuptools.setup(
```

