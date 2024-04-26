# Comparing `tmp/datasette_secrets-0.1a4.tar.gz` & `tmp/datasette_secrets-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette_secrets-0.1a4.tar", last modified: Thu Apr 25 02:24:21 2024, max compression
+gzip compressed data, was "datasette_secrets-0.2.tar", last modified: Fri Apr 26 23:22:09 2024, max compression
```

## Comparing `datasette_secrets-0.1a4.tar` & `datasette_secrets-0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:24:21.086045 datasette_secrets-0.1a4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 02:24:14.000000 datasette_secrets-0.1a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-25 02:24:21.086045 datasette_secrets-0.1a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-25 02:24:14.000000 datasette_secrets-0.1a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:24:21.082045 datasette_secrets-0.1a4/datasette_secrets/
--rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-04-25 02:24:14.000000 datasette_secrets-0.1a4/datasette_secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-25 02:24:14.000000 datasette_secrets-0.1a4/datasette_secrets/hookspecs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:24:21.086045 datasette_secrets-0.1a4/datasette_secrets/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-25 02:24:14.000000 datasette_secrets-0.1a4/datasette_secrets/templates/secrets_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-25 02:24:14.000000 datasette_secrets-0.1a4/datasette_secrets/templates/secrets_update.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:24:21.086045 datasette_secrets-0.1a4/datasette_secrets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-25 02:24:21.000000 datasette_secrets-0.1a4/datasette_secrets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-25 02:24:21.000000 datasette_secrets-0.1a4/datasette_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 02:24:21.000000 datasette_secrets-0.1a4/datasette_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-25 02:24:21.000000 datasette_secrets-0.1a4/datasette_secrets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-25 02:24:21.000000 datasette_secrets-0.1a4/datasette_secrets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 02:24:21.000000 datasette_secrets-0.1a4/datasette_secrets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-25 02:24:14.000000 datasette_secrets-0.1a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 02:24:21.086045 datasette_secrets-0.1a4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:24:21.086045 datasette_secrets-0.1a4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-04-25 02:24:14.000000 datasette_secrets-0.1a4/tests/test_secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:22:09.203534 datasette_secrets-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 23:21:57.000000 datasette_secrets-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-26 23:22:09.203534 datasette_secrets-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-26 23:21:57.000000 datasette_secrets-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:22:09.199535 datasette_secrets-0.2/datasette_secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)    10853 2024-04-26 23:21:57.000000 datasette_secrets-0.2/datasette_secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-26 23:21:57.000000 datasette_secrets-0.2/datasette_secrets/hookspecs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:22:09.199535 datasette_secrets-0.2/datasette_secrets/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-26 23:21:57.000000 datasette_secrets-0.2/datasette_secrets/templates/secrets_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-26 23:21:57.000000 datasette_secrets-0.2/datasette_secrets/templates/secrets_update.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:22:09.203534 datasette_secrets-0.2/datasette_secrets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-26 23:22:09.000000 datasette_secrets-0.2/datasette_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-26 23:22:09.000000 datasette_secrets-0.2/datasette_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 23:22:09.000000 datasette_secrets-0.2/datasette_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-26 23:22:09.000000 datasette_secrets-0.2/datasette_secrets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-26 23:22:09.000000 datasette_secrets-0.2/datasette_secrets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 23:22:09.000000 datasette_secrets-0.2/datasette_secrets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-26 23:21:57.000000 datasette_secrets-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 23:22:09.203534 datasette_secrets-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:22:09.199535 datasette_secrets-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10945 2024-04-26 23:21:57.000000 datasette_secrets-0.2/tests/test_secrets.py
```

### Comparing `datasette_secrets-0.1a4/LICENSE` & `datasette_secrets-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette_secrets-0.1a4/PKG-INFO` & `datasette_secrets-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: datasette-secrets
-Version: 0.1a4
+Version: 0.2
 Summary: Manage secrets such as API keys for use with other Datasette plugins
 Author: Datasette
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-secrets
 Project-URL: Changelog, https://github.com/datasette/datasette-secrets/releases
 Project-URL: Issues, https://github.com/datasette/datasette-secrets/issues
 Project-URL: CI, https://github.com/datasette/datasette-secrets/actions
 Classifier: Framework :: Datasette
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: datasette>=1.0a13
+Requires-Dist: datasette
 Requires-Dist: cryptography
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
+Requires-Dist: datasette-test>=0.3.2; extra == "test"
 
 # datasette-secrets
 
 [![PyPI](https://img.shields.io/pypi/v/datasette-secrets.svg)](https://pypi.org/project/datasette-secrets/)
 [![Changelog](https://img.shields.io/github/v/release/datasette/datasette-secrets?include_prereleases&label=changelog)](https://github.com/datasette/datasette-secrets/releases)
 [![Tests](https://github.com/datasette/datasette-secrets/actions/workflows/test.yml/badge.svg)](https://github.com/datasette/datasette-secrets/actions/workflows/test.yml)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/datasette/datasette-secrets/blob/main/LICENSE)
```

### Comparing `datasette_secrets-0.1a4/README.md` & `datasette_secrets-0.2/README.md`

 * *Files identical despite different names*

### Comparing `datasette_secrets-0.1a4/datasette_secrets/__init__.py` & `datasette_secrets-0.2/datasette_secrets/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import click
 from cryptography.fernet import Fernet
 import dataclasses
-from datasette import hookimpl, Forbidden, Permission, Response
+from datasette import hookimpl, Forbidden, Response
 from datasette.plugins import pm
 from datasette.utils import await_me_maybe, sqlite3
 import os
 from typing import Optional
 from . import hookspecs
 
 MAX_NOTE_LENGTH = 100
@@ -85,15 +85,15 @@
 );
 """
 
 
 def get_database(datasette):
     plugin_config = datasette.plugin_config("datasette-secrets") or {}
     database = plugin_config.get("database") or "_internal"
-    if database == "_internal":
+    if database == "_internal" and hasattr(datasette, "get_internal_database"):
         return datasette.get_internal_database()
     return datasette.get_database(database)
 
 
 def get_config(datasette):
     plugin_config = datasette.plugin_config("datasette-secrets") or {}
     encryption_key = plugin_config.get("encryption-key")
@@ -104,14 +104,16 @@
         "database": database,
         "encryption_key": encryption_key,
     }
 
 
 @hookimpl
 def register_permissions(datasette):
+    from datasette import Permission
+
     return [
         Permission(
             name="manage-secrets",
             abbr=None,
             description="Manage Datasette secrets",
             takes_database=False,
             takes_resource=False,
@@ -183,23 +185,30 @@
         """.format(
             ", ".join("?" for _ in environment_secrets_names)
         ),
         list(environment_secrets_names),
     )
     existing_secrets = {row["name"]: dict(row) for row in existing_secrets_result.rows}
     # Try to turn updated_by into actors
-    actors = await datasette.actors_from_ids(
-        {row["updated_by"] for row in existing_secrets.values() if row["updated_by"]}
-    )
-    for secret in existing_secrets.values():
-        if secret["updated_by"]:
-            actor = actors.get(secret["updated_by"])
-            if actor:
-                display = actor.get("username") or actor.get("name") or actor.get("id")
-                secret["updated_by"] = display
+    if hasattr(datasette, "actors_from_ids"):
+        actors = await datasette.actors_from_ids(
+            {
+                row["updated_by"]
+                for row in existing_secrets.values()
+                if row["updated_by"]
+            }
+        )
+        for secret in existing_secrets.values():
+            if secret["updated_by"]:
+                actor = actors.get(secret["updated_by"])
+                if actor:
+                    display = (
+                        actor.get("username") or actor.get("name") or actor.get("id")
+                    )
+                    secret["updated_by"] = display
     unset_secrets = [
         secret
         for secret in all_secrets
         if secret.name not in existing_secrets
         and secret.name not in environment_secrets_names
     ]
     return Response.html(
```

### Comparing `datasette_secrets-0.1a4/datasette_secrets/templates/secrets_index.html` & `datasette_secrets-0.2/datasette_secrets/templates/secrets_index.html`

 * *Files identical despite different names*

### Comparing `datasette_secrets-0.1a4/datasette_secrets/templates/secrets_update.html` & `datasette_secrets-0.2/datasette_secrets/templates/secrets_update.html`

 * *Files identical despite different names*

### Comparing `datasette_secrets-0.1a4/datasette_secrets.egg-info/PKG-INFO` & `datasette_secrets-0.2/datasette_secrets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: datasette-secrets
-Version: 0.1a4
+Version: 0.2
 Summary: Manage secrets such as API keys for use with other Datasette plugins
 Author: Datasette
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-secrets
 Project-URL: Changelog, https://github.com/datasette/datasette-secrets/releases
 Project-URL: Issues, https://github.com/datasette/datasette-secrets/issues
 Project-URL: CI, https://github.com/datasette/datasette-secrets/actions
 Classifier: Framework :: Datasette
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: datasette>=1.0a13
+Requires-Dist: datasette
 Requires-Dist: cryptography
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
+Requires-Dist: datasette-test>=0.3.2; extra == "test"
 
 # datasette-secrets
 
 [![PyPI](https://img.shields.io/pypi/v/datasette-secrets.svg)](https://pypi.org/project/datasette-secrets/)
 [![Changelog](https://img.shields.io/github/v/release/datasette/datasette-secrets?include_prereleases&label=changelog)](https://github.com/datasette/datasette-secrets/releases)
 [![Tests](https://github.com/datasette/datasette-secrets/actions/workflows/test.yml/badge.svg)](https://github.com/datasette/datasette-secrets/actions/workflows/test.yml)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/datasette/datasette-secrets/blob/main/LICENSE)
```

### Comparing `datasette_secrets-0.1a4/pyproject.toml` & `datasette_secrets-0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [project]
 name = "datasette-secrets"
-version = "0.1a4"
+version = "0.2"
 description = "Manage secrets such as API keys for use with other Datasette plugins"
 readme = "README.md"
 authors = [{name = "Datasette"}]
 license = {text = "Apache-2.0"}
 classifiers=[
     "Framework :: Datasette",
     "License :: OSI Approved :: Apache Software License"
 ]
 requires-python = ">=3.8"
 dependencies = [
-    "datasette>=1.0a13",
+    "datasette",
     "cryptography"
 ]
 
 [project.urls]
 Homepage = "https://github.com/datasette/datasette-secrets"
 Changelog = "https://github.com/datasette/datasette-secrets/releases"
 Issues = "https://github.com/datasette/datasette-secrets/issues"
 CI = "https://github.com/datasette/datasette-secrets/actions"
 
 [project.entry-points.datasette]
 secrets = "datasette_secrets"
 
 [project.optional-dependencies]
-test = ["pytest", "pytest-asyncio"]
+test = ["pytest", "pytest-asyncio", "datasette-test>=0.3.2"]
 
 [tool.pytest.ini_options]
 asyncio_mode = "strict"
 
 [tool.setuptools.package-data]
 datasette_secrets = ["templates/*"]
```

### Comparing `datasette_secrets-0.1a4/tests/test_secrets.py` & `datasette_secrets-0.2/tests/test_secrets.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from click.testing import CliRunner
 from cryptography.fernet import Fernet
 from datasette import hookimpl
-from datasette.app import Datasette
 from datasette.cli import cli
 from datasette.plugins import pm
+from datasette_test import Datasette, actor_cookie
 from datasette_secrets import get_secret, Secret, startup, get_config
 import pytest
 from unittest.mock import ANY
 
 TEST_ENCRYPTION_KEY = "-LujHtwFWGaBpznrV1zduoZBmCnMOW7J0H5hmeXgAVo="
 
 
+def get_internal_database(ds):
+    if hasattr(ds, "get_internal_database"):
+        return ds.get_internal_database()
+    else:
+        return ds.get_database("_internal")
+
+
 def test_generate_command():
     runner = CliRunner()
     result = runner.invoke(cli, ["secrets", "generate-encryption-key"])
     assert result.exit_code == 0
     key = result.output.strip()
     key_bytes = key.encode("utf-8")
     # This will throw an exception if key is invalid:
@@ -85,23 +92,21 @@
     pm.unregister(name="SecretOnePlugin")
     pm.unregister(name="SecretTwoPlugin")
 
 
 @pytest.fixture
 def ds():
     return Datasette(
-        config={
-            "plugins": {
-                "datasette-secrets": {
-                    "database": "_internal",
-                    "encryption-key": TEST_ENCRYPTION_KEY,
-                }
-            },
-            "permissions": {"manage-secrets": {"id": "admin"}},
-        }
+        plugin_config={
+            "datasette-secrets": {
+                "database": "_internal",
+                "encryption-key": TEST_ENCRYPTION_KEY,
+            }
+        },
+        permissions={"manage-secrets": {"id": "admin"}},
     )
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     "path,verb,data",
     (
@@ -111,15 +116,15 @@
 )
 @pytest.mark.parametrize("user", (None, "admin", "other"))
 async def test_permissions(ds, path, verb, data, user):
     method = ds.client.get if verb == "GET" else ds.client.post
     kwargs = {}
     if user:
         kwargs["cookies"] = {
-            "ds_actor": ds.client.actor_cookie({"id": user}),
+            "ds_actor": actor_cookie(ds, {"id": user}),
         }
     if data:
         kwargs["data"] = data
     response = await method(path, **kwargs)
     if user == "admin":
         assert response.status_code != 403
         # And check they have the menu item too
@@ -127,26 +132,26 @@
     else:
         assert response.status_code == 403
         assert '<a href="/-/secrets">Manage secrets</a>' not in response.text
 
 
 @pytest.mark.asyncio
 async def test_set_secret(ds, use_actors_plugin):
-    cookies = {"ds_actor": ds.client.actor_cookie({"id": "admin"})}
+    cookies = {"ds_actor": actor_cookie(ds, {"id": "admin"})}
     get_response = await ds.client.get("/-/secrets/EXAMPLE_SECRET", cookies=cookies)
     csrftoken = get_response.cookies["ds_csrftoken"]
     cookies["ds_csrftoken"] = csrftoken
     post_response = await ds.client.post(
         "/-/secrets/EXAMPLE_SECRET",
         cookies=cookies,
         data={"secret": "new-secret-value", "note": "new-note", "csrftoken": csrftoken},
     )
     assert post_response.status_code == 302
     assert post_response.headers["Location"] == "/-/secrets"
-    internal_db = ds.get_internal_database()
+    internal_db = get_internal_database(ds)
     secrets = await internal_db.execute("select * from datasette_secrets")
     rows = [dict(r) for r in secrets.rows]
     assert rows == [
         {
             "id": 1,
             "name": "EXAMPLE_SECRET",
             "note": "new-note",
@@ -170,15 +175,20 @@
     assert decrypted == b"new-secret-value"
 
     # Check that the listing is as expected, including showing the actor username
     response = await ds.client.get("/-/secrets", cookies=cookies)
     assert response.status_code == 200
     assert "EXAMPLE_SECRET" in response.text
     assert "new-note" in response.text
-    assert "<td>ADMIN</td>" in response.text
+
+    if hasattr(ds, "actors_from_ids"):
+        assert "<td>ADMIN</td>" in response.text
+    else:
+        # Pre 1.0, so can't use that mechanism
+        assert "<td>admin</td>" in response.text
 
     # Now let's edit it
     post_response2 = await ds.client.post(
         "/-/secrets/EXAMPLE_SECRET",
         cookies=cookies,
         data={"secret": "updated-secret-value", "note": "", "csrftoken": csrftoken},
     )
@@ -209,19 +219,19 @@
         "last_used_by": None,
     }
 
 
 @pytest.mark.asyncio
 async def test_get_secret(ds, monkeypatch):
     # First set it manually
-    cookies = {"ds_actor": ds.client.actor_cookie({"id": "admin"})}
+    cookies = {"ds_actor": actor_cookie(ds, {"id": "admin"})}
     get_response = await ds.client.get("/-/secrets/EXAMPLE_SECRET", cookies=cookies)
     csrftoken = get_response.cookies["ds_csrftoken"]
     cookies["ds_csrftoken"] = csrftoken
-    db = ds.get_internal_database()
+    db = get_internal_database(ds)
     # Reset state
     await db.execute_write(
         "update datasette_secrets set last_used_at = null, last_used_by = null"
     )
     post_response = await ds.client.post(
         "/-/secrets/EXAMPLE_SECRET",
         cookies=cookies,
@@ -284,15 +294,15 @@
 
 
 @pytest.mark.asyncio
 async def test_secret_index_page(ds, register_multiple_secrets):
     response = await ds.client.get(
         "/-/secrets",
         cookies={
-            "ds_actor": ds.client.actor_cookie({"id": "admin"}),
+            "ds_actor": actor_cookie(ds, {"id": "admin"}),
         },
     )
     assert response.status_code == 200
     expected_html = """
     <p style="margin-top: 2em">The following secrets have not been set:</p>
     <ul>
         <li><strong><a href="/-/secrets/OPENAI_API_KEY">OPENAI_API_KEY</a></strong>
```

