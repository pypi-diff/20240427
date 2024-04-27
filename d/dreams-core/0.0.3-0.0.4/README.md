# Comparing `tmp/dreams_core-0.0.3.tar.gz` & `tmp/dreams_core-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreams_core-0.0.3.tar", last modified: Thu Apr 25 05:02:35 2024, max compression
+gzip compressed data, was "dreams_core-0.0.4.tar", last modified: Sat Apr 27 00:23:00 2024, max compression
```

## Comparing `dreams_core-0.0.3.tar` & `dreams_core-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-04-25 05:02:35.195826 dreams_core-0.0.3/
--rw-r--r--   0 jeremy     (502) staff       (20)     1126 2024-04-24 21:32:45.000000 dreams_core-0.0.3/LICENSE
--rw-r--r--   0 jeremy     (502) staff       (20)      178 2024-04-25 04:05:52.000000 dreams_core-0.0.3/MANIFEST.in
--rw-r--r--   0 jeremy     (502) staff       (20)     1187 2024-04-25 05:02:35.195621 dreams_core-0.0.3/PKG-INFO
--rw-r--r--   0 jeremy     (502) staff       (20)      317 2024-04-24 22:09:04.000000 dreams_core-0.0.3/README.md
--rw-r--r--   0 jeremy     (502) staff       (20)      884 2024-04-25 05:01:18.000000 dreams_core-0.0.3/pyproject.toml
--rw-r--r--   0 jeremy     (502) staff       (20)       38 2024-04-25 05:02:35.195864 dreams_core-0.0.3/setup.cfg
-drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-04-25 05:02:35.193025 dreams_core-0.0.3/src/
-drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-04-25 05:02:35.194702 dreams_core-0.0.3/src/dreams_core/
--rw-r--r--   0 jeremy     (502) staff       (20)       21 2024-04-25 04:05:26.000000 dreams_core-0.0.3/src/dreams_core/__init__.py
--rw-r--r--   0 jeremy     (502) staff       (20)     4454 2024-04-25 04:03:22.000000 dreams_core-0.0.3/src/dreams_core/bigquery.py
--rw-r--r--   0 jeremy     (502) staff       (20)     5245 2024-04-25 04:03:30.000000 dreams_core-0.0.3/src/dreams_core/core.py
--rw-r--r--   0 jeremy     (502) staff       (20)     3897 2024-04-25 04:03:45.000000 dreams_core-0.0.3/src/dreams_core/dune.py
-drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-04-25 05:02:35.195400 dreams_core-0.0.3/src/dreams_core.egg-info/
--rw-r--r--   0 jeremy     (502) staff       (20)     1187 2024-04-25 05:02:35.000000 dreams_core-0.0.3/src/dreams_core.egg-info/PKG-INFO
--rw-r--r--   0 jeremy     (502) staff       (20)      394 2024-04-25 05:02:35.000000 dreams_core-0.0.3/src/dreams_core.egg-info/SOURCES.txt
--rw-r--r--   0 jeremy     (502) staff       (20)        1 2024-04-25 05:02:35.000000 dreams_core-0.0.3/src/dreams_core.egg-info/dependency_links.txt
--rw-r--r--   0 jeremy     (502) staff       (20)      159 2024-04-25 05:02:35.000000 dreams_core-0.0.3/src/dreams_core.egg-info/requires.txt
--rw-r--r--   0 jeremy     (502) staff       (20)       12 2024-04-25 05:02:35.000000 dreams_core-0.0.3/src/dreams_core.egg-info/top_level.txt
+drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-04-27 00:23:00.217876 dreams_core-0.0.4/
+-rw-r--r--   0 jeremy     (502) staff       (20)     1126 2024-04-24 21:32:45.000000 dreams_core-0.0.4/LICENSE
+-rw-r--r--   0 jeremy     (502) staff       (20)      178 2024-04-25 04:05:52.000000 dreams_core-0.0.4/MANIFEST.in
+-rw-r--r--   0 jeremy     (502) staff       (20)     1187 2024-04-27 00:23:00.217655 dreams_core-0.0.4/PKG-INFO
+-rw-r--r--   0 jeremy     (502) staff       (20)      317 2024-04-24 22:09:04.000000 dreams_core-0.0.4/README.md
+-rw-r--r--   0 jeremy     (502) staff       (20)      884 2024-04-27 00:22:36.000000 dreams_core-0.0.4/pyproject.toml
+-rw-r--r--   0 jeremy     (502) staff       (20)       38 2024-04-27 00:23:00.217932 dreams_core-0.0.4/setup.cfg
+drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-04-27 00:23:00.215402 dreams_core-0.0.4/src/
+drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-04-27 00:23:00.216578 dreams_core-0.0.4/src/dreams_core/
+-rw-r--r--   0 jeremy     (502) staff       (20)       21 2024-04-27 00:22:32.000000 dreams_core-0.0.4/src/dreams_core/__init__.py
+-rw-r--r--   0 jeremy     (502) staff       (20)     5233 2024-04-27 00:20:21.000000 dreams_core-0.0.4/src/dreams_core/core.py
+-rw-r--r--   0 jeremy     (502) staff       (20)     3897 2024-04-25 04:03:45.000000 dreams_core-0.0.4/src/dreams_core/dune.py
+-rw-r--r--   0 jeremy     (502) staff       (20)     4457 2024-04-27 00:12:49.000000 dreams_core-0.0.4/src/dreams_core/googlecloud.py
+drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-04-27 00:23:00.217414 dreams_core-0.0.4/src/dreams_core.egg-info/
+-rw-r--r--   0 jeremy     (502) staff       (20)     1187 2024-04-27 00:23:00.000000 dreams_core-0.0.4/src/dreams_core.egg-info/PKG-INFO
+-rw-r--r--   0 jeremy     (502) staff       (20)      369 2024-04-27 00:23:00.000000 dreams_core-0.0.4/src/dreams_core.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremy     (502) staff       (20)        1 2024-04-27 00:23:00.000000 dreams_core-0.0.4/src/dreams_core.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremy     (502) staff       (20)      159 2024-04-27 00:23:00.000000 dreams_core-0.0.4/src/dreams_core.egg-info/requires.txt
+-rw-r--r--   0 jeremy     (502) staff       (20)       12 2024-04-27 00:23:00.000000 dreams_core-0.0.4/src/dreams_core.egg-info/top_level.txt
```

### Comparing `dreams_core-0.0.3/LICENSE` & `dreams_core-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dreams_core-0.0.3/PKG-INFO` & `dreams_core-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreams_core
-Version: 0.0.3
+Version: 0.0.4
 Summary: brought to you by the dreamslabs discord community
 Author-email: tentabs <tentabs00@gmail.com>
 Project-URL: Community, https://discord.gg/dreamcrypto
 Project-URL: Github, https://github.com/dreams-labs/core-functions
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `dreams_core-0.0.3/pyproject.toml` & `dreams_core-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dreams_core"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="tentabs", email="tentabs00@gmail.com" },
 ]
 description = "brought to you by the dreamslabs discord community"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
```

### Comparing `dreams_core-0.0.3/src/dreams_core/bigquery.py` & `dreams_core-0.0.4/src/dreams_core/googlecloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import datetime
 import os
 import pandas as pd
 from google.cloud import bigquery
 from google.oauth2 import service_account
 from google.cloud import storage
 
-class BigQuery:
+class GoogleCloud:
     ''' 
     A class to interact with BigQuery. This class is designed
     to be used in the context of the Dreams project. It is not
     intended to be a general purpose BigQuery class.
 
     Params: 
         service_account_json (str): Path to the service account JSON file. if no value is input then
```

### Comparing `dreams_core-0.0.3/src/dreams_core/core.py` & `dreams_core-0.0.4/src/dreams_core/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 individual tools such as dune/bigquery/etc are available in other modules within this directory. 
 '''
 
 import numpy as np
 import google.auth
 from google.cloud import secretmanager_v1
 from google.oauth2 import service_account
-from .bigquery import BigQuery
+from .googlecloud import GoogleCloud as dgc
 
 
 def human_format(number):
     '''
     converts a number to a scaled human readable string (e.g 7437283-->7.4M)
 
     logic:
@@ -114,16 +114,15 @@
     query_sql = '''
         select cn.chain_id
         ,cn.chain_reference
         ,ch.*
         from reference.chain_nicknames cn
         left join core.chains ch on ch.chain_id = cn.chain_id
         '''
-    bq = BigQuery()
-    chain_nicknames_df = BigQuery().cache_sql(query_sql,'chain_nicknames')
+    chain_nicknames_df = dgc().cache_sql(query_sql,'chain_nicknames')
 
     # set everything to be lower case
     chain_nicknames_df['chain_reference'] = chain_nicknames_df['chain_reference'].str.lower()
     input_chain = input_chain.lower()
 
 
     # filter the df of all aliases for the input chain
```

### Comparing `dreams_core-0.0.3/src/dreams_core/dune.py` & `dreams_core-0.0.4/src/dreams_core/dune.py`

 * *Files identical despite different names*

### Comparing `dreams_core-0.0.3/src/dreams_core.egg-info/PKG-INFO` & `dreams_core-0.0.4/src/dreams_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreams_core
-Version: 0.0.3
+Version: 0.0.4
 Summary: brought to you by the dreamslabs discord community
 Author-email: tentabs <tentabs00@gmail.com>
 Project-URL: Community, https://discord.gg/dreamcrypto
 Project-URL: Github, https://github.com/dreams-labs/core-functions
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

