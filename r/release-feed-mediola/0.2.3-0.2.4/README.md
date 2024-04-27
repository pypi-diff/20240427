# Comparing `tmp/release_feed_mediola-0.2.3.tar.gz` & `tmp/release_feed_mediola-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "release_feed_mediola-0.2.3.tar", max compression
+gzip compressed data, was "release_feed_mediola-0.2.4.tar", max compression
```

## Comparing `release_feed_mediola-0.2.3.tar` & `release_feed_mediola-0.2.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11358 2024-02-11 10:49:26.856466 release_feed_mediola-0.2.3/LICENSE
--rw-r--r--   0        0        0     3279 2024-02-11 10:49:26.856466 release_feed_mediola-0.2.3/README.md
--rw-r--r--   0        0        0     1251 2024-02-11 10:49:26.856466 release_feed_mediola-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      479 2024-02-11 10:49:26.856466 release_feed_mediola-0.2.3/release_feed_mediola/__init__.py
--rw-r--r--   0        0        0       99 2024-02-11 10:49:26.856466 release_feed_mediola-0.2.3/release_feed_mediola/__main__.py
--rw-r--r--   0        0        0     4133 2024-02-11 10:49:26.856466 release_feed_mediola-0.2.3/release_feed_mediola/api.py
--rw-r--r--   0        0        0      490 2024-02-11 10:49:26.856466 release_feed_mediola-0.2.3/release_feed_mediola/cli.py
--rw-r--r--   0        0        0     1046 2024-02-11 10:49:26.856466 release_feed_mediola-0.2.3/release_feed_mediola/settings.py
--rw-r--r--   0        0        0     3798 1970-01-01 00:00:00.000000 release_feed_mediola-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-27 19:16:47.303205 release_feed_mediola-0.2.4/LICENSE
+-rw-r--r--   0        0        0     3279 2024-04-27 19:16:47.303205 release_feed_mediola-0.2.4/README.md
+-rw-r--r--   0        0        0     1247 2024-04-27 19:16:47.303205 release_feed_mediola-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      479 2024-04-27 19:16:47.303205 release_feed_mediola-0.2.4/release_feed_mediola/__init__.py
+-rw-r--r--   0        0        0       99 2024-04-27 19:16:47.303205 release_feed_mediola-0.2.4/release_feed_mediola/__main__.py
+-rw-r--r--   0        0        0     4133 2024-04-27 19:16:47.303205 release_feed_mediola-0.2.4/release_feed_mediola/api.py
+-rw-r--r--   0        0        0      490 2024-04-27 19:16:47.303205 release_feed_mediola-0.2.4/release_feed_mediola/cli.py
+-rw-r--r--   0        0        0     1046 2024-04-27 19:16:47.303205 release_feed_mediola-0.2.4/release_feed_mediola/settings.py
+-rw-r--r--   0        0        0     3793 1970-01-01 00:00:00.000000 release_feed_mediola-0.2.4/PKG-INFO
```

### Comparing `release_feed_mediola-0.2.3/LICENSE` & `release_feed_mediola-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `release_feed_mediola-0.2.3/README.md` & `release_feed_mediola-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `release_feed_mediola-0.2.3/pyproject.toml` & `release_feed_mediola-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.9.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "release_feed_mediola"
-version = "0.2.3"
+version = "0.2.4"
 description = "Atom feed for software product releases of Mediola AG"
 readme = "README.md"
 authors = ["Claudia Pellegrino <clau@tiqua.de>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "~3.11"
-feedgen = "^0.9.0"
+feedgen = "^1.0"
 requests = "^2.31.0"
 
 [tool.poetry.dev-dependencies]
 autopep8 = "*"
-mypy = "~=1.5.1"
+mypy = "~=1.8"
 pdoc = "~=14.0"
 poethepoet = "~=0.24"
 pylint = "~=3.0"
 pytest = "*"
 
 [tool.poetry.group.dev.dependencies]
 types-requests = "^2.31.0"
```

### Comparing `release_feed_mediola-0.2.3/release_feed_mediola/api.py` & `release_feed_mediola-0.2.4/release_feed_mediola/api.py`

 * *Files identical despite different names*

### Comparing `release_feed_mediola-0.2.3/release_feed_mediola/settings.py` & `release_feed_mediola-0.2.4/release_feed_mediola/settings.py`

 * *Files identical despite different names*

### Comparing `release_feed_mediola-0.2.3/PKG-INFO` & `release_feed_mediola-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: release_feed_mediola
-Version: 0.2.3
+Version: 0.2.4
 Summary: Atom feed for software product releases of Mediola AG
 License: Apache-2.0
 Author: Claudia Pellegrino
 Author-email: clau@tiqua.de
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: feedgen (>=0.9.0,<0.10.0)
+Requires-Dist: feedgen (>=1.0,<2.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # release-feed-mediola
 
 A tool that generates Atom feeds for software updates of
 [Mediola](https://www.mediola.com/) products.
```

