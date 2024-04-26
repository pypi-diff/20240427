# Comparing `tmp/datasette_test-0.3.1.tar.gz` & `tmp/datasette_test-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette_test-0.3.1.tar", last modified: Fri Apr 26 18:55:55 2024, max compression
+gzip compressed data, was "datasette_test-0.3.2.tar", last modified: Fri Apr 26 23:13:30 2024, max compression
```

## Comparing `datasette_test-0.3.1.tar` & `datasette_test-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:55:55.301807 datasette_test-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 18:55:49.000000 datasette_test-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-26 18:55:55.301807 datasette_test-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-26 18:55:49.000000 datasette_test-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:55:55.297807 datasette_test-0.3.1/datasette_test/
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-26 18:55:49.000000 datasette_test-0.3.1/datasette_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:55:55.301807 datasette_test-0.3.1/datasette_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-26 18:55:55.000000 datasette_test-0.3.1/datasette_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-26 18:55:55.000000 datasette_test-0.3.1/datasette_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 18:55:55.000000 datasette_test-0.3.1/datasette_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-26 18:55:55.000000 datasette_test-0.3.1/datasette_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 18:55:55.000000 datasette_test-0.3.1/datasette_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-26 18:55:49.000000 datasette_test-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 18:55:55.301807 datasette_test-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:55:55.301807 datasette_test-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-26 18:55:49.000000 datasette_test-0.3.1/tests/test_datasette_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:13:30.452250 datasette_test-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 23:13:23.000000 datasette_test-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-26 23:13:30.452250 datasette_test-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-26 23:13:23.000000 datasette_test-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:13:30.448250 datasette_test-0.3.2/datasette_test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-26 23:13:23.000000 datasette_test-0.3.2/datasette_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:13:30.452250 datasette_test-0.3.2/datasette_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-26 23:13:30.000000 datasette_test-0.3.2/datasette_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-26 23:13:30.000000 datasette_test-0.3.2/datasette_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 23:13:30.000000 datasette_test-0.3.2/datasette_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-26 23:13:30.000000 datasette_test-0.3.2/datasette_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 23:13:30.000000 datasette_test-0.3.2/datasette_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-26 23:13:23.000000 datasette_test-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 23:13:30.452250 datasette_test-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:13:30.448250 datasette_test-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-26 23:13:23.000000 datasette_test-0.3.2/tests/test_datasette_test.py
```

### Comparing `datasette_test-0.3.1/LICENSE` & `datasette_test-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette_test-0.3.1/PKG-INFO` & `datasette_test-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-test
-Version: 0.3.1
+Version: 0.3.2
 Summary: Utilities to help write tests for Datasette plugins and applications
 Author: Datasette
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-test
 Project-URL: Changelog, https://github.com/datasette/datasette-test/releases
 Project-URL: Issues, https://github.com/datasette/datasette-test/issues
 Project-URL: CI, https://github.com/datasette/datasette-test/actions
```

### Comparing `datasette_test-0.3.1/README.md` & `datasette_test-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `datasette_test-0.3.1/datasette_test/__init__.py` & `datasette_test-0.3.2/datasette_test/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,10 +50,10 @@
         except httpx.ConnectError:
             time.sleep(0.1)
     raise AssertionError("Timed out waiting for {} to respond".format(url))
 
 
 def actor_cookie(datasette, actor):
     if hasattr(datasette.client, "actor_cookie"):
-        return datasette.client.actor_cookie({"id": "root"})
+        return datasette.client.actor_cookie(actor)
     else:
         return datasette.sign({"a": actor}, "actor")
```

### Comparing `datasette_test-0.3.1/datasette_test.egg-info/PKG-INFO` & `datasette_test-0.3.2/datasette_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-test
-Version: 0.3.1
+Version: 0.3.2
 Summary: Utilities to help write tests for Datasette plugins and applications
 Author: Datasette
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-test
 Project-URL: Changelog, https://github.com/datasette/datasette-test/releases
 Project-URL: Issues, https://github.com/datasette/datasette-test/issues
 Project-URL: CI, https://github.com/datasette/datasette-test/actions
```

### Comparing `datasette_test-0.3.1/pyproject.toml` & `datasette_test-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "datasette-test"
-version = "0.3.1"
+version = "0.3.2"
 description = "Utilities to help write tests for Datasette plugins and applications"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [{name = "Datasette"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
```

### Comparing `datasette_test-0.3.1/tests/test_datasette_test.py` & `datasette_test-0.3.2/tests/test_datasette_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -42,7 +42,16 @@
     ds = Datasette(permissions={"view-instance": {"id": "root"}})
     response = await ds.client.get("/")
     assert response.status_code == 403
     response = await ds.client.get(
         "/", cookies={"ds_actor": actor_cookie(ds, {"id": "root"})}
     )
     assert response.status_code == 200
+
+
+@pytest.mark.asyncio
+@pytest.mark.parametrize("actor_id", ("root", "admin"))
+async def test_actor_cookie(actor_id):
+    ds = Datasette()
+    cookie = actor_cookie(ds, {"id": actor_id})
+    decoded = ds.unsign(cookie, "actor")
+    assert decoded == {"a": {"id": actor_id}}
```

