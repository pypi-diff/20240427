# Comparing `tmp/pygmtools-0.5.1.tar.gz` & `tmp/pygmtools-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmtools-0.5.1.tar", last modified: Wed Apr  3 23:16:29 2024, max compression
+gzip compressed data, was "pygmtools-0.5.2.tar", last modified: Sat Apr 27 19:07:21 2024, max compression
```

## Comparing `pygmtools-0.5.1.tar` & `pygmtools-0.5.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:16:29.978067 pygmtools-0.5.1/
--rwxr-xr-x   0 runner    (1001) docker     (127)      508 2024-04-03 23:16:20.000000 pygmtools-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 23:16:20.000000 pygmtools-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15977 2024-04-03 23:16:29.978067 pygmtools-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14371 2024-04-03 23:16:20.000000 pygmtools-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:16:29.978067 pygmtools-0.5.1/pygmtools/
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26430 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:16:29.978067 pygmtools-0.5.1/pygmtools/c_astar_src/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/c_astar_src/build_c_astar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/c_astar_src/c_astar.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/c_astar_src/c_astar_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/c_astar_src/priority_queue.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    53433 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/classic_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)    59047 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/dataset_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    59923 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/jittor_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/jittor_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    75822 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/linear_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)    21672 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/mindspore_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    43957 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/multi_graph_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)    81238 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/neural_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)    61477 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15282 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/numpy_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    59058 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/paddle_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    11632 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/paddle_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    30385 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/pytorch_astar_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    62804 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/pytorch_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/pytorch_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    23331 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/tensorflow_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/tensorflow_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    74983 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:16:29.978067 pygmtools-0.5.1/pygmtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15977 2024-04-03 23:16:29.000000 pygmtools-0.5.1/pygmtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-03 23:16:29.000000 pygmtools-0.5.1/pygmtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:16:29.000000 pygmtools-0.5.1/pygmtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-03 23:16:29.000000 pygmtools-0.5.1/pygmtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 23:16:29.000000 pygmtools-0.5.1/pygmtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 23:16:29.978067 pygmtools-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-03 23:16:20.000000 pygmtools-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:16:29.978067 pygmtools-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    21581 2024-04-03 23:16:20.000000 pygmtools-0.5.1/tests/test_classic_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-03 23:16:20.000000 pygmtools-0.5.1/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-03 23:16:20.000000 pygmtools-0.5.1/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-04-03 23:16:20.000000 pygmtools-0.5.1/tests/test_multi_graph_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13700 2024-04-03 23:16:20.000000 pygmtools-0.5.1/tests/test_neural_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-03 23:16:20.000000 pygmtools-0.5.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:07:21.512845 pygmtools-0.5.2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      508 2024-04-27 19:07:05.000000 pygmtools-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 19:07:05.000000 pygmtools-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15977 2024-04-27 19:07:21.512845 pygmtools-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14371 2024-04-27 19:07:05.000000 pygmtools-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:07:21.508845 pygmtools-0.5.2/pygmtools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26430 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:07:21.512845 pygmtools-0.5.2/pygmtools/c_astar_src/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/c_astar_src/build_c_astar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/c_astar_src/c_astar.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/c_astar_src/c_astar_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/c_astar_src/priority_queue.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    54259 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/classic_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59047 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/dataset_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60291 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/jittor_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/jittor_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75894 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/linear_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21755 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/mindspore_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43957 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/multi_graph_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81418 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/neural_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61671 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15282 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/numpy_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59318 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/paddle_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11632 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/paddle_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30385 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/pytorch_astar_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62937 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/pytorch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/pytorch_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23472 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/tensorflow_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/tensorflow_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75064 2024-04-27 19:07:06.000000 pygmtools-0.5.2/pygmtools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:07:21.512845 pygmtools-0.5.2/pygmtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15977 2024-04-27 19:07:21.000000 pygmtools-0.5.2/pygmtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-27 19:07:21.000000 pygmtools-0.5.2/pygmtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 19:07:21.000000 pygmtools-0.5.2/pygmtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-27 19:07:21.000000 pygmtools-0.5.2/pygmtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-27 19:07:21.000000 pygmtools-0.5.2/pygmtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 19:07:21.512845 pygmtools-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-27 19:07:06.000000 pygmtools-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:07:21.512845 pygmtools-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    21582 2024-04-27 19:07:06.000000 pygmtools-0.5.2/tests/test_classic_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-27 19:07:06.000000 pygmtools-0.5.2/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-27 19:07:06.000000 pygmtools-0.5.2/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-04-27 19:07:06.000000 pygmtools-0.5.2/tests/test_multi_graph_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13700 2024-04-27 19:07:06.000000 pygmtools-0.5.2/tests/test_neural_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-27 19:07:06.000000 pygmtools-0.5.2/tests/test_utils.py
```

### Comparing `pygmtools-0.5.1/PKG-INFO` & `pygmtools-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtools
-Version: 0.5.1
+Version: 0.5.2
 Summary: pygmtools provides graph matching solvers in Python API and supports numpy and pytorch backends. pygmtools also provides dataset API for standard graph matching benchmarks.
 Home-page: https://pygmtools.readthedocs.io/
 Author: ThinkLab at SJTU
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pygmtools-0.5.1/README.md` & `pygmtools-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.1/pygmtools/__init__.py` & `pygmtools-0.5.2/pygmtools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .multi_graph_solvers import cao, mgm_floyd, gamgm
 from .neural_solvers import pca_gm, ipca_gm, cie, ngm, genn_astar
 import pygmtools.utils as utils
 import importlib.util
 set_backend = utils.set_backend
 
 BACKEND = 'numpy'
-__version__ = '0.5.1'
+__version__ = '0.5.2'
 __author__ = 'ThinkLab at SJTU'
 
 SUPPORTED_BACKENDS = [
     'numpy',
     'pytorch',
     'jittor',
     'paddle',
```

### Comparing `pygmtools-0.5.1/pygmtools/benchmark.py` & `pygmtools-0.5.2/pygmtools/benchmark.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.1/pygmtools/c_astar_src/build_c_astar.py` & `pygmtools-0.5.2/pygmtools/c_astar_src/build_c_astar.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.1/pygmtools/c_astar_src/c_astar.pyx` & `pygmtools-0.5.2/pygmtools/c_astar_src/c_astar.pyx`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.1/pygmtools/c_astar_src/priority_queue.hpp` & `pygmtools-0.5.2/pygmtools/c_astar_src/priority_queue.hpp`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.1/pygmtools/classic_solvers.py` & `pygmtools-0.5.2/pygmtools/classic_solvers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,32 @@
 r"""
 Classic (learning-free) **two-graph matching** solvers. These two-graph matching solvers are recommended to solve
 matching problems with two explicit graphs, or problems formulated as Quadratic Assignment Problem (QAP).
 
-The two-graph matching problem considers both nodes and edges, formulated as a QAP (Lawler's):
+The two-graph matching problem considers both nodes and edges, formulated as Lawler's QAP:
 
 .. math::
 
     &\max_{\mathbf{X}} \ \texttt{vec}(\mathbf{X})^\top \mathbf{K} \texttt{vec}(\mathbf{X})\\
     s.t. \quad &\mathbf{X} \in \{0, 1\}^{n_1\times n_2}, \ \mathbf{X}\mathbf{1} = \mathbf{1}, \ \mathbf{X}^\top\mathbf{1} \leq \mathbf{1}
+
+All our solvers are designed to solve the Lawler's QAP, which is the most general form of the problem.
+
+.. note::
+
+    There are also many real-world problems being formulated as the so-called Koopmans-Beckmann's QAP:
+
+    .. math::
+
+        &\max_{\mathbf{X}} \ \text{tr}(\mathbf{X}^\top\mathbf{F}_1\mathbf{X}\mathbf{F}_2)+\text{tr}(\mathbf{K}_p^\top\mathbf{X})\\
+        s.t. \quad &\mathbf{X} \in \{0, 1\}^{n_1\times n_2}, \ \mathbf{X}\mathbf{1} = \mathbf{1}, \ \mathbf{X}^\top\mathbf{1} \leq \mathbf{1}
+
+    Its connection to Lawler's QAP is :math:`\mathbf{K} = \mathbf{F}_2\otimes\mathbf{F}_1^\top + \text{diag}(\mathbf{K}_p)`,
+    where :math:`\otimes` means Kronecker product.
+
 """
 
 # Copyright (c) 2022 Thinklab@SJTU
 # pygmtools is licensed under Mulan PSL v2.
 # You can use this software according to the terms and conditions of the Mulan PSL v2.
 # You may obtain a copy of Mulan PSL v2 at:
 # http://license.coscl.org.cn/MulanPSL2
@@ -367,18 +382,18 @@
     """
     if backend is None:
         backend = pygmtools.BACKEND
     _check_data_type(K, 'K', backend)
     if _check_shape(K, 2, backend):
         K = _unsqueeze(K, 0, backend)
         non_batched_input = True
-        if type(n1) is int and n1max is None:
+        if isinstance(n1, (int, np.integer)) and n1max is None:
             n1max = n1
             n1 = None
-        if type(n2) is int and n2max is None:
+        if isinstance(n2, (int, np.integer)) and n2max is None:
             n2max = n2
             n2 = None
     elif _check_shape(K, 3, backend):
         non_batched_input = False
     else:
         raise ValueError(f'the input argument K is expected to be 2-dimensional or 3-dimensional, got '
                          f'K:{len(_get_shape(K, backend))}dims!')
@@ -723,18 +738,18 @@
     """
     if backend is None:
         backend = pygmtools.BACKEND
     _check_data_type(K, 'K', backend)
     if _check_shape(K, 2, backend):
         K = _unsqueeze(K, 0, backend)
         non_batched_input = True
-        if type(n1) is int and n1max is None:
+        if isinstance(n1, (int, np.integer)) and n1max is None:
             n1max = n1
             n1 = None
-        if type(n2) is int and n2max is None:
+        if isinstance(n2, (int, np.integer)) and n2max is None:
             n2max = n2
             n2 = None
     elif _check_shape(K, 3, backend):
         non_batched_input = False
     else:
         raise ValueError(f'the input argument K is expected to be 2-dimensional or 3-dimensional, got '
                          f'K:{len(_get_shape(K, backend))}dims!')
@@ -1030,18 +1045,18 @@
     """
     if backend is None:
         backend = pygmtools.BACKEND
     _check_data_type(K, 'K', backend)
     if _check_shape(K, 2, backend):
         K = _unsqueeze(K, 0, backend)
         non_batched_input = True
-        if type(n1) is int and n1max is None:
+        if isinstance(n1, (int, np.integer)) and n1max is None:
             n1max = n1
             n1 = None
-        if type(n2) is int and n2max is None:
+        if isinstance(n2, (int, np.integer)) and n2max is None:
             n2max = n2
             n2 = None
     elif _check_shape(K, 3, backend):
         non_batched_input = False
     else:
         raise ValueError(f'the input argument K is expected to be 2-dimensional or 3-dimensional, got '
                          f'K:{len(_get_shape(K, backend))}dims!')
@@ -1161,18 +1176,18 @@
     """
     if backend is None:
         backend = pygmtools.BACKEND
     _check_data_type(K, 'K', backend)
     if _check_shape(K, 2, backend):
         K = _unsqueeze(K, 0, backend)
         non_batched_input = True
-        if type(n1) is int and n1max is None:
+        if isinstance(n1, (int, np.integer)) and n1max is None:
             n1max = n1
             n1 = None
-        if type(n2) is int and n2max is None:
+        if isinstance(n2, (int, np.integer)) and n2max is None:
             n2max = n2
             n2 = None
     elif _check_shape(K, 3, backend):
         non_batched_input = False
     else:
         raise ValueError(f'the input argument K is expected to be 2-dimensional or 3-dimensional, got '
                          f'K:{len(_get_shape(K, backend))}dims!')
```

### Comparing `pygmtools-0.5.1/pygmtools/dataset.py` & `pygmtools-0.5.2/pygmtools/dataset.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.1/pygmtools/dataset_config.py` & `pygmtools-0.5.2/pygmtools/dataset_config.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.1/pygmtools/jittor_backend.py` & `pygmtools-0.5.2/pygmtools/jittor_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,37 +279,45 @@
          max_iter) -> Var:
     """
     Jittor implementation of IPFP algorithm
     """
     batch_num, n1, n2, n1max, n2max, n1n2, v0 = _check_and_init_gm(K, n1, n2, n1max, n2max, x0)
     v = v0
     last_v = v
+    best_v = v
+    best_obj = jt.full((batch_num, 1, 1), -1)
 
     def comp_obj_score(v1, K, v2):
         return jt.bmm(jt.bmm(v1.view(batch_num, 1, -1), K), v2)
 
     for i in range(max_iter):
         cost = jt.bmm(K, v).reshape((batch_num, int(n2max), int(n1max))).transpose(1, 2)
         binary_sol = hungarian(cost, n1, n2)
         binary_v = binary_sol.transpose(1, 2).view(batch_num, -1, 1)
         alpha = comp_obj_score(v, K, binary_v - v)
         beta = comp_obj_score(binary_v - v, K, binary_v - v)
-        t0 = alpha / beta
-        cond = jt.logical_or(beta <= 0, t0 >= 1)
+        t0 = - alpha / beta
+        cond = jt.logical_or(beta >= 0, t0 >= 1)
         if cond.shape != binary_v.shape:
             cond = cond.expand(binary_v.shape)
         v = jt.where(cond, binary_v, v + t0 * (binary_v - v))
-        last_v_sol = comp_obj_score(last_v, K, last_v)
-        if jt.max(jt.abs(
-                last_v_sol - jt.bmm(cost.reshape(batch_num, 1, -1), binary_sol.reshape(batch_num, -1, 1))
-        ) / last_v_sol) < 1e-3:
+        last_v_obj = comp_obj_score(last_v, K, last_v)
+
+        current_obj = comp_obj_score(binary_v, K, binary_v)
+        cond = current_obj > best_obj
+        if cond.shape != binary_v.shape:
+            cond = cond.expand(binary_v.shape)
+        best_v = jt.where(cond, binary_v, best_v)  # current_obj > best_obj
+        best_obj = jt.where(current_obj > best_obj, current_obj, best_obj)
+
+        if jt.max(jt.abs(last_v_obj - current_obj) / last_v_obj) < 1e-3:
             break
         last_v = v
 
-    pred_x = binary_sol
+    pred_x = best_v.reshape((batch_num, int(n2max), int(n1max))).transpose(1, 2)
     return pred_x
 
 
 ############################################
 #      Multi-Graph Matching Solvers        #
 ############################################
```

### Comparing `pygmtools-0.5.1/pygmtools/jittor_modules.py` & `pygmtools-0.5.2/pygmtools/jittor_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.1/pygmtools/linear_solvers.py` & `pygmtools-0.5.2/pygmtools/linear_solvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -725,16 +725,16 @@
             }
     """
     if backend is None:
         backend = pygmtools.BACKEND
     _check_data_type(s, 's', backend)
     if _check_shape(s, 2, backend):
         s = _unsqueeze(s, 0, backend)
-        if type(n1) is int: n1 = from_numpy(np.array([n1]), backend=backend)
-        if type(n2) is int: n2 = from_numpy(np.array([n2]), backend=backend)
+        if isinstance(n1, (int, np.integer)): n1 = from_numpy(np.array([n1]), backend=backend)
+        if isinstance(n2, (int, np.integer)): n2 = from_numpy(np.array([n2]), backend=backend)
         non_batched_input = True
     elif _check_shape(s, 3, backend):
         non_batched_input = False
     else:
         raise ValueError(f'the input argument s is expected to be 2-dimensional or 3-dimensional, got '
                          f's:{len(_get_shape(s, backend))}dims!')
     if n1 is not None: _check_data_type(n1, 'n1', backend)
@@ -1294,16 +1294,16 @@
 
     """
     if backend is None:
         backend = pygmtools.BACKEND
     _check_data_type(s, backend)
     if _check_shape(s, 2, backend):
         s = _unsqueeze(s, 0, backend)
-        if type(n1) is int: n1 = from_numpy(np.array([n1]), backend=backend)
-        if type(n2) is int: n2 = from_numpy(np.array([n2]), backend=backend)
+        if isinstance(n1, (int, np.integer)): n1 = from_numpy(np.array([n1]), backend=backend)
+        if isinstance(n2, (int, np.integer)): n2 = from_numpy(np.array([n2]), backend=backend)
         non_batched_input = True
     elif _check_shape(s, 3, backend):
         non_batched_input = False
     else:
         raise ValueError(f'the input argument s is expected to be 2-dimensional or 3-dimensional, got '
                          f's:{len(_get_shape(s, backend))}dims!')
     if unmatch1 is not None and unmatch2 is not None:
```

### Comparing `pygmtools-0.5.1/pygmtools/mindspore_backend.py` & `pygmtools-0.5.2/pygmtools/mindspore_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,35 +276,39 @@
          max_iter) -> mindspore.Tensor:
     """
     mindspore implementation of IPFP algorithm
     """
     batch_num, n1, n2, n1max, n2max, n1n2, v0 = _check_and_init_gm(K, n1, n2, n1max, n2max, x0)
     v = v0
     last_v = v
+    best_v = v
+    best_obj = -1
 
     def comp_obj_score(v1, K, v2):
         return mindspore.ops.BatchMatMul()(mindspore.ops.BatchMatMul()(v1.view(batch_num, 1, -1), K), v2)
 
     for i in range(max_iter):
         cost = mindspore.ops.BatchMatMul()(K, v).reshape(batch_num, int(n2max), int(n1max)).swapaxes(1, 2)
         binary_sol = hungarian(cost, n1, n2)
         binary_v = binary_sol.swapaxes(1, 2).view(batch_num, -1, 1)
-        alpha = comp_obj_score(v, K, binary_v - v)  # + torch.mm(k_diag.view(1, -1), (binary_sol - v).view(-1, 1))
+        alpha = comp_obj_score(v, K, binary_v - v)
         beta = comp_obj_score(binary_v - v, K, binary_v - v)
-        t0 = alpha / beta
-        v = mindspore.numpy.where(mindspore.ops.logical_or(beta <= 0, t0 >= 1), binary_v, v + t0 * (binary_v - v))
-        last_v_sol = comp_obj_score(last_v, K, last_v)
-        if (mindspore.ops.max(mindspore.ops.abs(
-                last_v_sol - mindspore.ops.BatchMatMul()(cost.reshape((batch_num, 1, -1)),
-                                                         binary_sol.reshape((batch_num, -1, 1)))
-        ) / last_v_sol)[1] < 1e-3).any():
+        t0 = - alpha / beta
+        v = mindspore.numpy.where(mindspore.ops.logical_or(beta >= 0, t0 >= 1), binary_v, v + t0 * (binary_v - v))
+        last_v_obj = comp_obj_score(last_v, K, last_v)
+
+        current_obj = comp_obj_score(binary_v, K, binary_v)
+        best_v = mindspore.numpy.where(current_obj > best_obj, binary_v, best_v)
+        best_obj = mindspore.numpy.where(current_obj > best_obj, current_obj, best_obj)
+
+        if (mindspore.ops.max(mindspore.ops.abs(last_v_obj - current_obj) / last_v_obj)[1] < 1e-3).any():
             break
         last_v = v
 
-    pred_x = binary_sol
+    pred_x = best_v.reshape(batch_num, int(n2max), int(n1max)).swapaxes(1, 2)
     return pred_x
 
 
 def _check_and_init_gm(K, n1, n2, n1max, n2max, x0):
     # get batch number
     batch_num = K.shape[0]
     n1n2 = K.shape[1]
```

### Comparing `pygmtools-0.5.1/pygmtools/multi_graph_solvers.py` & `pygmtools-0.5.2/pygmtools/multi_graph_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.1/pygmtools/neural_solvers.py` & `pygmtools-0.5.2/pygmtools/neural_solvers.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,16 +281,16 @@
     non_batched_input = False
     if feat1 is not None: # if feat1 is None, this function skips the forward pass and only returns a network object
         for var, name in ((feat1, 'feat1'), (feat2, 'feat2'), (A1, 'A1'), (A2, 'A2')):
             _check_data_type(var, name, backend)
 
         if all([_check_shape(_, 2, backend) for _ in (feat1, feat2, A1, A2)]):
             feat1, feat2, A1, A2 = [_unsqueeze(_, 0, backend) for _ in (feat1, feat2, A1, A2)]
-            if type(n1) is int: n1 = from_numpy(np.array([n1]), backend=backend)
-            if type(n2) is int: n2 = from_numpy(np.array([n2]), backend=backend)
+            if isinstance(n1, (int, np.integer)): n1 = from_numpy(np.array([n1]), backend=backend)
+            if isinstance(n2, (int, np.integer)): n2 = from_numpy(np.array([n2]), backend=backend)
             non_batched_input = True
         elif all([_check_shape(_, 3, backend) for _ in (feat1, feat2, A1, A2)]):
             non_batched_input = False
         else:
             raise ValueError(
                 f'the input arguments feat1, feat2, A1, A2 are expected to be all 2-dimensional or 3-dimensional, got '
                 f'feat1:{len(_get_shape(feat1, backend))}dims, feat2:{len(_get_shape(feat2, backend))}dims, '
@@ -588,16 +588,16 @@
     non_batched_input = False
     if feat1 is not None:  # if feat1 is None, this function skips the forward pass and only returns a network object
         for var, name in ((feat1, 'feat1'), (feat2, 'feat2'), (A1, 'A1'), (A2, 'A2')):
             _check_data_type(var, name, backend)
 
         if all([_check_shape(_, 2, backend) for _ in (feat1, feat2, A1, A2)]):
             feat1, feat2, A1, A2 = [_unsqueeze(_, 0, backend) for _ in (feat1, feat2, A1, A2)]
-            if type(n1) is int: n1 = from_numpy(np.array([n1]), backend=backend)
-            if type(n2) is int: n2 = from_numpy(np.array([n2]), backend=backend)
+            if isinstance(n1, (int, np.integer)): n1 = from_numpy(np.array([n1]), backend=backend)
+            if isinstance(n2, (int, np.integer)): n2 = from_numpy(np.array([n2]), backend=backend)
             non_batched_input = True
         elif all([_check_shape(_, 3, backend) for _ in (feat1, feat2, A1, A2)]):
             non_batched_input = False
         else:
             raise ValueError(
                 f'the input arguments feat1, feat2, A1, A2 are expected to be all 2-dimensional or 3-dimensional, got '
                 f'feat1:{len(_get_shape(feat1, backend))}dims, feat2:{len(_get_shape(feat2, backend))}dims, '
@@ -909,16 +909,16 @@
                           (feat_edge1, 'feat_edge1'), (feat_edge2, 'feat_edge2')):
             _check_data_type(var, name, backend)
 
         if all([_check_shape(_, 2, backend) for _ in (feat_node1, feat_node2, A1, A2)]) \
                 and all([_check_shape(_, 3, backend) for _ in (feat_edge1, feat_edge2)]):
             feat_node1, feat_node2, A1, A2, feat_edge1, feat_edge2 =\
                 [_unsqueeze(_, 0, backend) for _ in (feat_node1, feat_node2, A1, A2, feat_edge1, feat_edge2)]
-            if type(n1) is int: n1 = from_numpy(np.array([n1]), backend=backend)
-            if type(n2) is int: n2 = from_numpy(np.array([n2]), backend=backend)
+            if isinstance(n1, (int, np.integer)): n1 = from_numpy(np.array([n1]), backend=backend)
+            if isinstance(n2, (int, np.integer)): n2 = from_numpy(np.array([n2]), backend=backend)
             non_batched_input = True
         elif all([_check_shape(_, 3, backend) for _ in (feat_node1, feat_node2, A1, A2)]) \
                 and all([_check_shape(_, 4, backend) for _ in (feat_edge1, feat_edge2)]):
             non_batched_input = False
         else:
             raise ValueError(
                 f'the dimensions of the input arguments are illegal. Got '
@@ -1235,18 +1235,18 @@
         backend = pygmtools.BACKEND
     non_batched_input = False
     if K is not None: # if K is None, this function skips the forward pass and only returns a network object
         _check_data_type(K, 'K', backend)
         if _check_shape(K, 2, backend):
             K = _unsqueeze(K, 0, backend)
             non_batched_input = True
-            if type(n1) is int and n1max is None:
+            if isinstance(n1, (int, np.integer)) and n1max is None:
                 n1max = n1
                 n1 = None
-            if type(n2) is int and n2max is None:
+            if isinstance(n2, (int, np.integer)) and n2max is None:
                 n2max = n2
                 n2 = None
         elif _check_shape(K, 3, backend):
             non_batched_input = False
         else:
             raise ValueError(f'the input argument K is expected to be 2-dimensional or 3-dimensional, got '
                              f'K:{len(_get_shape(K, backend))}dims!')
@@ -1440,16 +1440,16 @@
     non_batched_input = False
     if feat1 is not None: # if feat1 is None, this function skips the forward pass and only returns a network object
         for var, name in ((feat1, 'feat1'), (feat2, 'feat2'), (A1, 'A1'), (A2, 'A2')):
             _check_data_type(var, name, backend)
 
         if all([_check_shape(_, 2, backend) for _ in (feat1, feat2, A1, A2)]):
             feat1, feat2, A1, A2 = [_unsqueeze(_, 0, backend) for _ in (feat1, feat2, A1, A2)]
-            if type(n1) is int: n1 = from_numpy(np.array([n1]), backend=backend)
-            if type(n2) is int: n2 = from_numpy(np.array([n2]), backend=backend)
+            if isinstance(n1, (int, np.integer)): n1 = from_numpy(np.array([n1]), backend=backend)
+            if isinstance(n2, (int, np.integer)): n2 = from_numpy(np.array([n2]), backend=backend)
             non_batched_input = True
         elif all([_check_shape(_, 3, backend) for _ in (feat1, feat2, A1, A2)]):
             non_batched_input = False
         else:
             raise ValueError(
                 f'the input arguments feat1, feat2, A1, A2 are expected to be all 2-dimensional or 3-dimensional, got '
                 f'feat1:{len(_get_shape(feat1, backend))}dims, feat2:{len(_get_shape(feat2, backend))}dims, '
```

### Comparing `pygmtools-0.5.1/pygmtools/numpy_backend.py` & `pygmtools-0.5.2/pygmtools/numpy_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,34 +289,39 @@
          max_iter) -> np.ndarray:
     """
     numpy implementation of IPFP algorithm
     """
     batch_num, n1, n2, n1max, n2max, n1n2, v0 = _check_and_init_gm(K, n1, n2, n1max, n2max, x0)
     v = v0
     last_v = v
+    best_v = v
+    best_obj = -1
 
     def comp_obj_score(v1, K, v2):
         return np.matmul(np.matmul(v1.reshape((batch_num, 1, -1)), K), v2)
 
     for i in range(max_iter):
         cost = np.matmul(K, v).reshape((batch_num, n2max, n1max)).transpose((0, 2, 1))
         binary_sol = hungarian(cost, n1, n2)
         binary_v = binary_sol.transpose((0, 2, 1)).reshape((batch_num, -1, 1))
         alpha = comp_obj_score(v, K, binary_v - v)
         beta = comp_obj_score(binary_v - v, K, binary_v - v)
-        t0 = alpha / beta
-        v = np.where(np.logical_or(beta <= 0, t0 >= 1), binary_v, v + t0 * (binary_v - v))
-        last_v_sol = comp_obj_score(last_v, K, last_v)
-        if np.max(np.abs(
-                last_v_sol - np.matmul(cost.reshape((batch_num, 1, -1)), binary_sol.reshape((batch_num, -1, 1)))
-        ) / last_v_sol) < 1e-3:
+        t0 = - alpha / beta
+        v = np.where(np.logical_or(beta >= 0, t0 >= 1), binary_v, v + t0 * (binary_v - v))
+        last_v_obj = comp_obj_score(last_v, K, last_v)
+
+        current_obj = comp_obj_score(binary_v, K, binary_v)
+        best_v = np.where(current_obj > best_obj, binary_v, best_v)
+        best_obj = np.where(current_obj > best_obj, current_obj, best_obj)
+
+        if np.max(np.abs(last_v_obj - current_obj) / last_v_obj) < 1e-3:
             break
         last_v = v
 
-    pred_x = binary_sol
+    pred_x = best_v.reshape((batch_num, n2max, n1max)).transpose((0, 2, 1))
     return pred_x
 
 
 def _check_and_init_gm(K, n1, n2, n1max, n2max, x0):
     # get batch number
     batch_num = K.shape[0]
     n1n2 = K.shape[1]
```

### Comparing `pygmtools-0.5.1/pygmtools/numpy_modules.py` & `pygmtools-0.5.2/pygmtools/numpy_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.1/pygmtools/paddle_backend.py` & `pygmtools-0.5.2/pygmtools/paddle_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,34 +271,39 @@
          max_iter) -> paddle.Tensor:
     """
     Paddle implementation of IPFP algorithm
     """
     batch_num, n1, n2, n1max, n2max, n1n2, v0 = _check_and_init_gm(K, n1, n2, n1max, n2max, x0)
     v = v0
     last_v = v
+    best_v = v
+    best_obj = paddle.to_tensor(paddle.full((batch_num, 1, 1), -1.), place=K.place)
 
     def comp_obj_score(v1, K, v2):
         return paddle.bmm(paddle.bmm(paddle.reshape(v1, (batch_num, 1, -1)), K), v2)
 
     for i in range(max_iter):
         cost = paddle.reshape(paddle.bmm(K, v),(batch_num, n2max, n1max)).transpose((0, 2, 1))
         binary_sol = hungarian(cost, n1, n2)
         binary_v = paddle.reshape(binary_sol.transpose((0, 2, 1)),(batch_num, -1, 1))
         alpha = comp_obj_score(v, K, binary_v - v)
         beta = comp_obj_score(binary_v - v, K, binary_v - v)
-        t0 = alpha / beta
-        v = paddle.where(paddle.logical_or(beta <= 0, t0 >= 1), binary_v, v + t0 * (binary_v - v))
-        last_v_sol = comp_obj_score(last_v, K, last_v)
-        if paddle.max(paddle.abs(
-                last_v_sol - paddle.bmm(paddle.reshape(cost,(batch_num, 1, -1)), paddle.reshape(binary_sol, (batch_num, -1, 1)))
-        ) / last_v_sol) < 1e-3:
+        t0 = - alpha / beta
+        v = paddle.where(paddle.logical_or(beta >= 0, t0 >= 1), binary_v, v + t0 * (binary_v - v))
+        last_v_obj = comp_obj_score(last_v, K, last_v)
+
+        current_obj = comp_obj_score(binary_v, K, binary_v)
+        best_v = paddle.where(current_obj > best_obj, binary_v, best_v)
+        best_obj = paddle.where(current_obj > best_obj, current_obj, best_obj)
+
+        if paddle.max(paddle.abs(last_v_obj - current_obj) / last_v_obj) < 1e-3:
             break
         last_v = v
 
-    pred_x = binary_sol
+    pred_x = paddle.reshape(best_v, (batch_num, n2max, n1max)).transpose((0, 2, 1))
     return pred_x
 
 
 def _check_and_init_gm(K, n1, n2, n1max, n2max, x0):
     # get batch number
     batch_num = K.shape[0]
     n1n2 = K.shape[1]
```

### Comparing `pygmtools-0.5.1/pygmtools/paddle_modules.py` & `pygmtools-0.5.2/pygmtools/paddle_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.1/pygmtools/pytorch_astar_modules.py` & `pygmtools-0.5.2/pygmtools/pytorch_astar_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.1/pygmtools/pytorch_backend.py` & `pygmtools-0.5.2/pygmtools/pytorch_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,34 +278,39 @@
          max_iter) -> Tensor:
     """
     Pytorch implementation of IPFP algorithm
     """
     batch_num, n1, n2, n1max, n2max, n1n2, v0 = _check_and_init_gm(K, n1, n2, n1max, n2max, x0)
     v = v0
     last_v = v
+    best_v = v
+    best_obj = -1
 
     def comp_obj_score(v1, K, v2):
         return torch.bmm(torch.bmm(v1.view(batch_num, 1, -1), K), v2)
 
     for i in range(max_iter):
         cost = torch.bmm(K, v).reshape(batch_num, n2max, n1max).transpose(1, 2)
         binary_sol = hungarian(cost, n1, n2)
         binary_v = binary_sol.transpose(1, 2).view(batch_num, -1, 1)
-        alpha = comp_obj_score(v, K, binary_v - v)  # + torch.mm(k_diag.view(1, -1), (binary_sol - v).view(-1, 1))
+        alpha = comp_obj_score(v, K, binary_v - v)
         beta = comp_obj_score(binary_v - v, K, binary_v - v)
-        t0 = alpha / beta
-        v = torch.where(torch.logical_or(beta <= 0, t0 >= 1), binary_v, v + t0 * (binary_v - v))
-        last_v_sol = comp_obj_score(last_v, K, last_v)
-        if torch.max(torch.abs(
-                last_v_sol - torch.bmm(cost.reshape(batch_num, 1, -1), binary_sol.reshape(batch_num, -1, 1))
-        ) / last_v_sol) < 1e-3:
+        t0 = - alpha / beta
+        v = torch.where(torch.logical_or(beta >= 0, t0 >= 1), binary_v, v + t0 * (binary_v - v))
+        last_v_obj = comp_obj_score(last_v, K, last_v)
+
+        current_obj = comp_obj_score(binary_v, K, binary_v)
+        best_v = torch.where(current_obj > best_obj, binary_v, best_v)
+        best_obj = torch.where(current_obj > best_obj, current_obj, best_obj)
+
+        if torch.max(torch.abs(last_v_obj - current_obj) / last_v_obj) < 1e-3:
             break
         last_v = v
 
-    pred_x = binary_sol
+    pred_x = best_v.reshape(batch_num, n2max, n1max).transpose(1, 2)
     return pred_x
 
 
 def astar(K, n1, n2, n1max, n2max, beam_width):
     """
     Pytorch implementation of ASTAR algorithm (for solving QAP)
     """
```

### Comparing `pygmtools-0.5.1/pygmtools/pytorch_modules.py` & `pygmtools-0.5.2/pygmtools/pytorch_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.1/pygmtools/tensorflow_backend.py` & `pygmtools-0.5.2/pygmtools/tensorflow_backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -227,15 +227,15 @@
 #    Quadratic Assignment Problem Solvers   #
 #############################################
 
 
 def rrwm(K: tf.Tensor, n1: tf.Tensor, n2: tf.Tensor, n1max, n2max, x0: tf.Tensor,
          max_iter: int, sk_iter: int, alpha: float, beta: float) -> tf.Tensor:
     """
-    Pytorch implementation of RRWM algorithm.
+    Tensorflow implementation of RRWM algorithm.
     """
     batch_num, n1, n2, n1max, n2max, n1n2, v0 = _check_and_init_gm(K, n1, n2, n1max, n2max, x0)
     # rescale the values in K
     d = tf.reduce_sum(K, axis=2, keepdims=True)
     dmax = tf.reduce_max(d, axis=1, keepdims=True)
     K = K / (dmax + tf.reduce_min(d) * 1e-5)
     v = v0
@@ -279,39 +279,44 @@
 
     x = tf.transpose(tf.reshape(v, [batch_num, n2max, n1max]), [0, 2, 1])
     return x
 
 def ipfp(K: tf.Tensor, n1: tf.Tensor, n2: tf.Tensor, n1max, n2max, x0: tf.Tensor,
          max_iter) -> tf.Tensor:
     """
-    Pytorch implementation of IPFP algorithm
+    Tensorflow implementation of IPFP algorithm
     """
     batch_num, n1, n2, n1max, n2max, n1n2, v0 = _check_and_init_gm(K, n1, n2, n1max, n2max, x0)
     v = v0
     last_v = v
+    best_v = v
+    best_obj = -1
 
     def comp_obj_score(v1, K, v2):
         return tf.matmul(tf.matmul(tf.reshape(v1, [batch_num, 1, -1]), K), v2)
 
     for i in range(max_iter):
         cost = tf.transpose(tf.reshape(tf.matmul(K, v), [batch_num, n2max, n1max]), [0, 2, 1])
         binary_sol = hungarian(cost, n1, n2)
         binary_v = tf.reshape(tf.transpose(binary_sol, [0, 2, 1]), [batch_num, -1, 1])
-        alpha = comp_obj_score(v, K, binary_v - v)  # + torch.mm(k_diag.view(1, -1), (binary_sol - v).view(-1, 1))
+        alpha = comp_obj_score(v, K, binary_v - v)
         beta = comp_obj_score(binary_v - v, K, binary_v - v)
-        t0 = alpha / beta
-        v = tf.where(tf.math.logical_or(beta <= 0, t0 >= 1), binary_v, v + t0 * (binary_v - v))
-        last_v_sol = comp_obj_score(last_v, K, last_v)
-        if tf.reduce_max(tf.abs(
-                last_v_sol - tf.matmul(tf.reshape(cost, [batch_num, 1, -1]), tf.reshape(binary_sol, [batch_num, -1, 1]))
-        ) / last_v_sol) < 1e-3:
+        t0 = - alpha / beta
+        v = tf.where(tf.math.logical_or(beta >= 0, t0 >= 1), binary_v, v + t0 * (binary_v - v))
+        last_v_obj = comp_obj_score(last_v, K, last_v)
+
+        current_obj = comp_obj_score(binary_v, K, binary_v)
+        best_v = tf.where(current_obj > best_obj, binary_v, best_v)
+        best_obj = tf.where(current_obj > best_obj, current_obj, best_obj)
+
+        if tf.reduce_max(tf.abs(last_v_obj - current_obj) / last_v_obj) < 1e-3:
             break
         last_v = v
 
-    pred_x = binary_sol
+    pred_x = tf.transpose(tf.reshape(best_v, [batch_num, n2max, n1max]), [0, 2, 1])
     return pred_x
 
 
 def _check_and_init_gm(K, n1, n2, n1max, n2max, x0):
     # get batch number
     batch_num = K.shape[0]
     n1n2 = K.shape[1]
```

### Comparing `pygmtools-0.5.1/pygmtools/utils.py` & `pygmtools-0.5.2/pygmtools/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,18 +32,18 @@
 import requests
 from appdirs import user_cache_dir
 from tqdm.auto import tqdm
 
 import pygmtools
 
 NOT_IMPLEMENTED_MSG = \
-    'The backend function for {} is not implemented.\n' \
-    'If you are a user, this error message means the function you are calling is not available with this backend and ' \
-    'please use other backends as workarounds. Scroll up in the call stack and it will tell you which function is ' \
-    'causing this error.\n' \
+    'Import failed! It is likely that the backend function for {} is not implemented, OR the backend is not installed ' \
+    'correctly. Please Scroll up in the call stack and it will tell you who is causing this error.\n' \
+    'If you are a user, this error message usually means the function you are calling is not available with this backend ' \
+    'and please use other backends as workarounds. \n' \
     'If you are a developer, it will be truly appreciated if you could develop and share your ' \
     'implementation with the community! RP is welcomed via Github: https://github.com/Thinklab-SJTU/pygmtools'
 
 
 _BACKEND_MAP = {
     'numpy': 'numpy',
     'pytorch': 'torch',
```

### Comparing `pygmtools-0.5.1/pygmtools.egg-info/PKG-INFO` & `pygmtools-0.5.2/pygmtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtools
-Version: 0.5.1
+Version: 0.5.2
 Summary: pygmtools provides graph matching solvers in Python API and supports numpy and pytorch backends. pygmtools also provides dataset API for standard graph matching benchmarks.
 Home-page: https://pygmtools.readthedocs.io/
 Author: ThinkLab at SJTU
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pygmtools-0.5.1/pygmtools.egg-info/SOURCES.txt` & `pygmtools-0.5.2/pygmtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.1/setup.py` & `pygmtools-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.1/tests/test_classic_solvers.py` & `pygmtools-0.5.2/tests/test_classic_solvers.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             else:
                 _n1, _n2 = n1.item(), n2.item()
                 _conn1, _edge1 = pygm.utils.dense_to_sparse(_A1)
                 _conn2, _edge2 = pygm.utils.dense_to_sparse(_A2)
                 _K = pygm.utils.build_aff_mat(_F1, _edge1, _conn1, _F2, _edge2, _conn2, _n1, None, _n2, None,
                                               **aff_param_dict)
             if last_K is not None:
-                assert np.abs(pygm.utils.to_numpy(_K) - last_K).sum() < 0.1, \
+                assert np.abs(pygm.utils.to_numpy(_K) - last_K).max() < 0.01, \
                     f"Incorrect affinity matrix for {working_backend}, " \
                     f"params: {';'.join([k + '=' + str(v) for k, v in aff_param_dict.items()])};" \
                     f"{';'.join([k + '=' + str(v) for k, v in solver_param_dict.items()])}"
             last_K = pygm.utils.to_numpy(_K)
             _X = solver_func(_K, _n1, _n2, **solver_param_dict)
             if last_X is not None:
                 assert np.abs(pygm.utils.to_numpy(_X) - last_X).sum() < 1e-4, \
```

### Comparing `pygmtools-0.5.1/tests/test_dataset.py` & `pygmtools-0.5.2/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.1/tests/test_misc.py` & `pygmtools-0.5.2/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.1/tests/test_multi_graph_solvers.py` & `pygmtools-0.5.2/tests/test_multi_graph_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.1/tests/test_neural_solvers.py` & `pygmtools-0.5.2/tests/test_neural_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.1/tests/test_utils.py` & `pygmtools-0.5.2/tests/test_utils.py`

 * *Files identical despite different names*

