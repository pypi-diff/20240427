# Comparing `tmp/obvs-0.1.0.tar.gz` & `tmp/obvs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obvs-0.1.0.tar", max compression
+gzip compressed data, was "obvs-0.1.1.tar", max compression
```

## Comparing `obvs-0.1.0.tar` & `obvs-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1070 2024-04-27 03:25:59.294279 obvs-0.1.0/LICENSE
--rw-r--r--   0        0        0       83 2024-02-29 04:23:57.449418 obvs-0.1.0/obvs/__init__.py
--rw-r--r--   0        0        0    19237 2024-04-26 22:23:36.259612 obvs-0.1.0/obvs/lenses.py
--rw-r--r--   0        0        0     1493 2024-04-25 05:54:16.193553 obvs-0.1.0/obvs/logging.py
--rw-r--r--   0        0        0     4698 2024-04-26 22:23:36.259861 obvs-0.1.0/obvs/metrics.py
--rw-r--r--   0        0        0    15905 2024-04-25 05:54:16.193934 obvs-0.1.0/obvs/patchscope.py
--rw-r--r--   0        0        0    10149 2024-04-25 05:54:16.194228 obvs-0.1.0/obvs/patchscope_base.py
--rw-r--r--   0        0        0     3679 2024-04-25 05:54:16.194362 obvs-0.1.0/obvs/vis.py
--rw-r--r--   0        0        0     2992 2024-04-27 03:39:08.117520 obvs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 obvs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-27 03:25:59.294279 obvs-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1076 2024-04-25 05:54:16.192497 obvs-0.1.1/README.md
+-rw-r--r--   0        0        0       83 2024-02-29 04:23:57.449418 obvs-0.1.1/obvs/__init__.py
+-rw-r--r--   0        0        0    19237 2024-04-26 22:23:36.259612 obvs-0.1.1/obvs/lenses.py
+-rw-r--r--   0        0        0     1493 2024-04-25 05:54:16.193553 obvs-0.1.1/obvs/logging.py
+-rw-r--r--   0        0        0     4698 2024-04-26 22:23:36.259861 obvs-0.1.1/obvs/metrics.py
+-rw-r--r--   0        0        0    15905 2024-04-25 05:54:16.193934 obvs-0.1.1/obvs/patchscope.py
+-rw-r--r--   0        0        0    10149 2024-04-25 05:54:16.194228 obvs-0.1.1/obvs/patchscope_base.py
+-rw-r--r--   0        0        0     3679 2024-04-25 05:54:16.194362 obvs-0.1.1/obvs/vis.py
+-rw-r--r--   0        0        0     3013 2024-04-27 03:49:38.509495 obvs-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2310 1970-01-01 00:00:00.000000 obvs-0.1.1/PKG-INFO
```

### Comparing `obvs-0.1.0/LICENSE` & `obvs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `obvs-0.1.0/obvs/lenses.py` & `obvs-0.1.1/obvs/lenses.py`

 * *Files identical despite different names*

### Comparing `obvs-0.1.0/obvs/logging.py` & `obvs-0.1.1/obvs/logging.py`

 * *Files identical despite different names*

### Comparing `obvs-0.1.0/obvs/metrics.py` & `obvs-0.1.1/obvs/metrics.py`

 * *Files identical despite different names*

### Comparing `obvs-0.1.0/obvs/patchscope.py` & `obvs-0.1.1/obvs/patchscope.py`

 * *Files identical despite different names*

### Comparing `obvs-0.1.0/obvs/patchscope_base.py` & `obvs-0.1.1/obvs/patchscope_base.py`

 * *Files identical despite different names*

### Comparing `obvs-0.1.0/obvs/vis.py` & `obvs-0.1.1/obvs/vis.py`

 * *Files identical despite different names*

### Comparing `obvs-0.1.0/pyproject.toml` & `obvs-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 ###########
 # 📜 Poetry
 ###########
 [tool.poetry]
 name = "obvs"
-version = "0.1.0"
+version = "0.1.1"
 description = "Making Transformers Obvious"
 authors = ["Jamie Coombes <jamie@example.com>"]
 license = "MIT"
 packages = [{ include = "obvs" }]
+readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10.0"
 # Everything below here is alphabetically sorted
 ipykernel = "^6.28.0"
 torch = "==2.2.0"
 transformers = "^4.37.1"
```

### Comparing `obvs-0.1.0/PKG-INFO` & `obvs-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obvs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Making Transformers Obvious
 License: MIT
 Author: Jamie Coombes
 Author-email: jamie@example.com
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -26,7 +26,33 @@
 Requires-Dist: plotly (>=5.18.0,<6.0.0)
 Requires-Dist: tiktoken (>=0.5.2,<0.6.0)
 Requires-Dist: torch (==2.2.0)
 Requires-Dist: torchmetrics (>=1.3.1,<2.0.0)
 Requires-Dist: transformers (>=4.37.1,<5.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: zstandard (>=0.22.0,<0.23.0)
+Description-Content-Type: text/markdown
+
+# obvs
+
+[![CI](https://github.com/obvslib/obvs/actions/workflows/main.yaml/badge.svg)](https://github.com/obvslib/obvs/actions/workflows/main.yaml)
+
+Making Transformers Obvious
+
+## Project cheatsheet
+
+-   **pre-commit:** `pre-commit run --all-files`
+-   **pytest:** `pytest` or `pytest -s`
+-   **coverage:** `coverage run -m pytest` or `coverage html`
+-   **poetry sync:** `poetry install --no-root --sync`
+-   **updating requirements:** see [docs/updating_requirements.md](docs/updating_requirements.md)
+
+## Initial project setup
+
+1. See [docs/getting_started.md](docs/getting_started.md) or [docs/quickstart.md](docs/quickstart.md)
+   for how to get up & running.
+2. Check [docs/project_specific_setup.md](docs/project_specific_setup.md) for project specific setup.
+3. See [docs/using_poetry.md](docs/using_poetry.md) for how to update Python requirements using
+   [Poetry](https://python-poetry.org/).
+4. See [docs/detect_secrets.md](docs/detect_secrets.md) for more on creating a `.secrets.baseline`
+   file using [detect-secrets](https://github.com/Yelp/detect-secrets).
+
```

