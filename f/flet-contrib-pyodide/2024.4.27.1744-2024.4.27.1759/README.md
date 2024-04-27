# Comparing `tmp/flet_contrib_pyodide-2024.4.27.1744.tar.gz` & `tmp/flet_contrib_pyodide-2024.4.27.1759.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_contrib_pyodide-2024.4.27.1744.tar", max compression
+gzip compressed data, was "flet_contrib_pyodide-2024.4.27.1759.tar", max compression
```

## Comparing `flet_contrib_pyodide-2024.4.27.1744.tar` & `flet_contrib_pyodide-2024.4.27.1759.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2264 2024-04-27 17:43:13.492472 flet_contrib_pyodide-2024.4.27.1744/README.md
--rw-r--r--   0        0        0      664 2024-04-27 17:44:03.984907 flet_contrib_pyodide-2024.4.27.1744/pyproject.toml
--rw-r--r--   0        0        0      193 2024-04-27 17:43:13.492472 flet_contrib_pyodide-2024.4.27.1744/src/flet/__init__.py
--rw-r--r--   0        0        0       31 2024-04-27 17:43:13.492472 flet_contrib_pyodide-2024.4.27.1744/src/flet/canvas/__init__.py
--rw-r--r--   0        0        0     2169 2024-04-27 17:43:13.492472 flet_contrib_pyodide-2024.4.27.1744/src/flet/flet.py
--rw-r--r--   0        0        0       55 2024-04-27 17:43:13.492472 flet_contrib_pyodide-2024.4.27.1744/src/flet/matplotlib_chart.py
--rw-r--r--   0        0        0       47 2024-04-27 17:43:13.492472 flet_contrib_pyodide-2024.4.27.1744/src/flet/plotly_chart.py
--rw-r--r--   0        0        0     3581 2024-04-27 17:43:13.492472 flet_contrib_pyodide-2024.4.27.1744/src/flet/pyodide_connection.py
--rw-r--r--   0        0        0      103 2024-04-27 17:43:13.492472 flet_contrib_pyodide-2024.4.27.1744/src/flet/version.py
--rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 flet_contrib_pyodide-2024.4.27.1744/PKG-INFO
+-rw-r--r--   0        0        0     2264 2024-04-27 17:59:12.592626 flet_contrib_pyodide-2024.4.27.1759/README.md
+-rw-r--r--   0        0        0      664 2024-04-27 17:59:59.312775 flet_contrib_pyodide-2024.4.27.1759/pyproject.toml
+-rw-r--r--   0        0        0      193 2024-04-27 17:59:12.596626 flet_contrib_pyodide-2024.4.27.1759/src/flet/__init__.py
+-rw-r--r--   0        0        0       31 2024-04-27 17:59:12.596626 flet_contrib_pyodide-2024.4.27.1759/src/flet/canvas/__init__.py
+-rw-r--r--   0        0        0     2169 2024-04-27 17:59:12.596626 flet_contrib_pyodide-2024.4.27.1759/src/flet/flet.py
+-rw-r--r--   0        0        0       55 2024-04-27 17:59:12.596626 flet_contrib_pyodide-2024.4.27.1759/src/flet/matplotlib_chart.py
+-rw-r--r--   0        0        0       47 2024-04-27 17:59:12.596626 flet_contrib_pyodide-2024.4.27.1759/src/flet/plotly_chart.py
+-rw-r--r--   0        0        0     3581 2024-04-27 17:59:12.596626 flet_contrib_pyodide-2024.4.27.1759/src/flet/pyodide_connection.py
+-rw-r--r--   0        0        0      103 2024-04-27 17:59:12.596626 flet_contrib_pyodide-2024.4.27.1759/src/flet/version.py
+-rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 flet_contrib_pyodide-2024.4.27.1759/PKG-INFO
```

### Comparing `flet_contrib_pyodide-2024.4.27.1744/README.md` & `flet_contrib_pyodide-2024.4.27.1759/README.md`

 * *Files identical despite different names*

### Comparing `flet_contrib_pyodide-2024.4.27.1744/pyproject.toml` & `flet_contrib_pyodide-2024.4.27.1759/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-contrib-pyodide"
-version = "2024.04.27.1744"
+version = "2024.04.27.1759"
 description = "Flet for Pyodide - build standalone SPA in Python with Flutter UI."
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet", from = "src" },
@@ -13,15 +13,15 @@
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-flet-contrib-core = "2024.04.27.1744"
+flet-contrib-core = "2024.04.27.1759"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `flet_contrib_pyodide-2024.4.27.1744/src/flet/flet.py` & `flet_contrib_pyodide-2024.4.27.1759/src/flet/flet.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_pyodide-2024.4.27.1744/src/flet/pyodide_connection.py` & `flet_contrib_pyodide-2024.4.27.1759/src/flet/pyodide_connection.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_pyodide-2024.4.27.1744/PKG-INFO` & `flet_contrib_pyodide-2024.4.27.1759/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: flet-contrib-pyodide
-Version: 2024.4.27.1744
+Version: 2024.4.27.1759
 Summary: Flet for Pyodide - build standalone SPA in Python with Flutter UI.
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: flet-contrib-core (==2024.04.27.1744)
+Requires-Dist: flet-contrib-core (==2024.04.27.1759)
 Project-URL: documentation, https://flet.dev/docs
 Project-URL: homepage, https://flet.dev
 Project-URL: repository, https://github.com/flet-dev/flet
 Description-Content-Type: text/markdown
 
 # Flet for Pyodide - build standalone Single-Page Applications (SPA) in Python with Flutter UI
```

