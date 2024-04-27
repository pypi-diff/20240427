# Comparing `tmp/astroconst-0.0.8.tar.gz` & `tmp/astroconst-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astroconst-0.0.8.tar", last modified: Mon Sep 18 19:20:10 2023, max compression
+gzip compressed data, was "astroconst-0.0.9.tar", last modified: Sun Oct  8 15:41:04 2023, max compression
```

## Comparing `astroconst-0.0.8.tar` & `astroconst-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2023-09-18 19:20:10.226483 astroconst-0.0.8/
--rw-r--r--   0 sluys     (1000) sluys     (1000)    13827 2022-01-04 18:50:46.000000 astroconst-0.0.8/LICENCE
--rw-r--r--   0 sluys     (1000) sluys     (1000)     4034 2023-09-18 19:20:10.226483 astroconst-0.0.8/PKG-INFO
--rw-r--r--   0 sluys     (1000) sluys     (1000)     3128 2022-01-09 16:53:51.000000 astroconst-0.0.8/README.md
-drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2023-09-18 19:20:10.226483 astroconst-0.0.8/astroconst/
--rw-r--r--   0 sluys     (1000) sluys     (1000)    14811 2023-09-18 13:56:34.000000 astroconst-0.0.8/astroconst/__init__.py
--rw-r--r--   0 sluys     (1000) sluys     (1000)     9530 2023-01-30 10:58:23.000000 astroconst-0.0.8/astroconst/aa.py
-drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2023-09-18 19:20:10.226483 astroconst-0.0.8/astroconst.egg-info/
--rw-r--r--   0 sluys     (1000) sluys     (1000)     4034 2023-09-18 19:20:10.000000 astroconst-0.0.8/astroconst.egg-info/PKG-INFO
--rw-r--r--   0 sluys     (1000) sluys     (1000)      251 2023-09-18 19:20:10.000000 astroconst-0.0.8/astroconst.egg-info/SOURCES.txt
--rw-r--r--   0 sluys     (1000) sluys     (1000)        1 2023-09-18 19:20:10.000000 astroconst-0.0.8/astroconst.egg-info/dependency_links.txt
--rw-r--r--   0 sluys     (1000) sluys     (1000)        6 2023-09-18 19:20:10.000000 astroconst-0.0.8/astroconst.egg-info/requires.txt
--rw-r--r--   0 sluys     (1000) sluys     (1000)       11 2023-09-18 19:20:10.000000 astroconst-0.0.8/astroconst.egg-info/top_level.txt
--rw-r--r--   0 sluys     (1000) sluys     (1000)       87 2023-09-18 18:49:56.000000 astroconst-0.0.8/pyproject.toml
--rw-r--r--   0 sluys     (1000) sluys     (1000)      888 2023-09-18 19:20:10.227483 astroconst-0.0.8/setup.cfg
+drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2023-10-08 15:41:04.809876 astroconst-0.0.9/
+-rw-r--r--   0 sluys     (1000) sluys     (1000)    13827 2023-09-18 19:22:23.000000 astroconst-0.0.9/LICENCE
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     4131 2023-10-08 15:41:04.808876 astroconst-0.0.9/PKG-INFO
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     3128 2023-09-18 19:22:23.000000 astroconst-0.0.9/README.md
+drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2023-10-08 15:41:04.808876 astroconst-0.0.9/astroconst/
+-rw-r--r--   0 sluys     (1000) sluys     (1000)    14811 2023-09-18 19:22:23.000000 astroconst-0.0.9/astroconst/__init__.py
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     9530 2023-09-18 19:22:23.000000 astroconst-0.0.9/astroconst/aa.py
+drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2023-10-08 15:41:04.808876 astroconst-0.0.9/astroconst.egg-info/
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     4131 2023-10-08 15:41:04.000000 astroconst-0.0.9/astroconst.egg-info/PKG-INFO
+-rw-r--r--   0 sluys     (1000) sluys     (1000)      241 2023-10-08 15:41:04.000000 astroconst-0.0.9/astroconst.egg-info/SOURCES.txt
+-rw-r--r--   0 sluys     (1000) sluys     (1000)        1 2023-10-08 15:41:04.000000 astroconst-0.0.9/astroconst.egg-info/dependency_links.txt
+-rw-r--r--   0 sluys     (1000) sluys     (1000)        6 2023-10-08 15:41:04.000000 astroconst-0.0.9/astroconst.egg-info/requires.txt
+-rw-r--r--   0 sluys     (1000) sluys     (1000)        1 2023-10-08 15:41:04.000000 astroconst-0.0.9/astroconst.egg-info/top_level.txt
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     1198 2023-10-08 15:40:30.000000 astroconst-0.0.9/pyproject.toml
+-rw-r--r--   0 sluys     (1000) sluys     (1000)       38 2023-10-08 15:41:04.809876 astroconst-0.0.9/setup.cfg
```

### Comparing `astroconst-0.0.8/LICENCE` & `astroconst-0.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `astroconst-0.0.8/PKG-INFO` & `astroconst-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: astroconst
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python package that provides astronomical constants.
-Home-page: https://github.com/MarcvdSluys/AstroConst
-Author: Marc van der Sluys
+Author-email: Marc van der Sluys <git@vandersluys.nl>
 License: EUPL 1.2
+Project-URL: GitHub, https://github.com/MarcvdSluys/AstroConst
+Project-URL: ReadTheDocs, https://astroconst.readthedocs.io
 Keywords: constants,astronomy,physics,mathematics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Natural Language :: English
```

### Comparing `astroconst-0.0.8/README.md` & `astroconst-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `astroconst-0.0.8/astroconst/__init__.py` & `astroconst-0.0.9/astroconst/__init__.py`

 * *Files identical despite different names*

### Comparing `astroconst-0.0.8/astroconst/aa.py` & `astroconst-0.0.9/astroconst/aa.py`

 * *Files identical despite different names*

### Comparing `astroconst-0.0.8/astroconst.egg-info/PKG-INFO` & `astroconst-0.0.9/astroconst.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: astroconst
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python package that provides astronomical constants.
-Home-page: https://github.com/MarcvdSluys/AstroConst
-Author: Marc van der Sluys
+Author-email: Marc van der Sluys <git@vandersluys.nl>
 License: EUPL 1.2
+Project-URL: GitHub, https://github.com/MarcvdSluys/AstroConst
+Project-URL: ReadTheDocs, https://astroconst.readthedocs.io
 Keywords: constants,astronomy,physics,mathematics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Natural Language :: English
```

