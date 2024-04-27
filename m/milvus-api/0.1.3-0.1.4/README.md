# Comparing `tmp/milvus_api-0.1.3.tar.gz` & `tmp/milvus_api-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "milvus_api-0.1.3.tar", last modified: Fri Apr 26 01:47:20 2024, max compression
+gzip compressed data, was "milvus_api-0.1.4.tar", last modified: Sat Apr 27 02:58:56 2024, max compression
```

## Comparing `milvus_api-0.1.3.tar` & `milvus_api-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 01:47:20.728681 milvus_api-0.1.3/
--rw-rw-rw-   0        0        0     2811 2024-04-26 01:47:20.728681 milvus_api-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2352 2024-04-26 01:47:08.000000 milvus_api-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 01:47:20.681799 milvus_api-0.1.3/milvus_api/
--rw-rw-rw-   0        0        0        0 2024-04-25 15:55:58.000000 milvus_api-0.1.3/milvus_api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 01:47:20.713056 milvus_api-0.1.3/milvus_api/db_model/
--rw-rw-rw-   0        0        0        0 2024-04-25 13:02:02.000000 milvus_api-0.1.3/milvus_api/db_model/__init__.py
--rw-rw-rw-   0        0        0     5816 2024-04-26 01:37:48.000000 milvus_api-0.1.3/milvus_api/db_model/milvus_db.py
-drwxrwxrwx   0        0        0        0 2024-04-26 01:47:20.728681 milvus_api-0.1.3/milvus_api/embed_model/
--rw-rw-rw-   0        0        0        0 2024-04-25 15:06:57.000000 milvus_api-0.1.3/milvus_api/embed_model/__init__.py
--rw-rw-rw-   0        0        0     1257 2024-04-25 15:29:44.000000 milvus_api-0.1.3/milvus_api/embed_model/bgem3.py
-drwxrwxrwx   0        0        0        0 2024-04-26 01:47:20.713056 milvus_api-0.1.3/milvus_api.egg-info/
--rw-rw-rw-   0        0        0     2811 2024-04-26 01:47:20.000000 milvus_api-0.1.3/milvus_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-04-26 01:47:20.000000 milvus_api-0.1.3/milvus_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 01:47:20.000000 milvus_api-0.1.3/milvus_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2024-04-26 01:47:20.000000 milvus_api-0.1.3/milvus_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-26 01:47:20.000000 milvus_api-0.1.3/milvus_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 01:47:20.728681 milvus_api-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      616 2024-04-26 01:38:13.000000 milvus_api-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 02:58:56.377251 milvus_api-0.1.4/
+-rw-rw-rw-   0        0        0     2883 2024-04-27 02:58:56.377251 milvus_api-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2424 2024-04-27 02:58:35.000000 milvus_api-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 02:58:56.329592 milvus_api-0.1.4/milvus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-25 15:55:58.000000 milvus_api-0.1.4/milvus_api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 02:58:56.361239 milvus_api-0.1.4/milvus_api/db_model/
+-rw-rw-rw-   0        0        0        0 2024-04-25 13:02:02.000000 milvus_api-0.1.4/milvus_api/db_model/__init__.py
+-rw-rw-rw-   0        0        0     5812 2024-04-27 02:49:55.000000 milvus_api-0.1.4/milvus_api/db_model/milvus_db.py
+drwxrwxrwx   0        0        0        0 2024-04-27 02:58:56.372746 milvus_api-0.1.4/milvus_api/embed_model/
+-rw-rw-rw-   0        0        0        0 2024-04-25 15:06:57.000000 milvus_api-0.1.4/milvus_api/embed_model/__init__.py
+-rw-rw-rw-   0        0        0     1257 2024-04-25 15:29:44.000000 milvus_api-0.1.4/milvus_api/embed_model/bgem3.py
+drwxrwxrwx   0        0        0        0 2024-04-27 02:58:56.345605 milvus_api-0.1.4/milvus_api.egg-info/
+-rw-rw-rw-   0        0        0     2883 2024-04-27 02:58:56.000000 milvus_api-0.1.4/milvus_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-04-27 02:58:56.000000 milvus_api-0.1.4/milvus_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 02:58:56.000000 milvus_api-0.1.4/milvus_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2024-04-27 02:58:56.000000 milvus_api-0.1.4/milvus_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-27 02:58:56.000000 milvus_api-0.1.4/milvus_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 02:58:56.377251 milvus_api-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      616 2024-04-27 02:50:03.000000 milvus_api-0.1.4/setup.py
```

### Comparing `milvus_api-0.1.3/PKG-INFO` & `milvus_api-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milvus_api
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Milvus API used for quickly setting up a Milvus vector database
 Author: ShengWen
 Author-email: shengwen8785@example.com
 Description-Content-Type: text/markdown
 Requires-Dist: pymilvus==2.4.0
 Requires-Dist: milvus-model==0.2.0
 Requires-Dist: pydantic==2.7.0
@@ -55,17 +55,20 @@
 model_name = 'bgem3_model'
 
 # Initialize the model
 bgem3 = PyMilvusBGEM3(model_name)
 results = bgem3.encode(query)
 ```
 ## Release Note
-- 0.1.1: Modify this project structure to ensure that users can import 'milvus_api' normally.
-- 0.1.2: (BugFix): Cancel partial information of `info` function.
+- 0.1.4: (BugFix): Fix the logic error when do `search` operation.
 - 0.1.3: (BugFix): Fix the error caused by the non-specific `field` argument during creating collection.
+- 0.1.2: (BugFix): Cancel partial information of `info` function.
+- 0.1.1: Modify this project structure to ensure that users can import 'milvus_api' normally.
+
+
 
 ## Contributions
 Thanks to all developers who contributed to this project. If you would like to contribute code, please follow the existing code style and submit a pull request.
 
 ## Copyright and License
 This project is licensed under the [Apache License 2.0.](https://www.apache.org/licenses/LICENSE-2.0)
```

### Comparing `milvus_api-0.1.3/README.md` & `milvus_api-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -40,17 +40,20 @@
 model_name = 'bgem3_model'
 
 # Initialize the model
 bgem3 = PyMilvusBGEM3(model_name)
 results = bgem3.encode(query)
 ```
 ## Release Note
-- 0.1.1: Modify this project structure to ensure that users can import 'milvus_api' normally.
-- 0.1.2: (BugFix): Cancel partial information of `info` function.
+- 0.1.4: (BugFix): Fix the logic error when do `search` operation.
 - 0.1.3: (BugFix): Fix the error caused by the non-specific `field` argument during creating collection.
+- 0.1.2: (BugFix): Cancel partial information of `info` function.
+- 0.1.1: Modify this project structure to ensure that users can import 'milvus_api' normally.
+
+
 
 ## Contributions
 Thanks to all developers who contributed to this project. If you would like to contribute code, please follow the existing code style and submit a pull request.
 
 ## Copyright and License
 This project is licensed under the [Apache License 2.0.](https://www.apache.org/licenses/LICENSE-2.0)
```

### Comparing `milvus_api-0.1.3/milvus_api/db_model/milvus_db.py` & `milvus_api-0.1.4/milvus_api/db_model/milvus_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             top_k: the number of most similar results to return. Default is 1
             nprobe: the number of most similar clusters to return. Default is 1
             metric_type: to measure the metric of distance between vectors. this setting must be same when you create the collection
 
         Returns:
             results: The contents of 'top_k' similar results
         """
-        if not utility.has_collection(collection_name):  # True if collection exists, false if it does not.
+        if utility.has_collection(collection_name):  # True if collection exists, false if it does not.
             collection = Collection(collection_name)
             # The collection must be loaded before search operation.
             if str(utility.load_state(collection_name)) == "NotLoad":
                 collection.load(replica_number=2)
         else:
             raise ValueError(f"{collection_name} does not existed. Please check your collection name.")
```

### Comparing `milvus_api-0.1.3/milvus_api/embed_model/bgem3.py` & `milvus_api-0.1.4/milvus_api/embed_model/bgem3.py`

 * *Files identical despite different names*

### Comparing `milvus_api-0.1.3/milvus_api.egg-info/PKG-INFO` & `milvus_api-0.1.4/milvus_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milvus-api
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Milvus API used for quickly setting up a Milvus vector database
 Author: ShengWen
 Author-email: shengwen8785@example.com
 Description-Content-Type: text/markdown
 Requires-Dist: pymilvus==2.4.0
 Requires-Dist: milvus-model==0.2.0
 Requires-Dist: pydantic==2.7.0
@@ -55,17 +55,20 @@
 model_name = 'bgem3_model'
 
 # Initialize the model
 bgem3 = PyMilvusBGEM3(model_name)
 results = bgem3.encode(query)
 ```
 ## Release Note
-- 0.1.1: Modify this project structure to ensure that users can import 'milvus_api' normally.
-- 0.1.2: (BugFix): Cancel partial information of `info` function.
+- 0.1.4: (BugFix): Fix the logic error when do `search` operation.
 - 0.1.3: (BugFix): Fix the error caused by the non-specific `field` argument during creating collection.
+- 0.1.2: (BugFix): Cancel partial information of `info` function.
+- 0.1.1: Modify this project structure to ensure that users can import 'milvus_api' normally.
+
+
 
 ## Contributions
 Thanks to all developers who contributed to this project. If you would like to contribute code, please follow the existing code style and submit a pull request.
 
 ## Copyright and License
 This project is licensed under the [Apache License 2.0.](https://www.apache.org/licenses/LICENSE-2.0)
```

### Comparing `milvus_api-0.1.3/setup.py` & `milvus_api-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='milvus_api',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     install_requires=[
         "pymilvus==2.4.0",
         "milvus-model==0.2.0",
         "pydantic==2.7.0",
         "tqdm==4.66.2",
         "FlagEmbedding==1.2.9",
```

