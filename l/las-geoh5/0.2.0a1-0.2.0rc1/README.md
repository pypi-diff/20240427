# Comparing `tmp/las_geoh5-0.2.0a1.tar.gz` & `tmp/las_geoh5-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "las_geoh5-0.2.0a1.tar", max compression
+gzip compressed data, was "las_geoh5-0.2.0rc1.tar", max compression
```

## Comparing `las_geoh5-0.2.0a1.tar` & `las_geoh5-0.2.0rc1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      291 2024-04-23 17:07:21.289948 las_geoh5-0.2.0a1/las_geoh5/__init__.py
--rw-r--r--   0        0        0      240 2024-04-23 17:07:21.289948 las_geoh5-0.2.0a1/las_geoh5/export_files/__init__.py
--rw-r--r--   0        0        0     1734 2024-04-23 17:07:21.289948 las_geoh5-0.2.0a1/las_geoh5/export_files/driver.py
--rw-r--r--   0        0        0     1264 2024-04-23 17:07:21.289948 las_geoh5-0.2.0a1/las_geoh5/export_files/uijson.py
--rw-r--r--   0        0        0     6748 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5/export_las.py
--rw-r--r--   0        0        0      240 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5/import_directories/__init__.py
--rw-r--r--   0        0        0     2104 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5/import_directories/driver.py
--rw-r--r--   0        0        0     1057 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5/import_directories/uijson.py
--rw-r--r--   0        0        0      240 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5/import_files/__init__.py
--rw-r--r--   0        0        0     4632 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5/import_files/driver.py
--rw-r--r--   0        0        0     1468 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5/import_files/params.py
--rw-r--r--   0        0        0     3080 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5/import_files/uijson.py
--rw-r--r--   0        0        0    13319 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5/import_las.py
--rw-r--r--   0        0        0      122 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5/uijson/__init__.py
--rw-r--r--   0        0        0     2119 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5/uijson/write_uijson.py
--rw-r--r--   0        0        0      122 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5_assets/__init__.py
--rw-r--r--   0        0        0     1112 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5_assets/uijson/export_las_files.ui.json
--rw-r--r--   0        0        0      974 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5_assets/uijson/import_las_directories.ui.json
--rw-r--r--   0        0        0     2656 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5_assets/uijson/import_las_files.ui.json
--rw-r--r--   0        0        0     1093 2024-04-23 17:07:21.274278 las_geoh5-0.2.0a1/LICENSE.txt
--rw-r--r--   0        0        0     2262 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0     4962 2024-04-23 17:07:21.274278 las_geoh5-0.2.0a1/README.rst
--rw-r--r--   0        0        0     5980 1970-01-01 00:00:00.000000 las_geoh5-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0      702 2024-04-27 20:37:43.194475 las_geoh5-0.2.0rc1/las_geoh5/__init__.py
+-rw-r--r--   0        0        0      240 2024-04-23 21:10:39.081155 las_geoh5-0.2.0rc1/las_geoh5/export_files/__init__.py
+-rw-r--r--   0        0        0     1734 2024-04-23 21:10:39.082255 las_geoh5-0.2.0rc1/las_geoh5/export_files/driver.py
+-rw-r--r--   0        0        0     1264 2024-04-23 21:11:17.349111 las_geoh5-0.2.0rc1/las_geoh5/export_files/uijson.py
+-rw-r--r--   0        0        0     6748 2024-04-23 21:11:17.349111 las_geoh5-0.2.0rc1/las_geoh5/export_las.py
+-rw-r--r--   0        0        0      240 2024-04-23 21:10:39.083315 las_geoh5-0.2.0rc1/las_geoh5/import_directories/__init__.py
+-rw-r--r--   0        0        0     2104 2024-04-23 21:10:39.083315 las_geoh5-0.2.0rc1/las_geoh5/import_directories/driver.py
+-rw-r--r--   0        0        0     1057 2024-04-23 21:10:39.084314 las_geoh5-0.2.0rc1/las_geoh5/import_directories/uijson.py
+-rw-r--r--   0        0        0      240 2024-04-23 21:10:39.084314 las_geoh5-0.2.0rc1/las_geoh5/import_files/__init__.py
+-rw-r--r--   0        0        0     4632 2024-04-23 21:10:39.085372 las_geoh5-0.2.0rc1/las_geoh5/import_files/driver.py
+-rw-r--r--   0        0        0     1468 2024-04-23 21:10:39.085372 las_geoh5-0.2.0rc1/las_geoh5/import_files/params.py
+-rw-r--r--   0        0        0     3080 2024-04-23 21:10:39.085372 las_geoh5-0.2.0rc1/las_geoh5/import_files/uijson.py
+-rw-r--r--   0        0        0    13319 2024-04-23 21:10:39.086374 las_geoh5-0.2.0rc1/las_geoh5/import_las.py
+-rw-r--r--   0        0        0      122 2024-04-23 21:10:39.086374 las_geoh5-0.2.0rc1/las_geoh5/uijson/__init__.py
+-rw-r--r--   0        0        0     2119 2024-04-23 21:10:39.086374 las_geoh5-0.2.0rc1/las_geoh5/uijson/write_uijson.py
+-rw-r--r--   0        0        0      122 2024-04-23 21:10:39.087480 las_geoh5-0.2.0rc1/las_geoh5-assets/__init__.py
+-rw-r--r--   0        0        0     1112 2024-04-23 21:11:17.350225 las_geoh5-0.2.0rc1/las_geoh5-assets/uijson/export_las_files.ui.json
+-rw-r--r--   0        0        0      974 2024-04-23 21:10:39.088503 las_geoh5-0.2.0rc1/las_geoh5-assets/uijson/import_las_directories.ui.json
+-rw-r--r--   0        0        0     2656 2024-04-23 21:11:17.350225 las_geoh5-0.2.0rc1/las_geoh5-assets/uijson/import_las_files.ui.json
+-rw-r--r--   0        0        0     1093 2024-04-23 21:10:39.080154 las_geoh5-0.2.0rc1/LICENSE.txt
+-rw-r--r--   0        0        0     2591 2024-04-27 20:40:58.445160 las_geoh5-0.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     4992 2024-04-26 06:14:29.001844 las_geoh5-0.2.0rc1/README.rst
+-rw-r--r--   0        0        0     6011 1970-01-01 00:00:00.000000 las_geoh5-0.2.0rc1/PKG-INFO
```

### Comparing `las_geoh5-0.2.0a1/las_geoh5/export_files/driver.py` & `las_geoh5-0.2.0rc1/las_geoh5/export_files/driver.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0a1/las_geoh5/export_files/uijson.py` & `las_geoh5-0.2.0rc1/las_geoh5/export_files/uijson.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0a1/las_geoh5/export_las.py` & `las_geoh5-0.2.0rc1/las_geoh5/export_las.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0a1/las_geoh5/import_directories/driver.py` & `las_geoh5-0.2.0rc1/las_geoh5/import_directories/driver.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0a1/las_geoh5/import_directories/uijson.py` & `las_geoh5-0.2.0rc1/las_geoh5/import_directories/uijson.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0a1/las_geoh5/import_files/driver.py` & `las_geoh5-0.2.0rc1/las_geoh5/import_files/driver.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0a1/las_geoh5/import_files/params.py` & `las_geoh5-0.2.0rc1/las_geoh5/import_files/params.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0a1/las_geoh5/import_files/uijson.py` & `las_geoh5-0.2.0rc1/las_geoh5/import_files/uijson.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0a1/las_geoh5/import_las.py` & `las_geoh5-0.2.0rc1/las_geoh5/import_las.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0a1/las_geoh5/uijson/write_uijson.py` & `las_geoh5-0.2.0rc1/las_geoh5/uijson/write_uijson.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0a1/las_geoh5_assets/uijson/export_las_files.ui.json` & `las_geoh5-0.2.0rc1/las_geoh5-assets/uijson/export_las_files.ui.json`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0a1/las_geoh5_assets/uijson/import_las_directories.ui.json` & `las_geoh5-0.2.0rc1/las_geoh5-assets/uijson/import_las_directories.ui.json`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0a1/las_geoh5_assets/uijson/import_las_files.ui.json` & `las_geoh5-0.2.0rc1/las_geoh5-assets/uijson/import_las_files.ui.json`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0a1/LICENSE.txt` & `las_geoh5-0.2.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0a1/pyproject.toml` & `las_geoh5-0.2.0rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 [tool.poetry]
 name = "las-geoh5"
-version = "0.2.0-alpha.1"
+version = "0.2.0-rc.1"
 description = "Las/Geoh5 conversion"
 license = "MIT"
 readme = "README.rst"
 homepage = "https://mirageoscience.com"
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
 keywords = ["geology", "geophysics", "earth sciences", "io", "data", "interoperability"]
+
 packages = [
     { include = "las_geoh5" },
-    { include = "las_geoh5_assets" },
+    { include = "las_geoh5-assets" },
+]
+
+include = [
+    "COPYING",
+    "COPYING.LESSER",
+    "LICENSE",
+    "README.rst",
+    "THIRD_PARTY_SOFTWARE.rst",
 ]
+
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Physics",
@@ -23,25 +33,28 @@
     "Operating System :: Unix",
     "Operating System :: MacOS",
     "Natural Language :: English",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10, <3.11"
-pydantic = "~2.5"
 
-## dependencies on github repos
-#geoh5py = {git = "https://github.com/MiraGeoscience/geoh5py.git", branch = "release/0.9.0"}
-geoh5py = {version ="~0.9.0-alpha.4", allow-prereleases = true}
-
-## pip dependencies
 lasio = "~0.31"
-tqdm = "^4.64.0"
+pydantic = "~2.5.2"
+tqdm = "^4.66.1"
+
+## dependencies from Git repositories
+#------------------------------------
+geoh5py = {version ="~0.9.0rc1", allow-prereleases = true}
+#geoh5py = {git = "https://github.com/MiraGeoscience/geoh5py.git", branch = "release/0.9.0"}
+#geoh5py = {url = "https://github.com/MiraGeoscience/geoh5py/archive/refs/heads/release/0.9.0.zip#sha256="}
+#geoh5py = {url = "http://localhost:8888/geoh5py.tar.gz#sha256="}
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+Pygments = "*"
 pylint = "*"
 pytest = "*"
 pytest-cov = "*"
 tomli = "*"
 sphinx = "*"
 sphinx-autodoc-typehints = "*"
 sphinx-rtd-theme = "*"
@@ -62,15 +75,15 @@
 ignore_missing_imports = true
 scripts_are_modules = true
 show_error_context = true
 show_column_numbers = true
 check_untyped_defs = true
 
 plugins = [
-    #    'numpy.typing.mypy_plugin'
+    "pydantic.mypy"
 ]
 
 [tool.coverage.run]
 branch = true
 source = ["las_geoh5"]
 omit = []
```

### Comparing `las_geoh5-0.2.0a1/README.rst` & `las_geoh5-0.2.0rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 |coverage| |maintainability| |precommit_ci| |docs| |style| |version| |status| |pyversions|
 
 
-.. |docs| image:: https://readthedocs.org/projects/las-geoh5/badge/
+.. |docs| image:: https://readthedocs.com/projects/mirageoscience-las-geoh5/badge/?version=latest
     :alt: Documentation Status
-    :target: https://las-geoh5.readthedocs.io/en/latest/?badge=latest
+    :target: https://mirageoscience-las-geoh5.readthedocs-hosted.com/en/latest/?badge=latest
 
 .. |coverage| image:: https://codecov.io/gh/MiraGeoscience/las-geoh5/branch/develop/graph/badge.svg
     :alt: Code coverage
     :target: https://codecov.io/gh/MiraGeoscience/las-geoh5
 
 .. |style| image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :alt: Coding style
@@ -46,23 +46,22 @@
 
 .. contents:: Table of Contents
    :local:
    :depth: 3
 
 Documentation
 -------------
-`Online documentation <https://las-geoh5.readthedocs.io/en/latest/>`_
+`Online documentation <https://mirageoscience-las-geoh5.readthedocs-hosted.com/en/latest/>`_
 
 
 Install with PyPI
 -----------------
 
 Since las-geoh5 is a small package with only a few dependencies, we recommend installing
-w
-Still, you can install it in a conda environment without its dependencies (``--no-deps``).
+with the Python package index (PyPI) using pip.
 
 From PyPI
 ~~~~~~~~~
 
 To install the **las-geoh5** package published on PyPI:
 
 .. code-block:: bash
```

### Comparing `las_geoh5-0.2.0a1/PKG-INFO` & `las_geoh5-0.2.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: las-geoh5
-Version: 0.2.0a1
+Version: 0.2.0rc1
 Summary: Las/Geoh5 conversion
 Home-page: https://mirageoscience.com
 License: MIT
 Keywords: geology,geophysics,earth sciences,io,data,interoperability
 Author: Mira Geoscience
 Author-email: support@mirageoscience.com
 Requires-Python: >=3.10,<3.11
@@ -18,26 +18,26 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Dist: geoh5py (>=0.9.0-alpha.4,<0.10.0)
+Requires-Dist: geoh5py (>=0.9.0rc1,<0.10.0)
 Requires-Dist: lasio (>=0.31,<0.32)
-Requires-Dist: pydantic (>=2.5,<2.6)
-Requires-Dist: tqdm (>=4.64.0,<5.0.0)
+Requires-Dist: pydantic (>=2.5.2,<2.6.0)
+Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Description-Content-Type: text/x-rst
 
 |coverage| |maintainability| |precommit_ci| |docs| |style| |version| |status| |pyversions|
 
 
-.. |docs| image:: https://readthedocs.org/projects/las-geoh5/badge/
+.. |docs| image:: https://readthedocs.com/projects/mirageoscience-las-geoh5/badge/?version=latest
     :alt: Documentation Status
-    :target: https://las-geoh5.readthedocs.io/en/latest/?badge=latest
+    :target: https://mirageoscience-las-geoh5.readthedocs-hosted.com/en/latest/?badge=latest
 
 .. |coverage| image:: https://codecov.io/gh/MiraGeoscience/las-geoh5/branch/develop/graph/badge.svg
     :alt: Code coverage
     :target: https://codecov.io/gh/MiraGeoscience/las-geoh5
 
 .. |style| image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :alt: Coding style
@@ -76,23 +76,22 @@
 
 .. contents:: Table of Contents
    :local:
    :depth: 3
 
 Documentation
 -------------
-`Online documentation <https://las-geoh5.readthedocs.io/en/latest/>`_
+`Online documentation <https://mirageoscience-las-geoh5.readthedocs-hosted.com/en/latest/>`_
 
 
 Install with PyPI
 -----------------
 
 Since las-geoh5 is a small package with only a few dependencies, we recommend installing
-w
-Still, you can install it in a conda environment without its dependencies (``--no-deps``).
+with the Python package index (PyPI) using pip.
 
 From PyPI
 ~~~~~~~~~
 
 To install the **las-geoh5** package published on PyPI:
 
 .. code-block:: bash
```

