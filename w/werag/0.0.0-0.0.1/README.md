# Comparing `tmp/werag-0.0.0.tar.gz` & `tmp/werag-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "werag-0.0.0.tar", max compression
+gzip compressed data, was "werag-0.0.1.tar", max compression
```

## Comparing `werag-0.0.0.tar` & `werag-0.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2024-04-27 05:08:57.889950 werag-0.0.0/README.md
--rw-r--r--   0        0        0      611 2024-04-27 04:39:25.325221 werag-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-04-27 00:27:15.120287 werag-0.0.0/werag/.DS_Store
--rw-r--r--   0        0        0       25 2024-04-27 03:23:00.642045 werag-0.0.0/werag/__init__.py
--rw-r--r--   0        0        0     6472 2024-04-27 04:49:51.295425 werag-0.0.0/werag/client.py
--rw-r--r--   0        0        0     3811 2024-04-27 04:23:52.514873 werag-0.0.0/werag/crud.py
--rw-r--r--   0        0        0      397 2024-04-27 04:09:42.508612 werag-0.0.0/werag/db.py
--rw-r--r--   0        0        0      976 2024-04-27 02:28:24.575438 werag-0.0.0/werag/schema.py
--rw-r--r--   0        0        0        0 2024-04-27 00:20:44.080530 werag-0.0.0/werag/schemas/__init__.py
--rw-r--r--   0        0        0      818 2024-04-27 00:20:44.080642 werag-0.0.0/werag/schemas/chunk.py
--rw-r--r--   0        0        0      183 2024-04-27 02:33:17.900723 werag-0.0.0/werag/utils.py
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 werag-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-27 05:08:57.889950 werag-0.0.1/README.md
+-rw-r--r--   0        0        0      622 2024-04-27 07:36:31.503567 werag-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-04-27 00:27:15.120287 werag-0.0.1/werag/.DS_Store
+-rw-r--r--   0        0        0       25 2024-04-27 03:23:00.642045 werag-0.0.1/werag/__init__.py
+-rw-r--r--   0        0        0     6198 2024-04-27 05:37:31.637845 werag-0.0.1/werag/client.py
+-rw-r--r--   0        0        0     3811 2024-04-27 04:23:52.514873 werag-0.0.1/werag/crud.py
+-rw-r--r--   0        0        0      397 2024-04-27 04:09:42.508612 werag-0.0.1/werag/db.py
+-rw-r--r--   0        0        0      976 2024-04-27 02:28:24.575438 werag-0.0.1/werag/schema.py
+-rw-r--r--   0        0        0        0 2024-04-27 00:20:44.080530 werag-0.0.1/werag/schemas/__init__.py
+-rw-r--r--   0        0        0      818 2024-04-27 00:20:44.080642 werag-0.0.1/werag/schemas/chunk.py
+-rw-r--r--   0        0        0      183 2024-04-27 02:33:17.900723 werag-0.0.1/werag/utils.py
+-rw-r--r--   0        0        0      844 1970-01-01 00:00:00.000000 werag-0.0.1/PKG-INFO
```

### Comparing `werag-0.0.0/pyproject.toml` & `werag-0.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "werag"
-version = "0.0.0"
+version = "0.0.1"
 description = "python rag for wechat application"
 authors = ["zhenhao-ma <bob0103779@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "<3.13,>=3.10"
 pydantic = "^2.3.0"
@@ -12,14 +12,15 @@
 langchain-community = "^0"
 langchain-openai = "^0.0.2.post1"
 keble-helpers = "^0"
 html2text = "^2024.2.26"
 tenacity = "^8.2.3"
 sentence-transformers = "^2"
 wechatpy = "^1.8.18"
+bs4 = "^0"
 
 [tool.poetry.group.test.dependencies]
 pydantic-settings = "^2.2.1"
 pytest = "^8.1.1"
 
 
 [build-system]
```

### Comparing `werag-0.0.0/werag/.DS_Store` & `werag-0.0.1/werag/.DS_Store`

 * *Files identical despite different names*

### Comparing `werag-0.0.0/werag/client.py` & `werag-0.0.1/werag/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,24 +38,18 @@
             embedding_function = SentenceTransformerEmbeddings(model_name="all-MiniLM-L6-v2")
         self._chroma = get_chroma(collection_name=collection_name, persist_directory=persist_directory,
                                   embedding_function=embedding_function)
 
     def as_retriever(self, *, user: str,
                      content_type: Optional[str] = None,
                      search_type: Literal["similarity", "mmr", "similarity_score_threshold"] = "similarity",
-                     limit: int = 4,
-                     score_threshold: float = 0.8,
-                     fetch_k: int = 20,
-                     lambda_mult: float = 0.5):
+                     **kwargs):
         return self._chroma.as_retriever(search_kwargs={
-            # "k": limit,
-            # "score_threshold": score_threshold,
             "filter": self._crud.get_user_content_filter(user=user, content_type=content_type),
-            # "fetch_k": fetch_k,
-            # "lambda_mult": lambda_mult
+            **kwargs
         }, search_type=search_type)
 
     def save_content(self, *, user: str, content: str,
                      content_type: Optional[str] = None) -> UserContent:
         """Save a content base on user id"""
         return self._crud.save_user_content(client=self._chroma, user=user, content_type=content_type, content=content)
```

### Comparing `werag-0.0.0/werag/crud.py` & `werag-0.0.1/werag/crud.py`

 * *Files identical despite different names*

### Comparing `werag-0.0.0/werag/schema.py` & `werag-0.0.1/werag/schema.py`

 * *Files identical despite different names*

### Comparing `werag-0.0.0/werag/schemas/chunk.py` & `werag-0.0.1/werag/schemas/chunk.py`

 * *Files identical despite different names*

### Comparing `werag-0.0.0/PKG-INFO` & `werag-0.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: werag
-Version: 0.0.0
+Version: 0.0.1
 Summary: python rag for wechat application
 Author: zhenhao-ma
 Author-email: bob0103779@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: bs4 (>=0,<1)
 Requires-Dist: html2text (>=2024.2.26,<2025.0.0)
 Requires-Dist: keble-helpers (>=0,<1)
 Requires-Dist: langchain-chroma (>=0,<1)
 Requires-Dist: langchain-community (>=0,<1)
 Requires-Dist: langchain-openai (>=0.0.2.post1,<0.0.3)
 Requires-Dist: pydantic (>=2.3.0,<3.0.0)
 Requires-Dist: sentence-transformers (>=2,<3)
```

