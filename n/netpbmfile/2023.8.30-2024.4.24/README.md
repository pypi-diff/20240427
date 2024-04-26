# Comparing `tmp/netpbmfile-2023.8.30.tar.gz` & `tmp/netpbmfile-2024.4.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netpbmfile-2023.8.30.tar", last modified: Wed Aug 30 16:27:40 2023, max compression
+gzip compressed data, was "netpbmfile-2024.4.24.tar", last modified: Fri Apr 26 23:26:04 2024, max compression
```

## Comparing `netpbmfile-2023.8.30.tar` & `netpbmfile-2024.4.24.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-08-30 16:27:40.883419 netpbmfile-2023.8.30/
--rw-rw-rw-   0        0        0     1559 2023-08-30 16:27:35.000000 netpbmfile-2023.8.30/LICENSE
--rw-rw-rw-   0        0        0      452 2023-08-11 03:02:29.000000 netpbmfile-2023.8.30/MANIFEST.in
--rw-rw-rw-   0        0        0     5235 2023-08-30 16:27:40.883419 netpbmfile-2023.8.30/PKG-INFO
--rw-rw-rw-   0        0        0     4261 2023-08-30 16:27:35.000000 netpbmfile-2023.8.30/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-30 16:27:40.867795 netpbmfile-2023.8.30/netpbmfile/
--rw-rw-rw-   0        0        0      110 2020-01-01 10:25:54.000000 netpbmfile-2023.8.30/netpbmfile/__init__.py
--rw-rw-rw-   0        0        0      141 2020-01-09 14:46:14.000000 netpbmfile-2023.8.30/netpbmfile/__main__.py
--rw-rw-rw-   0        0        0    38489 2023-08-30 16:11:12.000000 netpbmfile-2023.8.30/netpbmfile/netpbmfile.py
--rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 netpbmfile-2023.8.30/netpbmfile/py.typed
-drwxrwxrwx   0        0        0        0 2023-08-30 16:27:40.883419 netpbmfile-2023.8.30/netpbmfile.egg-info/
--rw-rw-rw-   0        0        0     5235 2023-08-30 16:27:39.000000 netpbmfile-2023.8.30/netpbmfile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-08-30 16:27:40.000000 netpbmfile-2023.8.30/netpbmfile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-30 16:27:39.000000 netpbmfile-2023.8.30/netpbmfile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-08-30 16:27:39.000000 netpbmfile-2023.8.30/netpbmfile.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2023-08-30 16:27:39.000000 netpbmfile-2023.8.30/netpbmfile.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-30 16:27:39.000000 netpbmfile-2023.8.30/netpbmfile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-30 16:27:40.883419 netpbmfile-2023.8.30/setup.cfg
--rw-rw-rw-   0        0        0     2765 2023-08-30 03:49:48.000000 netpbmfile-2023.8.30/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-30 16:27:40.883419 netpbmfile-2023.8.30/tests/
--rw-rw-rw-   0        0        0      657 2023-08-30 05:26:18.000000 netpbmfile-2023.8.30/tests/conftest.py
--rw-rw-rw-   0        0        0    31872 2022-12-28 01:08:37.000000 netpbmfile-2023.8.30/tests/data.npy
--rw-rw-rw-   0        0        0    15498 2023-08-30 05:27:21.000000 netpbmfile-2023.8.30/tests/test_netpbmfile.py
+drwxrwxrwx   0        0        0        0 2024-04-26 23:26:04.375813 netpbmfile-2024.4.24/
+-rw-rw-rw-   0        0        0     1559 2024-04-26 23:26:03.000000 netpbmfile-2024.4.24/LICENSE
+-rw-rw-rw-   0        0        0      452 2023-08-11 03:02:29.000000 netpbmfile-2024.4.24/MANIFEST.in
+-rw-rw-rw-   0        0        0     5377 2024-04-26 23:26:04.375813 netpbmfile-2024.4.24/PKG-INFO
+-rw-rw-rw-   0        0        0     4297 2024-04-26 23:26:03.000000 netpbmfile-2024.4.24/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-26 23:26:04.360189 netpbmfile-2024.4.24/netpbmfile/
+-rw-rw-rw-   0        0        0      110 2020-01-01 10:25:54.000000 netpbmfile-2024.4.24/netpbmfile/__init__.py
+-rw-rw-rw-   0        0        0      141 2020-01-09 14:46:14.000000 netpbmfile-2024.4.24/netpbmfile/__main__.py
+-rw-rw-rw-   0        0        0    38648 2024-04-26 23:24:40.000000 netpbmfile-2024.4.24/netpbmfile/netpbmfile.py
+-rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 netpbmfile-2024.4.24/netpbmfile/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-26 23:26:04.375813 netpbmfile-2024.4.24/netpbmfile.egg-info/
+-rw-rw-rw-   0        0        0     5377 2024-04-26 23:26:04.000000 netpbmfile-2024.4.24/netpbmfile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2024-04-26 23:26:04.000000 netpbmfile-2024.4.24/netpbmfile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 23:26:04.000000 netpbmfile-2024.4.24/netpbmfile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-04-26 23:26:04.000000 netpbmfile-2024.4.24/netpbmfile.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2024-04-26 23:26:04.000000 netpbmfile-2024.4.24/netpbmfile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-26 23:26:04.000000 netpbmfile-2024.4.24/netpbmfile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 23:26:04.375813 netpbmfile-2024.4.24/setup.cfg
+-rw-rw-rw-   0        0        0     2765 2023-08-30 03:49:48.000000 netpbmfile-2024.4.24/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 23:26:04.375813 netpbmfile-2024.4.24/tests/
+-rw-rw-rw-   0        0        0      657 2023-08-30 05:26:18.000000 netpbmfile-2024.4.24/tests/conftest.py
+-rw-rw-rw-   0        0        0    31872 2022-12-28 01:08:37.000000 netpbmfile-2024.4.24/tests/data.npy
+-rw-rw-rw-   0        0        0    15496 2024-04-26 23:25:55.000000 netpbmfile-2024.4.24/tests/test_netpbmfile.py
```

### Comparing `netpbmfile-2023.8.30/LICENSE` & `netpbmfile-2024.4.24/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2011-2023, Christoph Gohlke
+Copyright (c) 2011-2024, Christoph Gohlke
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice,
    this list of conditions and the following disclaimer.
```

### Comparing `netpbmfile-2023.8.30/PKG-INFO` & `netpbmfile-2024.4.24/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netpbmfile
-Version: 2023.8.30
+Version: 2024.4.24
 Summary: Read and write Netpbm files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/netpbmfile/issues
 Project-URL: Source Code, https://github.com/cgohlke/netpbmfile
@@ -17,16 +17,19 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
-Provides-Extra: all
 License-File: LICENSE
+Requires-Dist: numpy
+Provides-Extra: all
+Requires-Dist: tifffile; extra == "all"
+Requires-Dist: matplotlib; extra == "all"
 
 Read and write Netpbm files
 ===========================
 
 Netpbmfile is a Python library to read and write image files in the Netpbm
 or related formats:
 
@@ -35,23 +38,23 @@
 - PPM (Portable Pixel Map): P3 (text) and P6 (binary)
 - PNM (Portable Any Map): shorthand for PBM, PGM, and PPM collectively
 - PAM (Portable Arbitrary Map): P7, bilevel, gray, and rgb
 - PGX (Portable Graymap Signed): PG, signed grayscale
 - PFM (Portable Float Map): Pf (gray), PF (rgb), and PF4 (rgba), read-only
 - XV thumbnail: P7 332 (rgb332), read-only
 
-The Netpbm formats are specified at http://netpbm.sourceforge.net/doc/.
+The Netpbm formats are specified at https://netpbm.sourceforge.net/doc/.
 
 The PGX format is specified in ITU-T Rec. T.803.
 
 No gamma correction or scaling is performed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.8.30
+:Version: 2024.4.24
 
 Quickstart
 ----------
 
 Install the netpbmfile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/netpbmfile/>`_::
 
@@ -64,20 +67,24 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.5, 3.12rc
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.25.2
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 
 Revisions
 ---------
 
+2024.4.24
+
+- Support NumPy 2.
+
 2023.8.30
 
 - Fix linting issues.
 - Add py.typed marker.
 
 2023.6.15
```

### Comparing `netpbmfile-2023.8.30/README.rst` & `netpbmfile-2024.4.24/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 - PPM (Portable Pixel Map): P3 (text) and P6 (binary)
 - PNM (Portable Any Map): shorthand for PBM, PGM, and PPM collectively
 - PAM (Portable Arbitrary Map): P7, bilevel, gray, and rgb
 - PGX (Portable Graymap Signed): PG, signed grayscale
 - PFM (Portable Float Map): Pf (gray), PF (rgb), and PF4 (rgba), read-only
 - XV thumbnail: P7 332 (rgb332), read-only
 
-The Netpbm formats are specified at http://netpbm.sourceforge.net/doc/.
+The Netpbm formats are specified at https://netpbm.sourceforge.net/doc/.
 
 The PGX format is specified in ITU-T Rec. T.803.
 
 No gamma correction or scaling is performed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.8.30
+:Version: 2024.4.24
 
 Quickstart
 ----------
 
 Install the netpbmfile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/netpbmfile/>`_::
 
@@ -38,20 +38,24 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.5, 3.12rc
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.25.2
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 
 Revisions
 ---------
 
+2024.4.24
+
+- Support NumPy 2.
+
 2023.8.30
 
 - Fix linting issues.
 - Add py.typed marker.
 
 2023.6.15
```

### Comparing `netpbmfile-2023.8.30/netpbmfile/netpbmfile.py` & `netpbmfile-2024.4.24/netpbmfile/netpbmfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # netpbmfile.py
 
-# Copyright (c) 2011-2023, Christoph Gohlke
+# Copyright (c) 2011-2024, Christoph Gohlke
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -39,23 +39,23 @@
 - PPM (Portable Pixel Map): P3 (text) and P6 (binary)
 - PNM (Portable Any Map): shorthand for PBM, PGM, and PPM collectively
 - PAM (Portable Arbitrary Map): P7, bilevel, gray, and rgb
 - PGX (Portable Graymap Signed): PG, signed grayscale
 - PFM (Portable Float Map): Pf (gray), PF (rgb), and PF4 (rgba), read-only
 - XV thumbnail: P7 332 (rgb332), read-only
 
-The Netpbm formats are specified at http://netpbm.sourceforge.net/doc/.
+The Netpbm formats are specified at https://netpbm.sourceforge.net/doc/.
 
 The PGX format is specified in ITU-T Rec. T.803.
 
 No gamma correction or scaling is performed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.8.30
+:Version: 2024.4.24
 
 Quickstart
 ----------
 
 Install the netpbmfile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/netpbmfile/>`_::
 
@@ -68,20 +68,24 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.5, 3.12rc
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.25.2
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 
 Revisions
 ---------
 
+2024.4.24
+
+- Support NumPy 2.
+
 2023.8.30
 
 - Fix linting issues.
 - Add py.typed marker.
 
 2023.6.15
 
@@ -192,47 +196,47 @@
 
     $ python -m netpbmfile _tmp.pgm
 
 """
 
 from __future__ import annotations
 
-__version__ = '2023.8.30'
+__version__ = '2024.4.24'
 
 __all__ = ['imread', 'imwrite', 'imsave', 'NetpbmFile']
 
 import math
 import os
 import re
 import sys
 import warnings
 from typing import TYPE_CHECKING
 
 import numpy
 
 if TYPE_CHECKING:
     from collections.abc import Iterable
-    from typing import Any, BinaryIO, Literal, Union
+    from typing import Any, BinaryIO, Literal
 
     from numpy.typing import ArrayLike, NDArray
 
-    ByteOrder = Union[Literal['>'], Literal['<']]
-    MagicNumber = Union[
-        Literal['P1'],
-        Literal['P2'],
-        Literal['P3'],
-        Literal['P4'],
-        Literal['P5'],
-        Literal['P6'],
-        Literal['P7'],
-        Literal['PG'],
-        Literal['Pf'],
-        Literal['PF'],
-        Literal['PF4'],
-        Literal['P7 332'],
+    ByteOrder = Literal['>', '<']
+    MagicNumber = Literal[
+        'P1',
+        'P2',
+        'P3',
+        'P4',
+        'P5',
+        'P6',
+        'P7',
+        'PG',
+        'Pf',
+        'PF',
+        'PF4',
+        'P7 332',
     ]
 
 
 def imread(
     file: str | os.PathLike[Any] | BinaryIO,
     /,
     *,
@@ -456,17 +460,19 @@
 
         if self.magicnumber in 'P1 P2 P3':
             self.frames = 1
         else:
             bytecount = self._fh.seek(0, 2) - len(self.header)
             shape = [
                 self.height,
-                int(math.ceil(self.width / 8))
-                if self.magicnumber in 'P4'
-                else self.width,
+                (
+                    int(math.ceil(self.width / 8))
+                    if self.magicnumber in 'P4'
+                    else self.width
+                ),
                 self.depth,
                 self.dtype.itemsize,
             ]
             self.frames = max(1, bytecount // product(shape))
 
     @classmethod
     def fromdata(
@@ -509,17 +515,17 @@
                 raise ValueError(
                     f'invalid dtype {data.dtype!r} for '
                     f'magicnumber {magicnumber!r}'
                 )
 
         if maxval is None:
             if issigned:
-                maxval = numpy.max(numpy.abs(data))
+                maxval = int(numpy.max(numpy.abs(data)))
             else:
-                maxval = numpy.max(data)
+                maxval = int(numpy.max(data))
             if maxval == 1:
                 maxval = 1
             else:
                 maxval = max(
                     255, int(2 ** math.ceil(math.log2(maxval + 1)) - 1)
                 )
         if not 0 < maxval < 2**32:
@@ -573,27 +579,31 @@
             self.width = data.shape[-1]
             self.height = data.shape[-2]
         else:
             raise ValueError(f'invalid magicnumber {magicnumber}')
 
         if magicnumber == 'PG' and data.dtype.kind == 'i':
             self._data = data.astype(
-                'i1'
-                if maxval < 128
-                else (
-                    cls.byteorder + 'i2'
-                    if maxval < 32768
-                    else cls.byteorder + 'i4'
-                )
+                (
+                    'i1'
+                    if maxval < 128
+                    else (
+                        cls.byteorder + 'i2'
+                        if maxval < 32768
+                        else cls.byteorder + 'i4'
+                    )
+                ),
+                copy=False,
             )
         elif magicnumber in 'P1 P4':
-            self._data = data.astype('bool')
+            self._data = data.astype('bool', copy=False)
         else:
             self._data = data.astype(
-                'u1' if maxval < 256 else ('>u2' if maxval < 65536 else '>u4')
+                'u1' if maxval < 256 else ('>u2' if maxval < 65536 else '>u4'),
+                copy=False,
             )
 
         self.frames = max(
             1, product(data.shape) // (self.height * self.width * self.depth)
         )
         self.magicnumber = magicnumber
         self.maxval = maxval
@@ -865,15 +875,15 @@
             size = product(shape[1:]) * dtype.itemsize
             size *= max(1, len(rawdata) // size)
             data = numpy.frombuffer(rawdata[:size], dtype).reshape(shape)
             if bilevel:
                 data = numpy.unpackbits(data, axis=-2)[:, :, : self.width, :]
 
         if bilevel:
-            data = data.astype('bool')
+            data = data.astype('bool', copy=False)
 
         if data.shape[0] < 2:
             data = data.reshape(data.shape[1:])
         if data.shape[-1] < 2:
             data = data.reshape(data.shape[:-1])
         if self.magicnumber == 'P7 332':
             rgb332 = numpy.array(list(numpy.ndindex(8, 8, 4)), 'u1')
@@ -1052,17 +1062,19 @@
         return indent(
             repr(self),
             f'magicnumber: {self.magicnumber}',
             f'axes: {self.axes}',
             f'shape: {self.shape}',
             f'dtype: {self.dtype}',
             # f'byteorder: {self.byteorder}',
-            f'scale: {self.scale}'
-            if self.magicnumber in 'PF4 Pf'
-            else f'maxval: {self.maxval}',
+            (
+                f'scale: {self.scale}'
+                if self.magicnumber in 'PF4 Pf'
+                else f'maxval: {self.maxval}'
+            ),
         )
 
 
 def product(iterable: Iterable[int], /) -> int:
     """Return product of sequence of numbers."""
     prod = 1
     for i in iterable:
```

### Comparing `netpbmfile-2023.8.30/netpbmfile.egg-info/PKG-INFO` & `netpbmfile-2024.4.24/netpbmfile.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netpbmfile
-Version: 2023.8.30
+Version: 2024.4.24
 Summary: Read and write Netpbm files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/netpbmfile/issues
 Project-URL: Source Code, https://github.com/cgohlke/netpbmfile
@@ -17,16 +17,19 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
-Provides-Extra: all
 License-File: LICENSE
+Requires-Dist: numpy
+Provides-Extra: all
+Requires-Dist: tifffile; extra == "all"
+Requires-Dist: matplotlib; extra == "all"
 
 Read and write Netpbm files
 ===========================
 
 Netpbmfile is a Python library to read and write image files in the Netpbm
 or related formats:
 
@@ -35,23 +38,23 @@
 - PPM (Portable Pixel Map): P3 (text) and P6 (binary)
 - PNM (Portable Any Map): shorthand for PBM, PGM, and PPM collectively
 - PAM (Portable Arbitrary Map): P7, bilevel, gray, and rgb
 - PGX (Portable Graymap Signed): PG, signed grayscale
 - PFM (Portable Float Map): Pf (gray), PF (rgb), and PF4 (rgba), read-only
 - XV thumbnail: P7 332 (rgb332), read-only
 
-The Netpbm formats are specified at http://netpbm.sourceforge.net/doc/.
+The Netpbm formats are specified at https://netpbm.sourceforge.net/doc/.
 
 The PGX format is specified in ITU-T Rec. T.803.
 
 No gamma correction or scaling is performed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.8.30
+:Version: 2024.4.24
 
 Quickstart
 ----------
 
 Install the netpbmfile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/netpbmfile/>`_::
 
@@ -64,20 +67,24 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.5, 3.12rc
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.25.2
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 
 Revisions
 ---------
 
+2024.4.24
+
+- Support NumPy 2.
+
 2023.8.30
 
 - Fix linting issues.
 - Add py.typed marker.
 
 2023.6.15
```

### Comparing `netpbmfile-2023.8.30/setup.py` & `netpbmfile-2024.4.24/setup.py`

 * *Files identical despite different names*

### Comparing `netpbmfile-2023.8.30/tests/conftest.py` & `netpbmfile-2024.4.24/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `netpbmfile-2023.8.30/tests/data.npy` & `netpbmfile-2024.4.24/tests/data.npy`

 * *Files identical despite different names*

### Comparing `netpbmfile-2023.8.30/tests/test_netpbmfile.py` & `netpbmfile-2024.4.24/tests/test_netpbmfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # test_netpbmfile.py
 
-# Copyright (c) 2011-2023, Christoph Gohlke
+# Copyright (c) 2011-2024, Christoph Gohlke
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright
 #   notice, this list of conditions and the following disclaimer.
@@ -25,30 +25,29 @@
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 """Unittests for the netpbmfile package.
 
-:Version: 2023.8.30
+:Version: 2024.4.24
 
 """
 
 import hashlib
 import io
 import os
 import sys
 import tempfile
 
+import netpbmfile
 import numpy
 import pytest
-from numpy.testing import assert_array_equal
-
-import netpbmfile
 from netpbmfile import NetpbmFile, imread, imwrite  # noqa
+from numpy.testing import assert_array_equal
 
 TEST_DIR = os.path.dirname(__file__)
 TEMP_DIR = os.path.join(TEST_DIR, '_tmp')
 
 if not os.path.exists(TEMP_DIR):
     TEMP_DIR = tempfile.gettempdir()
```

