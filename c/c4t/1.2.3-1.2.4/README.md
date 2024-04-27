# Comparing `tmp/c4t-1.2.3.tar.gz` & `tmp/c4t-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4t-1.2.3.tar", last modified: Thu Apr 25 11:15:28 2024, max compression
+gzip compressed data, was "c4t-1.2.4.tar", last modified: Sat Apr 27 08:07:02 2024, max compression
```

## Comparing `c4t-1.2.3.tar` & `c4t-1.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-25 11:15:28.615374 c4t-1.2.3/
--rw-r--r--   0 pairin    (1000) pairin    (1000)     1063 2024-03-16 17:32:43.000000 c4t-1.2.3/LICENSE
--rw-r--r--   0 pairin    (1000) pairin    (1000)     6275 2024-04-25 11:15:28.615374 c4t-1.2.3/PKG-INFO
--rw-r--r--   0 pairin    (1000) pairin    (1000)     4620 2024-03-29 00:26:43.000000 c4t-1.2.3/README.md
--rw-r--r--   0 pairin    (1000) pairin    (1000)     2117 2024-03-29 00:26:43.000000 c4t-1.2.3/pyproject.toml
--rw-r--r--   0 pairin    (1000) pairin    (1000)       38 2024-04-25 11:15:28.615374 c4t-1.2.3/setup.cfg
--rw-r--r--   0 pairin    (1000) pairin    (1000)      529 2024-03-16 17:32:43.000000 c4t-1.2.3/setup.py
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-25 11:15:28.605374 c4t-1.2.3/src/
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-25 11:15:28.605374 c4t-1.2.3/src/c4t/
--rw-r--r--   0 pairin    (1000) pairin    (1000)    13339 2024-03-29 00:26:43.000000 c4t-1.2.3/src/c4t/__init__.py
--rw-r--r--   0 pairin    (1000) pairin    (1000)     1409 2024-03-16 17:32:43.000000 c4t-1.2.3/src/c4t/cli.py
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-25 11:15:28.605374 c4t-1.2.3/src/c4t.egg-info/
--rw-r--r--   0 pairin    (1000) pairin    (1000)     6275 2024-04-25 11:15:28.000000 c4t-1.2.3/src/c4t.egg-info/PKG-INFO
--rw-r--r--   0 pairin    (1000) pairin    (1000)      279 2024-04-25 11:15:28.000000 c4t-1.2.3/src/c4t.egg-info/SOURCES.txt
--rw-r--r--   0 pairin    (1000) pairin    (1000)        1 2024-04-25 11:15:28.000000 c4t-1.2.3/src/c4t.egg-info/dependency_links.txt
--rw-r--r--   0 pairin    (1000) pairin    (1000)       36 2024-04-25 11:15:28.000000 c4t-1.2.3/src/c4t.egg-info/entry_points.txt
--rw-r--r--   0 pairin    (1000) pairin    (1000)      245 2024-04-25 11:15:28.000000 c4t-1.2.3/src/c4t.egg-info/requires.txt
--rw-r--r--   0 pairin    (1000) pairin    (1000)        4 2024-04-25 11:15:28.000000 c4t-1.2.3/src/c4t.egg-info/top_level.txt
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-25 11:15:28.605374 c4t-1.2.3/tests/
--rw-r--r--   0 pairin    (1000) pairin    (1000)     2941 2024-03-29 00:26:43.000000 c4t-1.2.3/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:07:02.347408 c4t-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-27 08:06:55.000000 c4t-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-04-27 08:07:02.347408 c4t-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-27 08:06:55.000000 c4t-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-27 08:06:55.000000 c4t-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 08:07:02.347408 c4t-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-27 08:06:55.000000 c4t-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:07:02.339408 c4t-1.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:07:02.343408 c4t-1.2.4/src/c4t/
+-rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-04-27 08:06:55.000000 c4t-1.2.4/src/c4t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-27 08:06:55.000000 c4t-1.2.4/src/c4t/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:07:02.343408 c4t-1.2.4/src/c4t.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-04-27 08:07:02.000000 c4t-1.2.4/src/c4t.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-27 08:07:02.000000 c4t-1.2.4/src/c4t.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 08:07:02.000000 c4t-1.2.4/src/c4t.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-27 08:07:02.000000 c4t-1.2.4/src/c4t.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-27 08:07:02.000000 c4t-1.2.4/src/c4t.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-27 08:07:02.000000 c4t-1.2.4/src/c4t.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:07:02.343408 c4t-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-27 08:06:55.000000 c4t-1.2.4/tests/tests.py
```

### Comparing `c4t-1.2.3/LICENSE` & `c4t-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `c4t-1.2.3/PKG-INFO` & `c4t-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4t
-Version: 1.2.3
+Version: 1.2.4
 Summary: Install Chrome for Testing assets.
 Author-email: p4irin <139928764+p4irin@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/p4irin/c4t
 Project-URL: Bug Tracker, https://github.com/p4irin/c4t/issues
 Keywords: chrome,testing,selenium,chromedriver,cft
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -40,15 +40,15 @@
 
 [![Build Status](https://dev.azure.com/p4irin/c4t/_apis/build/status%2Fp4irin.c4t?branchName=master&jobName=BuildAndTest&configuration=BuildAndTest%20Python38)](https://dev.azure.com/p4irin/c4t/_build/latest?definitionId=5&branchName=master)
 ![PyPI - Version](https://img.shields.io/pypi/v/c4t)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/c4t)
 ![PyPI - Format](https://img.shields.io/pypi/format/c4t)
 ![PyPI - License](https://img.shields.io/pypi/l/c4t)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-# c4t: Chrome for Testing - v1.2.3
+# c4t: Chrome for Testing - v1.2.4
 
 Install _Chrome for Testing_ assets. A flavor of Chrome, specifically for testing and a matching chromedriver. The version of assets installed are from the stable channel and currently only for _linux64_ platforms.
 
 ## Why Chrome for Testing?
 
 Taken from [the Chrome Developers Blog](https://developer.chrome.com/blog/chrome-for-testing/)
```

### Comparing `c4t-1.2.3/README.md` & `c4t-1.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [![Build Status](https://dev.azure.com/p4irin/c4t/_apis/build/status%2Fp4irin.c4t?branchName=master&jobName=BuildAndTest&configuration=BuildAndTest%20Python38)](https://dev.azure.com/p4irin/c4t/_build/latest?definitionId=5&branchName=master)
 ![PyPI - Version](https://img.shields.io/pypi/v/c4t)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/c4t)
 ![PyPI - Format](https://img.shields.io/pypi/format/c4t)
 ![PyPI - License](https://img.shields.io/pypi/l/c4t)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-# c4t: Chrome for Testing - v1.2.3
+# c4t: Chrome for Testing - v1.2.4
 
 Install _Chrome for Testing_ assets. A flavor of Chrome, specifically for testing and a matching chromedriver. The version of assets installed are from the stable channel and currently only for _linux64_ platforms.
 
 ## Why Chrome for Testing?
 
 Taken from [the Chrome Developers Blog](https://developer.chrome.com/blog/chrome-for-testing/)
```

### Comparing `c4t-1.2.3/pyproject.toml` & `c4t-1.2.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "c4t"
-version = "1.2.3"
+version = "1.2.4"
 authors = [
   { name="p4irin", email="139928764+p4irin@users.noreply.github.com" },
 ]
 description = "Install Chrome for Testing assets."
 readme = "README.md"
 requires-python = ">=3.8.10"
 keywords = [
@@ -65,15 +65,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 
 [tool.bumpver]
-current_version = "1.2.3"
+current_version = "1.2.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 commit = true
 tag = true
 push = false
```

### Comparing `c4t-1.2.3/setup.py` & `c4t-1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `c4t-1.2.3/src/c4t/__init__.py` & `c4t-1.2.4/src/c4t/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     browser.close()
     browser.quit()
 """
 
 
 __author__ = 'p4irin'
 __email__ = '139928764+p4irin@users.noreply.github.com'
-__version__ = '1.2.3'
+__version__ = '1.2.4'
 
 
 import requests
 import os
 import json
 import wget
 import zipfile
```

### Comparing `c4t-1.2.3/src/c4t/cli.py` & `c4t-1.2.4/src/c4t/cli.py`

 * *Files identical despite different names*

### Comparing `c4t-1.2.3/src/c4t.egg-info/PKG-INFO` & `c4t-1.2.4/src/c4t.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4t
-Version: 1.2.3
+Version: 1.2.4
 Summary: Install Chrome for Testing assets.
 Author-email: p4irin <139928764+p4irin@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/p4irin/c4t
 Project-URL: Bug Tracker, https://github.com/p4irin/c4t/issues
 Keywords: chrome,testing,selenium,chromedriver,cft
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -40,15 +40,15 @@
 
 [![Build Status](https://dev.azure.com/p4irin/c4t/_apis/build/status%2Fp4irin.c4t?branchName=master&jobName=BuildAndTest&configuration=BuildAndTest%20Python38)](https://dev.azure.com/p4irin/c4t/_build/latest?definitionId=5&branchName=master)
 ![PyPI - Version](https://img.shields.io/pypi/v/c4t)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/c4t)
 ![PyPI - Format](https://img.shields.io/pypi/format/c4t)
 ![PyPI - License](https://img.shields.io/pypi/l/c4t)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-# c4t: Chrome for Testing - v1.2.3
+# c4t: Chrome for Testing - v1.2.4
 
 Install _Chrome for Testing_ assets. A flavor of Chrome, specifically for testing and a matching chromedriver. The version of assets installed are from the stable channel and currently only for _linux64_ platforms.
 
 ## Why Chrome for Testing?
 
 Taken from [the Chrome Developers Blog](https://developer.chrome.com/blog/chrome-for-testing/)
```

### Comparing `c4t-1.2.3/tests/tests.py` & `c4t-1.2.4/tests/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import time
 from selenium.webdriver import ChromeOptions, ChromeService, Chrome
 import c4t
 
 __author__ = 'p4irin'
 __email__ = '139928764+p4irin@users.noreply.github.com'
-__version__ = '1.2.3'
+__version__ = '1.2.4'
 
 
 class C4tTests(unittest.TestCase):
 
     class _TestData:
         specific_version_of_assets = '116.0.5794.0'
```

