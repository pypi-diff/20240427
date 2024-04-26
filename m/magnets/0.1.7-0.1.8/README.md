# Comparing `tmp/magnets-0.1.7.tar.gz` & `tmp/magnets-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\magnets-0.1.7.tar", last modified: Fri Mar  4 16:37:04 2022, max compression
+gzip compressed data, was "magnets-0.1.8.tar", last modified: Sun Mar  3 22:52:53 2024, max compression
```

## Comparing `magnets-0.1.7.tar` & `magnets-0.1.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2022-03-04 16:37:04.891124 magnets-0.1.7/
--rw-rw-rw-   0        0        0      181 2021-05-13 18:27:43.000000 magnets-0.1.7/AUTHORS.rst
--rw-rw-rw-   0        0        0     3664 2021-05-13 18:27:43.000000 magnets-0.1.7/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2021-05-13 18:27:43.000000 magnets-0.1.7/HISTORY.rst
--rw-rw-rw-   0        0        0     1100 2021-05-13 18:27:43.000000 magnets-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      273 2021-05-13 18:27:43.000000 magnets-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     3774 2022-03-04 16:37:04.891124 magnets-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2200 2021-12-16 20:56:40.000000 magnets-0.1.7/README.rst
-drwxrwxrwx   0        0        0        0 2022-03-04 16:37:04.798368 magnets-0.1.7/docs/
--rw-rw-rw-   0        0        0      628 2021-05-13 18:27:43.000000 magnets-0.1.7/docs/Makefile
--rw-rw-rw-   0        0        0       29 2021-05-13 18:27:43.000000 magnets-0.1.7/docs/authors.rst
--rw-rw-rw-   0        0        0     4961 2021-05-13 18:27:43.000000 magnets-0.1.7/docs/conf.py
--rw-rw-rw-   0        0        0       34 2021-05-13 18:27:43.000000 magnets-0.1.7/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2021-05-13 18:27:43.000000 magnets-0.1.7/docs/history.rst
--rw-rw-rw-   0        0        0      324 2021-05-13 18:27:43.000000 magnets-0.1.7/docs/index.rst
--rw-rw-rw-   0        0        0     1181 2021-05-13 18:27:43.000000 magnets-0.1.7/docs/installation.rst
--rwxrwxrwx   0        0        0      805 2021-05-13 18:27:43.000000 magnets-0.1.7/docs/make.bat
--rw-rw-rw-   0        0        0       28 2021-05-13 18:27:43.000000 magnets-0.1.7/docs/readme.rst
--rw-rw-rw-   0        0        0       76 2021-05-13 18:27:43.000000 magnets-0.1.7/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2022-03-04 16:37:04.800368 magnets-0.1.7/magnets/
--rw-rw-rw-   0        0        0      247 2022-03-04 16:19:16.000000 magnets-0.1.7/magnets/__init__.py
-drwxrwxrwx   0        0        0        0 2022-03-04 16:37:04.850740 magnets-0.1.7/magnets/preprocessing/
--rw-rw-rw-   0        0        0       82 2021-03-27 23:47:36.000000 magnets-0.1.7/magnets/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     2792 2021-12-16 20:40:28.000000 magnets-0.1.7/magnets/preprocessing/branch_ends.py
--rw-rw-rw-   0        0        0     3931 2021-12-08 04:23:16.000000 magnets-0.1.7/magnets/preprocessing/parallel_pipes.py
-drwxrwxrwx   0        0        0        0 2022-03-04 16:37:04.867052 magnets-0.1.7/magnets/reduction/
--rw-rw-rw-   0        0        0      166 2021-05-01 18:14:20.000000 magnets-0.1.7/magnets/reduction/__init__.py
--rw-rw-rw-   0        0        0     1253 2022-01-18 20:44:55.000000 magnets-0.1.7/magnets/reduction/build_g_matrix.py
--rw-rw-rw-   0        0        0     9300 2022-03-04 16:07:08.000000 magnets-0.1.7/magnets/reduction/mod_reduction.py
--rw-rw-rw-   0        0        0     1756 2021-12-16 20:01:36.000000 magnets-0.1.7/magnets/reduction/reduce_model.py
--rw-rw-rw-   0        0        0     1216 2022-01-18 20:39:19.000000 magnets-0.1.7/magnets/reduction/reinitialize.py
-drwxrwxrwx   0        0        0        0 2022-03-04 16:37:04.876993 magnets-0.1.7/magnets/utils/
--rw-rw-rw-   0        0        0      189 2021-05-01 16:58:22.000000 magnets-0.1.7/magnets/utils/__init__.py
--rw-rw-rw-   0        0        0     2162 2021-12-16 20:03:47.000000 magnets-0.1.7/magnets/utils/call_on_functions.py
--rw-rw-rw-   0        0        0     6807 2022-01-18 20:41:30.000000 magnets-0.1.7/magnets/utils/characteristics.py
-drwxrwxrwx   0        0        0        0 2022-03-04 16:37:04.828065 magnets-0.1.7/magnets.egg-info/
--rw-rw-rw-   0        0        0     3774 2022-03-04 16:37:04.000000 magnets-0.1.7/magnets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      873 2022-03-04 16:37:04.000000 magnets-0.1.7/magnets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-04 16:37:04.000000 magnets-0.1.7/magnets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-05-13 20:57:36.000000 magnets-0.1.7/magnets.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      121 2022-03-04 16:37:04.000000 magnets-0.1.7/magnets.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-03-04 16:37:04.000000 magnets-0.1.7/magnets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      415 2022-03-04 16:37:04.897125 magnets-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1693 2022-03-04 16:19:16.000000 magnets-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2022-03-04 16:37:04.889999 magnets-0.1.7/tests/
--rw-rw-rw-   0        0        0       38 2021-05-13 18:27:43.000000 magnets-0.1.7/tests/__init__.py
--rw-rw-rw-   0        0        0      395 2021-05-13 21:20:53.000000 magnets-0.1.7/tests/test_magnets.py
+drwxrwxrwx   0        0        0        0 2024-03-03 22:52:53.248803 magnets-0.1.8/
+-rw-rw-rw-   0        0        0      181 2023-04-26 20:48:50.000000 magnets-0.1.8/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3664 2023-04-26 20:48:50.000000 magnets-0.1.8/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-26 20:48:50.000000 magnets-0.1.8/HISTORY.rst
+-rw-rw-rw-   0        0        0     1100 2023-04-26 20:48:50.000000 magnets-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-26 20:48:50.000000 magnets-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     7184 2024-03-03 22:52:53.249756 magnets-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6272 2024-03-03 22:36:48.000000 magnets-0.1.8/README.rst
+drwxrwxrwx   0        0        0        0 2024-03-03 22:52:53.008145 magnets-0.1.8/docs/
+-rw-rw-rw-   0        0        0      628 2023-04-26 20:48:50.000000 magnets-0.1.8/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-04-26 20:48:50.000000 magnets-0.1.8/docs/authors.rst
+-rw-rw-rw-   0        0        0     4961 2023-04-26 20:48:50.000000 magnets-0.1.8/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-04-26 20:48:50.000000 magnets-0.1.8/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-04-26 20:48:50.000000 magnets-0.1.8/docs/history.rst
+-rw-rw-rw-   0        0        0      324 2023-04-26 20:48:50.000000 magnets-0.1.8/docs/index.rst
+-rw-rw-rw-   0        0        0     1181 2023-04-26 20:48:50.000000 magnets-0.1.8/docs/installation.rst
+-rwxrwxrwx   0        0        0      805 2023-04-26 20:48:50.000000 magnets-0.1.8/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-04-26 20:48:50.000000 magnets-0.1.8/docs/readme.rst
+-rw-rw-rw-   0        0        0       76 2023-04-26 20:48:50.000000 magnets-0.1.8/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2024-03-03 22:52:53.010641 magnets-0.1.8/magnets/
+-rw-rw-rw-   0        0        0      247 2024-03-03 22:45:23.000000 magnets-0.1.8/magnets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-03 22:52:53.101306 magnets-0.1.8/magnets/preprocessing/
+-rw-rw-rw-   0        0        0       82 2023-04-26 20:48:50.000000 magnets-0.1.8/magnets/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2792 2023-04-26 20:48:50.000000 magnets-0.1.8/magnets/preprocessing/branch_ends.py
+-rw-rw-rw-   0        0        0     3931 2023-04-26 20:48:50.000000 magnets-0.1.8/magnets/preprocessing/parallel_pipes.py
+drwxrwxrwx   0        0        0        0 2024-03-03 22:52:53.180843 magnets-0.1.8/magnets/reduction/
+-rw-rw-rw-   0        0        0      166 2023-04-26 20:48:50.000000 magnets-0.1.8/magnets/reduction/__init__.py
+-rw-rw-rw-   0        0        0     1253 2023-04-26 20:48:50.000000 magnets-0.1.8/magnets/reduction/build_g_matrix.py
+-rw-rw-rw-   0        0        0     9419 2023-04-26 21:39:05.000000 magnets-0.1.8/magnets/reduction/mod_reduction.py
+-rw-rw-rw-   0        0        0     1793 2023-04-26 20:58:27.000000 magnets-0.1.8/magnets/reduction/reduce_model.py
+-rw-rw-rw-   0        0        0     1216 2023-04-26 20:48:50.000000 magnets-0.1.8/magnets/reduction/reinitialize.py
+drwxrwxrwx   0        0        0        0 2024-03-03 22:52:53.223907 magnets-0.1.8/magnets/utils/
+-rw-rw-rw-   0        0        0      189 2023-04-26 20:48:50.000000 magnets-0.1.8/magnets/utils/__init__.py
+-rw-rw-rw-   0        0        0     2409 2023-04-26 21:28:12.000000 magnets-0.1.8/magnets/utils/call_on_functions.py
+-rw-rw-rw-   0        0        0     6807 2023-04-26 20:48:50.000000 magnets-0.1.8/magnets/utils/characteristics.py
+drwxrwxrwx   0        0        0        0 2024-03-03 22:52:53.056515 magnets-0.1.8/magnets.egg-info/
+-rw-rw-rw-   0        0        0     7184 2024-03-03 22:52:52.000000 magnets-0.1.8/magnets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      873 2024-03-03 22:52:52.000000 magnets-0.1.8/magnets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-03 22:52:52.000000 magnets-0.1.8/magnets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-26 21:36:55.000000 magnets-0.1.8/magnets.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      121 2024-03-03 22:52:52.000000 magnets-0.1.8/magnets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-03-03 22:52:52.000000 magnets-0.1.8/magnets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      415 2024-03-03 22:52:53.253723 magnets-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1694 2024-03-03 22:45:23.000000 magnets-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-03 22:52:53.247761 magnets-0.1.8/tests/
+-rw-rw-rw-   0        0        0       38 2023-04-26 20:48:50.000000 magnets-0.1.8/tests/__init__.py
+-rw-rw-rw-   0        0        0      395 2023-04-26 20:48:50.000000 magnets-0.1.8/tests/test_magnets.py
```

### Comparing `magnets-0.1.7/CONTRIBUTING.rst` & `magnets-0.1.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `magnets-0.1.7/LICENSE` & `magnets-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `magnets-0.1.7/docs/Makefile` & `magnets-0.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `magnets-0.1.7/docs/conf.py` & `magnets-0.1.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `magnets-0.1.7/docs/installation.rst` & `magnets-0.1.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `magnets-0.1.7/docs/make.bat` & `magnets-0.1.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `magnets-0.1.7/magnets/preprocessing/branch_ends.py` & `magnets-0.1.8/magnets/preprocessing/branch_ends.py`

 * *Files identical despite different names*

### Comparing `magnets-0.1.7/magnets/preprocessing/parallel_pipes.py` & `magnets-0.1.8/magnets/preprocessing/parallel_pipes.py`

 * *Files identical despite different names*

### Comparing `magnets-0.1.7/magnets/reduction/build_g_matrix.py` & `magnets-0.1.8/magnets/reduction/build_g_matrix.py`

 * *Files identical despite different names*

### Comparing `magnets-0.1.7/magnets/reduction/mod_reduction.py` & `magnets-0.1.8/magnets/reduction/mod_reduction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import wntr
 from magnets.reduction import build_g_matrix
 from magnets.reduction import reinitialize
 from magnets.utils.characteristics import *
 from magnets.utils.call_on_functions import *
 import warnings
 
-def mod_reduction(wn, new_link_list, junc_dict, pipe_dict, unremovable_nodes, relations, nodes_to_be_removed, new_pipe_len, alpha, inp_file, max_nodal_degree, op_pt):
+def mod_reduction(wn, new_link_list, junc_dict, pipe_dict, unremovable_nodes, relations, nodes_to_be_removed, new_pipe_len, alpha, inp_file, max_nodal_degree, op_pt, save_filename):
     
     if max_nodal_degree == None: 
         max_nodal_degree = 100
         
     if (max_nodal_degree < 1 or (isinstance(max_nodal_degree, int) == False and max_nodal_degree != None)):
         warnings.warn('Invalid maximum nodal degree provided by user. \ Running simulation with maximum nodal degree = 100.')
         max_nodal_degree = 100
@@ -146,17 +146,20 @@
             
             for value in relations.values():
                 if removal_node in value:
                     value.remove(removal_node)
             for k in range(num_junc):
                 if removal_node in junc_dict[junc_names[k]]['Connected nodes']:
                     junc_dict[junc_names[k]]['Connected nodes'].remove(removal_node)
-                    
-    if '/' in inp_file:
-        index = inp_file.rindex('/') + 1
-        new_name = inp_file[:index] + 'reduced ' + str(op_pt) + ' ' + inp_file[index:] 
-        wn.write_inpfile(new_name)
-        
+    
+    if save_filename == None:
+        if '/' in inp_file:
+            index = inp_file.rindex('/') + 1
+            new_name = inp_file[:index] + 'reduced ' + str(op_pt) + ' ' + inp_file[index:] 
+            writeinpfile(wn, new_name)
+            
+        else:
+            writeinpfile(wn, 'reduced {} {}'.format(op_pt, inp_file))
     else:
-        wn.write_inpfile('reduced {} {}'.format(op_pt, inp_file))
+        writeinpfile(wn, save_filename + '.inp')
                     
     return 1
```

### Comparing `magnets-0.1.7/magnets/reduction/reduce_model.py` & `magnets-0.1.8/magnets/reduction/reduce_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from magnets.utils import call_on_functions
 from magnets.preprocessing import branch_ends 
 from magnets.preprocessing import parallel_pipes
 from magnets.reduction import reinitialize
 from magnets.reduction import build_g_matrix
 from magnets.reduction import mod_reduction
 
-def reduce_model(inp_file, op_pt = None, nodes_to_keep = None, max_nodal_degree = None):
+def reduce_model(inp_file, op_pt = None, nodes_to_keep = None, max_nodal_degree = None, save_filename = None):
     
     # initialize lists and junction/pipe characteristics
     wn, op_pt,  pipe_dict,junc_dict,unremovable_nodes,special_nodes,special_links,special_links_nodes, relations, new_link_list, results = characteristics(inp_file, op_pt, nodes_to_keep)
     
     # define constants
     alpha = call_on_functions.calculate_unit_coeff(pipe_dict, junc_dict, wn, results, op_pt, special_nodes)
     new_pipe_len = call_on_functions.new_pipe_length(wn, pipe_dict)
@@ -20,11 +20,11 @@
     # remove branch end nodes and merge parallel pipes
     wn, junc_dict, pipe_dict, relations, new_link_list = branch_ends(relations, wn, new_link_list, junc_dict, pipe_dict, unremovable_nodes)
     wn, junc_dict, pipe_dict, relations, new_link_list = parallel_pipes(relations, wn, new_link_list, junc_dict, pipe_dict, unremovable_nodes, special_nodes, special_links_nodes, special_links, alpha)
        
     # reduce model
     nodes_to_be_removed, link_list_only_junc, unremovable_nodes = reinitialize(wn,new_link_list, special_nodes, unremovable_nodes)
     junc_dict, pipe_dict = build_g_matrix(wn,junc_dict,pipe_dict, unremovable_nodes, special_nodes, alpha)
-    mod_reduction(wn, new_link_list, junc_dict, pipe_dict, unremovable_nodes, relations, nodes_to_be_removed, new_pipe_len, alpha, inp_file, max_nodal_degree, op_pt)
+    mod_reduction(wn, new_link_list, junc_dict, pipe_dict, unremovable_nodes, relations, nodes_to_be_removed, new_pipe_len, alpha, inp_file, max_nodal_degree, op_pt, save_filename)
     
     return wn
```

### Comparing `magnets-0.1.7/magnets/reduction/reinitialize.py` & `magnets-0.1.8/magnets/reduction/reinitialize.py`

 * *Files identical despite different names*

### Comparing `magnets-0.1.7/magnets/utils/call_on_functions.py` & `magnets-0.1.8/magnets/utils/call_on_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import numpy as np
+from packaging.version import Version, parse
+import wntr
 
 epsilon = 10**(-6)
 
 #function to calculate alpha
 def calculate_unit_coeff(pipe_dict, junc_dict, wn, results, op_pt, special_nodes):
     alpha = []
     pipe_names = wn.pipe_name_list
@@ -57,7 +59,13 @@
 #function to calculate pipe length of all new pipes
 def new_pipe_length(wn, pipe_dict):
     lengths = []
     pipe_names = wn.pipe_name_list
     for i in range(len(wn.pipe_name_list)):
         lengths.append(pipe_dict[pipe_names[i]]['Length'])
     return (np.mean(np.array(lengths)))
+
+def writeinpfile(wn, new_name):
+    if parse(str(wntr.__version__)) < parse('0.5.0'):
+        wn.write_inpfile(new_name)
+    else:
+        wntr.network.io.write_inpfile(wn, new_name)
```

### Comparing `magnets-0.1.7/magnets/utils/characteristics.py` & `magnets-0.1.8/magnets/utils/characteristics.py`

 * *Files identical despite different names*

### Comparing `magnets-0.1.7/magnets.egg-info/SOURCES.txt` & `magnets-0.1.8/magnets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magnets-0.1.7/setup.py` & `magnets-0.1.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     'pandas',
     'Pillow',
     'pyparsing',
     'python-dateutil',
     'pytz',
     'scipy',
     'six',
-    'wntr>=0.3.0'
+    'wntr>=0.3.0',
 ]
 
 setup_requirements = [ ]
 
 test_requirements = [ ]
 
 setup(
@@ -54,10 +54,10 @@
     keywords='magnets',
     name='magnets',
     packages=find_packages(include=['magnets', 'magnets.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/meghnathomas/magnets',
-    version='0.1.7',
+    version='0.1.8',
     zip_safe=False,
 )
```

