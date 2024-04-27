# Comparing `tmp/arrayutilities-1.0.0.tar.gz` & `tmp/arrayutilities-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrayutilities-1.0.0.tar", last modified: Sat Apr 27 17:39:58 2024, max compression
+gzip compressed data, was "arrayutilities-1.0.1.tar", last modified: Sat Apr 27 17:43:18 2024, max compression
```

## Comparing `arrayutilities-1.0.0.tar` & `arrayutilities-1.0.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:39:58.441608 arrayutilities-1.0.0/
--rw-r--r--   0 matt      (1000) matt      (1000)     1075 2024-04-27 13:08:28.000000 arrayutilities-1.0.0/LICENSE
--rw-r--r--   0 matt      (1000) matt      (1000)    18950 2024-04-27 17:39:58.441608 arrayutilities-1.0.0/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)    17169 2024-04-27 17:38:26.000000 arrayutilities-1.0.0/README.md
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:39:58.441608 arrayutilities-1.0.0/arrayutilities.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)    18950 2024-04-27 17:39:58.000000 arrayutilities-1.0.0/arrayutilities.egg-info/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)     1219 2024-04-27 17:39:58.000000 arrayutilities-1.0.0/arrayutilities.egg-info/SOURCES.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-04-27 17:39:58.000000 arrayutilities-1.0.0/arrayutilities.egg-info/dependency_links.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       17 2024-04-27 17:39:58.000000 arrayutilities-1.0.0/arrayutilities.egg-info/top_level.txt
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:39:58.441608 arrayutilities-1.0.0/arrayutils/
--rw-r--r--   0 matt      (1000) matt      (1000)    25579 2024-04-27 17:13:16.000000 arrayutilities-1.0.0/arrayutils/__init__.py
--rw-r--r--   0 matt      (1000) matt      (1000)      648 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/pyproject.toml
--rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-04-27 17:39:58.441608 arrayutilities-1.0.0/setup.cfg
--rw-r--r--   0 matt      (1000) matt      (1000)      393 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/setup.py
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:39:58.441608 arrayutilities-1.0.0/tests/
--rw-r--r--   0 matt      (1000) matt      (1000)        0 2024-04-27 13:11:34.000000 arrayutilities-1.0.0/tests/__init__.py
--rw-r--r--   0 matt      (1000) matt      (1000)      818 2024-04-27 17:38:47.000000 arrayutilities-1.0.0/tests/test_accessible.py
--rw-r--r--   0 matt      (1000) matt      (1000)      968 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_add.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1312 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_add_prefixed_keys_to.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1321 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_add_unprefixed_keys_to.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1589 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_array_visit_recursive.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1155 2024-04-27 17:38:47.000000 arrayutilities-1.0.0/tests/test_collapse.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1536 2024-04-27 17:38:47.000000 arrayutilities-1.0.0/tests/test_dot.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1559 2024-04-27 17:38:47.000000 arrayutilities-1.0.0/tests/test_exists.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1585 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_filter_prefixed.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1463 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_first.py
--rw-r--r--   0 matt      (1000) matt      (1000)     2058 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_flatten.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1634 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_forget.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1862 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_get.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1456 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_has.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1368 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_insert_after_key.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1389 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_insert_before_key.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1288 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_is_dict.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1035 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_is_list.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1695 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_join.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1666 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_last.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1642 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_list_to_array.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1699 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_merge_recursive.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1530 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_only.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1445 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_prepend.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1481 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_pull.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1658 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_query.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1448 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_random.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1106 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_recursive_ksort.py
--rw-r--r--   0 matt      (1000) matt      (1000)      998 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_set.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1103 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_shape_filter.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1045 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_shuffle.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1475 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_sort_by_priority.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1350 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_sort_recursive.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1076 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_stringify_keys.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1502 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_strpos.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1249 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_to_list.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1472 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_undot.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1216 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_usearch.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1303 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_where.py
--rw-r--r--   0 matt      (1000) matt      (1000)      996 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_where_not_none.py
--rw-r--r--   0 matt      (1000) matt      (1000)      903 2024-04-27 17:38:46.000000 arrayutilities-1.0.0/tests/test_wrap.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:43:18.628298 arrayutilities-1.0.1/
+-rw-r--r--   0 matt      (1000) matt      (1000)     1075 2024-04-27 13:08:28.000000 arrayutilities-1.0.1/LICENSE
+-rw-r--r--   0 matt      (1000) matt      (1000)    18950 2024-04-27 17:43:18.628298 arrayutilities-1.0.1/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)    17169 2024-04-27 17:38:26.000000 arrayutilities-1.0.1/README.md
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:43:18.618298 arrayutilities-1.0.1/arrayutilities/
+-rw-r--r--   0 matt      (1000) matt      (1000)    25579 2024-04-27 17:13:16.000000 arrayutilities-1.0.1/arrayutilities/__init__.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:43:18.628298 arrayutilities-1.0.1/arrayutilities.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)    18950 2024-04-27 17:43:18.000000 arrayutilities-1.0.1/arrayutilities.egg-info/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)     1223 2024-04-27 17:43:18.000000 arrayutilities-1.0.1/arrayutilities.egg-info/SOURCES.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-04-27 17:43:18.000000 arrayutilities-1.0.1/arrayutilities.egg-info/dependency_links.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       21 2024-04-27 17:43:18.000000 arrayutilities-1.0.1/arrayutilities.egg-info/top_level.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)      648 2024-04-27 17:42:49.000000 arrayutilities-1.0.1/pyproject.toml
+-rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-04-27 17:43:18.628298 arrayutilities-1.0.1/setup.cfg
+-rw-r--r--   0 matt      (1000) matt      (1000)      393 2024-04-27 17:42:55.000000 arrayutilities-1.0.1/setup.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:43:18.628298 arrayutilities-1.0.1/tests/
+-rw-r--r--   0 matt      (1000) matt      (1000)        0 2024-04-27 13:11:34.000000 arrayutilities-1.0.1/tests/__init__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      818 2024-04-27 17:38:47.000000 arrayutilities-1.0.1/tests/test_accessible.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      968 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_add.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1312 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_add_prefixed_keys_to.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1321 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_add_unprefixed_keys_to.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1589 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_array_visit_recursive.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1155 2024-04-27 17:38:47.000000 arrayutilities-1.0.1/tests/test_collapse.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1536 2024-04-27 17:38:47.000000 arrayutilities-1.0.1/tests/test_dot.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1559 2024-04-27 17:38:47.000000 arrayutilities-1.0.1/tests/test_exists.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1585 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_filter_prefixed.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1463 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_first.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     2058 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_flatten.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1634 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_forget.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1862 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_get.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1456 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_has.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1368 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_insert_after_key.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1389 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_insert_before_key.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1288 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_is_dict.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1035 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_is_list.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1695 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_join.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1666 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_last.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1642 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_list_to_array.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1699 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_merge_recursive.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1530 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_only.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1445 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_prepend.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1481 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_pull.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1658 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_query.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1448 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_random.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1106 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_recursive_ksort.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      998 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_set.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1103 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_shape_filter.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1045 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_shuffle.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1475 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_sort_by_priority.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1350 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_sort_recursive.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1076 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_stringify_keys.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1502 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_strpos.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1249 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_to_list.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1472 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_undot.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1216 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_usearch.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1303 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_where.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      996 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_where_not_none.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      903 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_wrap.py
```

### Comparing `arrayutilities-1.0.0/LICENSE` & `arrayutilities-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/PKG-INFO` & `arrayutilities-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrayutilities
-Version: 1.0.0
+Version: 1.0.1
 Summary: A library for list, dict, and UserDict manipulations.
 Author: Matthew Batchelder
 Author-email: Matthew Batchelder <borkweb@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Matthew Batchelder
```

### Comparing `arrayutilities-1.0.0/README.md` & `arrayutilities-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/arrayutilities.egg-info/PKG-INFO` & `arrayutilities-1.0.1/arrayutilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrayutilities
-Version: 1.0.0
+Version: 1.0.1
 Summary: A library for list, dict, and UserDict manipulations.
 Author: Matthew Batchelder
 Author-email: Matthew Batchelder <borkweb@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Matthew Batchelder
```

### Comparing `arrayutilities-1.0.0/arrayutilities.egg-info/SOURCES.txt` & `arrayutilities-1.0.1/arrayutilities.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
+arrayutilities/__init__.py
 arrayutilities.egg-info/PKG-INFO
 arrayutilities.egg-info/SOURCES.txt
 arrayutilities.egg-info/dependency_links.txt
 arrayutilities.egg-info/top_level.txt
-arrayutils/__init__.py
 tests/__init__.py
 tests/test_accessible.py
 tests/test_add.py
 tests/test_add_prefixed_keys_to.py
 tests/test_add_unprefixed_keys_to.py
 tests/test_array_visit_recursive.py
 tests/test_collapse.py
```

### Comparing `arrayutilities-1.0.0/arrayutils/__init__.py` & `arrayutilities-1.0.1/arrayutilities/__init__.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/pyproject.toml` & `arrayutilities-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-sysetm]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "arrayutilities"
-version = "1.0.0"
+version = "1.0.1"
 description = "A library for list, dict, and UserDict manipulations."
 readme = "README.md"
 authors = [{ name = "Matthew Batchelder", email = "borkweb@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `arrayutilities-1.0.0/tests/test_accessible.py` & `arrayutilities-1.0.1/tests/test_accessible.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_add.py` & `arrayutilities-1.0.1/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_add_prefixed_keys_to.py` & `arrayutilities-1.0.1/tests/test_add_prefixed_keys_to.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_add_unprefixed_keys_to.py` & `arrayutilities-1.0.1/tests/test_add_unprefixed_keys_to.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_array_visit_recursive.py` & `arrayutilities-1.0.1/tests/test_array_visit_recursive.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_collapse.py` & `arrayutilities-1.0.1/tests/test_collapse.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_dot.py` & `arrayutilities-1.0.1/tests/test_dot.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_exists.py` & `arrayutilities-1.0.1/tests/test_exists.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_filter_prefixed.py` & `arrayutilities-1.0.1/tests/test_filter_prefixed.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_first.py` & `arrayutilities-1.0.1/tests/test_first.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_flatten.py` & `arrayutilities-1.0.1/tests/test_flatten.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_forget.py` & `arrayutilities-1.0.1/tests/test_forget.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_get.py` & `arrayutilities-1.0.1/tests/test_get.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_has.py` & `arrayutilities-1.0.1/tests/test_has.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_insert_after_key.py` & `arrayutilities-1.0.1/tests/test_insert_after_key.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_insert_before_key.py` & `arrayutilities-1.0.1/tests/test_insert_before_key.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_is_dict.py` & `arrayutilities-1.0.1/tests/test_is_dict.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_is_list.py` & `arrayutilities-1.0.1/tests/test_is_list.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_join.py` & `arrayutilities-1.0.1/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_last.py` & `arrayutilities-1.0.1/tests/test_last.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_list_to_array.py` & `arrayutilities-1.0.1/tests/test_list_to_array.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_merge_recursive.py` & `arrayutilities-1.0.1/tests/test_merge_recursive.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_only.py` & `arrayutilities-1.0.1/tests/test_only.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_prepend.py` & `arrayutilities-1.0.1/tests/test_prepend.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_pull.py` & `arrayutilities-1.0.1/tests/test_pull.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_query.py` & `arrayutilities-1.0.1/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_random.py` & `arrayutilities-1.0.1/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_recursive_ksort.py` & `arrayutilities-1.0.1/tests/test_recursive_ksort.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_set.py` & `arrayutilities-1.0.1/tests/test_set.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_shape_filter.py` & `arrayutilities-1.0.1/tests/test_shape_filter.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_shuffle.py` & `arrayutilities-1.0.1/tests/test_shuffle.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_sort_by_priority.py` & `arrayutilities-1.0.1/tests/test_sort_by_priority.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_sort_recursive.py` & `arrayutilities-1.0.1/tests/test_sort_recursive.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_stringify_keys.py` & `arrayutilities-1.0.1/tests/test_stringify_keys.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_strpos.py` & `arrayutilities-1.0.1/tests/test_strpos.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_to_list.py` & `arrayutilities-1.0.1/tests/test_to_list.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_undot.py` & `arrayutilities-1.0.1/tests/test_undot.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_usearch.py` & `arrayutilities-1.0.1/tests/test_usearch.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_where.py` & `arrayutilities-1.0.1/tests/test_where.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_where_not_none.py` & `arrayutilities-1.0.1/tests/test_where_not_none.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.0/tests/test_wrap.py` & `arrayutilities-1.0.1/tests/test_wrap.py`

 * *Files identical despite different names*

