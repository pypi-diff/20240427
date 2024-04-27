# Comparing `tmp/pyneople-0.2.6.tar.gz` & `tmp/pyneople-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneople-0.2.6.tar", last modified: Wed Apr 24 14:31:58 2024, max compression
+gzip compressed data, was "pyneople-0.2.7.tar", last modified: Sat Apr 27 10:48:10 2024, max compression
```

## Comparing `pyneople-0.2.6.tar` & `pyneople-0.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:31:58.664324 pyneople-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-24 14:31:45.000000 pyneople-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-24 14:31:58.664324 pyneople-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-24 14:31:45.000000 pyneople-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 14:31:45.000000 pyneople-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:31:58.664324 pyneople-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-24 14:31:45.000000 pyneople-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:31:58.660323 pyneople-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:31:58.660323 pyneople-0.2.6/src/pyneople/
--rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-04-24 14:31:45.000000 pyneople-0.2.6/src/pyneople/METADATA.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 14:31:45.000000 pyneople-0.2.6/src/pyneople/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34094 2024-04-24 14:31:45.000000 pyneople-0.2.6/src/pyneople/character.py
--rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-04-24 14:31:45.000000 pyneople-0.2.6/src/pyneople/database_connecter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-04-24 14:31:45.000000 pyneople-0.2.6/src/pyneople/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:31:58.664324 pyneople-0.2.6/src/pyneople.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-24 14:31:58.000000 pyneople-0.2.6/src/pyneople.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-24 14:31:58.000000 pyneople-0.2.6/src/pyneople.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:31:58.000000 pyneople-0.2.6/src/pyneople.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 14:31:58.000000 pyneople-0.2.6/src/pyneople.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:48:10.984887 pyneople-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-27 10:48:01.000000 pyneople-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-27 10:48:10.984887 pyneople-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-27 10:48:01.000000 pyneople-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-27 10:48:01.000000 pyneople-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 10:48:10.984887 pyneople-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-27 10:48:01.000000 pyneople-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:48:10.980887 pyneople-0.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:48:10.980887 pyneople-0.2.7/src/pyneople/
+-rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-04-27 10:48:01.000000 pyneople-0.2.7/src/pyneople/METADATA.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-27 10:48:01.000000 pyneople-0.2.7/src/pyneople/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34094 2024-04-27 10:48:01.000000 pyneople-0.2.7/src/pyneople/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-04-27 10:48:01.000000 pyneople-0.2.7/src/pyneople/database_connecter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-04-27 10:48:01.000000 pyneople-0.2.7/src/pyneople/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:48:10.980887 pyneople-0.2.7/src/pyneople.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-27 10:48:10.000000 pyneople-0.2.7/src/pyneople.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-27 10:48:10.000000 pyneople-0.2.7/src/pyneople.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 10:48:10.000000 pyneople-0.2.7/src/pyneople.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-27 10:48:10.000000 pyneople-0.2.7/src/pyneople.egg-info/top_level.txt
```

### Comparing `pyneople-0.2.6/LICENSE` & `pyneople-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.6/PKG-INFO` & `pyneople-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.2.6
+Version: 0.2.7
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/pyneople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/pyneople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyneople-0.2.6/setup.py` & `pyneople-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyneople",
-    version="0.2.6",
+    version="0.2.7",
     author="ippo252525",
     author_email="ippo252525@gmail.com",
     description="Neople Open API wrapper for data analyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ippo252525/pyneople",
     project_urls={
```

### Comparing `pyneople-0.2.6/src/pyneople/METADATA.py` & `pyneople-0.2.7/src/pyneople/METADATA.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.6/src/pyneople/character.py` & `pyneople-0.2.7/src/pyneople/character.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.6/src/pyneople/database_connecter.py` & `pyneople-0.2.7/src/pyneople/database_connecter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from .character import CharacterFame, CharacterSearch
 from .functions import get_request, ServerMaintenanceError, PyneopleError
 from multiprocessing import Process, Queue, Value
+from typing import Callable
 from pymongo import MongoClient
 import time
 import psycopg2
 from psycopg2 import sql
 
-def store_data_to_mongodb(
+def store_fame_data_to_mongodb(
         arg_mongo_client_instance : MongoClient,
         arg_database_name : str,
         arg_collection_name : str,
         arg_api_key_list : list[str],
         arg_character_search_instance : CharacterSearch,
         arg_max_fame : int):
     # start_time = time.time()
@@ -94,19 +95,24 @@
             'arg_job_id' : job_id,
             'arg_job_grow_id' : job_grow_id,
             'arg_is_all_job_grow' : True
         }
         args_queue.put(args_dict)        
 
     for process in processes:
-        process.join()           
-                
+        process.join()        
+
 class PostgreSQLConnecter():
     
     def __init__(self, arg_database_connection_dict : dict):
+        """
+        생성자 함수로 database connect의 인자로 전달되는 dict를 입력받는다.
+            Args:
+                arg_database_connection_dict(dict) : psycopg2.connect 함수의 인자로 사용될 dict
+        """
         self.connection = psycopg2.connect(**arg_database_connection_dict)
 
     def execute(self, arg_sql : str):
         '''
         sql문을 실행시키고 commit까지 완료 시키는 함수
             Args:
                 arg_sql(str) : 실행되어야 하는 sql문
@@ -198,8 +204,67 @@
         insert_query = sql.SQL("INSERT INTO {} ({}) VALUES {}").format(
             sql.Identifier(arg_table_name),
             sql.SQL(', ').join(map(sql.Identifier, arg_columns)),
             sql.SQL(', ').join(map(sql.Literal, arg_data))
             )
         if arg_ignore_duplication:
             insert_query += sql.SQL(" ON CONFLICT DO NOTHING") 
-        arg_cursor.execute(insert_query)                    
+        arg_cursor.execute(insert_query)                    
+
+def mongodb_to_postgresql(arg_postgresql_connecter : PostgreSQLConnecter, 
+                          arg_postgresql_table_name : str,
+                          arg_mongo_client : MongoClient, 
+                          arg_mongo_database_name : str,
+                          arg_mongo_collection_name : str,
+                          arg_preprocess_function : Callable, 
+                          batch_size : int = 100):
+    """
+    MomgoDB 에 저장된 데이터를 Postgresql로 전처리 후 batch_size씩 저장하는 함수
+        Args :
+            arg_postgresql_connecter(PostgreSQLConnecter) : pyneople database connecter
+            arg_postgresql_table_name(str) :  저장하려는 PostgreSQL table name
+            arg_mongo_client(MongoClient) : pymongo 의 MongoClient 객체
+            arg_mongo_database_name(str) : MongoDB의 database name
+            arg_mongo_collection_name(str) : MongoDB의 collection name
+            arg_preprocess_function(Callable) : 전처리 함수(input으로 MongoDB의 document가 들어가며 tuple 또는 tuple로 이루어진 list를 반환해야 한다.)
+            batch_size(int) : 한번에 조회, 저장하는 document 개수
+    """
+    postgresql_columns = arg_postgresql_connecter.get_column_names(arg_postgresql_table_name)
+    postgresql_cursor = arg_postgresql_connecter.connection.cursor()
+
+    mongo_database = arg_mongo_client[arg_mongo_database_name]
+    mongo_collection = mongo_database[arg_mongo_collection_name]
+    
+    # 일괄 처리 크기
+    total_data_count = mongo_collection.count_documents({})
+    count = 0
+    # MongoDB 데이터 조회 및 PostgreSQL에 삽입
+    for skip in range(0, total_data_count, batch_size):
+
+        mongo_cursor = mongo_collection.find().skip(skip).limit(batch_size)
+        batch_data = list(mongo_cursor)
+
+        if not batch_data:
+            break
+
+        # PostgreSQL에 데이터 삽입
+        insert_data_list = []
+        for document in batch_data:
+            if isinstance(arg_preprocess_function(document), tuple):
+                insert_data_list.append(arg_preprocess_function(document))
+            elif isinstance(arg_preprocess_function(document), list):
+                insert_data_list += arg_preprocess_function(document)
+            else:
+                TypeError("전처리 함수는 tuple 또는 list of tuple을 반환해야 합니다.")
+        arg_postgresql_connecter.insert_into_table(postgresql_cursor, arg_postgresql_table_name, postgresql_columns, insert_data_list)
+        arg_postgresql_connecter.connection.commit()
+        count += batch_size
+        print(f"{count}/{total_data_count}", end="\r")
+
+        
+    # 연결 종료
+    arg_mongo_client.close()
+    postgresql_cursor.close()
+    arg_postgresql_connecter.connection.close()
+    print("done")    
+
+
```

### Comparing `pyneople-0.2.6/src/pyneople/functions.py` & `pyneople-0.2.7/src/pyneople/functions.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.6/src/pyneople.egg-info/PKG-INFO` & `pyneople-0.2.7/src/pyneople.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.2.6
+Version: 0.2.7
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/pyneople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/pyneople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

