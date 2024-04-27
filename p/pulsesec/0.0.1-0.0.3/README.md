# Comparing `tmp/pulsesec-0.0.1.tar.gz` & `tmp/pulsesec-0.0.3.tar.gz`

## Comparing `pulsesec-0.0.1.tar` & `pulsesec-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pulsesec-0.0.1/requirements.txt
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 pulsesec-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pulsesec-0.0.1/examples/classify/main.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pulsesec-0.0.1/pulse/__init__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 pulsesec-0.0.1/pulse/errors.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 pulsesec-0.0.1/pulse/pulse.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 pulsesec-0.0.1/pulse/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pulsesec-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 pulsesec-0.0.1/tests/test_api.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pulsesec-0.0.1/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pulsesec-0.0.1/LICENSE
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 pulsesec-0.0.1/README.md
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 pulsesec-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 pulsesec-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pulsesec-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 pulsesec-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pulsesec-0.0.3/examples/classify/main.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pulsesec-0.0.3/pulse/__init__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 pulsesec-0.0.3/pulse/errors.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 pulsesec-0.0.3/pulse/pulse.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 pulsesec-0.0.3/pulse/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pulsesec-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 pulsesec-0.0.3/tests/test_api.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pulsesec-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pulsesec-0.0.3/LICENSE
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 pulsesec-0.0.3/README.md
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 pulsesec-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 pulsesec-0.0.3/PKG-INFO
```

### Comparing `pulsesec-0.0.1/.github/workflows/publish.yml` & `pulsesec-0.0.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pulsesec-0.0.1/examples/classify/main.py` & `pulsesec-0.0.3/examples/classify/main.py`

 * *Files identical despite different names*

### Comparing `pulsesec-0.0.1/pulse/errors.py` & `pulsesec-0.0.3/pulse/errors.py`

 * *Files identical despite different names*

### Comparing `pulsesec-0.0.1/pulse/pulse.py` & `pulsesec-0.0.3/pulse/pulse.py`

 * *Files identical despite different names*

### Comparing `pulsesec-0.0.1/tests/test_api.py` & `pulsesec-0.0.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pulsesec-0.0.1/.gitignore` & `pulsesec-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pulsesec-0.0.1/LICENSE` & `pulsesec-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pulsesec-0.0.1/README.md` & `pulsesec-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Pulse Security - Python SDK
 
 ## Installation
 
 ```sh
-$ pip install pulsesecurity
+$ pip install pulsesec
 ```
 
 ## Example
 
 ```py
 from pulse import PulseAPI, TokenNotFoundError, TokenUsedError, TokenExpiredError
 import os
```

### Comparing `pulsesec-0.0.1/pyproject.toml` & `pulsesec-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pulsesec"
-version = "0.0.1"
+version = "0.0.3"
 authors = [{ name = "Pulse Security", email = "contact@pulsesecurity.org" }]
 description = "Pulse Security - Python SDK"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = ["aiohttp", "dataclass-wizard"]
 
 [project.urls]
```

### Comparing `pulsesec-0.0.1/PKG-INFO` & `pulsesec-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pulsesec
-Version: 0.0.1
+Version: 0.0.3
 Summary: Pulse Security - Python SDK
 Project-URL: Homepage, https://github.com/pulsesec/pulse-sdk-py
 Project-URL: Issues, https://github.com/pulsesec/pulse-sdk-py/issues
 Author-email: Pulse Security <contact@pulsesecurity.org>
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: aiohttp
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 
 # Pulse Security - Python SDK
 
 ## Installation
 
 ```sh
-$ pip install pulsesecurity
+$ pip install pulsesec
 ```
 
 ## Example
 
 ```py
 from pulse import PulseAPI, TokenNotFoundError, TokenUsedError, TokenExpiredError
 import os
```

