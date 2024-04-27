# Comparing `tmp/barter_auth-0.2.8.tar.gz` & `tmp/barter_auth-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barter_auth-0.2.8.tar", last modified: Fri Jan 12 11:15:51 2024, max compression
+gzip compressed data, was "barter_auth-0.2.9.tar", last modified: Fri Jan 12 11:36:35 2024, max compression
```

## Comparing `barter_auth-0.2.8.tar` & `barter_auth-0.2.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 toha      (1000) toha      (1000)        0 2024-01-12 11:15:51.648162 barter_auth-0.2.8/
--rw-rw-r--   0 toha      (1000) toha      (1000)     1073 2023-12-04 13:19:05.000000 barter_auth-0.2.8/LICENSE
--rw-rw-r--   0 toha      (1000) toha      (1000)     4150 2024-01-12 11:15:51.648162 barter_auth-0.2.8/PKG-INFO
--rw-rw-r--   0 toha      (1000) toha      (1000)     3552 2024-01-12 08:12:33.000000 barter_auth-0.2.8/README.md
--rw-rw-r--   0 toha      (1000) toha      (1000)      923 2024-01-12 11:15:34.000000 barter_auth-0.2.8/pyproject.toml
--rw-rw-r--   0 toha      (1000) toha      (1000)       38 2024-01-12 11:15:51.648162 barter_auth-0.2.8/setup.cfg
--rw-rw-r--   0 toha      (1000) toha      (1000)     1159 2024-01-12 11:15:34.000000 barter_auth-0.2.8/setup.py
-drwxrwxr-x   0 toha      (1000) toha      (1000)        0 2024-01-12 11:15:51.648162 barter_auth-0.2.8/src/
--rw-rw-r--   0 toha      (1000) toha      (1000)        0 2023-12-11 06:11:09.000000 barter_auth-0.2.8/src/__init__.py
-drwxrwxr-x   0 toha      (1000) toha      (1000)        0 2024-01-12 11:15:51.648162 barter_auth-0.2.8/src/barter_auth/
--rw-rw-r--   0 toha      (1000) toha      (1000)       45 2023-12-22 20:53:13.000000 barter_auth-0.2.8/src/barter_auth/__init__.py
--rw-rw-r--   0 toha      (1000) toha      (1000)     3127 2024-01-11 09:00:19.000000 barter_auth-0.2.8/src/barter_auth/auth.py
--rw-rw-r--   0 toha      (1000) toha      (1000)      812 2023-12-16 20:32:41.000000 barter_auth-0.2.8/src/barter_auth/constants.py
--rw-rw-r--   0 toha      (1000) toha      (1000)     4133 2024-01-11 09:00:19.000000 barter_auth-0.2.8/src/barter_auth/exceptions.py
-drwxrwxr-x   0 toha      (1000) toha      (1000)        0 2024-01-12 11:15:51.648162 barter_auth-0.2.8/src/barter_auth/models/
--rw-rw-r--   0 toha      (1000) toha      (1000)       47 2023-12-18 20:06:18.000000 barter_auth-0.2.8/src/barter_auth/models/__init__.py
--rw-rw-r--   0 toha      (1000) toha      (1000)     3477 2024-01-12 11:15:34.000000 barter_auth-0.2.8/src/barter_auth/models/profiles.py
--rw-rw-r--   0 toha      (1000) toha      (1000)     2057 2024-01-11 09:00:19.000000 barter_auth-0.2.8/src/barter_auth/models/users.py
-drwxrwxr-x   0 toha      (1000) toha      (1000)        0 2024-01-12 11:15:51.648162 barter_auth-0.2.8/src/barter_auth/permissions/
--rw-rw-r--   0 toha      (1000) toha      (1000)       26 2023-12-22 23:11:46.000000 barter_auth-0.2.8/src/barter_auth/permissions/__init__.py
--rw-rw-r--   0 toha      (1000) toha      (1000)     3992 2023-12-23 00:12:46.000000 barter_auth-0.2.8/src/barter_auth/permissions/constants.py
--rw-rw-r--   0 toha      (1000) toha      (1000)     4818 2024-01-12 04:48:51.000000 barter_auth-0.2.8/src/barter_auth/providers.py
--rw-rw-r--   0 toha      (1000) toha      (1000)      674 2024-01-12 06:50:51.000000 barter_auth-0.2.8/src/barter_auth/settings.py
-drwxrwxr-x   0 toha      (1000) toha      (1000)        0 2024-01-12 11:15:51.648162 barter_auth-0.2.8/src/barter_auth.egg-info/
--rw-rw-r--   0 toha      (1000) toha      (1000)     4150 2024-01-12 11:15:51.000000 barter_auth-0.2.8/src/barter_auth.egg-info/PKG-INFO
--rw-rw-r--   0 toha      (1000) toha      (1000)      612 2024-01-12 11:15:51.000000 barter_auth-0.2.8/src/barter_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 toha      (1000) toha      (1000)        1 2024-01-12 11:15:51.000000 barter_auth-0.2.8/src/barter_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 toha      (1000) toha      (1000)      103 2024-01-12 11:15:51.000000 barter_auth-0.2.8/src/barter_auth.egg-info/requires.txt
--rw-rw-r--   0 toha      (1000) toha      (1000)       21 2024-01-12 11:15:51.000000 barter_auth-0.2.8/src/barter_auth.egg-info/top_level.txt
+drwxrwxr-x   0 toha      (1000) toha      (1000)        0 2024-01-12 11:36:35.483963 barter_auth-0.2.9/
+-rw-rw-r--   0 toha      (1000) toha      (1000)     1073 2023-12-04 13:19:05.000000 barter_auth-0.2.9/LICENSE
+-rw-rw-r--   0 toha      (1000) toha      (1000)     4150 2024-01-12 11:36:35.483963 barter_auth-0.2.9/PKG-INFO
+-rw-rw-r--   0 toha      (1000) toha      (1000)     3552 2024-01-12 08:12:33.000000 barter_auth-0.2.9/README.md
+-rw-rw-r--   0 toha      (1000) toha      (1000)      923 2024-01-12 11:36:30.000000 barter_auth-0.2.9/pyproject.toml
+-rw-rw-r--   0 toha      (1000) toha      (1000)       38 2024-01-12 11:36:35.483963 barter_auth-0.2.9/setup.cfg
+-rw-rw-r--   0 toha      (1000) toha      (1000)     1159 2024-01-12 11:36:30.000000 barter_auth-0.2.9/setup.py
+drwxrwxr-x   0 toha      (1000) toha      (1000)        0 2024-01-12 11:36:35.479963 barter_auth-0.2.9/src/
+-rw-rw-r--   0 toha      (1000) toha      (1000)        0 2023-12-11 06:11:09.000000 barter_auth-0.2.9/src/__init__.py
+drwxrwxr-x   0 toha      (1000) toha      (1000)        0 2024-01-12 11:36:35.483963 barter_auth-0.2.9/src/barter_auth/
+-rw-rw-r--   0 toha      (1000) toha      (1000)       45 2023-12-22 20:53:13.000000 barter_auth-0.2.9/src/barter_auth/__init__.py
+-rw-rw-r--   0 toha      (1000) toha      (1000)     3127 2024-01-11 09:00:19.000000 barter_auth-0.2.9/src/barter_auth/auth.py
+-rw-rw-r--   0 toha      (1000) toha      (1000)      812 2023-12-16 20:32:41.000000 barter_auth-0.2.9/src/barter_auth/constants.py
+-rw-rw-r--   0 toha      (1000) toha      (1000)     4133 2024-01-11 09:00:19.000000 barter_auth-0.2.9/src/barter_auth/exceptions.py
+drwxrwxr-x   0 toha      (1000) toha      (1000)        0 2024-01-12 11:36:35.483963 barter_auth-0.2.9/src/barter_auth/models/
+-rw-rw-r--   0 toha      (1000) toha      (1000)       47 2023-12-18 20:06:18.000000 barter_auth-0.2.9/src/barter_auth/models/__init__.py
+-rw-rw-r--   0 toha      (1000) toha      (1000)     3494 2024-01-12 11:36:30.000000 barter_auth-0.2.9/src/barter_auth/models/profiles.py
+-rw-rw-r--   0 toha      (1000) toha      (1000)     2057 2024-01-11 09:00:19.000000 barter_auth-0.2.9/src/barter_auth/models/users.py
+drwxrwxr-x   0 toha      (1000) toha      (1000)        0 2024-01-12 11:36:35.483963 barter_auth-0.2.9/src/barter_auth/permissions/
+-rw-rw-r--   0 toha      (1000) toha      (1000)       26 2023-12-22 23:11:46.000000 barter_auth-0.2.9/src/barter_auth/permissions/__init__.py
+-rw-rw-r--   0 toha      (1000) toha      (1000)     3992 2023-12-23 00:12:46.000000 barter_auth-0.2.9/src/barter_auth/permissions/constants.py
+-rw-rw-r--   0 toha      (1000) toha      (1000)     4818 2024-01-12 04:48:51.000000 barter_auth-0.2.9/src/barter_auth/providers.py
+-rw-rw-r--   0 toha      (1000) toha      (1000)      674 2024-01-12 06:50:51.000000 barter_auth-0.2.9/src/barter_auth/settings.py
+drwxrwxr-x   0 toha      (1000) toha      (1000)        0 2024-01-12 11:36:35.483963 barter_auth-0.2.9/src/barter_auth.egg-info/
+-rw-rw-r--   0 toha      (1000) toha      (1000)     4150 2024-01-12 11:36:35.000000 barter_auth-0.2.9/src/barter_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 toha      (1000) toha      (1000)      612 2024-01-12 11:36:35.000000 barter_auth-0.2.9/src/barter_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 toha      (1000) toha      (1000)        1 2024-01-12 11:36:35.000000 barter_auth-0.2.9/src/barter_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 toha      (1000) toha      (1000)      103 2024-01-12 11:36:35.000000 barter_auth-0.2.9/src/barter_auth.egg-info/requires.txt
+-rw-rw-r--   0 toha      (1000) toha      (1000)       21 2024-01-12 11:36:35.000000 barter_auth-0.2.9/src/barter_auth.egg-info/top_level.txt
```

### Comparing `barter_auth-0.2.8/LICENSE` & `barter_auth-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `barter_auth-0.2.8/PKG-INFO` & `barter_auth-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barter_auth
-Version: 0.2.8
+Version: 0.2.9
 Summary: Barter authentication package
 Home-page: https://github.com/kabilovtoha/barter_auth
 Author: akatoha
 Author-email: kabilov <kabilov2011@gmail.com>
 License: BSD
 Project-URL: Homepage, https://github.com/kabilovtoha/barter_auth
 Project-URL: Bug Tracker, https://github.com/kabilovtoha/barter_auth/issues
```

### Comparing `barter_auth-0.2.8/README.md` & `barter_auth-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `barter_auth-0.2.8/pyproject.toml` & `barter_auth-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "barter_auth"
-version = "0.2.8"
+version = "0.2.9"
 authors = [
     { name = "kabilov", email = "kabilov2011@gmail.com" },
 ]
 description = "Barter authentication package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `barter_auth-0.2.8/setup.py` & `barter_auth-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 
 setup(
     name='barter-auth',
-    version='0.2.8',
+    version='0.2.9',
     include_package_data=True,
     license='BSD',
     description='Django bulk admin enables you to bulk add, bulk edit, bulk upload and bulk select in django admin.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/kabilovtoha/barter_auth',
     author='akatoha',
```

### Comparing `barter_auth-0.2.8/src/barter_auth/auth.py` & `barter_auth-0.2.9/src/barter_auth/auth.py`

 * *Files identical despite different names*

### Comparing `barter_auth-0.2.8/src/barter_auth/constants.py` & `barter_auth-0.2.9/src/barter_auth/constants.py`

 * *Files identical despite different names*

### Comparing `barter_auth-0.2.8/src/barter_auth/exceptions.py` & `barter_auth-0.2.9/src/barter_auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `barter_auth-0.2.8/src/barter_auth/models/profiles.py` & `barter_auth-0.2.9/src/barter_auth/models/profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 from datetime import datetime
 from uuid import UUID
 
 from pydantic import BaseModel
 
 from ..constants import Role
 
+__all__ = [
+    'Profile', 'AnonymousProfile',
+    'Advertiser', 'Instagram', 'Anonymous',
+    'Category',
+]
 
 class Advertiser(BaseModel):
     class Config:
         # pydantic.config.BaseConfig
         frozen = True
 
     uuid: UUID
@@ -153,11 +158,7 @@
     def is_blogger(self):
         return self.role == Role.INSTAGRAM
 
     def is_advertiser(self):
         return self.role == Role.ADVERTISER
 
 
-__all__ = [
-    'Profile', 'AnonymousProfile',
-    'Advertiser', 'Instagram', 'Anonymous',
-]
```

### Comparing `barter_auth-0.2.8/src/barter_auth/models/users.py` & `barter_auth-0.2.9/src/barter_auth/models/users.py`

 * *Files identical despite different names*

### Comparing `barter_auth-0.2.8/src/barter_auth/permissions/constants.py` & `barter_auth-0.2.9/src/barter_auth/permissions/constants.py`

 * *Files identical despite different names*

### Comparing `barter_auth-0.2.8/src/barter_auth/providers.py` & `barter_auth-0.2.9/src/barter_auth/providers.py`

 * *Files identical despite different names*

### Comparing `barter_auth-0.2.8/src/barter_auth/settings.py` & `barter_auth-0.2.9/src/barter_auth/settings.py`

 * *Files identical despite different names*

### Comparing `barter_auth-0.2.8/src/barter_auth.egg-info/PKG-INFO` & `barter_auth-0.2.9/src/barter_auth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barter-auth
-Version: 0.2.8
+Version: 0.2.9
 Summary: Barter authentication package
 Home-page: https://github.com/kabilovtoha/barter_auth
 Author: akatoha
 Author-email: kabilov <kabilov2011@gmail.com>
 License: BSD
 Project-URL: Homepage, https://github.com/kabilovtoha/barter_auth
 Project-URL: Bug Tracker, https://github.com/kabilovtoha/barter_auth/issues
```

### Comparing `barter_auth-0.2.8/src/barter_auth.egg-info/SOURCES.txt` & `barter_auth-0.2.9/src/barter_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

