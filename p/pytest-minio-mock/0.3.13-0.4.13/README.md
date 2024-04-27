# Comparing `tmp/pytest_minio_mock-0.3.13.tar.gz` & `tmp/pytest_minio_mock-0.4.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_minio_mock-0.3.13.tar", last modified: Fri Apr 26 08:54:21 2024, max compression
+gzip compressed data, was "pytest_minio_mock-0.4.13.tar", last modified: Sat Apr 27 12:12:57 2024, max compression
```

## Comparing `pytest_minio_mock-0.3.13.tar` & `pytest_minio_mock-0.4.13.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 ouss       (501) staff       (20)        0 2024-04-26 08:54:21.072612 pytest_minio_mock-0.3.13/
--rw-r--r--   0 ouss       (501) staff       (20)     1086 2024-04-22 11:08:27.000000 pytest_minio_mock-0.3.13/LICENSE
--rw-r--r--   0 ouss       (501) staff       (20)        0 2023-11-28 15:52:51.000000 pytest_minio_mock-0.3.13/MANIFEST.in
--rw-r--r--   0 ouss       (501) staff       (20)     5192 2024-04-26 08:54:21.072397 pytest_minio_mock-0.3.13/PKG-INFO
--rw-r--r--   0 ouss       (501) staff       (20)     3869 2024-04-21 19:28:01.000000 pytest_minio_mock-0.3.13/README.md
-drwxr-xr-x   0 ouss       (501) staff       (20)        0 2024-04-26 08:54:21.069864 pytest_minio_mock-0.3.13/pytest_minio_mock/
--rw-r--r--   0 ouss       (501) staff       (20)     1015 2024-04-26 08:52:30.000000 pytest_minio_mock-0.3.13/pytest_minio_mock/__init__.py
--rw-r--r--   0 ouss       (501) staff       (20)    44860 2024-04-26 08:24:20.000000 pytest_minio_mock-0.3.13/pytest_minio_mock/plugin.py
-drwxr-xr-x   0 ouss       (501) staff       (20)        0 2024-04-26 08:54:21.072066 pytest_minio_mock-0.3.13/pytest_minio_mock.egg-info/
--rw-r--r--   0 ouss       (501) staff       (20)     5192 2024-04-26 08:54:21.000000 pytest_minio_mock-0.3.13/pytest_minio_mock.egg-info/PKG-INFO
--rw-r--r--   0 ouss       (501) staff       (20)      405 2024-04-26 08:54:21.000000 pytest_minio_mock-0.3.13/pytest_minio_mock.egg-info/SOURCES.txt
--rw-r--r--   0 ouss       (501) staff       (20)        1 2024-04-26 08:54:21.000000 pytest_minio_mock-0.3.13/pytest_minio_mock.egg-info/dependency_links.txt
--rw-r--r--   0 ouss       (501) staff       (20)       56 2024-04-26 08:54:21.000000 pytest_minio_mock-0.3.13/pytest_minio_mock.egg-info/entry_points.txt
--rw-r--r--   0 ouss       (501) staff       (20)       65 2024-04-26 08:54:21.000000 pytest_minio_mock-0.3.13/pytest_minio_mock.egg-info/requires.txt
--rw-r--r--   0 ouss       (501) staff       (20)       18 2024-04-26 08:54:21.000000 pytest_minio_mock-0.3.13/pytest_minio_mock.egg-info/top_level.txt
--rw-r--r--   0 ouss       (501) staff       (20)       38 2024-04-26 08:54:21.072659 pytest_minio_mock-0.3.13/setup.cfg
--rw-r--r--   0 ouss       (501) staff       (20)     1781 2024-04-26 08:34:48.000000 pytest_minio_mock-0.3.13/setup.py
-drwxr-xr-x   0 ouss       (501) staff       (20)        0 2024-04-26 08:54:21.071687 pytest_minio_mock-0.3.13/tests/
--rw-r--r--   0 ouss       (501) staff       (20)        0 2024-04-26 08:31:50.000000 pytest_minio_mock-0.3.13/tests/__init__.py
--rw-r--r--   0 ouss       (501) staff       (20)      104 2024-04-20 11:16:24.000000 pytest_minio_mock-0.3.13/tests/conftest.py
--rw-r--r--   0 ouss       (501) staff       (20)    16739 2024-04-26 08:24:20.000000 pytest_minio_mock-0.3.13/tests/test_minio_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:12:57.816839 pytest_minio_mock-0.4.13/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-27 12:12:52.000000 pytest_minio_mock-0.4.13/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 12:12:52.000000 pytest_minio_mock-0.4.13/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-27 12:12:57.816839 pytest_minio_mock-0.4.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-27 12:12:52.000000 pytest_minio_mock-0.4.13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:12:57.812839 pytest_minio_mock-0.4.13/pytest_minio_mock/
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-27 12:12:52.000000 pytest_minio_mock-0.4.13/pytest_minio_mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49156 2024-04-27 12:12:52.000000 pytest_minio_mock-0.4.13/pytest_minio_mock/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:12:57.816839 pytest_minio_mock-0.4.13/pytest_minio_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-27 12:12:57.000000 pytest_minio_mock-0.4.13/pytest_minio_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-27 12:12:57.000000 pytest_minio_mock-0.4.13/pytest_minio_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 12:12:57.000000 pytest_minio_mock-0.4.13/pytest_minio_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-27 12:12:57.000000 pytest_minio_mock-0.4.13/pytest_minio_mock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-27 12:12:57.000000 pytest_minio_mock-0.4.13/pytest_minio_mock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 12:12:57.000000 pytest_minio_mock-0.4.13/pytest_minio_mock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 12:12:57.816839 pytest_minio_mock-0.4.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-27 12:12:52.000000 pytest_minio_mock-0.4.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:12:57.816839 pytest_minio_mock-0.4.13/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    18517 2024-04-27 12:12:52.000000 pytest_minio_mock-0.4.13/tests/test_minio_mock.py
```

### Comparing `pytest_minio_mock-0.3.13/LICENSE` & `pytest_minio_mock-0.4.13/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_minio_mock-0.3.13/PKG-INFO` & `pytest_minio_mock-0.4.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-minio-mock
-Version: 0.3.13
+Version: 0.4.13
 Summary: A pytest plugin for mocking Minio S3 interactions
 Home-page: https://github.com/oussjarrousse/pytest-minio-mock
 Author: Oussama Jarrousse
 Author-email: oussama@jarrousse.org
 License: MIT
 Project-URL: Source, https://github.com/oussjarrousse/pytest-minio-mock/
 Project-URL: Tracker, https://github.com/oussjarrousse/pytest-minio-mock/issues
```

### Comparing `pytest_minio_mock-0.3.13/README.md` & `pytest_minio_mock-0.4.13/README.md`

 * *Files identical despite different names*

### Comparing `pytest_minio_mock-0.3.13/pytest_minio_mock/__init__.py` & `pytest_minio_mock-0.4.13/pytest_minio_mock/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 
 For more information and usage examples, please refer to the project's README.md.
 
 """
 
 __title__ = "pytest-minio-mock"
 __description__ = "A pytest plugin for mocking Minio S3 interactions"
-__version__ = "0.3.13"
+__version__ = "0.4.13"
 __status__ = "Production"
 __license__ = "MIT"
 __author__ = "Oussama Jarrousse"
 __maintainer__ = "Oussama Jarrousse"
 __email__ = "oussama@jarrousse.org"
 __credits__ = ["Gustavo Satheler", "@cottephi", "Wouter van Atteveldt"]
```

### Comparing `pytest_minio_mock-0.3.13/pytest_minio_mock/plugin.py` & `pytest_minio_mock-0.4.13/pytest_minio_mock/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,27 +17,27 @@
     minio_mock: A pytest fixture to patch the Minio client with a mock for testing.
 
 This module allows you to test file uploads, downloads, bucket creations, and other Minio operations
 by simulating the Minio environment. It's useful in scenarios where you want to ensure your
 application interacts correctly with Minio, without the overhead of connecting to an actual Minio
 server.
 """
-
 import copy
 import datetime
 import io
 import logging
 import os
 from uuid import uuid4
 
 import pytest
 import validators
 from minio import Minio
 from minio.commonconfig import ENABLED
-from minio.datatypes import Object, Bucket
+from minio.datatypes import Bucket
+from minio.datatypes import Object
 from minio.error import S3Error
 from minio.versioningconfig import OFF
 from minio.versioningconfig import SUSPENDED
 from minio.versioningconfig import VersioningConfig
 from urllib3.connection import HTTPConnection
 from urllib3.response import HTTPResponse
 
@@ -217,14 +217,41 @@
         # If versioning is OFF, there can only be one version of an object (store a read version_id non-the-less)
         if versioning.status == OFF:
             self._versions = {}
 
         self.put_object_version(version_id, obj)
         return obj
 
+    def stat_object(
+        self,
+        version_id,
+        versioning: VersioningConfig,
+        ssec=None,
+        extra_headers=None,
+        extra_query_params=None,
+    ):
+        """
+        Returns
+            the stat of the object if versioning is disabled
+            the stat of the latest version of the object if versioning is enabled
+        """
+        obj_version = self.get_object(version_id=version_id, versioning=versioning)
+        the_stat_object_version = Object(
+            bucket_name=self.bucket_name,
+            object_name=self.object_name,
+            last_modified=obj_version.last_modified,
+            version_id=None
+            if obj_version.version_id == "null"
+            else obj_version.version_id,
+            is_latest="true" if obj_version.is_latest else "false",
+            is_delete_marker=obj_version.is_delete_marker,
+        )
+
+        return the_stat_object_version
+
     def get_object(self, version_id, versioning: VersioningConfig):
         """
         Returns
             the stored object if versioning is disabled
             the latest version of the object if versioning is enabled
         """
         if version_id and version_id != "null" and not validators.uuid(version_id):
@@ -447,15 +474,15 @@
         )
 
         return obj
 
     def remove_object(self, object_name, version_id=None):
         """ """
         if object_name not in self.objects:
-            # object does not exist, so nothing to do
+            # Object does not exist, so nothing to do
             return
         try:
             if self.versioning.status == OFF:
                 if not version_id:
                     del self.objects[object_name]
                     return
             return self.objects[object_name].remove_object(version_id, self.versioning)
@@ -491,14 +518,71 @@
                 request_id=None,
                 code=e.code,
                 bucket_name=self.bucket_name,
                 object_name=object_name,
             )
         return the_object_version
 
+    def stat_object(
+        self,
+        object_name,
+        ssec=None,
+        version_id=None,
+        extra_headers=None,
+        extra_query_params=None,
+    ) -> Object:
+        """
+        Get object information and metadata of an object in the mock Minio server
+
+        Args:
+            object_name (str): The name of the object to remove.
+            ssec (SseCustomerKey| None, optional): Server-side encryption customer key.
+            version_id (str | None, optional): The version about which to retrieve information and metadata.
+            extra_headers ( dict | None, optional ):
+            extra_query_params ( dict | None, optional): Extra query parameters for advanced usage.
+
+        Returns:
+            Object: Object information as Object.
+        """
+
+        try:
+            the_object = self.objects[object_name]
+        except KeyError as e:
+            raise S3Error(
+                message="Object does not exist",
+                resource=f"/{self.bucket_name}/{object_name}",
+                request_id=None,
+                host_id=None,
+                response="mocked_response",
+                code="NoSuchKey",
+                bucket_name=self.bucket_name,
+                object_name=object_name,
+            )
+
+        try:
+            the_object_version_stat = the_object.stat_object(
+                version_id=version_id,
+                versioning=self.versioning,
+                ssec=ssec,
+                extra_headers=extra_headers,
+                extra_query_params=extra_query_params,
+            )
+        except S3Error as e:
+            raise S3Error(
+                message=e.message,
+                response=e.response,
+                resource=f"/{self.bucket_name}/{object_name}",
+                host_id=None,
+                request_id=None,
+                code=e.code,
+                bucket_name=self.bucket_name,
+                object_name=object_name,
+            )
+        return the_object_version_stat
+
     def list_objects(
         self,
         prefix=None,
         recursive=False,
         start_after=None,
         include_version=False,
     ):
@@ -533,20 +617,20 @@
                         continue
                 # Directly add the object for recursive listing
                 # or if it's a file in the current directory
                 if include_version:
                     # Minio API always sort versions by time,
                     # it also includes delete markers at the end newwst first
                     versions_list = obj.list_versions()
-                    for version, obj_version in versions_list:
+                    for version_id, obj_version in versions_list:
                         yield Object(
                             bucket_name=self.bucket_name,
                             object_name=object_name,
                             last_modified=obj_version.last_modified,
-                            version_id=version,
+                            version_id=version_id,
                             is_latest="true" if obj_version.is_latest else "false",
                             is_delete_marker=obj_version.is_delete_marker,
                         )
                 else:
                     obj_version = obj.get_latest()
                     # only yield if the object is not a delete marker
                     if not obj_version.is_delete_marker:
@@ -770,28 +854,27 @@
             None: The method writes the object's data to a file and has no return value.
         """
         the_object = self.get_object(
             bucket_name,
             object_name,
             version_id=version_id,
             request_headers=request_headers,
-            sse=sse,
             extra_query_params=extra_query_params,
         )
         with open(file_path, "wb") as f:
             f.write(the_object.data)
 
     def get_object(
         self,
         bucket_name,
         object_name,
         offset: int = 0,
         length: int = 0,
         request_headers=None,
-        sse=None,
+        ssec=None,
         version_id=None,
         extra_query_params=None,
     ):
         """
         Retrieves an object from the mock Minio server.
 
         Simulates the retrieval of an object's content from a specified bucket, allowing for
@@ -801,15 +884,15 @@
             bucket_name (str): The name of the bucket.
             object_name (str): The name of the object to retrieve.
             offset (int, optional): The start byte position of object data to retrieve. Defaults
                 to 0.
             length (int, optional): The number of bytes of object data to retrieve. Defaults to 0,
                 which means the whole object.
             request_headers (dict, optional): Additional headers for the request. Defaults to None.
-            sse (optional): Server-side encryption option. Defaults to None.
+            ssec ( SseCustomerKey | None, optional): Server-side encryption option. Defaults to None.
             version_id (str | None, optional): The version ID of the object. Defaults to None.
             extra_query_params (dict, optional): Additional query parameters. Defaults to None.
 
         Returns:
             HTTPResponse: A response object containing the object data.
         """
         self._health_check()
@@ -1071,15 +1154,18 @@
         Simulates listing all the buckets available to the user in the Minio server.
 
         Returns:
             list: A list of bucket names.
         """
         try:
             self._health_check()
-            return [Bucket(name, bucket._creation_date) for (name, bucket) in list(self.buckets.items())]
+            return [
+                Bucket(name, bucket._creation_date)
+                for (name, bucket) in list(self.buckets.items())
+            ]
         except Exception as e:
             logging.error(e)
             raise e
 
     def bucket_exists(self, bucket_name):
         """
         Checks if a bucket exists in the mock Minio server.
@@ -1257,14 +1343,56 @@
             None: The method has no return value but indicates successful removal.
         """
         self._health_check()
         return self.buckets[bucket_name].remove_object(
             object_name, version_id=version_id
         )
 
+    def stat_object(
+        self,
+        bucket_name,
+        object_name,
+        ssec=None,
+        version_id=None,
+        extra_headers=None,
+        extra_query_params=None,
+    ) -> Object:
+        """
+        Get object information and metadata of an object in the mock Minio server
+
+        Args:
+            bucket_name (str): The name of the bucket.
+            object_name (str): The name of the object to remove.
+            ssec (SseCustomerKey| None, optional): Server-side encryption customer key.
+            version_id (str | None, optional): The version about which to retrieve information and metadata.
+            extra_headers ( dict | None, optional ):
+            extra_query_params ( dict | None, optional): Extra query parameters for advanced usage.
+
+        Raises:
+            S3Error:
+
+        Returns:
+            Object: Object information as Object.
+
+        """
+        self._health_check()
+
+        the_stat_object = self.buckets[bucket_name].stat_object(
+            object_name=object_name,
+            ssec=ssec,
+            version_id=version_id,
+            extra_headers=extra_headers,
+            extra_query_params=extra_query_params,
+        )
+
+        if not the_stat_object:
+            raise RuntimeError("Implementation Error")
+
+        return the_stat_object
+
 
 @pytest.fixture
 def minio_mock_servers():
     """
     Pytest fixture to yield a Servers instance.
 
     Yields:
```

### Comparing `pytest_minio_mock-0.3.13/pytest_minio_mock.egg-info/PKG-INFO` & `pytest_minio_mock-0.4.13/pytest_minio_mock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-minio-mock
-Version: 0.3.13
+Version: 0.4.13
 Summary: A pytest plugin for mocking Minio S3 interactions
 Home-page: https://github.com/oussjarrousse/pytest-minio-mock
 Author: Oussama Jarrousse
 Author-email: oussama@jarrousse.org
 License: MIT
 Project-URL: Source, https://github.com/oussjarrousse/pytest-minio-mock/
 Project-URL: Tracker, https://github.com/oussjarrousse/pytest-minio-mock/issues
```

### Comparing `pytest_minio_mock-0.3.13/setup.py` & `pytest_minio_mock-0.4.13/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     license="MIT",
     author="Oussama Jarrousse",
     author_email="oussama@jarrousse.org",
     description="A pytest plugin for mocking Minio S3 interactions",
     long_description=open("README.md").read(),
     keywords="pytest minio mock",
     extras_require={"dev": ["pre-commit", "tox"]},
-    version="0.3.13",
+    version="0.4.13",
     long_description_content_type="text/markdown",
     classifiers=[
         "Framework :: Pytest",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
```

### Comparing `pytest_minio_mock-0.3.13/tests/test_minio_mock.py` & `pytest_minio_mock-0.4.13/tests/test_minio_mock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import sys
 
 import pytest
 import validators
 from minio import Minio
 from minio.commonconfig import ENABLED
+from minio.datatypes import Bucket
 from minio.error import S3Error
 from minio.versioningconfig import OFF
 from minio.versioningconfig import SUSPENDED
 from minio.versioningconfig import VersioningConfig
-from minio.datatypes import Bucket
 
 from pytest_minio_mock.plugin import MockMinioBucket
 from pytest_minio_mock.plugin import MockMinioObject
 
 
 @pytest.mark.UNIT
 class TestsMockMinioObject:
@@ -443,7 +443,53 @@
     client_1_buckets = ["bucket-1", "bucket-2", "bucket-3"]
     for bucket in client_1_buckets:
         client_1.make_bucket(bucket)
 
     client_2 = Minio("http://local.host:9000")
     client_2_buckets = client_2.list_buckets()
     assert client_2_buckets == client_1_buckets
+
+
+@pytest.mark.UNIT
+def test_stat_object(minio_mock):
+    bucket_name = "test-bucket"
+    object_name = "test-object"
+    file_path = "tests/fixtures/maya.jpeg"
+
+    client = Minio("http://local.host:9000")
+    client.make_bucket(bucket_name)
+    client.fput_object(bucket_name, object_name, file_path)
+
+    object_stat = client.stat_object(bucket_name=bucket_name, object_name=object_name)
+
+    assert object_stat.bucket_name == bucket_name
+    assert object_stat.object_name == object_name
+    assert object_stat.version_id is None
+
+    client.remove_object(bucket_name, object_name)
+
+    with pytest.raises(S3Error) as error:
+        _ = client.stat_object(bucket_name=bucket_name, object_name=object_name)
+    assert error.value.code == "NoSuchKey"
+    assert error.value.message == "Object does not exist"
+
+    client.fput_object(bucket_name, object_name, file_path)
+    client.set_bucket_versioning(bucket_name, VersioningConfig(ENABLED))
+
+    object_stat = client.stat_object(bucket_name=bucket_name, object_name=object_name)
+    assert object_stat.bucket_name == bucket_name
+    assert object_stat.object_name == object_name
+    assert object_stat.version_id is None
+    object_stat = client.stat_object(
+        bucket_name=bucket_name, object_name=object_name, version_id="null"
+    )
+    assert object_stat.bucket_name == bucket_name
+    assert object_stat.object_name == object_name
+    assert object_stat.version_id is None
+    client.fput_object(bucket_name, object_name, file_path)
+    objects = list(client.list_objects(bucket_name=bucket_name, include_version=True))
+    object_stat = client.stat_object(
+        bucket_name=bucket_name,
+        object_name=object_name,
+        version_id=objects[1].version_id,
+    )
+    assert object_stat.version_id is None
```

