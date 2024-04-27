# Comparing `tmp/que_sdk-0.1.2.tar.gz` & `tmp/que_sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "que_sdk-0.1.2.tar", max compression
+gzip compressed data, was "que_sdk-0.1.3.tar", max compression
```

## Comparing `que_sdk-0.1.2.tar` & `que_sdk-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1060 2024-04-12 14:53:33.472804 que_sdk-0.1.2/LICENSE
--rw-r--r--   0        0        0       10 2024-04-19 17:17:10.806057 que_sdk-0.1.2/README.md
--rw-r--r--   0        0        0     1130 2024-04-23 09:03:40.690601 que_sdk-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      435 2024-04-20 08:19:42.640114 que_sdk-0.1.2/que_sdk/__init__.py
--rw-r--r--   0        0        0       65 2024-04-18 19:15:55.848369 que_sdk-0.1.2/que_sdk/_internal/__init__.py
--rw-r--r--   0        0        0      367 2024-04-13 18:33:05.063314 que_sdk-0.1.2/que_sdk/_internal/auth.py
--rw-r--r--   0        0        0     2257 2024-04-19 18:42:30.920224 que_sdk-0.1.2/que_sdk/_internal/base.py
--rw-r--r--   0        0        0     6339 2024-04-20 08:19:42.654293 que_sdk-0.1.2/que_sdk/client.py
--rw-r--r--   0        0        0     5564 2024-04-23 09:01:58.852361 que_sdk-0.1.2/que_sdk/clients.py
--rw-r--r--   0        0        0        0 2024-04-12 19:15:10.383938 que_sdk-0.1.2/que_sdk/py.typed.py
--rw-r--r--   0        0        0     1008 2024-04-23 08:59:04.018042 que_sdk-0.1.2/que_sdk/schemas.py
--rw-r--r--   0        0        0      329 2024-04-19 17:19:02.229326 que_sdk-0.1.2/que_sdk/types.py
--rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 que_sdk-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-04-12 14:53:33.472804 que_sdk-0.1.3/LICENSE
+-rw-r--r--   0        0        0       10 2024-04-19 17:17:10.806057 que_sdk-0.1.3/README.md
+-rw-r--r--   0        0        0     1130 2024-04-27 21:02:31.215152 que_sdk-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      435 2024-04-20 08:19:42.640114 que_sdk-0.1.3/que_sdk/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-18 19:15:55.848369 que_sdk-0.1.3/que_sdk/_internal/__init__.py
+-rw-r--r--   0        0        0      367 2024-04-13 18:33:05.063314 que_sdk-0.1.3/que_sdk/_internal/auth.py
+-rw-r--r--   0        0        0     2257 2024-04-19 18:42:30.920224 que_sdk-0.1.3/que_sdk/_internal/base.py
+-rw-r--r--   0        0        0     6339 2024-04-20 08:19:42.654293 que_sdk-0.1.3/que_sdk/client.py
+-rw-r--r--   0        0        0     5575 2024-04-27 21:02:10.142041 que_sdk-0.1.3/que_sdk/clients.py
+-rw-r--r--   0        0        0        0 2024-04-12 19:15:10.383938 que_sdk-0.1.3/que_sdk/py.typed.py
+-rw-r--r--   0        0        0     1008 2024-04-23 08:59:04.018042 que_sdk-0.1.3/que_sdk/schemas.py
+-rw-r--r--   0        0        0      329 2024-04-19 17:19:02.229326 que_sdk-0.1.3/que_sdk/types.py
+-rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 que_sdk-0.1.3/PKG-INFO
```

### Comparing `que_sdk-0.1.2/LICENSE` & `que_sdk-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `que_sdk-0.1.2/pyproject.toml` & `que_sdk-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "que_sdk"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["DavidRomanovizc"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `que_sdk-0.1.2/que_sdk/_internal/base.py` & `que_sdk-0.1.3/que_sdk/_internal/base.py`

 * *Files identical despite different names*

### Comparing `que_sdk-0.1.2/que_sdk/client.py` & `que_sdk-0.1.3/que_sdk/client.py`

 * *Files identical despite different names*

### Comparing `que_sdk-0.1.2/que_sdk/clients.py` & `que_sdk-0.1.3/que_sdk/clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     async def reactivate_user(self, access_token: str) -> http.HTTPStatus:
         """
         Reactivate the current user.
 
         :param access_token: access token
         :return: status code
         """
-        url = f"{self._base_url}/users/me/"
+        url = f"{self._base_url}/users/me/reactivate/"
         status_code, _ = await self._make_request(
             method="POST",
             url=url,
             access_token=access_token,
         )
         return http.HTTPStatus(status_code)
```

### Comparing `que_sdk-0.1.2/que_sdk/schemas.py` & `que_sdk-0.1.3/que_sdk/schemas.py`

 * *Files identical despite different names*

