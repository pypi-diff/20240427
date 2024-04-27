# Comparing `tmp/novas-3.1.1.5.tar.gz` & `tmp/novas-3.1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/novas-3.1.1.5.tar", last modified: Sat Jan 25 16:20:22 2020, max compression
+gzip compressed data, was "novas-3.1.1.6.tar", last modified: Sat Apr 27 12:02:03 2024, max compression
```

## Comparing `novas-3.1.1.5.tar` & `novas-3.1.1.6.tar`

### file list

```diff
@@ -1,34 +1,41 @@
-drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2020-01-25 16:20:22.000000 novas-3.1.1.5/
-drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2020-01-25 16:20:22.000000 novas-3.1.1.5/Cdist/
--rw-r-----   0 brandon   (1000) brandon   (1000)    25120 2019-07-19 14:44:08.000000 novas-3.1.1.5/Cdist/eph_manager.c
--rw-r-----   0 brandon   (1000) brandon   (1000)     1397 2019-07-19 14:44:08.000000 novas-3.1.1.5/Cdist/eph_manager.h
--rw-r-----   0 brandon   (1000) brandon   (1000)   263604 2019-07-19 14:44:08.000000 novas-3.1.1.5/Cdist/novas.c
--rw-r-----   0 brandon   (1000) brandon   (1000)    16671 2019-07-19 14:44:08.000000 novas-3.1.1.5/Cdist/novas.h
--rw-r-----   0 brandon   (1000) brandon   (1000)     2324 2019-07-19 14:44:08.000000 novas-3.1.1.5/Cdist/novascon.c
--rw-r-----   0 brandon   (1000) brandon   (1000)     2016 2019-07-19 14:44:08.000000 novas-3.1.1.5/Cdist/novascon.h
--rw-r-----   0 brandon   (1000) brandon   (1000)   236927 2019-07-19 14:44:08.000000 novas-3.1.1.5/Cdist/nutation.c
--rw-r-----   0 brandon   (1000) brandon   (1000)      652 2019-07-19 14:44:08.000000 novas-3.1.1.5/Cdist/nutation.h
--rw-r-----   0 brandon   (1000) brandon   (1000)     2567 2019-07-19 14:44:08.000000 novas-3.1.1.5/Cdist/readeph0.c
--rw-r-----   0 brandon   (1000) brandon   (1000)      642 2019-07-19 14:44:08.000000 novas-3.1.1.5/Cdist/solarsystem.h
--rw-r-----   0 brandon   (1000) brandon   (1000)     8922 2019-07-19 14:44:08.000000 novas-3.1.1.5/Cdist/solsys1.c
--rw-r-----   0 brandon   (1000) brandon   (1000)    12066 2020-01-25 16:20:22.000000 novas-3.1.1.5/PKG-INFO
--rw-r-----   0 brandon   (1000) brandon   (1000)     5225 2019-07-19 14:44:08.000000 novas-3.1.1.5/README
--rw-r-----   0 brandon   (1000) brandon   (1000)     9239 2019-07-19 14:44:08.000000 novas-3.1.1.5/README-PyPI
--rwxr-x---   0 brandon   (1000) brandon   (1000)     4323 2019-07-19 14:44:08.000000 novas-3.1.1.5/asc2eph.py
-drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2020-01-25 16:20:22.000000 novas-3.1.1.5/compat/
--rw-r-----   0 brandon   (1000) brandon   (1000)       59 2019-07-19 14:44:08.000000 novas-3.1.1.5/compat/__init__.py
--rw-r-----   0 brandon   (1000) brandon   (1000)   161113 2019-07-19 14:44:08.000000 novas-3.1.1.5/compat/compat.py
--rw-r-----   0 brandon   (1000) brandon   (1000)    11058 2019-07-19 14:44:08.000000 novas-3.1.1.5/compat/eph_manager.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     4596 2019-07-19 14:44:08.000000 novas-3.1.1.5/compat/nutation.py
--rw-r-----   0 brandon   (1000) brandon   (1000)        0 2019-07-19 14:44:08.000000 novas-3.1.1.5/compat/readeph0.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     6625 2019-07-19 14:44:08.000000 novas-3.1.1.5/compat/solsys.py
-drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2020-01-25 16:20:22.000000 novas-3.1.1.5/novas_py/
--rw-r-----   0 brandon   (1000) brandon   (1000)     2086 2019-07-19 14:44:08.000000 novas-3.1.1.5/novas_py/__init__.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     1646 2019-07-19 14:44:08.000000 novas-3.1.1.5/novas_py/constants.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     7786 2020-01-25 16:19:36.000000 novas-3.1.1.5/setup.py
-drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2020-01-25 16:20:22.000000 novas-3.1.1.5/tests/
--rw-r-----   0 brandon   (1000) brandon   (1000)        0 2019-07-19 14:44:08.000000 novas-3.1.1.5/tests/__init__.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     1080 2019-07-19 14:44:08.000000 novas-3.1.1.5/tests/checkout-stars-full.py
--rw-r-----   0 brandon   (1000) brandon   (1000)    48109 2019-07-19 14:44:08.000000 novas-3.1.1.5/tests/test_compat.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     8210 2019-07-19 14:44:08.000000 novas-3.1.1.5/tests/test_example.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     1309 2019-07-19 14:44:08.000000 novas-3.1.1.5/tests/test_github_issues.py
+drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2024-04-27 12:02:03.976591 novas-3.1.1.6/
+drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2024-04-27 12:02:03.972592 novas-3.1.1.6/Cdist/
+-rw-r-----   0 brandon   (1000) brandon   (1000)    25120 2019-07-19 14:44:08.000000 novas-3.1.1.6/Cdist/eph_manager.c
+-rw-r-----   0 brandon   (1000) brandon   (1000)     1397 2019-07-19 14:44:08.000000 novas-3.1.1.6/Cdist/eph_manager.h
+-rw-r-----   0 brandon   (1000) brandon   (1000)   263604 2020-11-11 22:38:36.000000 novas-3.1.1.6/Cdist/novas.c
+-rw-r-----   0 brandon   (1000) brandon   (1000)    16671 2019-07-19 14:44:08.000000 novas-3.1.1.6/Cdist/novas.h
+-rw-r-----   0 brandon   (1000) brandon   (1000)     2324 2019-07-19 14:44:08.000000 novas-3.1.1.6/Cdist/novascon.c
+-rw-r-----   0 brandon   (1000) brandon   (1000)     2016 2019-07-19 14:44:08.000000 novas-3.1.1.6/Cdist/novascon.h
+-rw-r-----   0 brandon   (1000) brandon   (1000)   236927 2019-07-19 14:44:08.000000 novas-3.1.1.6/Cdist/nutation.c
+-rw-r-----   0 brandon   (1000) brandon   (1000)      652 2019-07-19 14:44:08.000000 novas-3.1.1.6/Cdist/nutation.h
+-rw-r-----   0 brandon   (1000) brandon   (1000)     2567 2019-07-19 14:44:08.000000 novas-3.1.1.6/Cdist/readeph0.c
+-rw-r-----   0 brandon   (1000) brandon   (1000)      642 2019-07-19 14:44:08.000000 novas-3.1.1.6/Cdist/solarsystem.h
+-rw-r-----   0 brandon   (1000) brandon   (1000)     8922 2019-07-19 14:44:08.000000 novas-3.1.1.6/Cdist/solsys1.c
+-rw-r-----   0 brandon   (1000) brandon   (1000)       57 2019-07-19 14:44:08.000000 novas-3.1.1.6/MANIFEST.in
+-rw-r--r--   0 brandon   (1000) brandon   (1000)    11522 2024-04-27 12:02:03.976591 novas-3.1.1.6/PKG-INFO
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)    10257 2024-04-27 12:00:33.000000 novas-3.1.1.6/README-PyPI
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)     5779 2021-01-05 13:02:13.000000 novas-3.1.1.6/README.rst
+-rwxr-x---   0 brandon   (1000) brandon   (1000)     4323 2019-07-19 14:44:08.000000 novas-3.1.1.6/asc2eph.py
+drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2024-04-27 12:02:03.972592 novas-3.1.1.6/compat/
+-rw-r-----   0 brandon   (1000) brandon   (1000)       59 2019-07-19 14:44:08.000000 novas-3.1.1.6/compat/__init__.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)   161115 2020-11-13 00:40:24.000000 novas-3.1.1.6/compat/compat.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)    11058 2019-07-19 14:44:08.000000 novas-3.1.1.6/compat/eph_manager.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     4596 2019-07-19 14:44:08.000000 novas-3.1.1.6/compat/nutation.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)        0 2019-07-19 14:44:08.000000 novas-3.1.1.6/compat/readeph0.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     6625 2019-07-19 14:44:08.000000 novas-3.1.1.6/compat/solsys.py
+drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2024-04-27 12:02:03.972592 novas-3.1.1.6/novas.egg-info/
+-rw-r--r--   0 brandon   (1000) brandon   (1000)    11522 2024-04-27 12:02:03.000000 novas-3.1.1.6/novas.egg-info/PKG-INFO
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)      633 2024-04-27 12:02:03.000000 novas-3.1.1.6/novas.egg-info/SOURCES.txt
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)        1 2024-04-27 12:02:03.000000 novas-3.1.1.6/novas.egg-info/dependency_links.txt
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)        6 2024-04-27 12:02:03.000000 novas-3.1.1.6/novas.egg-info/top_level.txt
+drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2024-04-27 12:02:03.972592 novas-3.1.1.6/novas_py/
+-rw-r-----   0 brandon   (1000) brandon   (1000)     2086 2019-07-19 14:44:08.000000 novas-3.1.1.6/novas_py/__init__.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     1646 2019-07-19 14:44:08.000000 novas-3.1.1.6/novas_py/constants.py
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)       38 2024-04-27 12:02:03.976591 novas-3.1.1.6/setup.cfg
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)     8111 2024-04-27 11:49:58.000000 novas-3.1.1.6/setup.py
+drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2024-04-27 12:02:03.972592 novas-3.1.1.6/tests/
+-rw-r-----   0 brandon   (1000) brandon   (1000)        0 2019-07-19 14:44:08.000000 novas-3.1.1.6/tests/__init__.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     1080 2019-07-19 14:44:08.000000 novas-3.1.1.6/tests/checkout-stars-full.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)    48109 2019-07-19 14:44:08.000000 novas-3.1.1.6/tests/test_compat.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     8210 2019-07-19 14:44:08.000000 novas-3.1.1.6/tests/test_example.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     1309 2019-07-19 14:44:08.000000 novas-3.1.1.6/tests/test_github_issues.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `novas-3.1.1.5/Cdist/eph_manager.c` & `novas-3.1.1.6/Cdist/eph_manager.c`

 * *Files identical despite different names*

### Comparing `novas-3.1.1.5/Cdist/eph_manager.h` & `novas-3.1.1.6/Cdist/eph_manager.h`

 * *Files identical despite different names*

### Comparing `novas-3.1.1.5/Cdist/novas.c` & `novas-3.1.1.6/Cdist/novas.c`

 * *Files identical despite different names*

### Comparing `novas-3.1.1.5/Cdist/novas.h` & `novas-3.1.1.6/Cdist/novas.h`

 * *Files identical despite different names*

### Comparing `novas-3.1.1.5/Cdist/novascon.c` & `novas-3.1.1.6/Cdist/novascon.c`

 * *Files identical despite different names*

### Comparing `novas-3.1.1.5/Cdist/novascon.h` & `novas-3.1.1.6/Cdist/novascon.h`

 * *Files identical despite different names*

### Comparing `novas-3.1.1.5/Cdist/nutation.c` & `novas-3.1.1.6/Cdist/nutation.c`

 * *Files identical despite different names*

### Comparing `novas-3.1.1.5/Cdist/nutation.h` & `novas-3.1.1.6/Cdist/nutation.h`

 * *Files identical despite different names*

### Comparing `novas-3.1.1.5/Cdist/readeph0.c` & `novas-3.1.1.6/Cdist/readeph0.c`

 * *Files identical despite different names*

### Comparing `novas-3.1.1.5/Cdist/solarsystem.h` & `novas-3.1.1.6/Cdist/solarsystem.h`

 * *Files identical despite different names*

### Comparing `novas-3.1.1.5/Cdist/solsys1.c` & `novas-3.1.1.6/Cdist/solsys1.c`

 * *Files identical despite different names*

### Comparing `novas-3.1.1.5/README` & `novas-3.1.1.6/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 ###################
 Welcome to NOVAS Py
 ###################
 
+.. important::
+
+   This GitHub repository is merely a mirror of this official United
+   States Naval Observatory software library, with the code tweaked to
+   make possible its release on the Python Package Index as the `novas
+   package`_.  None of the library’s actual authors are involved with
+   this repository.  Its official documentation is here:
+
+   * `User’s Guide to NOVAS`_
+
 What is NOVAS?
 ==============
 
 NOVAS is an integrated package of functions for computing various
 commonly needed quantities in positional astronomy. The package can
 supply, in one or two function calls, the instantaneous coordinates of
 any star or solar system body in a variety of coordinate systems.  At a
@@ -19,15 +29,15 @@
 
 What is NOVAS Py?
 =================
 
 With NOVAS Py, the USNO is expanding NOVAS to the Python programming
 language. The NOVAS Py module is simply a wrapper around the NOVAS C code;
 *all computations are still performed by the C code*. NOVAS Py makes use of
-Python's `ctypes module`_.
+Python's `ctypes`_ module.
 
 Installation
 ============
 
 The NOVAS Py Module
 -------------------
 
@@ -105,15 +115,17 @@
 Using NOVAS Py
 ==============
 
 Once installation is complete, the NOVAS functions can be found under
 the ``novas.compat`` namespace. Nutation models can be found under
 ``novas.nutation``, and constants under ``novas.constants``.
 
+.. _novas package: https://pypi.org/project/novas/
+.. _User’s Guide to NOVAS: https://github.com/brandon-rhodes/python-novas/raw/master/Cdist/NOVAS_C3.1_Guide.pdf
 .. _precession: http://asa.usno.navy.mil/SecM/Glossary.html#precession
 .. _nutation: http://asa.usno.navy.mil/SecM/Glossary.html#nutation
 .. _aberration: http://asa.usno.navy.mil/SecM/Glossary.html#aberration
 .. _parallax: http://asa.usno.navy.mil/SecM/Glossary.html#parallax
 .. _deflection of light: http://asa.usno.navy.mil/SecM/Glossary.html#deflection-light
 .. _ctypes: https://docs.python.org/3.4/library/ctypes.html
 .. _webpage: http://ssd.jpl.nasa.gov/?planet_eph_export
-.. _unittest2 module: http://pypi.python.org/pypi/unittest2
+.. _unittest2 module: https://pypi.org/project/unittest2/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `novas-3.1.1.5/README-PyPI` & `novas-3.1.1.6/README-PyPI`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+
+Welcome
+-------
+
+This is United States Naval Observatory software, which they have
+happily made available for use by the public.
+
+It has been packaged and released on PyPI by `Brandon Rhodes`_ to make
+it easier to install, built from a `GitHub repository`_ mirror of the
+project’s original source code.  None of the library’s actual authors
+are involved with the repository or package; their work is released only
+through the official `NOVAS home page`_ and their official documentation
+is the `User’s Guide to NOVAS`_ PDF.
+
 What is NOVAS?
 --------------
 
 NOVAS is an integrated package of functions for computing various
 commonly needed quantities in positional astronomy.  The package can
 supply, in one or two function calls, the instantaneous coordinates of
 any star or solar system body in a variety of coordinate systems.  At a
@@ -15,33 +29,32 @@
 
 This Python package includes both the NOVAS library and the Python
 wrapper that are available from the `NOVAS home page`_ at the United
 States Naval Observatory.  This version includes a few bug fixes and
 packaging adjustments that are not in the most recent June 2011
 release of the software from the Naval Observatory itself.  You can
 find these changes described at the bottom of this page in the
-Changelog, and you can also review them yourself at the `project
-repository on GitHub`_.
-
-This package has been uploaded to the Python Package Index by Brandon
-Rhodes <brandon@rhodesmill.org>.  Please contact me, and not the busy
-folks at the Naval Observatory, about any problems you encounter when
-trying to install it — any problems with how it has been packaged are
-my fault, not theirs!  For questions about how to use the library, you
-can also ask for help on Stack Overflow, where I watch for questions
-that involve Python and astronomy.
+Changelog, and you can also review them yourself at the
+`GitHub repository`_.
 
 Quick Examples
 --------------
 
-Importing the library and opening the planetary ephemeris:
+You can download planetary ephemerides from several sources online,
+including:
+
+* `https://naif.jpl.nasa.gov/pub/naif/generic_kernels/spk/planets/ <https://naif.jpl.nasa.gov/pub/naif/generic_kernels/spk/planets/>`_
+* `https://naif.jpl.nasa.gov/pub/naif/generic_kernels/spk/planets/a_old_versions/ <https://naif.jpl.nasa.gov/pub/naif/generic_kernels/spk/planets/a_old_versions/>`_
+
+You can then import the NOVAS Python library and open a planetary
+ephemeris with:
 
 >>> from novas import compat as novas
 >>> from novas.compat import eph_manager
->>> jd_start, jd_end, number = eph_manager.ephem_open()
+>>> jd_start, jd_end, number = eph_manager.ephem_open('de421.bsp')
 
 Converting a calendar date to a Julian date:
 
 >>> jd_tt = novas.julian_date(2012, 10, 2, 12.0)
 >>> jd_tt
 2456203.0
 
@@ -140,19 +153,31 @@
 
 You can find more information and documentation on the project's
 official `NOVAS home page`_ at the Naval Observatory.
 
 Changelog
 ---------
 
-Version 3.1.1.4 — 2016 December 1
+Version 3.1.1.6 — 2024 April 27
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+* Declare compatibility with Python versions through Python 3.12.
+
+* Add ``arm64`` to compile arguments, to support Apple’s M1 platform.
+
+* Fix: ``equ2hor()`` docstring said that ``dec`` argument should be in
+  hours, whereas it should, in fact, be in degrees.
+
+Version 3.1.1.5 — 2016 December 1
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-* Updated all source code with improvements and rewrites from the new
-  official version 3.1.1 from the Naval Observatory.
+* Declare compatibility with Python versions through Python 3.7.
+
+* Fix: ``cel_pole()`` now correctly limits its ``type`` argument to the
+  integers 1 and 2, rather than the integers 0 and 1.
 
 Version 3.1.1.3 — 2015 January 23
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 * Fixed a fatal typo in ``astro_star()`` that caused it to always raise
   ``ArgumentError: argument 3: <class 'TypeError'>: wrong type``
 
@@ -190,16 +215,15 @@
 * Python code can now access the ``ephem_close()`` routine inside the
   ``eph_manager`` module.
 * Bugfix: the ``eph_manager.state()`` function was always raising an
   exception if invoked.
 * Bugfix: to ``eph_manager.c`` as recommended in the `NOVAS FAQ`_.
 * Bugfix: to ``novas.c`` as recommended in the `NOVAS FAQ`_.
 
-To examine the code changes yourself, you can visit the `project
-repository on GitHub`_.
+To examine the code changes yourself, visit the `GitHub repository`_.
 
 Version 3.1 — 2012 September 19
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Initial release of the library on the Python Package Index.
 
 License and Citation
@@ -225,8 +249,10 @@
 .. _aberration: http://asa.usno.navy.mil/SecM/Glossary.html#aberration
 .. _parallax: http://asa.usno.navy.mil/SecM/Glossary.html#parallax
 .. _deflection of light: http://asa.usno.navy.mil/SecM/Glossary.html#deflection-light
 .. _webpage: http://ssd.jpl.nasa.gov/?planet_eph_export
 .. _unittest2 module: http://pypi.python.org/pypi/unittest2
 .. _NOVAS home page: http://aa.usno.navy.mil/software/novas/novas_py/novaspy_intro.php
 .. _NOVAS FAQ: http://aa.usno.navy.mil/software/novas/novas_faq.php
-.. _project repository on GitHub: https://github.com/brandon-rhodes/python-novas
+.. _GitHub repository: https://github.com/brandon-rhodes/python-novas
+.. _User’s Guide to NOVAS: https://github.com/brandon-rhodes/python-novas/raw/master/Cdist/NOVAS_C3.1_Guide.pdf
+.. _Brandon Rhodes: https://rhodesmill.org/brandon/
```

### Comparing `novas-3.1.1.5/asc2eph.py` & `novas-3.1.1.6/asc2eph.py`

 * *Files identical despite different names*

### Comparing `novas-3.1.1.5/compat/compat.py` & `novas-3.1.1.6/compat/compat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1239,15 +1239,15 @@
     location : OnSurface
         Instance of OnSurface type object containing observer's
         location.
     ra : float
         Topocentric right ascension of object of interest, in hours,
         referred to true equator and equinox of date.
     dec : float
-        Topocentric declination of object of interest, in hours,
+        Topocentric declination of object of interest, in degrees,
         referred to true equator and equinox of date.
     ref_option : {0, 1, 2}, optional
             = 0 ... no refraction (default)
             = 1 ... include refraction, using 'standard' atmospheric
                 conditions.
             = 2 ... include refraction, using atmospheric parameters
                 input in the 'location' object.
```

### Comparing `novas-3.1.1.5/compat/eph_manager.py` & `novas-3.1.1.6/compat/eph_manager.py`

 * *Files identical despite different names*

### Comparing `novas-3.1.1.5/compat/nutation.py` & `novas-3.1.1.6/compat/nutation.py`

 * *Files identical despite different names*

### Comparing `novas-3.1.1.5/compat/solsys.py` & `novas-3.1.1.6/compat/solsys.py`

 * *Files identical despite different names*

### Comparing `novas-3.1.1.5/novas_py/__init__.py` & `novas-3.1.1.6/novas_py/__init__.py`

 * *Files identical despite different names*

### Comparing `novas-3.1.1.5/novas_py/constants.py` & `novas-3.1.1.6/novas_py/constants.py`

 * *Files identical despite different names*

### Comparing `novas-3.1.1.5/setup.py` & `novas-3.1.1.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -132,14 +132,15 @@
         novaslib = [(
             'novas', {
                 'package': 'novas',
                 'sources': c_sources,
                 'include_dirs': ['Cdist'],
                 'extra_compile_args': ['-arch', 'i386',
                                        '-arch', 'x86_64',
+                                       '-arch', 'arm64',
                                        '-O2', '-Wall', '-fPIC']
             }
         )]
     elif 'windows' in system:
         raise OSError("Operating system not supported at this time")
     else:
         novaslib = [(
@@ -175,14 +176,19 @@
             'Operating System :: POSIX :: Linux',
             'Programming Language :: Python :: 2.7',
             'Programming Language :: Python :: 3.3',
             'Programming Language :: Python :: 3.4',
             'Programming Language :: Python :: 3.5',
             'Programming Language :: Python :: 3.6',
             'Programming Language :: Python :: 3.7',
+            'Programming Language :: Python :: 3.8',
+            'Programming Language :: Python :: 3.9',
+            'Programming Language :: Python :: 3.10',
+            'Programming Language :: Python :: 3.11',
+            'Programming Language :: Python :: 3.12',
             'Topic :: Scientific/Engineering :: Astronomy',
         ],
 
         'packages': ['novas', 'novas.compat'],
         'package_dir': {
             'novas': 'novas_py',
             'novas.compat': 'compat'
@@ -191,15 +197,15 @@
         'cmdclass': {
             'build_clib': build_dynamic_clib,
         }
     }
 
     # Begin customizations by Brandon Rhodes for release on PyPI
     options['name'] = 'novas'
-    options['version'] = '3.1.1.5'
+    options['version'] = '3.1.1.6'
     options['description'] = ('The United States Naval Observatory'
                               ' NOVAS astronomy library')
     options['long_description'] = (codecs.open('README-PyPI', 'r', 'utf-8')
                                    .read())
     options['maintainer'] = (options['author'] +
                              '; packaged for PyPI by Brandon Rhodes')
     options['maintainer_email'] = 'brandon@rhodesmill.org'
```

### Comparing `novas-3.1.1.5/tests/checkout-stars-full.py` & `novas-3.1.1.6/tests/checkout-stars-full.py`

 * *Files identical despite different names*

### Comparing `novas-3.1.1.5/tests/test_compat.py` & `novas-3.1.1.6/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `novas-3.1.1.5/tests/test_example.py` & `novas-3.1.1.6/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `novas-3.1.1.5/tests/test_github_issues.py` & `novas-3.1.1.6/tests/test_github_issues.py`

 * *Files identical despite different names*

