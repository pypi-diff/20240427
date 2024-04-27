# Comparing `tmp/werag-0.0.1.tar.gz` & `tmp/werag-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "werag-0.0.1.tar", max compression
+gzip compressed data, was "werag-0.0.2.tar", max compression
```

## Comparing `werag-0.0.1.tar` & `werag-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2024-04-27 05:08:57.889950 werag-0.0.1/README.md
--rw-r--r--   0        0        0      622 2024-04-27 07:36:31.503567 werag-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-04-27 00:27:15.120287 werag-0.0.1/werag/.DS_Store
--rw-r--r--   0        0        0       25 2024-04-27 03:23:00.642045 werag-0.0.1/werag/__init__.py
--rw-r--r--   0        0        0     6198 2024-04-27 05:37:31.637845 werag-0.0.1/werag/client.py
--rw-r--r--   0        0        0     3811 2024-04-27 04:23:52.514873 werag-0.0.1/werag/crud.py
--rw-r--r--   0        0        0      397 2024-04-27 04:09:42.508612 werag-0.0.1/werag/db.py
--rw-r--r--   0        0        0      976 2024-04-27 02:28:24.575438 werag-0.0.1/werag/schema.py
--rw-r--r--   0        0        0        0 2024-04-27 00:20:44.080530 werag-0.0.1/werag/schemas/__init__.py
--rw-r--r--   0        0        0      818 2024-04-27 00:20:44.080642 werag-0.0.1/werag/schemas/chunk.py
--rw-r--r--   0        0        0      183 2024-04-27 02:33:17.900723 werag-0.0.1/werag/utils.py
--rw-r--r--   0        0        0      844 1970-01-01 00:00:00.000000 werag-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-27 05:08:57.889950 werag-0.0.2/README.md
+-rw-r--r--   0        0        0      640 2024-04-27 09:28:18.653807 werag-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-04-27 00:27:15.120287 werag-0.0.2/werag/.DS_Store
+-rw-r--r--   0        0        0       25 2024-04-27 03:23:00.642045 werag-0.0.2/werag/__init__.py
+-rw-r--r--   0        0        0     6198 2024-04-27 05:37:31.637845 werag-0.0.2/werag/client.py
+-rw-r--r--   0        0        0     3811 2024-04-27 04:23:52.514873 werag-0.0.2/werag/crud.py
+-rw-r--r--   0        0        0      397 2024-04-27 04:09:42.508612 werag-0.0.2/werag/db.py
+-rw-r--r--   0        0        0      976 2024-04-27 02:28:24.575438 werag-0.0.2/werag/schema.py
+-rw-r--r--   0        0        0        0 2024-04-27 00:20:44.080530 werag-0.0.2/werag/schemas/__init__.py
+-rw-r--r--   0        0        0      818 2024-04-27 00:20:44.080642 werag-0.0.2/werag/schemas/chunk.py
+-rw-r--r--   0        0        0      183 2024-04-27 02:33:17.900723 werag-0.0.2/werag/utils.py
+-rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 werag-0.0.2/PKG-INFO
```

### Comparing `werag-0.0.1/pyproject.toml` & `werag-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "werag"
-version = "0.0.1"
+version = "0.0.2"
 description = "python rag for wechat application"
 authors = ["zhenhao-ma <bob0103779@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "<3.13,>=3.10"
 pydantic = "^2.3.0"
 langchain-chroma = "^0"
+chroma = "0.3.29"
 langchain-community = "^0"
 langchain-openai = "^0.0.2.post1"
 keble-helpers = "^0"
 html2text = "^2024.2.26"
 tenacity = "^8.2.3"
 sentence-transformers = "^2"
 wechatpy = "^1.8.18"
```

### Comparing `werag-0.0.1/werag/.DS_Store` & `werag-0.0.2/werag/.DS_Store`

 * *Files identical despite different names*

### Comparing `werag-0.0.1/werag/client.py` & `werag-0.0.2/werag/client.py`

 * *Files identical despite different names*

### Comparing `werag-0.0.1/werag/crud.py` & `werag-0.0.2/werag/crud.py`

 * *Files identical despite different names*

### Comparing `werag-0.0.1/werag/schema.py` & `werag-0.0.2/werag/schema.py`

 * *Files identical despite different names*

### Comparing `werag-0.0.1/werag/schemas/chunk.py` & `werag-0.0.2/werag/schemas/chunk.py`

 * *Files identical despite different names*

### Comparing `werag-0.0.1/PKG-INFO` & `werag-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: werag
-Version: 0.0.1
+Version: 0.0.2
 Summary: python rag for wechat application
 Author: zhenhao-ma
 Author-email: bob0103779@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: bs4 (>=0,<1)
+Requires-Dist: chroma (==0.3.29)
 Requires-Dist: html2text (>=2024.2.26,<2025.0.0)
 Requires-Dist: keble-helpers (>=0,<1)
 Requires-Dist: langchain-chroma (>=0,<1)
 Requires-Dist: langchain-community (>=0,<1)
 Requires-Dist: langchain-openai (>=0.0.2.post1,<0.0.3)
 Requires-Dist: pydantic (>=2.3.0,<3.0.0)
 Requires-Dist: sentence-transformers (>=2,<3)
```

