# Comparing `tmp/func_adl-3.3.1b3.tar.gz` & `tmp/func_adl-3.3.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/func_adl-3.3.1b3.tar", last modified: Sat Apr 27 06:44:37 2024, max compression
+gzip compressed data, was "dist/func_adl-3.3.1b4.tar", last modified: Sat Apr 27 07:07:32 2024, max compression
```

## Comparing `func_adl-3.3.1b3.tar` & `func_adl-3.3.1b4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/func_adl/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/func_adl/ast/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/ast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/ast/aggregate_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/ast/ast_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/ast/call_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/ast/func_adl_ast_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20311 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/ast/function_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/ast/meta_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/ast/syntatic_sugar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/event_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15904 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/object_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    37909 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/type_based_replacement.py
--rw-r--r--   0 runner    (1001) docker     (127)    24565 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/util_ast.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/util_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/func_adl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/func_adl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/func_adl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/func_adl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/func_adl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/func_adl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/tests/test_event_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/tests/test_object_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    33178 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/tests/test_type_based_replacement.py
--rw-r--r--   0 runner    (1001) docker     (127)    16732 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/tests/test_type_based_replacement_py310.py
--rw-r--r--   0 runner    (1001) docker     (127)    22510 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/tests/test_util_ast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/tests/test_util_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:07:32.000000 func_adl-3.3.1b4/
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-27 07:07:32.000000 func_adl-3.3.1b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:07:32.000000 func_adl-3.3.1b4/func_adl/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/func_adl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:07:32.000000 func_adl-3.3.1b4/func_adl/ast/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/func_adl/ast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/func_adl/ast/aggregate_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/func_adl/ast/ast_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/func_adl/ast/call_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/func_adl/ast/func_adl_ast_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20311 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/func_adl/ast/function_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/func_adl/ast/meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/func_adl/ast/syntatic_sugar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/func_adl/event_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/func_adl/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15904 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/func_adl/object_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38265 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/func_adl/type_based_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24565 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/func_adl/util_ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/func_adl/util_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:07:32.000000 func_adl-3.3.1b4/func_adl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-27 07:07:32.000000 func_adl-3.3.1b4/func_adl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-27 07:07:32.000000 func_adl-3.3.1b4/func_adl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 07:07:32.000000 func_adl-3.3.1b4/func_adl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-27 07:07:32.000000 func_adl-3.3.1b4/func_adl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 07:07:32.000000 func_adl-3.3.1b4/func_adl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 07:07:32.000000 func_adl-3.3.1b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:07:32.000000 func_adl-3.3.1b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/tests/test_event_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/tests/test_object_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33630 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/tests/test_type_based_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16732 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/tests/test_type_based_replacement_py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22510 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/tests/test_util_ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-27 07:07:28.000000 func_adl-3.3.1b4/tests/test_util_types.py
```

### Comparing `func_adl-3.3.1b3/PKG-INFO` & `func_adl-3.3.1b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func_adl
-Version: 3.3.1b3
+Version: 3.3.1b4
 Summary: Functional Analysis Description Language Base Package
 Home-page: https://github.com/iris-hep/func_adl
 Author: G. Watts (IRIS-HEP/UW Seattle)
 Author-email: gwatts@uw.edu
 Maintainer: Gordon Watts (IRIS-HEP/UW Seattle)
 Maintainer-email: gwatts@uw.edu
 License: MIT
```

### Comparing `func_adl-3.3.1b3/README.md` & `func_adl-3.3.1b4/README.md`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b3/func_adl/ast/aggregate_shortcuts.py` & `func_adl-3.3.1b4/func_adl/ast/aggregate_shortcuts.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b3/func_adl/ast/call_stack.py` & `func_adl-3.3.1b4/func_adl/ast/call_stack.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b3/func_adl/ast/func_adl_ast_utils.py` & `func_adl-3.3.1b4/func_adl/ast/func_adl_ast_utils.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b3/func_adl/ast/function_simplifier.py` & `func_adl-3.3.1b4/func_adl/ast/function_simplifier.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b3/func_adl/ast/meta_data.py` & `func_adl-3.3.1b4/func_adl/ast/meta_data.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b3/func_adl/ast/syntatic_sugar.py` & `func_adl-3.3.1b4/func_adl/ast/syntatic_sugar.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b3/func_adl/event_dataset.py` & `func_adl-3.3.1b4/func_adl/event_dataset.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b3/func_adl/functions.py` & `func_adl-3.3.1b4/func_adl/functions.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b3/func_adl/object_stream.py` & `func_adl-3.3.1b4/func_adl/object_stream.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b3/func_adl/type_based_replacement.py` & `func_adl-3.3.1b4/func_adl/type_based_replacement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import ast
 import copy
 import inspect
 import logging
 import sys
-from dataclasses import dataclass, make_dataclass
+from dataclasses import dataclass, is_dataclass, make_dataclass
 from typing import (
     Any,
     Callable,
     Dict,
     Generic,
     Iterable,
     List,
@@ -967,14 +967,19 @@
                 key_index = [
                     e for e, k in enumerate(t_node.value.keys) if k.value == key  # type: ignore
                 ]
                 if len(key_index) == 0:
                     raise ValueError(f"Key {key} not found in dict expression!!")
                 value = t_node.value.values[key_index[0]]
                 self._found_types[node] = self.lookup_type(value)
+            elif ((dc := self.lookup_type(t_node.value)) is not None) and is_dataclass(dc):
+                dc_types = get_type_hints(dc)
+                if node.attr not in dc_types:
+                    raise ValueError(f"Key {node.attr} not found in dataclass/dictionary {dc}")
+                self._found_types[node] = dc_types[node.attr]
             return t_node
 
     tt = type_transformer(o_stream)
     r_a = tt.visit(a)
 
     return tt.stream, r_a, tt.lookup_type(a)
```

### Comparing `func_adl-3.3.1b3/func_adl/util_ast.py` & `func_adl-3.3.1b4/func_adl/util_ast.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b3/func_adl/util_types.py` & `func_adl-3.3.1b4/func_adl/util_types.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b3/func_adl.egg-info/PKG-INFO` & `func_adl-3.3.1b4/func_adl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func-adl
-Version: 3.3.1b3
+Version: 3.3.1b4
 Summary: Functional Analysis Description Language Base Package
 Home-page: https://github.com/iris-hep/func_adl
 Author: G. Watts (IRIS-HEP/UW Seattle)
 Author-email: gwatts@uw.edu
 Maintainer: Gordon Watts (IRIS-HEP/UW Seattle)
 Maintainer-email: gwatts@uw.edu
 License: MIT
```

### Comparing `func_adl-3.3.1b3/func_adl.egg-info/SOURCES.txt` & `func_adl-3.3.1b4/func_adl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b3/setup.py` & `func_adl-3.3.1b4/setup.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b3/tests/test_event_dataset.py` & `func_adl-3.3.1b4/tests/test_event_dataset.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b3/tests/test_object_stream.py` & `func_adl-3.3.1b4/tests/test_object_stream.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b3/tests/test_type_based_replacement.py` & `func_adl-3.3.1b4/tests/test_type_based_replacement.py`

 * *Files 2% similar despite different names*

```diff
@@ -560,14 +560,28 @@
     sig = inspect.signature(obj_itr.__init__)
     assert len(sig.parameters) == 3
     assert "pt" in sig.parameters
     j_info = sig.parameters["pt"]
     assert j_info.annotation == float
 
 
+def test_dictionary_through_Select_reference():
+    """Make sure the Select statement carries the typing all the way through,
+    including a later reference"""
+
+    s = ast_lambda(
+        "e.Jets().Select(lambda j: {'pt': j.pt(), 'eta': j.eta()}).Select(lambda info: info.pt)"
+    )
+    objs = ObjectStream[Event](ast.Name(id="e", ctx=ast.Load()))
+
+    _, _, expr_type = remap_by_types(objs, "e", Event, s)
+
+    assert expr_type == Iterable[float]
+
+
 def test_indexed_tuple():
     "Check that we can type-follow through tuples"
 
     s = ast_lambda("(e.Jets(),)[0].Select(lambda j: j.pt())")
     objs = ObjectStream[Event](ast.Name(id="e", ctx=ast.Load()))
 
     new_objs, new_s, expr_type = remap_by_types(objs, "e", Event, s)
```

### Comparing `func_adl-3.3.1b3/tests/test_type_based_replacement_py310.py` & `func_adl-3.3.1b4/tests/test_type_based_replacement_py310.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b3/tests/test_util_ast.py` & `func_adl-3.3.1b4/tests/test_util_ast.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b3/tests/test_util_types.py` & `func_adl-3.3.1b4/tests/test_util_types.py`

 * *Files identical despite different names*

