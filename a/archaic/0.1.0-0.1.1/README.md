# Comparing `tmp/archaic-0.1.0.tar.gz` & `tmp/archaic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archaic-0.1.0.tar", last modified: Thu Apr 25 02:27:33 2024, max compression
+gzip compressed data, was "archaic-0.1.1.tar", last modified: Fri Apr 26 12:38:11 2024, max compression
```

## Comparing `archaic-0.1.0.tar` & `archaic-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 02:27:33.511755 archaic-0.1.0/
--rw-rw-rw-   0        0        0      504 2024-04-25 02:27:33.510313 archaic-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        9 2024-04-20 18:47:21.000000 archaic-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 02:27:33.489883 archaic-0.1.0/archaic/
--rw-rw-rw-   0        0        0       63 2024-04-22 00:10:34.000000 archaic-0.1.0/archaic/__init__.py
--rw-rw-rw-   0        0        0     8123 2024-04-25 01:48:18.000000 archaic-0.1.0/archaic/feature_class.py
--rw-rw-rw-   0        0        0     3465 2024-04-24 11:53:55.000000 archaic-0.1.0/archaic/info.py
--rw-rw-rw-   0        0        0     6052 2024-04-23 15:09:08.000000 archaic-0.1.0/archaic/predicate.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:27:33.508737 archaic-0.1.0/archaic.egg-info/
--rw-rw-rw-   0        0        0      504 2024-04-25 02:27:33.000000 archaic-0.1.0/archaic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2024-04-25 02:27:33.000000 archaic-0.1.0/archaic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 02:27:33.000000 archaic-0.1.0/archaic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-25 02:27:33.000000 archaic-0.1.0/archaic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      619 2024-04-20 18:47:21.000000 archaic-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-25 02:27:33.511755 archaic-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 12:38:11.740250 archaic-0.1.1/
+-rw-rw-rw-   0        0        0      504 2024-04-26 12:38:11.738210 archaic-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2024-04-20 18:47:21.000000 archaic-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 12:38:11.715407 archaic-0.1.1/archaic/
+-rw-rw-rw-   0        0        0       63 2024-04-22 00:10:34.000000 archaic-0.1.1/archaic/__init__.py
+-rw-rw-rw-   0        0        0     8172 2024-04-26 12:22:54.000000 archaic-0.1.1/archaic/feature_class.py
+-rw-rw-rw-   0        0        0     3348 2024-04-26 12:20:33.000000 archaic-0.1.1/archaic/info.py
+-rw-rw-rw-   0        0        0     6052 2024-04-23 15:09:08.000000 archaic-0.1.1/archaic/predicate.py
+drwxrwxrwx   0        0        0        0 2024-04-26 12:38:11.736701 archaic-0.1.1/archaic.egg-info/
+-rw-rw-rw-   0        0        0      504 2024-04-26 12:38:11.000000 archaic-0.1.1/archaic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2024-04-26 12:38:11.000000 archaic-0.1.1/archaic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 12:38:11.000000 archaic-0.1.1/archaic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-26 12:38:11.000000 archaic-0.1.1/archaic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      619 2024-04-26 00:05:51.000000 archaic-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-26 12:38:11.740250 archaic-0.1.1/setup.cfg
```

### Comparing `archaic-0.1.0/archaic/feature_class.py` & `archaic-0.1.1/archaic/feature_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,23 +140,28 @@
         ids: Set[int] = set()
         for where_clause in self._get_where_clauses_from_ids(items):
             for id in self.delete_where(where_clause):
                 ids.add(id)
         return list(ids)
 
     def _create(self, **kwargs: Any) -> T:
-        if self.info.has_default_constructor:
-            item = self.info.model()
-            for property in self.info.properties:
-                setattr(item, property, kwargs.get(property))
-            return item
-        return self.info.model(
-            **{k: v for k, v in kwargs.items() if k in self.info.properties}
+        item = self.info.model(
+            **{
+                k: v
+                for k, v in kwargs.items()
+                if k in self.info.properties and k in self.info.keys
+            }
         )
 
+        for property in self.info.properties:
+            if property not in self.info.keys:
+                setattr(item, property, kwargs.get(property))
+
+        return item
+
     def _get_values(self, item: T, properties: Iterable[str]) -> List[Any]:
         values: List[Any] = []
         for property in properties:
             values.append(getattr(item, property) if hasattr(item, property) else None)
         return values
 
     def _get_where_clauses_from_ids(
```

### Comparing `archaic-0.1.0/archaic/info.py` & `archaic-0.1.1/archaic/info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import arcpy
 import re
 
 from inspect import signature
-from itertools import chain
 from types import SimpleNamespace
 from typing import TYPE_CHECKING, Dict, Generic, Set, Type, TypeVar
 
 if TYPE_CHECKING:
     from archaic.feature_class import FeatureClass
 
 T = TypeVar("T")
@@ -15,24 +14,21 @@
 class Info(Generic[T]):
     def __init__(self, feature_class: "FeatureClass[T]") -> None:
         if hasattr(feature_class, "__orig_class__"):
             model = feature_class.__orig_class__.__args__[0]  # type: ignore
         else:
             model = SimpleNamespace
 
-        keys = chain(
-            signature(model.__init__).parameters.keys(),
-            signature(model.__new__).parameters.keys(),
-        )
-
         description = arcpy.Describe(feature_class._data_path)
 
         # Members.
         self.model: Type[T] = model  # type: ignore
-        self.has_default_constructor = len(set(keys)) == 3
+        self.keys = [
+            key for key in signature(model.__init__).parameters.keys() if key != "self"
+        ]
         self.data_path: str = description.catalogPath  # type: ignore
         self.oid_field: str
         self.oid_property: str
         self.properties: Dict[str, str] = {}
         self.edit_properties: Dict[str, str] = {}
 
         # Inspect the fields.
```

### Comparing `archaic-0.1.0/archaic/predicate.py` & `archaic-0.1.1/archaic/predicate.py`

 * *Files identical despite different names*

### Comparing `archaic-0.1.0/pyproject.toml` & `archaic-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "archaic"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "Simplifies handling of ArcPy rows"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

