# Comparing `tmp/django_hierarchical_models-1.1.0.tar.gz` & `tmp/django_hierarchical_models-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_hierarchical_models-1.1.0.tar", max compression
+gzip compressed data, was "django_hierarchical_models-1.2.0.tar", max compression
```

## Comparing `django_hierarchical_models-1.1.0.tar` & `django_hierarchical_models-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1069 2024-04-25 14:11:21.750670 django_hierarchical_models-1.1.0/LICENSE
--rw-r--r--   0        0        0     3627 2024-04-25 14:11:21.750670 django_hierarchical_models-1.1.0/README.md
--rw-r--r--   0        0        0       22 2024-04-25 14:11:21.750670 django_hierarchical_models-1.1.0/django_hierarchical_models/__init__.py
--rw-r--r--   0        0        0      499 2024-04-25 14:11:21.754670 django_hierarchical_models-1.1.0/django_hierarchical_models/models/__init__.py
--rw-r--r--   0        0        0     1871 2024-04-25 14:11:21.754670 django_hierarchical_models-1.1.0/django_hierarchical_models/models/alm.py
--rw-r--r--   0        0        0      754 2024-04-25 14:11:21.754670 django_hierarchical_models-1.1.0/django_hierarchical_models/models/exceptions.py
--rw-r--r--   0        0        0    14214 2024-04-25 14:11:21.754670 django_hierarchical_models-1.1.0/django_hierarchical_models/models/interface.py
--rw-r--r--   0        0        0     1104 2024-04-25 14:11:21.754670 django_hierarchical_models-1.1.0/django_hierarchical_models/models/node.py
--rw-r--r--   0        0        0    12674 2024-04-25 14:11:21.754670 django_hierarchical_models-1.1.0/django_hierarchical_models/models/nsm.py
--rw-r--r--   0        0        0     2808 2024-04-25 14:11:21.754670 django_hierarchical_models-1.1.0/django_hierarchical_models/models/pem.py
--rw-r--r--   0        0        0     1141 2024-04-25 14:11:21.754670 django_hierarchical_models-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4419 1970-01-01 00:00:00.000000 django_hierarchical_models-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-26 23:00:57.580664 django_hierarchical_models-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3627 2024-04-26 23:00:57.580664 django_hierarchical_models-1.2.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-26 23:00:57.580664 django_hierarchical_models-1.2.0/django_hierarchical_models/__init__.py
+-rw-r--r--   0        0        0      499 2024-04-26 23:00:57.580664 django_hierarchical_models-1.2.0/django_hierarchical_models/models/__init__.py
+-rw-r--r--   0        0        0     2028 2024-04-26 23:00:57.580664 django_hierarchical_models-1.2.0/django_hierarchical_models/models/alm.py
+-rw-r--r--   0        0        0      754 2024-04-26 23:00:57.580664 django_hierarchical_models-1.2.0/django_hierarchical_models/models/exceptions.py
+-rw-r--r--   0        0        0    14702 2024-04-26 23:00:57.580664 django_hierarchical_models-1.2.0/django_hierarchical_models/models/interface.py
+-rw-r--r--   0        0        0     1104 2024-04-26 23:00:57.580664 django_hierarchical_models-1.2.0/django_hierarchical_models/models/node.py
+-rw-r--r--   0        0        0    12977 2024-04-26 23:00:57.580664 django_hierarchical_models-1.2.0/django_hierarchical_models/models/nsm.py
+-rw-r--r--   0        0        0     2958 2024-04-26 23:00:57.580664 django_hierarchical_models-1.2.0/django_hierarchical_models/models/pem.py
+-rw-r--r--   0        0        0     1141 2024-04-26 23:00:57.580664 django_hierarchical_models-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4419 1970-01-01 00:00:00.000000 django_hierarchical_models-1.2.0/PKG-INFO
```

### Comparing `django_hierarchical_models-1.1.0/LICENSE` & `django_hierarchical_models-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_hierarchical_models-1.1.0/README.md` & `django_hierarchical_models-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -46,10 +46,10 @@
 These benchmarks are to illustrate the relative performance of the different models. As
 of now they are kind of whacked out. These tests were run with Postgres.
 
 | Model            | Query Ancestors | Query Parent | Query Children | Query Direct Children | Create | Create Child | Delete | Delete Parent | Add Child | Remove Child | Set Parent | Set Parent Unchecked* |
 |------------------|-----------------|--------------|----------------|-----------------------|--------|--------------|--------|---------------|-----------|--------------|------------|-----------------------|
 | Adjacency List   | 9.56            | 2.76         | 5.17           | 0.96                  | 0.98   | 0.33         | 0.72   | 0.95          | 0.69      | 1.64         | 133.60     | 0.93                  |
 | Path Enumeration | 9.17            | 2.67         | 29.71          | 0.84                  | 0.99   | 0.32         | 0.75   | 1.26          | 0.94      | 1.79         | 2.98       |                       |
-| Nested Set       | 719.37          | 964.90       | 1033.37        | 1011.12               | 240.15 | 91.82        | 179.92 | 270.84        | 95.08     | 411.03       | 863.99     |                       |
+| Nested Set       | 169.86          | 118.97       | 211.75         | 107.30                | 3.31   | 59.19        | 113.79 | 175.11        | 71.13     | 293.61       | 572.47     |                       |
 
 \* function only available on Adjacency List Model
```

### Comparing `django_hierarchical_models-1.1.0/django_hierarchical_models/models/alm.py` & `django_hierarchical_models-1.2.0/django_hierarchical_models/models/alm.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     # ------------------------ override HierarchicalModel ------------------- #
 
     def parent(self: T) -> T | None:
         self.refresh_from_db(fields=("_parent",))
         return self._parent  # type: ignore
 
     def is_child_of(self: T, parent: T) -> bool:
-        self.refresh_from_db(fields=("_parent",))
         self_parent = self._parent
         while self_parent is not None:
             if self_parent == parent:
                 return True
             self_parent = self_parent._parent
         return False
 
@@ -54,7 +53,14 @@
 
     def set_parent_unchecked(self: T, parent: T | None):
         """Sets the parent of this instance without checking for cycles."""
         self._set_parent(parent)
 
     def direct_children(self: T) -> QuerySet[T]:
         return self._manager.filter(_parent=self)
+
+    def root(self: T) -> T:
+        root = self
+        self.refresh_from_db(fields=("_parent",))
+        while root._parent is not None:
+            root = root._parent  # type: ignore
+        return root
```

### Comparing `django_hierarchical_models-1.1.0/django_hierarchical_models/models/exceptions.py` & `django_hierarchical_models-1.2.0/django_hierarchical_models/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_hierarchical_models-1.1.0/django_hierarchical_models/models/interface.py` & `django_hierarchical_models-1.2.0/django_hierarchical_models/models/interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import copy
 from collections import deque
 from collections.abc import Callable
 from typing import TypeVar
 
 from django.db import models
 from django.db.models import QuerySet
 from django.db.models.manager import BaseManager
@@ -254,15 +253,16 @@
 def _no_no_no(
     root: Node[T],
     _: int,
     __: int,
     ___: int,
     sibling_transform: Callable[[QuerySet[T]], QuerySet[T]] | None,
 ):
-    queue = deque([(copy.copy(root), root)])
+    queue: deque[tuple[Node[T], Node[T]]] = deque()
+    queue.append((Node(None), root))  # type: ignore
     while queue:
         parent_node, node = queue.popleft()
         parent_node.children.append(node)
         children = node.instance.direct_children()
         if sibling_transform is not None:
             children = sibling_transform(children)
         for child in children:
@@ -273,15 +273,16 @@
 def _yes_no_no(
     root: Node[T],
     max_generations: int,
     _: int,
     __: int,
     sibling_transform: Callable[[QuerySet[T]], QuerySet[T]] | None,
 ):
-    queue = deque([(copy.copy(root), root, 0)])
+    queue: deque[tuple[Node[T], Node[T], int]] = deque()
+    queue.append((Node(None), root, 0))  # type: ignore
     while queue:
         parent_node, node, generation = queue.popleft()
         parent_node.children.append(node)
         if generation < max_generations:
             children = node.instance.direct_children()
             if sibling_transform is not None:
                 children = sibling_transform(children)
@@ -293,15 +294,16 @@
 def _no_yes_no(
     root: Node[T],
     _: int,
     max_siblings: int,
     __: int,
     sibling_transform: Callable[[QuerySet[T]], QuerySet[T]] | None,
 ):
-    queue = deque([(copy.copy(root), root)])
+    queue: deque[tuple[Node[T], Node[T]]] = deque()
+    queue.append((Node(None), root))  # type: ignore
     while queue:
         parent_node, node = queue.popleft()
         parent_node.children.append(node)
         children = node.instance.direct_children()
         if sibling_transform is not None:
             children = sibling_transform(children)
         for child in children[:max_siblings]:
@@ -312,15 +314,16 @@
 def _no_no_yes(
     root: Node[T],
     _: int,
     __: int,
     max_total: int,
     sibling_transform: Callable[[QuerySet[T]], QuerySet[T]] | None,
 ):
-    queue = deque([(copy.copy(root), root)])
+    queue: deque[tuple[Node[T], Node[T]]] = deque()
+    queue.append((Node(None), root))  # type: ignore
     max_total -= 1
     while queue:
         parent_node, node = queue.popleft()
         parent_node.children.append(node)
         children = node.instance.direct_children()
         if sibling_transform is not None:
             children = sibling_transform(children)
@@ -333,15 +336,16 @@
 def _yes_yes_no(
     root: Node[T],
     max_generations: int,
     max_siblings: int,
     _: int,
     sibling_transform: Callable[[QuerySet[T]], QuerySet[T]] | None,
 ):
-    queue = deque([(copy.copy(root), root, 0)])
+    queue: deque[tuple[Node[T], Node[T], int]] = deque()
+    queue.append((Node(None), root, 0))  # type: ignore
     while queue:
         parent_node, node, generation = queue.popleft()
         parent_node.children.append(node)
         if generation < max_generations:
             children = node.instance.direct_children()
             if sibling_transform is not None:
                 children = sibling_transform(children)
@@ -353,15 +357,16 @@
 def _yes_no_yes(
     root: Node[T],
     max_generations: int,
     _: int,
     max_total: int,
     sibling_transform: Callable[[QuerySet[T]], QuerySet[T]] | None,
 ):
-    queue = deque([(copy.copy(root), root, 0)])
+    queue: deque[tuple[Node[T], Node[T], int]] = deque()
+    queue.append((Node(None), root, 0))  # type: ignore
     max_total -= 1
     while queue:
         parent_node, node, generation = queue.popleft()
         parent_node.children.append(node)
         if generation < max_generations:
             children = node.instance.direct_children()
             if sibling_transform is not None:
@@ -375,15 +380,16 @@
 def _no_yes_yes(
     root: Node[T],
     _: int,
     max_siblings: int,
     max_total: int,
     sibling_transform: Callable[[QuerySet[T]], QuerySet[T]] | None,
 ):
-    queue = deque([(copy.copy(root), root)])
+    queue: deque[tuple[Node[T], Node[T]]] = deque()
+    queue.append((Node(None), root))  # type: ignore
     max_total -= 1
     while queue:
         parent_node, node = queue.popleft()
         parent_node.children.append(node)
         num_siblings = min(max_siblings, max_total)
         children = node.instance.direct_children()
         if sibling_transform is not None:
@@ -397,15 +403,16 @@
 def _yes_yes_yes(
     root: Node[T],
     max_generations: int,
     max_siblings: int,
     max_total: int,
     sibling_transform: Callable[[QuerySet[T]], QuerySet[T]] | None,
 ):
-    queue = deque([(copy.copy(root), root, 0)])
+    queue: deque[tuple[Node[T], Node[T], int]] = deque()
+    queue.append((Node(None), root, 0))  # type: ignore
     max_total -= 1
     while queue:
         parent_node, node, generation = queue.popleft()
         parent_node.children.append(node)
         if generation < max_generations:
             num_siblings = min(max_siblings, max_total)
             children = node.instance.direct_children()
```

### Comparing `django_hierarchical_models-1.1.0/django_hierarchical_models/models/node.py` & `django_hierarchical_models-1.2.0/django_hierarchical_models/models/node.py`

 * *Files identical despite different names*

### Comparing `django_hierarchical_models-1.1.0/django_hierarchical_models/models/nsm.py` & `django_hierarchical_models-1.2.0/django_hierarchical_models/models/nsm.py`

 * *Files 17% similar despite different names*

```diff
@@ -272,14 +272,23 @@
                 )
 
         self._shift_chunk(*between_shift)
         self._shift_chunk(*skin_shift)
         self_chunk = self._manager.filter(pk__in=self_chunk_items)
         self._shift_chunk(self_chunk, *self_shift)
 
+    def ancestors(self: T, max_level: int | None = None) -> list[T]:
+        self.refresh_from_db(fields=("_left", "_right"))
+        ancestors = self._manager.filter(
+            _left__lt=self._left, _right__gt=self._right
+        ).order_by("-_left")
+        if max_level is not None:
+            ancestors = ancestors[:max_level]
+        return list(ancestors)
+
     def direct_children(self: T) -> QuerySet[T]:
         """Gets all the direct descendants of a model.
 
         If there are no children the QuerySet will be emtpy.
 
         This method first queries for models that are within the bounds of this
         instance. After that they are ordered by smallest and the first is
@@ -290,19 +299,20 @@
             An unordered QuerySet of all direct children of this model.
         """
         self.refresh_from_db(fields=("_left", "_right"))
         children_chunk = self._manager.filter(
             _left__gt=self._left, _right__lt=self._right
         ).order_by("_left")
         direct_children = []
-        next_child = children_chunk.first()
-        while next_child is not None:
-            direct_children.append(next_child.pk)
-            children_chunk = children_chunk.filter(_left__gt=next_child._right)
-            next_child = children_chunk.first()
+
+        right_value = -1
+        for child in children_chunk:
+            if child._left > right_value:
+                direct_children.append(child.pk)
+                right_value = child._right
         return self._manager.filter(pk__in=direct_children)
 
     def root(self: T) -> T:
         self.refresh_from_db(fields=("_left", "_right"))
         parents_query = self._manager.filter(
             _left__lt=self._left, _right__gt=self._right
         )
```

### Comparing `django_hierarchical_models-1.1.0/django_hierarchical_models/models/pem.py` & `django_hierarchical_models-1.2.0/django_hierarchical_models/models/pem.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from django_hierarchical_models.models.interface import HierarchicalModelInterface
 
 T = TypeVar("T", bound="PathEnumerationModel")
 
 
 class PathEnumerationModel(HierarchicalModelInterface):
-    pass
 
     # ------------------------ class members -------------------------------- #
 
     _ancestors = models.JSONField(default=list)
 
     # ------------------------ builtin methods ------------------------------ #
 
@@ -63,15 +62,20 @@
     def is_child_of(self: T, parent: T) -> bool:
         self.refresh_from_db(fields=("_ancestors",))
         return parent.pk in self._ancestors
 
     def direct_children(self: T) -> QuerySet[T]:
         return self._manager.filter(_ancestors__0=self.pk)
 
+    def root(self: T) -> T:
+        self.refresh_from_db(fields=("_ancestors",))
+        if len(self._ancestors) == 0:
+            return self
+        return self._manager.get(pk=self._ancestors[-1])
+
     def _set_parent(self: T, parent: T | None):
         if parent is None:
             self._ancestors = []
         else:
             parent.refresh_from_db(fields=("_ancestors",))
-            self._ancestors = parent._ancestors.copy()
-            self._ancestors.insert(0, parent.pk)
+            self._ancestors = [parent.pk] + parent._ancestors
         self.save(update_fields=("_ancestors",))
```

### Comparing `django_hierarchical_models-1.1.0/pyproject.toml` & `django_hierarchical_models-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-hierarchical-models"
-version = "1.1.0"
+version = "1.2.0"
 description = "Adds hierarchical models to Django"
 authors = ["Josh Bedwell <rcxwhiz@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/rcxwhiz/django-hierarchical-models"
 packages = [{include = "django_hierarchical_models"}]
 classifiers = [
```

### Comparing `django_hierarchical_models-1.1.0/PKG-INFO` & `django_hierarchical_models-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-hierarchical-models
-Version: 1.1.0
+Version: 1.2.0
 Summary: Adds hierarchical models to Django
 Home-page: https://github.com/rcxwhiz/django-hierarchical-models
 License: MIT
 Author: Josh Bedwell
 Author-email: rcxwhiz@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Framework :: Django
@@ -67,11 +67,11 @@
 These benchmarks are to illustrate the relative performance of the different models. As
 of now they are kind of whacked out. These tests were run with Postgres.
 
 | Model            | Query Ancestors | Query Parent | Query Children | Query Direct Children | Create | Create Child | Delete | Delete Parent | Add Child | Remove Child | Set Parent | Set Parent Unchecked* |
 |------------------|-----------------|--------------|----------------|-----------------------|--------|--------------|--------|---------------|-----------|--------------|------------|-----------------------|
 | Adjacency List   | 9.56            | 2.76         | 5.17           | 0.96                  | 0.98   | 0.33         | 0.72   | 0.95          | 0.69      | 1.64         | 133.60     | 0.93                  |
 | Path Enumeration | 9.17            | 2.67         | 29.71          | 0.84                  | 0.99   | 0.32         | 0.75   | 1.26          | 0.94      | 1.79         | 2.98       |                       |
-| Nested Set       | 719.37          | 964.90       | 1033.37        | 1011.12               | 240.15 | 91.82        | 179.92 | 270.84        | 95.08     | 411.03       | 863.99     |                       |
+| Nested Set       | 169.86          | 118.97       | 211.75         | 107.30                | 3.31   | 59.19        | 113.79 | 175.11        | 71.13     | 293.61       | 572.47     |                       |
 
 \* function only available on Adjacency List Model
```

