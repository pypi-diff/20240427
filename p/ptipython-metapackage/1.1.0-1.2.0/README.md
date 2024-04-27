# Comparing `tmp/ptipython-metapackage-1.1.0.tar.gz` & `tmp/ptipython_metapackage-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptipython-metapackage-1.1.0.tar", last modified: Mon Apr  1 01:33:47 2024, max compression
+gzip compressed data, was "ptipython_metapackage-1.2.0.tar", last modified: Sat Apr 27 01:22:17 2024, max compression
```

## Comparing `ptipython-metapackage-1.1.0.tar` & `ptipython_metapackage-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:33:47.712799 ptipython-metapackage-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-01 01:33:40.000000 ptipython-metapackage-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-01 01:33:47.712799 ptipython-metapackage-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-01 01:33:40.000000 ptipython-metapackage-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:33:47.712799 ptipython-metapackage-1.1.0/ptipython_metapackage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-01 01:33:47.000000 ptipython-metapackage-1.1.0/ptipython_metapackage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-01 01:33:47.000000 ptipython-metapackage-1.1.0/ptipython_metapackage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 01:33:47.000000 ptipython-metapackage-1.1.0/ptipython_metapackage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-01 01:33:47.000000 ptipython-metapackage-1.1.0/ptipython_metapackage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-01 01:33:47.000000 ptipython-metapackage-1.1.0/ptipython_metapackage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 01:33:47.000000 ptipython-metapackage-1.1.0/ptipython_metapackage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-01 01:33:40.000000 ptipython-metapackage-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 01:33:47.712799 ptipython-metapackage-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:33:47.712799 ptipython-metapackage-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-01 01:33:40.000000 ptipython-metapackage-1.1.0/tests/test_bump_metapackage_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-01 01:33:40.000000 ptipython-metapackage-1.1.0/tests/test_compare_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:22:17.551237 ptipython_metapackage-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-27 01:22:08.000000 ptipython_metapackage-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-27 01:22:17.551237 ptipython_metapackage-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-27 01:22:08.000000 ptipython_metapackage-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:22:17.551237 ptipython_metapackage-1.2.0/ptipython_metapackage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-27 01:22:17.000000 ptipython_metapackage-1.2.0/ptipython_metapackage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-27 01:22:17.000000 ptipython_metapackage-1.2.0/ptipython_metapackage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 01:22:17.000000 ptipython_metapackage-1.2.0/ptipython_metapackage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-27 01:22:17.000000 ptipython_metapackage-1.2.0/ptipython_metapackage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-27 01:22:17.000000 ptipython_metapackage-1.2.0/ptipython_metapackage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 01:22:17.000000 ptipython_metapackage-1.2.0/ptipython_metapackage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-27 01:22:08.000000 ptipython_metapackage-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 01:22:17.551237 ptipython_metapackage-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:22:17.551237 ptipython_metapackage-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-27 01:22:08.000000 ptipython_metapackage-1.2.0/tests/test_bump_metapackage_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-27 01:22:08.000000 ptipython_metapackage-1.2.0/tests/test_compare_versions.py
```

### Comparing `ptipython-metapackage-1.1.0/LICENSE` & `ptipython_metapackage-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ptipython-metapackage-1.1.0/pyproject.toml` & `ptipython_metapackage-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ptipython-metapackage"
-version = "1.1.0"
+version = "1.2.0"
 description = "ptipython metapackage"
 readme = "README.md"
 license = {text = "BSD-3-Clause"}
 authors = [
     {name = "Dmitry Meyer", email = "me@undef.im"},
 ]
 classifiers = [
@@ -17,15 +17,15 @@
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
 ]
 keywords = ["ptipython", "ptpython", "ipython"]
 requires-python = ">= 3.10"
-dependencies = ["ptpython == 3.0.26", "ipython == 8.23.0"]
+dependencies = ["ptpython == 3.0.26", "ipython == 8.24.0"]
 
 [project.scripts]
 ptipython = "ptpython.entry_points.run_ptipython:run"
 ptpython = "ptpython.entry_points.run_ptpython:run"
 ipython = "IPython:start_ipython"
 
 [project.urls]
```

### Comparing `ptipython-metapackage-1.1.0/tests/test_compare_versions.py` & `ptipython_metapackage-1.2.0/tests/test_compare_versions.py`

 * *Files identical despite different names*

