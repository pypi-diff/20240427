# Comparing `tmp/jaraco.fabric-6.1.1.tar.gz` & `tmp/jaraco_fabric-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.fabric-6.1.1.tar", last modified: Mon Jan 29 17:30:42 2024, max compression
+gzip compressed data, was "jaraco_fabric-6.2.0.tar", last modified: Sat Apr 27 14:21:34 2024, max compression
```

## Comparing `jaraco.fabric-6.1.1.tar` & `jaraco_fabric-6.2.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:30:42.002489 jaraco.fabric-6.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:30:41.998489 jaraco.fabric-6.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:30:41.998489 jaraco.fabric-6.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-01-29 17:30:42.002489 jaraco.fabric-6.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:30:41.998489 jaraco.fabric-6.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:30:41.994489 jaraco.fabric-6.1.1/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:30:42.002489 jaraco.fabric-6.1.1/jaraco/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/jaraco/fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/jaraco/fabric/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/jaraco/fabric/apt.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/jaraco/fabric/fabfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/jaraco/fabric/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/jaraco/fabric/mongod.service
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/jaraco/fabric/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/jaraco/fabric/monkey.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/jaraco/fabric/python.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/jaraco/fabric/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:30:42.002489 jaraco.fabric-6.1.1/jaraco.fabric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-01-29 17:30:41.000000 jaraco.fabric-6.1.1/jaraco.fabric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-01-29 17:30:41.000000 jaraco.fabric-6.1.1/jaraco.fabric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 17:30:41.000000 jaraco.fabric-6.1.1/jaraco.fabric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-01-29 17:30:41.000000 jaraco.fabric-6.1.1/jaraco.fabric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-29 17:30:41.000000 jaraco.fabric-6.1.1/jaraco.fabric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-01-29 17:30:42.002489 jaraco.fabric-6.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-01-29 17:30:22.000000 jaraco.fabric-6.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:21:34.581524 jaraco_fabric-6.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:21:34.573524 jaraco_fabric-6.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:21:34.573524 jaraco_fabric-6.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-27 14:21:34.581524 jaraco_fabric-6.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:21:34.573524 jaraco_fabric-6.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:21:34.569524 jaraco_fabric-6.2.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:21:34.577524 jaraco_fabric-6.2.0/jaraco/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/jaraco/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/jaraco/fabric/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/jaraco/fabric/apt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/jaraco/fabric/certs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/jaraco/fabric/fabfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/jaraco/fabric/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/jaraco/fabric/mongod.service
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/jaraco/fabric/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/jaraco/fabric/monkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/jaraco/fabric/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/jaraco/fabric/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:21:34.577524 jaraco_fabric-6.2.0/jaraco.fabric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-27 14:21:34.000000 jaraco_fabric-6.2.0/jaraco.fabric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-27 14:21:34.000000 jaraco_fabric-6.2.0/jaraco.fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 14:21:34.000000 jaraco_fabric-6.2.0/jaraco.fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-27 14:21:34.000000 jaraco_fabric-6.2.0/jaraco.fabric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-27 14:21:34.000000 jaraco_fabric-6.2.0/jaraco.fabric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 14:21:34.581524 jaraco_fabric-6.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-27 14:21:15.000000 jaraco_fabric-6.2.0/tox.ini
```

### Comparing `jaraco.fabric-6.1.1/.github/workflows/main.yml` & `jaraco_fabric-6.2.0/.github/workflows/main.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 name: tests
 
 on:
   merge_group:
   push:
     branches-ignore:
-    # disabled for jaraco/skeleton#103
-    # - gh-readonly-queue/**  # Temporary merge queue-related GH-made branches
+    # temporary GH branches relating to merge queues (jaraco/skeleton#93)
+    - gh-readonly-queue/**
+    tags:
+    # required if branches-ignore is supplied (jaraco/skeleton#103)
+    - '**'
   pull_request:
 
 permissions:
   contents: read
 
 env:
   # Environment variable to support color support (jaraco/skeleton#66)
@@ -24,32 +27,34 @@
   TOX_OVERRIDE: >-
     testenv.pass_env+=GITHUB_*,FORCE_COLOR
 
 
 jobs:
   test:
     strategy:
+      # https://blog.jaraco.com/efficient-use-of-ci-resources/
       matrix:
         python:
         - "3.8"
-        - "3.11"
         - "3.12"
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
+        - python: "3.11"
+          platform: ubuntu-latest
         - python: pypy3.10
           platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
-    continue-on-error: ${{ matrix.python == '3.13' }}
+    continue-on-error: ${{ matrix.python == '3.13' || (matrix.python == '3.8' || matrix.python == '3.9') && matrix.platform == 'macos-latest' }}
     steps:
       - uses: actions/checkout@v4
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
           allow-prereleases: true
```

### Comparing `jaraco.fabric-6.1.1/LICENSE` & `jaraco_fabric-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.fabric-6.1.1/NEWS.rst` & `jaraco_fabric-6.2.0/NEWS.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v6.2.0
+======
+
+Features
+--------
+
+- Added certs module.
+
+
 v6.1.1
 ======
 
 No significant changes.
 
 
 v6.1.0
```

### Comparing `jaraco.fabric-6.1.1/PKG-INFO` & `jaraco_fabric-6.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: jaraco.fabric
-Version: 6.1.1
+Version: 6.2.0
 Summary: Fabric tasks by jaraco
-Home-page: https://github.com/jaraco/jaraco.fabric
-Author: Jason R. Coombs
-Author-email: jaraco@jaraco.com
+Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
+Project-URL: Homepage, https://github.com/jaraco/jaraco.fabric
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: jaraco.apt
 Requires-Dist: jaraco.itertools
 Requires-Dist: pyyaml
 Requires-Dist: importlib_resources
+Requires-Dist: jaraco.home
 Provides-Extra: testing
-Requires-Dist: pytest>=6; extra == "testing"
+Requires-Dist: pytest!=8.1.*,>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
-Requires-Dist: pytest-mypy; platform_python_implementation != "PyPy" and extra == "testing"
+Requires-Dist: pytest-mypy; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
 Requires-Dist: fabric; extra == "testing"
 Requires-Dist: types-setuptools; extra == "testing"
 Requires-Dist: types-pyyaml; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
-Requires-Dist: sphinx<7.2.5; extra == "docs"
 Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
 Requires-Dist: rst.linker>=1.9; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-lint; extra == "docs"
 
 .. image:: https://img.shields.io/pypi/v/jaraco.fabric.svg
    :target: https://pypi.org/project/jaraco.fabric
@@ -46,15 +46,15 @@
 .. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
     :target: https://github.com/astral-sh/ruff
     :alt: Ruff
 
 .. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
 ..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2023-informational
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
 
 Fabric tasks and helpers. Includes modules implementing
 Fabric tasks.
 
 The easiest way to use jaraco.fabric is to install it and
 invoke it using ``python -m jaraco.fabric``. For example,
```

### Comparing `jaraco.fabric-6.1.1/README.rst` & `jaraco_fabric-6.2.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 .. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
     :target: https://github.com/astral-sh/ruff
     :alt: Ruff
 
 .. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
 ..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2023-informational
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
 
 Fabric tasks and helpers. Includes modules implementing
 Fabric tasks.
 
 The easiest way to use jaraco.fabric is to install it and
 invoke it using ``python -m jaraco.fabric``. For example,
```

### Comparing `jaraco.fabric-6.1.1/docs/conf.py` & `jaraco_fabric-6.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.fabric-6.1.1/jaraco/fabric/apt.py` & `jaraco_fabric-6.2.0/jaraco/fabric/apt.py`

 * *Files identical despite different names*

### Comparing `jaraco.fabric-6.1.1/jaraco/fabric/files.py` & `jaraco_fabric-6.2.0/jaraco/fabric/files.py`

 * *Files identical despite different names*

### Comparing `jaraco.fabric-6.1.1/jaraco/fabric/mongodb.py` & `jaraco_fabric-6.2.0/jaraco/fabric/mongodb.py`

 * *Files identical despite different names*

### Comparing `jaraco.fabric-6.1.1/jaraco.fabric.egg-info/PKG-INFO` & `jaraco_fabric-6.2.0/jaraco.fabric.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: jaraco.fabric
-Version: 6.1.1
+Version: 6.2.0
 Summary: Fabric tasks by jaraco
-Home-page: https://github.com/jaraco/jaraco.fabric
-Author: Jason R. Coombs
-Author-email: jaraco@jaraco.com
+Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
+Project-URL: Homepage, https://github.com/jaraco/jaraco.fabric
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: jaraco.apt
 Requires-Dist: jaraco.itertools
 Requires-Dist: pyyaml
 Requires-Dist: importlib_resources
+Requires-Dist: jaraco.home
 Provides-Extra: testing
-Requires-Dist: pytest>=6; extra == "testing"
+Requires-Dist: pytest!=8.1.*,>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
-Requires-Dist: pytest-mypy; platform_python_implementation != "PyPy" and extra == "testing"
+Requires-Dist: pytest-mypy; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
 Requires-Dist: fabric; extra == "testing"
 Requires-Dist: types-setuptools; extra == "testing"
 Requires-Dist: types-pyyaml; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
-Requires-Dist: sphinx<7.2.5; extra == "docs"
 Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
 Requires-Dist: rst.linker>=1.9; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-lint; extra == "docs"
 
 .. image:: https://img.shields.io/pypi/v/jaraco.fabric.svg
    :target: https://pypi.org/project/jaraco.fabric
@@ -46,15 +46,15 @@
 .. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
     :target: https://github.com/astral-sh/ruff
     :alt: Ruff
 
 .. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
 ..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2023-informational
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
 
 Fabric tasks and helpers. Includes modules implementing
 Fabric tasks.
 
 The easiest way to use jaraco.fabric is to install it and
 invoke it using ``python -m jaraco.fabric``. For example,
```

### Comparing `jaraco.fabric-6.1.1/jaraco.fabric.egg-info/SOURCES.txt` & `jaraco_fabric-6.2.0/jaraco.fabric.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 LICENSE
 NEWS.rst
 README.rst
 mypy.ini
 pyproject.toml
 pytest.ini
 ruff.toml
-setup.cfg
 towncrier.toml
 tox.ini
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
 docs/history.rst
 docs/index.rst
@@ -21,14 +20,15 @@
 jaraco.fabric.egg-info/SOURCES.txt
 jaraco.fabric.egg-info/dependency_links.txt
 jaraco.fabric.egg-info/requires.txt
 jaraco.fabric.egg-info/top_level.txt
 jaraco/fabric/__init__.py
 jaraco/fabric/__main__.py
 jaraco/fabric/apt.py
+jaraco/fabric/certs.py
 jaraco/fabric/fabfile.py
 jaraco/fabric/files.py
 jaraco/fabric/mongod.service
 jaraco/fabric/mongodb.py
 jaraco/fabric/monkey.py
 jaraco/fabric/python.py
 jaraco/fabric/wrapper.py
```

### Comparing `jaraco.fabric-6.1.1/pytest.ini` & `jaraco_fabric-6.2.0/pytest.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 [pytest]
 norecursedirs=dist build .tox .eggs
-addopts=--doctest-modules --import-mode=importlib
+addopts=
+	--doctest-modules
+	--import-mode importlib
+consider_namespace_packages=true
 filterwarnings=
 	## upstream
 
 	# Ensure ResourceWarnings are emitted
 	default::ResourceWarning
 
 	# realpython/pytest-mypy#152
```

### Comparing `jaraco.fabric-6.1.1/tox.ini` & `jaraco_fabric-6.2.0/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 usedevelop = True
 extras =
 	testing
 
 [testenv:diffcov]
 description = run tests and check that diff from main is covered
 deps =
+	{[testenv]deps}
 	diff-cover
 commands =
 	pytest {posargs} --cov-report xml
 	diff-cover coverage.xml --compare-branch=origin/main --html-report diffcov.html
 	diff-cover coverage.xml --compare-branch=origin/main --fail-under=100
 
 [testenv:docs]
```

