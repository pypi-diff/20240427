# Comparing `tmp/latch_cloud_clients-0.1.6.tar.gz` & `tmp/latch_cloud_clients-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_cloud_clients-0.1.6.tar", max compression
+gzip compressed data, was "latch_cloud_clients-0.1.7.tar", max compression
```

## Comparing `latch_cloud_clients-0.1.6.tar` & `latch_cloud_clients-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     7052 2024-04-19 18:57:40.206110 latch_cloud_clients-0.1.6/LICENSE
--rw-r--r--   0        0        0      121 2024-04-24 21:08:53.493221 latch_cloud_clients-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-04-19 18:57:40.207571 latch_cloud_clients-0.1.6/latch_cloud_clients/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 19:11:11.691773 latch_cloud_clients-0.1.6/latch_cloud_clients/aws/__init__.py
--rw-r--r--   0        0        0    14297 2024-04-25 15:28:32.366171 latch_cloud_clients-0.1.6/latch_cloud_clients/aws/storage_client.py
--rw-r--r--   0        0        0        0 2024-04-23 19:28:36.193575 latch_cloud_clients-0.1.6/latch_cloud_clients/gcp/__init__.py
--rw-r--r--   0        0        0     2923 2024-04-24 18:33:31.527944 latch_cloud_clients-0.1.6/latch_cloud_clients/gcp/client_pool.py
--rw-r--r--   0        0        0    18229 2024-04-25 20:54:06.787355 latch_cloud_clients-0.1.6/latch_cloud_clients/gcp/storage.py
--rw-r--r--   0        0        0     9534 2024-04-25 16:52:13.344438 latch_cloud_clients-0.1.6/latch_cloud_clients/gcp/storage_client.py
--rw-r--r--   0        0        0      790 2024-04-24 21:40:21.430232 latch_cloud_clients-0.1.6/latch_cloud_clients/get_storage_client.py
--rw-r--r--   0        0        0        0 2024-04-19 18:57:40.208421 latch_cloud_clients-0.1.6/latch_cloud_clients/py.typed
--rw-r--r--   0        0        0     2944 2024-04-25 01:41:32.831875 latch_cloud_clients-0.1.6/latch_cloud_clients/utils.py
--rw-r--r--   0        0        0     1502 2024-04-25 20:54:14.877493 latch_cloud_clients-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 latch_cloud_clients-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     7052 2024-04-19 18:57:40.206110 latch_cloud_clients-0.1.7/LICENSE
+-rw-r--r--   0        0        0      121 2024-04-24 21:08:53.493221 latch_cloud_clients-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 18:57:40.207571 latch_cloud_clients-0.1.7/latch_cloud_clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 19:11:11.691773 latch_cloud_clients-0.1.7/latch_cloud_clients/aws/__init__.py
+-rw-r--r--   0        0        0    14297 2024-04-25 15:28:32.366171 latch_cloud_clients-0.1.7/latch_cloud_clients/aws/storage_client.py
+-rw-r--r--   0        0        0        0 2024-04-23 19:28:36.193575 latch_cloud_clients-0.1.7/latch_cloud_clients/gcp/__init__.py
+-rw-r--r--   0        0        0     2923 2024-04-24 18:33:31.527944 latch_cloud_clients-0.1.7/latch_cloud_clients/gcp/client_pool.py
+-rw-r--r--   0        0        0    18315 2024-04-26 22:16:26.369378 latch_cloud_clients-0.1.7/latch_cloud_clients/gcp/storage.py
+-rw-r--r--   0        0        0     9534 2024-04-25 16:52:13.344438 latch_cloud_clients-0.1.7/latch_cloud_clients/gcp/storage_client.py
+-rw-r--r--   0        0        0      809 2024-04-26 17:58:15.128561 latch_cloud_clients-0.1.7/latch_cloud_clients/get_storage_client.py
+-rw-r--r--   0        0        0        0 2024-04-19 18:57:40.208421 latch_cloud_clients-0.1.7/latch_cloud_clients/py.typed
+-rw-r--r--   0        0        0     2944 2024-04-25 01:41:32.831875 latch_cloud_clients-0.1.7/latch_cloud_clients/utils.py
+-rw-r--r--   0        0        0     1502 2024-04-26 22:18:25.682336 latch_cloud_clients-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 latch_cloud_clients-0.1.7/PKG-INFO
```

### Comparing `latch_cloud_clients-0.1.6/LICENSE` & `latch_cloud_clients-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.6/latch_cloud_clients/aws/storage_client.py` & `latch_cloud_clients-0.1.7/latch_cloud_clients/aws/storage_client.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.6/latch_cloud_clients/gcp/client_pool.py` & `latch_cloud_clients-0.1.7/latch_cloud_clients/gcp/client_pool.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.6/latch_cloud_clients/gcp/storage.py` & `latch_cloud_clients-0.1.7/latch_cloud_clients/gcp/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,20 +350,23 @@
     async def delete_blob(
         self, bucket_name: str, key: str, generation: str | None = None
     ):
         params = {}
         if generation is not None:
             params["generation"] = generation
 
-        await self._make_api_request(
-            "DELETE",
-            urljoin(self.api_url, f"b/{bucket_name}/o/{quote(key, safe='')}"),
-            "DeleteBlob",
-            params=params,
-        )
+        try:
+            await self._make_api_request(
+                "DELETE",
+                urljoin(self.api_url, f"b/{bucket_name}/o/{quote(key, safe='')}"),
+                "DeleteBlob",
+                params=params,
+            )
+        except NotFound:
+            return None
 
     def get_signed_download_url(
         self,
         bucket_name: str,
         key: str | None,
         content_disposition: str | None = None,
         content_type: str | None = None,
```

### Comparing `latch_cloud_clients-0.1.6/latch_cloud_clients/gcp/storage_client.py` & `latch_cloud_clients-0.1.7/latch_cloud_clients/gcp/storage_client.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.6/latch_cloud_clients/get_storage_client.py` & `latch_cloud_clients-0.1.7/latch_cloud_clients/get_storage_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,13 +18,13 @@
 def get_storage_client(root_type: LDataNodeType | None) -> StorageClient:
     if root_type is not None and root_type not in [
         LDataNodeType.account_root,
         LDataNodeType.mount,
         LDataNodeType.mount_gcp,
         LDataNodeType.mount_azure,
     ]:
-        raise ValueError("Root is not a mount")
+        raise ValueError(f"Root is not a mount, got: {root_type}")
 
     if root_type == LDataNodeType.mount_gcp:
         return GCPStorageClient()
     else:
         return S3StorageClient()
```

### Comparing `latch_cloud_clients-0.1.6/latch_cloud_clients/utils.py` & `latch_cloud_clients-0.1.7/latch_cloud_clients/utils.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.6/pyproject.toml` & `latch_cloud_clients-0.1.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latch-cloud-clients"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Taras Priadka <taras@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_cloud_clients"}]
 
 [tool.poetry.dependencies]
```

### Comparing `latch_cloud_clients-0.1.6/PKG-INFO` & `latch_cloud_clients-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latch-cloud-clients
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 License: CC0 1.0
 Author: Taras Priadka
 Author-email: taras@latch.bio
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

