# Comparing `tmp/adbnx_adapter-5.0.1.tar.gz` & `tmp/adbnx_adapter-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adbnx_adapter-5.0.1.tar", last modified: Fri Jan 19 15:04:58 2024, max compression
+gzip compressed data, was "adbnx_adapter-5.0.2.tar", last modified: Sat Apr 27 00:51:21 2024, max compression
```

## Comparing `adbnx_adapter-5.0.1.tar` & `adbnx_adapter-5.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 15:04:58.460239 adbnx_adapter-5.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-19 15:04:43.000000 adbnx_adapter-5.0.1/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)    10058 2024-01-19 15:04:43.000000 adbnx_adapter-5.0.1/.gitchangelog.rc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 15:04:58.456239 adbnx_adapter-5.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 15:04:58.456239 adbnx_adapter-5.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-01-19 15:04:43.000000 adbnx_adapter-5.0.1/.github/workflows/analyze.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-01-19 15:04:43.000000 adbnx_adapter-5.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-01-19 15:04:43.000000 adbnx_adapter-5.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-01-19 15:04:43.000000 adbnx_adapter-5.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    18804 2024-01-19 15:04:43.000000 adbnx_adapter-5.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-01-19 15:04:43.000000 adbnx_adapter-5.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-19 15:04:43.000000 adbnx_adapter-5.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21135 2024-01-19 15:04:58.460239 adbnx_adapter-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-01-19 15:04:43.000000 adbnx_adapter-5.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 15:04:58.456239 adbnx_adapter-5.0.1/adbnx_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-01-19 15:04:43.000000 adbnx_adapter-5.0.1/adbnx_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-01-19 15:04:43.000000 adbnx_adapter-5.0.1/adbnx_adapter/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)    27974 2024-01-19 15:04:43.000000 adbnx_adapter-5.0.1/adbnx_adapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-01-19 15:04:43.000000 adbnx_adapter-5.0.1/adbnx_adapter/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-01-19 15:04:43.000000 adbnx_adapter-5.0.1/adbnx_adapter/typings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-01-19 15:04:43.000000 adbnx_adapter-5.0.1/adbnx_adapter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 15:04:58.460239 adbnx_adapter-5.0.1/adbnx_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21135 2024-01-19 15:04:58.000000 adbnx_adapter-5.0.1/adbnx_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-01-19 15:04:58.000000 adbnx_adapter-5.0.1/adbnx_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 15:04:58.000000 adbnx_adapter-5.0.1/adbnx_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-01-19 15:04:58.000000 adbnx_adapter-5.0.1/adbnx_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-19 15:04:58.000000 adbnx_adapter-5.0.1/adbnx_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-01-19 15:04:43.000000 adbnx_adapter-5.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-19 15:04:58.460239 adbnx_adapter-5.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-19 15:04:43.000000 adbnx_adapter-5.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:51:21.001123 adbnx_adapter-5.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-27 00:51:08.000000 adbnx_adapter-5.0.2/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)    10058 2024-04-27 00:51:08.000000 adbnx_adapter-5.0.2/.gitchangelog.rc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:51:20.993123 adbnx_adapter-5.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:51:20.997123 adbnx_adapter-5.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-27 00:51:08.000000 adbnx_adapter-5.0.2/.github/workflows/analyze.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-27 00:51:08.000000 adbnx_adapter-5.0.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-27 00:51:08.000000 adbnx_adapter-5.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-27 00:51:08.000000 adbnx_adapter-5.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    19281 2024-04-27 00:51:08.000000 adbnx_adapter-5.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-04-27 00:51:08.000000 adbnx_adapter-5.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-27 00:51:08.000000 adbnx_adapter-5.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21135 2024-04-27 00:51:21.001123 adbnx_adapter-5.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-04-27 00:51:08.000000 adbnx_adapter-5.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:51:20.997123 adbnx_adapter-5.0.2/adbnx_adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-27 00:51:08.000000 adbnx_adapter-5.0.2/adbnx_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-27 00:51:08.000000 adbnx_adapter-5.0.2/adbnx_adapter/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28000 2024-04-27 00:51:08.000000 adbnx_adapter-5.0.2/adbnx_adapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-04-27 00:51:08.000000 adbnx_adapter-5.0.2/adbnx_adapter/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-27 00:51:08.000000 adbnx_adapter-5.0.2/adbnx_adapter/typings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-27 00:51:08.000000 adbnx_adapter-5.0.2/adbnx_adapter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:51:21.001123 adbnx_adapter-5.0.2/adbnx_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21135 2024-04-27 00:51:20.000000 adbnx_adapter-5.0.2/adbnx_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-27 00:51:20.000000 adbnx_adapter-5.0.2/adbnx_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 00:51:20.000000 adbnx_adapter-5.0.2/adbnx_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-27 00:51:20.000000 adbnx_adapter-5.0.2/adbnx_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-27 00:51:20.000000 adbnx_adapter-5.0.2/adbnx_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-27 00:51:08.000000 adbnx_adapter-5.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 00:51:21.001123 adbnx_adapter-5.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 00:51:08.000000 adbnx_adapter-5.0.2/setup.py
```

### Comparing `adbnx_adapter-5.0.1/.gitchangelog.rc` & `adbnx_adapter-5.0.2/.gitchangelog.rc`

 * *Files identical despite different names*

### Comparing `adbnx_adapter-5.0.1/.github/workflows/analyze.yml` & `adbnx_adapter-5.0.2/.github/workflows/analyze.yml`

 * *Files identical despite different names*

### Comparing `adbnx_adapter-5.0.1/.github/workflows/build.yml` & `adbnx_adapter-5.0.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adbnx_adapter-5.0.1/.github/workflows/release.yml` & `adbnx_adapter-5.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adbnx_adapter-5.0.1/.gitignore` & `adbnx_adapter-5.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `adbnx_adapter-5.0.1/CHANGELOG.md` & `adbnx_adapter-5.0.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+## 5.0.1 (2024-01-19)
+
+### Other
+
+* Optimize `__fetch_adb_docs` (#93) [Anthony Mahanna]
+
+  * optimize `__fetch_adb_docs`
+
+  * set `continue-on-error`
+
+  * fix: set metagraph `edgeCollections` as optional
+
+  not sure why anyone would want this, but still technically possible nevertheless..
+
+  * cleanup: `aql_return_value`
+
+* Update Build Distribution Command (#92) [Anthony Mahanna]
+
+  initial commit
+
+* Changelog: release 5.0.0 (#91) [github-actions[bot]]
+
+  !gitchangelog
+
+
 ## 5.0.0 (2023-11-22)
 
 ### Fix
 
 * Missing docstring entry. [aMahanna]
 
 ### Other
```

### Comparing `adbnx_adapter-5.0.1/LICENSE` & `adbnx_adapter-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adbnx_adapter-5.0.1/PKG-INFO` & `adbnx_adapter-5.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbnx_adapter
-Version: 5.0.1
+Version: 5.0.2
 Summary: Convert ArangoDB graphs to NetworkX & vice-versa.
 Author-email: Anthony Mahanna <anthony.mahanna@arangodb.com>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `adbnx_adapter-5.0.1/README.md` & `adbnx_adapter-5.0.2/README.md`

 * *Files identical despite different names*

### Comparing `adbnx_adapter-5.0.1/adbnx_adapter/abc.py` & `adbnx_adapter-5.0.2/adbnx_adapter/abc.py`

 * *Files identical despite different names*

### Comparing `adbnx_adapter-5.0.1/adbnx_adapter/adapter.py` & `adbnx_adapter-5.0.2/adbnx_adapter/adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                 },
             },
         }
         """
         logger.debug(f"--arangodb_to_networkx('{name}')--")
 
         # Create a new NetworkX graph if one is not provided
-        nx_graph = nx_graph or NXMultiDiGraph(name=name)
+        nx_graph = nx_graph if nx_graph is not None else NXMultiDiGraph(name=name)
 
         # This maps the ArangoDB vertex IDs to NetworkX node IDs
         adb_map: Dict[str, NxId] = dict()
 
         ######################
         # Vertex Collections #
         ######################
```

### Comparing `adbnx_adapter-5.0.1/adbnx_adapter/controller.py` & `adbnx_adapter-5.0.2/adbnx_adapter/controller.py`

 * *Files identical despite different names*

### Comparing `adbnx_adapter-5.0.1/adbnx_adapter/utils.py` & `adbnx_adapter-5.0.2/adbnx_adapter/utils.py`

 * *Files identical despite different names*

### Comparing `adbnx_adapter-5.0.1/adbnx_adapter.egg-info/PKG-INFO` & `adbnx_adapter-5.0.2/adbnx_adapter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbnx_adapter
-Version: 5.0.1
+Version: 5.0.2
 Summary: Convert ArangoDB graphs to NetworkX & vice-versa.
 Author-email: Anthony Mahanna <anthony.mahanna@arangodb.com>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `adbnx_adapter-5.0.1/adbnx_adapter.egg-info/SOURCES.txt` & `adbnx_adapter-5.0.2/adbnx_adapter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adbnx_adapter-5.0.1/pyproject.toml` & `adbnx_adapter-5.0.2/pyproject.toml`

 * *Files identical despite different names*

