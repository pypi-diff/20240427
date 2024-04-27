# Comparing `tmp/cfractions-2.2.0.tar.gz` & `tmp/cfractions-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfractions-2.2.0.tar", last modified: Fri Dec 30 04:16:15 2022, max compression
+gzip compressed data, was "cfractions-2.3.0.tar", last modified: Sat Apr 27 00:59:44 2024, max compression
```

## Comparing `cfractions-2.2.0.tar` & `cfractions-2.3.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 04:16:15.458748 cfractions-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2022-12-30 04:16:05.000000 cfractions-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-30 04:16:05.000000 cfractions-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2022-12-30 04:16:15.458748 cfractions-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2022-12-30 04:16:05.000000 cfractions-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 04:16:15.454748 cfractions-2.2.0/cfractions/
--rw-r--r--   0 runner    (1001) docker     (123)     8838 2022-12-30 04:16:05.000000 cfractions-2.2.0/cfractions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2022-12-30 04:16:05.000000 cfractions-2.2.0/cfractions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-30 04:16:05.000000 cfractions-2.2.0/cfractions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 04:16:15.454748 cfractions-2.2.0/cfractions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2022-12-30 04:16:15.000000 cfractions-2.2.0/cfractions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      291 2022-12-30 04:16:15.000000 cfractions-2.2.0/cfractions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-30 04:16:15.000000 cfractions-2.2.0/cfractions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-30 04:16:15.000000 cfractions-2.2.0/cfractions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-30 04:16:15.000000 cfractions-2.2.0/cfractions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-30 04:16:15.458748 cfractions-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2022-12-30 04:16:05.000000 cfractions-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 04:16:15.454748 cfractions-2.2.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)    91343 2022-12-30 04:16:05.000000 cfractions-2.2.0/src/cfractions.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:59:44.589760 cfractions-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-27 00:59:39.000000 cfractions-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-27 00:59:39.000000 cfractions-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-04-27 00:59:44.589760 cfractions-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-04-27 00:59:39.000000 cfractions-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:59:44.589760 cfractions-2.3.0/cfractions/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-27 00:59:39.000000 cfractions-2.3.0/cfractions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12464 2024-04-27 00:59:39.000000 cfractions-2.3.0/cfractions/_fractions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 00:59:39.000000 cfractions-2.3.0/cfractions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:59:44.589760 cfractions-2.3.0/cfractions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-04-27 00:59:44.000000 cfractions-2.3.0/cfractions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-27 00:59:44.000000 cfractions-2.3.0/cfractions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 00:59:44.000000 cfractions-2.3.0/cfractions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 00:59:44.000000 cfractions-2.3.0/cfractions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-27 00:59:44.000000 cfractions-2.3.0/cfractions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-27 00:59:44.000000 cfractions-2.3.0/cfractions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-27 00:59:39.000000 cfractions-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 00:59:44.589760 cfractions-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-27 00:59:39.000000 cfractions-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:59:44.589760 cfractions-2.3.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    91340 2024-04-27 00:59:39.000000 cfractions-2.3.0/src/cfractions.c
```

### Comparing `cfractions-2.2.0/LICENSE` & `cfractions-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cfractions-2.2.0/PKG-INFO` & `cfractions-2.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,9 @@
-Metadata-Version: 2.1
-Name: cfractions
-Version: 2.2.0
-Summary: Python C API alternative to `fractions` module.
-Home-page: https://github.com/lycantropos/cfractions/
-Download-URL: https://github.com/lycantropos/cfractions/archive/master.zip
-Author: Azat Ibrakov
-Author-email: azatibrakov@gmail.com
-License: MIT License
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 cfractions
-==========
+========
 
 [![](https://github.com/lycantropos/cfractions/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/lycantropos/cfractions/actions/workflows/ci.yml "Github Actions")
 [![](https://codecov.io/gh/lycantropos/cfractions/branch/master/graph/badge.svg)](https://codecov.io/gh/lycantropos/cfractions "Codecov")
 [![](https://img.shields.io/github/license/lycantropos/cfractions.svg)](https://github.com/lycantropos/cfractions/blob/master/LICENSE "License")
 [![](https://badge.fury.io/py/cfractions.svg)](https://badge.fury.io/py/cfractions "PyPI")
 
 Summary
@@ -37,16 +16,16 @@
 - speed & memory efficiency compared to pure-`Python` counterpart,
 - full spectre of arithmetic & comparison operations,
 - `Python3.6+` support,
 - `PyPy` support (by falling back to `fractions.Fraction` proxy).
 
 ---
 
-In what follows `python` is an alias for `python3.7` or `pypy3.7`
-or any later version (`python3.8`, `pypy3.8` and so on).
+In what follows `python` is an alias for `python3.8` or `pypy3.8`
+or any later version (`python3.9`, `pypy3.9` and so on).
 
 Installation
 ------------
 
 Install the latest `pip` & `setuptools` packages versions
 ```bash
 python -m pip install --upgrade pip setuptools
@@ -65,15 +44,15 @@
 ```bash
 git clone https://github.com/lycantropos/cfractions.git
 cd cfractions
 ```
 
 Install
 ```bash
-python setup.py install
+python -m pip install -e .
 ```
 
 Usage
 -----
 ```python
 >>> from cfractions import Fraction
 >>> Fraction()
@@ -127,15 +106,15 @@
 values are `patch`/`minor`/`major`.
 
 Bump version
 ```bash
 bump2version --verbose $CATEGORY
 ```
 
-This will set version to `major.minor.patch-alpha`. 
+This will set version to `major.minor.patch-alpha`.
 
 #### Release
 
 Test bumping version
 ```bash
 bump2version --dry-run --verbose release
 ```
@@ -145,17 +124,17 @@
 bump2version --verbose release
 ```
 
 This will set version to `major.minor.patch`.
 
 ### Running tests
 
-Install dependencies
+Install with dependencies
 ```bash
-python -m pip install -r requirements-tests.txt
+python -m pip install -e .[tests]
 ```
 
 Plain
 ```bash
 pytest
 ```
```

### Comparing `cfractions-2.2.0/setup.py` & `cfractions-2.3.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,77 @@
-import platform
-from pathlib import Path
+[project]
+name = "cfractions"
+authors = [{ name = "Azat Ibrakov", email = "azatibrakov@gmail.com" }]
+readme = "README.md"
+license = { file = "LICENSE" }
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Programming Language :: Python :: Implementation :: PyPy",
+]
+requires-python = ">=3.8"
+dependencies = [
+    "typing-extensions>=4.11.0",
+]
+dynamic = ["version"]
+
+[project.optional-dependencies]
+tests = [
+    "hypothesis>=6.100.1,<7.0",
+    "pytest>=8.1.2,<9.0"
+]
+
+[build-system]
+requires = [
+    "setuptools",
+    "wheel"
+]
+build-backend = "setuptools.build_meta"
+
+[tool.coverage.run]
+source = ["cfractions"]
+
+[tool.pytest.ini_options]
+addopts = "--verbose -s --hypothesis-profile=default"
+
+[tool.ruff]
+line-length = 79
+
+[tool.ruff.format]
+docstring-code-format = true
+quote-style = "single"
+skip-magic-trailing-comma = true
+
+[tool.ruff.lint]
+select = [
+    # flake8-bugbear
+    "B",
+    # pycodestyle
+    "E",
+    # Pyflakes
+    "F",
+    # flake8-future-annotations
+    "FA",
+    # isort
+    "I",
+    # flake8-simplify
+    "SIM",
+    # pyupgrade
+    "UP",
+]
+ignore = [
+    "E203", # Whitespace before ':'
+]
+
+[tool.ruff.lint.isort]
+case-sensitive = true
+combine-as-imports = true
+relative-imports-order = "closest-to-furthest"
+split-on-trailing-comma = false
 
-from setuptools import (find_packages,
-                        setup)
-
-import cfractions
-
-project_base_url = 'https://github.com/lycantropos/cfractions/'
-
-
-def read_file(path_string: str) -> str:
-    return Path(path_string).read_text(encoding='utf-8')
-
-
-parameters = dict(
-        name=cfractions.__name__,
-        packages=find_packages(exclude=('tests', 'tests.*')),
-        package_data={cfractions.__name__: ['py.typed', '__init__.pyi']},
-        version=cfractions.__version__,
-        description=cfractions.__doc__,
-        long_description=read_file('README.md'),
-        long_description_content_type='text/markdown',
-        author='Azat Ibrakov',
-        author_email='azatibrakov@gmail.com',
-        license='MIT License',
-        classifiers=[
-            'License :: OSI Approved :: MIT License',
-            'Programming Language :: Python :: 3.7',
-            'Programming Language :: Python :: 3.8',
-            'Programming Language :: Python :: 3.9',
-            'Programming Language :: Python :: 3.10',
-            'Programming Language :: Python :: 3.11',
-            'Programming Language :: Python :: Implementation :: CPython',
-            'Programming Language :: Python :: Implementation :: PyPy',
-        ],
-        url=project_base_url,
-        download_url=project_base_url + 'archive/master.zip',
-        python_requires='>=3.7'
-)
-if platform.python_implementation() == 'CPython':
-    from glob import glob
-
-    from setuptools import Extension
-
-    parameters.update(ext_modules=[Extension(cfractions.__name__ + '._'
-                                             + cfractions.__name__,
-                                             glob('src/*.c'))],
-                      zip_safe=False)
-setup(**parameters)
+[tool.setuptools.dynamic]
+version = { attr = "cfractions.__version__" }
```

### Comparing `cfractions-2.2.0/src/cfractions.c` & `cfractions-2.3.0/src/cfractions.c`

 * *Files 0% similar despite different names*

```diff
@@ -271,16 +271,15 @@
   return index;
 }
 #else
 static Py_ssize_t search_unsigned_PyLong(int kind, const void *data,
                                          Py_ssize_t size, Py_ssize_t start) {
   Py_ssize_t index = start;
   for (; index < size && Py_UNICODE_ISDIGIT(PyUnicode_READ(kind, data, index));
-       ++index)
-    ;
+       ++index);
   return index;
 }
 #endif
 
 static Py_ssize_t search_signed_PyLong(int kind, const void *data,
                                        Py_ssize_t size, Py_ssize_t start) {
   return search_unsigned_PyLong(
@@ -2442,30 +2441,30 @@
 }
 
 static PyMemberDef Fraction_members[] = {
     {"numerator", T_OBJECT_EX, offsetof(FractionObject, numerator), READONLY,
      "Numerator of the fraction."},
     {"denominator", T_OBJECT_EX, offsetof(FractionObject, denominator),
      READONLY, "Denominator of the fraction."},
-    {NULL} /* sentinel */
+    {NULL, 0, 0, 0, NULL} /* sentinel */
 };
 
 static PyMethodDef Fraction_methods[] = {
     {"as_integer_ratio", (PyCFunction)Fraction_as_integer_ratio, METH_NOARGS,
      NULL},
     {"limit_denominator", (PyCFunction)Fraction_limit_denominator, METH_VARARGS,
      NULL},
     {"__ceil__", (PyCFunction)Fraction_ceil, METH_NOARGS, NULL},
     {"__copy__", (PyCFunction)Fraction_copy, METH_NOARGS, NULL},
     {"__deepcopy__", (PyCFunction)Fraction_copy, METH_VARARGS, NULL},
     {"__floor__", (PyCFunction)Fraction_floor, METH_NOARGS, NULL},
     {"__reduce__", (PyCFunction)Fraction_reduce, METH_NOARGS, NULL},
     {"__round__", (PyCFunction)Fraction_round, METH_VARARGS, NULL},
     {"__trunc__", (PyCFunction)Fraction_trunc, METH_NOARGS, NULL},
-    {NULL, NULL} /* sentinel */
+    {NULL, NULL, 0, NULL} /* sentinel */
 };
 
 static PyNumberMethods Fraction_as_number = {
     .nb_absolute = (unaryfunc)Fraction_absolute,
     .nb_add = Fraction_add,
     .nb_bool = (inquiry)Fraction_bool,
     .nb_divmod = Fraction_divmod,
@@ -2481,15 +2480,15 @@
 };
 
 static PyTypeObject FractionType = {
     PyVarObject_HEAD_INIT(NULL, 0).tp_as_number = &Fraction_as_number,
     .tp_basicsize = sizeof(FractionObject),
     .tp_dealloc = (destructor)Fraction_dealloc,
     .tp_doc = PyDoc_STR("Represents rational numbers in the exact form."),
-    .tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE,
+    .tp_flags = Py_TPFLAGS_DEFAULT,
     .tp_hash = (hashfunc)Fraction_hash,
     .tp_itemsize = 0,
     .tp_members = Fraction_members,
     .tp_methods = Fraction_methods,
     .tp_name = "cfractions.Fraction",
     .tp_new = Fraction_new,
     .tp_repr = (reprfunc)Fraction_repr,
```

