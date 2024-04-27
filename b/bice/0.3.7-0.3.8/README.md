# Comparing `tmp/bice-0.3.7.tar.gz` & `tmp/bice-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bice-0.3.7.tar", last modified: Mon Apr 18 22:39:25 2022, max compression
+gzip compressed data, was "bice-0.3.8.tar", last modified: Sat Apr 27 19:37:25 2024, max compression
```

## Comparing `bice-0.3.7.tar` & `bice-0.3.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2022-04-18 22:39:25.068682 bice-0.3.7/
--rw-rw-r--   0 simon     (1000) simon     (1000)     1071 2022-04-18 15:00:21.000000 bice-0.3.7/LICENSE
--rw-rw-r--   0 simon     (1000) simon     (1000)     2314 2022-04-18 22:39:25.068682 bice-0.3.7/PKG-INFO
--rw-rw-r--   0 simon     (1000) simon     (1000)     2029 2022-04-18 15:00:21.000000 bice-0.3.7/README.md
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2022-04-18 22:39:25.064681 bice-0.3.7/bice/
--rw-rw-r--   0 simon     (1000) simon     (1000)      285 2022-04-18 17:49:21.000000 bice-0.3.7/bice/__init__.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2022-04-18 22:39:25.068682 bice-0.3.7/bice/continuation/
--rw-rw-r--   0 simon     (1000) simon     (1000)      540 2022-04-18 17:49:21.000000 bice-0.3.7/bice/continuation/__init__.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     6635 2022-04-18 22:36:29.000000 bice-0.3.7/bice/continuation/bifurcations.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     6559 2022-04-18 21:54:40.000000 bice-0.3.7/bice/continuation/constraints.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     8964 2022-04-18 22:16:10.000000 bice-0.3.7/bice/continuation/continuation_steppers.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     2409 2022-04-18 18:16:06.000000 bice-0.3.7/bice/continuation/deflation.py
--rw-rw-r--   0 simon     (1000) simon     (1000)    13424 2022-04-18 18:38:52.000000 bice-0.3.7/bice/continuation/timeperiodic.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2022-04-18 22:39:25.068682 bice-0.3.7/bice/core/
--rw-rw-r--   0 simon     (1000) simon     (1000)      500 2022-04-18 17:49:21.000000 bice-0.3.7/bice/core/__init__.py
--rw-rw-r--   0 simon     (1000) simon     (1000)    16267 2022-04-18 22:04:06.000000 bice-0.3.7/bice/core/equation.py
--rw-rw-r--   0 simon     (1000) simon     (1000)    33597 2022-04-18 22:34:02.000000 bice-0.3.7/bice/core/problem.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     6195 2022-04-18 18:40:40.000000 bice-0.3.7/bice/core/profiling.py
--rw-rw-r--   0 simon     (1000) simon     (1000)    12624 2022-04-18 18:56:51.000000 bice-0.3.7/bice/core/solution.py
--rw-rw-r--   0 simon     (1000) simon     (1000)    10312 2022-04-18 18:57:01.000000 bice-0.3.7/bice/core/solvers.py
--rw-rw-r--   0 simon     (1000) simon     (1000)      458 2022-04-18 22:36:24.000000 bice-0.3.7/bice/core/types.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2022-04-18 22:39:25.068682 bice-0.3.7/bice/measure/
--rw-rw-r--   0 simon     (1000) simon     (1000)       98 2022-04-18 17:49:21.000000 bice-0.3.7/bice/measure/__init__.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     4101 2022-04-18 22:37:10.000000 bice-0.3.7/bice/measure/lyapunov.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2022-04-18 22:39:25.068682 bice-0.3.7/bice/pde/
--rw-rw-r--   0 simon     (1000) simon     (1000)      267 2022-04-18 17:49:21.000000 bice-0.3.7/bice/pde/__init__.py
--rw-rw-r--   0 simon     (1000) simon     (1000)    19123 2022-04-18 18:43:10.000000 bice-0.3.7/bice/pde/finite_differences.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     1697 2022-04-18 18:19:25.000000 bice-0.3.7/bice/pde/pde.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     2743 2022-04-18 21:58:04.000000 bice-0.3.7/bice/pde/pseudospectral.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2022-04-18 22:39:25.068682 bice-0.3.7/bice/time_steppers/
--rw-rw-r--   0 simon     (1000) simon     (1000)      242 2022-04-18 17:49:21.000000 bice-0.3.7/bice/time_steppers/__init__.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     2435 2022-04-18 20:43:01.000000 bice-0.3.7/bice/time_steppers/bdf.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     5370 2022-04-18 22:35:23.000000 bice-0.3.7/bice/time_steppers/runge_kutta.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     1689 2022-04-18 17:49:21.000000 bice-0.3.7/bice/time_steppers/time_steppers.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2022-04-18 22:39:25.064681 bice-0.3.7/bice.egg-info/
--rw-rw-r--   0 simon     (1000) simon     (1000)     2314 2022-04-18 22:39:24.000000 bice-0.3.7/bice.egg-info/PKG-INFO
--rw-rw-r--   0 simon     (1000) simon     (1000)      855 2022-04-18 22:39:25.000000 bice-0.3.7/bice.egg-info/SOURCES.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)        1 2022-04-18 22:39:24.000000 bice-0.3.7/bice.egg-info/dependency_links.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)       44 2022-04-18 22:39:24.000000 bice-0.3.7/bice.egg-info/requires.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)       11 2022-04-18 22:39:24.000000 bice-0.3.7/bice.egg-info/top_level.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)      103 2022-04-18 22:39:25.068682 bice-0.3.7/setup.cfg
--rw-rw-r--   0 simon     (1000) simon     (1000)      671 2022-04-18 22:38:53.000000 bice-0.3.7/setup.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2022-04-18 22:39:25.068682 bice-0.3.7/tests/
--rw-rw-r--   0 simon     (1000) simon     (1000)        0 2022-04-18 15:00:21.000000 bice-0.3.7/tests/__init__.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     2894 2022-04-18 15:00:21.000000 bice-0.3.7/tests/test_she.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 19:37:25.442844 bice-0.3.8/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1071 2024-04-27 19:10:43.000000 bice-0.3.8/LICENSE
+-rw-r--r--   0 simon     (1000) simon     (1000)     2021 2024-04-27 19:37:25.442844 bice-0.3.8/PKG-INFO
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2015 2024-04-27 19:36:28.000000 bice-0.3.8/README.md
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 19:37:25.434844 bice-0.3.8/bice/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      285 2024-04-27 19:10:43.000000 bice-0.3.8/bice/__init__.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 19:37:25.438844 bice-0.3.8/bice/continuation/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      540 2024-04-27 19:10:43.000000 bice-0.3.8/bice/continuation/__init__.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     6640 2024-04-27 19:10:43.000000 bice-0.3.8/bice/continuation/bifurcations.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     6569 2024-04-27 19:10:43.000000 bice-0.3.8/bice/continuation/constraints.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     8964 2024-04-27 19:10:43.000000 bice-0.3.8/bice/continuation/continuation_steppers.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2409 2024-04-27 19:10:43.000000 bice-0.3.8/bice/continuation/deflation.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)    13424 2024-04-27 19:10:43.000000 bice-0.3.8/bice/continuation/timeperiodic.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 19:37:25.438844 bice-0.3.8/bice/core/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      500 2024-04-27 19:10:43.000000 bice-0.3.8/bice/core/__init__.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)    16267 2024-04-27 19:10:43.000000 bice-0.3.8/bice/core/equation.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)    33807 2024-04-27 19:10:43.000000 bice-0.3.8/bice/core/problem.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     6195 2024-04-27 19:10:43.000000 bice-0.3.8/bice/core/profiling.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)    12624 2024-04-27 19:10:43.000000 bice-0.3.8/bice/core/solution.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)    10312 2024-04-27 19:10:43.000000 bice-0.3.8/bice/core/solvers.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)      458 2024-04-27 19:10:43.000000 bice-0.3.8/bice/core/types.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 19:37:25.438844 bice-0.3.8/bice/measure/
+-rw-rw-r--   0 simon     (1000) simon     (1000)       98 2024-04-27 19:10:43.000000 bice-0.3.8/bice/measure/__init__.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     4101 2024-04-27 19:10:43.000000 bice-0.3.8/bice/measure/lyapunov.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 19:37:25.438844 bice-0.3.8/bice/pde/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      267 2024-04-27 19:10:43.000000 bice-0.3.8/bice/pde/__init__.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)    19123 2024-04-27 19:10:43.000000 bice-0.3.8/bice/pde/finite_differences.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1697 2024-04-27 19:10:43.000000 bice-0.3.8/bice/pde/pde.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2743 2024-04-27 19:10:43.000000 bice-0.3.8/bice/pde/pseudospectral.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 19:37:25.442844 bice-0.3.8/bice/time_steppers/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      242 2024-04-27 19:10:43.000000 bice-0.3.8/bice/time_steppers/__init__.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2435 2024-04-27 19:10:43.000000 bice-0.3.8/bice/time_steppers/bdf.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     5370 2024-04-27 19:10:43.000000 bice-0.3.8/bice/time_steppers/runge_kutta.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1689 2024-04-27 19:10:43.000000 bice-0.3.8/bice/time_steppers/time_steppers.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 19:37:25.442844 bice-0.3.8/bice.egg-info/
+-rw-r--r--   0 simon     (1000) simon     (1000)     2021 2024-04-27 19:37:25.000000 bice-0.3.8/bice.egg-info/PKG-INFO
+-rw-rw-r--   0 simon     (1000) simon     (1000)      855 2024-04-27 19:37:25.000000 bice-0.3.8/bice.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)        1 2024-04-27 19:37:25.000000 bice-0.3.8/bice.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)       44 2024-04-27 19:37:25.000000 bice-0.3.8/bice.egg-info/requires.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)       11 2024-04-27 19:37:25.000000 bice-0.3.8/bice.egg-info/top_level.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)      103 2024-04-27 19:37:25.442844 bice-0.3.8/setup.cfg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      671 2024-04-27 19:23:51.000000 bice-0.3.8/setup.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 19:37:25.442844 bice-0.3.8/tests/
+-rw-rw-r--   0 simon     (1000) simon     (1000)        0 2024-04-27 19:10:44.000000 bice-0.3.8/tests/__init__.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2894 2024-04-27 19:10:44.000000 bice-0.3.8/tests/test_she.py
```

### Comparing `bice-0.3.7/LICENSE` & `bice-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bice-0.3.7/PKG-INFO` & `bice-0.3.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 Metadata-Version: 2.1
 Name: bice
-Version: 0.3.7
+Version: 0.3.8
 Summary: Numerical continuation and bifurcation package
-Home-page: UNKNOWN
 Author: Simon Hartmann
 Author-email: s.hartmann@wwu.de
 License: MIT
-Description: # BICE
-        
-        A numerical path continuation software for algebraic equations, ODEs, and PDEs.
-        
-        Implements methods for the parameter continuation (arclength method) in the solution space of
-        a user-defined equation and provides a toolbox for the stability and bifurcation analysis.
-        
-        In addition, interfaces to various solvers and time-stepping methods are provided.
-        
-        ## Installation
-        
-        To install the latest published version from PyPI simply execute:
-        
-        ```bash
-        pip3 install bice
-        ```
-        
-        Alternatively, `bice` can be installed locally using the source code from our [git repository](https://zivgitlab.uni-muenster.de/s_hart20/bice).
-        
-        ### Requirements
-        
-        The software depends on Python 3 and the following third-party packages:
-        `numpy`, `scipy`, `matplotlib`, `findiff`, and `numdifftools`.
-        All will be installed automatically when installing `bice`.
-        
-        ## Tutorials
-        
-        We have first tutorials!
-        
-        - [Heat equation tutorial](https://zivgitlab.uni-muenster.de/s_hart20/bice/-/blob/master/demos/notebooks/heat_eq.ipynb): a simple tutorial on how to use bice to implement a first partial differential equation and perform a time simulation of it.
-        - [Swift-Hohenberg equation tutorial](https://zivgitlab.uni-muenster.de/s_hart20/bice/-/blob/master/demos/notebooks/she.ipynb): a simple tutorial on how to use bice's path continuation capabilities.
-        - [Predator-prey model tutorial](https://zivgitlab.uni-muenster.de/s_hart20/bice/-/blob/master/demos/notebooks/lve.ipynb): an introduction into the continuation of periodic orbits.
-        
-        More will follow soon.
-        
-        Meanwhile you can check out the less documented [demos](demos/).
-        
-        ## Documentation
-        
-        Click here for the
-        [online version of the documentation](https://s_hart20.zivgitlabpages.uni-muenster.de/bice/).
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: findiff
+Requires-Dist: numdifftools
+
+# BICE
+
+A numerical path continuation software for algebraic equations, ODEs, and PDEs.
+
+Implements methods for the parameter continuation (arclength method) in the solution space of
+a user-defined equation and provides a toolbox for the stability and bifurcation analysis.
+
+In addition, interfaces to various solvers and time-stepping methods are provided.
+
+## Installation
+
+To install the latest published version from PyPI simply execute:
+
+```bash
+pip3 install bice
+```
+
+Alternatively, `bice` can be installed locally using the source code from our [git repository](https://github.com/simon123h/bice).
+
+### Requirements
+
+The software depends on Python 3 and the following third-party packages:
+`numpy`, `scipy`, `matplotlib`, `findiff`, and `numdifftools`.
+All will be installed automatically when installing `bice`.
+
+## Tutorials
+
+We have first tutorials!
+
+- [Heat equation tutorial](https://github.com/simon123h/bice/-/blob/master/demos/notebooks/heat_eq.ipynb): a simple tutorial on how to use bice to implement a first partial differential equation and perform a time simulation of it.
+- [Swift-Hohenberg equation tutorial](https://github.com/simon123h/bice/-/blob/master/demos/notebooks/she.ipynb): a simple tutorial on how to use bice's path continuation capabilities.
+- [Predator-prey model tutorial](https://github.com/simon123h/bice/-/blob/master/demos/notebooks/lve.ipynb): an introduction into the continuation of periodic orbits.
+
+More will follow soon.
+
+Meanwhile you can check out the less documented [demos](demos/).
+
+## Documentation
+
+Click here for the
+[online version of the documentation](https://s_hart20.zivgitlabpages.uni-muenster.de/bice/).
```

### Comparing `bice-0.3.7/README.md` & `bice-0.3.8/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ```bash
 pip3 install bice
 ```
 
 If you instead want to install the package locally, e.g. for development purposes, you may download the latest version from this git and install it using:
 
 ```bash
-git clone https://zivgitlab.uni-muenster.de/s_hart20/bice
+git clone https://github.com/simon123h/bice
 pip3 install -e bice/
 ```
 
 in any directory of your choice. The installation is performed using `setup.py`.
 
 ### Requirements
```

### Comparing `bice-0.3.7/bice/continuation/__init__.py` & `bice-0.3.8/bice/continuation/__init__.py`

 * *Files identical despite different names*

### Comparing `bice-0.3.7/bice/continuation/bifurcations.py` & `bice-0.3.8/bice/continuation/bifurcations.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from bice.core.equation import Equation
 from bice.core.types import Array, Matrix
 
 
 class BifurcationConstraint(Equation):
     # TODO: add docstring
-    def __init__(self, phi: Array, free_parameter: Tuple[Any, str]):
+    def __init__(self, phi: np.ndarray, free_parameter: Tuple[Any, str]):
         super().__init__()
         # the constraint equation couples to some other equations of the problem
         self.is_coupled = True
         # copy and normalize the null-eigenvector phi
         phi = phi.copy() / np.linalg.norm(phi)
         #: reference to the free parameter
         self.free_parameter = free_parameter
```

### Comparing `bice-0.3.7/bice/continuation/constraints.py` & `bice-0.3.8/bice/continuation/constraints.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         self_idx = self.group.idx[self]
         eq_idx = self.group.idx[self.ref_eq]
         # optionally split only the part that is referenced by self.variable
         if self.variable is not None:
             eq_shape = self.ref_eq.shape[1:]
             var_ndofs = np.prod(eq_shape)
             start = eq_idx.start + self.variable * var_ndofs
-            eq_idx = slice(start, start + var_ndofs)
+            eq_idx = slice(int(start), int(start + var_ndofs))
         # employ the constraint equation
         if self.fixed_volume is None:
             # calculate the difference in volumes between current
             # and previous unknowns of the reference equation
             res[self_idx] = np.mean(u[eq_idx] - self.group.u[eq_idx])
         else:
             # parametric constraint: calculate the difference between current
```

### Comparing `bice-0.3.7/bice/continuation/continuation_steppers.py` & `bice-0.3.8/bice/continuation/continuation_steppers.py`

 * *Files identical despite different names*

### Comparing `bice-0.3.7/bice/continuation/deflation.py` & `bice-0.3.8/bice/continuation/deflation.py`

 * *Files identical despite different names*

### Comparing `bice-0.3.7/bice/continuation/timeperiodic.py` & `bice-0.3.8/bice/continuation/timeperiodic.py`

 * *Files identical despite different names*

### Comparing `bice-0.3.7/bice/core/equation.py` & `bice-0.3.8/bice/core/equation.py`

 * *Files identical despite different names*

### Comparing `bice-0.3.7/bice/core/problem.py` & `bice-0.3.8/bice/core/problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,15 +365,15 @@
         data = {}
         # the number of equations
         equations = self.list_equations()
         data['Problem.nequations'] = len(equations)
         # the problem's time
         data['Problem.time'] = self.time
         # store the value of the continuation parameter
-        if self.continuation_parameter is not None:
+        if self.continuation_parameter is not None and self.get_continuation_parameter() is not None:
             data['Problem.p'] = self.get_continuation_parameter()
         # The problem's unknowns won't need to be stored, since unknowns are
         # individually saved by the respective equations.
         # Fill the dict with data from each equation:
         for eq in equations:
             # obtain the equation's dict
             eq_data = eq.save()
@@ -484,14 +484,17 @@
                 eigval_ax.set_ylabel("eigenvalues")
             if eigvec_ax is not None:
                 # clear the axes
                 eigvec_ax.clear()
                 # map the eigenvectors onto the equations and plot them
                 if self.eigen_solver.latest_eigenvectors is not None:
                     ev = self.eigen_solver.latest_eigenvectors[0]
+                    # fix orientation of eigenvector
+                    sign = np.sign(ev.real.dot(self.u))
+                    ev *= sign if sign != 0 else 1
                     # backup the unknowns
                     u_old = self.u.copy()
                     # overwrite the unknowns with the eigenvalues (or their real part only)
                     if not np.iscomplexobj(self.u):
                         self.u = ev.real
                     else:
                         self.u = ev
```

### Comparing `bice-0.3.7/bice/core/profiling.py` & `bice-0.3.8/bice/core/profiling.py`

 * *Files identical despite different names*

### Comparing `bice-0.3.7/bice/core/solution.py` & `bice-0.3.8/bice/core/solution.py`

 * *Files identical despite different names*

### Comparing `bice-0.3.7/bice/core/solvers.py` & `bice-0.3.8/bice/core/solvers.py`

 * *Files identical despite different names*

### Comparing `bice-0.3.7/bice/measure/lyapunov.py` & `bice-0.3.8/bice/measure/lyapunov.py`

 * *Files identical despite different names*

### Comparing `bice-0.3.7/bice/pde/finite_differences.py` & `bice-0.3.8/bice/pde/finite_differences.py`

 * *Files identical despite different names*

### Comparing `bice-0.3.7/bice/pde/pde.py` & `bice-0.3.8/bice/pde/pde.py`

 * *Files identical despite different names*

### Comparing `bice-0.3.7/bice/pde/pseudospectral.py` & `bice-0.3.8/bice/pde/pseudospectral.py`

 * *Files identical despite different names*

### Comparing `bice-0.3.7/bice/time_steppers/bdf.py` & `bice-0.3.8/bice/time_steppers/bdf.py`

 * *Files identical despite different names*

### Comparing `bice-0.3.7/bice/time_steppers/runge_kutta.py` & `bice-0.3.8/bice/time_steppers/runge_kutta.py`

 * *Files identical despite different names*

### Comparing `bice-0.3.7/bice/time_steppers/time_steppers.py` & `bice-0.3.8/bice/time_steppers/time_steppers.py`

 * *Files identical despite different names*

### Comparing `bice-0.3.7/bice.egg-info/PKG-INFO` & `bice-0.3.8/bice.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 Metadata-Version: 2.1
 Name: bice
-Version: 0.3.7
+Version: 0.3.8
 Summary: Numerical continuation and bifurcation package
-Home-page: UNKNOWN
 Author: Simon Hartmann
 Author-email: s.hartmann@wwu.de
 License: MIT
-Description: # BICE
-        
-        A numerical path continuation software for algebraic equations, ODEs, and PDEs.
-        
-        Implements methods for the parameter continuation (arclength method) in the solution space of
-        a user-defined equation and provides a toolbox for the stability and bifurcation analysis.
-        
-        In addition, interfaces to various solvers and time-stepping methods are provided.
-        
-        ## Installation
-        
-        To install the latest published version from PyPI simply execute:
-        
-        ```bash
-        pip3 install bice
-        ```
-        
-        Alternatively, `bice` can be installed locally using the source code from our [git repository](https://zivgitlab.uni-muenster.de/s_hart20/bice).
-        
-        ### Requirements
-        
-        The software depends on Python 3 and the following third-party packages:
-        `numpy`, `scipy`, `matplotlib`, `findiff`, and `numdifftools`.
-        All will be installed automatically when installing `bice`.
-        
-        ## Tutorials
-        
-        We have first tutorials!
-        
-        - [Heat equation tutorial](https://zivgitlab.uni-muenster.de/s_hart20/bice/-/blob/master/demos/notebooks/heat_eq.ipynb): a simple tutorial on how to use bice to implement a first partial differential equation and perform a time simulation of it.
-        - [Swift-Hohenberg equation tutorial](https://zivgitlab.uni-muenster.de/s_hart20/bice/-/blob/master/demos/notebooks/she.ipynb): a simple tutorial on how to use bice's path continuation capabilities.
-        - [Predator-prey model tutorial](https://zivgitlab.uni-muenster.de/s_hart20/bice/-/blob/master/demos/notebooks/lve.ipynb): an introduction into the continuation of periodic orbits.
-        
-        More will follow soon.
-        
-        Meanwhile you can check out the less documented [demos](demos/).
-        
-        ## Documentation
-        
-        Click here for the
-        [online version of the documentation](https://s_hart20.zivgitlabpages.uni-muenster.de/bice/).
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: findiff
+Requires-Dist: numdifftools
+
+# BICE
+
+A numerical path continuation software for algebraic equations, ODEs, and PDEs.
+
+Implements methods for the parameter continuation (arclength method) in the solution space of
+a user-defined equation and provides a toolbox for the stability and bifurcation analysis.
+
+In addition, interfaces to various solvers and time-stepping methods are provided.
+
+## Installation
+
+To install the latest published version from PyPI simply execute:
+
+```bash
+pip3 install bice
+```
+
+Alternatively, `bice` can be installed locally using the source code from our [git repository](https://github.com/simon123h/bice).
+
+### Requirements
+
+The software depends on Python 3 and the following third-party packages:
+`numpy`, `scipy`, `matplotlib`, `findiff`, and `numdifftools`.
+All will be installed automatically when installing `bice`.
+
+## Tutorials
+
+We have first tutorials!
+
+- [Heat equation tutorial](https://github.com/simon123h/bice/-/blob/master/demos/notebooks/heat_eq.ipynb): a simple tutorial on how to use bice to implement a first partial differential equation and perform a time simulation of it.
+- [Swift-Hohenberg equation tutorial](https://github.com/simon123h/bice/-/blob/master/demos/notebooks/she.ipynb): a simple tutorial on how to use bice's path continuation capabilities.
+- [Predator-prey model tutorial](https://github.com/simon123h/bice/-/blob/master/demos/notebooks/lve.ipynb): an introduction into the continuation of periodic orbits.
+
+More will follow soon.
+
+Meanwhile you can check out the less documented [demos](demos/).
+
+## Documentation
+
+Click here for the
+[online version of the documentation](https://s_hart20.zivgitlabpages.uni-muenster.de/bice/).
```

### Comparing `bice-0.3.7/bice.egg-info/SOURCES.txt` & `bice-0.3.8/bice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bice-0.3.7/setup.py` & `bice-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 if description_file.is_file():
     long_description = description_file.read_text()
 else:
     long_description = ""
 
 setup(
     name="bice",
-    version="0.3.7",
+    version="0.3.8",
     description="Numerical continuation and bifurcation package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Simon Hartmann",
     author_email="s.hartmann@wwu.de",
     license="MIT",
     packages=find_packages(),
```

### Comparing `bice-0.3.7/tests/test_she.py` & `bice-0.3.8/tests/test_she.py`

 * *Files identical despite different names*

