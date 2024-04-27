# Comparing `tmp/func_adl-3.3.1b2.tar.gz` & `tmp/func_adl-3.3.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/func_adl-3.3.1b2.tar", last modified: Thu Apr 25 08:04:49 2024, max compression
+gzip compressed data, was "dist/func_adl-3.3.1b3.tar", last modified: Sat Apr 27 06:44:37 2024, max compression
```

## Comparing `func_adl-3.3.1b2.tar` & `func_adl-3.3.1b3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:04:49.000000 func_adl-3.3.1b2/
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-25 08:04:49.000000 func_adl-3.3.1b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:04:49.000000 func_adl-3.3.1b2/func_adl/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/func_adl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:04:49.000000 func_adl-3.3.1b2/func_adl/ast/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/func_adl/ast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/func_adl/ast/aggregate_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/func_adl/ast/ast_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/func_adl/ast/call_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/func_adl/ast/func_adl_ast_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20311 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/func_adl/ast/function_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/func_adl/ast/meta_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/func_adl/ast/syntatic_sugar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/func_adl/event_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/func_adl/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15904 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/func_adl/object_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    37396 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/func_adl/type_based_replacement.py
--rw-r--r--   0 runner    (1001) docker     (127)    24565 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/func_adl/util_ast.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/func_adl/util_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:04:49.000000 func_adl-3.3.1b2/func_adl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-25 08:04:49.000000 func_adl-3.3.1b2/func_adl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-25 08:04:49.000000 func_adl-3.3.1b2/func_adl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:04:49.000000 func_adl-3.3.1b2/func_adl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-25 08:04:49.000000 func_adl-3.3.1b2/func_adl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 08:04:49.000000 func_adl-3.3.1b2/func_adl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 08:04:49.000000 func_adl-3.3.1b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:04:49.000000 func_adl-3.3.1b2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/tests/test_event_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/tests/test_object_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    31853 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/tests/test_type_based_replacement.py
--rw-r--r--   0 runner    (1001) docker     (127)    16732 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/tests/test_type_based_replacement_py310.py
--rw-r--r--   0 runner    (1001) docker     (127)    22510 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/tests/test_util_ast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-25 08:04:40.000000 func_adl-3.3.1b2/tests/test_util_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/func_adl/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/func_adl/ast/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/ast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/ast/aggregate_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/ast/ast_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/ast/call_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/ast/func_adl_ast_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20311 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/ast/function_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/ast/meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/ast/syntatic_sugar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/event_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15904 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/object_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37909 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/type_based_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24565 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/util_ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/func_adl/util_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/func_adl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/func_adl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/func_adl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/func_adl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/func_adl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/func_adl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:44:37.000000 func_adl-3.3.1b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/tests/test_event_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/tests/test_object_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33178 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/tests/test_type_based_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16732 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/tests/test_type_based_replacement_py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22510 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/tests/test_util_ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-27 06:44:33.000000 func_adl-3.3.1b3/tests/test_util_types.py
```

### Comparing `func_adl-3.3.1b2/PKG-INFO` & `func_adl-3.3.1b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func_adl
-Version: 3.3.1b2
+Version: 3.3.1b3
 Summary: Functional Analysis Description Language Base Package
 Home-page: https://github.com/iris-hep/func_adl
 Author: G. Watts (IRIS-HEP/UW Seattle)
 Author-email: gwatts@uw.edu
 Maintainer: Gordon Watts (IRIS-HEP/UW Seattle)
 Maintainer-email: gwatts@uw.edu
 License: MIT
```

### Comparing `func_adl-3.3.1b2/README.md` & `func_adl-3.3.1b3/README.md`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b2/func_adl/ast/aggregate_shortcuts.py` & `func_adl-3.3.1b3/func_adl/ast/aggregate_shortcuts.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b2/func_adl/ast/call_stack.py` & `func_adl-3.3.1b3/func_adl/ast/call_stack.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b2/func_adl/ast/func_adl_ast_utils.py` & `func_adl-3.3.1b3/func_adl/ast/func_adl_ast_utils.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b2/func_adl/ast/function_simplifier.py` & `func_adl-3.3.1b3/func_adl/ast/function_simplifier.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b2/func_adl/ast/meta_data.py` & `func_adl-3.3.1b3/func_adl/ast/meta_data.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b2/func_adl/ast/syntatic_sugar.py` & `func_adl-3.3.1b3/func_adl/ast/syntatic_sugar.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b2/func_adl/event_dataset.py` & `func_adl-3.3.1b3/func_adl/event_dataset.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b2/func_adl/functions.py` & `func_adl-3.3.1b3/func_adl/functions.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b2/func_adl/object_stream.py` & `func_adl-3.3.1b3/func_adl/object_stream.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b2/func_adl/type_based_replacement.py` & `func_adl-3.3.1b3/func_adl/type_based_replacement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import ast
 import copy
 import inspect
 import logging
 import sys
-from dataclasses import dataclass
+from dataclasses import dataclass, make_dataclass
 from typing import (
     Any,
     Callable,
     Dict,
     Generic,
     Iterable,
     List,
@@ -919,14 +919,27 @@
             elif node.id in _global_functions:
                 self._found_types[node] = Callable
             else:
                 logging.getLogger(__name__).warning(f"Unknown type for name {node.id}")
                 self._found_types[node] = Any
             return node
 
+        def visit_Dict(self, node: ast.Dict) -> Any:
+            t_node = self.generic_visit(node)
+            assert isinstance(t_node, ast.Dict)
+
+            fields: List[Tuple[str, type]] = [
+                (ast.literal_eval(f), self.lookup_type(v))  # type: ignore
+                for f, v in zip(t_node.keys, t_node.values)
+            ]
+            dict_dataclass = make_dataclass("dict_dataclass", fields)
+
+            self._found_types[t_node] = dict_dataclass
+            return t_node
+
         def visit_Constant(self, node: ast.Constant) -> Any:
             self._found_types[node] = type(node.value)
             return node
 
         def visit_Num(self, node: ast.Num) -> Any:  # pragma: no cover
             "3.7 compatability"
             self._found_types[node] = type(node.n)
```

### Comparing `func_adl-3.3.1b2/func_adl/util_ast.py` & `func_adl-3.3.1b3/func_adl/util_ast.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b2/func_adl/util_types.py` & `func_adl-3.3.1b3/func_adl/util_types.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b2/func_adl.egg-info/PKG-INFO` & `func_adl-3.3.1b3/func_adl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func-adl
-Version: 3.3.1b2
+Version: 3.3.1b3
 Summary: Functional Analysis Description Language Base Package
 Home-page: https://github.com/iris-hep/func_adl
 Author: G. Watts (IRIS-HEP/UW Seattle)
 Author-email: gwatts@uw.edu
 Maintainer: Gordon Watts (IRIS-HEP/UW Seattle)
 Maintainer-email: gwatts@uw.edu
 License: MIT
```

### Comparing `func_adl-3.3.1b2/func_adl.egg-info/SOURCES.txt` & `func_adl-3.3.1b3/func_adl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b2/setup.py` & `func_adl-3.3.1b3/setup.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b2/tests/test_event_dataset.py` & `func_adl-3.3.1b3/tests/test_event_dataset.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b2/tests/test_object_stream.py` & `func_adl-3.3.1b3/tests/test_object_stream.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b2/tests/test_type_based_replacement.py` & `func_adl-3.3.1b3/tests/test_type_based_replacement.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import ast
 import copy
+import inspect
 import logging
+from inspect import isclass
 from typing import Any, Callable, Iterable, Optional, Tuple, Type, TypeVar, cast
 
 import pytest
 
 from func_adl import ObjectStream
 from func_adl.type_based_replacement import (
     func_adl_callable,
     func_adl_callback,
     func_adl_parameterized_call,
     register_func_adl_os_collection,
     remap_by_types,
     remap_from_lambda,
 )
+from func_adl.util_types import is_iterable, unwrap_iterable
 
 
 class Track:
     def pt(self) -> float: ...  # noqa
 
     def eta(self) -> float: ...  # noqa
 
@@ -500,14 +503,31 @@
 
     assert expr_type == Iterable[float]
 
     assert len(caplog.text) == 0
 
 
 def test_dictionary():
+    "Make sure that dictionaries turn into named types"
+
+    s = ast_lambda("{'jets': e.Jets()}")
+    objs = ObjectStream[Event](ast.Name(id="e", ctx=ast.Load()))
+
+    new_objs, new_s, expr_type = remap_by_types(objs, "e", Event, s)
+
+    # Fix to look for the named class with the correct types.
+    assert isclass(expr_type)
+    sig = inspect.signature(expr_type.__init__)
+    assert len(sig.parameters) == 2
+    assert "jets" in sig.parameters
+    j_info = sig.parameters["jets"]
+    assert str(j_info.annotation) == "typing.Iterable[tests.test_type_based_replacement.Jet]"
+
+
+def test_dictionary_sequence():
     "Check that we can type-follow through dictionaries"
 
     s = ast_lambda("{'jets': e.Jets()}.jets.Select(lambda j: j.pt())")
     objs = ObjectStream[Event](ast.Name(id="e", ctx=ast.Load()))
 
     new_objs, new_s, expr_type = remap_by_types(objs, "e", Event, s)
 
@@ -522,16 +542,34 @@
         objs = ObjectStream[Event](ast.Name(id="e", ctx=ast.Load()))
 
         new_objs, new_s, expr_type = remap_by_types(objs, "e", Event, s)
 
     assert "jetsss" in str(e)
 
 
+def test_dictionary_through_Select():
+    """Make sure the Select statement carries the typing all the way through"""
+
+    s = ast_lambda("e.Jets().Select(lambda j: {'pt': j.pt(), 'eta': j.eta()})")
+    objs = ObjectStream[Event](ast.Name(id="e", ctx=ast.Load()))
+
+    _, _, expr_type = remap_by_types(objs, "e", Event, s)
+
+    assert is_iterable(expr_type)
+    obj_itr = unwrap_iterable(expr_type)
+    assert isclass(obj_itr)
+    sig = inspect.signature(obj_itr.__init__)
+    assert len(sig.parameters) == 3
+    assert "pt" in sig.parameters
+    j_info = sig.parameters["pt"]
+    assert j_info.annotation == float
+
+
 def test_indexed_tuple():
-    "Check that we can type-follow through dictionaries"
+    "Check that we can type-follow through tuples"
 
     s = ast_lambda("(e.Jets(),)[0].Select(lambda j: j.pt())")
     objs = ObjectStream[Event](ast.Name(id="e", ctx=ast.Load()))
 
     new_objs, new_s, expr_type = remap_by_types(objs, "e", Event, s)
 
     assert expr_type == Iterable[float]
```

### Comparing `func_adl-3.3.1b2/tests/test_type_based_replacement_py310.py` & `func_adl-3.3.1b3/tests/test_type_based_replacement_py310.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b2/tests/test_util_ast.py` & `func_adl-3.3.1b3/tests/test_util_ast.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.1b2/tests/test_util_types.py` & `func_adl-3.3.1b3/tests/test_util_types.py`

 * *Files identical despite different names*

