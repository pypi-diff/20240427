# Comparing `tmp/astrapy-1.0.0rc1.tar.gz` & `tmp/astrapy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrapy-1.0.0rc1.tar", max compression
+gzip compressed data, was "astrapy-1.1.0.tar", max compression
```

## Comparing `astrapy-1.0.0rc1.tar` & `astrapy-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-10-20 10:38:03.741711 astrapy-1.0.0rc1/LICENSE.md
--rw-r--r--   0        0        0    10974 2024-04-08 08:38:26.205443 astrapy-1.0.0rc1/README.md
--rw-r--r--   0        0        0     2653 2024-04-08 10:22:20.216094 astrapy-1.0.0rc1/astrapy/__init__.py
--rw-r--r--   0        0        0    82432 2024-04-08 08:35:47.194001 astrapy-1.0.0rc1/astrapy/admin.py
--rw-r--r--   0        0        0      727 2024-03-11 09:47:43.734364 astrapy-1.0.0rc1/astrapy/api/__init__.py
--rw-r--r--   0        0        0    17415 2024-04-08 08:35:47.194001 astrapy-1.0.0rc1/astrapy/client.py
--rw-r--r--   0        0        0   212238 2024-04-08 08:38:26.209443 astrapy-1.0.0rc1/astrapy/collection.py
--rw-r--r--   0        0        0     3004 2024-04-08 08:35:47.194001 astrapy-1.0.0rc1/astrapy/constants.py
--rw-r--r--   0        0        0      569 2024-03-11 09:47:43.734364 astrapy-1.0.0rc1/astrapy/core/__init__.py
--rw-r--r--   0        0        0     6136 2024-03-20 08:51:12.760597 astrapy-1.0.0rc1/astrapy/core/api.py
--rw-r--r--   0        0        0     1692 2024-03-20 08:51:12.760597 astrapy-1.0.0rc1/astrapy/core/core_types.py
--rw-r--r--   0        0        0   126840 2024-04-08 08:38:26.209443 astrapy-1.0.0rc1/astrapy/core/db.py
--rw-r--r--   0        0        0     1009 2024-03-20 08:51:12.764597 astrapy-1.0.0rc1/astrapy/core/defaults.py
--rw-r--r--   0        0        0      907 2024-03-20 08:51:12.764597 astrapy-1.0.0rc1/astrapy/core/ids.py
--rw-r--r--   0        0        0    46165 2024-04-08 08:35:47.198001 astrapy-1.0.0rc1/astrapy/core/ops.py
--rw-r--r--   0        0        0    13214 2024-03-26 11:39:32.183165 astrapy-1.0.0rc1/astrapy/core/utils.py
--rw-r--r--   0        0        0    35775 2024-04-08 08:35:47.198001 astrapy-1.0.0rc1/astrapy/cursors.py
--rw-r--r--   0        0        0    61320 2024-04-08 08:38:26.209443 astrapy-1.0.0rc1/astrapy/database.py
--rw-r--r--   0        0        0      888 2024-03-22 10:30:22.402650 astrapy-1.0.0rc1/astrapy/db/__init__.py
--rw-r--r--   0        0        0    28390 2024-04-08 08:35:47.198001 astrapy-1.0.0rc1/astrapy/exceptions.py
--rw-r--r--   0        0        0      874 2024-03-22 14:33:28.281929 astrapy-1.0.0rc1/astrapy/ids.py
--rw-r--r--   0        0        0    14210 2024-04-08 08:38:26.209443 astrapy-1.0.0rc1/astrapy/info.py
--rw-r--r--   0        0        0    29870 2024-04-08 08:38:26.209443 astrapy-1.0.0rc1/astrapy/operations.py
--rw-r--r--   0        0        0      717 2024-03-11 09:47:43.734364 astrapy-1.0.0rc1/astrapy/ops/__init__.py
--rw-r--r--   0        0        0        0 2023-12-06 09:49:25.678169 astrapy-1.0.0rc1/astrapy/py.typed
--rw-r--r--   0        0        0     6111 2024-03-14 10:05:46.376976 astrapy-1.0.0rc1/astrapy/results.py
--rw-r--r--   0        0        0     2113 2024-04-08 09:04:51.888478 astrapy-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0    12161 1970-01-01 00:00:00.000000 astrapy-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-10-19 21:10:53.110159 astrapy-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0    11564 2024-04-17 21:17:22.390941 astrapy-1.1.0/README.md
+-rw-r--r--   0        0        0     2653 2024-04-16 08:29:58.955559 astrapy-1.1.0/astrapy/__init__.py
+-rw-r--r--   0        0        0    82432 2024-04-16 08:29:58.955559 astrapy-1.1.0/astrapy/admin.py
+-rw-r--r--   0        0        0      727 2024-04-16 08:29:58.955559 astrapy-1.1.0/astrapy/api/__init__.py
+-rw-r--r--   0        0        0    17415 2024-04-16 08:29:58.955559 astrapy-1.1.0/astrapy/client.py
+-rw-r--r--   0        0        0   214387 2024-04-27 10:55:31.525851 astrapy-1.1.0/astrapy/collection.py
+-rw-r--r--   0        0        0     3004 2024-04-16 08:29:58.959558 astrapy-1.1.0/astrapy/constants.py
+-rw-r--r--   0        0        0      569 2024-04-16 08:29:58.959558 astrapy-1.1.0/astrapy/core/__init__.py
+-rw-r--r--   0        0        0     6136 2024-04-16 08:29:58.959558 astrapy-1.1.0/astrapy/core/api.py
+-rw-r--r--   0        0        0     1692 2024-04-16 08:29:58.959558 astrapy-1.1.0/astrapy/core/core_types.py
+-rw-r--r--   0        0        0   126840 2024-04-16 08:29:58.959558 astrapy-1.1.0/astrapy/core/db.py
+-rw-r--r--   0        0        0     1009 2024-04-16 08:29:58.959558 astrapy-1.1.0/astrapy/core/defaults.py
+-rw-r--r--   0        0        0      907 2024-04-16 08:29:58.963558 astrapy-1.1.0/astrapy/core/ids.py
+-rw-r--r--   0        0        0    46165 2024-04-16 08:29:58.963558 astrapy-1.1.0/astrapy/core/ops.py
+-rw-r--r--   0        0        0    13214 2024-04-16 08:29:58.963558 astrapy-1.1.0/astrapy/core/utils.py
+-rw-r--r--   0        0        0    35775 2024-04-16 08:29:58.963558 astrapy-1.1.0/astrapy/cursors.py
+-rw-r--r--   0        0        0    61320 2024-04-16 08:29:58.963558 astrapy-1.1.0/astrapy/database.py
+-rw-r--r--   0        0        0      888 2024-04-16 08:29:58.963558 astrapy-1.1.0/astrapy/db/__init__.py
+-rw-r--r--   0        0        0    28390 2024-04-16 08:29:58.963558 astrapy-1.1.0/astrapy/exceptions.py
+-rw-r--r--   0        0        0      874 2024-04-16 08:29:58.963558 astrapy-1.1.0/astrapy/ids.py
+-rw-r--r--   0        0        0    14210 2024-04-16 08:29:58.967558 astrapy-1.1.0/astrapy/info.py
+-rw-r--r--   0        0        0    29870 2024-04-16 08:29:58.967558 astrapy-1.1.0/astrapy/operations.py
+-rw-r--r--   0        0        0      717 2024-04-16 08:29:58.967558 astrapy-1.1.0/astrapy/ops/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 09:22:49.497793 astrapy-1.1.0/astrapy/py.typed
+-rw-r--r--   0        0        0     6111 2024-04-16 08:29:58.967558 astrapy-1.1.0/astrapy/results.py
+-rw-r--r--   0        0        0     2110 2024-04-27 10:55:31.525851 astrapy-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    12748 1970-01-01 00:00:00.000000 astrapy-1.1.0/PKG-INFO
```

### Comparing `astrapy-1.0.0rc1/LICENSE.md` & `astrapy-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `astrapy-1.0.0rc1/README.md` & `astrapy-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # AstraPy
 
 A pythonic client for [DataStax Astra DB](https://astra.datastax.com).
 
-_This README targets AstraPy version **1.0.0+**, which introducesa a whole new API. Click [here](https://github.com/datastax/astrapy/blob/cd3f5ce8146093e10a095709c0f5c3f8e3f2c7da/README.md) for the pre-existing API (fully compatible with newer versions)._
+_This README targets AstraPy version **1.0.0+**, which introduces a whole new API.
+Click [here](https://github.com/datastax/astrapy/blob/cd3f5ce8146093e10a095709c0f5c3f8e3f2c7da/README.md) for the pre-existing API (fully compatible with newer versions)._
 
 
 ## Quickstart
 
 Install with `pip install astrapy`.
 
 Get the *API Endpoint* and the *Token* to your Astra DB instance at [astra.datastax.com](https://astra.datastax.com).
@@ -67,26 +68,26 @@
 #   Surfers' paradise: 0.98238194
 #   Friendly aliens in town: 0.91873914
 ```
 
 Next steps:
 
 - More info and usage patterns are given in the docstrings of classes and methods
-- [AstraPy reference](https://docs.datastax.com/en/astra/astra-db-vector/clients/python.html)
-- [Data API reference](https://docs.datastax.com/en/astra/astra-db-vector/api-reference/data-api-commands.html)
+- [Data API reference](https://docs.datastax.com/en/astra/astra-db-vector/api-reference/overview.html)
+- [AstraPy reference](https://docs.datastax.com/en/astra/astra-db-vector/api-reference/dataapiclient.html)
 - Package on [PyPI](https://pypi.org/project/astrapy/)
 
 ## AstraPy's API
 
 ### Abstraction diagram
 
 AstraPy's abstractions for working at the data and admin layers are structured
 as depicted by this diagram:
 
-![AstraPy, abstractions chart](pictures/astrapy_abstractions.png)
+![AstraPy, abstractions chart](https://raw.githubusercontent.com/datastax/astrapy/master/pictures/astrapy_abstractions.png)
 
 Here's a small admin-oriented example:
 
 ```python
 import astrapy
 
 my_client = astrapy.DataAPIClient("AstraCS:...")
@@ -104,15 +105,15 @@
 my_database_admin.create_namespace("my_dreamspace")
 ```
 
 ### Exceptions
 
 The package comes with its own set of exceptions, arranged in this hierarchy:
 
-![AstraPy, exception hierarchy](pictures/astrapy_exceptions.png)
+![AstraPy, exception hierarchy](https://raw.githubusercontent.com/datastax/astrapy/master/pictures/astrapy_exceptions.png)
 
 For more information, and code examples, check out the docstrings and consult
 the API reference linked above.
 
 ### Working with dates
 
 Date and datetime objects, i.e. instances of the standard library
@@ -194,42 +195,53 @@
 ```
 
 Features must be thoroughly covered in tests (see `tests/idiomatic/*` for
 naming convention and module structure).
 
 ### Running tests
 
-Full testing requires environment variables:
+"Full regular" testing requires environment variables:
 
 ```bash
 export ASTRA_DB_APPLICATION_TOKEN="AstraCS:..."
 export ASTRA_DB_API_ENDPOINT="https://.......apps.astra.datastax.com"
 
 export ASTRA_DB_KEYSPACE="default_keyspace"
 # Optional:
 export ASTRA_DB_SECONDARY_KEYSPACE="..."
 ```
 
 Tests can be started in various ways:
 
 ```bash
-# test the core modules
-poetry run pytest tests/core
 # test the "idiomatic" layer
 poetry run pytest tests/idiomatic
 poetry run pytest tests/idiomatic/unit
 poetry run pytest tests/idiomatic/integration
 
 # remove logging noise:
 poetry run pytest [...] -o log_cli=0
+```
+
+The above runs the regular testing (i.e. non-Admin, non-core).
+The (idiomatic) Admin part is tested manually by you, on Astra accounts with room
+for up to 3 new databases, possibly both on prod and dev, and uses specific env vars,
+as can be seen on `tests/idiomatic/integration/test_admin.py`.
+
+Should you be interested in testing the "core" modules, moreover,
+this is also something for you to run manually (do that if you touch "core"):
+
+```bash
+# test the core modules
+poetry run pytest tests/core
 
 # do not drop collections:
 TEST_SKIP_COLLECTION_DELETE=1 poetry run pytest [...]
 
-# include astrapy.core.ops testing (must cleanup after that):
+# include astrapy.core.ops testing (tester must clean up after that):
 TEST_ASTRADBOPS=1 poetry run pytest [...]
 ```
 
 ## Appendices
 
 ### Appendix A: quick reference for imports
```

### Comparing `astrapy-1.0.0rc1/astrapy/__init__.py` & `astrapy-1.1.0/astrapy/__init__.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.0.0rc1/astrapy/admin.py` & `astrapy-1.1.0/astrapy/admin.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.0.0rc1/astrapy/api/__init__.py` & `astrapy-1.1.0/astrapy/api/__init__.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.0.0rc1/astrapy/client.py` & `astrapy-1.1.0/astrapy/client.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.0.0rc1/astrapy/collection.py` & `astrapy-1.1.0/astrapy/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1262,14 +1262,47 @@
                     return count
         else:
             raise DataAPIFaultyResponseException(
                 text="Faulty response from count_documents API command.",
                 raw_response=cd_response,
             )
 
+    def estimated_document_count(
+        self,
+        *,
+        max_time_ms: Optional[int] = None,
+    ) -> int:
+        """
+        Query the API server for an estimate of the document count in the collection.
+
+        Contrary to `count_documents`, this method has no filtering parameters.
+
+        Args:
+            max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+
+        Returns:
+            a server-provided estimate count of the documents in the collection.
+
+        Example:
+            >>> my_coll.estimated_document_count()
+            35700
+        """
+        ed_response = self.command(
+            {"estimatedDocumentCount": {}},
+            max_time_ms=max_time_ms,
+        )
+        if "count" in ed_response.get("status", {}):
+            count: int = ed_response["status"]["count"]
+            return count
+        else:
+            raise DataAPIFaultyResponseException(
+                text="Faulty response from estimated_document_count API command.",
+                raw_response=ed_response,
+            )
+
     @recast_method_sync
     def find_one_and_replace(
         self,
         filter: Dict[str, Any],
         replacement: DocumentType,
         *,
         projection: Optional[ProjectionType] = None,
@@ -3490,14 +3523,47 @@
                     return count
         else:
             raise DataAPIFaultyResponseException(
                 text="Faulty response from count_documents API command.",
                 raw_response=cd_response,
             )
 
+    async def estimated_document_count(
+        self,
+        *,
+        max_time_ms: Optional[int] = None,
+    ) -> int:
+        """
+        Query the API server for an estimate of the document count in the collection.
+
+        Contrary to `count_documents`, this method has no filtering parameters.
+
+        Args:
+            max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+
+        Returns:
+            a server-provided estimate count of the documents in the collection.
+
+        Example:
+            >>> asyncio.run(my_async_coll.estimated_document_count())
+            35700
+        """
+        ed_response = await self.command(
+            {"estimatedDocumentCount": {}},
+            max_time_ms=max_time_ms,
+        )
+        if "count" in ed_response.get("status", {}):
+            count: int = ed_response["status"]["count"]
+            return count
+        else:
+            raise DataAPIFaultyResponseException(
+                text="Faulty response from estimated_document_count API command.",
+                raw_response=ed_response,
+            )
+
     @recast_method_async
     async def find_one_and_replace(
         self,
         filter: Dict[str, Any],
         replacement: DocumentType,
         *,
         projection: Optional[ProjectionType] = None,
```

### Comparing `astrapy-1.0.0rc1/astrapy/constants.py` & `astrapy-1.1.0/astrapy/constants.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.0.0rc1/astrapy/core/__init__.py` & `astrapy-1.1.0/astrapy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.0.0rc1/astrapy/core/api.py` & `astrapy-1.1.0/astrapy/core/api.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.0.0rc1/astrapy/core/core_types.py` & `astrapy-1.1.0/astrapy/core/core_types.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.0.0rc1/astrapy/core/db.py` & `astrapy-1.1.0/astrapy/core/db.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.0.0rc1/astrapy/core/defaults.py` & `astrapy-1.1.0/astrapy/core/defaults.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.0.0rc1/astrapy/core/ids.py` & `astrapy-1.1.0/astrapy/core/ids.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.0.0rc1/astrapy/core/ops.py` & `astrapy-1.1.0/astrapy/core/ops.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.0.0rc1/astrapy/core/utils.py` & `astrapy-1.1.0/astrapy/core/utils.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.0.0rc1/astrapy/cursors.py` & `astrapy-1.1.0/astrapy/cursors.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.0.0rc1/astrapy/database.py` & `astrapy-1.1.0/astrapy/database.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.0.0rc1/astrapy/db/__init__.py` & `astrapy-1.1.0/astrapy/db/__init__.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.0.0rc1/astrapy/exceptions.py` & `astrapy-1.1.0/astrapy/exceptions.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.0.0rc1/astrapy/ids.py` & `astrapy-1.1.0/astrapy/ids.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.0.0rc1/astrapy/info.py` & `astrapy-1.1.0/astrapy/info.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.0.0rc1/astrapy/operations.py` & `astrapy-1.1.0/astrapy/operations.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.0.0rc1/astrapy/ops/__init__.py` & `astrapy-1.1.0/astrapy/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.0.0rc1/astrapy/results.py` & `astrapy-1.1.0/astrapy/results.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.0.0rc1/pyproject.toml` & `astrapy-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "astrapy"
-version = "1.0.0rc1"
+version = "1.1.0"
 description = "AstraPy is a Pythonic SDK for DataStax Astra and its Data API"
 authors = [
     "Stefano Lottini <stefano.lottini@datastax.com>",
     "Eric Hare <eric.hare@datastax.com>",
 ]
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `astrapy-1.0.0rc1/PKG-INFO` & `astrapy-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrapy
-Version: 1.0.0rc1
+Version: 1.1.0
 Summary: AstraPy is a Pythonic SDK for DataStax Astra and its Data API
 Home-page: https://github.com/datastax/astrapy
 License: Apache-2.0
 Keywords: DataStax,Astra
 Author: Stefano Lottini
 Author-email: stefano.lottini@datastax.com
 Requires-Python: >=3.8.0,<4.0.0
@@ -27,15 +27,16 @@
 Project-URL: Repository, https://github.com/datastax/astrapy
 Description-Content-Type: text/markdown
 
 # AstraPy
 
 A pythonic client for [DataStax Astra DB](https://astra.datastax.com).
 
-_This README targets AstraPy version **1.0.0+**, which introducesa a whole new API. Click [here](https://github.com/datastax/astrapy/blob/cd3f5ce8146093e10a095709c0f5c3f8e3f2c7da/README.md) for the pre-existing API (fully compatible with newer versions)._
+_This README targets AstraPy version **1.0.0+**, which introduces a whole new API.
+Click [here](https://github.com/datastax/astrapy/blob/cd3f5ce8146093e10a095709c0f5c3f8e3f2c7da/README.md) for the pre-existing API (fully compatible with newer versions)._
 
 
 ## Quickstart
 
 Install with `pip install astrapy`.
 
 Get the *API Endpoint* and the *Token* to your Astra DB instance at [astra.datastax.com](https://astra.datastax.com).
@@ -96,26 +97,26 @@
 #   Surfers' paradise: 0.98238194
 #   Friendly aliens in town: 0.91873914
 ```
 
 Next steps:
 
 - More info and usage patterns are given in the docstrings of classes and methods
-- [AstraPy reference](https://docs.datastax.com/en/astra/astra-db-vector/clients/python.html)
-- [Data API reference](https://docs.datastax.com/en/astra/astra-db-vector/api-reference/data-api-commands.html)
+- [Data API reference](https://docs.datastax.com/en/astra/astra-db-vector/api-reference/overview.html)
+- [AstraPy reference](https://docs.datastax.com/en/astra/astra-db-vector/api-reference/dataapiclient.html)
 - Package on [PyPI](https://pypi.org/project/astrapy/)
 
 ## AstraPy's API
 
 ### Abstraction diagram
 
 AstraPy's abstractions for working at the data and admin layers are structured
 as depicted by this diagram:
 
-![AstraPy, abstractions chart](pictures/astrapy_abstractions.png)
+![AstraPy, abstractions chart](https://raw.githubusercontent.com/datastax/astrapy/master/pictures/astrapy_abstractions.png)
 
 Here's a small admin-oriented example:
 
 ```python
 import astrapy
 
 my_client = astrapy.DataAPIClient("AstraCS:...")
@@ -133,15 +134,15 @@
 my_database_admin.create_namespace("my_dreamspace")
 ```
 
 ### Exceptions
 
 The package comes with its own set of exceptions, arranged in this hierarchy:
 
-![AstraPy, exception hierarchy](pictures/astrapy_exceptions.png)
+![AstraPy, exception hierarchy](https://raw.githubusercontent.com/datastax/astrapy/master/pictures/astrapy_exceptions.png)
 
 For more information, and code examples, check out the docstrings and consult
 the API reference linked above.
 
 ### Working with dates
 
 Date and datetime objects, i.e. instances of the standard library
@@ -223,42 +224,53 @@
 ```
 
 Features must be thoroughly covered in tests (see `tests/idiomatic/*` for
 naming convention and module structure).
 
 ### Running tests
 
-Full testing requires environment variables:
+"Full regular" testing requires environment variables:
 
 ```bash
 export ASTRA_DB_APPLICATION_TOKEN="AstraCS:..."
 export ASTRA_DB_API_ENDPOINT="https://.......apps.astra.datastax.com"
 
 export ASTRA_DB_KEYSPACE="default_keyspace"
 # Optional:
 export ASTRA_DB_SECONDARY_KEYSPACE="..."
 ```
 
 Tests can be started in various ways:
 
 ```bash
-# test the core modules
-poetry run pytest tests/core
 # test the "idiomatic" layer
 poetry run pytest tests/idiomatic
 poetry run pytest tests/idiomatic/unit
 poetry run pytest tests/idiomatic/integration
 
 # remove logging noise:
 poetry run pytest [...] -o log_cli=0
+```
+
+The above runs the regular testing (i.e. non-Admin, non-core).
+The (idiomatic) Admin part is tested manually by you, on Astra accounts with room
+for up to 3 new databases, possibly both on prod and dev, and uses specific env vars,
+as can be seen on `tests/idiomatic/integration/test_admin.py`.
+
+Should you be interested in testing the "core" modules, moreover,
+this is also something for you to run manually (do that if you touch "core"):
+
+```bash
+# test the core modules
+poetry run pytest tests/core
 
 # do not drop collections:
 TEST_SKIP_COLLECTION_DELETE=1 poetry run pytest [...]
 
-# include astrapy.core.ops testing (must cleanup after that):
+# include astrapy.core.ops testing (tester must clean up after that):
 TEST_ASTRADBOPS=1 poetry run pytest [...]
 ```
 
 ## Appendices
 
 ### Appendix A: quick reference for imports
```

