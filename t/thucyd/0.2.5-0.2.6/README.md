# Comparing `tmp/thucyd-0.2.5.tar.gz` & `tmp/thucyd-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thucyd-0.2.5.tar", last modified: Sat Jan 27 23:05:02 2024, max compression
+gzip compressed data, was "thucyd-0.2.6.tar", last modified: Sat Apr 27 20:12:33 2024, max compression
```

## Comparing `thucyd-0.2.5.tar` & `thucyd-0.2.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jaydamask   (501) staff       (20)        0 2024-01-27 23:05:02.502647 thucyd-0.2.5/
--rw-------   0 jaydamask   (501) staff       (20)    11372 2019-06-17 15:13:10.000000 thucyd-0.2.5/LICENSE
--rw-r--r--   0 jaydamask   (501) staff       (20)      114 2023-12-28 23:36:11.000000 thucyd-0.2.5/MANIFEST.in
--rw-r--r--   0 jaydamask   (501) staff       (20)     4226 2024-01-27 23:05:02.502259 thucyd-0.2.5/PKG-INFO
--rw-r--r--   0 jaydamask   (501) staff       (20)     3060 2024-01-02 22:30:37.000000 thucyd-0.2.5/README.md
--rw-r--r--   0 jaydamask   (501) staff       (20)      863 2024-01-27 22:27:16.000000 thucyd-0.2.5/pyproject.toml
--rw-r--r--   0 jaydamask   (501) staff       (20)       38 2024-01-27 23:05:02.502741 thucyd-0.2.5/setup.cfg
--rw-r--r--   0 jaydamask   (501) staff       (20)     2310 2024-01-27 22:27:16.000000 thucyd-0.2.5/setup.py
-drwxr-xr-x   0 jaydamask   (501) staff       (20)        0 2024-01-27 23:05:02.496302 thucyd-0.2.5/src/
-drwxr-xr-x   0 jaydamask   (501) staff       (20)        0 2024-01-27 23:05:02.498734 thucyd-0.2.5/src/thucyd/
--rw-r--r--   0 jaydamask   (501) staff       (20)      381 2024-01-27 22:27:16.000000 thucyd-0.2.5/src/thucyd/__init__.py
-drwxr-xr-x   0 jaydamask   (501) staff       (20)        0 2024-01-27 23:05:02.501619 thucyd-0.2.5/src/thucyd/eigen/
--rw-------   0 jaydamask   (501) staff       (20)      359 2019-07-06 15:17:24.000000 thucyd-0.2.5/src/thucyd/eigen/__init__.py
--rw-r--r--   0 jaydamask   (501) staff       (20)    25971 2024-01-16 14:43:46.000000 thucyd-0.2.5/src/thucyd/eigen/impl.py
-drwxr-xr-x   0 jaydamask   (501) staff       (20)        0 2024-01-27 23:05:02.501009 thucyd-0.2.5/src/thucyd.egg-info/
--rw-r--r--   0 jaydamask   (501) staff       (20)     4226 2024-01-27 23:05:02.000000 thucyd-0.2.5/src/thucyd.egg-info/PKG-INFO
--rw-------   0 jaydamask   (501) staff       (20)      332 2024-01-27 23:05:02.000000 thucyd-0.2.5/src/thucyd.egg-info/SOURCES.txt
--rw-------   0 jaydamask   (501) staff       (20)        1 2024-01-27 23:05:02.000000 thucyd-0.2.5/src/thucyd.egg-info/dependency_links.txt
--rw-------   0 jaydamask   (501) staff       (20)        1 2019-07-06 19:54:07.000000 thucyd-0.2.5/src/thucyd.egg-info/not-zip-safe
--rw-------   0 jaydamask   (501) staff       (20)       12 2024-01-27 23:05:02.000000 thucyd-0.2.5/src/thucyd.egg-info/requires.txt
--rw-------   0 jaydamask   (501) staff       (20)        7 2024-01-27 23:05:02.000000 thucyd-0.2.5/src/thucyd.egg-info/top_level.txt
+drwxr-xr-x   0 jaydamask   (501) staff       (20)        0 2024-04-27 20:12:33.323679 thucyd-0.2.6/
+-rw-------   0 jaydamask   (501) staff       (20)    11372 2019-06-17 15:13:10.000000 thucyd-0.2.6/LICENSE
+-rw-r--r--   0 jaydamask   (501) staff       (20)      114 2023-12-28 23:36:11.000000 thucyd-0.2.6/MANIFEST.in
+-rw-r--r--   0 jaydamask   (501) staff       (20)     4199 2024-04-27 20:12:33.323438 thucyd-0.2.6/PKG-INFO
+-rw-r--r--   0 jaydamask   (501) staff       (20)     3060 2024-01-02 22:30:37.000000 thucyd-0.2.6/README.md
+-rw-r--r--   0 jaydamask   (501) staff       (20)      863 2024-04-27 19:28:53.000000 thucyd-0.2.6/pyproject.toml
+-rw-r--r--   0 jaydamask   (501) staff       (20)       38 2024-04-27 20:12:33.323805 thucyd-0.2.6/setup.cfg
+-rw-r--r--   0 jaydamask   (501) staff       (20)     2310 2024-04-27 19:28:53.000000 thucyd-0.2.6/setup.py
+drwxr-xr-x   0 jaydamask   (501) staff       (20)        0 2024-04-27 20:12:33.318228 thucyd-0.2.6/src/
+drwxr-xr-x   0 jaydamask   (501) staff       (20)        0 2024-04-27 20:12:33.320428 thucyd-0.2.6/src/thucyd/
+-rw-r--r--   0 jaydamask   (501) staff       (20)      381 2024-04-27 19:28:53.000000 thucyd-0.2.6/src/thucyd/__init__.py
+drwxr-xr-x   0 jaydamask   (501) staff       (20)        0 2024-04-27 20:12:33.322886 thucyd-0.2.6/src/thucyd/eigen/
+-rw-------   0 jaydamask   (501) staff       (20)      359 2019-07-06 15:17:24.000000 thucyd-0.2.6/src/thucyd/eigen/__init__.py
+-rw-r--r--   0 jaydamask   (501) staff       (20)    25910 2024-04-27 19:18:41.000000 thucyd-0.2.6/src/thucyd/eigen/impl.py
+drwxr-xr-x   0 jaydamask   (501) staff       (20)        0 2024-04-27 20:12:33.322302 thucyd-0.2.6/src/thucyd.egg-info/
+-rw-r--r--   0 jaydamask   (501) staff       (20)     4199 2024-04-27 20:12:33.000000 thucyd-0.2.6/src/thucyd.egg-info/PKG-INFO
+-rw-------   0 jaydamask   (501) staff       (20)      332 2024-04-27 20:12:33.000000 thucyd-0.2.6/src/thucyd.egg-info/SOURCES.txt
+-rw-------   0 jaydamask   (501) staff       (20)        1 2024-04-27 20:12:33.000000 thucyd-0.2.6/src/thucyd.egg-info/dependency_links.txt
+-rw-------   0 jaydamask   (501) staff       (20)        1 2019-07-06 19:54:07.000000 thucyd-0.2.6/src/thucyd.egg-info/not-zip-safe
+-rw-------   0 jaydamask   (501) staff       (20)       12 2024-04-27 20:12:33.000000 thucyd-0.2.6/src/thucyd.egg-info/requires.txt
+-rw-------   0 jaydamask   (501) staff       (20)        7 2024-04-27 20:12:33.000000 thucyd-0.2.6/src/thucyd.egg-info/top_level.txt
```

### Comparing `thucyd-0.2.5/LICENSE` & `thucyd-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `thucyd-0.2.5/PKG-INFO` & `thucyd-0.2.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thucyd
-Version: 0.2.5
+Version: 0.2.6
 Summary: Reference library for advanced eigenanalysis.
 Home-page: https://gitlab.com/thucyd-dev/thucyd
 Author: Jay Damask
 Author-email: jaydamask@buell-lane-press.co
 License: Apache License 2.0
 Project-URL: Documentation, https://gitlab.com/thucyd-dev/thucyd/
 Project-URL: Changelog, https://gitlab.com/thucyd-dev/thucyd/
@@ -21,15 +21,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.23
 
 <img src="https://gitlab.com/thucyd-dev/thucyd/raw/master/images/thucyd-tile-logo.1500px.png" alt="thucyd-logo" height="150"> 
 
 # Advanced Eigenanalysis 
 
 [![pipeline status](https://gitlab.com/thucyd-dev/thucyd/badges/master/pipeline.svg)](https://gitlab.com/thucyd-dev/thucyd/pipelines)
 [![coverage report](https://gitlab.com/thucyd-dev/thucyd/badges/master/coverage.svg)](https://gitlab.com/thucyd-dev/thucyd/commits/master)
```

### Comparing `thucyd-0.2.5/README.md` & `thucyd-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `thucyd-0.2.5/pyproject.toml` & `thucyd-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # thucyd project configuration
 
 [tool.bumpversion]
-current_version = "0.2.5"
+current_version = "0.2.6"
 commit = false
 tag = false
 message = "Version updated from {current_version} to {new_version}"
 
 [[tool.bumpversion.files]]
 filename = "setup.py"
```

### Comparing `thucyd-0.2.5/setup.py` & `thucyd-0.2.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 setup(
     # id
     name="thucyd",
     url="https://gitlab.com/thucyd-dev/thucyd",
     # key meta
-    version="0.2.5",
+    version="0.2.6",
     license="Apache License 2.0",
     description="""Reference library for advanced eigenanalysis.""",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     # authorship and related
     author="Jay Damask",
     author_email="jaydamask@buell-lane-press.co",
```

### Comparing `thucyd-0.2.5/src/thucyd/eigen/impl.py` & `thucyd-0.2.6/src/thucyd/eigen/impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 This is a reference implementation against which performant implementations
 can be compared.
 
 -------------------------------------------------------------------------------
 """
 
-
 import numpy as np
 import warnings
 
 # define API exposure
 __all__ = [
     "orient_eigenvectors",
     "generate_oriented_eigenvectors",
@@ -44,38 +43,33 @@
 
     Parameters
     ----------
     V: np.ndarray
         Eigenvector matrix with columns vectors
     E: np.ndarray
         Eigenvalue vector whose entries are associated to the columns of V
-    method: bool (default: False)
-        Flag to indicate whether the first eigenvector should point within the
-        first orthant of the space.
+    method: str (default: arcsin)
+        Option to invoke arcsin or arctan2 method {arcsin|arctan2}
     orient_to_first_orthant: bool (default: False)
         Flag to indicate whether the first eigenvector should point within the
         first orthant of the space. Only applicable for the `arctan2` method.
 
     Returns
     -------
     Vor: np.ndarray
         Eigenvector matrix cast into an oriented basis, see Note 1.
-
     Eor: np.ndarray
         Eigenvalue vector whose entries are associated to the columns of Vor,
         see Note 2.
-
     sign_flip_vector: np.ndarray
         Vector of signs that was applied to (sorted) `V` such that `Vor` is
         oriented.
-
     theta_matrix: np.ndarray
         upper-triangular matrix of angles embedded in `Vor` with respect to the
         constituent basis in which (sorted) `V` is materialized.
-
     sort_indices: np.ndarray
         Permutation vector such that Vsort = V[:, sort_indices].
 
     Notes
     -----
     1. The columns of `Vor` are ordered such that their associated eigenvalues
        are sorted in descending order of absolute value. That the absolute
@@ -126,26 +120,22 @@
         Flag to indicate whether the first eigenvector should point within the
         first orthant of the space.
 
     Returns
     -------
     Vor: np.ndarray
         Eigenvector matrix cast into an oriented basis.
-
     Eor: np.ndarray
         Eigenvalue vector whose entries are associated to the columns of Vor.
-
     sign_flip_vector: np.ndarray
         Vector of signs that was applied to (sorted) `V` such that `Vor` is
         oriented.
-
     theta_matrix: np.ndarray
         upper-trianglar matrix of angles embedded in `Vor` with respect to the
         constituent basis in which (sorted) `V` is matrialized.
-
     sort_indices: np.ndarray
         Permutation vector such that Vsort = V[:, sort_indices].
     """
 
     # To begin, sort (V, E) by descending absolute-value of eigenvalues in E.
     Vsort, Esort, sort_indices = sort_eigenvectors(V, E)
 
@@ -202,26 +192,22 @@
     E: np.ndarray
         Eigenvalue vector conformant to V
 
     Returns
     -------
     Vor: np.ndarray
         Eigenvector matrix cast into an oriented basis.
-
     Eor: np.ndarray
         Eigenvalue vector conformant to Vor.
-
     sign_flip_vector: np.ndarray
         Vector of signs that was applied to (sorted) `V` such that `Vor` is
         oriented.
-
     theta_matrix: np.ndarray
         upper-trianglar matrix of angles embedded in `Vor` with respect to the
         constituent basis in which (sorted) `V` is matrialized.
-
     sort_indices: np.ndarray
         Permutation vector such that Vsort = V[:, sort_indices].
     """
 
     # To begin, sort (V, E) by descending absolute-value of eigenvalues in E.
     Vsort, Esort, sort_indices = sort_eigenvectors(V, E)
```

### Comparing `thucyd-0.2.5/src/thucyd.egg-info/PKG-INFO` & `thucyd-0.2.6/src/thucyd.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thucyd
-Version: 0.2.5
+Version: 0.2.6
 Summary: Reference library for advanced eigenanalysis.
 Home-page: https://gitlab.com/thucyd-dev/thucyd
 Author: Jay Damask
 Author-email: jaydamask@buell-lane-press.co
 License: Apache License 2.0
 Project-URL: Documentation, https://gitlab.com/thucyd-dev/thucyd/
 Project-URL: Changelog, https://gitlab.com/thucyd-dev/thucyd/
@@ -21,15 +21,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.23
 
 <img src="https://gitlab.com/thucyd-dev/thucyd/raw/master/images/thucyd-tile-logo.1500px.png" alt="thucyd-logo" height="150"> 
 
 # Advanced Eigenanalysis 
 
 [![pipeline status](https://gitlab.com/thucyd-dev/thucyd/badges/master/pipeline.svg)](https://gitlab.com/thucyd-dev/thucyd/pipelines)
 [![coverage report](https://gitlab.com/thucyd-dev/thucyd/badges/master/coverage.svg)](https://gitlab.com/thucyd-dev/thucyd/commits/master)
```

