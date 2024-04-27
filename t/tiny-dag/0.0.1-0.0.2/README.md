# Comparing `tmp/tiny-dag-0.0.1.tar.gz` & `tmp/tiny_dag-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ossi/Repos/Personal/PySimpleGraph/dist/tmpcx2r1wrt/tiny-dag-0.0.1.tar", last modified: Sun Nov 14 11:26:18 2021, max compression
+gzip compressed data, was "tiny_dag-0.0.2.tar", last modified: Sat Apr 27 09:31:34 2024, max compression
```

## Comparing `tiny-dag-0.0.1.tar` & `tiny_dag-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2021-11-14 11:26:18.000000 tiny-dag-0.0.1/
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2021-11-14 11:26:18.000000 tiny-dag-0.0.1/src/
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2021-11-14 11:26:18.000000 tiny-dag-0.0.1/src/tinydag/
--rw-rw-r--   0 ossi      (1000) ossi      (1000)     5966 2021-11-14 11:13:44.000000 tiny-dag-0.0.1/src/tinydag/graph.py
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      711 2021-10-02 09:55:25.000000 tiny-dag-0.0.1/src/tinydag/node.py
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        0 2021-11-14 11:13:24.000000 tiny-dag-0.0.1/src/tinydag/__init__.py
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2021-11-14 11:26:18.000000 tiny-dag-0.0.1/src/tiny_dag.egg-info/
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        1 2021-11-14 11:26:18.000000 tiny-dag-0.0.1/src/tiny_dag.egg-info/dependency_links.txt
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        8 2021-11-14 11:26:18.000000 tiny-dag-0.0.1/src/tiny_dag.egg-info/top_level.txt
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      286 2021-11-14 11:26:18.000000 tiny-dag-0.0.1/src/tiny_dag.egg-info/SOURCES.txt
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        9 2021-11-14 11:26:18.000000 tiny-dag-0.0.1/src/tiny_dag.egg-info/requires.txt
--rw-rw-r--   0 ossi      (1000) ossi      (1000)     1221 2021-11-14 11:26:18.000000 tiny-dag-0.0.1/src/tiny_dag.egg-info/PKG-INFO
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      104 2021-11-11 15:02:10.000000 tiny-dag-0.0.1/pyproject.toml
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      668 2021-11-14 11:26:18.000000 tiny-dag-0.0.1/setup.cfg
--rw-rw-r--   0 ossi      (1000) ossi      (1000)     1072 2021-09-28 18:25:01.000000 tiny-dag-0.0.1/LICENSE
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      671 2021-11-14 11:22:24.000000 tiny-dag-0.0.1/README.md
--rw-rw-r--   0 ossi      (1000) ossi      (1000)     1221 2021-11-14 11:26:18.000000 tiny-dag-0.0.1/PKG-INFO
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-27 09:31:34.056354 tiny_dag-0.0.2/
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)     1072 2024-04-27 07:53:55.000000 tiny_dag-0.0.2/LICENSE
+-rw-r--r--   0 ossi      (1000) ossi      (1000)     1410 2024-04-27 09:31:34.056354 tiny_dag-0.0.2/PKG-INFO
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      872 2024-04-27 07:53:55.000000 tiny_dag-0.0.2/README.md
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      104 2024-04-27 09:26:48.000000 tiny_dag-0.0.2/pyproject.toml
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      668 2024-04-27 09:31:34.060354 tiny_dag-0.0.2/setup.cfg
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-27 09:31:34.056354 tiny_dag-0.0.2/src/
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-27 09:31:34.056354 tiny_dag-0.0.2/src/tiny_dag.egg-info/
+-rw-r--r--   0 ossi      (1000) ossi      (1000)     1410 2024-04-27 09:31:34.000000 tiny_dag-0.0.2/src/tiny_dag.egg-info/PKG-INFO
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      286 2024-04-27 09:31:34.000000 tiny_dag-0.0.2/src/tiny_dag.egg-info/SOURCES.txt
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        1 2024-04-27 09:31:34.000000 tiny_dag-0.0.2/src/tiny_dag.egg-info/dependency_links.txt
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        9 2024-04-27 09:31:34.000000 tiny_dag-0.0.2/src/tiny_dag.egg-info/requires.txt
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        8 2024-04-27 09:31:34.000000 tiny_dag-0.0.2/src/tiny_dag.egg-info/top_level.txt
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-27 09:31:34.056354 tiny_dag-0.0.2/src/tinydag/
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        0 2024-04-27 07:53:55.000000 tiny_dag-0.0.2/src/tinydag/__init__.py
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)     5962 2024-04-27 08:13:34.000000 tiny_dag-0.0.2/src/tinydag/graph.py
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      711 2024-04-27 07:53:55.000000 tiny_dag-0.0.2/src/tinydag/node.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tiny-dag-0.0.1/src/tinydag/graph.py` & `tiny_dag-0.0.2/src/tinydag/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 from copy import copy
 from typing import List, Callable, Union
 
 import graphviz as graphviz
 from graphviz import Digraph
 
-from src.tinydag.node import Node
+from tinydag.node import Node
 
 logger = logging.getLogger(__name__)
 
 
 class GraphError(Exception):
     pass
```

### Comparing `tiny-dag-0.0.1/src/tinydag/node.py` & `tiny_dag-0.0.2/src/tinydag/node.py`

 * *Files identical despite different names*

### Comparing `tiny-dag-0.0.1/src/tiny_dag.egg-info/PKG-INFO` & `tiny_dag-0.0.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,26 @@
-Metadata-Version: 2.1
-Name: tiny-dag
-Version: 0.0.1
-Summary: Mimimal DAG implementation with Python
-Home-page: https://github.com/omyllymaki/tiny-dag
-Author: Ossi Myllymäki
-Author-email: omyllymaki@gmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/omyllymaki/tiny-dag/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Tiny DAG
 
 Bare bones implementation of computation (directed, acyclic) graph for Python.
 
 # Requirements
 
 - Python >= 3.6
 - graphviz
 
+# Installation
+
+Binary installers for the latest released version are available at the Python Package Index (PyPI):
+https://pypi.org/project/tiny-dag/
+
+Install by typing
+```
+pip3 install tiny-dag
+```
+
 # Usage example
 
 ```
 from tinydag.graph import Graph
 from tinydag.node import Node
 
 add = lambda a, b: a + b
@@ -45,9 +38,8 @@
 data = {"x": 5, "y": 3, "z": 3}
 results = graph.calculate(data)
 ```
 
 render method produces following figure:
 <p align="center">
 <img src="sample_graph.jpg" width="800px" />
-</p>
-
+</p>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tiny-dag-0.0.1/setup.cfg` & `tiny_dag-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tiny-dag
-version = 0.0.1
+version = 0.0.2
 author = Ossi Myllymäki
 author_email = omyllymaki@gmail.com
 description = Mimimal DAG implementation with Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/omyllymaki/tiny-dag
 project_urls =
```

### Comparing `tiny-dag-0.0.1/LICENSE` & `tiny_dag-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tiny-dag-0.0.1/PKG-INFO` & `tiny_dag-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 Metadata-Version: 2.1
 Name: tiny-dag
-Version: 0.0.1
+Version: 0.0.2
 Summary: Mimimal DAG implementation with Python
 Home-page: https://github.com/omyllymaki/tiny-dag
 Author: Ossi Myllymäki
 Author-email: omyllymaki@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/omyllymaki/tiny-dag/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: graphviz
 
 # Tiny DAG
 
 Bare bones implementation of computation (directed, acyclic) graph for Python.
 
 # Requirements
 
 - Python >= 3.6
 - graphviz
 
+# Installation
+
+Binary installers for the latest released version are available at the Python Package Index (PyPI):
+https://pypi.org/project/tiny-dag/
+
+Install by typing
+```
+pip3 install tiny-dag
+```
+
 # Usage example
 
 ```
 from tinydag.graph import Graph
 from tinydag.node import Node
 
 add = lambda a, b: a + b
@@ -46,8 +55,7 @@
 results = graph.calculate(data)
 ```
 
 render method produces following figure:
 <p align="center">
 <img src="sample_graph.jpg" width="800px" />
 </p>
-
```

