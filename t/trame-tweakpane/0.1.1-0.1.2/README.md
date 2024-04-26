# Comparing `tmp/trame_tweakpane-0.1.1.tar.gz` & `tmp/trame_tweakpane-0.1.2.tar.gz`

## Comparing `trame_tweakpane-0.1.1.tar` & `trame_tweakpane-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.1/examples/readme_example.py
--rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.1/examples/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.1/tests/test_import.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.1/trame/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.1/trame/modules/__init__.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.1/trame/modules/tweakpane.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.1/trame/widgets/__init__.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.1/trame/widgets/tweakpane.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.1/trame_tweakpane/__init__.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.1/trame_tweakpane/module/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.1/trame_tweakpane/widgets/__init__.py
--rw-r--r--   0        0        0     8543 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.1/trame_tweakpane/widgets/tweakpane.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.1/LICENSE
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.1/README.rst
--rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.2/examples/readme_example.py
+-rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.2/examples/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.2/tests/test_import.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.2/trame/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.2/trame/modules/__init__.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.2/trame/modules/tweakpane.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.2/trame/widgets/__init__.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.2/trame/widgets/tweakpane.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.2/trame_tweakpane/__init__.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.2/trame_tweakpane/module/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.2/trame_tweakpane/widgets/__init__.py
+-rw-r--r--   0        0        0     8543 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.2/trame_tweakpane/widgets/tweakpane.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.2/README.rst
+-rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 trame_tweakpane-0.1.2/PKG-INFO
```

### Comparing `trame_tweakpane-0.1.1/examples/readme_example.py` & `trame_tweakpane-0.1.2/examples/readme_example.py`

 * *Files identical despite different names*

### Comparing `trame_tweakpane-0.1.1/examples/simple.py` & `trame_tweakpane-0.1.2/examples/simple.py`

 * *Files identical despite different names*

### Comparing `trame_tweakpane-0.1.1/trame_tweakpane/widgets/tweakpane.py` & `trame_tweakpane-0.1.2/trame_tweakpane/widgets/tweakpane.py`

 * *Files identical despite different names*

### Comparing `trame_tweakpane-0.1.1/LICENSE` & `trame_tweakpane-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trame_tweakpane-0.1.1/README.rst` & `trame_tweakpane-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `trame_tweakpane-0.1.1/pyproject.toml` & `trame_tweakpane-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "trame-tweakpane"
-version = "0.1.1"
+version = "0.1.2"
 requires-python = ">= 3.7"
 dependencies = [
   "trame-client",
 ]
 
 authors = [
   {name = "Sebastien Jourdain", email = "sebastien.jourdain@kitware.com"},
```

### Comparing `trame_tweakpane-0.1.1/PKG-INFO` & `trame_tweakpane-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: trame-tweakpane
-Version: 0.1.1
+Version: 0.1.2
 Summary: TweakPane widgets for trame
 Author-email: Sebastien Jourdain <sebastien.jourdain@kitware.com>
 Maintainer-email: Sebastien Jourdain <sebastien.jourdain@kitware.com>
 License: MIT License
         
         Copyright (c) 2024, Kitware Inc.
```

