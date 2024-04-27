# Comparing `tmp/django_graphql_jwt_oauth2-1.2.2.tar.gz` & `tmp/django_graphql_jwt_oauth2-1.2.3.tar.gz`

## Comparing `django_graphql_jwt_oauth2-1.2.2.tar` & `django_graphql_jwt_oauth2-1.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.2/graphql_jwt_oauth2/__init__.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.2/graphql_jwt_oauth2/constants.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.2/graphql_jwt_oauth2/decorators.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.2/graphql_jwt_oauth2/errors.py
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.2/graphql_jwt_oauth2/provider.py
--rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.2/graphql_jwt_oauth2/queries.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.2/graphql_jwt_oauth2/state_manager.py
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.2/graphql_jwt_oauth2/utils.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.2/graphql_jwt_oauth2/django_graphql_jwt_oauth2.egg-info/PKG-INFO
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.2/graphql_jwt_oauth2/django_graphql_jwt_oauth2.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.2/graphql_jwt_oauth2/django_graphql_jwt_oauth2.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.2/graphql_jwt_oauth2/django_graphql_jwt_oauth2.egg-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.2/graphql_jwt_oauth2/providers/__init__.py
--rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.2/graphql_jwt_oauth2/providers/google.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.2/.gitignore
--rw-r--r--   0        0        0    17098 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.2/LICENSE
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.2/README.md
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.2/pyproject.toml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.3/graphql_jwt_oauth2/__init__.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.3/graphql_jwt_oauth2/constants.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.3/graphql_jwt_oauth2/decorators.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.3/graphql_jwt_oauth2/errors.py
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.3/graphql_jwt_oauth2/provider.py
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.3/graphql_jwt_oauth2/queries.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.3/graphql_jwt_oauth2/state_manager.py
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.3/graphql_jwt_oauth2/utils.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.3/graphql_jwt_oauth2/django_graphql_jwt_oauth2.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.3/graphql_jwt_oauth2/django_graphql_jwt_oauth2.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.3/graphql_jwt_oauth2/django_graphql_jwt_oauth2.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.3/graphql_jwt_oauth2/django_graphql_jwt_oauth2.egg-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.3/graphql_jwt_oauth2/providers/__init__.py
+-rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.3/graphql_jwt_oauth2/providers/google.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.3/.gitignore
+-rw-r--r--   0        0        0    17098 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.3/LICENSE
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.3/README.md
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 django_graphql_jwt_oauth2-1.2.3/PKG-INFO
```

### Comparing `django_graphql_jwt_oauth2-1.2.2/graphql_jwt_oauth2/constants.py` & `django_graphql_jwt_oauth2-1.2.3/graphql_jwt_oauth2/constants.py`

 * *Files identical despite different names*

### Comparing `django_graphql_jwt_oauth2-1.2.2/graphql_jwt_oauth2/decorators.py` & `django_graphql_jwt_oauth2-1.2.3/graphql_jwt_oauth2/decorators.py`

 * *Files identical despite different names*

### Comparing `django_graphql_jwt_oauth2-1.2.2/graphql_jwt_oauth2/errors.py` & `django_graphql_jwt_oauth2-1.2.3/graphql_jwt_oauth2/errors.py`

 * *Files identical despite different names*

### Comparing `django_graphql_jwt_oauth2-1.2.2/graphql_jwt_oauth2/provider.py` & `django_graphql_jwt_oauth2-1.2.3/graphql_jwt_oauth2/provider.py`

 * *Files identical despite different names*

### Comparing `django_graphql_jwt_oauth2-1.2.2/graphql_jwt_oauth2/queries.py` & `django_graphql_jwt_oauth2-1.2.3/graphql_jwt_oauth2/queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
                 Resolver for generating OAuth2 login links.
 
                 :param self: Instance of the class
                 :param info: GraphQL query information
                 :param kwargs: Keyword arguments
                 :return: Authorization URL for the OAuth2 provider
                 """
-                print("being called")
                 state_payload = {"resource": parent.get("resource")}
                 additional_state_payload_json = parent.get("additional_state_payload")
                 if additional_state_payload_json:
                     additional_state_payload = json.loads(additional_state_payload_json)
                     state_payload.update(additional_state_payload)
 
                 encoded_state = OAuth2StateManager(payload=state_payload).encoded_state
```

### Comparing `django_graphql_jwt_oauth2-1.2.2/graphql_jwt_oauth2/state_manager.py` & `django_graphql_jwt_oauth2-1.2.3/graphql_jwt_oauth2/state_manager.py`

 * *Files identical despite different names*

### Comparing `django_graphql_jwt_oauth2-1.2.2/graphql_jwt_oauth2/utils.py` & `django_graphql_jwt_oauth2-1.2.3/graphql_jwt_oauth2/utils.py`

 * *Files identical despite different names*

### Comparing `django_graphql_jwt_oauth2-1.2.2/graphql_jwt_oauth2/django_graphql_jwt_oauth2.egg-info/PKG-INFO` & `django_graphql_jwt_oauth2-1.2.3/graphql_jwt_oauth2/django_graphql_jwt_oauth2.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `django_graphql_jwt_oauth2-1.2.2/graphql_jwt_oauth2/providers/google.py` & `django_graphql_jwt_oauth2-1.2.3/graphql_jwt_oauth2/providers/google.py`

 * *Files identical despite different names*

### Comparing `django_graphql_jwt_oauth2-1.2.2/LICENSE` & `django_graphql_jwt_oauth2-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_graphql_jwt_oauth2-1.2.2/pyproject.toml` & `django_graphql_jwt_oauth2-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-graphql-jwt-oauth2"
-version = "1.2.2"
+version = "1.2.3"
 #authors = [
 #  { name="Example Author", email="author@example.com" },
 #]
 description = "An extension to django-graphene-jwt to allow oauth2 authentication to a Django app."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `django_graphql_jwt_oauth2-1.2.2/PKG-INFO` & `django_graphql_jwt_oauth2-1.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-graphql-jwt-oauth2
-Version: 1.2.2
+Version: 1.2.3
 Summary: An extension to django-graphene-jwt to allow oauth2 authentication to a Django app.
 Project-URL: Homepage, https://github.com/AztlanEngineering/django-graphql-jwt-oauth2
 Project-URL: Issues, https://github.com/AztlanEngineering/django-graphql-jwt-oauth2/issues
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -15,7 +15,8 @@
 - Make sure Sphinx generates docs from all files
 - generate html instead of md ???
 - add general introduction and usage guide on the docs
 
 Build
 `hatch build` or `python -m hatch build`
 `hatch publish` or `python -m hatch publish` with username `__token__`. Make sure the [keyrings backend](https://github.com/jaraco/keyrings.alt) is installed. 
+On arch `pacman -S python-hatch python-keyrings-alt`, publish with `username:__token__`
```

