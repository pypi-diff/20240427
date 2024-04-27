# Comparing `tmp/dirconfig-0.2.3.tar.gz` & `tmp/dirconfig-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirconfig-0.2.3.tar", last modified: Mon Apr  8 03:04:32 2024, max compression
+gzip compressed data, was "dirconfig-0.2.4.tar", last modified: Sat Apr 27 05:18:42 2024, max compression
```

## Comparing `dirconfig-0.2.3.tar` & `dirconfig-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:04:32.849766 dirconfig-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-08 03:04:19.000000 dirconfig-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-08 03:04:32.849766 dirconfig-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-08 03:04:19.000000 dirconfig-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:04:32.845766 dirconfig-0.2.3/dirconfig/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 03:04:19.000000 dirconfig-0.2.3/dirconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-08 03:04:19.000000 dirconfig-0.2.3/dirconfig/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:04:32.845766 dirconfig-0.2.3/dirconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-08 03:04:32.000000 dirconfig-0.2.3/dirconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-08 03:04:32.000000 dirconfig-0.2.3/dirconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:04:32.000000 dirconfig-0.2.3/dirconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 03:04:32.000000 dirconfig-0.2.3/dirconfig.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 03:04:32.000000 dirconfig-0.2.3/dirconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 03:04:32.000000 dirconfig-0.2.3/dirconfig.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 03:04:32.849766 dirconfig-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-08 03:04:30.000000 dirconfig-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:04:32.849766 dirconfig-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 03:04:19.000000 dirconfig-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-08 03:04:19.000000 dirconfig-0.2.3/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 05:18:42.634647 dirconfig-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-27 05:18:20.000000 dirconfig-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-04-27 05:18:42.634647 dirconfig-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-04-27 05:18:20.000000 dirconfig-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 05:18:42.634647 dirconfig-0.2.4/dirconfig/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 05:18:20.000000 dirconfig-0.2.4/dirconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9525 2024-04-27 05:18:20.000000 dirconfig-0.2.4/dirconfig/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 05:18:42.634647 dirconfig-0.2.4/dirconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-04-27 05:18:42.000000 dirconfig-0.2.4/dirconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-27 05:18:42.000000 dirconfig-0.2.4/dirconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 05:18:42.000000 dirconfig-0.2.4/dirconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-27 05:18:42.000000 dirconfig-0.2.4/dirconfig.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-27 05:18:42.000000 dirconfig-0.2.4/dirconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-27 05:18:42.000000 dirconfig-0.2.4/dirconfig.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 05:18:42.634647 dirconfig-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-27 05:18:40.000000 dirconfig-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 05:18:42.634647 dirconfig-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 05:18:20.000000 dirconfig-0.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-27 05:18:20.000000 dirconfig-0.2.4/tests/test_main.py
```

### Comparing `dirconfig-0.2.3/LICENSE` & `dirconfig-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dirconfig-0.2.3/setup.py` & `dirconfig-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dirconfig",
-    version="0.2.3",
+    version="0.2.4",
     author="Judah Paul",
     author_email="me@judahpaul.com",
     description="A simple directory configuration tool",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/judahpaul16/dirconfig",
     packages=find_packages(),
```

### Comparing `dirconfig-0.2.3/tests/test_main.py` & `dirconfig-0.2.4/tests/test_main.py`

 * *Files identical despite different names*

