# Comparing `tmp/aiosalesforce-0.5.7.tar.gz` & `tmp/aiosalesforce-0.6.0.tar.gz`

## Comparing `aiosalesforce-0.5.7.tar` & `aiosalesforce-0.6.0.tar`

### file list

```diff
@@ -1,27 +1,32 @@
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/src/aiosalesforce/__init__.py
--rw-r--r--   0        0        0     8674 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/src/aiosalesforce/client.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/src/aiosalesforce/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/src/aiosalesforce/py.typed
--rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/src/aiosalesforce/sobject.py
--rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/src/aiosalesforce/utils.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/src/aiosalesforce/auth/__init__.py
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/src/aiosalesforce/auth/base.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/src/aiosalesforce/auth/client_credentials_flow.py
--rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/src/aiosalesforce/auth/jwt_bearer_flow.py
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/src/aiosalesforce/auth/soap.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/src/aiosalesforce/bulk/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/src/aiosalesforce/bulk/v2/__init__.py
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/src/aiosalesforce/bulk/v2/_csv.py
--rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/src/aiosalesforce/bulk/v2/client.py
--rw-r--r--   0        0        0    13858 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/src/aiosalesforce/bulk/v2/ingest.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/src/aiosalesforce/events/__init__.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/src/aiosalesforce/events/event_bus.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/src/aiosalesforce/events/events.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/src/aiosalesforce/retries/__init__.py
--rw-r--r--   0        0        0     9272 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/src/aiosalesforce/retries/policy.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/src/aiosalesforce/retries/rules.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/LICENSE
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/README.md
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 aiosalesforce-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/__init__.py
+-rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/client.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/py.typed
+-rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/sobject.py
+-rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/utils.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/auth/__init__.py
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/auth/base.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/auth/client_credentials_flow.py
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/auth/jwt_bearer_flow.py
+-rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/auth/soap.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/bulk/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/bulk/v2/__init__.py
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/bulk/v2/_csv.py
+-rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/bulk/v2/client.py
+-rw-r--r--   0        0        0    13848 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/bulk/v2/ingest.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/composite/__init__.py
+-rw-r--r--   0        0        0    16130 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/composite/batch.py
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/composite/client.py
+-rw-r--r--   0        0        0    18342 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/composite/composite.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/composite/exceptions.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/events/__init__.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/events/event_bus.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/events/events.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/retries/__init__.py
+-rw-r--r--   0        0        0     9272 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/retries/policy.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/src/aiosalesforce/retries/rules.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/README.md
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 aiosalesforce-0.6.0/PKG-INFO
```

### Comparing `aiosalesforce-0.5.7/src/aiosalesforce/__init__.py` & `aiosalesforce-0.6.0/src/aiosalesforce/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.5.7"
+__version__ = "0.6.0"
 
 __all__ = [
     "ClientCredentialsFlow",
     "JwtBearerFlow",
     "SoapLogin",
     "Salesforce",
     "BulkApiBatchConsumptionEvent",
```

### Comparing `aiosalesforce-0.5.7/src/aiosalesforce/client.py` & `aiosalesforce-0.6.0/src/aiosalesforce/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Any, AsyncIterator, Awaitable, Callable, Iterable, NoReturn
 
 import httpx
 
 from aiosalesforce import __version__
 from aiosalesforce.auth import Auth
 from aiosalesforce.bulk import BulkClientV2
+from aiosalesforce.composite import CompositeClient
 from aiosalesforce.events import (
     Event,
     EventBus,
     RequestEvent,
     ResponseEvent,
 )
 from aiosalesforce.exceptions import SalesforceWarning, raise_salesforce_error
@@ -86,19 +87,19 @@
 
         self.event_bus = EventBus(event_hooks)
         self.retry_policy = retry_policy or RetryPolicy()
         self._semaphore = asyncio.Semaphore(concurrency_limit)
 
     @property
     def version(self) -> str:
+        """API version in the format '60.0'."""
         return self.__version
 
     @version.setter
     def version(self, value: str) -> None:
-        """API version in the format '60.0'."""
         if not (match_ := re.fullmatch(r"^(v)?(\d+)(\.(0)?)?$", value)):
             raise ValueError(
                 f"Invalid Salesforce API version: '{value}'. "
                 f"A valid version should look like '60.0'."
             )
         self.__version = f"{match_.groups()[1]}.0"
 
@@ -128,14 +129,16 @@
         self.__base_url = str(match_.groups()[0])
 
     @wraps(httpx.AsyncClient.request)
     async def request(self, *args, **kwargs) -> httpx.Response:
         """
         Make an HTTP request to Salesforce.
 
+        Raises an appropriate exception if the request is not successful.
+
         """
         request = self.httpx_client.build_request(*args, **kwargs)
         access_token = await self.auth.get_access_token(self)
         request.headers.update(
             {
                 "Authorization": f"Bearer {access_token}",
                 "User-Agent": f"aiosalesforce/{__version__}",
@@ -202,15 +205,15 @@
             SOQL query.
         include_all_records : bool, default False
             If True, includes all (active/deleted/archived) records.
 
         Yields
         -------
         dict
-            Query result record.
+            Record.
 
         """
         operation = "query" if not include_all_records else "queryAll"
 
         next_url: str | None = None
         while True:
             if next_url is None:
@@ -242,23 +245,37 @@
 
         """
         return SobjectClient(self)
 
     @cached_property
     def bulk_v1(self) -> NoReturn:
         """
-        Get Salesforce Bulk API 1.0 client.
+        Salesforce Bulk API 1.0 client.
 
         Use this client to execute bulk ingest and query operations.
 
         """
         raise NotImplementedError("Bulk API v1 is currently not supported")
 
     @cached_property
     def bulk_v2(self) -> BulkClientV2:
         """
-        Get Salesforce Bulk API 2.0 client.
+        Salesforce Bulk API 2.0 client.
 
         Use this client to execute bulk ingest and query operations.
 
         """
         return BulkClientV2(self)
+
+    @cached_property
+    def composite(self) -> CompositeClient:
+        """
+        Salesforce REST API composite client.
+
+        Use this client to perform composite operations:
+        * Composite Batch
+        * Composite
+        * Composite Graph
+        * sObject Tree
+
+        """
+        return CompositeClient(self)
```

### Comparing `aiosalesforce-0.5.7/src/aiosalesforce/exceptions.py` & `aiosalesforce-0.6.0/src/aiosalesforce/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.7/src/aiosalesforce/sobject.py` & `aiosalesforce-0.6.0/src/aiosalesforce/sobject.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
 
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Iterable
 
+import httpx
+
 from aiosalesforce.utils import json_dumps, json_loads
 
 if TYPE_CHECKING:
     from .client import Salesforce
 
 logger = logging.getLogger(__name__)
 
@@ -32,15 +34,15 @@
     base_url: str
     """Base URL in the format https://[subdomain(s)].my.salesforce.com/services/data/v[version]/sobjects"""
 
     def __init__(self, salesforce_client: "Salesforce") -> None:
         self.salesforce_client = salesforce_client
         self.base_url = "/".join(
             [
-                f"{self.salesforce_client.base_url}",
+                self.salesforce_client.base_url,
                 "services",
                 "data",
                 f"v{self.salesforce_client.version}",
                 "sobjects",
             ]
         )
 
@@ -99,30 +101,31 @@
         fields : Iterable[str], optional
             Fields to get for the record.
             By default returns all fields.
 
         Returns
         -------
         dict
-            _description_
-        """
-        url = f"{self.base_url}/{sobject}"
-        if external_id_field is None:
-            url += f"/{id_}"
-        else:
-            url += f"/{external_id_field}/{id_}"
+            sObject data.
 
-        params: dict = {}
+        """
+        url = httpx.URL(
+            "/".join(
+                [
+                    self.base_url,
+                    sobject,
+                    id_ if external_id_field is None else f"{external_id_field}/{id_}",
+                ]
+            )
+        )
         if fields is not None:
-            params["fields"] = ",".join(fields)
-
+            url = url.copy_add_param("fields", ",".join(fields))
         response = await self.salesforce_client.request(
             "GET",
             url,
-            params=params,
             headers={"Accept": "application/json"},
         )
         return json_loads(response.content)
 
     async def update(
         self,
         sobject: str,
@@ -170,20 +173,24 @@
         id_ : str
             Salesforce record ID or external ID (if external_id_field is provided).
         external_id_field : str, optional
             External ID field name.
             If not provided, id_ is treated as a record ID.
 
         """
-        url = f"{self.base_url}/{sobject}"
-        if external_id_field is None:
-            url += f"/{id_}"
-        else:
-            url += f"/{external_id_field}/{id_}"
-        await self.salesforce_client.request("DELETE", url)
+        await self.salesforce_client.request(
+            "DELETE",
+            "/".join(
+                [
+                    self.base_url,
+                    sobject,
+                    id_ if external_id_field is None else f"{external_id_field}/{id_}",
+                ]
+            ),
+        )
 
     async def upsert(
         self,
         sobject: str,
         id_: str,
         /,
         external_id_field: str,
```

### Comparing `aiosalesforce-0.5.7/src/aiosalesforce/utils.py` & `aiosalesforce-0.6.0/src/aiosalesforce/utils.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.7/src/aiosalesforce/auth/base.py` & `aiosalesforce-0.6.0/src/aiosalesforce/auth/base.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.7/src/aiosalesforce/auth/client_credentials_flow.py` & `aiosalesforce-0.6.0/src/aiosalesforce/auth/client_credentials_flow.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.7/src/aiosalesforce/auth/jwt_bearer_flow.py` & `aiosalesforce-0.6.0/src/aiosalesforce/auth/jwt_bearer_flow.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.7/src/aiosalesforce/auth/soap.py` & `aiosalesforce-0.6.0/src/aiosalesforce/auth/soap.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.7/src/aiosalesforce/bulk/v2/_csv.py` & `aiosalesforce-0.6.0/src/aiosalesforce/bulk/v2/_csv.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.7/src/aiosalesforce/bulk/v2/client.py` & `aiosalesforce-0.6.0/src/aiosalesforce/bulk/v2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     base_url: str
     """Base URL in the format https://[subdomain(s)].my.salesforce.com/services/data/v[version]/jobs"""
 
     def __init__(self, salesforce_client: "Salesforce") -> None:
         self.salesforce_client = salesforce_client
         self.base_url = "/".join(
             [
-                f"{self.salesforce_client.base_url}",
+                self.salesforce_client.base_url,
                 "services",
                 "data",
                 f"v{self.salesforce_client.version}",
                 "jobs",
             ]
         )
```

### Comparing `aiosalesforce-0.5.7/src/aiosalesforce/bulk/v2/ingest.py` & `aiosalesforce-0.6.0/src/aiosalesforce/bulk/v2/ingest.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
     bulk_client: "BulkClientV2"
     base_url: str
     """Base URL in the format https://[subdomain(s)].my.salesforce.com/services/data/v[version]/jobs/ingest"""
 
     def __init__(self, bulk_client: "BulkClientV2") -> None:
         self.bulk_client = bulk_client
-        self.base_url = "/".join([self.bulk_client.base_url, "ingest"])
+        self.base_url = f"{self.bulk_client.base_url}/ingest"
 
     async def create_job(
         self,
         operation: OperationType,
         sobject: str,
         external_id_field: str | None = None,
         assignment_rule_id: str | None = None,
```

### Comparing `aiosalesforce-0.5.7/src/aiosalesforce/events/event_bus.py` & `aiosalesforce-0.6.0/src/aiosalesforce/events/event_bus.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.7/src/aiosalesforce/events/events.py` & `aiosalesforce-0.6.0/src/aiosalesforce/events/events.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.7/src/aiosalesforce/retries/__init__.py` & `aiosalesforce-0.6.0/src/aiosalesforce/retries/__init__.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.7/src/aiosalesforce/retries/policy.py` & `aiosalesforce-0.6.0/src/aiosalesforce/retries/policy.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.7/src/aiosalesforce/retries/rules.py` & `aiosalesforce-0.6.0/src/aiosalesforce/retries/rules.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.7/LICENSE` & `aiosalesforce-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.7/README.md` & `aiosalesforce-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.7/pyproject.toml` & `aiosalesforce-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.7/PKG-INFO` & `aiosalesforce-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aiosalesforce
-Version: 0.5.7
+Version: 0.6.0
 Summary: Salesforce REST API client
 Project-URL: Homepage, https://github.com/georgebv/aiosalesforce
 Project-URL: Documentation, https://github.com/georgebv/aiosalesforce
 Project-URL: Repository, https://github.com/georgebv/aiosalesforce
 Author-email: Georgii Bocharov <bocharovgeorgii@gmail.com>
 License: Copyright 2024 Georgii Bocharov
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: aiosalesforce Version: 0.5.7 Summary: Salesforce
+Metadata-Version: 2.3 Name: aiosalesforce Version: 0.6.0 Summary: Salesforce
 REST API client Project-URL: Homepage, https://github.com/georgebv/
 aiosalesforce Project-URL: Documentation, https://github.com/georgebv/
 aiosalesforce Project-URL: Repository, https://github.com/georgebv/
 aiosalesforce Author-email: Georgii Bocharov
 gmail.com> License: Copyright 2024 Georgii Bocharov Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
```

