# Comparing `tmp/cairocffi-1.6.1.tar.gz` & `tmp/cairocffi-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cairocffi-1.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cairocffi-1.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cairocffi-1.6.1.tar` & `cairocffi-1.7.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1534 2020-10-29 21:18:23.141438 cairocffi-1.6.1/LICENSE
--rw-r--r--   0        0        0       22 2023-03-25 08:13:29.041670 cairocffi-1.6.1/MANIFEST.in
--rw-r--r--   0        0        0     8998 2023-07-24 08:29:41.938151 cairocffi-1.6.1/NEWS.rst
--rw-r--r--   0        0        0     1624 2023-06-12 13:34:52.103553 cairocffi-1.6.1/README.rst
--rw-r--r--   0        0        0     4023 2023-07-24 08:26:28.109928 cairocffi-1.6.1/cairocffi/__init__.py
--rw-r--r--   0        0        0    55889 2023-03-25 08:13:29.050670 cairocffi-1.6.1/cairocffi/constants.py
--rw-r--r--   0        0        0    84444 2023-06-12 13:31:26.008613 cairocffi-1.6.1/cairocffi/context.py
--rw-r--r--   0        0        0     3231 2023-07-23 08:08:07.669624 cairocffi-1.6.1/cairocffi/ffi.py
--rw-r--r--   0        0        0    19496 2023-06-12 13:31:20.781538 cairocffi-1.6.1/cairocffi/fonts.py
--rw-r--r--   0        0        0     8025 2023-06-12 11:29:31.080552 cairocffi-1.6.1/cairocffi/matrix.py
--rw-r--r--   0        0        0    12969 2023-06-12 13:29:55.499320 cairocffi-1.6.1/cairocffi/patterns.py
--rw-r--r--   0        0        0     7244 2023-06-12 13:31:03.919298 cairocffi-1.6.1/cairocffi/pixbuf.py
--rw-r--r--   0        0        0    57784 2023-06-12 13:31:09.782381 cairocffi-1.6.1/cairocffi/surfaces.py
--rw-r--r--   0        0        0    46867 2023-06-12 13:37:13.806570 cairocffi-1.6.1/cairocffi/test_cairo.py
--rw-r--r--   0        0        0      405 2023-03-11 07:55:03.040563 cairocffi-1.6.1/cairocffi/test_numpy.py
--rw-r--r--   0        0        0     2398 2023-03-11 07:55:03.040563 cairocffi-1.6.1/cairocffi/test_pixbuf.py
--rw-r--r--   0        0        0     6338 2023-03-11 07:55:03.040563 cairocffi-1.6.1/cairocffi/test_xcb.py
--rw-r--r--   0        0        0     2011 2023-06-12 10:21:04.001054 cairocffi-1.6.1/cairocffi/xcb.py
--rw-r--r--   0        0        0    21443 2023-06-12 11:34:13.698751 cairocffi-1.6.1/docs/api.rst
--rw-r--r--   0        0        0     4313 2023-06-12 13:29:47.039199 cairocffi-1.6.1/docs/cffi_api.rst
--rw-r--r--   0        0        0       54 2023-03-11 07:55:03.041563 cairocffi-1.6.1/docs/changelog.rst
--rw-r--r--   0        0        0     2792 2023-07-13 15:47:16.814348 cairocffi-1.6.1/docs/conf.py
--rw-r--r--   0        0        0      169 2023-06-12 10:49:57.878672 cairocffi-1.6.1/docs/index.rst
--rw-r--r--   0        0        0     5440 2023-06-12 13:32:34.458590 cairocffi-1.6.1/docs/overview.rst
--rw-r--r--   0        0        0     1234 2020-10-29 21:18:23.144438 cairocffi-1.6.1/docs/pixbuf.rst
--rw-r--r--   0        0        0      273 2020-10-29 21:18:23.144438 cairocffi-1.6.1/docs/xcb.rst
--rw-r--r--   0        0        0     1881 2023-07-23 08:09:25.495449 cairocffi-1.6.1/pyproject.toml
--rw-r--r--   0        0        0      777 2020-10-29 21:18:23.144438 cairocffi-1.6.1/utils/cairo_coverage.py
--rw-r--r--   0        0        0     1390 2020-10-29 21:18:23.144438 cairocffi-1.6.1/utils/cairocffi_to_pycairo.py
--rw-r--r--   0        0        0      756 2020-10-29 21:18:23.144438 cairocffi-1.6.1/utils/compare_pycairo.py
--rw-r--r--   0        0        0     3001 2023-03-25 08:13:29.052671 cairocffi-1.6.1/utils/mkconstants.py
--rw-r--r--   0        0        0     1853 2020-10-29 21:18:23.144438 cairocffi-1.6.1/utils/pango_example.py
--rw-r--r--   0        0        0     1056 2020-10-29 21:18:23.144438 cairocffi-1.6.1/utils/pycairo_to_cairocffi.py
--rw-r--r--   0        0        0      999 2023-03-11 07:55:03.041563 cairocffi-1.6.1/utils/tests.py
--rw-r--r--   0        0        0     3342 1970-01-01 00:00:00.000000 cairocffi-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1534 2020-10-29 21:18:23.141438 cairocffi-1.7.0/LICENSE
+-rw-r--r--   0        0        0       22 2023-03-25 08:13:29.041670 cairocffi-1.7.0/MANIFEST.in
+-rw-r--r--   0        0        0     9334 2024-04-27 12:40:02.120414 cairocffi-1.7.0/NEWS.rst
+-rw-r--r--   0        0        0     1624 2024-04-27 11:19:25.519863 cairocffi-1.7.0/README.rst
+-rw-r--r--   0        0        0     4579 2024-04-27 12:40:02.120414 cairocffi-1.7.0/cairocffi/__init__.py
+-rw-r--r--   0        0        0    55889 2023-03-25 08:13:29.050670 cairocffi-1.7.0/cairocffi/constants.py
+-rw-r--r--   0        0        0    84444 2023-06-12 13:31:26.008613 cairocffi-1.7.0/cairocffi/context.py
+-rw-r--r--   0        0        0     3231 2023-07-23 08:08:07.669624 cairocffi-1.7.0/cairocffi/ffi.py
+-rw-r--r--   0        0        0    19496 2023-06-12 13:31:20.781538 cairocffi-1.7.0/cairocffi/fonts.py
+-rw-r--r--   0        0        0     8038 2024-04-27 12:39:56.323326 cairocffi-1.7.0/cairocffi/matrix.py
+-rw-r--r--   0        0        0    12969 2023-06-12 13:29:55.499320 cairocffi-1.7.0/cairocffi/patterns.py
+-rw-r--r--   0        0        0     7244 2023-06-12 13:31:03.919298 cairocffi-1.7.0/cairocffi/pixbuf.py
+-rw-r--r--   0        0        0    57812 2024-04-27 12:39:56.324326 cairocffi-1.7.0/cairocffi/surfaces.py
+-rw-r--r--   0        0        0    46910 2024-04-27 12:39:56.324326 cairocffi-1.7.0/cairocffi/test_cairo.py
+-rw-r--r--   0        0        0      406 2024-04-27 12:39:56.324326 cairocffi-1.7.0/cairocffi/test_numpy.py
+-rw-r--r--   0        0        0     2398 2023-03-11 07:55:03.040563 cairocffi-1.7.0/cairocffi/test_pixbuf.py
+-rw-r--r--   0        0        0     6330 2024-04-27 12:39:56.325326 cairocffi-1.7.0/cairocffi/test_xcb.py
+-rw-r--r--   0        0        0     2011 2023-06-12 10:21:04.001054 cairocffi-1.7.0/cairocffi/xcb.py
+-rw-r--r--   0        0        0    21443 2023-06-12 11:34:13.698751 cairocffi-1.7.0/docs/api.rst
+-rw-r--r--   0        0        0     4313 2023-06-12 13:29:47.039199 cairocffi-1.7.0/docs/cffi_api.rst
+-rw-r--r--   0        0        0       54 2023-03-11 07:55:03.041563 cairocffi-1.7.0/docs/changelog.rst
+-rw-r--r--   0        0        0     2792 2023-07-13 15:47:16.814348 cairocffi-1.7.0/docs/conf.py
+-rw-r--r--   0        0        0      169 2023-06-12 10:49:57.878672 cairocffi-1.7.0/docs/index.rst
+-rw-r--r--   0        0        0     5577 2024-03-11 13:31:04.801544 cairocffi-1.7.0/docs/overview.rst
+-rw-r--r--   0        0        0     1234 2020-10-29 21:18:23.144438 cairocffi-1.7.0/docs/pixbuf.rst
+-rw-r--r--   0        0        0      273 2020-10-29 21:18:23.144438 cairocffi-1.7.0/docs/xcb.rst
+-rw-r--r--   0        0        0     1904 2024-04-27 12:39:56.325326 cairocffi-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0      792 2024-04-27 12:39:56.325326 cairocffi-1.7.0/utils/cairo_coverage.py
+-rw-r--r--   0        0        0     1405 2024-04-27 12:39:56.325326 cairocffi-1.7.0/utils/cairocffi_to_pycairo.py
+-rw-r--r--   0        0        0      757 2024-04-27 12:39:56.325326 cairocffi-1.7.0/utils/compare_pycairo.py
+-rw-r--r--   0        0        0     3029 2024-04-27 12:39:56.325326 cairocffi-1.7.0/utils/mkconstants.py
+-rw-r--r--   0        0        0     1854 2024-04-27 12:39:56.325326 cairocffi-1.7.0/utils/pango_example.py
+-rw-r--r--   0        0        0     1071 2024-04-27 12:39:56.326326 cairocffi-1.7.0/utils/pycairo_to_cairocffi.py
+-rw-r--r--   0        0        0      997 2024-04-27 12:39:56.326326 cairocffi-1.7.0/utils/tests.py
+-rw-r--r--   0        0        0     3302 1970-01-01 00:00:00.000000 cairocffi-1.7.0/PKG-INFO
```

### Comparing `cairocffi-1.6.1/LICENSE` & `cairocffi-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.1/NEWS.rst` & `cairocffi-1.7.0/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 cairocffi changelog
 -------------------
 
 
+Version 1.7.0
+.............
+
+Released on 2024-04-27
+
+* Drop Python 3.7 support, add Python 3.12 support
+* `#221 <https://github.com/Kozea/cairocffi/pull/225>`_:
+  Add environment variable to set folder where DLLs are installed on Windows
+* `#225 <https://github.com/Kozea/cairocffi/pull/225>`_:
+  Use Ruff instead of Flake8 and isort
+
+
 Version 1.6.1
 .............
 
 Released on 2023-07-24
 
 * `#217 <https://github.com/Kozea/cairocffi/issues/217>`_:
   Repair installation with PyInstaller
```

### Comparing `cairocffi-1.6.1/README.rst` & `cairocffi-1.7.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 .. _CFFI: https://cffi.readthedocs.org/
 .. _Pycairo: https://pycairo.readthedocs.io/
 .. _cairo: http://cairographics.org/
 .. _GDK-PixBuf: https://gitlab.gnome.org/GNOME/gdk-pixbuf
 
 * Free software: BSD license
-* For Python 3.7+, tested on CPython and PyPy
+* For Python 3.8+, tested on CPython and PyPy
 * Documentation: https://doc.courtbouillon.org/cairocffi/
 * Changelog: https://doc.courtbouillon.org/cairocffi/stable/changelog.html
 * Code, issues, tests: https://github.com/Kozea/cairocffi
 * Code of conduct: https://www.courtbouillon.org/code-of-conduct
 * Professional support: https://www.courtbouillon.org
 * Donation: https://opencollective.com/courtbouillon
 * API partially compatible with Pycairo.
```

### Comparing `cairocffi-1.6.1/cairocffi/__init__.py` & `cairocffi-1.7.0/cairocffi/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,34 +5,47 @@
     CFFI-based cairo bindings for Python. See README for details.
 
     :copyright: Copyright 2013-2019 by Simon Sapin
     :license: BSD, see LICENSE for details.
 
 """
 
+import os
 import sys
+from contextlib import suppress
 from ctypes.util import find_library
 
 from . import constants
 from .ffi import ffi
 
-VERSION = __version__ = '1.6.1'
+VERSION = __version__ = '1.7.0'
 # supported version of cairo, used to be pycairo version too:
 version = '1.17.2'
 version_info = (1, 17, 2)
 
 
+# Python 3.8 no longer searches for DLLs in PATH, so we can add everything in
+# CAIROCFFI_DLL_DIRECTORIES manually. Note that unlike PATH, add_dll_directory
+# has no defined order, so if there are two cairo DLLs in PATH we might get a
+# random one.
+dll_directories = os.getenv('CAIROCFFI_DLL_DIRECTORIES')
+if dll_directories and hasattr(os, 'add_dll_directory'):
+    for path in dll_directories.split(';'):
+        with suppress((OSError, FileNotFoundError)):
+            os.add_dll_directory(path)
+
+
 def dlopen(ffi, library_names, filenames):
     """Try various names for the same library, for different platforms."""
     exceptions = []
 
     for library_name in library_names:
         library_filename = find_library(library_name)
         if library_filename:
-            filenames = (library_filename,) + filenames
+            filenames = (library_filename, *filenames)
         else:
             exceptions.append(
                 'no library called "{}" was found'.format(library_name))
 
     for filename in filenames:
         try:
             return ffi.dlopen(filename)
@@ -45,15 +58,15 @@
 
 
 cairo = dlopen(
     ffi, ('cairo-2', 'cairo', 'libcairo-2'),
     ('libcairo.so.2', 'libcairo.2.dylib', 'libcairo-2.dll'))
 
 
-class _keepref(object):
+class _keepref(object):  # noqa: N801
     """Function wrapper that keeps a reference to another object."""
     def __init__(self, ref, func):
         self.ref = ref
         self.func = func
 
     def __call__(self, *args, **kwargs):
         self.func(*args, **kwargs)
```

### Comparing `cairocffi-1.6.1/cairocffi/constants.py` & `cairocffi-1.7.0/cairocffi/constants.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.1/cairocffi/context.py` & `cairocffi-1.7.0/cairocffi/context.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.1/cairocffi/ffi.py` & `cairocffi-1.7.0/cairocffi/ffi.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.1/cairocffi/fonts.py` & `cairocffi-1.7.0/cairocffi/fonts.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.1/cairocffi/matrix.py` & `cairocffi-1.7.0/cairocffi/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
     def __ne__(self, other):
         return self.as_tuple() != other.as_tuple()
 
     def __repr__(self):
         class_ = type(self)
         return '%s(%g, %g, %g, %g, %g, %g)' % (
-            (class_.__name__,) + self.as_tuple())
+            (class_.__name__, *self.as_tuple()))
 
     def multiply(self, other):
         """Multiply with another matrix
         and return the result as a new :class:`Matrix` object.
         Same as ``self * other``.
 
         """
@@ -231,15 +231,15 @@
         :returns: A ``(new_dx, new_dy)`` tuple of floats.
 
         """
         xy = ffi.new('double[2]', [dx, dy])
         cairo.cairo_matrix_transform_distance(self._pointer, xy + 0, xy + 1)
         return tuple(xy)
 
-    def _component_property(name):
+    def _component_property(name):  # noqa: N805
         return property(
             lambda self: getattr(self._pointer, name),
             lambda self, value: setattr(self._pointer, name, value),
             doc='Read-write attribute access to a single float component.')
 
     xx = _component_property('xx')
     yx = _component_property('yx')
```

### Comparing `cairocffi-1.6.1/cairocffi/patterns.py` & `cairocffi-1.7.0/cairocffi/patterns.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.1/cairocffi/pixbuf.py` & `cairocffi-1.7.0/cairocffi/pixbuf.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.1/cairocffi/surfaces.py` & `cairocffi-1.7.0/cairocffi/surfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     :attr:`closure` is a tuple of cairo_destroy_func_t and void* cdata objects,
     as expected by cairo_surface_set_mime_data().
 
     Either :meth:`save` must be called before the callback,
     or none of them must be called.
 
     """
-    instances = set()
+    instances = set()  # noqa: RUF012
 
     def __init__(self, *objects):
         self.objects = objects
         weakself = weakref.ref(self)
 
         def closure(_):
             value = weakself()
@@ -651,15 +651,15 @@
         if return_bytes:
             target = io.BytesIO()
         if hasattr(target, 'write'):
             try:
                 write_func = _make_write_func(target)
                 _check_status(cairo.cairo_surface_write_to_png_stream(
                     self._pointer, write_func, ffi.NULL))
-            except (SystemError, MemoryError):  # noqa
+            except (SystemError, MemoryError):  # pragma: no cover
                 # Callback creation has failed
                 if hasattr(target, 'name'):
                     # File-like object has a name, write here
                     _check_status(cairo.cairo_surface_write_to_png(
                         self._pointer, _encode_filename(target.name)))
                 else:
                     # Use a fallback temporary file
```

### Comparing `cairocffi-1.6.1/cairocffi/test_cairo.py` & `cairocffi-1.7.0/cairocffi/test_cairo.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,19 +16,20 @@
 import io
 import math
 import os
 import shutil
 import sys
 import tempfile
 
-import cairocffi
 import pikepdf
 import pytest
 
-from . import (
+import cairocffi
+
+from . import (  # isort:skip
     PDF_METADATA_AUTHOR, PDF_METADATA_CREATE_DATE, PDF_METADATA_CREATOR,
     PDF_METADATA_KEYWORDS, PDF_METADATA_MOD_DATE, PDF_METADATA_SUBJECT,
     PDF_METADATA_TITLE, PDF_OUTLINE_FLAG_BOLD, PDF_OUTLINE_FLAG_OPEN,
     PDF_OUTLINE_ROOT, SVG_UNIT_PC, SVG_UNIT_PT, SVG_UNIT_PX, SVG_UNIT_USER,
     TAG_LINK, Context, FontFace, FontOptions, ImageSurface, LinearGradient,
     Matrix, Pattern, PDFSurface, PSSurface, RadialGradient, RecordingSurface,
     ScaledFont, SolidPattern, Surface, SurfacePattern, SVGSurface, ToyFontFace,
@@ -1029,28 +1030,28 @@
     context.fill()
 
     surface = ImageSurface(cairocffi.FORMAT_ARGB32, 4, 4)
     context = Context(surface)
     context.mask(SurfacePattern(mask_surface))
     o = pixel(b'\x00\x00\x00\x00')
     b = pixel(b'\x80\x00\x00\x00')
-    B = pixel(b'\xFF\x00\x00\x00')
+    B = pixel(b'\xFF\x00\x00\x00')  # noqa: N806
     assert surface.get_data()[:] == (
         B + o + o + o +
         o + b + o + o +
         o + o + o + o +
         o + o + o + o
     )
 
     surface = ImageSurface(cairocffi.FORMAT_ARGB32, 4, 4)
     context = Context(surface)
     context.mask_surface(mask_surface, surface_x=1, surface_y=2)
     o = pixel(b'\x00\x00\x00\x00')
     b = pixel(b'\x80\x00\x00\x00')
-    B = pixel(b'\xFF\x00\x00\x00')
+    B = pixel(b'\xFF\x00\x00\x00')  # noqa: N806
     assert surface.get_data()[:] == (
         o + o + o + o +
         o + o + o + o +
         o + B + o + o +
         o + o + b + o
     )
```

### Comparing `cairocffi-1.6.1/cairocffi/test_pixbuf.py` & `cairocffi-1.7.0/cairocffi/test_pixbuf.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.1/cairocffi/test_xcb.py` & `cairocffi-1.7.0/cairocffi/test_xcb.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 """
 
 import os
 import time
 
 import pytest
 
-xcffib = pytest.importorskip('xcffib')  # noqa
+xcffib = pytest.importorskip('xcffib')
 
 import xcffib.xproto  # noqa isort:skip
 from xcffib.xproto import ConfigWindow, CW, EventMask, GC  # noqa isort:skip
 
 from . import Context, XCBSurface, cairo_version  # noqa isort:skip
```

### Comparing `cairocffi-1.6.1/cairocffi/xcb.py` & `cairocffi-1.7.0/cairocffi/xcb.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.1/docs/api.rst` & `cairocffi-1.7.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.1/docs/cffi_api.rst` & `cairocffi-1.7.0/docs/cffi_api.rst`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.1/docs/conf.py` & `cairocffi-1.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.1/docs/overview.rst` & `cairocffi-1.7.0/docs/overview.rst`

 * *Files 1% similar despite different names*

```diff
@@ -56,17 +56,21 @@
 cairocffi will dynamically load cairo as a shared library at this point.
 If it fails to find it, you will see an exception like this::
 
     OSError: library not found: 'cairo'
 
 Make sure cairo is correctly installed and available through your system’s
 usual mechanisms.
+
 On Linux, the ``LD_LIBRARY_PATH`` environment variable can be used to indicate
 where to find shared libraries.
 
+On Windows, you can put the folder where Cairo and other DLLs are installed in
+the ``CAIROCFFI_DLL_DIRECTORIES`` environment variable.
+
 .. _Pycairo: http://cairographics.org/pycairo/
 
 
 Installing cairo on Windows
 ...........................
 
 cairocffi needs a ``libcairo-2.dll`` file
```

### Comparing `cairocffi-1.6.1/docs/pixbuf.rst` & `cairocffi-1.7.0/docs/pixbuf.rst`

 * *Files identical despite different names*

### Comparing `cairocffi-1.6.1/pyproject.toml` & `cairocffi-1.7.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -4,56 +4,56 @@
 
 [project]
 name = 'cairocffi'
 description = 'cffi-based cairo bindings for Python'
 keywords = ['cairo', 'cffi', 'binding']
 authors = [{name = 'Simon Sapin', email = 'contact@courtbouillon.org'}]
 maintainers = [{name = 'CourtBouillon', email = 'contact@courtbouillon.org'}]
-requires-python = '>=3.7'
+requires-python = '>=3.8'
 readme = {file = 'README.rst', content-type = 'text/x-rst'}
 license = {file = 'LICENSE'}
 dependencies = [
     'cffi >= 1.1.0',
 ]
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: BSD License',
     'Operating System :: POSIX :: Linux',
     'Operating System :: MacOS :: MacOS X',
     'Operating System :: Microsoft :: Windows',
     'Programming Language :: Python :: 3 :: Only',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
     'Topic :: Multimedia :: Graphics',
 ]
 dynamic = ['version']
 
 [project.urls]
 Documentation = 'https://doc.courtbouillon.org/cairocffi/'
 Code = 'https://github.com/Kozea/cairocffi/'
 Issues = 'https://github.com/Kozea/cairocffi/issues'
 Changelog = 'https://doc.courtbouillon.org/cairocffi/stable/changelog.html'
 Donation = 'https://opencollective.com/courtbouillon'
 
 [project.optional-dependencies]
 doc = ['sphinx', 'sphinx_rtd_theme']
-test = ['pytest', 'flake8', 'isort', 'numpy', 'pikepdf']
+test = ['pytest', 'ruff', 'numpy', 'pikepdf']
 xcb = ['xcffib >= 1.4.0']
 
 [tool.flit.sdist]
 exclude = ['.*']
 
 [tool.coverage.run]
 branch = true
 include = ['cairocffi/*']
 
 [tool.coverage.report]
 exclude_lines = ['pragma: no cover', 'def __repr__', 'raise NotImplementedError']
 omit = ['.*']
 
-[tool.isort]
-default_section = 'FIRSTPARTY'
-multi_line_output = 4
+[tool.ruff.lint]
+select = ['E', 'W', 'F', 'I', 'N', 'RUF']
+ignore = ['RUF001', 'RUF002', 'RUF003']
```

### Comparing `cairocffi-1.6.1/utils/cairo_coverage.py` & `cairocffi-1.7.0/utils/cairo_coverage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import inspect
 
-import cairocffi
 import pycparser
 
+import cairocffi
+
 ALL_THE_CODE = ''.join(
     line
     for module in [
         cairocffi, cairocffi.surfaces, cairocffi.patterns,
         cairocffi.fonts, cairocffi.context, cairocffi.matrix]
     for line in inspect.getsourcelines(module)[0])
 
 
 class Visitor(pycparser.c_ast.NodeVisitor):
-    def visit_Decl(self, node):
+    def visit_Decl(self, node):  # noqa: N802
         for _, child in node.children():
             if isinstance(child, pycparser.c_ast.FuncDecl):
                 if ('cairo.' + node.name) not in ALL_THE_CODE and not (
                         node.name.endswith('user_data')):
                     print(node.name)
                 break
```

### Comparing `cairocffi-1.6.1/utils/cairocffi_to_pycairo.py` & `cairocffi-1.7.0/utils/cairocffi_to_pycairo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import ctypes
 
 import cairo  # pycairo
+
 import cairocffi
 
 pycairo = ctypes.PyDLL(cairo._cairo.__file__)
 pycairo.PycairoContext_FromContext.restype = ctypes.c_void_p
 pycairo.PycairoContext_FromContext.argtypes = 3 * [ctypes.c_void_p]
 ctypes.pythonapi.PyList_Append.argtypes = 2 * [ctypes.c_void_p]
 
 
-def _UNSAFE_cairocffi_context_to_pycairo(cairocffi_context):
+def _UNSAFE_cairocffi_context_to_pycairo(cairocffi_context):  # noqa: N802
     # Sanity check. Continuing with another type would probably segfault.
     if not isinstance(cairocffi_context, cairocffi.Context):
         raise TypeError('Expected a cairocffi.Context, got %r'
                         % cairocffi_context)
 
     # Create a reference for PycairoContext_FromContext to take ownership of.
     cairocffi.cairo.cairo_reference(cairocffi_context._pointer)
```

### Comparing `cairocffi-1.6.1/utils/compare_pycairo.py` & `cairocffi-1.7.0/utils/compare_pycairo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import cairo as pycairo
+
 import cairocffi
 
 # We want the real pycairo
 assert pycairo is not cairocffi
 
 
 print('Missing pycairo API:\n')
```

### Comparing `cairocffi-1.6.1/utils/mkconstants.py` & `cairocffi-1.7.0/utils/mkconstants.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,23 +12,23 @@
     elif isinstance(node, pycparser.c_ast.UnaryOp) and node.op == '-':
         return '-' + parse_constant(node.expr)
     else:
         raise TypeError(node)
 
 
 class PrintEnumsVisitor(pycparser.c_ast.NodeVisitor):
-    def visit_Decl(self, node):
+    def visit_Decl(self, node):  # noqa: N802
         if node.name and node.name.startswith('CAIRO_'):  # len('CAIRO_') == 6
             if node.init.type == 'string':
                 print('%s = b%s' % (node.name[6:], node.init.value))
             else:
                 print('%s = %s' % (node.name[6:], node.init.value))
             print('')
 
-    def visit_Enum(self, node):
+    def visit_Enum(self, node):  # noqa: N802
         value = 0
         for enumerator in node.values.enumerators:
             if enumerator.value is not None:
                 value_string = parse_constant(enumerator.value)
                 value = int(value_string, 0)
             else:
                 value_string = str(value)
```

### Comparing `cairocffi-1.6.1/utils/pango_example.py` & `cairocffi-1.7.0/utils/pango_example.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import cairocffi
 import cffi
 
+import cairocffi
+
 ffi = cffi.FFI()
 ffi.cdef('''
     /* GLib */
     typedef void cairo_t;
     typedef void* gpointer;
     void g_object_unref (gpointer object);
```

### Comparing `cairocffi-1.6.1/utils/pycairo_to_cairocffi.py` & `cairocffi-1.7.0/utils/pycairo_to_cairocffi.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import cairo  # pycairo
+
 import cairocffi
 
 
-def _UNSAFE_pycairo_context_to_cairocffi(pycairo_context):
+def _UNSAFE_pycairo_context_to_cairocffi(pycairo_context):  # noqa: N802
     # Sanity check. Continuing with another type would probably segfault.
     if not isinstance(pycairo_context, cairo.Context):
         raise TypeError('Expected a cairo.Context, got %r' % pycairo_context)
 
     # On CPython, id() gives the memory address of a Python object.
     # pycairo implements Context as a C struct:
     #     typedef struct {
```

### Comparing `cairocffi-1.6.1/utils/tests.py` & `cairocffi-1.7.0/utils/tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import io
 
-import cairo  # noqa, pycairo
-import cairocffi
+import cairo  # noqa: F401
 import pango_example
 from cairocffi_to_pycairo import _UNSAFE_cairocffi_context_to_pycairo
 from pycairo_to_cairocffi import _UNSAFE_pycairo_context_to_cairocffi
 
+import cairocffi
+
 
 def test():
     cairocffi_context = cairocffi.Context(cairocffi.PDFSurface(None, 10, 20))
     cairocffi_context.scale(2, 3)
     pycairo_context = _UNSAFE_cairocffi_context_to_pycairo(cairocffi_context)
     cairocffi_context2 = _UNSAFE_pycairo_context_to_cairocffi(pycairo_context)
     assert tuple(cairocffi_context.get_matrix()) == (2, 0, 0, 3, 0, 0)
```

### Comparing `cairocffi-1.6.1/PKG-INFO` & `cairocffi-1.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: cairocffi
-Version: 1.6.1
+Version: 1.7.0
 Summary: cffi-based cairo bindings for Python
 Keywords: cairo,cffi,binding
 Author-email: Simon Sapin <contact@courtbouillon.org>
 Maintainer-email: CourtBouillon <contact@courtbouillon.org>
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Graphics
 Requires-Dist: cffi >= 1.1.0
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: sphinx_rtd_theme ; extra == "doc"
 Requires-Dist: pytest ; extra == "test"
-Requires-Dist: flake8 ; extra == "test"
-Requires-Dist: isort ; extra == "test"
+Requires-Dist: ruff ; extra == "test"
 Requires-Dist: numpy ; extra == "test"
 Requires-Dist: pikepdf ; extra == "test"
 Requires-Dist: xcffib >= 1.4.0 ; extra == "xcb"
 Project-URL: Changelog, https://doc.courtbouillon.org/cairocffi/stable/changelog.html
 Project-URL: Code, https://github.com/Kozea/cairocffi/
 Project-URL: Documentation, https://doc.courtbouillon.org/cairocffi/
 Project-URL: Donation, https://opencollective.com/courtbouillon
@@ -48,15 +47,15 @@
 
 .. _CFFI: https://cffi.readthedocs.org/
 .. _Pycairo: https://pycairo.readthedocs.io/
 .. _cairo: http://cairographics.org/
 .. _GDK-PixBuf: https://gitlab.gnome.org/GNOME/gdk-pixbuf
 
 * Free software: BSD license
-* For Python 3.7+, tested on CPython and PyPy
+* For Python 3.8+, tested on CPython and PyPy
 * Documentation: https://doc.courtbouillon.org/cairocffi/
 * Changelog: https://doc.courtbouillon.org/cairocffi/stable/changelog.html
 * Code, issues, tests: https://github.com/Kozea/cairocffi
 * Code of conduct: https://www.courtbouillon.org/code-of-conduct
 * Professional support: https://www.courtbouillon.org
 * Donation: https://opencollective.com/courtbouillon
 * API partially compatible with Pycairo.
```

