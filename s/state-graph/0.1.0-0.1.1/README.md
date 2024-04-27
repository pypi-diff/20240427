# Comparing `tmp/state_graph-0.1.0.tar.gz` & `tmp/state_graph-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "state_graph-0.1.0.tar", last modified: Tue Apr 23 12:00:23 2024, max compression
+gzip compressed data, was "state_graph-0.1.1.tar", last modified: Sat Apr 27 11:24:29 2024, max compression
```

## Comparing `state_graph-0.1.0.tar` & `state_graph-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-23 12:00:23.854839 state_graph-0.1.0/
--rw-r--r--   0 salamanderxing   (501) staff       (20)      173 2024-04-23 12:00:23.854635 state_graph-0.1.0/PKG-INFO
--rw-r--r--   0 salamanderxing   (501) staff       (20)       38 2024-04-23 12:00:23.854881 state_graph-0.1.0/setup.cfg
--rw-r--r--   0 salamanderxing   (501) staff       (20)      264 2024-04-17 10:48:06.000000 state_graph-0.1.0/setup.py
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-23 12:00:23.853599 state_graph-0.1.0/state_graph/
--rw-r--r--   0 salamanderxing   (501) staff       (20)    19361 2024-04-19 09:46:02.000000 state_graph-0.1.0/state_graph/__init__.py
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-23 12:00:23.854408 state_graph-0.1.0/state_graph.egg-info/
--rw-r--r--   0 salamanderxing   (501) staff       (20)      173 2024-04-23 12:00:23.000000 state_graph-0.1.0/state_graph.egg-info/PKG-INFO
--rw-r--r--   0 salamanderxing   (501) staff       (20)      206 2024-04-23 12:00:23.000000 state_graph-0.1.0/state_graph.egg-info/SOURCES.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)        1 2024-04-23 12:00:23.000000 state_graph-0.1.0/state_graph.egg-info/dependency_links.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)       43 2024-04-23 12:00:23.000000 state_graph-0.1.0/state_graph.egg-info/requires.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)       12 2024-04-23 12:00:23.000000 state_graph-0.1.0/state_graph.egg-info/top_level.txt
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-27 11:24:29.355243 state_graph-0.1.1/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      196 2024-04-27 11:24:29.355071 state_graph-0.1.1/PKG-INFO
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       38 2024-04-27 11:24:29.355279 state_graph-0.1.1/setup.cfg
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      276 2024-04-27 11:24:10.000000 state_graph-0.1.1/setup.py
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-27 11:24:29.353998 state_graph-0.1.1/state_graph/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)    19491 2024-04-27 11:23:37.000000 state_graph-0.1.1/state_graph/__init__.py
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-27 11:24:29.354900 state_graph-0.1.1/state_graph.egg-info/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      196 2024-04-27 11:24:29.000000 state_graph-0.1.1/state_graph.egg-info/PKG-INFO
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      206 2024-04-27 11:24:29.000000 state_graph-0.1.1/state_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)        1 2024-04-27 11:24:29.000000 state_graph-0.1.1/state_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       51 2024-04-27 11:24:29.000000 state_graph-0.1.1/state_graph.egg-info/requires.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       12 2024-04-27 11:24:29.000000 state_graph-0.1.1/state_graph.egg-info/top_level.txt
```

### Comparing `state_graph-0.1.0/state_graph/__init__.py` & `state_graph-0.1.1/state_graph/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from re import I
 from regex import P
 from rich import print
 import os
 from typing import TypedDict, Any, get_type_hints, Annotated, get_origin
 import operator
-from abc import ABC, abstractmethod
-import numpy as np
-import ipdb
-import operator
 from pydantic import BaseModel
 from typing import (
     Awaitable,
     Callable,
     Literal,
     get_args,
     TypeVar,
     Any,
     Annotated,
 )
 import asyncio
 import networkx as nx
+from IPython.display import display, HTML
+
 
 # beartype_this_package()
 
 T = TypeVar("T", bound=BaseModel)
 
 
 def is_mutable(model_class):
@@ -394,15 +392,15 @@
             if self.current_node.name in self.__on_state_exit_callbacks:
                 callback = self.__on_state_exit_callbacks[self.current_node.name]
                 if callback is not None:
                     await callback(self.context)
 
             self.current_node = self.get_next_node(self.current_node.name, self.context)
             print(
-                f"[red bold underline] {self.current_node.name} [/red bold underline]"
+                f"\n[red bold underline] {self.current_node.name} [/red bold underline]"
             )
             if self.current_node.name in self.__on_state_enter_callbacks:
                 callback = self.__on_state_enter_callbacks[self.current_node.name]
                 if callback is not None:
                     await callback(self.context)
 
             if isinstance(self.current_node, EndNode):
@@ -430,15 +428,15 @@
             assert (
                 next_node_name in edge.out_nodes
             ), f"Edge {edge.name} does not have a valid out node"
             return self.nodes[next_node_name]
 
         raise RuntimeError("No next node found")
 
-    def plot(self, destination: str = "."):
+    def plot(self, destination: str | None = None):
         assert self.__is_compiled, "Graph must be compiled before plotting"
         # Start of the Mermaid.js diagram
         mermaid_diagram = f"""
 ---        
 title: {self.name}
 ---
 stateDiagram-v2
@@ -483,16 +481,21 @@
         <body style="background-color: #222; padding: 0; margin:0;">
             <div class="mermaid">
                 {mermaid_diagram}
             </div>
         </body>
         </html>"""
 
-        with open(os.path.join(destination, "graph.html"), "w") as f:
-            f.write(out_html)
+        # if destination is None:
+        #     destination = "."
+        if destination is not None:
+            with open(os.path.join(destination, "graph.html"), "w") as f:
+                f.write(out_html)
+        else:
+            display(HTML(out_html))
 
 
 async def main():
 
     async def stream_token(token: str):
         print(token)
```

