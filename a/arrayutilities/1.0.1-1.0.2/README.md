# Comparing `tmp/arrayutilities-1.0.1.tar.gz` & `tmp/arrayutilities-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrayutilities-1.0.1.tar", last modified: Sat Apr 27 17:43:18 2024, max compression
+gzip compressed data, was "arrayutilities-1.0.2.tar", last modified: Sat Apr 27 17:48:13 2024, max compression
```

## Comparing `arrayutilities-1.0.1.tar` & `arrayutilities-1.0.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:43:18.628298 arrayutilities-1.0.1/
--rw-r--r--   0 matt      (1000) matt      (1000)     1075 2024-04-27 13:08:28.000000 arrayutilities-1.0.1/LICENSE
--rw-r--r--   0 matt      (1000) matt      (1000)    18950 2024-04-27 17:43:18.628298 arrayutilities-1.0.1/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)    17169 2024-04-27 17:38:26.000000 arrayutilities-1.0.1/README.md
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:43:18.618298 arrayutilities-1.0.1/arrayutilities/
--rw-r--r--   0 matt      (1000) matt      (1000)    25579 2024-04-27 17:13:16.000000 arrayutilities-1.0.1/arrayutilities/__init__.py
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:43:18.628298 arrayutilities-1.0.1/arrayutilities.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)    18950 2024-04-27 17:43:18.000000 arrayutilities-1.0.1/arrayutilities.egg-info/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)     1223 2024-04-27 17:43:18.000000 arrayutilities-1.0.1/arrayutilities.egg-info/SOURCES.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-04-27 17:43:18.000000 arrayutilities-1.0.1/arrayutilities.egg-info/dependency_links.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       21 2024-04-27 17:43:18.000000 arrayutilities-1.0.1/arrayutilities.egg-info/top_level.txt
--rw-r--r--   0 matt      (1000) matt      (1000)      648 2024-04-27 17:42:49.000000 arrayutilities-1.0.1/pyproject.toml
--rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-04-27 17:43:18.628298 arrayutilities-1.0.1/setup.cfg
--rw-r--r--   0 matt      (1000) matt      (1000)      393 2024-04-27 17:42:55.000000 arrayutilities-1.0.1/setup.py
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:43:18.628298 arrayutilities-1.0.1/tests/
--rw-r--r--   0 matt      (1000) matt      (1000)        0 2024-04-27 13:11:34.000000 arrayutilities-1.0.1/tests/__init__.py
--rw-r--r--   0 matt      (1000) matt      (1000)      818 2024-04-27 17:38:47.000000 arrayutilities-1.0.1/tests/test_accessible.py
--rw-r--r--   0 matt      (1000) matt      (1000)      968 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_add.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1312 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_add_prefixed_keys_to.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1321 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_add_unprefixed_keys_to.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1589 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_array_visit_recursive.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1155 2024-04-27 17:38:47.000000 arrayutilities-1.0.1/tests/test_collapse.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1536 2024-04-27 17:38:47.000000 arrayutilities-1.0.1/tests/test_dot.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1559 2024-04-27 17:38:47.000000 arrayutilities-1.0.1/tests/test_exists.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1585 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_filter_prefixed.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1463 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_first.py
--rw-r--r--   0 matt      (1000) matt      (1000)     2058 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_flatten.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1634 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_forget.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1862 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_get.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1456 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_has.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1368 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_insert_after_key.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1389 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_insert_before_key.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1288 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_is_dict.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1035 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_is_list.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1695 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_join.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1666 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_last.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1642 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_list_to_array.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1699 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_merge_recursive.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1530 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_only.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1445 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_prepend.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1481 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_pull.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1658 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_query.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1448 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_random.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1106 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_recursive_ksort.py
--rw-r--r--   0 matt      (1000) matt      (1000)      998 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_set.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1103 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_shape_filter.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1045 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_shuffle.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1475 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_sort_by_priority.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1350 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_sort_recursive.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1076 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_stringify_keys.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1502 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_strpos.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1249 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_to_list.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1472 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_undot.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1216 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_usearch.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1303 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_where.py
--rw-r--r--   0 matt      (1000) matt      (1000)      996 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_where_not_none.py
--rw-r--r--   0 matt      (1000) matt      (1000)      903 2024-04-27 17:38:46.000000 arrayutilities-1.0.1/tests/test_wrap.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:48:13.760130 arrayutilities-1.0.2/
+-rw-r--r--   0 matt      (1000) matt      (1000)     1075 2024-04-27 13:08:28.000000 arrayutilities-1.0.2/LICENSE
+-rw-r--r--   0 matt      (1000) matt      (1000)    18908 2024-04-27 17:48:13.760130 arrayutilities-1.0.2/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)    17127 2024-04-27 17:47:07.000000 arrayutilities-1.0.2/README.md
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:48:13.750130 arrayutilities-1.0.2/arrayutilities/
+-rw-r--r--   0 matt      (1000) matt      (1000)    25579 2024-04-27 17:13:16.000000 arrayutilities-1.0.2/arrayutilities/__init__.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:48:13.760130 arrayutilities-1.0.2/arrayutilities.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)    18908 2024-04-27 17:48:13.000000 arrayutilities-1.0.2/arrayutilities.egg-info/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)     1223 2024-04-27 17:48:13.000000 arrayutilities-1.0.2/arrayutilities.egg-info/SOURCES.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-04-27 17:48:13.000000 arrayutilities-1.0.2/arrayutilities.egg-info/dependency_links.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       21 2024-04-27 17:48:13.000000 arrayutilities-1.0.2/arrayutilities.egg-info/top_level.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)      648 2024-04-27 17:47:48.000000 arrayutilities-1.0.2/pyproject.toml
+-rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-04-27 17:48:13.760130 arrayutilities-1.0.2/setup.cfg
+-rw-r--r--   0 matt      (1000) matt      (1000)      393 2024-04-27 17:47:45.000000 arrayutilities-1.0.2/setup.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:48:13.760130 arrayutilities-1.0.2/tests/
+-rw-r--r--   0 matt      (1000) matt      (1000)        0 2024-04-27 13:11:34.000000 arrayutilities-1.0.2/tests/__init__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      818 2024-04-27 17:38:47.000000 arrayutilities-1.0.2/tests/test_accessible.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      968 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_add.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1312 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_add_prefixed_keys_to.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1321 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_add_unprefixed_keys_to.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1589 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_array_visit_recursive.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1155 2024-04-27 17:38:47.000000 arrayutilities-1.0.2/tests/test_collapse.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1536 2024-04-27 17:38:47.000000 arrayutilities-1.0.2/tests/test_dot.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1559 2024-04-27 17:38:47.000000 arrayutilities-1.0.2/tests/test_exists.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1585 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_filter_prefixed.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1463 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_first.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     2058 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_flatten.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1634 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_forget.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1862 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_get.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1456 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_has.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1368 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_insert_after_key.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1389 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_insert_before_key.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1288 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_is_dict.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1035 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_is_list.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1695 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_join.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1666 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_last.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1642 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_list_to_array.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1699 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_merge_recursive.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1530 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_only.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1445 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_prepend.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1481 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_pull.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1658 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_query.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1448 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_random.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1106 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_recursive_ksort.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      998 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_set.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1103 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_shape_filter.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1045 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_shuffle.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1475 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_sort_by_priority.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1350 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_sort_recursive.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1076 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_stringify_keys.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1502 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_strpos.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1249 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_to_list.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1472 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_undot.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1216 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_usearch.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1303 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_where.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      996 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_where_not_none.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      903 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_wrap.py
```

### Comparing `arrayutilities-1.0.1/LICENSE` & `arrayutilities-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/PKG-INFO` & `arrayutilities-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrayutilities
-Version: 1.0.1
+Version: 1.0.2
 Summary: A library for list, dict, and UserDict manipulations.
 Author: Matthew Batchelder
 Author-email: Matthew Batchelder <borkweb@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Matthew Batchelder
         
@@ -103,15 +103,15 @@
 
 ```python
 from arrayutilities import Arr
 ```
 
 <a id="Arr.accessible"></a>
 
-#### accessible
+### accessible
 
 ```python
 @staticmethod
 def accessible(value)
 ```
 
 Determines if the given value is a list, dict, or UserDict.
@@ -123,15 +123,15 @@
 
 **Returns**:
 
 - `boolean` - Whether the the value is a list, dict, or UserDict.
 
 <a id="Arr.add"></a>
 
-#### add
+### add
 
 ```python
 @staticmethod
 def add(array, key, value)
 ```
 
 Add an element to an array if it doesn't exist.
@@ -145,15 +145,15 @@
 
 **Returns**:
 
   Manipulated array
 
 <a id="Arr.add_prefixed_keys_to"></a>
 
-#### add\_prefixed\_keys\_to
+### add\_prefixed\_keys\_to
 
 ```python
 @staticmethod
 def add_prefixed_keys_to(array, recursive=False)
 ```
 
 Duplicates any key not prefixed with '_' creating a prefixed duplicate one.
@@ -166,15 +166,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.add_unprefixed_keys_to"></a>
 
-#### add\_unprefixed\_keys\_to
+### add\_unprefixed\_keys\_to
 
 ```python
 @staticmethod
 def add_unprefixed_keys_to(array, recursive=False)
 ```
 
 Duplicates any key prefixed with '_' creating an un-prefixed duplicate one.
@@ -187,15 +187,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.array_visit_recursive"></a>
 
-#### array\_visit\_recursive
+### array\_visit\_recursive
 
 ```python
 @staticmethod
 def array_visit_recursive(input_array, visitor)
 ```
 
 Recursively visits all elements of an array applying the specified callback to each element key and value.
@@ -211,15 +211,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.collapse"></a>
 
-#### collapse
+### collapse
 
 ```python
 @staticmethod
 def collapse(array)
 ```
 
 Collapse an array of arrays into a single array.
@@ -231,15 +231,15 @@
 
 **Returns**:
 
   Collapsed array.
 
 <a id="Arr.dot"></a>
 
-#### dot
+### dot
 
 ```python
 @staticmethod
 def dot(array, prepend='')
 ```
 
 Flatten a multi-dimensional associative array with dots.
@@ -252,15 +252,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.exists"></a>
 
-#### exists
+### exists
 
 ```python
 @staticmethod
 def exists(array, key)
 ```
 
 Determine if the given key exists in the provided array.
@@ -273,15 +273,15 @@
 
 **Returns**:
 
 - `boolean` - Whether or not the key exists.
 
 <a id="Arr.filter_prefixed"></a>
 
-#### filter\_prefixed
+### filter\_prefixed
 
 ```python
 @staticmethod
 def filter_prefixed(array, prefix)
 ```
 
 Filters an associative array non-recursively, keeping only the values attached to keys starting with the specified prefix.
@@ -294,15 +294,15 @@
 
 **Returns**:
 
   Filtered array.
 
 <a id="Arr.first"></a>
 
-#### first
+### first
 
 ```python
 @staticmethod
 def first(array, callback=None, default=None)
 ```
 
 Return the first element in an array passing a given truth test.
@@ -316,15 +316,15 @@
 
 **Returns**:
 
   Found value or default.
 
 <a id="Arr.flatten"></a>
 
-#### flatten
+### flatten
 
 ```python
 @staticmethod
 def flatten(array, depth=float('inf'))
 ```
 
 Flatten a multi-dimensional array into a single level.
@@ -337,15 +337,15 @@
 
 **Returns**:
 
   Flattened array.
 
 <a id="Arr.forget"></a>
 
-#### forget
+### forget
 
 ```python
 @staticmethod
 def forget(array, keys)
 ```
 
 Remove one or many array items from a given array using "dot" notation.
@@ -353,15 +353,15 @@
 **Arguments**:
 
 - `array` - Array to manipulate.
 - `keys` _str|array_ - Key or keys to remove.
 
 <a id="Arr.get"></a>
 
-#### get
+### get
 
 ```python
 @staticmethod
 def get(array, keys, default=None)
 ```
 
 Find a value inside of an array or object, including one nested a few levels deep.
@@ -375,15 +375,15 @@
 
 **Returns**:
 
 - `_type_` - _description_
 
 <a id="Arr.has"></a>
 
-#### has
+### has
 
 ```python
 @staticmethod
 def has(array, keys)
 ```
 
 Check if an item or items exist in an array using "dot" notation.
@@ -396,15 +396,15 @@
 
 **Returns**:
 
 - `boolean` - Whether the key exists or not.
 
 <a id="Arr.insert_after_key"></a>
 
-#### insert\_after\_key
+### insert\_after\_key
 
 ```python
 @staticmethod
 def insert_after_key(key, source_array, insert)
 ```
 
 Insert an array after a specified key within another array.
@@ -418,15 +418,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.insert_before_key"></a>
 
-#### insert\_before\_key
+### insert\_before\_key
 
 ```python
 @staticmethod
 def insert_before_key(key, source_array, insert)
 ```
 
 Insert an array before a specified key within another array.
@@ -440,15 +440,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.is_dict"></a>
 
-#### is\_dict
+### is\_dict
 
 ```python
 @staticmethod
 def is_dict(array)
 ```
 
 Returns whether the array is a dict or not.
@@ -460,15 +460,15 @@
 
 **Returns**:
 
 - `boolean` - Whether the array is a dict or not.
 
 <a id="Arr.is_list"></a>
 
-#### is\_list
+### is\_list
 
 ```python
 @staticmethod
 def is_list(array)
 ```
 
 Returns whether the array is a list or not.
@@ -480,15 +480,15 @@
 
 **Returns**:
 
 - `boolean` - Whether the array is a list or not.
 
 <a id="Arr.join"></a>
 
-#### join
+### join
 
 ```python
 @staticmethod
 def join(array, glue, final_glue='')
 ```
 
 Join all items using a string. The final items can use a separate glue string.
@@ -502,15 +502,15 @@
 
 **Returns**:
 
 - `str` - Joined string.
 
 <a id="Arr.last"></a>
 
-#### last
+### last
 
 ```python
 @staticmethod
 def last(array, callback=None, default=None)
 ```
 
 Return the last element in an array passing a given truth test.
@@ -524,15 +524,15 @@
 
 **Returns**:
 
   Found value or default.
 
 <a id="Arr.list_to_array"></a>
 
-#### list\_to\_array
+### list\_to\_array
 
 ```python
 @staticmethod
 def list_to_array(value, sep=',')
 ```
 
 Converts a list to an array filtering out empty string elements.
@@ -547,15 +547,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.merge_recursive"></a>
 
-#### merge\_recursive
+### merge\_recursive
 
 ```python
 @staticmethod
 def merge_recursive(array1, array2)
 ```
 
 Recursively merge two arrays preserving keys.
@@ -568,15 +568,15 @@
 
 **Returns**:
 
   Merged array.
 
 <a id="Arr.only"></a>
 
-#### only
+### only
 
 ```python
 @staticmethod
 def only(array, keys)
 ```
 
 Get a subset of the items from the given array.
@@ -589,15 +589,15 @@
 
 **Returns**:
 
   Array subset.
 
 <a id="Arr.prepend"></a>
 
-#### prepend
+### prepend
 
 ```python
 @staticmethod
 def prepend(array, value, key=None)
 ```
 
 Push an item onto the beginning of an array.
@@ -611,15 +611,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.pull"></a>
 
-#### pull
+### pull
 
 ```python
 @staticmethod
 def pull(array, key, default=None)
 ```
 
 Get a value from the array, and remove it.
@@ -633,15 +633,15 @@
 
 **Returns**:
 
 - `Any` - The found value or default.
 
 <a id="Arr.query"></a>
 
-#### query
+### query
 
 ```python
 @staticmethod
 def query(data)
 ```
 
 Convert the array into a query string.
@@ -653,15 +653,15 @@
 
 **Returns**:
 
 - `str` - URL query string.
 
 <a id="Arr.random"></a>
 
-#### random
+### random
 
 ```python
 @staticmethod
 def random(array, number=None, preserve_keys=False)
 ```
 
 Get one or a specified number of random values from an array.
@@ -680,15 +680,15 @@
 
 **Returns**:
 
   Array with the random values.
 
 <a id="Arr.recursive_ksort"></a>
 
-#### recursive\_ksort
+### recursive\_ksort
 
 ```python
 @staticmethod
 def recursive_ksort(array)
 ```
 
 Recursively key-sort an array.
@@ -700,15 +700,15 @@
 
 **Returns**:
 
   Sorted array.
 
 <a id="Arr.set"></a>
 
-#### set
+### set
 
 ```python
 @staticmethod
 def set(array, keys, value)
 ```
 
 Set key/value within an array, can set a key nested inside of a multidimensional array.
@@ -724,15 +724,15 @@
 
 **Returns**:
 
   The manipulated array.
 
 <a id="Arr.shape_filter"></a>
 
-#### shape\_filter
+### shape\_filter
 
 ```python
 @staticmethod
 def shape_filter(array, shape)
 ```
 
 Shapes, filtering it, an array to the specified expected set of required keys.
@@ -747,15 +747,15 @@
 
 **Returns**:
 
   The manipulated array.
 
 <a id="Arr.shuffle"></a>
 
-#### shuffle
+### shuffle
 
 ```python
 @staticmethod
 def shuffle(array, seed=None)
 ```
 
 Shuffle the given array and return the result.
@@ -768,15 +768,15 @@
 
 **Returns**:
 
   The shuffled array.
 
 <a id="Arr.sort_by_priority"></a>
 
-#### sort\_by\_priority
+### sort\_by\_priority
 
 ```python
 @staticmethod
 def sort_by_priority(array)
 ```
 
 Sort based on Priority.
@@ -788,15 +788,15 @@
 
 **Returns**:
 
   Sorted dict.
 
 <a id="Arr.sort_recursive"></a>
 
-#### sort\_recursive
+### sort\_recursive
 
 ```python
 @staticmethod
 def sort_recursive(array, descending=False)
 ```
 
 Recursively sort an array by keys and values.
@@ -809,15 +809,15 @@
 
 **Returns**:
 
   Sorted array.
 
 <a id="Arr.sort_recursive_desc"></a>
 
-#### sort\_recursive\_desc
+### sort\_recursive\_desc
 
 ```python
 @staticmethod
 def sort_recursive_desc(array)
 ```
 
 Recursively sort an array by keys and values in descending order.
@@ -829,15 +829,15 @@
 
 **Returns**:
 
   Sorted array.
 
 <a id="Arr.stringify_keys"></a>
 
-#### stringify\_keys
+### stringify\_keys
 
 ```python
 @staticmethod
 def stringify_keys(input_array, prefix=None)
 ```
 
 Stringifies the numeric keys of an array.
@@ -850,15 +850,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.strpos"></a>
 
-#### strpos
+### strpos
 
 ```python
 @staticmethod
 def strpos(haystack, needles, offset=0)
 ```
 
 Behaves exactly like the native PHP's strpos(), but accepts an array of needles.
@@ -872,15 +872,15 @@
 
 **Returns**:
 
 - `_type_` - _description_
 
 <a id="Arr.to_list"></a>
 
-#### to\_list
+### to\_list
 
 ```python
 @staticmethod
 def to_list(list_items, sep=',')
 ```
 
 Returns a list separated by the specified separator.
@@ -893,15 +893,15 @@
 
 **Returns**:
 
   The list separated by the specified separator or the original list if the list is empty.
 
 <a id="Arr.undot"></a>
 
-#### undot
+### undot
 
 ```python
 @staticmethod
 def undot(obj)
 ```
 
 Convert a flatten "dot" notation array into an expanded array.
@@ -913,15 +913,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.usearch"></a>
 
-#### usearch
+### usearch
 
 ```python
 @staticmethod
 def usearch(needle, haystack, callback)
 ```
 
 Searches an array using a callback and returns the index of the first match.
@@ -936,15 +936,15 @@
 
 **Returns**:
 
   Either the index of the first match or False if no match was found.
 
 <a id="Arr.where"></a>
 
-#### where
+### where
 
 ```python
 @staticmethod
 def where(array, callback)
 ```
 
 Filter the array using the given callback.
@@ -957,15 +957,15 @@
 
 **Returns**:
 
   The filtered array.
 
 <a id="Arr.where_not_none"></a>
 
-#### where\_not\_none
+### where\_not\_none
 
 ```python
 @staticmethod
 def where_not_none(array)
 ```
 
 Filter items where the value is not None.
@@ -977,15 +977,15 @@
 
 **Returns**:
 
   The filtered array.
 
 <a id="Arr.wrap"></a>
 
-#### wrap
+### wrap
 
 ```python
 @staticmethod
 def wrap(value)
 ```
 
 If the given value is not a list, dict, or UserDict and not None, wrap it in one.
```

### Comparing `arrayutilities-1.0.1/README.md` & `arrayutilities-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 ```python
 from arrayutilities import Arr
 ```
 
 <a id="Arr.accessible"></a>
 
-#### accessible
+### accessible
 
 ```python
 @staticmethod
 def accessible(value)
 ```
 
 Determines if the given value is a list, dict, or UserDict.
@@ -86,15 +86,15 @@
 
 **Returns**:
 
 - `boolean` - Whether the the value is a list, dict, or UserDict.
 
 <a id="Arr.add"></a>
 
-#### add
+### add
 
 ```python
 @staticmethod
 def add(array, key, value)
 ```
 
 Add an element to an array if it doesn't exist.
@@ -108,15 +108,15 @@
 
 **Returns**:
 
   Manipulated array
 
 <a id="Arr.add_prefixed_keys_to"></a>
 
-#### add\_prefixed\_keys\_to
+### add\_prefixed\_keys\_to
 
 ```python
 @staticmethod
 def add_prefixed_keys_to(array, recursive=False)
 ```
 
 Duplicates any key not prefixed with '_' creating a prefixed duplicate one.
@@ -129,15 +129,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.add_unprefixed_keys_to"></a>
 
-#### add\_unprefixed\_keys\_to
+### add\_unprefixed\_keys\_to
 
 ```python
 @staticmethod
 def add_unprefixed_keys_to(array, recursive=False)
 ```
 
 Duplicates any key prefixed with '_' creating an un-prefixed duplicate one.
@@ -150,15 +150,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.array_visit_recursive"></a>
 
-#### array\_visit\_recursive
+### array\_visit\_recursive
 
 ```python
 @staticmethod
 def array_visit_recursive(input_array, visitor)
 ```
 
 Recursively visits all elements of an array applying the specified callback to each element key and value.
@@ -174,15 +174,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.collapse"></a>
 
-#### collapse
+### collapse
 
 ```python
 @staticmethod
 def collapse(array)
 ```
 
 Collapse an array of arrays into a single array.
@@ -194,15 +194,15 @@
 
 **Returns**:
 
   Collapsed array.
 
 <a id="Arr.dot"></a>
 
-#### dot
+### dot
 
 ```python
 @staticmethod
 def dot(array, prepend='')
 ```
 
 Flatten a multi-dimensional associative array with dots.
@@ -215,15 +215,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.exists"></a>
 
-#### exists
+### exists
 
 ```python
 @staticmethod
 def exists(array, key)
 ```
 
 Determine if the given key exists in the provided array.
@@ -236,15 +236,15 @@
 
 **Returns**:
 
 - `boolean` - Whether or not the key exists.
 
 <a id="Arr.filter_prefixed"></a>
 
-#### filter\_prefixed
+### filter\_prefixed
 
 ```python
 @staticmethod
 def filter_prefixed(array, prefix)
 ```
 
 Filters an associative array non-recursively, keeping only the values attached to keys starting with the specified prefix.
@@ -257,15 +257,15 @@
 
 **Returns**:
 
   Filtered array.
 
 <a id="Arr.first"></a>
 
-#### first
+### first
 
 ```python
 @staticmethod
 def first(array, callback=None, default=None)
 ```
 
 Return the first element in an array passing a given truth test.
@@ -279,15 +279,15 @@
 
 **Returns**:
 
   Found value or default.
 
 <a id="Arr.flatten"></a>
 
-#### flatten
+### flatten
 
 ```python
 @staticmethod
 def flatten(array, depth=float('inf'))
 ```
 
 Flatten a multi-dimensional array into a single level.
@@ -300,15 +300,15 @@
 
 **Returns**:
 
   Flattened array.
 
 <a id="Arr.forget"></a>
 
-#### forget
+### forget
 
 ```python
 @staticmethod
 def forget(array, keys)
 ```
 
 Remove one or many array items from a given array using "dot" notation.
@@ -316,15 +316,15 @@
 **Arguments**:
 
 - `array` - Array to manipulate.
 - `keys` _str|array_ - Key or keys to remove.
 
 <a id="Arr.get"></a>
 
-#### get
+### get
 
 ```python
 @staticmethod
 def get(array, keys, default=None)
 ```
 
 Find a value inside of an array or object, including one nested a few levels deep.
@@ -338,15 +338,15 @@
 
 **Returns**:
 
 - `_type_` - _description_
 
 <a id="Arr.has"></a>
 
-#### has
+### has
 
 ```python
 @staticmethod
 def has(array, keys)
 ```
 
 Check if an item or items exist in an array using "dot" notation.
@@ -359,15 +359,15 @@
 
 **Returns**:
 
 - `boolean` - Whether the key exists or not.
 
 <a id="Arr.insert_after_key"></a>
 
-#### insert\_after\_key
+### insert\_after\_key
 
 ```python
 @staticmethod
 def insert_after_key(key, source_array, insert)
 ```
 
 Insert an array after a specified key within another array.
@@ -381,15 +381,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.insert_before_key"></a>
 
-#### insert\_before\_key
+### insert\_before\_key
 
 ```python
 @staticmethod
 def insert_before_key(key, source_array, insert)
 ```
 
 Insert an array before a specified key within another array.
@@ -403,15 +403,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.is_dict"></a>
 
-#### is\_dict
+### is\_dict
 
 ```python
 @staticmethod
 def is_dict(array)
 ```
 
 Returns whether the array is a dict or not.
@@ -423,15 +423,15 @@
 
 **Returns**:
 
 - `boolean` - Whether the array is a dict or not.
 
 <a id="Arr.is_list"></a>
 
-#### is\_list
+### is\_list
 
 ```python
 @staticmethod
 def is_list(array)
 ```
 
 Returns whether the array is a list or not.
@@ -443,15 +443,15 @@
 
 **Returns**:
 
 - `boolean` - Whether the array is a list or not.
 
 <a id="Arr.join"></a>
 
-#### join
+### join
 
 ```python
 @staticmethod
 def join(array, glue, final_glue='')
 ```
 
 Join all items using a string. The final items can use a separate glue string.
@@ -465,15 +465,15 @@
 
 **Returns**:
 
 - `str` - Joined string.
 
 <a id="Arr.last"></a>
 
-#### last
+### last
 
 ```python
 @staticmethod
 def last(array, callback=None, default=None)
 ```
 
 Return the last element in an array passing a given truth test.
@@ -487,15 +487,15 @@
 
 **Returns**:
 
   Found value or default.
 
 <a id="Arr.list_to_array"></a>
 
-#### list\_to\_array
+### list\_to\_array
 
 ```python
 @staticmethod
 def list_to_array(value, sep=',')
 ```
 
 Converts a list to an array filtering out empty string elements.
@@ -510,15 +510,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.merge_recursive"></a>
 
-#### merge\_recursive
+### merge\_recursive
 
 ```python
 @staticmethod
 def merge_recursive(array1, array2)
 ```
 
 Recursively merge two arrays preserving keys.
@@ -531,15 +531,15 @@
 
 **Returns**:
 
   Merged array.
 
 <a id="Arr.only"></a>
 
-#### only
+### only
 
 ```python
 @staticmethod
 def only(array, keys)
 ```
 
 Get a subset of the items from the given array.
@@ -552,15 +552,15 @@
 
 **Returns**:
 
   Array subset.
 
 <a id="Arr.prepend"></a>
 
-#### prepend
+### prepend
 
 ```python
 @staticmethod
 def prepend(array, value, key=None)
 ```
 
 Push an item onto the beginning of an array.
@@ -574,15 +574,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.pull"></a>
 
-#### pull
+### pull
 
 ```python
 @staticmethod
 def pull(array, key, default=None)
 ```
 
 Get a value from the array, and remove it.
@@ -596,15 +596,15 @@
 
 **Returns**:
 
 - `Any` - The found value or default.
 
 <a id="Arr.query"></a>
 
-#### query
+### query
 
 ```python
 @staticmethod
 def query(data)
 ```
 
 Convert the array into a query string.
@@ -616,15 +616,15 @@
 
 **Returns**:
 
 - `str` - URL query string.
 
 <a id="Arr.random"></a>
 
-#### random
+### random
 
 ```python
 @staticmethod
 def random(array, number=None, preserve_keys=False)
 ```
 
 Get one or a specified number of random values from an array.
@@ -643,15 +643,15 @@
 
 **Returns**:
 
   Array with the random values.
 
 <a id="Arr.recursive_ksort"></a>
 
-#### recursive\_ksort
+### recursive\_ksort
 
 ```python
 @staticmethod
 def recursive_ksort(array)
 ```
 
 Recursively key-sort an array.
@@ -663,15 +663,15 @@
 
 **Returns**:
 
   Sorted array.
 
 <a id="Arr.set"></a>
 
-#### set
+### set
 
 ```python
 @staticmethod
 def set(array, keys, value)
 ```
 
 Set key/value within an array, can set a key nested inside of a multidimensional array.
@@ -687,15 +687,15 @@
 
 **Returns**:
 
   The manipulated array.
 
 <a id="Arr.shape_filter"></a>
 
-#### shape\_filter
+### shape\_filter
 
 ```python
 @staticmethod
 def shape_filter(array, shape)
 ```
 
 Shapes, filtering it, an array to the specified expected set of required keys.
@@ -710,15 +710,15 @@
 
 **Returns**:
 
   The manipulated array.
 
 <a id="Arr.shuffle"></a>
 
-#### shuffle
+### shuffle
 
 ```python
 @staticmethod
 def shuffle(array, seed=None)
 ```
 
 Shuffle the given array and return the result.
@@ -731,15 +731,15 @@
 
 **Returns**:
 
   The shuffled array.
 
 <a id="Arr.sort_by_priority"></a>
 
-#### sort\_by\_priority
+### sort\_by\_priority
 
 ```python
 @staticmethod
 def sort_by_priority(array)
 ```
 
 Sort based on Priority.
@@ -751,15 +751,15 @@
 
 **Returns**:
 
   Sorted dict.
 
 <a id="Arr.sort_recursive"></a>
 
-#### sort\_recursive
+### sort\_recursive
 
 ```python
 @staticmethod
 def sort_recursive(array, descending=False)
 ```
 
 Recursively sort an array by keys and values.
@@ -772,15 +772,15 @@
 
 **Returns**:
 
   Sorted array.
 
 <a id="Arr.sort_recursive_desc"></a>
 
-#### sort\_recursive\_desc
+### sort\_recursive\_desc
 
 ```python
 @staticmethod
 def sort_recursive_desc(array)
 ```
 
 Recursively sort an array by keys and values in descending order.
@@ -792,15 +792,15 @@
 
 **Returns**:
 
   Sorted array.
 
 <a id="Arr.stringify_keys"></a>
 
-#### stringify\_keys
+### stringify\_keys
 
 ```python
 @staticmethod
 def stringify_keys(input_array, prefix=None)
 ```
 
 Stringifies the numeric keys of an array.
@@ -813,15 +813,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.strpos"></a>
 
-#### strpos
+### strpos
 
 ```python
 @staticmethod
 def strpos(haystack, needles, offset=0)
 ```
 
 Behaves exactly like the native PHP's strpos(), but accepts an array of needles.
@@ -835,15 +835,15 @@
 
 **Returns**:
 
 - `_type_` - _description_
 
 <a id="Arr.to_list"></a>
 
-#### to\_list
+### to\_list
 
 ```python
 @staticmethod
 def to_list(list_items, sep=',')
 ```
 
 Returns a list separated by the specified separator.
@@ -856,15 +856,15 @@
 
 **Returns**:
 
   The list separated by the specified separator or the original list if the list is empty.
 
 <a id="Arr.undot"></a>
 
-#### undot
+### undot
 
 ```python
 @staticmethod
 def undot(obj)
 ```
 
 Convert a flatten "dot" notation array into an expanded array.
@@ -876,15 +876,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.usearch"></a>
 
-#### usearch
+### usearch
 
 ```python
 @staticmethod
 def usearch(needle, haystack, callback)
 ```
 
 Searches an array using a callback and returns the index of the first match.
@@ -899,15 +899,15 @@
 
 **Returns**:
 
   Either the index of the first match or False if no match was found.
 
 <a id="Arr.where"></a>
 
-#### where
+### where
 
 ```python
 @staticmethod
 def where(array, callback)
 ```
 
 Filter the array using the given callback.
@@ -920,15 +920,15 @@
 
 **Returns**:
 
   The filtered array.
 
 <a id="Arr.where_not_none"></a>
 
-#### where\_not\_none
+### where\_not\_none
 
 ```python
 @staticmethod
 def where_not_none(array)
 ```
 
 Filter items where the value is not None.
@@ -940,15 +940,15 @@
 
 **Returns**:
 
   The filtered array.
 
 <a id="Arr.wrap"></a>
 
-#### wrap
+### wrap
 
 ```python
 @staticmethod
 def wrap(value)
 ```
 
 If the given value is not a list, dict, or UserDict and not None, wrap it in one.
```

### Comparing `arrayutilities-1.0.1/arrayutilities/__init__.py` & `arrayutilities-1.0.2/arrayutilities/__init__.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/arrayutilities.egg-info/PKG-INFO` & `arrayutilities-1.0.2/arrayutilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrayutilities
-Version: 1.0.1
+Version: 1.0.2
 Summary: A library for list, dict, and UserDict manipulations.
 Author: Matthew Batchelder
 Author-email: Matthew Batchelder <borkweb@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Matthew Batchelder
         
@@ -103,15 +103,15 @@
 
 ```python
 from arrayutilities import Arr
 ```
 
 <a id="Arr.accessible"></a>
 
-#### accessible
+### accessible
 
 ```python
 @staticmethod
 def accessible(value)
 ```
 
 Determines if the given value is a list, dict, or UserDict.
@@ -123,15 +123,15 @@
 
 **Returns**:
 
 - `boolean` - Whether the the value is a list, dict, or UserDict.
 
 <a id="Arr.add"></a>
 
-#### add
+### add
 
 ```python
 @staticmethod
 def add(array, key, value)
 ```
 
 Add an element to an array if it doesn't exist.
@@ -145,15 +145,15 @@
 
 **Returns**:
 
   Manipulated array
 
 <a id="Arr.add_prefixed_keys_to"></a>
 
-#### add\_prefixed\_keys\_to
+### add\_prefixed\_keys\_to
 
 ```python
 @staticmethod
 def add_prefixed_keys_to(array, recursive=False)
 ```
 
 Duplicates any key not prefixed with '_' creating a prefixed duplicate one.
@@ -166,15 +166,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.add_unprefixed_keys_to"></a>
 
-#### add\_unprefixed\_keys\_to
+### add\_unprefixed\_keys\_to
 
 ```python
 @staticmethod
 def add_unprefixed_keys_to(array, recursive=False)
 ```
 
 Duplicates any key prefixed with '_' creating an un-prefixed duplicate one.
@@ -187,15 +187,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.array_visit_recursive"></a>
 
-#### array\_visit\_recursive
+### array\_visit\_recursive
 
 ```python
 @staticmethod
 def array_visit_recursive(input_array, visitor)
 ```
 
 Recursively visits all elements of an array applying the specified callback to each element key and value.
@@ -211,15 +211,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.collapse"></a>
 
-#### collapse
+### collapse
 
 ```python
 @staticmethod
 def collapse(array)
 ```
 
 Collapse an array of arrays into a single array.
@@ -231,15 +231,15 @@
 
 **Returns**:
 
   Collapsed array.
 
 <a id="Arr.dot"></a>
 
-#### dot
+### dot
 
 ```python
 @staticmethod
 def dot(array, prepend='')
 ```
 
 Flatten a multi-dimensional associative array with dots.
@@ -252,15 +252,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.exists"></a>
 
-#### exists
+### exists
 
 ```python
 @staticmethod
 def exists(array, key)
 ```
 
 Determine if the given key exists in the provided array.
@@ -273,15 +273,15 @@
 
 **Returns**:
 
 - `boolean` - Whether or not the key exists.
 
 <a id="Arr.filter_prefixed"></a>
 
-#### filter\_prefixed
+### filter\_prefixed
 
 ```python
 @staticmethod
 def filter_prefixed(array, prefix)
 ```
 
 Filters an associative array non-recursively, keeping only the values attached to keys starting with the specified prefix.
@@ -294,15 +294,15 @@
 
 **Returns**:
 
   Filtered array.
 
 <a id="Arr.first"></a>
 
-#### first
+### first
 
 ```python
 @staticmethod
 def first(array, callback=None, default=None)
 ```
 
 Return the first element in an array passing a given truth test.
@@ -316,15 +316,15 @@
 
 **Returns**:
 
   Found value or default.
 
 <a id="Arr.flatten"></a>
 
-#### flatten
+### flatten
 
 ```python
 @staticmethod
 def flatten(array, depth=float('inf'))
 ```
 
 Flatten a multi-dimensional array into a single level.
@@ -337,15 +337,15 @@
 
 **Returns**:
 
   Flattened array.
 
 <a id="Arr.forget"></a>
 
-#### forget
+### forget
 
 ```python
 @staticmethod
 def forget(array, keys)
 ```
 
 Remove one or many array items from a given array using "dot" notation.
@@ -353,15 +353,15 @@
 **Arguments**:
 
 - `array` - Array to manipulate.
 - `keys` _str|array_ - Key or keys to remove.
 
 <a id="Arr.get"></a>
 
-#### get
+### get
 
 ```python
 @staticmethod
 def get(array, keys, default=None)
 ```
 
 Find a value inside of an array or object, including one nested a few levels deep.
@@ -375,15 +375,15 @@
 
 **Returns**:
 
 - `_type_` - _description_
 
 <a id="Arr.has"></a>
 
-#### has
+### has
 
 ```python
 @staticmethod
 def has(array, keys)
 ```
 
 Check if an item or items exist in an array using "dot" notation.
@@ -396,15 +396,15 @@
 
 **Returns**:
 
 - `boolean` - Whether the key exists or not.
 
 <a id="Arr.insert_after_key"></a>
 
-#### insert\_after\_key
+### insert\_after\_key
 
 ```python
 @staticmethod
 def insert_after_key(key, source_array, insert)
 ```
 
 Insert an array after a specified key within another array.
@@ -418,15 +418,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.insert_before_key"></a>
 
-#### insert\_before\_key
+### insert\_before\_key
 
 ```python
 @staticmethod
 def insert_before_key(key, source_array, insert)
 ```
 
 Insert an array before a specified key within another array.
@@ -440,15 +440,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.is_dict"></a>
 
-#### is\_dict
+### is\_dict
 
 ```python
 @staticmethod
 def is_dict(array)
 ```
 
 Returns whether the array is a dict or not.
@@ -460,15 +460,15 @@
 
 **Returns**:
 
 - `boolean` - Whether the array is a dict or not.
 
 <a id="Arr.is_list"></a>
 
-#### is\_list
+### is\_list
 
 ```python
 @staticmethod
 def is_list(array)
 ```
 
 Returns whether the array is a list or not.
@@ -480,15 +480,15 @@
 
 **Returns**:
 
 - `boolean` - Whether the array is a list or not.
 
 <a id="Arr.join"></a>
 
-#### join
+### join
 
 ```python
 @staticmethod
 def join(array, glue, final_glue='')
 ```
 
 Join all items using a string. The final items can use a separate glue string.
@@ -502,15 +502,15 @@
 
 **Returns**:
 
 - `str` - Joined string.
 
 <a id="Arr.last"></a>
 
-#### last
+### last
 
 ```python
 @staticmethod
 def last(array, callback=None, default=None)
 ```
 
 Return the last element in an array passing a given truth test.
@@ -524,15 +524,15 @@
 
 **Returns**:
 
   Found value or default.
 
 <a id="Arr.list_to_array"></a>
 
-#### list\_to\_array
+### list\_to\_array
 
 ```python
 @staticmethod
 def list_to_array(value, sep=',')
 ```
 
 Converts a list to an array filtering out empty string elements.
@@ -547,15 +547,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.merge_recursive"></a>
 
-#### merge\_recursive
+### merge\_recursive
 
 ```python
 @staticmethod
 def merge_recursive(array1, array2)
 ```
 
 Recursively merge two arrays preserving keys.
@@ -568,15 +568,15 @@
 
 **Returns**:
 
   Merged array.
 
 <a id="Arr.only"></a>
 
-#### only
+### only
 
 ```python
 @staticmethod
 def only(array, keys)
 ```
 
 Get a subset of the items from the given array.
@@ -589,15 +589,15 @@
 
 **Returns**:
 
   Array subset.
 
 <a id="Arr.prepend"></a>
 
-#### prepend
+### prepend
 
 ```python
 @staticmethod
 def prepend(array, value, key=None)
 ```
 
 Push an item onto the beginning of an array.
@@ -611,15 +611,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.pull"></a>
 
-#### pull
+### pull
 
 ```python
 @staticmethod
 def pull(array, key, default=None)
 ```
 
 Get a value from the array, and remove it.
@@ -633,15 +633,15 @@
 
 **Returns**:
 
 - `Any` - The found value or default.
 
 <a id="Arr.query"></a>
 
-#### query
+### query
 
 ```python
 @staticmethod
 def query(data)
 ```
 
 Convert the array into a query string.
@@ -653,15 +653,15 @@
 
 **Returns**:
 
 - `str` - URL query string.
 
 <a id="Arr.random"></a>
 
-#### random
+### random
 
 ```python
 @staticmethod
 def random(array, number=None, preserve_keys=False)
 ```
 
 Get one or a specified number of random values from an array.
@@ -680,15 +680,15 @@
 
 **Returns**:
 
   Array with the random values.
 
 <a id="Arr.recursive_ksort"></a>
 
-#### recursive\_ksort
+### recursive\_ksort
 
 ```python
 @staticmethod
 def recursive_ksort(array)
 ```
 
 Recursively key-sort an array.
@@ -700,15 +700,15 @@
 
 **Returns**:
 
   Sorted array.
 
 <a id="Arr.set"></a>
 
-#### set
+### set
 
 ```python
 @staticmethod
 def set(array, keys, value)
 ```
 
 Set key/value within an array, can set a key nested inside of a multidimensional array.
@@ -724,15 +724,15 @@
 
 **Returns**:
 
   The manipulated array.
 
 <a id="Arr.shape_filter"></a>
 
-#### shape\_filter
+### shape\_filter
 
 ```python
 @staticmethod
 def shape_filter(array, shape)
 ```
 
 Shapes, filtering it, an array to the specified expected set of required keys.
@@ -747,15 +747,15 @@
 
 **Returns**:
 
   The manipulated array.
 
 <a id="Arr.shuffle"></a>
 
-#### shuffle
+### shuffle
 
 ```python
 @staticmethod
 def shuffle(array, seed=None)
 ```
 
 Shuffle the given array and return the result.
@@ -768,15 +768,15 @@
 
 **Returns**:
 
   The shuffled array.
 
 <a id="Arr.sort_by_priority"></a>
 
-#### sort\_by\_priority
+### sort\_by\_priority
 
 ```python
 @staticmethod
 def sort_by_priority(array)
 ```
 
 Sort based on Priority.
@@ -788,15 +788,15 @@
 
 **Returns**:
 
   Sorted dict.
 
 <a id="Arr.sort_recursive"></a>
 
-#### sort\_recursive
+### sort\_recursive
 
 ```python
 @staticmethod
 def sort_recursive(array, descending=False)
 ```
 
 Recursively sort an array by keys and values.
@@ -809,15 +809,15 @@
 
 **Returns**:
 
   Sorted array.
 
 <a id="Arr.sort_recursive_desc"></a>
 
-#### sort\_recursive\_desc
+### sort\_recursive\_desc
 
 ```python
 @staticmethod
 def sort_recursive_desc(array)
 ```
 
 Recursively sort an array by keys and values in descending order.
@@ -829,15 +829,15 @@
 
 **Returns**:
 
   Sorted array.
 
 <a id="Arr.stringify_keys"></a>
 
-#### stringify\_keys
+### stringify\_keys
 
 ```python
 @staticmethod
 def stringify_keys(input_array, prefix=None)
 ```
 
 Stringifies the numeric keys of an array.
@@ -850,15 +850,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.strpos"></a>
 
-#### strpos
+### strpos
 
 ```python
 @staticmethod
 def strpos(haystack, needles, offset=0)
 ```
 
 Behaves exactly like the native PHP's strpos(), but accepts an array of needles.
@@ -872,15 +872,15 @@
 
 **Returns**:
 
 - `_type_` - _description_
 
 <a id="Arr.to_list"></a>
 
-#### to\_list
+### to\_list
 
 ```python
 @staticmethod
 def to_list(list_items, sep=',')
 ```
 
 Returns a list separated by the specified separator.
@@ -893,15 +893,15 @@
 
 **Returns**:
 
   The list separated by the specified separator or the original list if the list is empty.
 
 <a id="Arr.undot"></a>
 
-#### undot
+### undot
 
 ```python
 @staticmethod
 def undot(obj)
 ```
 
 Convert a flatten "dot" notation array into an expanded array.
@@ -913,15 +913,15 @@
 
 **Returns**:
 
   Manipulated array.
 
 <a id="Arr.usearch"></a>
 
-#### usearch
+### usearch
 
 ```python
 @staticmethod
 def usearch(needle, haystack, callback)
 ```
 
 Searches an array using a callback and returns the index of the first match.
@@ -936,15 +936,15 @@
 
 **Returns**:
 
   Either the index of the first match or False if no match was found.
 
 <a id="Arr.where"></a>
 
-#### where
+### where
 
 ```python
 @staticmethod
 def where(array, callback)
 ```
 
 Filter the array using the given callback.
@@ -957,15 +957,15 @@
 
 **Returns**:
 
   The filtered array.
 
 <a id="Arr.where_not_none"></a>
 
-#### where\_not\_none
+### where\_not\_none
 
 ```python
 @staticmethod
 def where_not_none(array)
 ```
 
 Filter items where the value is not None.
@@ -977,15 +977,15 @@
 
 **Returns**:
 
   The filtered array.
 
 <a id="Arr.wrap"></a>
 
-#### wrap
+### wrap
 
 ```python
 @staticmethod
 def wrap(value)
 ```
 
 If the given value is not a list, dict, or UserDict and not None, wrap it in one.
```

### Comparing `arrayutilities-1.0.1/arrayutilities.egg-info/SOURCES.txt` & `arrayutilities-1.0.2/arrayutilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/pyproject.toml` & `arrayutilities-1.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-sysetm]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "arrayutilities"
-version = "1.0.1"
+version = "1.0.2"
 description = "A library for list, dict, and UserDict manipulations."
 readme = "README.md"
 authors = [{ name = "Matthew Batchelder", email = "borkweb@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `arrayutilities-1.0.1/tests/test_accessible.py` & `arrayutilities-1.0.2/tests/test_accessible.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_add.py` & `arrayutilities-1.0.2/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_add_prefixed_keys_to.py` & `arrayutilities-1.0.2/tests/test_add_prefixed_keys_to.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_add_unprefixed_keys_to.py` & `arrayutilities-1.0.2/tests/test_add_unprefixed_keys_to.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_array_visit_recursive.py` & `arrayutilities-1.0.2/tests/test_array_visit_recursive.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_collapse.py` & `arrayutilities-1.0.2/tests/test_collapse.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_dot.py` & `arrayutilities-1.0.2/tests/test_dot.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_exists.py` & `arrayutilities-1.0.2/tests/test_exists.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_filter_prefixed.py` & `arrayutilities-1.0.2/tests/test_filter_prefixed.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_first.py` & `arrayutilities-1.0.2/tests/test_first.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_flatten.py` & `arrayutilities-1.0.2/tests/test_flatten.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_forget.py` & `arrayutilities-1.0.2/tests/test_forget.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_get.py` & `arrayutilities-1.0.2/tests/test_get.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_has.py` & `arrayutilities-1.0.2/tests/test_has.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_insert_after_key.py` & `arrayutilities-1.0.2/tests/test_insert_after_key.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_insert_before_key.py` & `arrayutilities-1.0.2/tests/test_insert_before_key.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_is_dict.py` & `arrayutilities-1.0.2/tests/test_is_dict.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_is_list.py` & `arrayutilities-1.0.2/tests/test_is_list.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_join.py` & `arrayutilities-1.0.2/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_last.py` & `arrayutilities-1.0.2/tests/test_last.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_list_to_array.py` & `arrayutilities-1.0.2/tests/test_list_to_array.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_merge_recursive.py` & `arrayutilities-1.0.2/tests/test_merge_recursive.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_only.py` & `arrayutilities-1.0.2/tests/test_only.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_prepend.py` & `arrayutilities-1.0.2/tests/test_prepend.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_pull.py` & `arrayutilities-1.0.2/tests/test_pull.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_query.py` & `arrayutilities-1.0.2/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_random.py` & `arrayutilities-1.0.2/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_recursive_ksort.py` & `arrayutilities-1.0.2/tests/test_recursive_ksort.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_set.py` & `arrayutilities-1.0.2/tests/test_set.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_shape_filter.py` & `arrayutilities-1.0.2/tests/test_shape_filter.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_shuffle.py` & `arrayutilities-1.0.2/tests/test_shuffle.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_sort_by_priority.py` & `arrayutilities-1.0.2/tests/test_sort_by_priority.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_sort_recursive.py` & `arrayutilities-1.0.2/tests/test_sort_recursive.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_stringify_keys.py` & `arrayutilities-1.0.2/tests/test_stringify_keys.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_strpos.py` & `arrayutilities-1.0.2/tests/test_strpos.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_to_list.py` & `arrayutilities-1.0.2/tests/test_to_list.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_undot.py` & `arrayutilities-1.0.2/tests/test_undot.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_usearch.py` & `arrayutilities-1.0.2/tests/test_usearch.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_where.py` & `arrayutilities-1.0.2/tests/test_where.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_where_not_none.py` & `arrayutilities-1.0.2/tests/test_where_not_none.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.1/tests/test_wrap.py` & `arrayutilities-1.0.2/tests/test_wrap.py`

 * *Files identical despite different names*

