# Comparing `tmp/akkd_file_tree-0.0.5.tar.gz` & `tmp/akkd_file_tree-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akkd_file_tree-0.0.5.tar", last modified: Sat Apr 27 21:23:05 2024, max compression
+gzip compressed data, was "akkd_file_tree-0.0.6.tar", last modified: Sat Apr 27 21:29:01 2024, max compression
```

## Comparing `akkd_file_tree-0.0.5.tar` & `akkd_file_tree-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 21:23:05.464553 akkd_file_tree-0.0.5/
--rw-rw-rw-   0        0        0       89 2024-04-27 20:20:29.000000 akkd_file_tree-0.0.5/AUTHORS.md
--rw-rw-rw-   0        0        0     1102 2024-04-27 20:20:29.000000 akkd_file_tree-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      833 2024-04-27 21:23:05.464553 akkd_file_tree-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       56 2024-04-27 21:16:39.000000 akkd_file_tree-0.0.5/README.md
--rw-rw-rw-   0        0        0     1443 2024-04-27 21:23:05.465554 akkd_file_tree-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      610 2024-04-27 21:20:44.000000 akkd_file_tree-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 21:23:05.444509 akkd_file_tree-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-27 21:23:05.463554 akkd_file_tree-0.0.5/src/akkd_file_tree.egg-info/
--rw-rw-rw-   0        0        0      833 2024-04-27 21:23:05.000000 akkd_file_tree-0.0.5/src/akkd_file_tree.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2024-04-27 21:23:05.000000 akkd_file_tree-0.0.5/src/akkd_file_tree.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 21:23:05.000000 akkd_file_tree-0.0.5/src/akkd_file_tree.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-27 21:23:05.000000 akkd_file_tree-0.0.5/src/akkd_file_tree.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-27 20:53:13.000000 akkd_file_tree-0.0.5/src/akkd_file_tree.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       86 2024-04-27 21:23:05.000000 akkd_file_tree-0.0.5/src/akkd_file_tree.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-27 21:23:05.000000 akkd_file_tree-0.0.5/src/akkd_file_tree.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-27 21:23:05.462547 akkd_file_tree-0.0.5/src/file_tree/
--rw-rw-rw-   0        0        0       72 2024-04-27 20:25:40.000000 akkd_file_tree-0.0.5/src/file_tree/__init__.py
--rw-rw-rw-   0        0        0    33851 2024-04-27 20:20:29.000000 akkd_file_tree-0.0.5/src/file_tree/_file_tree.py
--rw-rw-rw-   0        0        0     1013 2024-04-27 20:20:29.000000 akkd_file_tree-0.0.5/src/file_tree/utils.py
--rw-rw-rw-   0        0        0       22 2024-04-27 21:04:23.000000 akkd_file_tree-0.0.5/src/file_tree/version.py
+drwxrwxrwx   0        0        0        0 2024-04-27 21:29:01.157032 akkd_file_tree-0.0.6/
+-rw-rw-rw-   0        0        0       89 2024-04-27 20:20:29.000000 akkd_file_tree-0.0.6/AUTHORS.md
+-rw-rw-rw-   0        0        0     1102 2024-04-27 20:20:29.000000 akkd_file_tree-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      748 2024-04-27 21:29:01.157032 akkd_file_tree-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2024-04-27 21:16:39.000000 akkd_file_tree-0.0.6/README.md
+-rw-rw-rw-   0        0        0     1443 2024-04-27 21:29:01.158033 akkd_file_tree-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      659 2024-04-27 21:28:44.000000 akkd_file_tree-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 21:29:01.141443 akkd_file_tree-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-27 21:29:01.156025 akkd_file_tree-0.0.6/src/akkd_file_tree.egg-info/
+-rw-rw-rw-   0        0        0      748 2024-04-27 21:29:01.000000 akkd_file_tree-0.0.6/src/akkd_file_tree.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2024-04-27 21:29:01.000000 akkd_file_tree-0.0.6/src/akkd_file_tree.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 21:29:01.000000 akkd_file_tree-0.0.6/src/akkd_file_tree.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-27 21:29:01.000000 akkd_file_tree-0.0.6/src/akkd_file_tree.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-27 20:53:13.000000 akkd_file_tree-0.0.6/src/akkd_file_tree.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       86 2024-04-27 21:29:01.000000 akkd_file_tree-0.0.6/src/akkd_file_tree.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-27 21:29:01.000000 akkd_file_tree-0.0.6/src/akkd_file_tree.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 21:29:01.156025 akkd_file_tree-0.0.6/src/file_tree/
+-rw-rw-rw-   0        0        0       72 2024-04-27 20:25:40.000000 akkd_file_tree-0.0.6/src/file_tree/__init__.py
+-rw-rw-rw-   0        0        0    33851 2024-04-27 20:20:29.000000 akkd_file_tree-0.0.6/src/file_tree/_file_tree.py
+-rw-rw-rw-   0        0        0     1013 2024-04-27 20:20:29.000000 akkd_file_tree-0.0.6/src/file_tree/utils.py
+-rw-rw-rw-   0        0        0       22 2024-04-27 21:28:51.000000 akkd_file_tree-0.0.6/src/file_tree/version.py
```

### Comparing `akkd_file_tree-0.0.5/LICENSE.txt` & `akkd_file_tree-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `akkd_file_tree-0.0.5/setup.cfg` & `akkd_file_tree-0.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `akkd_file_tree-0.0.5/src/file_tree/_file_tree.py` & `akkd_file_tree-0.0.6/src/file_tree/_file_tree.py`

 * *Files identical despite different names*

### Comparing `akkd_file_tree-0.0.5/src/file_tree/utils.py` & `akkd_file_tree-0.0.6/src/file_tree/utils.py`

 * *Files identical despite different names*

