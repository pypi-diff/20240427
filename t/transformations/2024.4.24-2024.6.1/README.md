# Comparing `tmp/transformations-2024.4.24.tar.gz` & `tmp/transformations-2024.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformations-2024.4.24.tar", last modified: Sat Apr 27 04:42:16 2024, max compression
+gzip compressed data, was "transformations-2024.6.1.tar", last modified: Mon Jan  8 03:04:16 2024, max compression
```

## Comparing `transformations-2024.4.24.tar` & `transformations-2024.6.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 04:42:16.866294 transformations-2024.4.24/
-drwxrwxrwx   0        0        0        0 2024-04-27 04:42:16.861750 transformations-2024.4.24/.github/
-drwxrwxrwx   0        0        0        0 2024-04-27 04:42:16.866294 transformations-2024.4.24/.github/workflows/
--rw-rw-rw-   0        0        0      916 2024-04-27 04:41:32.000000 transformations-2024.4.24/.github/workflows/wheel.yml
--rw-rw-rw-   0        0        0     1559 2024-04-27 04:42:15.000000 transformations-2024.4.24/LICENSE
--rw-rw-rw-   0        0        0      442 2024-01-07 20:00:29.000000 transformations-2024.4.24/MANIFEST.in
--rw-rw-rw-   0        0        0     9114 2024-04-27 04:42:16.866294 transformations-2024.4.24/PKG-INFO
--rw-rw-rw-   0        0        0     8057 2024-04-27 04:42:15.000000 transformations-2024.4.24/README.rst
--rw-rw-rw-   0        0        0      102 2024-01-06 21:20:36.000000 transformations-2024.4.24/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-27 04:42:16.866294 transformations-2024.4.24/setup.cfg
--rw-rw-rw-   0        0        0     2716 2024-04-20 04:04:20.000000 transformations-2024.4.24/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 04:42:16.866294 transformations-2024.4.24/transformations/
--rw-rw-rw-   0        0        0      116 2020-01-01 04:09:36.000000 transformations-2024.4.24/transformations/__init__.py
--rw-rw-rw-   0        0        0      385 2024-04-27 00:41:40.000000 transformations-2024.4.24/transformations/conftest.py
--rw-rw-rw-   0        0        0   120827 2024-04-27 01:42:42.000000 transformations-2024.4.24/transformations/transformations.c
--rw-rw-rw-   0        0        0    69913 2024-04-27 00:44:31.000000 transformations-2024.4.24/transformations/transformations.py
-drwxrwxrwx   0        0        0        0 2024-04-27 04:42:16.866294 transformations-2024.4.24/transformations.egg-info/
--rw-rw-rw-   0        0        0     9114 2024-04-27 04:42:16.000000 transformations-2024.4.24/transformations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2024-04-27 04:42:16.000000 transformations-2024.4.24/transformations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 04:42:16.000000 transformations-2024.4.24/transformations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-27 04:42:16.000000 transformations-2024.4.24/transformations.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2024-04-27 04:42:16.000000 transformations-2024.4.24/transformations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-27 04:42:16.000000 transformations-2024.4.24/transformations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-01-08 03:04:16.273677 transformations-2024.6.1/
+drwxrwxrwx   0        0        0        0 2024-01-08 03:04:16.258047 transformations-2024.6.1/.github/
+drwxrwxrwx   0        0        0        0 2024-01-08 03:04:16.273677 transformations-2024.6.1/.github/workflows/
+-rw-rw-rw-   0        0        0      897 2024-01-07 22:01:24.000000 transformations-2024.6.1/.github/workflows/wheel.yml
+-rw-rw-rw-   0        0        0     1559 2024-01-08 03:04:15.000000 transformations-2024.6.1/LICENSE
+-rw-rw-rw-   0        0        0      442 2024-01-07 20:00:29.000000 transformations-2024.6.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     9077 2024-01-08 03:04:16.273677 transformations-2024.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8021 2024-01-08 03:04:15.000000 transformations-2024.6.1/README.rst
+-rw-rw-rw-   0        0        0      102 2024-01-06 21:20:36.000000 transformations-2024.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-01-08 03:04:16.273677 transformations-2024.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     2716 2024-01-07 19:57:40.000000 transformations-2024.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-08 03:04:16.273677 transformations-2024.6.1/transformations/
+-rw-rw-rw-   0        0        0      116 2020-01-01 04:09:36.000000 transformations-2024.6.1/transformations/__init__.py
+-rw-rw-rw-   0        0        0      344 2024-01-07 21:36:22.000000 transformations-2024.6.1/transformations/conftest.py
+-rw-rw-rw-   0        0        0   120825 2024-01-07 20:01:49.000000 transformations-2024.6.1/transformations/transformations.c
+-rw-rw-rw-   0        0        0    70080 2024-01-08 03:02:23.000000 transformations-2024.6.1/transformations/transformations.py
+drwxrwxrwx   0        0        0        0 2024-01-08 03:04:16.273677 transformations-2024.6.1/transformations.egg-info/
+-rw-rw-rw-   0        0        0     9077 2024-01-08 03:04:15.000000 transformations-2024.6.1/transformations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2024-01-08 03:04:16.000000 transformations-2024.6.1/transformations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-08 03:04:15.000000 transformations-2024.6.1/transformations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-01-08 03:04:15.000000 transformations-2024.6.1/transformations.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2024-01-08 03:04:15.000000 transformations-2024.6.1/transformations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-01-08 03:04:15.000000 transformations-2024.6.1/transformations.egg-info/top_level.txt
```

### Comparing `transformations-2024.4.24/.github/workflows/wheel.yml` & `transformations-2024.6.1/.github/workflows/wheel.yml`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,18 @@
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-22.04, macos-12, windows-2019]
     steps:
       - uses: actions/checkout@v4
-      - uses: pypa/cibuildwheel@v2.17.0
+      - uses: pypa/cibuildwheel@v2.16.2
         env:
-          # CIBW_ENVIRONMENT: "PIP_PRE=1"
-          CIBW_BUILD_VERBOSITY: 3
           CIBW_SKIP: "pp* cp37* cp38* *musllinux* *i686 *ppc64le *s390x cp39*win*arm64 cp310*win*arm64"
+          CIBW_BEFORE_BUILD: python -m pip install numpy
           # CIBW_ARCHS_LINUX: auto aarch64
           CIBW_ARCHS_LINUX: auto
           CIBW_ARCHS_MACOS: x86_64 arm64
           CIBW_ARCHS_WINDOWS: AMD64 ARM64 x86
           CIBW_TEST_REQUIRES: numpy pytest
           CIBW_TEST_COMMAND: python -m pytest --doctest-modules --pyargs transformations
       - uses: actions/upload-artifact@v4
```

### Comparing `transformations-2024.4.24/LICENSE` & `transformations-2024.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `transformations-2024.4.24/PKG-INFO` & `transformations-2024.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformations
-Version: 2024.4.24
+Version: 2024.6.1
 Summary: Homogeneous Transformation Matrices and Quaternions
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/transformations/issues
 Project-URL: Source Code, https://github.com/cgohlke/transformations
@@ -35,15 +35,15 @@
 and quaternions. Also includes an Arcball control object and
 functions to decompose transformation matrices.
 
 The transformations library is no longer actively developed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.24
+:Version: 2024.6.1
 
 Quickstart
 ----------
 
 Install the transformations package and all dependencies from the
 `Python Package Index <https://pypi.org/project/transformations/>`_::
 
@@ -56,25 +56,21 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.7, 3.12.1
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.3
 
 Revisions
 ---------
 
-2024.4.24
-
-- Support NumPy 2.
-
-2024.1.6
+2024.6.1
 
 - Remove support for Python 3.8 and numpy 1.22 (NEP 29).
 
 2022.9.26
 
 - Add dimension check on superimposition_matrix (#2).
```

### Comparing `transformations-2024.4.24/README.rst` & `transformations-2024.6.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 and quaternions. Also includes an Arcball control object and
 functions to decompose transformation matrices.
 
 The transformations library is no longer actively developed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.24
+:Version: 2024.6.1
 
 Quickstart
 ----------
 
 Install the transformations package and all dependencies from the
 `Python Package Index <https://pypi.org/project/transformations/>`_::
 
@@ -29,25 +29,21 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.7, 3.12.1
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.3
 
 Revisions
 ---------
 
-2024.4.24
-
-- Support NumPy 2.
-
-2024.1.6
+2024.6.1
 
 - Remove support for Python 3.8 and numpy 1.22 (NEP 29).
 
 2022.9.26
 
 - Add dimension check on superimposition_matrix (#2).
```

### Comparing `transformations-2024.4.24/setup.py` & `transformations-2024.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `transformations-2024.4.24/transformations/transformations.c` & `transformations-2024.6.1/transformations/transformations.c`

 * *Files 0% similar despite different names*

```diff
@@ -35,21 +35,21 @@
 Transformations.c is a Python C extension module that provides faster\n\
 implementations for the transformations package.\n\
 \n\
 Refer to the transformations.py module for documentation and tests.\n\
 \n\
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_\n\
 :License: BSD 3-Clause\n\
-:Version: 2024.4.24\n\
+:Version: 2024.6.1\n\
 "
 
-#define _VERSION_ "2024.4.24"
+#define _VERSION_ "2024.6.1"
 
 #define WIN32_LEAN_AND_MEAN
-#define NPY_NO_DEPRECATED_API NPY_2_0_API_VERSION
+#define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION
 
 #include "Python.h"
 
 #ifdef _WIN32
 #include <windows.h>
 #include <wincrypt.h>
 #endif
```

### Comparing `transformations-2024.4.24/transformations/transformations.py` & `transformations-2024.6.1/transformations/transformations.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 and quaternions. Also includes an Arcball control object and
 functions to decompose transformation matrices.
 
 The transformations library is no longer actively developed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.24
+:Version: 2024.6.1
 
 Quickstart
 ----------
 
 Install the transformations package and all dependencies from the
 `Python Package Index <https://pypi.org/project/transformations/>`_::
 
@@ -59,25 +59,21 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.7, 3.12.1
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.3
 
 Revisions
 ---------
 
-2024.4.24
-
-- Support NumPy 2.
-
-2024.1.6
+2024.6.1
 
 - Remove support for Python 3.8 and numpy 1.22 (NEP 29).
 
 2022.9.26
 
 - Add dimension check on superimposition_matrix (#2).
 
@@ -244,15 +240,15 @@
 >>> numpy.allclose(unit_vector(v1), unit_vector(v2))
 True
 
 """
 
 from __future__ import annotations
 
-__version__ = '2024.4.24'
+__version__ = '2024.6.1'
 
 import math
 
 import numpy
 
 
 def identity_matrix():
@@ -288,15 +284,15 @@
 
     >>> v0 = numpy.random.random(3) - 0.5
     >>> v1 = translation_from_matrix(translation_matrix(v0))
     >>> numpy.allclose(v0, v1)
     True
 
     """
-    return numpy.asarray(matrix)[:3, 3].copy()
+    return numpy.array(matrix, copy=False)[:3, 3].copy()
 
 
 def reflection_matrix(point, normal):
     """Return matrix to mirror at plane defined by point and normal vector.
 
     >>> v0 = numpy.random.random(4) - 0.5
     >>> v0[3] = 1.
@@ -329,15 +325,15 @@
     >>> M0 = reflection_matrix(v0, v1)
     >>> point, normal = reflection_from_matrix(M0)
     >>> M1 = reflection_matrix(point, normal)
     >>> is_same_transform(M0, M1)
     True
 
     """
-    M = numpy.asarray(matrix, dtype=numpy.float64)
+    M = numpy.array(matrix, dtype=numpy.float64, copy=False)
     # normal: unit eigenvector corresponding to eigenvalue -1
     w, V = numpy.linalg.eig(M[:3, :3])
     i = numpy.where(abs(numpy.real(w) + 1.0) < 1e-8)[0]
     if len(i) == 0:
         raise ValueError('no unit eigenvector corresponding to eigenvalue -1')
     normal = numpy.real(V[:, i[0]]).squeeze()
     # point: any unit eigenvector corresponding to eigenvalue 1
@@ -389,15 +385,15 @@
             [-direction[1], direction[0], 0.0],
         ]
     )
     M = numpy.identity(4)
     M[:3, :3] = R
     if point is not None:
         # rotation not around origin
-        point = numpy.asarray(point[:3], dtype=numpy.float64)
+        point = numpy.array(point[:3], dtype=numpy.float64, copy=False)
         M[:3, 3] = point - numpy.dot(R, point)
     return M
 
 
 def rotation_from_matrix(matrix):
     """Return rotation angle and axis from rotation matrix.
 
@@ -407,15 +403,15 @@
     >>> R0 = rotation_matrix(angle, direc, point)
     >>> angle, direc, point = rotation_from_matrix(R0)
     >>> R1 = rotation_matrix(angle, direc, point)
     >>> is_same_transform(R0, R1)
     True
 
     """
-    R = numpy.asarray(matrix, dtype=numpy.float64)
+    R = numpy.array(matrix, dtype=numpy.float64, copy=False)
     R33 = R[:3, :3]
     # direction: unit eigenvector of R33 corresponding to eigenvalue of 1
     w, W = numpy.linalg.eig(R33.T)
     i = numpy.where(abs(numpy.real(w) - 1.0) < 1e-8)[0]
     if len(i) == 0:
         raise ValueError('no unit eigenvector corresponding to eigenvalue 1')
     direction = numpy.real(W[:, i[-1]]).squeeze()
@@ -492,15 +488,15 @@
     >>> S0 = scale_matrix(factor, origin, direct)
     >>> factor, origin, direction = scale_from_matrix(S0)
     >>> S1 = scale_matrix(factor, origin, direction)
     >>> is_same_transform(S0, S1)
     True
 
     """
-    M = numpy.asarray(matrix, dtype=numpy.float64)
+    M = numpy.array(matrix, dtype=numpy.float64, copy=False)
     M33 = M[:3, :3]
     factor = numpy.trace(M33) - 2.0
     try:
         # direction: unit eigenvector corresponding to eigenvalue factor
         w, V = numpy.linalg.eig(M33)
         i = numpy.where(abs(numpy.real(w) - factor) < 1e-8)[0][0]
         direction = numpy.real(V[:, i]).squeeze()
@@ -549,32 +545,34 @@
     >>> numpy.allclose(v1[1], v0[1])
     True
     >>> numpy.allclose(v1[0], 3-v1[1])
     True
 
     """
     M = numpy.identity(4)
-    point = numpy.asarray(point[:3], dtype=numpy.float64)
+    point = numpy.array(point[:3], dtype=numpy.float64, copy=False)
     normal = unit_vector(normal[:3])
     if perspective is not None:
         # perspective projection
-        perspective = numpy.asarray(perspective[:3], dtype=numpy.float64)
+        perspective = numpy.array(
+            perspective[:3], dtype=numpy.float64, copy=False
+        )
         M[0, 0] = M[1, 1] = M[2, 2] = numpy.dot(perspective - point, normal)
         M[:3, :3] -= numpy.outer(perspective, normal)
         if pseudo:
             # preserve relative depth
             M[:3, :3] -= numpy.outer(normal, normal)
             M[:3, 3] = numpy.dot(point, normal) * (perspective + normal)
         else:
             M[:3, 3] = numpy.dot(point, normal) * perspective
         M[3, :3] = -normal
         M[3, 3] = numpy.dot(perspective, normal)
     elif direction is not None:
         # parallel projection
-        direction = numpy.asarray(direction[:3], dtype=numpy.float64)
+        direction = numpy.array(direction[:3], dtype=numpy.float64, copy=False)
         scale = numpy.dot(direction, normal)
         M[:3, :3] -= numpy.outer(direction, normal) / scale
         M[:3, 3] = direction * (numpy.dot(point, normal) / scale)
     else:
         # orthogonal projection
         M[:3, :3] -= numpy.outer(normal, normal)
         M[:3, 3] = numpy.dot(point, normal) * normal
@@ -609,15 +607,15 @@
     >>> P0 = projection_matrix(point, normal, perspective=persp, pseudo=True)
     >>> result = projection_from_matrix(P0, pseudo=True)
     >>> P1 = projection_matrix(*result)
     >>> is_same_transform(P0, P1)
     True
 
     """
-    M = numpy.asarray(matrix, dtype=numpy.float64)
+    M = numpy.array(matrix, dtype=numpy.float64, copy=False)
     M33 = M[:3, :3]
     w, V = numpy.linalg.eig(M)
     i = numpy.where(abs(numpy.real(w) - 1.0) < 1e-8)[0]
     if not pseudo and len(i) > 0:
         # point: any eigenvector corresponding to eigenvalue 1
         point = numpy.real(V[:, i[-1]]).squeeze()
         point /= point[3]
@@ -749,15 +747,15 @@
     >>> S0 = shear_matrix(angle, direct, point, normal)
     >>> angle, direct, point, normal = shear_from_matrix(S0)
     >>> S1 = shear_matrix(angle, direct, point, normal)
     >>> is_same_transform(S0, S1)
     True
 
     """
-    M = numpy.asarray(matrix, dtype=numpy.float64)
+    M = numpy.array(matrix, dtype=numpy.float64, copy=False)
     M33 = M[:3, :3]
     # normal: cross independent eigenvectors corresponding to the eigenvalue 1
     w, V = numpy.linalg.eig(M33)
     i = numpy.where(abs(numpy.real(w) - 1.0) < 1e-4)[0]
     if len(i) < 2:
         raise ValueError(f'no two linear independent eigenvectors found {w}')
     V = numpy.real(V[:, i]).squeeze().T
@@ -1105,16 +1103,16 @@
     >>> v = numpy.empty((4, 100, 3))
     >>> v[:, :, 0] = v0
     >>> M = superimposition_matrix(v0, v1, scale=True, usesvd=False)
     >>> numpy.allclose(v1, numpy.dot(M, v[:, :, 0]))
     True
 
     """
-    v0 = numpy.asarray(v0, dtype=numpy.float64)
-    v1 = numpy.asarray(v1, dtype=numpy.float64)
+    v0 = numpy.array(v0, dtype=numpy.float64, copy=False)
+    v1 = numpy.array(v1, dtype=numpy.float64, copy=False)
     if (
         v0.shape != v1.shape
         or v0.ndim != 2
         or v0.shape[0] not in (3, 4)
         or v0.shape[1] < 3
     ):
         raise ValueError('invalid input shapes')
@@ -1211,15 +1209,15 @@
         _TUPLE2AXES[axes]  # noqa: validation
         firstaxis, parity, repetition, frame = axes
 
     i = firstaxis
     j = _NEXT_AXIS[i + parity]
     k = _NEXT_AXIS[i - parity + 1]
 
-    M = numpy.asarray(matrix, dtype=numpy.float64)[:3, :3]
+    M = numpy.array(matrix, dtype=numpy.float64, copy=False)[:3, :3]
     if repetition:
         sy = math.sqrt(M[i, j] * M[i, j] + M[i, k] * M[i, k])
         if sy > _EPS:
             ax = math.atan2(M[i, j], M[i, k])
             ay = math.atan2(sy, M[i, i])
             az = math.atan2(M[j, i], -M[k, i])
         else:
@@ -1408,15 +1406,15 @@
     True
     >>> R = euler_matrix(0.0, 0.0, numpy.pi/2.0)
     >>> is_same_quaternion(quaternion_from_matrix(R, isprecise=False),
     ...                    quaternion_from_matrix(R, isprecise=True))
     True
 
     """
-    M = numpy.asarray(matrix, dtype=numpy.float64)[:4, :4]
+    M = numpy.array(matrix, dtype=numpy.float64, copy=False)[:4, :4]
     if isprecise:
         q = numpy.empty((4,))
         t = numpy.trace(M)
         if t > M[3, 3]:
             q[0] = t
             q[3] = M[1, 0] - M[0, 1]
             q[2] = M[0, 2] - M[2, 0]
@@ -1759,15 +1757,15 @@
     if a[2] == 1.0:
         return numpy.array([1.0, 0.0, 0.0])
     return unit_vector([-a[1], a[0], 0.0])
 
 
 def arcball_nearest_axis(point, axes):
     """Return axis, which arc is nearest to point."""
-    point = numpy.asarray(point, dtype=numpy.float64)
+    point = numpy.array(point, dtype=numpy.float64, copy=False)
     nearest = None
     mx = -1.0
     for axis in axes:
         t = numpy.dot(arcball_constrain_to_axis(point, axis), point)
         if t > mx:
             nearest = axis
             mx = t
@@ -1879,15 +1877,15 @@
     if out is None:
         data = numpy.array(data, dtype=numpy.float64, copy=True)
         if data.ndim == 1:
             data /= math.sqrt(numpy.dot(data, data))
             return data
     else:
         if out is not data:
-            out[:] = numpy.asarray(data)
+            out[:] = numpy.array(data, copy=False)
         data = out
     length = numpy.atleast_1d(numpy.sum(data * data, axis))
     numpy.sqrt(length, length)
     if axis is not None:
         length = numpy.expand_dims(length, axis)
     data /= length
     if out is None:
@@ -1951,16 +1949,16 @@
     >>> v0 = [[2, 0, 0], [2, 0, 0], [0, 2, 0], [2, 0, 0]]
     >>> v1 = [[0, 3, 0], [0, 0, 3], [0, 0, 3], [3, 3, 3]]
     >>> a = angle_between_vectors(v0, v1, axis=1)
     >>> numpy.allclose(a, [1.5708, 1.5708, 1.5708, 0.95532])
     True
 
     """
-    v0 = numpy.asarray(v0, dtype=numpy.float64)
-    v1 = numpy.asarray(v1, dtype=numpy.float64)
+    v0 = numpy.array(v0, dtype=numpy.float64, copy=False)
+    v1 = numpy.array(v1, dtype=numpy.float64, copy=False)
     dot = numpy.sum(v0 * v1, axis=axis)
     dot /= vector_norm(v0, axis=axis) * vector_norm(v1, axis=axis)
     dot = numpy.clip(dot, -1.0, 1.0)
     return numpy.arccos(dot if directed else numpy.fabs(dot))
 
 
 def inverse_matrix(matrix):
```

### Comparing `transformations-2024.4.24/transformations.egg-info/PKG-INFO` & `transformations-2024.6.1/transformations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformations
-Version: 2024.4.24
+Version: 2024.6.1
 Summary: Homogeneous Transformation Matrices and Quaternions
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/transformations/issues
 Project-URL: Source Code, https://github.com/cgohlke/transformations
@@ -35,15 +35,15 @@
 and quaternions. Also includes an Arcball control object and
 functions to decompose transformation matrices.
 
 The transformations library is no longer actively developed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.24
+:Version: 2024.6.1
 
 Quickstart
 ----------
 
 Install the transformations package and all dependencies from the
 `Python Package Index <https://pypi.org/project/transformations/>`_::
 
@@ -56,25 +56,21 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.7, 3.12.1
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.3
 
 Revisions
 ---------
 
-2024.4.24
-
-- Support NumPy 2.
-
-2024.1.6
+2024.6.1
 
 - Remove support for Python 3.8 and numpy 1.22 (NEP 29).
 
 2022.9.26
 
 - Add dimension check on superimposition_matrix (#2).
```

