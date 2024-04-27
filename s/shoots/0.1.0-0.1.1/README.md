# Comparing `tmp/shoots-0.1.0.tar.gz` & `tmp/shoots-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shoots-0.1.0.tar", last modified: Sat Feb 24 14:10:55 2024, max compression
+gzip compressed data, was "shoots-0.1.1.tar", last modified: Sat Apr 27 12:19:33 2024, max compression
```

## Comparing `shoots-0.1.0.tar` & `shoots-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 rickspencer   (501) staff       (20)        0 2024-02-24 14:10:55.521392 shoots-0.1.0/
--rw-r--r--   0 rickspencer   (501) staff       (20)     1059 2024-02-24 13:45:13.000000 shoots-0.1.0/LICENSE
--rw-r--r--   0 rickspencer   (501) staff       (20)    11244 2024-02-24 14:10:55.521112 shoots-0.1.0/PKG-INFO
--rw-r--r--   0 rickspencer   (501) staff       (20)    10529 2024-02-24 13:45:50.000000 shoots-0.1.0/README.md
--rw-r--r--   0 rickspencer   (501) staff       (20)       38 2024-02-24 14:10:55.521437 shoots-0.1.0/setup.cfg
--rw-r--r--   0 rickspencer   (501) staff       (20)     1016 2024-02-24 13:29:00.000000 shoots-0.1.0/setup.py
-drwxr-xr-x   0 rickspencer   (501) staff       (20)        0 2024-02-24 14:10:55.518002 shoots-0.1.0/shoots/
--rw-r--r--   0 rickspencer   (501) staff       (20)      217 2024-02-10 22:52:03.000000 shoots-0.1.0/shoots/__init__.py
--rw-r--r--   0 rickspencer   (501) staff       (20)      294 2024-02-10 22:35:05.000000 shoots-0.1.0/shoots/jwt_client_auth_handler.py
--rw-r--r--   0 rickspencer   (501) staff       (20)     3038 2024-02-10 22:35:05.000000 shoots-0.1.0/shoots/jwt_server_auth.py
--rw-r--r--   0 rickspencer   (501) staff       (20)    23725 2024-02-11 21:11:35.000000 shoots-0.1.0/shoots/shoots_client.py
--rw-r--r--   0 rickspencer   (501) staff       (20)    24054 2024-02-24 13:37:42.000000 shoots-0.1.0/shoots/shoots_server.py
-drwxr-xr-x   0 rickspencer   (501) staff       (20)        0 2024-02-24 14:10:55.520671 shoots-0.1.0/shoots.egg-info/
--rw-r--r--   0 rickspencer   (501) staff       (20)    11244 2024-02-24 14:10:55.000000 shoots-0.1.0/shoots.egg-info/PKG-INFO
--rw-r--r--   0 rickspencer   (501) staff       (20)      479 2024-02-24 14:10:55.000000 shoots-0.1.0/shoots.egg-info/SOURCES.txt
--rw-r--r--   0 rickspencer   (501) staff       (20)        1 2024-02-24 14:10:55.000000 shoots-0.1.0/shoots.egg-info/dependency_links.txt
--rw-r--r--   0 rickspencer   (501) staff       (20)       60 2024-02-24 14:10:55.000000 shoots-0.1.0/shoots.egg-info/entry_points.txt
--rw-r--r--   0 rickspencer   (501) staff       (20)       99 2024-02-24 14:10:55.000000 shoots-0.1.0/shoots.egg-info/requires.txt
--rw-r--r--   0 rickspencer   (501) staff       (20)       13 2024-02-24 14:10:55.000000 shoots-0.1.0/shoots.egg-info/top_level.txt
-drwxr-xr-x   0 rickspencer   (501) staff       (20)        0 2024-02-24 14:10:55.520360 shoots-0.1.0/tests/
--rw-r--r--   0 rickspencer   (501) staff       (20)        0 2024-02-10 22:35:05.000000 shoots-0.1.0/tests/__init__.py
--rw-r--r--   0 rickspencer   (501) staff       (20)    10588 2024-02-10 22:46:41.000000 shoots-0.1.0/tests/base_test.py
--rw-r--r--   0 rickspencer   (501) staff       (20)      587 2024-02-10 22:35:05.000000 shoots-0.1.0/tests/insecure_test.py
--rw-r--r--   0 rickspencer   (501) staff       (20)     2671 2024-02-10 22:51:40.000000 shoots-0.1.0/tests/jwt_test.py
--rw-r--r--   0 rickspencer   (501) staff       (20)     2566 2024-02-11 21:11:35.000000 shoots-0.1.0/tests/large_datasets_test.py
--rw-r--r--   0 rickspencer   (501) staff       (20)      511 2024-02-10 22:35:05.000000 shoots-0.1.0/tests/run_tests.py
--rw-r--r--   0 rickspencer   (501) staff       (20)     5534 2024-02-10 22:35:05.000000 shoots-0.1.0/tests/tls_test.py
+drwxr-xr-x   0 rickspencer   (501) staff       (20)        0 2024-04-27 12:19:33.162746 shoots-0.1.1/
+-rw-r--r--   0 rickspencer   (501) staff       (20)     1059 2024-02-24 14:43:43.000000 shoots-0.1.1/LICENSE
+-rw-r--r--   0 rickspencer   (501) staff       (20)    11575 2024-04-27 12:19:33.162475 shoots-0.1.1/PKG-INFO
+-rw-r--r--   0 rickspencer   (501) staff       (20)    10860 2024-03-30 13:47:01.000000 shoots-0.1.1/README.md
+-rw-r--r--   0 rickspencer   (501) staff       (20)       38 2024-04-27 12:19:33.162809 shoots-0.1.1/setup.cfg
+-rw-r--r--   0 rickspencer   (501) staff       (20)     1016 2024-04-27 12:19:18.000000 shoots-0.1.1/setup.py
+drwxr-xr-x   0 rickspencer   (501) staff       (20)        0 2024-04-27 12:19:33.160152 shoots-0.1.1/shoots/
+-rw-r--r--   0 rickspencer   (501) staff       (20)      319 2024-04-21 21:59:53.000000 shoots-0.1.1/shoots/__init__.py
+-rw-r--r--   0 rickspencer   (501) staff       (20)      294 2024-02-10 22:35:05.000000 shoots-0.1.1/shoots/jwt_client_auth_handler.py
+-rw-r--r--   0 rickspencer   (501) staff       (20)     3038 2024-02-10 22:35:05.000000 shoots-0.1.1/shoots/jwt_server_auth.py
+-rw-r--r--   0 rickspencer   (501) staff       (20)    26108 2024-04-21 21:59:53.000000 shoots-0.1.1/shoots/shoots_client.py
+-rw-r--r--   0 rickspencer   (501) staff       (20)    25957 2024-04-21 21:59:53.000000 shoots-0.1.1/shoots/shoots_server.py
+drwxr-xr-x   0 rickspencer   (501) staff       (20)        0 2024-04-27 12:19:33.162008 shoots-0.1.1/shoots.egg-info/
+-rw-r--r--   0 rickspencer   (501) staff       (20)    11575 2024-04-27 12:19:33.000000 shoots-0.1.1/shoots.egg-info/PKG-INFO
+-rw-r--r--   0 rickspencer   (501) staff       (20)      479 2024-04-27 12:19:33.000000 shoots-0.1.1/shoots.egg-info/SOURCES.txt
+-rw-r--r--   0 rickspencer   (501) staff       (20)        1 2024-04-27 12:19:33.000000 shoots-0.1.1/shoots.egg-info/dependency_links.txt
+-rw-r--r--   0 rickspencer   (501) staff       (20)       60 2024-04-27 12:19:33.000000 shoots-0.1.1/shoots.egg-info/entry_points.txt
+-rw-r--r--   0 rickspencer   (501) staff       (20)       99 2024-04-27 12:19:33.000000 shoots-0.1.1/shoots.egg-info/requires.txt
+-rw-r--r--   0 rickspencer   (501) staff       (20)       13 2024-04-27 12:19:33.000000 shoots-0.1.1/shoots.egg-info/top_level.txt
+drwxr-xr-x   0 rickspencer   (501) staff       (20)        0 2024-04-27 12:19:33.161807 shoots-0.1.1/tests/
+-rw-r--r--   0 rickspencer   (501) staff       (20)        0 2024-02-10 22:35:05.000000 shoots-0.1.1/tests/__init__.py
+-rw-r--r--   0 rickspencer   (501) staff       (20)    13314 2024-04-21 21:59:53.000000 shoots-0.1.1/tests/base_test.py
+-rw-r--r--   0 rickspencer   (501) staff       (20)      587 2024-02-10 22:35:05.000000 shoots-0.1.1/tests/insecure_test.py
+-rw-r--r--   0 rickspencer   (501) staff       (20)     2671 2024-02-10 22:51:40.000000 shoots-0.1.1/tests/jwt_test.py
+-rw-r--r--   0 rickspencer   (501) staff       (20)     2566 2024-02-11 21:11:35.000000 shoots-0.1.1/tests/large_datasets_test.py
+-rw-r--r--   0 rickspencer   (501) staff       (20)      511 2024-02-10 22:35:05.000000 shoots-0.1.1/tests/run_tests.py
+-rw-r--r--   0 rickspencer   (501) staff       (20)     5534 2024-02-10 22:35:05.000000 shoots-0.1.1/tests/tls_test.py
```

### Comparing `shoots-0.1.0/LICENSE` & `shoots-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shoots-0.1.0/PKG-INFO` & `shoots-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shoots
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Pandas dataframe data lake
 Home-page: https://github.com/rickspencer3/shoots
 Author: Rick Spencer
 Author-email: richard.linger.spencer.3@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,14 +34,32 @@
 
 Under the hood, the server receives and serves pandas dataframes, storing thenm on disk in [Apache Parquet](https://parquet.apache.org/) format. However, shoots is designed so that, as a user, you don't need to know about the underlying storage formats and libraries.
 
 # shoots_client
 The client pieces wrap the [Apache FlightClient](https://arrow.apache.org/docs/python/generated/pyarrow.flight.FlightClient.html) to offer an interface for pandas developers, abstracting away the Apache Arrow and Flight concepts.
 
 # usage
+## installation
+There is a [pypi package](https://pypi.org/project/shoots/) so you can install using pip(3):
+
+```bash
+pip install shoots
+```
+or
+
+```bash
+pip3 install shoots
+```
+
+This will allow you to run the Shoots server directly from the cli along with any command line arguments as documented below:
+
+```bash
+shoots-server
+```
+
 ## starting up the server
 ### terminal
 Running the server is a simple matter of running the python module, depending on your system:
 
 ```bash
 python shoots_server.py
 ```
@@ -287,15 +305,15 @@
 To run the tests, navigate to the project directory, add the project directory to your python path, and run the tests (from the project directory):
 
 ```bash
 $ export PYTHONPATH="/path/to/shoots:$PYTHONPATH"
 $ python3 tests/run_tests.py   
 ```
 
-This will run all 3 test casees in parallel.
+This will run all 3 test cases in parallel.
 
 To run a single test, you can drop into the tests directory and run the test directly:
 
 ```bash
 $ cd tests                                                 
 tests $ python3 -m unittest tls_test.TLSTest 
 ```
@@ -309,14 +327,14 @@
 # License
 This edition of the code is licensed under the MIT license.
 
 # Roadmap
 I intend to work on the following in the coming weeks, in no particular order:
 
 - [X] add a runtime option for the root bucket directory, use it for testing
-- [ ] pip packaging
+- [X] pip packaging
 - [ ] pattern matching for ```list()```
 - [X] downsampling via sql on the server
 - [ ] combining dataframes on the server
 - [X] compressing and cleaning dataframes on the server
 - [X] authentication
 - [ ] UI with SQL tree view browser and editor
```

### Comparing `shoots-0.1.0/README.md` & `shoots-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,32 @@
 
 Under the hood, the server receives and serves pandas dataframes, storing thenm on disk in [Apache Parquet](https://parquet.apache.org/) format. However, shoots is designed so that, as a user, you don't need to know about the underlying storage formats and libraries.
 
 # shoots_client
 The client pieces wrap the [Apache FlightClient](https://arrow.apache.org/docs/python/generated/pyarrow.flight.FlightClient.html) to offer an interface for pandas developers, abstracting away the Apache Arrow and Flight concepts.
 
 # usage
+## installation
+There is a [pypi package](https://pypi.org/project/shoots/) so you can install using pip(3):
+
+```bash
+pip install shoots
+```
+or
+
+```bash
+pip3 install shoots
+```
+
+This will allow you to run the Shoots server directly from the cli along with any command line arguments as documented below:
+
+```bash
+shoots-server
+```
+
 ## starting up the server
 ### terminal
 Running the server is a simple matter of running the python module, depending on your system:
 
 ```bash
 python shoots_server.py
 ```
@@ -264,15 +282,15 @@
 To run the tests, navigate to the project directory, add the project directory to your python path, and run the tests (from the project directory):
 
 ```bash
 $ export PYTHONPATH="/path/to/shoots:$PYTHONPATH"
 $ python3 tests/run_tests.py   
 ```
 
-This will run all 3 test casees in parallel.
+This will run all 3 test cases in parallel.
 
 To run a single test, you can drop into the tests directory and run the test directly:
 
 ```bash
 $ cd tests                                                 
 tests $ python3 -m unittest tls_test.TLSTest 
 ```
@@ -286,14 +304,14 @@
 # License
 This edition of the code is licensed under the MIT license.
 
 # Roadmap
 I intend to work on the following in the coming weeks, in no particular order:
 
 - [X] add a runtime option for the root bucket directory, use it for testing
-- [ ] pip packaging
+- [X] pip packaging
 - [ ] pattern matching for ```list()```
 - [X] downsampling via sql on the server
 - [ ] combining dataframes on the server
 - [X] compressing and cleaning dataframes on the server
 - [X] authentication
 - [ ] UI with SQL tree view browser and editor
```

### Comparing `shoots-0.1.0/setup.py` & `shoots-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def read_requirements(filename):
     with open(filename, 'r') as f:
         return [line.strip() for line in f.readlines() if line.strip()]
     
 setup(
     name='shoots',
-    version='0.1.0',
+    version='0.1.1',
     author='Rick Spencer',
     author_email='richard.linger.spencer.3@gmail.com',
     description='A Pandas dataframe data lake',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/rickspencer3/shoots',
     packages=find_packages(),
```

### Comparing `shoots-0.1.0/shoots/jwt_server_auth.py` & `shoots-0.1.1/shoots/jwt_server_auth.py`

 * *Files identical despite different names*

### Comparing `shoots-0.1.0/shoots/shoots_client.py` & `shoots-0.1.1/shoots/shoots_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pydantic import BaseModel, ValidationError, validator, model_validator
 from pydantic_settings import BaseSettings
 from typing import Optional
 import pyarrow as pa
-from pyarrow.flight import FlightDescriptor, FlightClient, Ticket, Action
+from pyarrow.flight import FlightDescriptor, FlightClient, Ticket, Action, FlightServerError
 import pandas as pd
 import json
 from enum import Enum
 from .jwt_client_auth_handler import JWTClientAuthHandler
 
 class PutMode(Enum):
     """
@@ -139,14 +139,24 @@
 
     @validator('name')
     def validate_name(cls, v):
         if not v or not isinstance(v, str):
             raise ValueError('name must be a non-empty string')
         return v
 
+class DataFusionError(Exception):
+    """Custom exception for DataFusion-related errors."""
+    def __init__(self, message):
+        super().__init__(message)
+
+class BucketNotEmptyError(Exception):
+    """Custom exception for delete_bucket."""
+    def __init__(self, message):
+        super().__init__(message)
+
 class ShootsClient:
     """
     Client class for interacting with a ShootsServer instance.
     """
     def __init__(self, 
                  host: str, 
                  port: int, 
@@ -165,14 +175,15 @@
 
         Args:
             host (str): The hostname or IP address of the FlightServer.
             port (int): The port number on which the FlightServer is listening.
             tls (bool): Whether or not the server to connect to uses TLS.
             root_cert (string): A root certificate used by the server for tls signing if the server is using self-signed tls.
             token (string): A JWT to provide to the server. Requires TLS to be True.
+
         Raises:
             ValidationError: Occurs:
                  - If the provided host or port values are not valid
                  - A token is provided but tls is False
         
         Example:
             To create a client instance that connects to a FlightServer running
@@ -242,16 +253,16 @@
             bucket (Optional[str]): The name of the bucket where the dataframe will be stored. 
                                     If None, a default bucket may be used.
             batch_size(Optional[int]): The number of rows to write per batch. May be useful for optimizing write performance or memory on the server or client. Default is 5,000 rows.
 
         Raises:
             ValidationError: If the provided arguments are not valid or if there is a 
                             problem with the DataFrame format.
-            FlightServerError: If the dataframe already exists and the put mode was set to ERROR.
-            FlightServerError: Other problems encountered on the server while trying to write.
+            FileExistsError: If the dataframe already exists and the put mode was set to ERROR.
+            FlightServerError: Unhandled errors encountered on the server while trying to write.
 
         Example:
             To send a DataFrame 'df' to the server and store it as 'my_dataframe' in the 
             'my_bucket' bucket, use the following:
 
             ```python
             client = ShootsClient("localhost", 8080)
@@ -271,27 +282,29 @@
                              batch_size=batch_size)
 
             command_info = json.dumps({"name": req.name,
                                  "mode": req.mode.value,
                                  "bucket":req.bucket,
                                  "batch_size":req.batch_size}).encode()
             
-            
             descriptor = FlightDescriptor.for_command(command_info)
             table = pa.Table.from_pandas(req.dataframe)
 
-            writer, _ = self.client.do_put(descriptor, table.schema)
-            
-            row_count = table.num_rows
-            with writer:
-                for start_idx in range(0, row_count, batch_size):
-                    end_idx = min(start_idx + batch_size, row_count)
-                    chunk = table.slice(start_idx, end_idx - start_idx)
-                    writer.write_table(chunk)
-
+            try:
+                writer, _ = self.client.do_put(descriptor, table.schema)
+                
+                row_count = table.num_rows
+                with writer:
+                    for start_idx in range(0, row_count, batch_size):
+                        end_idx = min(start_idx + batch_size, row_count)
+                        chunk = table.slice(start_idx, end_idx - start_idx)
+                        writer.write_table(chunk)
+            except FlightServerError as e:
+                raise self._translate_flight_error(e)
+                
         except ValidationError as e:
             print(f"Validation error: {e}")
 
     def get(self, name: str, sql: Optional[str] = None, bucket: Optional[str] = None):
         """
         Retrieves a dataframe from the server based on the specified dataframe name, optional SQL query, and bucket.
 
@@ -308,15 +321,17 @@
 
         Returns:
             pd.DataFrame: A DataFrame containing the retrieved data.
 
         Raises:
             ValidationError: If the provided arguments are not valid or if the request 
                             cannot be processed by the server.
-            FlightServerError: An error is encountered on the server, such as the specified dataframe cannot be found.
+            DataFusionError: The supplied SQL could not be processed by the server.
+            FileNotFoundError: The specified dataframe cannot be found.
+            FlightServerError: Unhandled errors arising from the server.
 
         Example:
             To retrieve a dataframe named 'my_dataframe' from the server, and filter it using an 
             SQL query, use the following:
 
             ```python
             client = ShootsClient("localhost", 8080)
@@ -327,29 +342,36 @@
             req = GetRequest(name=name, sql=sql, bucket=bucket)
             ticket_info = {"name":req.name, "bucket":req.bucket}
             if sql is not None:
                 ticket_info["sql"] = req.sql
 
             ticket_bytes = json.dumps(ticket_info)
             ticket = Ticket(ticket_bytes)
-            reader = self.client.do_get(ticket)
-            return reader.read_all().to_pandas()
-        
+            try:
+                reader = self.client.do_get(ticket)
+                df = reader.read_all().to_pandas()
+                return df
+            except FlightServerError as e:
+                raise self._translate_flight_error(e)
+ 
         except ValidationError as e:
             print(f"Validation error: {e}")
 
     def buckets(self):
         """
         Retrieves a list of all available buckets from the server.
 
         Buckets are logical groupings or directories in which
         dataframes are stored on the server. The method returns a list of bucket names.
 
         Returns:
             list: A list of strings, each representing a bucket name.
+        
+        Raises:
+            FlightServerError: Unhandled errors arising from the server.
 
         Example:
             To get a list of all buckets from the server, use the following:
 
             ```python
             client = ShootsClient("localhost", 8080)
             bucket_list = client.buckets()
@@ -375,32 +397,36 @@
                                     error if the bucket is not empty. DELETE_CONTENTS mode 
                                     deletes the bucket and its contents.
 
         Returns:
             str: A message indicating the result of the deletion operation.
 
         Raises:
-            FlightServerError: If the server encounters an error processing the deletion request.
-
+            BucketNotEmptyError: The specified bucket is not empty, and the BucketDeleteMode is set to ERROR.
+            FileNotFoundError: The specified bucket cannot be found.    
+        
         Example:
             To delete a bucket named 'my_bucket' and its contents, use the following:
 
             ```python
             client = ShootsClient("localhost", 8080)
             result_message = client.delete_bucket(name="my_bucket", mode=BucketDeleteMode.DELETE_CONTENTS)
             print(result_message)
             ```
         """
         req = DeleteBucketRequest(name=name, mode=mode)
         action_info = {"name":req.name, "mode":req.mode.value}
         aciton_bytes = json.dumps(action_info).encode()
         action = Action("delete_bucket",aciton_bytes)
-        result = self.client.do_action(action)
-        return self._flight_result_to_string(result)       
-
+        try:
+            result = self.client.do_action(action)
+            return self._flight_result_to_string(result)       
+        except FlightServerError as e:
+            raise self._translate_flight_error(e)
+        
     def list(self, bucket: Optional[str] = None, regex: Optional[str] = None):
         """
         Lists dataframes available on the server, optionally filtered by a specific bucket.
 
         Each dataframe is returned with its name and schema.
 
         Args:
@@ -415,27 +441,33 @@
 
             ```python
             client = ShootsClient("localhost", 8080)
             dataframes = client.list(bucket="my_bucket")
             for dataframe in dataframes:
                 print(dataframe["name"], dataframe["schema"])
             ```
-
+        Raises:
+            FileNotFounderror: The specified bucket does not exist on the server.
+            FlightServerError: Unhandled errors arising from the server.
         Note:
             The method returns an empty list if no dataframes match the filtering criteria or if 
             the server does not have any dataframes. The 'schema' in the returned dictionary is 
             an Apache Arrow schema object.
         """
         descriptor_info = {"bucket":bucket, "regex":regex}
         descriptor_bytes = json.dumps(descriptor_info).encode()
-        flights = self.client.list_flights(criteria=descriptor_bytes)
-        dataframes = []
-        for flight in flights:
-            dataframes.append({"name":flight.descriptor.path[0].decode(), "schema":flight.schema})
-        return dataframes
+        try:
+            flights = self.client.list_flights(criteria=descriptor_bytes)
+
+            dataframes = []
+            for flight in flights:
+                dataframes.append({"name":flight.descriptor.path[0].decode(), "schema":flight.schema})
+            return dataframes
+        except FlightServerError as e:
+            raise self._translate_flight_error(e)
 
     def shutdown(self):
         """
         Sends a shutdown request to the server.
 
         This method is used to send a command to the FlightServer to initiate its shutdown
         procedure. It is useful for programmatically stopping the server from the client side.
@@ -471,15 +503,16 @@
             bucket (Optional[str]): The name of the bucket containing the dataframe. If None, 
                                     the default bucket or a server-defined location is used.
 
         Returns:
             str: A message indicating the result of the delete operation.
 
         Raises:
-            FlightServerError: If the server encounters an error processing the delete request.
+            FileNotFoundError: The specified dataframe does not exist.
+            FlightServerError: Unhandled errors arising from the server.
 
         Example:
             To delete a dataframe named 'my_dataframe' from the server, use the following:
 
             ```python
             client = ShootsClient("localhost", 8081)
             delete_result = client.delete(name="my_dataframe", bucket="my_bucket")
@@ -488,17 +521,19 @@
 
         Note:
             Be cautious when using this method as deleting a dataframe is irreversible. Ensure 
             that the dataframe is correctly specified.
         """
         action_bytes = json.dumps({"name":name, "bucket":bucket}).encode()
         action = Action("delete",action_bytes)
-        result = self.client.do_action(action)
-
-        return self._flight_result_to_string(result)
+        try:
+            result = self.client.do_action(action)
+            return self._flight_result_to_string(result)
+        except FlightServerError as e:
+            raise self._translate_flight_error(e)
     
     def resample(self, 
                 source: str, 
                 target: str, 
                 rule: Optional[str] = None, 
                 time_col: Optional[str] = None,
                 aggregation_func: Optional[str] = None,
@@ -522,17 +557,18 @@
             target_bucket (Optional[str]): Bucket for where to store the resampled dataframe, if any
 
             The following arguments are ignoed if the sql argument is provide, and required if not.
             rule (str): String representation of time delta for windowing (example: 1s)
             time_col (str): The name of the time stamp column to window on
             aggregation_func (str): The name of the function to aggregate (examples: mean, max, count)
 
-
         Raises:
-            FlightServerError
+            FlightServerError: Unhandled errors arising from the server.
+            FileNotFoundError: Either the source dataframe or the target bucket do not exist.
+            DataFusionError: The supplied SQL could not be processed.
         
         Example:
             Resampling with a SQL query:
             ```python
             self.client.resample(source="my_source_dataframe", 
                                 target="my_resampled_dataframe",
                                 sql="SELECT * FROM my_source_dataframe LIMIT 10",
@@ -544,15 +580,14 @@
             self.client.resample(source="my_source_dataframe", 
                                 target="my_resampled_dataframe",
                                 rule="10s",
                                 time_col="timestamp",
                                 aggregation_func="mean",
                                 mode=PutMode.APPEND)
             ```
-
         """
 
         req = ResampleRequest(
                 source=source,
                 target=target,
                 sql=sql,
                 rule=rule,
@@ -573,17 +608,19 @@
         else:
             resample_info["rule"] = req.rule
             resample_info["time_col"] = req.time_col
             resample_info["aggregation_func"] = req.aggregation_func
         
         action_bytes = json.dumps(resample_info).encode()
         action = Action("resample",action_bytes)
-        result = self.client.do_action(action)
-        return json.loads(self._flight_result_to_string(result))
-      
+        try:
+            result = self.client.do_action(action)
+            return json.loads(self._flight_result_to_string(result))
+        except FlightServerError as e:
+            raise self._translate_flight_error(e)
     def ping(self):
         """
         Sends a 'ping' to th server.
 
         Useful for testing if the server is alive and the connection is working.
 
         Returns:
@@ -602,8 +639,25 @@
 
     def _flight_result_to_string(self, result):
         msg = ""
         for r in result:
             msg += r.body.to_pybytes().decode() + "\n"
         
         msg = msg.rstrip("\n")
-        return msg
+        return msg
+    
+
+    def _translate_flight_error(self, e):
+        try:
+            exception_info = json.loads(e.extra_info)
+            exception_type = exception_info.get("type")
+            message = exception_info.get("message", "")
+
+            exception_map = {
+                "FileExistsError": FileExistsError,
+                "DataFusionError": DataFusionError,
+                "FileNotFoundError": FileNotFoundError,
+                "BucketNotEmptyError":BucketNotEmptyError
+            }
+            return exception_map[exception_type](message)
+        except:
+            return e
```

### Comparing `shoots-0.1.0/shoots/shoots_server.py` & `shoots-0.1.1/shoots/shoots_server.py`

 * *Files 9% similar despite different names*

```diff
@@ -130,36 +130,47 @@
         """
         try:
             
             ticket_info = json.loads(ticket.ticket.decode())
             name = ticket_info["name"]
             bucket = ticket_info["bucket"]
             file_path = self._create_file_path(name, bucket)
+            if not os.path.exists(file_path):
+                exception = {"type":"FileNotFoundError",
+                             "message": f"dataframe {name} in bucket {bucket} not found"}
+                raise flight.FlightServerError(extra_info=json.dumps(exception))
+            
             if "sql" in ticket_info:
                 sql_query = ticket_info["sql"]
                 table = self._get_arrow_table_from_sql(name, file_path, sql_query)
-                
                 return flight.RecordBatchStream(table)
             
             else:
                 table = pq.read_table(file_path)
                 return flight.RecordBatchStream(table)
-            
+
+        except flight.FlightServerError as e:
+            raise e
+
         except Exception as e:
             raise flight.FlightServerError(extra_info=str(e))
 
     def _get_arrow_table_from_sql(self, name, file_path, sql_query):
         try:
             ctx = SessionContext()
             ctx.register_parquet(name, file_path)
             result = ctx.sql(sql_query)
             table = result.to_arrow_table()
             return table
         except Exception as e:
-            print(e)
+            if "DataFusion error" in str(e):
+                exception = {"type":"DataFusionError", "message":str(e)}
+                raise flight.FlightServerError(extra_info = json.dumps(exception))
+            else:
+                raise e
         
     def do_put(self, context, descriptor, reader, writer):
         """
         Handles uploading or appending data to a dataframe.
         
         You can optionally specify a mode to determine the behavior in case there is already a dataframe with the same name stored:
          - error - (default) The put operation will return a FlightServerError, and no changes will take place
@@ -216,15 +227,17 @@
         if os.path.exists(file_path):
             if mode == "append":
                 existing_table = pq.read_table(file_path)
                 data_table = pa.concat_tables([data_table, existing_table])
                 pq.write_table(data_table, file_path)
             
             elif(mode == "error"):
-                raise flight.FlightServerError(f"File {name} Exists", extra_info="File Exists")
+                exception = {"type":"FileExistsError",
+                             "message":f"Dataframe {name} Exists"}
+                raise flight.FlightServerError(f"File {name} Exists", extra_info=json.dumps(exception))
             else:
                 pq.write_table(data_table, file_path)
         else:
             pq.write_table(data_table, file_path)
 
     def list_flights(self, context, criteria):
         """
@@ -252,28 +265,46 @@
                     print(flight.descriptor.path[0].decode(), flight.schema)                
             ```
 
         Note:
             The regex criteria is not yet implemented on the server.
         """
 
+        
+
         criteria_info = json.loads(criteria.decode())
         bucket = criteria_info["bucket"]
         regex = criteria_info["regex"]
+
+        # gaurd against the bucket not existing
+        if bucket:
+            bucket_dir = os.path.join(self.bucket_dir, bucket)
+            if not os.path.exists(bucket_dir):
+                exception = {"type":"FileNotFoundError",
+                             "message":f"No such bucket {bucket}"}
+                raise flight.FlightServerError(extra_info=json.dumps(exception))
+            
+        # call helper function to get a list of files, bucket may be NONE
         files = self._list_parquet_files(bucket)
+
+        # open each parquet to grab the schema
         for file in files:
+            # set the file_path for each parquet file, in a bucket or not
             file_path = os.path.join(self.bucket_dir, file)
             if bucket:
                 file_path = os.path.join(self.bucket_dir, bucket, file)
+
+            # read in the schame and yield a FlightDestriptor for each parquet file
             parquet_file = pq.ParquetFile(file_path)
             schema = parquet_file.schema.to_arrow_schema()
             descriptor = flight.FlightDescriptor.for_path(file[:-8])
+
             yield flight.FlightInfo(schema,
                             descriptor,
-                            [],  # No endpoints, replace with actual data locations if applicable
+                            [],
                             parquet_file.metadata.num_rows,
                             parquet_file.metadata.serialized_size)
 
     def do_action(self, context, action):
         """
         Performs a specific action based on the request.
 
@@ -366,28 +397,32 @@
             if action_info.get("sql",False):
                 return self._resample_with_sql(action_info)
             else:
                 return self._resample_time_series(action_info)
         if action == "ping":
             result = flight.Result(b'pong')
             return [result]
-    
+
     def _resample_with_sql(self, resample_info):
         source = resample_info["source"]
         target = resample_info["target"]
         source_bucket = resample_info["source_bucket"]
         target_bucket = resample_info["target_bucket"]
         sql = resample_info["sql"]
         mode = resample_info["mode"]
 
         self._raise_if_invalid_put_mode(mode)
 
         target_rows = -1
 
         file_path = self._create_file_path(source, source_bucket)
+        if not os.path.exists(file_path):
+            exception = {"type":"FileNotFoundError",
+                "message":f"Dataframe {source} not found"}
+            raise flight.FlightServerError(extra_info=json.dumps(exception))
         table = self._get_arrow_table_from_sql(source, file_path, sql)
         target_rows = table.num_rows
         self._write_arrow_table(target, mode, target_bucket, table)
         return self._flight_result_from_dict({"target_rows":target_rows})
     
     def _resample_time_series(self, resample_info):
         source = resample_info["source"]
@@ -427,15 +462,18 @@
                 self._write_arrow_table(target, mode ,target_bucket, table)
 
         return self._flight_result_from_dict({"source_rows":source_rows,
                                               "target_rows":target_rows})
 
     def _load_dataframe_from_file(self, source, source_bucket):
         file_name = self._create_file_path(source, source_bucket)
-        
+        if not os.path.exists(file_name):
+            exception = {"type":"FileNotFoundError",
+                "message":f"Dataframe {source} not found"}
+            raise flight.FlightServerError(extra_info=json.dumps(exception))
         table = pq.read_table(file_name)
         df_source = table.to_pandas()
         return df_source
 
     def list_actions(self, context):
         """
         Lists all available actions that the server can perform.
@@ -467,28 +505,30 @@
         os.makedirs(bucket_path, exist_ok=True)
 
         file_name = f"{name}.parquet"
 
         file_path = os.path.join(bucket_path, file_name)
         
         return file_path
-        
+
     def _delete_bucket(self, delete_info):
         bucket = delete_info["name"]
         mode = delete_info["mode"]
         bucket_path = os.path.join(self.bucket_dir, bucket)
         if not os.path.isdir(bucket_path):
-            raise flight.FlightServerError(f"No such bucket: {bucket}",
-                                            extra_info="No Such Bucket")
+            exception = {"type":"FileNotFoundError",
+                "message":f"Bucket {bucket} not found"}
+            raise flight.FlightServerError(extra_info=json.dumps(exception))
         
         bucket_is_empty = not os.listdir(bucket_path)
         if not bucket_is_empty:
             if mode == "error":
-                raise flight.FlightServerError(f"Bucket Not Empty: {bucket}",
-                                                extra_info="Bucket Not Empty")
+                exception = {"type":"BucketNotEmptyError",
+                             "message":f"Bucket Not Empty: {bucket}"}
+                raise flight.FlightServerError(extra_info=json.dumps(exception))
             elif mode == "delete":
                 shutil.rmtree(bucket_path)
         else: 
             os.rmdir(bucket_path) 
         result_info = {"message":f"bucket {bucket} deleted"}
         return self._flight_result_from_dict(result_info)
 
@@ -518,16 +558,18 @@
         name = delete_info["name"]
         bucket = delete_info["bucket"]
         file_path = self._create_file_path(name, bucket)
 
         try:
             os.remove(file_path)
         except FileNotFoundError:
-            raise flight.FlightServerError(f"Dataframe {name} not found",
-                                extra_info="No Such Dataset")
+            exception = {"type":"FileNotFoundError",
+                         "message":f"Dataframe {name} not found"}
+            raise flight.FlightServerError(extra_info=json.dumps(exception))
+        
         except PermissionError:
             raise flight.FlightUnauthorizedError(f"Insufficent permisions to delete {name}")
         except OSError as e:
             raise flight.FlightServerError(f"Error encountered deleting {name}",
                                            extra_info=str(e))
         
         result_info = {"success":True, "message":f"deleted {name}"}
```

### Comparing `shoots-0.1.0/shoots.egg-info/PKG-INFO` & `shoots-0.1.1/shoots.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shoots
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Pandas dataframe data lake
 Home-page: https://github.com/rickspencer3/shoots
 Author: Rick Spencer
 Author-email: richard.linger.spencer.3@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,14 +34,32 @@
 
 Under the hood, the server receives and serves pandas dataframes, storing thenm on disk in [Apache Parquet](https://parquet.apache.org/) format. However, shoots is designed so that, as a user, you don't need to know about the underlying storage formats and libraries.
 
 # shoots_client
 The client pieces wrap the [Apache FlightClient](https://arrow.apache.org/docs/python/generated/pyarrow.flight.FlightClient.html) to offer an interface for pandas developers, abstracting away the Apache Arrow and Flight concepts.
 
 # usage
+## installation
+There is a [pypi package](https://pypi.org/project/shoots/) so you can install using pip(3):
+
+```bash
+pip install shoots
+```
+or
+
+```bash
+pip3 install shoots
+```
+
+This will allow you to run the Shoots server directly from the cli along with any command line arguments as documented below:
+
+```bash
+shoots-server
+```
+
 ## starting up the server
 ### terminal
 Running the server is a simple matter of running the python module, depending on your system:
 
 ```bash
 python shoots_server.py
 ```
@@ -287,15 +305,15 @@
 To run the tests, navigate to the project directory, add the project directory to your python path, and run the tests (from the project directory):
 
 ```bash
 $ export PYTHONPATH="/path/to/shoots:$PYTHONPATH"
 $ python3 tests/run_tests.py   
 ```
 
-This will run all 3 test casees in parallel.
+This will run all 3 test cases in parallel.
 
 To run a single test, you can drop into the tests directory and run the test directly:
 
 ```bash
 $ cd tests                                                 
 tests $ python3 -m unittest tls_test.TLSTest 
 ```
@@ -309,14 +327,14 @@
 # License
 This edition of the code is licensed under the MIT license.
 
 # Roadmap
 I intend to work on the following in the coming weeks, in no particular order:
 
 - [X] add a runtime option for the root bucket directory, use it for testing
-- [ ] pip packaging
+- [X] pip packaging
 - [ ] pattern matching for ```list()```
 - [X] downsampling via sql on the server
 - [ ] combining dataframes on the server
 - [X] compressing and cleaning dataframes on the server
 - [X] authentication
 - [ ] UI with SQL tree view browser and editor
```

### Comparing `shoots-0.1.0/tests/base_test.py` & `shoots-0.1.1/tests/base_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from shoots import PutMode, BucketDeleteMode
+from shoots import PutMode, BucketDeleteMode, DataFusionError, BucketNotEmptyError
 import pandas as pd
 import numpy as np
 from pyarrow.flight import FlightServerError
 import threading
 import shutil
 import random
 import string
@@ -53,20 +53,20 @@
         res = self.shoots_client.get("test1")
         self.assertEqual(res.shape[0],1)
         self.assertEqual(res.iloc(0)[0].col1, 1)
         
         self.shoots_client.delete("test1")
 
     def test_delete_file_not_found(self):
-        with self.assertRaises(FlightServerError):
+        with self.assertRaises(FileNotFoundError):
             self.shoots_client.delete("abcdefghijklmnopqrstuvwxyz")
         
     def test_write_error(self):
         self.shoots_client.put("test1",self.dataframe1,mode=PutMode.ERROR)
-        with self.assertRaises(FlightServerError):
+        with self.assertRaises(FileExistsError):
             self.shoots_client.put("test1",self.dataframe1,mode=PutMode.ERROR)
         self.shoots_client.delete("test1")
 
     def test_write_append(self):
         self.shoots_client.put("test1",self.dataframe0,mode=PutMode.ERROR)
         self.shoots_client.put("test1",self.dataframe1,mode=PutMode.APPEND)
         res = self.shoots_client.get("test1")
@@ -92,27 +92,55 @@
     
     def test_read_write_to_bucket(self):
         bucket = "test_bucket"
         self.shoots_client.put("test1",self.dataframe0,mode=PutMode.REPLACE,bucket=bucket)
         res = self.shoots_client.get("test1",bucket=bucket)
         self.assertEqual(res.shape[0],1)
         self.shoots_client.delete("test1", bucket=bucket)
+    
+    def test_get_no_such_df(self):
+        with self.assertRaises(FileNotFoundError):
+            self.shoots_client.get("asdfasdfasdf")
 
-    def test_list_and_delete_bucket(self):
+    def test_list_and_delete_bucket_with_flags(self):
+        # set up the bucket, add data, and make sure it is created
         bucket = "testing_bucket"
         self.shoots_client.put("test1",self.dataframe0,mode=PutMode.REPLACE,bucket=bucket)
         buckets = self.shoots_client.buckets()
         self.assertIn(bucket, buckets)
-        with self.assertRaises(FlightServerError):
-            self.shoots_client.delete_bucket("test1", mode=BucketDeleteMode.ERROR)
 
+        # make sure you can't delete the bucket if delete mode is ERROR
+        with self.assertRaises(BucketNotEmptyError):
+            self.shoots_client.delete_bucket(bucket, mode=BucketDeleteMode.ERROR)
+        buckets = self.shoots_client.buckets()
+        self.assertIn(bucket, buckets)
+
+        # make sure you can delete the bucker if delete mode is DELETE_CONTENTS        
         self.shoots_client.delete_bucket(bucket, mode=BucketDeleteMode.DELETE_CONTENTS)
         buckets = self.shoots_client.buckets()
         self.assertNotIn(bucket, buckets)
 
+    def test_no_such_bucket(self):
+        with self.assertRaises(FileNotFoundError):
+            self.shoots_client.delete_bucket("asfdasfasdfasdfasdf")
+
+    def test_delete_bucket(self):
+        # set up the bucket, add data, and make sure it is created
+        bucket = "testing_bucket"
+        df_name = "test2"
+        self.shoots_client.put(df_name,self.dataframe0,mode=PutMode.REPLACE,bucket=bucket)
+        buckets = self.shoots_client.buckets()
+        self.assertIn(bucket, buckets)
+
+        # make sure you can delete an empty bucket
+        self.shoots_client.delete(df_name,bucket=bucket)
+        self.shoots_client.delete_bucket(bucket, mode=BucketDeleteMode.ERROR)
+        buckets = self.shoots_client.buckets()
+        self.assertNotIn(bucket, buckets)
+
     def test_list(self):
         self.shoots_client.put("test1",self.dataframe0,mode=PutMode.REPLACE)
         self.shoots_client.put("test2",self.dataframe0,mode=PutMode.REPLACE)
         
         files_count = len(self.shoots_client.list())
         
         try:
@@ -136,14 +164,25 @@
         self.assertEqual(res["target_rows"], 10)
 
         df = self.shoots_client.get("ten")
         self.assertEqual(df.shape[0], 10)
         self.shoots_client.delete(source)
         self.shoots_client.delete("ten")
 
+    def test_resample_with_bad_sql(self):
+        df_name = "100x"
+        self.shoots_client.put(df_name,self.dataframe0,mode=PutMode.REPLACE)
+        with self.assertRaises(DataFusionError):
+            sql = "select * from 100x"
+            self.shoots_client.resample(source=df_name,
+                                        target="target",
+                                        sql=sql)
+
+        self.shoots_client.delete(df_name)
+
     def test_resample_no_buckets(self):
         num_rows = 1000000
         df = self._generate_dataframe_with_timestamp(num_rows)
 
         self.shoots_client.put(name="million", dataframe=df)
 
         res = self.shoots_client.resample(source="million", 
@@ -219,14 +258,28 @@
 
         df_thousands = self.shoots_client.get("thousand",bucket=target_bucket)
         self.assertEqual(df_thousands.shape[0], 1000)    
 
         self.shoots_client.delete("million", bucket=source_bucket)
         self.shoots_client.delete("thousand", bucket=target_bucket)
 
+    def test_resample_no_such(self):
+        with self.assertRaises(FileNotFoundError):
+            self.shoots_client.resample(source="xxxxx", 
+                             target="yyyyy",
+                             rule="10s",
+                             time_col="timestamp",
+                             aggregation_func="mean")
+        
+        with self.assertRaises(FileNotFoundError):
+            sql = f"SELECT * FROM xxxx LIMIT 10"
+            res = self.shoots_client.resample(source="xxxx",
+                                   target="yyyy",
+                                   sql=sql)
+
     def _generate_dataframe(self, num_rows):
         integers = np.random.randint(0, 100, size=num_rows)  # Random integers between 0 and 99
         floats = np.random.random(size=num_rows)  # Random floats
         strings = [''.join(random.choices(string.ascii_lowercase, k=5)) for _ in range(num_rows)]  # Random 5-letter strings
 
         # Create the DataFrame
         return pd.DataFrame({
@@ -245,14 +298,18 @@
             'timestamp': date_range_milliseconds,
             'data': np.random.randn(num_rows)  # Example data column with random numbers
         })
         
         return df
 
     def test_list_with_bucket(self):
+        with self.assertRaises(FileNotFoundError):
+            self.shoots_client.list(bucket="thereisnobucketnamedthis")
+
+
         self.shoots_client.put("test1",
                         self.dataframe0,
                         mode=PutMode.REPLACE,
                         bucket="listybucket")
         self.shoots_client.put("test2",
                         self.dataframe0,
                         mode=PutMode.REPLACE,
@@ -269,16 +326,23 @@
             self.assertIn("test2", names)
         except:
             self.shoots_client.delete("test1",
                         bucket="listybucket")
             self.shoots_client.delete("test2",
                         bucket="listybucket")
             raise
-        
+
         self.shoots_client.delete("test1",
                         bucket="listybucket")
         self.shoots_client.delete("test2",
                         bucket="listybucket")
 
     def test_ping(self):
         result = self.shoots_client.ping()
-        self.assertCountEqual(result,"pong")
+        self.assertCountEqual(result,"pong")
+    
+    def test_bad_sql(self):
+        self.shoots_client.put("100x",self.dataframe0,mode=PutMode.REPLACE)    
+        sql = "SELECT * FROM 100x"
+        with self.assertRaises(DataFusionError):
+            self.shoots_client.get("100x", sql)
+        self.shoots_client.delete("100x")
```

### Comparing `shoots-0.1.0/tests/insecure_test.py` & `shoots-0.1.1/tests/insecure_test.py`

 * *Files identical despite different names*

### Comparing `shoots-0.1.0/tests/jwt_test.py` & `shoots-0.1.1/tests/jwt_test.py`

 * *Files identical despite different names*

### Comparing `shoots-0.1.0/tests/large_datasets_test.py` & `shoots-0.1.1/tests/large_datasets_test.py`

 * *Files identical despite different names*

### Comparing `shoots-0.1.0/tests/tls_test.py` & `shoots-0.1.1/tests/tls_test.py`

 * *Files identical despite different names*

