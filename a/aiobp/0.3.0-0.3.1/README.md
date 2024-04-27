# Comparing `tmp/aiobp-0.3.0.tar.gz` & `tmp/aiobp-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiobp-0.3.0.tar", max compression
+gzip compressed data, was "aiobp-0.3.1.tar", max compression
```

## Comparing `aiobp-0.3.0.tar` & `aiobp-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1057 2024-01-29 17:17:42.453698 aiobp-0.3.0/LICENSE
--rw-r--r--   0        0        0     2455 2024-02-20 15:29:36.631957 aiobp-0.3.0/README.md
--rw-r--r--   0        0        0      177 2024-01-29 17:22:10.519225 aiobp-0.3.0/aiobp/__init__.py
--rw-r--r--   0        0        0      665 2024-01-29 16:50:33.893664 aiobp-0.3.0/aiobp/config/__init__.py
--rw-r--r--   0        0        0     3215 2024-02-20 16:08:04.633393 aiobp-0.3.0/aiobp/config/annotations.py
--rw-r--r--   0        0        0     1395 2024-02-20 15:49:52.311481 aiobp-0.3.0/aiobp/config/conf.py
--rw-r--r--   0        0        0      329 2024-01-29 15:02:53.137137 aiobp-0.3.0/aiobp/config/exceptions.py
--rw-r--r--   0        0        0     1182 2024-02-20 15:50:44.138554 aiobp-0.3.0/aiobp/config/json.py
--rw-r--r--   0        0        0      164 2024-01-29 17:01:49.865893 aiobp-0.3.0/aiobp/logging/__init__.py
--rw-r--r--   0        0        0     3660 2024-04-26 15:53:53.276368 aiobp-0.3.0/aiobp/logging/custom.py
--rw-r--r--   0        0        0      304 2024-01-29 14:10:35.443889 aiobp-0.3.0/aiobp/logging/log.py
--rw-r--r--   0        0        0     9133 2024-04-26 13:26:30.776470 aiobp-0.3.0/aiobp/runner.py
--rw-r--r--   0        0        0      989 2024-04-26 15:55:12.033670 aiobp-0.3.0/aiobp/task.py
--rw-r--r--   0        0        0      397 2024-04-26 15:56:03.810755 aiobp-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2888 1970-01-01 00:00:00.000000 aiobp-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2024-04-27 19:39:01.104119 aiobp-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2455 2024-04-27 19:39:01.104119 aiobp-0.3.1/README.md
+-rw-r--r--   0        0        0      177 2024-04-27 19:39:01.104119 aiobp-0.3.1/aiobp/__init__.py
+-rw-r--r--   0        0        0      665 2024-04-27 19:39:01.104119 aiobp-0.3.1/aiobp/config/__init__.py
+-rw-r--r--   0        0        0     3215 2024-04-27 19:39:01.104119 aiobp-0.3.1/aiobp/config/annotations.py
+-rw-r--r--   0        0        0     1395 2024-04-27 19:39:01.104119 aiobp-0.3.1/aiobp/config/conf.py
+-rw-r--r--   0        0        0      329 2024-04-27 19:39:01.104119 aiobp-0.3.1/aiobp/config/exceptions.py
+-rw-r--r--   0        0        0     1182 2024-04-27 19:39:01.104119 aiobp-0.3.1/aiobp/config/json.py
+-rw-r--r--   0        0        0      164 2024-04-27 19:39:01.104119 aiobp-0.3.1/aiobp/logging/__init__.py
+-rw-r--r--   0        0        0     3677 2024-04-27 19:56:51.762480 aiobp-0.3.1/aiobp/logging/custom.py
+-rw-r--r--   0        0        0      304 2024-04-27 19:39:01.104119 aiobp-0.3.1/aiobp/logging/log.py
+-rw-r--r--   0        0        0     9133 2024-04-27 19:39:01.104119 aiobp-0.3.1/aiobp/runner.py
+-rw-r--r--   0        0        0      989 2024-04-27 19:39:01.104119 aiobp-0.3.1/aiobp/task.py
+-rw-r--r--   0        0        0      397 2024-04-27 19:57:48.895651 aiobp-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2888 1970-01-01 00:00:00.000000 aiobp-0.3.1/PKG-INFO
```

### Comparing `aiobp-0.3.0/LICENSE` & `aiobp-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiobp-0.3.0/README.md` & `aiobp-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `aiobp-0.3.0/aiobp/config/__init__.py` & `aiobp-0.3.1/aiobp/config/__init__.py`

 * *Files identical despite different names*

### Comparing `aiobp-0.3.0/aiobp/config/annotations.py` & `aiobp-0.3.1/aiobp/config/annotations.py`

 * *Files identical despite different names*

### Comparing `aiobp-0.3.0/aiobp/config/conf.py` & `aiobp-0.3.1/aiobp/config/conf.py`

 * *Files identical despite different names*

### Comparing `aiobp-0.3.0/aiobp/config/json.py` & `aiobp-0.3.1/aiobp/config/json.py`

 * *Files identical despite different names*

### Comparing `aiobp-0.3.0/aiobp/logging/custom.py` & `aiobp-0.3.1/aiobp/logging/custom.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Customize Python logger"""
 
 import logging
 import logging.handlers
 import sys
 
-from typing import Optional, Type, TracebackType
+from types import TracebackType
+from typing import Optional, Type
 
 
 class LoggingConfig:
     """Loging configuration"""
 
     level: str = 'DEBUG'
     filename: Optional[str] = None
```

### Comparing `aiobp-0.3.0/aiobp/runner.py` & `aiobp-0.3.1/aiobp/runner.py`

 * *Files identical despite different names*

### Comparing `aiobp-0.3.0/aiobp/task.py` & `aiobp-0.3.1/aiobp/task.py`

 * *Files identical despite different names*

### Comparing `aiobp-0.3.0/PKG-INFO` & `aiobp-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiobp
-Version: 0.3.0
+Version: 0.3.1
 Summary: Boilerplate for asyncio service
 Author: INSOFT s.r.o.
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

