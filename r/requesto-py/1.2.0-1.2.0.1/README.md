# Comparing `tmp/requesto-py-1.2.0.tar.gz` & `tmp/requesto_py-1.2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requesto-py-1.2.0.tar", last modified: Sun Apr  7 17:44:41 2024, max compression
+gzip compressed data, was "requesto_py-1.2.0.1.tar", last modified: Sat Apr 27 13:06:31 2024, max compression
```

## Comparing `requesto-py-1.2.0.tar` & `requesto_py-1.2.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 17:44:41.761184 requesto-py-1.2.0/
--rw-rw-rw-   0        0        0    35823 2024-04-07 17:41:12.000000 requesto-py-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     2879 2024-04-07 17:44:41.760184 requesto-py-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2260 2024-04-07 17:41:12.000000 requesto-py-1.2.0/README.md
--rw-rw-rw-   0        0        0      727 2024-04-07 17:44:29.000000 requesto-py-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-07 17:44:41.762184 requesto-py-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-07 17:44:41.735872 requesto-py-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-07 17:44:41.750463 requesto-py-1.2.0/src/requesto/
--rw-rw-rw-   0        0        0      139 2024-04-07 17:41:12.000000 requesto-py-1.2.0/src/requesto/Exceptions.py
--rw-rw-rw-   0        0        0     2308 2024-04-07 17:41:12.000000 requesto-py-1.2.0/src/requesto/PostgresDb.py
--rw-rw-rw-   0        0        0     1179 2024-04-07 17:41:12.000000 requesto-py-1.2.0/src/requesto/SqliteDb.py
--rw-rw-rw-   0        0        0      278 2024-04-07 17:41:12.000000 requesto-py-1.2.0/src/requesto/User.py
--rw-rw-rw-   0        0        0     1675 2024-04-07 17:41:12.000000 requesto-py-1.2.0/src/requesto/__init__.py
--rw-rw-rw-   0        0        0    12586 2024-04-07 17:41:12.000000 requesto-py-1.2.0/src/requesto/requesto.py
-drwxrwxrwx   0        0        0        0 2024-04-07 17:44:41.759188 requesto-py-1.2.0/src/requesto_py.egg-info/
--rw-rw-rw-   0        0        0     2879 2024-04-07 17:44:41.000000 requesto-py-1.2.0/src/requesto_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2024-04-07 17:44:41.000000 requesto-py-1.2.0/src/requesto_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 17:44:41.000000 requesto-py-1.2.0/src/requesto_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-07 17:44:41.000000 requesto-py-1.2.0/src/requesto_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 13:06:31.250882 requesto_py-1.2.0.1/
+-rw-rw-rw-   0        0        0    35823 2024-04-07 17:41:12.000000 requesto_py-1.2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2881 2024-04-27 13:06:31.249884 requesto_py-1.2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2260 2024-04-07 17:41:12.000000 requesto_py-1.2.0.1/README.md
+-rw-rw-rw-   0        0        0      729 2024-04-07 17:53:30.000000 requesto_py-1.2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-27 13:06:31.250882 requesto_py-1.2.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-27 13:06:31.233879 requesto_py-1.2.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-27 13:06:31.241882 requesto_py-1.2.0.1/src/requesto/
+-rw-rw-rw-   0        0        0      139 2024-04-07 17:41:12.000000 requesto_py-1.2.0.1/src/requesto/Exceptions.py
+-rw-rw-rw-   0        0        0     2365 2024-04-27 13:03:40.000000 requesto_py-1.2.0.1/src/requesto/PostgresDb.py
+-rw-rw-rw-   0        0        0     1179 2024-04-07 17:41:12.000000 requesto_py-1.2.0.1/src/requesto/SqliteDb.py
+-rw-rw-rw-   0        0        0      278 2024-04-07 17:41:12.000000 requesto_py-1.2.0.1/src/requesto/User.py
+-rw-rw-rw-   0        0        0     1675 2024-04-08 15:55:09.000000 requesto_py-1.2.0.1/src/requesto/__init__.py
+-rw-rw-rw-   0        0        0    12586 2024-04-07 17:41:12.000000 requesto_py-1.2.0.1/src/requesto/requesto.py
+drwxrwxrwx   0        0        0        0 2024-04-27 13:06:31.248884 requesto_py-1.2.0.1/src/requesto_py.egg-info/
+-rw-rw-rw-   0        0        0     2881 2024-04-27 13:06:31.000000 requesto_py-1.2.0.1/src/requesto_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2024-04-27 13:06:31.000000 requesto_py-1.2.0.1/src/requesto_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 13:06:31.000000 requesto_py-1.2.0.1/src/requesto_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-27 13:06:31.000000 requesto_py-1.2.0.1/src/requesto_py.egg-info/top_level.txt
```

### Comparing `requesto-py-1.2.0/LICENSE` & `requesto_py-1.2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `requesto-py-1.2.0/PKG-INFO` & `requesto_py-1.2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requesto-py
-Version: 1.2.0
+Version: 1.2.0.1
 Summary: Lightweight python wrapper library for psycopg2 and sqlite3 databases without tons of useless code.
 Author-email: NaroMori <reply.naromori@google.com>
 Project-URL: Homepage, https://github.com/SOLIDusr/requesto-py
 Project-URL: Issues, https://github.com/SOLIDusr/requesto-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `requesto-py-1.2.0/README.md` & `requesto_py-1.2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `requesto-py-1.2.0/pyproject.toml` & `requesto_py-1.2.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0", "psycopg2>=2.9.9", "pip>=23.3.2"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "requesto-py"
-version = "1.2.0"
+version = "1.2.0.1"
 authors = [
   { name="NaroMori", email="reply.naromori@google.com" },
 ]
 description = "Lightweight python wrapper library for psycopg2 and sqlite3 databases without tons of useless code."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `requesto-py-1.2.0/src/requesto/PostgresDb.py` & `requesto_py-1.2.0.1/src/requesto/PostgresDb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .requesto import DataBase
 from .User import User
-
+from .Exceptions import ConnectionDetailsMissingException
 try:
     import psycopg2 as pg
 except ImportError:
     raise ImportError("Psycopg2 is not installed. Please install it using pip.")
 
 
 class PostgresDb(DataBase):
```

### Comparing `requesto-py-1.2.0/src/requesto/SqliteDb.py` & `requesto_py-1.2.0.1/src/requesto/SqliteDb.py`

 * *Files identical despite different names*

### Comparing `requesto-py-1.2.0/src/requesto/__init__.py` & `requesto_py-1.2.0.1/src/requesto/__init__.py`

 * *Files identical despite different names*

### Comparing `requesto-py-1.2.0/src/requesto/requesto.py` & `requesto_py-1.2.0.1/src/requesto/requesto.py`

 * *Files identical despite different names*

### Comparing `requesto-py-1.2.0/src/requesto_py.egg-info/PKG-INFO` & `requesto_py-1.2.0.1/src/requesto_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requesto-py
-Version: 1.2.0
+Version: 1.2.0.1
 Summary: Lightweight python wrapper library for psycopg2 and sqlite3 databases without tons of useless code.
 Author-email: NaroMori <reply.naromori@google.com>
 Project-URL: Homepage, https://github.com/SOLIDusr/requesto-py
 Project-URL: Issues, https://github.com/SOLIDusr/requesto-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

