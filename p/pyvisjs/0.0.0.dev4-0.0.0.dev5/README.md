# Comparing `tmp/pyvisjs-0.0.0.dev4.tar.gz` & `tmp/pyvisjs-0.0.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvisjs-0.0.0.dev4.tar", last modified: Wed Apr 24 18:49:31 2024, max compression
+gzip compressed data, was "pyvisjs-0.0.0.dev5.tar", last modified: Sat Apr 27 15:43:50 2024, max compression
```

## Comparing `pyvisjs-0.0.0.dev4.tar` & `pyvisjs-0.0.0.dev5.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 18:49:31.507796 pyvisjs-0.0.0.dev4/
--rw-rw-rw-   0 root         (0) root         (0)     1355 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1054 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     3452 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3384 2024-04-24 18:49:31.507796 pyvisjs-0.0.0.dev4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1454 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 18:49:31.502796 pyvisjs-0.0.0.dev4/examples/
--rw-rw-rw-   0 root         (0) root         (0)      537 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/examples/main.py
--rw-rw-rw-   0 root         (0) root         (0)      194 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/examples/readme_usage.py
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/folder_structure.txt
--rw-rw-rw-   0 root         (0) root         (0)      830 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 18:49:31.504796 pyvisjs-0.0.0.dev4/pyvisjs/
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/pyvisjs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/pyvisjs/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/pyvisjs/edge.py
--rw-rw-rw-   0 root         (0) root         (0)     1786 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/pyvisjs/network.py
--rw-rw-rw-   0 root         (0) root         (0)      687 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/pyvisjs/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 18:49:31.505796 pyvisjs-0.0.0.dev4/pyvisjs/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1043 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/pyvisjs/templates/basic.html
--rw-rw-rw-   0 root         (0) root         (0)     1114 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/pyvisjs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 18:49:31.506796 pyvisjs-0.0.0.dev4/pyvisjs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3384 2024-04-24 18:49:31.000000 pyvisjs-0.0.0.dev4/pyvisjs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      543 2024-04-24 18:49:31.000000 pyvisjs-0.0.0.dev4/pyvisjs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 18:49:31.000000 pyvisjs-0.0.0.dev4/pyvisjs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-24 18:49:31.000000 pyvisjs-0.0.0.dev4/pyvisjs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-24 18:49:31.000000 pyvisjs-0.0.0.dev4/pyvisjs.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 18:49:31.507796 pyvisjs-0.0.0.dev4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 18:49:31.506796 pyvisjs-0.0.0.dev4/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      778 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/tests/test_edge.py
--rw-rw-rw-   0 root         (0) root         (0)     5310 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/tests/test_network.py
--rw-rw-rw-   0 root         (0) root         (0)     1540 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/tests/test_node.py
--rw-rw-rw-   0 root         (0) root         (0)     2507 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 15:43:50.510591 pyvisjs-0.0.0.dev5/
+-rw-rw-rw-   0 root         (0) root         (0)     1355 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3452 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3384 2024-04-27 15:43:50.510591 pyvisjs-0.0.0.dev5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1454 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 15:43:50.505591 pyvisjs-0.0.0.dev5/examples/
+-rw-rw-rw-   0 root         (0) root         (0)      539 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/examples/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      194 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/examples/readme_usage.py
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/folder_structure.txt
+-rw-rw-rw-   0 root         (0) root         (0)      830 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 15:43:50.507591 pyvisjs-0.0.0.dev5/pyvisjs/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/pyvisjs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/pyvisjs/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/pyvisjs/base_dictable.py
+-rw-rw-rw-   0 root         (0) root         (0)      478 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/pyvisjs/edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/pyvisjs/network.py
+-rw-rw-rw-   0 root         (0) root         (0)      478 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/pyvisjs/node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 15:43:50.508591 pyvisjs-0.0.0.dev5/pyvisjs/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      899 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/pyvisjs/templates/basic.html
+-rw-rw-rw-   0 root         (0) root         (0)      998 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/pyvisjs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 15:43:50.509590 pyvisjs-0.0.0.dev5/pyvisjs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3384 2024-04-27 15:43:50.000000 pyvisjs-0.0.0.dev5/pyvisjs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      596 2024-04-27 15:43:50.000000 pyvisjs-0.0.0.dev5/pyvisjs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 15:43:50.000000 pyvisjs-0.0.0.dev5/pyvisjs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-27 15:43:50.000000 pyvisjs-0.0.0.dev5/pyvisjs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-27 15:43:50.000000 pyvisjs-0.0.0.dev5/pyvisjs.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 15:43:50.510591 pyvisjs-0.0.0.dev5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 15:43:50.509590 pyvisjs-0.0.0.dev5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1921 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/tests/test_base_dictable.py
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/tests/test_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     6122 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/tests/test_network.py
+-rw-rw-rw-   0 root         (0) root         (0)     1142 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/tests/test_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2507 2024-04-27 15:43:35.000000 pyvisjs-0.0.0.dev5/tests/test_utils.py
```

### Comparing `pyvisjs-0.0.0.dev4/.gitignore` & `pyvisjs-0.0.0.dev5/.gitignore`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev4/.gitlab-ci.yml` & `pyvisjs-0.0.0.dev5/.gitlab-ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -21,21 +21,17 @@
   before_script:
     - pip install --upgrade pip
     - pip install -r requirements.txt
     - pip install -e .
   script:
     - pytest --noconftest
   rules:
-    - when: on_success
-      changes:
-        - "*.py"
-    - when: never
-      changes:
-        - "_version.py"
-        - "examples/**/*"
+    - changes:
+        - pyvisjs/[^_]*.py
+        - tests/*.py
 #  except:
 #    - dev
 #  only:
 #    - dev
 
 deploy_to_pypi:
   stage: deploy
```

### Comparing `pyvisjs-0.0.0.dev4/CONTRIBUTING.md` & `pyvisjs-0.0.0.dev5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev4/LICENSE` & `pyvisjs-0.0.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev4/PKG-INFO` & `pyvisjs-0.0.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 0.0.0.dev4
+Version: 0.0.0.dev5
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyvisjs-0.0.0.dev4/README.md` & `pyvisjs-0.0.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev4/examples/main.py` & `pyvisjs-0.0.0.dev5/examples/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pyvisjs import Network, Node, Edge
 
 def main() -> None:
 
     nd1 = Node(1, "node! 1")
     nd2 = Node(2, "node!! 2")
     nd3 = Node(3, "node!!! 3")
-    nd4 = Node(4, "node!!!! 4")
+    nd4 = Node(4, "node!!!!!! 4")
 
     eg1 = Edge(1, 2)
     eg2 = Edge(2, 3)
     eg3 = Edge(3, 4)
 
     data = {
         "nodes": [nd1, nd2, nd3, nd4],
```

### Comparing `pyvisjs-0.0.0.dev4/folder_structure.txt` & `pyvisjs-0.0.0.dev5/folder_structure.txt`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev4/pyproject.toml` & `pyvisjs-0.0.0.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev4/pyvisjs/network.py` & `pyvisjs-0.0.0.dev5/pyvisjs/network.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from .base_dictable import BaseDictable
 from .utils import open_file, save_file
 from .node import Node
 from .edge import Edge
 from jinja2 import Environment, PackageLoader, select_autoescape
 from typing import Dict
 
-class Network:
+class Network(BaseDictable):
 
     def __init__(self, name="Network", data:Dict = {"nodes": [], "edges": []}, width="600px", height="400px"):
+        only_show_data_attr = lambda attr: attr == "data"
+        super().__init__(attr_filter_func=only_show_data_attr)
         self.name = name
         self.width = width
         self.height = height
         self.data = data
         self.env = Environment(
             loader=PackageLoader("pyvisjs"),
             autoescape=select_autoescape()
@@ -26,24 +29,27 @@
     def add_edge(self, from_id, to_id):
         self.add_node(from_id)
         self.add_node(to_id)
 
         if not [edge.start for edge in self.data["edges"] if edge.start == from_id and edge.end == to_id]:
             self.data["edges"].append(Edge(from_id, to_id))
 
+    def to_dict(self):
+        return super().to_dict()["data"]
+
     def show(self, file_name):
         self.render_template(open_in_browser=True, output_filename=file_name)
 
     def render_template(self, open_in_browser=False, save_to_output=False, output_filename="default.html", template_filename="basic.html") -> str:
         html_output = self.env \
             .get_template(template_filename) \
             .render(
                 width=self.width,
                 height=self.height,
-                data=self.data
+                data=self.to_dict()
             )
 
         if save_to_output or open_in_browser:
             file_path = save_file(output_filename, html_output)
 
         if open_in_browser:
             open_file(file_path)
```

### Comparing `pyvisjs-0.0.0.dev4/pyvisjs/templates/basic.html` & `pyvisjs-0.0.0.dev5/pyvisjs/templates/basic.html`

 * *Files 23% similar despite different names*

```diff
@@ -12,26 +12,18 @@
 </head>
 
 <body>
 <div id="visjsnet"></div>
 
 <script type="text/javascript">
     // create an array with nodes
-    var nodes = new vis.DataSet([
-    {% for node in data["nodes"] %}
-        {{ node.to_json()|safe }},
-    {%- endfor %}
-    ]);
+    var nodes = new vis.DataSet({{data["nodes"]|tojson}});
 
     // create an array with edges
-    var edges = new vis.DataSet([
-    {% for edge in data["edges"] %}
-        {{ edge.to_json()|safe }},
-    {%- endfor %}
-    ]);
+    var edges = new vis.DataSet({{data["edges"]|tojson}});
 
     // create a network
     var container = document.getElementById('visjsnet');
 
     // provide the data in the vis format
     var data = {
         nodes: nodes,
```

### Comparing `pyvisjs-0.0.0.dev4/pyvisjs/utils.py` & `pyvisjs-0.0.0.dev5/pyvisjs/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,19 +5,14 @@
 def open_file(url):
     """
     :param url: web url or a file path on your computer
     >>> open_file("https://stackoverflow.com")
     >>> open_file("\\\\pyvisjs\\\\templates\\\\basic.html")  
     """
 
-    #current_directory = os.getcwd()
-
-    #if current_directory not in url:
-    #    url = current_directory + url
-
     try: # should work on Windows
         os.startfile(url)
     except AttributeError:
         try: # should work on MacOS and most linux versions
             subprocess.call(['open', url])
         except:
             raise
```

### Comparing `pyvisjs-0.0.0.dev4/pyvisjs.egg-info/PKG-INFO` & `pyvisjs-0.0.0.dev5/pyvisjs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 0.0.0.dev4
+Version: 0.0.0.dev5
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyvisjs-0.0.0.dev4/pyvisjs.egg-info/SOURCES.txt` & `pyvisjs-0.0.0.dev5/pyvisjs.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 folder_structure.txt
 pyproject.toml
 requirements.txt
 examples/main.py
 examples/readme_usage.py
 pyvisjs/__init__.py
 pyvisjs/_version.py
+pyvisjs/base_dictable.py
 pyvisjs/edge.py
 pyvisjs/network.py
 pyvisjs/node.py
 pyvisjs/utils.py
 pyvisjs.egg-info/PKG-INFO
 pyvisjs.egg-info/SOURCES.txt
 pyvisjs.egg-info/dependency_links.txt
 pyvisjs.egg-info/requires.txt
 pyvisjs.egg-info/top_level.txt
 pyvisjs/templates/basic.html
 tests/__init__.py
+tests/test_base_dictable.py
 tests/test_edge.py
 tests/test_network.py
 tests/test_node.py
 tests/test_utils.py
```

### Comparing `pyvisjs-0.0.0.dev4/tests/test_edge.py` & `pyvisjs-0.0.0.dev5/tests/test_edge.py`

 * *Files 21% similar despite different names*

```diff
@@ -27,21 +27,7 @@
     # mock
 
     # call
     e = Edge(START_ID, END_ID)
     
     # assert
     assert e.to_dict() == EDGE_DICT
-
-def test_edge_to_json():
-    # init
-    START_ID = 1
-    END_ID = 2
-    EDGE_JSON = f"""{{"from": {START_ID}, "to": {END_ID}}}"""
-
-    # mock
-
-    # call
-    e = Edge(START_ID, END_ID)
-    
-    # assert
-    assert e.to_json() == EDGE_JSON
```

### Comparing `pyvisjs-0.0.0.dev4/tests/test_network.py` & `pyvisjs-0.0.0.dev5/tests/test_network.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,24 +7,24 @@
     DEFAULT_WIDTH = "600px"
     DEFAULT_HEIGHT = "400px"
 
     # mock
 
 
     # call
-    n = Network("Network1")
+    n = Network("Network2")
     
     # assert
-    assert n.name == "Network1"
+    assert n.name == "Network2"
     assert n.width == DEFAULT_WIDTH
     assert n.height == DEFAULT_HEIGHT
     assert n.env is not None
     assert n.data == {"nodes": [], "edges": []}
 
-def test_add_nodes():
+def test_network_add_nodes():
     # init
 
     # mock
 
     # call
     n = Network("Network1")
     n.add_node(1)
@@ -34,15 +34,15 @@
     # assert
     assert len(n.data["nodes"]) == 2
     assert n.data["nodes"][0].id == 1
     assert n.data["nodes"][0].label == "1"
     assert n.data["nodes"][1].id == 2
     assert n.data["nodes"][1].label == "name2"
 
-def test_add_edges():
+def test_network_add_edges():
     # init
 
     # mock
 
     # call
     n = Network("Network1")
     n.add_node(1)
@@ -58,18 +58,45 @@
 
     assert len(n.data["edges"]) == 2
     assert n.data["edges"][0].start == 1
     assert n.data["edges"][0].end == 2
     assert n.data["edges"][1].start == 2
     assert n.data["edges"][1].end == 3
 
+def test_network_to_dict():
+    # init
+    NETWORK_DICT = {
+        "nodes": [
+            { "id": 1, "label": "1", "color": None, "shape": "dot", "size": None, "cid": None },
+            { "id": 2, "label": "name2", "color": None, "shape": "dot", "size": None, "cid": None },
+            { "id": 3, "label": "3", "color": None, "shape": "dot", "size": None, "cid": None },
+        ],
+        "edges": [
+            { "from": 1, "to": 2 },
+            { "from": 2, "to": 3 }
+        ]
+    }
+
+    # mock
+
+    # call
+    n = Network("Network1")
+    n.add_node(1)
+    n.add_node(2, "name2")
+    n.add_edge(1, 2) # both nodes exist
+    n.add_edge(2, 3) # one node missing
+    n.add_edge(2, 3) # duplicate edge
+    
+    # assert
+    assert n.to_dict() == NETWORK_DICT
+
 @patch('pyvisjs.network.open_file')
 @patch('pyvisjs.network.save_file')
 @patch('pyvisjs.network.Environment')
-def test_render_template_with_all_default_values(mock_Environment, mock_save_file, mock_open_file):
+def test_network_render_template_with_all_default_values(mock_Environment, mock_save_file, mock_open_file):
     # init
     RENDER_RESULT = "<html>template</html>"
     DEFAULT_TEMPLATE_FILENAME = "basic.html"
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
     mock_render = mock_get_template.return_value.render
@@ -85,15 +112,15 @@
     mock_open_file.assert_not_called()
     assert html_output == RENDER_RESULT
 
 
 @patch('pyvisjs.network.open_file')
 @patch('pyvisjs.network.save_file')
 @patch('pyvisjs.network.Environment')
-def test_render_template_with_open_in_browser(mock_Environment, mock_save_file, mock_open_file):
+def test_network_render_template_with_open_in_browser(mock_Environment, mock_save_file, mock_open_file):
     # init
     RENDER_RESULT = "<html>template</html>"
     DEFAULT_TEMPLATE_FILENAME = "basic.html"
     DEFAULT_OUTPUT_FILENAME = "default.html"
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
@@ -111,15 +138,15 @@
     mock_open_file.assert_called_once_with(DEFAULT_OUTPUT_FILENAME)
     assert html_output == RENDER_RESULT
 
 
 @patch('pyvisjs.network.open_file')
 @patch('pyvisjs.network.save_file')
 @patch('pyvisjs.network.Environment')
-def test_render_template_with_save_to_output(mock_Environment, mock_save_file, mock_open_file):
+def test_network_render_template_with_save_to_output(mock_Environment, mock_save_file, mock_open_file):
     # init
     RENDER_RESULT = "<html>template</html>"
     DEFAULT_TEMPLATE_FILENAME = "basic.html"
     DEFAULT_OUTPUT_FILENAME = "default.html"
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
@@ -136,15 +163,15 @@
     mock_open_file.assert_not_called()
     assert html_output == RENDER_RESULT
 
 
 @patch('pyvisjs.network.open_file')
 @patch('pyvisjs.network.save_file')
 @patch('pyvisjs.network.Environment')
-def test_render_template_with_open_and_save_no_defaults(mock_Environment, mock_save_file, mock_open_file):
+def test_network_render_template_with_open_and_save_no_defaults(mock_Environment, mock_save_file, mock_open_file):
     # init
     RENDER_RESULT = "<html>template</html>"
     CUSTOM_TEMPLATE_FILENAME = "custom_template.html"
     CUSTOM_OUTPUT_FILENAME = "custom_output.html"
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
```

### Comparing `pyvisjs-0.0.0.dev4/tests/test_node.py` & `pyvisjs-0.0.0.dev5/tests/test_node.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,40 +30,25 @@
 
 def test_node_to_dict():
     # init
     NODE_ID = 1
     NODE_LABEL = "label"
     NODE_COLOR = "lime"
     NODE_SHAPE = "circle"
+    NODE_CID = None
     NODE_SIZE = 50
     NODE_DICT = {
             "id": NODE_ID,
             "label": NODE_LABEL,
             "color": NODE_COLOR,
             "shape": NODE_SHAPE,
             "size": NODE_SIZE,
+            "cid": NODE_CID,
         }
 
     # mock
 
     # call
     n = Node(NODE_ID, NODE_LABEL, NODE_COLOR, NODE_SHAPE, NODE_SIZE)
     
     # assert
     assert n.to_dict() == NODE_DICT
-
-def test_node_to_json():
-    # init
-    NODE_ID = 1
-    NODE_LABEL = "label1"
-    NODE_COLOR = "lime"
-    NODE_SHAPE = "circle"
-    NODE_SIZE = 50
-    NODE_JSON = f"""{{"id": {NODE_ID}, "label": "{NODE_LABEL}", "color": "{NODE_COLOR}", "shape": "{NODE_SHAPE}", "size": {NODE_SIZE}}}"""
-
-    # mock
-
-    # call
-    n = Node(NODE_ID, NODE_LABEL, NODE_COLOR, NODE_SHAPE, NODE_SIZE)
-    
-    # assert
-    assert n.to_json() == NODE_JSON
```

### Comparing `pyvisjs-0.0.0.dev4/tests/test_utils.py` & `pyvisjs-0.0.0.dev5/tests/test_utils.py`

 * *Files identical despite different names*

