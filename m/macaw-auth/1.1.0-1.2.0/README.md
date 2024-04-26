# Comparing `tmp/macaw_auth-1.1.0.tar.gz` & `tmp/macaw_auth-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macaw_auth-1.1.0.tar", last modified: Fri Apr 19 03:45:28 2024, max compression
+gzip compressed data, was "macaw_auth-1.2.0.tar", last modified: Fri Apr 26 22:14:12 2024, max compression
```

## Comparing `macaw_auth-1.1.0.tar` & `macaw_auth-1.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:45:28.982154 macaw_auth-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-19 03:45:28.982154 macaw_auth-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:45:28.982154 macaw_auth-1.1.0/macaw_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-19 03:45:28.000000 macaw_auth-1.1.0/macaw_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-19 03:45:28.000000 macaw_auth-1.1.0/macaw_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 03:45:28.000000 macaw_auth-1.1.0/macaw_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-19 03:45:28.000000 macaw_auth-1.1.0/macaw_auth.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-19 03:45:28.000000 macaw_auth-1.1.0/macaw_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 03:45:28.000000 macaw_auth-1.1.0/macaw_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 03:45:28.982154 macaw_auth-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:45:28.978153 macaw_auth-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:45:28.978153 macaw_auth-1.1.0/src/macaw_auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:45:28.978153 macaw_auth-1.1.0/src/macaw_auth/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/classes/aws_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/classes/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/classes/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/classes/idp_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/classes/sts_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/classes/user_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/classes/username_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:45:28.978153 macaw_auth-1.1.0/src/macaw_auth/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:45:28.982154 macaw_auth-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/tests/test_usernames.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:14:12.561889 macaw_auth-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-26 22:14:12.561889 macaw_auth-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:14:12.561889 macaw_auth-1.2.0/macaw_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-26 22:14:12.000000 macaw_auth-1.2.0/macaw_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-26 22:14:12.000000 macaw_auth-1.2.0/macaw_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 22:14:12.000000 macaw_auth-1.2.0/macaw_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-26 22:14:12.000000 macaw_auth-1.2.0/macaw_auth.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 22:14:12.000000 macaw_auth-1.2.0/macaw_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 22:14:12.000000 macaw_auth-1.2.0/macaw_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 22:14:12.561889 macaw_auth-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:14:12.557889 macaw_auth-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:14:12.561889 macaw_auth-1.2.0/src/macaw_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:14:12.561889 macaw_auth-1.2.0/src/macaw_auth/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/classes/aws_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/classes/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/classes/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/classes/idp_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/classes/sts_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/classes/user_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/classes/username_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:14:12.561889 macaw_auth-1.2.0/src/macaw_auth/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:14:12.561889 macaw_auth-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/tests/test_usernames.py
```

### Comparing `macaw_auth-1.1.0/LICENSE` & `macaw_auth-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `macaw_auth-1.1.0/PKG-INFO` & `macaw_auth-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macaw-auth
-Version: 1.1.0
+Version: 1.2.0
 Summary: Tool to obtain AWS CLI credentials from ADFS.
 Author-email: Travis Samuel <tsamuel@alum.mit.edu>
 Project-URL: Homepage, https://github.com/tsamuel33/macaw-auth
 Project-URL: Bug Tracker, https://github.com/tsamuel33/macaw-auth/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `macaw_auth-1.1.0/README.md` & `macaw_auth-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `macaw_auth-1.1.0/macaw_auth.egg-info/PKG-INFO` & `macaw_auth-1.2.0/macaw_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macaw-auth
-Version: 1.1.0
+Version: 1.2.0
 Summary: Tool to obtain AWS CLI credentials from ADFS.
 Author-email: Travis Samuel <tsamuel@alum.mit.edu>
 Project-URL: Homepage, https://github.com/tsamuel33/macaw-auth
 Project-URL: Bug Tracker, https://github.com/tsamuel33/macaw-auth/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `macaw_auth-1.1.0/macaw_auth.egg-info/SOURCES.txt` & `macaw_auth-1.2.0/macaw_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `macaw_auth-1.1.0/pyproject.toml` & `macaw_auth-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.5.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macaw-auth"
-version = "1.1.0"
+version = "1.2.0"
 description = "Tool to obtain AWS CLI credentials from ADFS."
 readme = "README.md"
 authors = [
     { name="Travis Samuel", email="tsamuel@alum.mit.edu" },
 ]
 requires-python = ">3.7"
 classifiers = [
```

### Comparing `macaw_auth-1.1.0/src/macaw_auth/classes/aws_credentials.py` & `macaw_auth-1.2.0/src/macaw_auth/classes/aws_credentials.py`

 * *Files identical despite different names*

### Comparing `macaw_auth-1.1.0/src/macaw_auth/classes/configuration.py` & `macaw_auth-1.2.0/src/macaw_auth/classes/configuration.py`

 * *Files identical despite different names*

### Comparing `macaw_auth-1.1.0/src/macaw_auth/classes/errors.py` & `macaw_auth-1.2.0/src/macaw_auth/classes/errors.py`

 * *Files identical despite different names*

### Comparing `macaw_auth-1.1.0/src/macaw_auth/classes/sts_saml.py` & `macaw_auth-1.2.0/src/macaw_auth/classes/sts_saml.py`

 * *Files identical despite different names*

### Comparing `macaw_auth-1.1.0/src/macaw_auth/classes/user_credentials.py` & `macaw_auth-1.2.0/src/macaw_auth/classes/user_credentials.py`

 * *Files identical despite different names*

### Comparing `macaw_auth-1.1.0/src/macaw_auth/classes/username_validation.py` & `macaw_auth-1.2.0/src/macaw_auth/classes/username_validation.py`

 * *Files identical despite different names*

### Comparing `macaw_auth-1.1.0/src/macaw_auth/cli/__main__.py` & `macaw_auth-1.2.0/src/macaw_auth/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `macaw_auth-1.1.0/src/macaw_auth/cli/cli.py` & `macaw_auth-1.2.0/src/macaw_auth/cli/cli.py`

 * *Files identical despite different names*

### Comparing `macaw_auth-1.1.0/tests/test_usernames.py` & `macaw_auth-1.2.0/tests/test_usernames.py`

 * *Files identical despite different names*

