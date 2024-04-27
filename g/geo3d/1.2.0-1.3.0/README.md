# Comparing `tmp/geo3d-1.2.0.tar.gz` & `tmp/geo3d-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo3d-1.2.0.tar", last modified: Wed Apr 24 13:29:00 2024, max compression
+gzip compressed data, was "geo3d-1.3.0.tar", last modified: Sat Apr 27 07:43:09 2024, max compression
```

## Comparing `geo3d-1.2.0.tar` & `geo3d-1.3.0.tar`

### file list

```diff
@@ -1,59 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:00.852776 geo3d-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 13:28:45.000000 geo3d-1.2.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:00.844776 geo3d-1.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-24 13:28:45.000000 geo3d-1.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:00.844776 geo3d-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-24 13:28:45.000000 geo3d-1.2.0/.github/workflows/build_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-24 13:28:45.000000 geo3d-1.2.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-24 13:28:45.000000 geo3d-1.2.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-24 13:28:45.000000 geo3d-1.2.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-24 13:28:45.000000 geo3d-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-24 13:28:45.000000 geo3d-1.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-24 13:28:45.000000 geo3d-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-24 13:29:00.852776 geo3d-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-24 13:28:45.000000 geo3d-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:00.848776 geo3d-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-24 13:28:45.000000 geo3d-1.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    14988 2024-04-24 13:28:45.000000 geo3d-1.2.0/docs/basic_usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-24 13:28:45.000000 geo3d-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-24 13:28:45.000000 geo3d-1.2.0/docs/fit.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-24 13:28:45.000000 geo3d-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-24 13:28:45.000000 geo3d-1.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-24 13:28:45.000000 geo3d-1.2.0/docs/queries.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:00.848776 geo3d-1.2.0/geo3d/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/fit.py
--rw-r--r--   0 runner    (1001) docker     (127)    16367 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/plane.py
--rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     7132 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:00.852776 geo3d-1.2.0/geo3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-24 13:29:00.000000 geo3d-1.2.0/geo3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-24 13:29:00.000000 geo3d-1.2.0/geo3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:29:00.000000 geo3d-1.2.0/geo3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-24 13:29:00.000000 geo3d-1.2.0/geo3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 13:29:00.000000 geo3d-1.2.0/geo3d.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:00.852776 geo3d-1.2.0/profiling/
--rw-r--r--   0 runner    (1001) docker     (127)    25441 2024-04-24 13:28:45.000000 geo3d-1.2.0/profiling/speed_tests.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-24 13:28:45.000000 geo3d-1.2.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-24 13:28:45.000000 geo3d-1.2.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-24 13:28:45.000000 geo3d-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:29:00.852776 geo3d-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-24 13:28:45.000000 geo3d-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:00.852776 geo3d-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-24 13:28:45.000000 geo3d-1.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-24 13:28:45.000000 geo3d-1.2.0/tests/test_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-24 13:28:45.000000 geo3d-1.2.0/tests/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-24 13:28:45.000000 geo3d-1.2.0/tests/test_plane.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-24 13:28:45.000000 geo3d-1.2.0/tests/test_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-24 13:28:45.000000 geo3d-1.2.0/tests/test_quat_algs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-24 13:28:45.000000 geo3d-1.2.0/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-24 13:28:45.000000 geo3d-1.2.0/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-24 13:28:45.000000 geo3d-1.2.0/tests/test_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:43:09.125236 geo3d-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:43:09.117236 geo3d-1.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-27 07:42:33.000000 geo3d-1.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:43:09.117236 geo3d-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-27 07:42:33.000000 geo3d-1.3.0/.github/workflows/build_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-27 07:42:33.000000 geo3d-1.3.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-27 07:42:33.000000 geo3d-1.3.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-27 07:42:33.000000 geo3d-1.3.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-27 07:42:33.000000 geo3d-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-27 07:42:33.000000 geo3d-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-27 07:43:09.125236 geo3d-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-27 07:42:33.000000 geo3d-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:43:09.117236 geo3d-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-27 07:42:33.000000 geo3d-1.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    14988 2024-04-27 07:42:33.000000 geo3d-1.3.0/docs/basic_usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-27 07:42:33.000000 geo3d-1.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-27 07:42:33.000000 geo3d-1.3.0/docs/fit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-27 07:42:33.000000 geo3d-1.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-27 07:42:33.000000 geo3d-1.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-27 07:42:33.000000 geo3d-1.3.0/docs/queries.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:43:09.117236 geo3d-1.3.0/profiling/
+-rw-r--r--   0 runner    (1001) docker     (127)    25441 2024-04-27 07:42:33.000000 geo3d-1.3.0/profiling/speed_tests.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-27 07:42:33.000000 geo3d-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 07:43:09.125236 geo3d-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:43:09.117236 geo3d-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:43:09.121236 geo3d-1.3.0/src/geo3d/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-27 07:42:33.000000 geo3d-1.3.0/src/geo3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-27 07:42:33.000000 geo3d-1.3.0/src/geo3d/auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-27 07:42:33.000000 geo3d-1.3.0/src/geo3d/fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16367 2024-04-27 07:42:33.000000 geo3d-1.3.0/src/geo3d/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-27 07:42:33.000000 geo3d-1.3.0/src/geo3d/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-27 07:42:33.000000 geo3d-1.3.0/src/geo3d/plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-04-27 07:42:33.000000 geo3d-1.3.0/src/geo3d/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7132 2024-04-27 07:42:33.000000 geo3d-1.3.0/src/geo3d/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-27 07:42:33.000000 geo3d-1.3.0/src/geo3d/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-27 07:42:33.000000 geo3d-1.3.0/src/geo3d/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-27 07:42:33.000000 geo3d-1.3.0/src/geo3d/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-27 07:42:33.000000 geo3d-1.3.0/src/geo3d/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-04-27 07:42:33.000000 geo3d-1.3.0/src/geo3d/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:43:09.121236 geo3d-1.3.0/src/geo3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-27 07:43:09.000000 geo3d-1.3.0/src/geo3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-27 07:43:09.000000 geo3d-1.3.0/src/geo3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 07:43:09.000000 geo3d-1.3.0/src/geo3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-27 07:43:09.000000 geo3d-1.3.0/src/geo3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-27 07:43:09.000000 geo3d-1.3.0/src/geo3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:43:09.121236 geo3d-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-27 07:42:33.000000 geo3d-1.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-27 07:42:33.000000 geo3d-1.3.0/tests/test_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-27 07:42:33.000000 geo3d-1.3.0/tests/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-27 07:42:33.000000 geo3d-1.3.0/tests/test_plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-27 07:42:33.000000 geo3d-1.3.0/tests/test_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-27 07:42:33.000000 geo3d-1.3.0/tests/test_quat_algs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-27 07:42:33.000000 geo3d-1.3.0/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-27 07:42:33.000000 geo3d-1.3.0/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-27 07:42:33.000000 geo3d-1.3.0/tests/test_vector.py
```

### Comparing `geo3d-1.2.0/.github/workflows/build_docs.yml` & `geo3d-1.3.0/.github/workflows/build_docs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         with:
           python-version: "3.11"
         
       # Runs a single command using the runners shell
       - name: Build the Sphinx Docs
         run: |
           python -m pip install -U pip
-          python -m pip install -r requirements-dev.txt
+          python -m pip install sphinx nbsphinx sphinx_copybutton
           sudo apt-get install pandoc
           cd docs && make html
 
       # Runs a set of commands using the runners shell
       - name: Deploy to GitHub Pages
         # You may pin to the exact commit or the version.
         # uses: JamesIves/github-pages-deploy-action@54066045208a389f6e16e9030494962f8afb4dfc
```

### Comparing `geo3d-1.2.0/.github/workflows/codeql-analysis.yml` & `geo3d-1.3.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/.github/workflows/test.yml` & `geo3d-1.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/LICENSE.txt` & `geo3d-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/README.md` & `geo3d-1.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -10,25 +10,25 @@
   - express points and vectors in different frames
   - create frames from primary and secondary axes vectors
   - align two point groups by minimizing point-to-point distances
   - fit planes to points
 
 Requires Python 3.7 or up .
 
-## Installation 
+## Installation
+
 To install the module and its core requirements, run
 ```sh
-pip install --user -e .
+pip install geo3d
 ```
-within the base directory. 
 
-To install all requirements, including the ones for unit testing and documentation.
+Maintainers should install in editable mode, including all additional requirements for unit testing and documentation:
 
 ```sh
-pip install --user -e .[dev]
+pip install -e .[dev]
 ```
 
 ## Usage 
 Instructions on basic usage can be found in the jupyter notebook in [`/docs`](./docs), 
 which are also deployed to [himbeles.github.io/geo3d](https://himbeles.github.io/geo3d).
 
 ## Testing
```

### Comparing `geo3d-1.2.0/docs/Makefile` & `geo3d-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/docs/basic_usage.ipynb` & `geo3d-1.3.0/docs/basic_usage.ipynb`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/docs/conf.py` & `geo3d-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/docs/fit.ipynb` & `geo3d-1.3.0/docs/fit.ipynb`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/docs/make.bat` & `geo3d-1.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/docs/queries.ipynb` & `geo3d-1.3.0/docs/queries.ipynb`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/geo3d/auxiliary.py` & `geo3d-1.3.0/src/geo3d/auxiliary.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/geo3d/fit.py` & `geo3d-1.3.0/src/geo3d/fit.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/geo3d/frame.py` & `geo3d-1.3.0/src/geo3d/frame.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/geo3d/linalg.py` & `geo3d-1.3.0/src/geo3d/linalg.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/geo3d/plane.py` & `geo3d-1.3.0/src/geo3d/plane.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/geo3d/point.py` & `geo3d-1.3.0/src/geo3d/point.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/geo3d/quaternion.py` & `geo3d-1.3.0/src/geo3d/quaternion.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/geo3d/query.py` & `geo3d-1.3.0/src/geo3d/query.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/geo3d/rotation.py` & `geo3d-1.3.0/src/geo3d/rotation.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/geo3d/vector.py` & `geo3d-1.3.0/src/geo3d/vector.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/profiling/speed_tests.ipynb` & `geo3d-1.3.0/profiling/speed_tests.ipynb`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/tests/test_frame.py` & `geo3d-1.3.0/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/tests/test_point.py` & `geo3d-1.3.0/tests/test_point.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/tests/test_quat_algs.py` & `geo3d-1.3.0/tests/test_quat_algs.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/tests/test_queries.py` & `geo3d-1.3.0/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/tests/test_transform.py` & `geo3d-1.3.0/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.2.0/tests/test_vector.py` & `geo3d-1.3.0/tests/test_vector.py`

 * *Files identical despite different names*

