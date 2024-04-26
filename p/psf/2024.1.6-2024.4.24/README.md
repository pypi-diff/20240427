# Comparing `tmp/psf-2024.1.6.tar.gz` & `tmp/psf-2024.4.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psf-2024.1.6.tar", last modified: Sun Jan  7 09:38:25 2024, max compression
+gzip compressed data, was "psf-2024.4.24.tar", last modified: Fri Apr 26 23:38:47 2024, max compression
```

## Comparing `psf-2024.1.6.tar` & `psf-2024.4.24.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-01-07 09:38:25.573469 psf-2024.1.6/
-drwxrwxrwx   0        0        0        0 2024-01-07 09:38:25.557837 psf-2024.1.6/.github/
-drwxrwxrwx   0        0        0        0 2024-01-07 09:38:25.573469 psf-2024.1.6/.github/workflows/
--rw-rw-rw-   0        0        0      848 2024-01-07 09:00:13.000000 psf-2024.1.6/.github/workflows/wheel.yml
--rw-rw-rw-   0        0        0     1576 2024-01-07 09:38:24.000000 psf-2024.1.6/LICENSE
--rw-rw-rw-   0        0        0      407 2024-01-07 09:11:23.000000 psf-2024.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4929 2024-01-07 09:38:25.573469 psf-2024.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     3834 2024-01-07 09:38:24.000000 psf-2024.1.6/README.rst
-drwxrwxrwx   0        0        0        0 2024-01-07 09:38:25.573469 psf-2024.1.6/psf/
--rw-rw-rw-   0        0        0       89 2020-01-01 02:37:31.000000 psf-2024.1.6/psf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-07 09:38:25.573469 psf-2024.1.6/psf/examples/
--rw-rw-rw-   0        0        0     4486 2024-01-07 09:37:15.000000 psf-2024.1.6/psf/examples/psf_example.py
--rw-rw-rw-   0        0        0    38415 2023-04-26 17:40:40.000000 psf-2024.1.6/psf/psf.c
--rw-rw-rw-   0        0        0    32872 2024-01-07 09:30:36.000000 psf-2024.1.6/psf/psf.py
--rw-rw-rw-   0        0        0        0 2024-01-07 09:06:41.000000 psf-2024.1.6/psf/py.typed
-drwxrwxrwx   0        0        0        0 2024-01-07 09:38:25.573469 psf-2024.1.6/psf.egg-info/
--rw-rw-rw-   0        0        0     4929 2024-01-07 09:38:25.000000 psf-2024.1.6/psf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-01-07 09:38:25.000000 psf-2024.1.6/psf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-07 09:38:25.000000 psf-2024.1.6/psf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-01-07 09:38:25.000000 psf-2024.1.6/psf.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       24 2024-01-07 09:38:25.000000 psf-2024.1.6/psf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-01-07 09:38:25.000000 psf-2024.1.6/psf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      102 2024-01-06 21:20:36.000000 psf-2024.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-07 09:38:25.573469 psf-2024.1.6/setup.cfg
--rw-rw-rw-   0        0        0     2636 2024-01-07 09:38:11.000000 psf-2024.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 23:38:47.823592 psf-2024.4.24/
+drwxrwxrwx   0        0        0        0 2024-04-26 23:38:47.807966 psf-2024.4.24/.github/
+drwxrwxrwx   0        0        0        0 2024-04-26 23:38:47.807966 psf-2024.4.24/.github/workflows/
+-rw-rw-rw-   0        0        0      858 2024-04-26 23:35:40.000000 psf-2024.4.24/.github/workflows/wheel.yml
+-rw-rw-rw-   0        0        0     1576 2024-04-26 23:38:46.000000 psf-2024.4.24/LICENSE
+-rw-rw-rw-   0        0        0      406 2024-01-07 20:00:16.000000 psf-2024.4.24/MANIFEST.in
+-rw-rw-rw-   0        0        0     4966 2024-04-26 23:38:47.823592 psf-2024.4.24/PKG-INFO
+-rw-rw-rw-   0        0        0     3870 2024-04-26 23:38:46.000000 psf-2024.4.24/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-26 23:38:47.807966 psf-2024.4.24/psf/
+-rw-rw-rw-   0        0        0       89 2020-01-01 02:37:31.000000 psf-2024.4.24/psf/__init__.py
+-rw-rw-rw-   0        0        0      274 2024-01-07 21:43:10.000000 psf-2024.4.24/psf/conftest.py
+drwxrwxrwx   0        0        0        0 2024-04-26 23:38:47.823592 psf-2024.4.24/psf/examples/
+-rw-rw-rw-   0        0        0     4484 2024-04-26 23:31:12.000000 psf-2024.4.24/psf/examples/psf_example.py
+-rw-rw-rw-   0        0        0    38415 2024-04-20 04:10:19.000000 psf-2024.4.24/psf/psf.c
+-rw-rw-rw-   0        0        0    32907 2024-04-26 23:36:50.000000 psf-2024.4.24/psf/psf.py
+-rw-rw-rw-   0        0        0        0 2024-01-07 09:06:41.000000 psf-2024.4.24/psf/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-26 23:38:47.823592 psf-2024.4.24/psf.egg-info/
+-rw-rw-rw-   0        0        0     4966 2024-04-26 23:38:47.000000 psf-2024.4.24/psf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2024-04-26 23:38:47.000000 psf-2024.4.24/psf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 23:38:47.000000 psf-2024.4.24/psf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-26 23:38:47.000000 psf-2024.4.24/psf.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       24 2024-04-26 23:38:47.000000 psf-2024.4.24/psf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-26 23:38:47.000000 psf-2024.4.24/psf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      102 2024-01-06 21:20:36.000000 psf-2024.4.24/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-26 23:38:47.823592 psf-2024.4.24/setup.cfg
+-rw-rw-rw-   0        0        0     2636 2024-01-07 09:38:11.000000 psf-2024.4.24/setup.py
```

### Comparing `psf-2024.1.6/.github/workflows/wheel.yml` & `psf-2024.4.24/.github/workflows/wheel.yml`

 * *Files 13% similar despite different names*

```diff
@@ -8,18 +8,18 @@
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-22.04, macos-12, windows-2019]
     steps:
       - uses: actions/checkout@v4
-      - uses: pypa/cibuildwheel@v2.16.2
+      - uses: pypa/cibuildwheel@v2.17.0
         env:
           CIBW_SKIP: "pp* cp37* cp38* *musllinux* *i686 *ppc64le *s390x cp39*win*arm64 cp310*win*arm64"
-          CIBW_BEFORE_BUILD: python -m pip install numpy
+          CIBW_BEFORE_BUILD: python -m pip install numpy>=2.0.0rc1
           # CIBW_ARCHS_LINUX: auto aarch64
           CIBW_ARCHS_LINUX: auto
           CIBW_ARCHS_MACOS: x86_64 arm64
           CIBW_ARCHS_WINDOWS: AMD64 ARM64 x86
           CIBW_TEST_REQUIRES: numpy
           CIBW_TEST_COMMAND: python -m psf.psf
       - uses: actions/upload-artifact@v4
```

### Comparing `psf-2024.1.6/LICENSE` & `psf-2024.4.24/LICENSE`

 * *Files identical despite different names*

### Comparing `psf-2024.1.6/PKG-INFO` & `psf-2024.4.24/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psf
-Version: 2024.1.6
+Version: 2024.4.24
 Summary: Point Spread Function calculations for fluorescence microscopy
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/psf/issues
 Project-URL: Source Code, https://github.com/cgohlke/psf
@@ -33,15 +33,15 @@
 Psf is a Python library to calculate Point Spread Functions (PSF) for
 fluorescence microscopy.
 
 The psf library is no longer actively developed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.1.6
+:Version: 2024.4.24
 
 Quickstart
 ----------
 
 Install the psf package and all dependencies from the
 `Python Package Index <https://pypi.org/project/psf/>`_::
 
@@ -54,22 +54,26 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.7, 3.12.1
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.3
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_  3.8.2
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_  3.8.4
   (optional for plotting)
 
 Revisions
 ---------
 
+2024.4.24
+
+- Support NumPy 2.
+
 2024.1.6
 
 - Change PSF.TYPES from dict to set (breaking).
 
 2023.4.26
 
 - Use enums.
```

### Comparing `psf-2024.1.6/README.rst` & `psf-2024.4.24/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Psf is a Python library to calculate Point Spread Functions (PSF) for
 fluorescence microscopy.
 
 The psf library is no longer actively developed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.1.6
+:Version: 2024.4.24
 
 Quickstart
 ----------
 
 Install the psf package and all dependencies from the
 `Python Package Index <https://pypi.org/project/psf/>`_::
 
@@ -25,22 +25,26 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.7, 3.12.1
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.3
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_  3.8.2
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_  3.8.4
   (optional for plotting)
 
 Revisions
 ---------
 
+2024.4.24
+
+- Support NumPy 2.
+
 2024.1.6
 
 - Change PSF.TYPES from dict to set (breaking).
 
 2023.4.26
 
 - Use enums.
```

### Comparing `psf-2024.1.6/psf/examples/psf_example.py` & `psf-2024.4.24/psf/examples/psf_example.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 
 Demonstrate the use of the psf library for calculating point spread functions
 for fluorescence microscopy.
 
 """
 
 import numpy
-from matplotlib import pyplot
-
 import psf
+from matplotlib import pyplot
 
 
 def psf_example(
     cmap='hot',
     savebin=False,
     savetif=False,
     savevol=False,
```

### Comparing `psf-2024.1.6/psf/psf.c` & `psf-2024.4.24/psf/psf.c`

 * *Files identical despite different names*

### Comparing `psf-2024.1.6/psf/psf.py` & `psf-2024.4.24/psf/psf.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 Psf is a Python library to calculate Point Spread Functions (PSF) for
 fluorescence microscopy.
 
 The psf library is no longer actively developed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.1.6
+:Version: 2024.4.24
 
 Quickstart
 ----------
 
 Install the psf package and all dependencies from the
 `Python Package Index <https://pypi.org/project/psf/>`_::
 
@@ -55,22 +55,26 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.7, 3.12.1
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.3
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_  3.8.2
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_  3.8.4
   (optional for plotting)
 
 Revisions
 ---------
 
+2024.4.24
+
+- Support NumPy 2.
+
 2024.1.6
 
 - Change PSF.TYPES from dict to set (breaking).
 
 2023.4.26
 
 - Use enums.
@@ -168,15 +172,15 @@
 
 Refer to `psf_example.py` in the source distribution for more examples.
 
 """
 
 from __future__ import annotations
 
-__version__ = '2024.1.6'
+__version__ = '2024.4.24'
 
 __all__ = [
     'PSF',
     'PsfType',
     'Pinhole',
     'PinholeShape',
     'Dimensions',
@@ -197,24 +201,23 @@
 ]
 
 import enum
 import math
 import threading
 import time
 from collections import UserDict
+from typing import TYPE_CHECKING
 
 import numpy
 
 try:
     from . import _psf
 except ImportError:
     import _psf  # type: ignore
 
-from typing import TYPE_CHECKING
-
 if TYPE_CHECKING:
     from collections.abc import Iterable, Mapping
     from typing import Any, TypeVar
 
     from numpy.typing import ArrayLike, NDArray
 
     DimensionT = TypeVar('DimensionT')
```

### Comparing `psf-2024.1.6/psf.egg-info/PKG-INFO` & `psf-2024.4.24/psf.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psf
-Version: 2024.1.6
+Version: 2024.4.24
 Summary: Point Spread Function calculations for fluorescence microscopy
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/psf/issues
 Project-URL: Source Code, https://github.com/cgohlke/psf
@@ -33,15 +33,15 @@
 Psf is a Python library to calculate Point Spread Functions (PSF) for
 fluorescence microscopy.
 
 The psf library is no longer actively developed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.1.6
+:Version: 2024.4.24
 
 Quickstart
 ----------
 
 Install the psf package and all dependencies from the
 `Python Package Index <https://pypi.org/project/psf/>`_::
 
@@ -54,22 +54,26 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.7, 3.12.1
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.3
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_  3.8.2
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_  3.8.4
   (optional for plotting)
 
 Revisions
 ---------
 
+2024.4.24
+
+- Support NumPy 2.
+
 2024.1.6
 
 - Change PSF.TYPES from dict to set (breaking).
 
 2023.4.26
 
 - Use enums.
```

### Comparing `psf-2024.1.6/setup.py` & `psf-2024.4.24/setup.py`

 * *Files identical despite different names*

