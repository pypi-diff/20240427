# Comparing `tmp/llama_index_graph_stores_falkordb-0.1.3.tar.gz` & `tmp/llama_index_graph_stores_falkordb-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_graph_stores_falkordb-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_graph_stores_falkordb-0.1.4.tar", max compression
```

## Comparing `llama_index_graph_stores_falkordb-0.1.3.tar` & `llama_index_graph_stores_falkordb-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       48 2024-04-03 01:39:40.431653 llama_index_graph_stores_falkordb-0.1.3/README.md
--rw-r--r--   0        0        0      104 2024-04-03 01:39:40.431653 llama_index_graph_stores_falkordb-0.1.3/llama_index/graph_stores/falkordb/__init__.py
--rw-r--r--   0        0        0     5967 2024-04-03 01:39:40.431653 llama_index_graph_stores_falkordb-0.1.3/llama_index/graph_stores/falkordb/base.py
--rw-r--r--   0        0        0     1483 2024-04-03 01:39:40.431653 llama_index_graph_stores_falkordb-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 llama_index_graph_stores_falkordb-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       48 2024-04-27 05:48:31.087497 llama_index_graph_stores_falkordb-0.1.4/README.md
+-rw-r--r--   0        0        0      104 2024-04-27 05:48:31.087497 llama_index_graph_stores_falkordb-0.1.4/llama_index/graph_stores/falkordb/__init__.py
+-rw-r--r--   0        0        0     6165 2024-04-27 05:48:31.087497 llama_index_graph_stores_falkordb-0.1.4/llama_index/graph_stores/falkordb/base.py
+-rw-r--r--   0        0        0     1483 2024-04-27 05:48:31.087497 llama_index_graph_stores_falkordb-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 llama_index_graph_stores_falkordb-0.1.4/PKG-INFO
```

### Comparing `llama_index_graph_stores_falkordb-0.1.3/llama_index/graph_stores/falkordb/base.py` & `llama_index_graph_stores_falkordb-0.1.4/llama_index/graph_stores/falkordb/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Simple graph store index."""
 
 import logging
 from typing import Any, Dict, List, Optional
 
+import redis
 from falkordb import FalkorDB
 from llama_index.core.graph_stores.types import GraphStore
 
 logger = logging.getLogger(__name__)
 
 
 class FalkorDBGraphStore(GraphStore):
@@ -27,15 +28,20 @@
         node_label: str = "Entity",
         **kwargs: Any,
     ) -> None:
         """Initialize params."""
         self._node_label = node_label
 
         self._driver = FalkorDB.from_url(url).select_graph(database)
-        self._driver.query(f"CREATE INDEX FOR (n:`{self._node_label}`) ON (n.id)")
+
+        try:
+            self._driver.query(f"CREATE INDEX FOR (n:`{self._node_label}`) ON (n.id)")
+        except redis.ResponseError as e:
+            # TODO: to find an appropriate way to handle this issue.
+            logger.warning("Create index failed: %s", e)
 
         self._database = database
 
         self.schema = ""
         self.get_query = f"""
             MATCH (n1:`{self._node_label}`)-[r]->(n2:`{self._node_label}`)
             WHERE n1.id = $subj RETURN type(r), n2.id
```

### Comparing `llama_index_graph_stores_falkordb-0.1.3/pyproject.toml` & `llama_index_graph_stores_falkordb-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index graph stores falkordb integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-graph-stores-falkordb"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 falkordb = "^1.0.4"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_graph_stores_falkordb-0.1.3/PKG-INFO` & `llama_index_graph_stores_falkordb-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-graph-stores-falkordb
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index graph stores falkordb integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

