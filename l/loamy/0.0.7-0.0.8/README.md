# Comparing `tmp/loamy-0.0.7.tar.gz` & `tmp/loamy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loamy-0.0.7.tar", max compression
+gzip compressed data, was "loamy-0.0.8.tar", max compression
```

## Comparing `loamy-0.0.7.tar` & `loamy-0.0.8.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1067 2024-04-24 01:45:20.515570 loamy-0.0.7/LICENSE
--rw-r--r--   0        0        0     2973 2024-04-24 01:45:20.515570 loamy-0.0.7/README.md
--rw-r--r--   0        0        0     1340 2024-04-24 01:45:20.515570 loamy-0.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 01:45:20.515570 loamy-0.0.7/src/loamy/__init__.py
--rw-r--r--   0        0        0    10583 2024-04-24 01:45:20.515570 loamy-0.0.7/src/loamy/session.py
--rw-r--r--   0        0        0     3761 1970-01-01 00:00:00.000000 loamy-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-27 20:39:31.899984 loamy-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2972 2024-04-27 20:39:31.899984 loamy-0.0.8/README.md
+-rw-r--r--   0        0        0     1450 2024-04-27 20:39:31.899984 loamy-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-27 20:39:31.899984 loamy-0.0.8/src/loamy/__init__.py
+-rw-r--r--   0        0        0       93 2024-04-27 20:39:31.899984 loamy-0.0.8/src/loamy/py.typed
+-rw-r--r--   0        0        0    10583 2024-04-27 20:39:31.899984 loamy-0.0.8/src/loamy/session.py
+-rw-r--r--   0        0        0     3870 1970-01-01 00:00:00.000000 loamy-0.0.8/PKG-INFO
```

### Comparing `loamy-0.0.7/LICENSE` & `loamy-0.0.8/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Zach Fuller
+Copyright (c) 2024 Zach Fuller
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `loamy-0.0.7/README.md` & `loamy-0.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![PyPI version](https://badge.fury.io/py/loamy.svg)](https://badge.fury.io/py/loamy)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue)](https://img.shields.io/badge/license-MIT-blue)
 
 # Overview
 
-This project allows you to execute a list of http operations asynchronously from within an synchronous context.
+This project allows you to execute a list of http operations asynchronously from within a synchronous context.
 
 It does not care whether you should do this. It simply allows you to do so if you desire.
 
 ## Installing
 
 The package is available via pip.
```

### Comparing `loamy-0.0.7/pyproject.toml` & `loamy-0.0.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "loamy"
-version = "0.0.7"
-description = ""
+version = "0.0.8"
+description = "This project allows you to execute a list of http operations asynchronously from within a synchronous context."
 authors = ["Zach Fuller <zach.fuller1222@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/fullerzz/loamy"
 packages = [{include = "loamy", from = "src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `loamy-0.0.7/src/loamy/session.py` & `loamy-0.0.8/src/loamy/session.py`

 * *Files identical despite different names*

### Comparing `loamy-0.0.7/PKG-INFO` & `loamy-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: loamy
-Version: 0.0.7
-Summary: 
+Version: 0.0.8
+Summary: This project allows you to execute a list of http operations asynchronously from within a synchronous context.
 Home-page: https://github.com/fullerzz/loamy
 License: MIT
 Author: Zach Fuller
 Author-email: zach.fuller1222@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -25,15 +25,15 @@
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![PyPI version](https://badge.fury.io/py/loamy.svg)](https://badge.fury.io/py/loamy)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue)](https://img.shields.io/badge/license-MIT-blue)
 
 # Overview
 
-This project allows you to execute a list of http operations asynchronously from within an synchronous context.
+This project allows you to execute a list of http operations asynchronously from within a synchronous context.
 
 It does not care whether you should do this. It simply allows you to do so if you desire.
 
 ## Installing
 
 The package is available via pip.
```

