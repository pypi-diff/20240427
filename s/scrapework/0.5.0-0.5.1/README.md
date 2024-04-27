# Comparing `tmp/scrapework-0.5.0.tar.gz` & `tmp/scrapework-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapework-0.5.0.tar", max compression
+gzip compressed data, was "scrapework-0.5.1.tar", max compression
```

## Comparing `scrapework-0.5.0.tar` & `scrapework-0.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4204 2024-04-27 04:36:13.284043 scrapework-0.5.0/README.md
--rw-r--r--   0        0        0      897 2024-04-27 04:36:23.592099 scrapework-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-27 04:36:13.284043 scrapework-0.5.0/scrapework/__init__.py
--rw-r--r--   0        0        0     2265 2024-04-27 04:36:13.284043 scrapework-0.5.0/scrapework/cache.py
--rw-r--r--   0        0        0        0 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/core/__init__.py
--rw-r--r--   0        0        0      506 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/core/collector.py
--rw-r--r--   0        0        0      567 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/core/context.py
--rw-r--r--   0        0        0      424 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/core/http_client.py
--rw-r--r--   0        0        0      873 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/core/logger.py
--rw-r--r--   0        0        0     2435 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/handlers.py
--rw-r--r--   0        0        0     3729 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/items.py
--rw-r--r--   0        0        0     2979 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/middleware.py
--rw-r--r--   0        0        0      221 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/module.py
--rw-r--r--   0        0        0      194 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/monitors.py
--rw-r--r--   0        0        0      862 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/observer.py
--rw-r--r--   0        0        0      979 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/parsers.py
--rw-r--r--   0        0        0      546 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/processors.py
--rw-r--r--   0        0        0     3258 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/reporter.py
--rw-r--r--   0        0        0     4638 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/request.py
--rw-r--r--   0        0        0     5901 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/scraper.py
--rw-r--r--   0        0        0     5254 1970-01-01 00:00:00.000000 scrapework-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     4204 2024-04-27 04:41:09.272196 scrapework-0.5.1/README.md
+-rw-r--r--   0        0        0      897 2024-04-27 04:41:21.768247 scrapework-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-27 04:41:09.276196 scrapework-0.5.1/scrapework/__init__.py
+-rw-r--r--   0        0        0     2265 2024-04-27 04:41:09.276196 scrapework-0.5.1/scrapework/cache.py
+-rw-r--r--   0        0        0        0 2024-04-27 04:41:09.276196 scrapework-0.5.1/scrapework/core/__init__.py
+-rw-r--r--   0        0        0      506 2024-04-27 04:41:09.276196 scrapework-0.5.1/scrapework/core/collector.py
+-rw-r--r--   0        0        0      567 2024-04-27 04:41:09.276196 scrapework-0.5.1/scrapework/core/context.py
+-rw-r--r--   0        0        0      424 2024-04-27 04:41:09.276196 scrapework-0.5.1/scrapework/core/http_client.py
+-rw-r--r--   0        0        0      873 2024-04-27 04:41:09.276196 scrapework-0.5.1/scrapework/core/logger.py
+-rw-r--r--   0        0        0     2435 2024-04-27 04:41:09.276196 scrapework-0.5.1/scrapework/handlers.py
+-rw-r--r--   0        0        0     3729 2024-04-27 04:41:09.276196 scrapework-0.5.1/scrapework/items.py
+-rw-r--r--   0        0        0     2979 2024-04-27 04:41:09.276196 scrapework-0.5.1/scrapework/middleware.py
+-rw-r--r--   0        0        0      221 2024-04-27 04:41:09.276196 scrapework-0.5.1/scrapework/module.py
+-rw-r--r--   0        0        0      194 2024-04-27 04:41:09.276196 scrapework-0.5.1/scrapework/monitors.py
+-rw-r--r--   0        0        0      862 2024-04-27 04:41:09.276196 scrapework-0.5.1/scrapework/observer.py
+-rw-r--r--   0        0        0      979 2024-04-27 04:41:09.276196 scrapework-0.5.1/scrapework/parsers.py
+-rw-r--r--   0        0        0      546 2024-04-27 04:41:09.276196 scrapework-0.5.1/scrapework/processors.py
+-rw-r--r--   0        0        0     3258 2024-04-27 04:41:09.276196 scrapework-0.5.1/scrapework/reporter.py
+-rw-r--r--   0        0        0     4638 2024-04-27 04:41:09.276196 scrapework-0.5.1/scrapework/request.py
+-rw-r--r--   0        0        0     5901 2024-04-27 04:41:09.276196 scrapework-0.5.1/scrapework/scraper.py
+-rw-r--r--   0        0        0     5254 1970-01-01 00:00:00.000000 scrapework-0.5.1/PKG-INFO
```

### Comparing `scrapework-0.5.0/README.md` & `scrapework-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.0/pyproject.toml` & `scrapework-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapework"
-version = "v0.5.0"
+version = "v0.5.1"
 description = "simple scraping framework"
 authors = ["Stéphane Busso <stephane.busso@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sbusso/scrapework"
 homepage = "https://github.com/sbusso/scrapework"
```

### Comparing `scrapework-0.5.0/scrapework/cache.py` & `scrapework-0.5.1/scrapework/cache.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.0/scrapework/core/context.py` & `scrapework-0.5.1/scrapework/core/context.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.0/scrapework/core/logger.py` & `scrapework-0.5.1/scrapework/core/logger.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.0/scrapework/handlers.py` & `scrapework-0.5.1/scrapework/handlers.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.0/scrapework/items.py` & `scrapework-0.5.1/scrapework/items.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.0/scrapework/middleware.py` & `scrapework-0.5.1/scrapework/middleware.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.0/scrapework/observer.py` & `scrapework-0.5.1/scrapework/observer.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.0/scrapework/parsers.py` & `scrapework-0.5.1/scrapework/parsers.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.0/scrapework/processors.py` & `scrapework-0.5.1/scrapework/processors.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.0/scrapework/reporter.py` & `scrapework-0.5.1/scrapework/reporter.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.0/scrapework/request.py` & `scrapework-0.5.1/scrapework/request.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.0/scrapework/scraper.py` & `scrapework-0.5.1/scrapework/scraper.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.0/PKG-INFO` & `scrapework-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapework
-Version: 0.5.0
+Version: 0.5.1
 Summary: simple scraping framework
 Home-page: https://github.com/sbusso/scrapework
 License: MIT
 Author: Stéphane Busso
 Author-email: stephane.busso@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

