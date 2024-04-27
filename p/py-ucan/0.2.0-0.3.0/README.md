# Comparing `tmp/py_ucan-0.2.0.tar.gz` & `tmp/py_ucan-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ucan-0.2.0.tar", max compression
+gzip compressed data, was "py_ucan-0.3.0.tar", max compression
```

## Comparing `py_ucan-0.2.0.tar` & `py_ucan-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1066 2024-04-27 09:01:34.283038 py_ucan-0.2.0/LICENSE
--rw-r--r--   0        0        0       10 2024-04-27 06:27:53.422389 py_ucan-0.2.0/README.md
--rw-r--r--   0        0        0    10294 2024-04-27 10:32:04.464089 py_ucan-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1630 2024-04-27 10:27:50.133444 py_ucan-0.2.0/src/ucan/__init__.py
--rw-r--r--   0        0        0      744 2024-04-27 06:27:39.037912 py_ucan-0.2.0/src/ucan/constants.py
--rw-r--r--   0        0        0       30 2024-04-27 07:51:44.150692 py_ucan-0.2.0/src/ucan/core/__init__.py
--rw-r--r--   0        0        0     6739 2024-04-27 07:49:57.900956 py_ucan-0.2.0/src/ucan/core/attenuation.py
--rw-r--r--   0        0        0     1754 2024-04-27 07:42:30.128183 py_ucan-0.2.0/src/ucan/core/plugins.py
--rw-r--r--   0        0        0     1484 2024-04-27 07:43:09.695592 py_ucan-0.2.0/src/ucan/core/semver.py
--rw-r--r--   0        0        0     6704 2024-04-27 07:58:16.682253 py_ucan-0.2.0/src/ucan/core/token.py
--rw-r--r--   0        0        0     4284 2024-04-27 07:50:02.795646 py_ucan-0.2.0/src/ucan/core/types.py
--rw-r--r--   0        0        0     5889 2024-04-27 07:43:46.342187 py_ucan-0.2.0/src/ucan/core/verify.py
--rw-r--r--   0        0        0      181 2024-04-27 06:59:07.757459 py_ucan-0.2.0/src/ucan/default_plugins/__init__.py
--rw-r--r--   0        0        0     2851 2024-04-27 07:43:42.465314 py_ucan-0.2.0/src/ucan/default_plugins/ed25519.py
--rw-r--r--   0        0        0        0 2024-04-27 06:27:39.022503 py_ucan-0.2.0/src/ucan/py.typed
--rw-r--r--   0        0        0      914 2024-04-27 07:42:01.415915 py_ucan-0.2.0/src/ucan/schemas.py
--rw-r--r--   0        0        0      205 2024-04-27 08:59:27.774923 py_ucan-0.2.0/src/ucan/typing.py
--rw-r--r--   0        0        0     2192 2024-04-27 06:44:13.438522 py_ucan-0.2.0/src/ucan/utils.py
--rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 py_ucan-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-27 10:53:59.719839 py_ucan-0.3.0/LICENSE
+-rw-r--r--   0        0        0       10 2024-04-27 10:53:59.719839 py_ucan-0.3.0/README.md
+-rw-r--r--   0        0        0    10294 2024-04-27 10:54:00.675832 py_ucan-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1630 2024-04-27 10:54:00.683832 py_ucan-0.3.0/src/ucan/__init__.py
+-rw-r--r--   0        0        0      744 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/constants.py
+-rw-r--r--   0        0        0       30 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/core/__init__.py
+-rw-r--r--   0        0        0     6739 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/core/attenuation.py
+-rw-r--r--   0        0        0     1754 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/core/plugins.py
+-rw-r--r--   0        0        0     1484 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/core/semver.py
+-rw-r--r--   0        0        0     6735 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/core/token.py
+-rw-r--r--   0        0        0     4284 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/core/types.py
+-rw-r--r--   0        0        0     5889 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/core/verify.py
+-rw-r--r--   0        0        0      181 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/default_plugins/__init__.py
+-rw-r--r--   0        0        0     2851 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/default_plugins/ed25519.py
+-rw-r--r--   0        0        0        0 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/py.typed
+-rw-r--r--   0        0        0      914 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/schemas.py
+-rw-r--r--   0        0        0      205 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/typing.py
+-rw-r--r--   0        0        0     2192 2024-04-27 10:53:59.719839 py_ucan-0.3.0/src/ucan/utils.py
+-rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 py_ucan-0.3.0/PKG-INFO
```

### Comparing `py_ucan-0.2.0/LICENSE` & `py_ucan-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ucan-0.2.0/pyproject.toml` & `py_ucan-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 build-backend = "poetry.core.masonry.api"
 
 # ----------------------------------------------------------------------------------------------------------------------
 # poetry
 [tool.poetry]
 package-mode = true
 name = "py-ucan"
-version = "0.2.0"
+version = "0.3.0"
 description = "Python Ucan"
 readme = "README.md"
 authors = [
     "Subham Agarwal <subhamagr@users.noreply.github.com>",
 ]
 maintainers = []
 # links
```

### Comparing `py_ucan-0.2.0/src/ucan/__init__.py` & `py_ucan-0.3.0/src/ucan/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from ucan.core import attenuation as attenuationlib
 from ucan.core import token as tokenlib
 from ucan.core import verify as verifylib
 from ucan.core.plugins import Plugins
 from ucan.default_plugins import ed25519_plugin, EdKeypair
 
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 
 __all__ = (
     "Plugins",
     "PluginInjectedAPI",
     "default_plugins",
     "injected_api",
```

### Comparing `py_ucan-0.2.0/src/ucan/constants.py` & `py_ucan-0.3.0/src/ucan/constants.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.2.0/src/ucan/core/attenuation.py` & `py_ucan-0.3.0/src/ucan/core/attenuation.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.2.0/src/ucan/core/plugins.py` & `py_ucan-0.3.0/src/ucan/core/plugins.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.2.0/src/ucan/core/semver.py` & `py_ucan-0.3.0/src/ucan/core/semver.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.2.0/src/ucan/core/token.py` & `py_ucan-0.3.0/src/ucan/core/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""ucan.core.token module."""
+
 from __future__ import annotations
 
 import math
 import typing as t
 import typing_extensions as te
 
 import jwt
```

### Comparing `py_ucan-0.2.0/src/ucan/core/types.py` & `py_ucan-0.3.0/src/ucan/core/types.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.2.0/src/ucan/core/verify.py` & `py_ucan-0.3.0/src/ucan/core/verify.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.2.0/src/ucan/default_plugins/ed25519.py` & `py_ucan-0.3.0/src/ucan/default_plugins/ed25519.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.2.0/src/ucan/schemas.py` & `py_ucan-0.3.0/src/ucan/schemas.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.2.0/src/ucan/utils.py` & `py_ucan-0.3.0/src/ucan/utils.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.2.0/PKG-INFO` & `py_ucan-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ucan
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python Ucan
 Home-page: https://github.com/fileverse/py-ucan
 Author: Subham Agarwal
 Author-email: subhamagr@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

