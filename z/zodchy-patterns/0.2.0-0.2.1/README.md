# Comparing `tmp/zodchy_patterns-0.2.0.tar.gz` & `tmp/zodchy_patterns-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodchy_patterns-0.2.0.tar", max compression
+gzip compressed data, was "zodchy_patterns-0.2.1.tar", max compression
```

## Comparing `zodchy_patterns-0.2.0.tar` & `zodchy_patterns-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       17 2024-04-13 13:27:36.273813 zodchy_patterns-0.2.0/README.md
--rw-r--r--   0        0        0      435 2024-04-18 15:44:02.099131 zodchy_patterns-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       42 2024-04-18 15:44:02.094165 zodchy_patterns-0.2.0/zodchy_patterns/__init__.py
--rw-r--r--   0        0        0      368 2024-04-18 15:44:02.102702 zodchy_patterns-0.2.0/zodchy_patterns/events/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 15:27:46.945461 zodchy_patterns-0.2.0/zodchy_patterns/events/io/__init__.py
--rw-r--r--   0        0        0     1771 2024-04-18 15:44:02.106121 zodchy_patterns-0.2.0/zodchy_patterns/events/io/error.py
--rw-r--r--   0        0        0      314 2024-04-18 15:44:02.089184 zodchy_patterns-0.2.0/zodchy_patterns/events/io/generic.py
--rw-r--r--   0        0        0     1095 2024-04-18 15:44:02.083540 zodchy_patterns-0.2.0/zodchy_patterns/events/io/info.py
--rw-r--r--   0        0        0      499 2024-04-11 07:57:07.720475 zodchy_patterns-0.2.0/zodchy_patterns/mapping.py
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 zodchy_patterns-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-04-13 13:27:36.273813 zodchy_patterns-0.2.1/README.md
+-rw-r--r--   0        0        0      435 2024-04-27 11:27:06.984056 zodchy_patterns-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-04-18 15:44:02.094165 zodchy_patterns-0.2.1/zodchy_patterns/__init__.py
+-rw-r--r--   0        0        0      368 2024-04-18 15:44:02.102702 zodchy_patterns-0.2.1/zodchy_patterns/events/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:27:46.945461 zodchy_patterns-0.2.1/zodchy_patterns/events/io/__init__.py
+-rw-r--r--   0        0        0     1776 2024-04-27 11:27:06.970090 zodchy_patterns-0.2.1/zodchy_patterns/events/io/error.py
+-rw-r--r--   0        0        0      319 2024-04-27 11:27:06.976528 zodchy_patterns-0.2.1/zodchy_patterns/events/io/generic.py
+-rw-r--r--   0        0        0     1095 2024-04-18 15:44:02.083540 zodchy_patterns-0.2.1/zodchy_patterns/events/io/info.py
+-rw-r--r--   0        0        0      499 2024-04-11 07:57:07.720475 zodchy_patterns-0.2.1/zodchy_patterns/mapping.py
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 zodchy_patterns-0.2.1/PKG-INFO
```

### Comparing `zodchy_patterns-0.2.0/zodchy_patterns/events/io/error.py` & `zodchy_patterns-0.2.1/zodchy_patterns/events/io/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import dataclasses
 from zodchy import codex
 
 from . import generic
 
 
 @dataclasses.dataclass
-class HttpError(generic.HttpEvent, codex.Error):
+class HttpError(generic.HttpEvent, codex.cqea.Error):
     code: int = 500
     message: str | None = None
     details: dict | None = None
 
     def get_content(self) -> dict:
         details = self.details or {}
         for field in dataclasses.fields(self):
```

### Comparing `zodchy_patterns-0.2.0/zodchy_patterns/events/io/info.py` & `zodchy_patterns-0.2.1/zodchy_patterns/events/io/info.py`

 * *Files identical despite different names*

### Comparing `zodchy_patterns-0.2.0/PKG-INFO` & `zodchy_patterns-0.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: zodchy-patterns
-Version: 0.2.0
+Version: 0.2.1
 Summary: Collection of patterns to use in CQRS applications
 Home-page: https://github.com/smairon/zodchy-patterns
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: zodchy (>=0.1.0,<0.2.0)
+Requires-Dist: zodchy (>=0.2.0,<0.3.0)
 Project-URL: Repository, https://github.com/smairon/zodchy-patterns
 Description-Content-Type: text/markdown
 
 # Zodchy patterns
```

