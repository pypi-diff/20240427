# Comparing `tmp/kickthespypet_api-0.0.1.tar.gz` & `tmp/kickthespypet_api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kickthespypet_api-0.0.1.tar", max compression
+gzip compressed data, was "kickthespypet_api-0.0.2.tar", max compression
```

## Comparing `kickthespypet_api-0.0.1.tar` & `kickthespypet_api-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     5230 2024-04-26 23:43:47.433331 kickthespypet_api-0.0.1/kickthespypet_api/__init__.py
--rw-r--r--   0        0        0      231 2024-04-26 23:49:39.655614 kickthespypet_api-0.0.1/kickthespypet_api/types.py
--rw-r--r--   0        0        0    17096 2024-04-26 23:56:57.517072 kickthespypet_api-0.0.1/LICENSE
--rw-r--r--   0        0        0      818 2024-04-27 00:06:49.503510 kickthespypet_api-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      974 2024-04-26 23:53:30.866676 kickthespypet_api-0.0.1/README.md
--rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 kickthespypet_api-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5230 2024-04-26 23:43:47.433331 kickthespypet_api-0.0.2/kickthespypet_api/__init__.py
+-rw-r--r--   0        0        0      231 2024-04-26 23:49:39.655614 kickthespypet_api-0.0.2/kickthespypet_api/types.py
+-rw-r--r--   0        0        0    17096 2024-04-26 23:56:57.517072 kickthespypet_api-0.0.2/LICENSE
+-rw-r--r--   0        0        0      817 2024-04-27 00:08:08.920153 kickthespypet_api-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      974 2024-04-26 23:53:30.866676 kickthespypet_api-0.0.2/README.md
+-rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 kickthespypet_api-0.0.2/PKG-INFO
```

### Comparing `kickthespypet_api-0.0.1/kickthespypet_api/__init__.py` & `kickthespypet_api-0.0.2/kickthespypet_api/__init__.py`

 * *Files identical despite different names*

### Comparing `kickthespypet_api-0.0.1/LICENSE` & `kickthespypet_api-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kickthespypet_api-0.0.1/pyproject.toml` & `kickthespypet_api-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "kickthespypet-api"
-version = "0.0.1"
+version = "0.0.2"
 description = "kickthespy.pet API wrapper"
 authors = ["timelesnesses <timelessnesses@timelessnesses.me>"]
 readme = "README.md"
 package-mode = true
 license = "MPL-2.0"
 repository = "https://github.com/timelessnesses/kickthespypet-api"
 keywords = [
     "async", "python3", "kickthespy.pet", "spy.pet"
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = "^3.9"
 requests = "^2.31.0"
 aiohttp = "^3.9.5"
 
 [tool.poetry.extras]
 orjson = ["orjson"]
 
 [tool.poetry.urls]
```

### Comparing `kickthespypet_api-0.0.1/README.md` & `kickthespypet_api-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `kickthespypet_api-0.0.1/PKG-INFO` & `kickthespypet_api-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: kickthespypet-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: kickthespy.pet API wrapper
 Home-page: https://github.com/timelessnesses/kickthespypet-api
 License: MPL-2.0
 Keywords: async,python3,kickthespy.pet,spy.pet
 Author: timelesnesses
 Author-email: timelessnesses@timelessnesses.me
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: orjson
 Requires-Dist: aiohttp (>=3.9.5,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/timelessnesses/kickthespypet-api/issues
 Project-URL: Repository, https://github.com/timelessnesses/kickthespypet-api
 Description-Content-Type: text/markdown
```

