# Comparing `tmp/tcolorpy-0.1.4.tar.gz` & `tmp/tcolorpy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcolorpy-0.1.4.tar", last modified: Sat Sep 16 12:35:04 2023, max compression
+gzip compressed data, was "tcolorpy-0.1.6.tar", last modified: Sat Apr 27 16:13:48 2024, max compression
```

## Comparing `tcolorpy-0.1.4.tar` & `tcolorpy-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,46 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-09-16 12:35:04.589871 tcolorpy-0.1.4/
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2023-09-16 12:34:39.000000 tcolorpy-0.1.4/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      203 2023-09-16 12:34:39.000000 tcolorpy-0.1.4/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     5712 2023-09-16 12:35:04.589871 tcolorpy-0.1.4/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     4177 2023-09-16 12:34:39.000000 tcolorpy-0.1.4/README.rst
--rw-r--r--   0 toor      (1000) toor      (1000)     1327 2023-09-16 12:34:39.000000 tcolorpy-0.1.4/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-09-16 12:35:04.589871 tcolorpy-0.1.4/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-09-16 12:34:39.000000 tcolorpy-0.1.4/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-09-16 12:34:39.000000 tcolorpy-0.1.4/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-09-16 12:35:04.589871 tcolorpy-0.1.4/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2470 2023-09-16 12:34:39.000000 tcolorpy-0.1.4/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-09-16 12:35:04.589871 tcolorpy-0.1.4/tcolorpy/
--rw-r--r--   0 toor      (1000) toor      (1000)      705 2023-09-16 12:34:39.000000 tcolorpy-0.1.4/tcolorpy/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1701 2023-09-16 12:34:39.000000 tcolorpy-0.1.4/tcolorpy/__main__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-09-16 12:34:39.000000 tcolorpy-0.1.4/tcolorpy/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1080 2023-09-16 12:34:39.000000 tcolorpy-0.1.4/tcolorpy/_const.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7495 2023-09-16 12:34:39.000000 tcolorpy-0.1.4/tcolorpy/_truecolor.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-09-16 12:34:39.000000 tcolorpy-0.1.4/tcolorpy/py.typed
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-09-16 12:35:04.589871 tcolorpy-0.1.4/tcolorpy.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     5712 2023-09-16 12:35:04.000000 tcolorpy-0.1.4/tcolorpy.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      485 2023-09-16 12:35:04.000000 tcolorpy-0.1.4/tcolorpy.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-09-16 12:35:04.000000 tcolorpy-0.1.4/tcolorpy.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-09-16 12:34:49.000000 tcolorpy-0.1.4/tcolorpy.egg-info/not-zip-safe
--rw-r--r--   0 toor      (1000) toor      (1000)       46 2023-09-16 12:35:04.000000 tcolorpy-0.1.4/tcolorpy.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        9 2023-09-16 12:35:04.000000 tcolorpy-0.1.4/tcolorpy.egg-info/top_level.txt
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-09-16 12:35:04.589871 tcolorpy-0.1.4/test/
--rw-r--r--   0 toor      (1000) toor      (1000)     2784 2023-09-16 12:34:39.000000 tcolorpy-0.1.4/test/test_color.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3432 2023-09-16 12:34:39.000000 tcolorpy-0.1.4/test/test_truecolor.py
--rw-r--r--   0 toor      (1000) toor      (1000)      896 2023-09-16 12:34:39.000000 tcolorpy-0.1.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:13:48.201067 tcolorpy-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:13:48.193067 tcolorpy-0.1.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:13:48.193067 tcolorpy-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-27 16:13:48.201067 tcolorpy-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:13:48.193067 tcolorpy-0.1.6/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      737 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/examples/ansi_colors.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1584 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/examples/ansi_styles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      637 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/examples/background_colors.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      144 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/examples/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:13:48.193067 tcolorpy-0.1.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/requirements/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 16:13:48.201067 tcolorpy-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:13:48.197067 tcolorpy-0.1.6/ss/
+-rw-r--r--   0 runner    (1001) docker     (127)    49596 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/ss/ansi_colors.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/ss/oneline.png
+-rw-r--r--   0 runner    (1001) docker     (127)   234252 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/ss/styles.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:13:48.197067 tcolorpy-0.1.6/tcolorpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/tcolorpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/tcolorpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/tcolorpy/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/tcolorpy/_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/tcolorpy/_truecolor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/tcolorpy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:13:48.197067 tcolorpy-0.1.6/tcolorpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-27 16:13:48.000000 tcolorpy-0.1.6/tcolorpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-27 16:13:48.000000 tcolorpy-0.1.6/tcolorpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:13:48.000000 tcolorpy-0.1.6/tcolorpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:13:35.000000 tcolorpy-0.1.6/tcolorpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-27 16:13:48.000000 tcolorpy-0.1.6/tcolorpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-27 16:13:48.000000 tcolorpy-0.1.6/tcolorpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:13:48.197067 tcolorpy-0.1.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/test/test_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/test/test_truecolor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-27 16:13:16.000000 tcolorpy-0.1.6/tox.ini
```

### Comparing `tcolorpy-0.1.4/LICENSE` & `tcolorpy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tcolorpy-0.1.4/PKG-INFO` & `tcolorpy-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,81 @@
 Metadata-Version: 2.1
 Name: tcolorpy
-Version: 0.1.4
+Version: 0.1.6
 Summary: tcolopy is a Python library to apply true color for terminal text.
 Home-page: https://github.com/thombashi/tcolorpy
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
+Project-URL: Changlog, https://github.com/thombashi/tcolorpy/blob/master/CHANGELOG.md
 Project-URL: Source, https://github.com/thombashi/tcolorpy
 Project-URL: Tracker, https://github.com/thombashi/tcolorpy/issues
 Keywords: ANSI escape,terminal color,truecolor
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Terminals
 Classifier: Topic :: Text Processing
+Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Provides-Extra: test
 Requires-Dist: pytest>=6.0.1; extra == "test"
-Requires-Dist: pytest-md-report>=0.4.1; extra == "test"
+Requires-Dist: pytest-md-report>=0.5; extra == "test"
 
 .. contents:: **tcolorpy**
    :backlinks: top
    :depth: 2
 
 
 Summary
 ============================================
 tcolopy is a Python library to apply true color for terminal text.
 
-.. image:: https://badge.fury.io/py/tcolorpy.svg
+|PyPI pkg ver| |conda pkg ver| |Supported Python implementations| |Supported Python versions| |CI status| |CodeQL| |coverage|
+
+.. |PyPI pkg ver| image:: https://badge.fury.io/py/tcolorpy.svg
     :target: https://badge.fury.io/py/tcolorpy
     :alt: PyPI package version
 
-.. image:: https://anaconda.org/conda-forge/tcolorpy/badges/version.svg
+.. |conda pkg ver| image:: https://anaconda.org/conda-forge/tcolorpy/badges/version.svg
     :target: https://anaconda.org/conda-forge/tcolorpy
     :alt: conda-forge package version
 
-.. image:: https://img.shields.io/pypi/pyversions/tcolorpy.svg
+.. |Supported Python implementations| image:: https://img.shields.io/pypi/implementation/tcolorpy.svg
     :target: https://pypi.org/project/tcolorpy
-    :alt: Supported Python versions
+    :alt: Supported Python implementations
 
-.. image:: https://img.shields.io/pypi/implementation/tcolorpy.svg
+.. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/tcolorpy.svg
     :target: https://pypi.org/project/tcolorpy
-    :alt: Supported Python implementations
+    :alt: Supported Python versions
 
-.. image:: https://github.com/thombashi/tcolorpy/workflows/Tests/badge.svg
-    :target: https://github.com/thombashi/tcolorpy/actions?query=workflow%3ATests
-    :alt: Linux/macOS/Windows CI status
+.. |CI status| image:: https://github.com/thombashi/tcolorpy/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/tcolorpy/actions/workflows/ci.yml
+    :alt: CI status of Linux/macOS/Windows
+
+.. |CodeQL| image:: https://github.com/thombashi/tcolorpy/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/tcolorpy/actions/workflows/github-code-scanning/codeql
+    :alt: CodeQL
 
-.. image:: https://coveralls.io/repos/github/thombashi/tcolorpy/badge.svg?branch=master
+.. |coverage| image:: https://coveralls.io/repos/github/thombashi/tcolorpy/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/tcolorpy?branch=master
     :alt: Test coverage: coveralls
 
 
 Installation
 ============================================
```

### Comparing `tcolorpy-0.1.4/README.rst` & `tcolorpy-0.1.6/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -3,35 +3,41 @@
    :depth: 2
 
 
 Summary
 ============================================
 tcolopy is a Python library to apply true color for terminal text.
 
-.. image:: https://badge.fury.io/py/tcolorpy.svg
+|PyPI pkg ver| |conda pkg ver| |Supported Python implementations| |Supported Python versions| |CI status| |CodeQL| |coverage|
+
+.. |PyPI pkg ver| image:: https://badge.fury.io/py/tcolorpy.svg
     :target: https://badge.fury.io/py/tcolorpy
     :alt: PyPI package version
 
-.. image:: https://anaconda.org/conda-forge/tcolorpy/badges/version.svg
+.. |conda pkg ver| image:: https://anaconda.org/conda-forge/tcolorpy/badges/version.svg
     :target: https://anaconda.org/conda-forge/tcolorpy
     :alt: conda-forge package version
 
-.. image:: https://img.shields.io/pypi/pyversions/tcolorpy.svg
+.. |Supported Python implementations| image:: https://img.shields.io/pypi/implementation/tcolorpy.svg
     :target: https://pypi.org/project/tcolorpy
-    :alt: Supported Python versions
+    :alt: Supported Python implementations
 
-.. image:: https://img.shields.io/pypi/implementation/tcolorpy.svg
+.. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/tcolorpy.svg
     :target: https://pypi.org/project/tcolorpy
-    :alt: Supported Python implementations
+    :alt: Supported Python versions
 
-.. image:: https://github.com/thombashi/tcolorpy/workflows/Tests/badge.svg
-    :target: https://github.com/thombashi/tcolorpy/actions?query=workflow%3ATests
-    :alt: Linux/macOS/Windows CI status
+.. |CI status| image:: https://github.com/thombashi/tcolorpy/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/tcolorpy/actions/workflows/ci.yml
+    :alt: CI status of Linux/macOS/Windows
+
+.. |CodeQL| image:: https://github.com/thombashi/tcolorpy/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/tcolorpy/actions/workflows/github-code-scanning/codeql
+    :alt: CodeQL
 
-.. image:: https://coveralls.io/repos/github/thombashi/tcolorpy/badge.svg?branch=master
+.. |coverage| image:: https://coveralls.io/repos/github/thombashi/tcolorpy/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/tcolorpy?branch=master
     :alt: Test coverage: coveralls
 
 
 Installation
 ============================================
```

### Comparing `tcolorpy-0.1.4/pyproject.toml` & `tcolorpy-0.1.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 [build-system]
 build-backend = "setuptools.build_meta"
-requires = ["setuptools>=61.0"]
+requires = [
+  "setuptools>=64",
+  "setuptools_scm>=7,<8; python_version<'3.8'",
+  "setuptools_scm>=8; python_version>='3.8'",
+]
+
+[tool.setuptools_scm]
+version_scheme = "guess-next-dev"
+local_scheme = "no-local-version"
 
 [tool.black]
 exclude = '''
 /(
       \.eggs
     | \.git
     | \.mypy_cache
@@ -15,28 +23,27 @@
     | buck-out
     | build
     | dist
 )/
 | docs/conf.py
 '''
 line-length = 100
-target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
+target-version = ['py37', 'py38', 'py39', 'py310', 'py311', 'py312']
 
 [tool.coverage.run]
 branch = true
 source = ['tcolorpy']
 
 [tool.coverage.report]
 exclude_lines = [
   'except ImportError',
   'raise NotImplementedError',
   'pass',
   'ABCmeta',
   'abstractmethod',
-  'abstractproperty',
   'abstractclassmethod',
   'warnings.warn',
 ]
 precision = 1
 show_missing = true
 
 [tool.isort]
@@ -66,15 +73,39 @@
 show_error_codes = true
 show_error_context = true
 warn_redundant_casts = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
+[tool.pyright]
+exclude = [
+    "**/node_modules",
+    "**/__pycache__",
+    ".tox",
+    ".venv",
+    "_build",
+    "_sandbox",
+    "build",
+    "dist"
+]
+pythonVersion = "3.7"
+
 [tool.pytest.ini_options]
 testpaths = [
   "test",
 ]
 
 md_report = true
 md_report_color = "auto"
 md_report_verbose = 0
+
+[tool.ruff]
+line-length = 100
+target-version = "py37"
+exclude = [
+    ".eggs/",
+    ".tox/",
+    "_sandbox/*",
+    "build/",
+    "docs/conf.py",
+]
```

### Comparing `tcolorpy-0.1.4/setup.py` & `tcolorpy-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,27 +27,27 @@
     LONG_DESCRIPTION = f.read()
 
 with open(os.path.join(REQUIREMENT_DIR, "test_requirements.txt")) as f:
     TESTS_REQUIRES = [line.strip() for line in f if line.strip()]
 
 setuptools.setup(
     name=MODULE_NAME,
-    version=pkg_info["__version__"],
     url=REPOSITORY_URL,
     author=pkg_info["__author__"],
     author_email=pkg_info["__email__"],
     description="tcolopy is a Python library to apply true color for terminal text.",
     include_package_data=True,
     keywords=["ANSI escape", "terminal color", "truecolor"],
     license=pkg_info["__license__"],
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/x-rst",
     packages=setuptools.find_packages(exclude=["test*"]),
     package_data={MODULE_NAME: ["py.typed"]},
     project_urls={
+        "Changlog": f"{REPOSITORY_URL:s}/blob/master/CHANGELOG.md",
         "Source": REPOSITORY_URL,
         "Tracker": f"{REPOSITORY_URL:s}/issues",
     },
     python_requires=">=3.7",
     extras_require={"test": TESTS_REQUIRES},
     classifiers=[
         "Development Status :: 4 - Beta",
@@ -56,18 +56,20 @@
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Terminals",
         "Topic :: Text Processing",
+        "Typing :: Typed",
     ],
     zip_safe=False,
     cmdclass=get_release_command_class(),
 )
```

### Comparing `tcolorpy-0.1.4/tcolorpy/__main__.py` & `tcolorpy-0.1.6/tcolorpy/__main__.py`

 * *Files identical despite different names*

### Comparing `tcolorpy-0.1.4/tcolorpy/_const.py` & `tcolorpy-0.1.6/tcolorpy/_const.py`

 * *Files identical despite different names*

### Comparing `tcolorpy-0.1.4/tcolorpy/_truecolor.py` & `tcolorpy-0.1.6/tcolorpy/_truecolor.py`

 * *Files identical despite different names*

### Comparing `tcolorpy-0.1.4/tcolorpy.egg-info/PKG-INFO` & `tcolorpy-0.1.6/tcolorpy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,81 @@
 Metadata-Version: 2.1
 Name: tcolorpy
-Version: 0.1.4
+Version: 0.1.6
 Summary: tcolopy is a Python library to apply true color for terminal text.
 Home-page: https://github.com/thombashi/tcolorpy
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
+Project-URL: Changlog, https://github.com/thombashi/tcolorpy/blob/master/CHANGELOG.md
 Project-URL: Source, https://github.com/thombashi/tcolorpy
 Project-URL: Tracker, https://github.com/thombashi/tcolorpy/issues
 Keywords: ANSI escape,terminal color,truecolor
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Terminals
 Classifier: Topic :: Text Processing
+Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Provides-Extra: test
 Requires-Dist: pytest>=6.0.1; extra == "test"
-Requires-Dist: pytest-md-report>=0.4.1; extra == "test"
+Requires-Dist: pytest-md-report>=0.5; extra == "test"
 
 .. contents:: **tcolorpy**
    :backlinks: top
    :depth: 2
 
 
 Summary
 ============================================
 tcolopy is a Python library to apply true color for terminal text.
 
-.. image:: https://badge.fury.io/py/tcolorpy.svg
+|PyPI pkg ver| |conda pkg ver| |Supported Python implementations| |Supported Python versions| |CI status| |CodeQL| |coverage|
+
+.. |PyPI pkg ver| image:: https://badge.fury.io/py/tcolorpy.svg
     :target: https://badge.fury.io/py/tcolorpy
     :alt: PyPI package version
 
-.. image:: https://anaconda.org/conda-forge/tcolorpy/badges/version.svg
+.. |conda pkg ver| image:: https://anaconda.org/conda-forge/tcolorpy/badges/version.svg
     :target: https://anaconda.org/conda-forge/tcolorpy
     :alt: conda-forge package version
 
-.. image:: https://img.shields.io/pypi/pyversions/tcolorpy.svg
+.. |Supported Python implementations| image:: https://img.shields.io/pypi/implementation/tcolorpy.svg
     :target: https://pypi.org/project/tcolorpy
-    :alt: Supported Python versions
+    :alt: Supported Python implementations
 
-.. image:: https://img.shields.io/pypi/implementation/tcolorpy.svg
+.. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/tcolorpy.svg
     :target: https://pypi.org/project/tcolorpy
-    :alt: Supported Python implementations
+    :alt: Supported Python versions
 
-.. image:: https://github.com/thombashi/tcolorpy/workflows/Tests/badge.svg
-    :target: https://github.com/thombashi/tcolorpy/actions?query=workflow%3ATests
-    :alt: Linux/macOS/Windows CI status
+.. |CI status| image:: https://github.com/thombashi/tcolorpy/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/tcolorpy/actions/workflows/ci.yml
+    :alt: CI status of Linux/macOS/Windows
+
+.. |CodeQL| image:: https://github.com/thombashi/tcolorpy/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/tcolorpy/actions/workflows/github-code-scanning/codeql
+    :alt: CodeQL
 
-.. image:: https://coveralls.io/repos/github/thombashi/tcolorpy/badge.svg?branch=master
+.. |coverage| image:: https://coveralls.io/repos/github/thombashi/tcolorpy/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/tcolorpy?branch=master
     :alt: Test coverage: coveralls
 
 
 Installation
 ============================================
```

### Comparing `tcolorpy-0.1.4/test/test_color.py` & `tcolorpy-0.1.6/test/test_color.py`

 * *Files identical despite different names*

### Comparing `tcolorpy-0.1.4/test/test_truecolor.py` & `tcolorpy-0.1.6/test/test_truecolor.py`

 * *Files identical despite different names*

### Comparing `tcolorpy-0.1.4/tox.ini` & `tcolorpy-0.1.6/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tox]
 envlist =
-    py{37,38,39,310,311}
+    py{37,38,39,310,311,312}
     pypy3
     build
     cov
     fmt
     lint
 
 [testenv]
 extras =
     test
 commands =
     pytest {posargs}
 
 [testenv:build]
 deps =
-    build>=0.10
+    build>=1
     twine
 commands =
     python -m build
-    twine check dist/*.whl dist/*.tar.gz
+    ; twine check dist/*.whl dist/*.tar.gz
 
 [testenv:clean]
 skip_install = true
 deps =
     cleanpy>=0.4
 commands =
     cleanpy --all --exclude-envs .
@@ -34,26 +34,45 @@
     test
 deps =
     coverage[toml]>=5
 commands =
     coverage run -m pytest {posargs:-vv}
     coverage report -m
 
+[testenv:fmt-black]
+skip_install = true
+deps =
+    autoflake>=2
+    black>=24.1
+    isort>=5
+commands =
+    autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports .
+    isort .
+    black setup.py test pathvalidate
+
 [testenv:fmt]
 skip_install = true
 deps =
     autoflake>=2
-    black>=23.1
     isort>=5
+    ruff>=0.3.5
 commands =
     autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports .
     isort .
-    black setup.py test tcolorpy examples
+    ruff format
 
 [testenv:lint]
-skip_install = true
+extras =
+    test
 deps =
+    codespell>=2
     mypy>=1
-    pylama>=8.4.1
+    pyright>=1.1
+    releasecmd
+    ruff>=0.3.5
+    setuptools_scm
 commands =
     mypy tcolorpy setup.py
-    pylama
+    codespell tcolorpy test -q2 --check-filenames
+    pyright
+    ruff format --check
+    ruff check
```

