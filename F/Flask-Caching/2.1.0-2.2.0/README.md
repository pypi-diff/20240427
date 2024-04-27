# Comparing `tmp/Flask-Caching-2.1.0.tar.gz` & `tmp/flask_caching-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Caching-2.1.0.tar", last modified: Sun Oct  8 14:15:45 2023, max compression
+gzip compressed data, was "flask_caching-2.2.0.tar", last modified: Sat Apr 27 16:05:14 2024, max compression
```

## Comparing `Flask-Caching-2.1.0.tar` & `flask_caching-2.2.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2023-10-08 14:15:45.174530 Flask-Caching-2.1.0/
--rw-r--r--   0 gfvante    (501) staff       (20)     3119 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/LICENSE
--rw-r--r--   0 gfvante    (501) staff       (20)      260 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/MANIFEST.in
--rw-r--r--   0 gfvante    (501) staff       (20)     2167 2023-10-08 14:15:45.174613 Flask-Caching-2.1.0/PKG-INFO
--rw-r--r--   0 gfvante    (501) staff       (20)     1062 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/README.rst
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2023-10-08 14:15:45.169073 Flask-Caching-2.1.0/docs/
--rw-r--r--   0 gfvante    (501) staff       (20)     7634 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/docs/Makefile
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2023-10-08 14:15:45.169330 Flask-Caching-2.1.0/docs/_static/
--rw-r--r--   0 gfvante    (501) staff       (20)    14917 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/docs/_static/flask-cache.png
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2023-10-08 14:15:45.169596 Flask-Caching-2.1.0/docs/_templates/
--rw-r--r--   0 gfvante    (501) staff       (20)      210 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/docs/_templates/sidebarintro.html
--rw-r--r--   0 gfvante    (501) staff       (20)      697 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/docs/api.rst
--rw-r--r--   0 gfvante    (501) staff       (20)       28 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/docs/changelog.rst
--rw-r--r--   0 gfvante    (501) staff       (20)    10603 2023-10-08 13:54:02.000000 Flask-Caching-2.1.0/docs/conf.py
--rw-r--r--   0 gfvante    (501) staff       (20)    26361 2023-10-07 22:16:15.000000 Flask-Caching-2.1.0/docs/index.rst
--rw-r--r--   0 gfvante    (501) staff       (20)       67 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/docs/license.rst
--rw-r--r--   0 gfvante    (501) staff       (20)     7465 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/docs/make.bat
--rw-r--r--   0 gfvante    (501) staff       (20)     2069 2023-10-08 14:15:45.175147 Flask-Caching-2.1.0/setup.cfg
--rwxr-xr-x   0 gfvante    (501) staff       (20)      204 2023-10-07 22:16:15.000000 Flask-Caching-2.1.0/setup.py
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2023-10-08 14:15:45.166021 Flask-Caching-2.1.0/src/
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2023-10-08 14:15:45.170365 Flask-Caching-2.1.0/src/Flask_Caching.egg-info/
--rw-r--r--   0 gfvante    (501) staff       (20)     2167 2023-10-08 14:15:45.000000 Flask-Caching-2.1.0/src/Flask_Caching.egg-info/PKG-INFO
--rw-r--r--   0 gfvante    (501) staff       (20)     1197 2023-10-08 14:15:45.000000 Flask-Caching-2.1.0/src/Flask_Caching.egg-info/SOURCES.txt
--rw-r--r--   0 gfvante    (501) staff       (20)        1 2023-10-08 14:15:45.000000 Flask-Caching-2.1.0/src/Flask_Caching.egg-info/dependency_links.txt
--rw-r--r--   0 gfvante    (501) staff       (20)       30 2023-10-08 14:15:45.000000 Flask-Caching-2.1.0/src/Flask_Caching.egg-info/requires.txt
--rw-r--r--   0 gfvante    (501) staff       (20)       14 2023-10-08 14:15:45.000000 Flask-Caching-2.1.0/src/Flask_Caching.egg-info/top_level.txt
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2023-10-08 14:15:45.170890 Flask-Caching-2.1.0/src/flask_caching/
--rw-r--r--   0 gfvante    (501) staff       (20)    41004 2023-10-08 13:55:49.000000 Flask-Caching-2.1.0/src/flask_caching/__init__.py
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2023-10-08 14:15:45.172206 Flask-Caching-2.1.0/src/flask_caching/backends/
--rw-r--r--   0 gfvante    (501) staff       (20)     2214 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/src/flask_caching/backends/__init__.py
--rw-r--r--   0 gfvante    (501) staff       (20)     1500 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/src/flask_caching/backends/base.py
--rw-r--r--   0 gfvante    (501) staff       (20)     2680 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/src/flask_caching/backends/filesystemcache.py
--rw-r--r--   0 gfvante    (501) staff       (20)     7634 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/src/flask_caching/backends/memcache.py
--rw-r--r--   0 gfvante    (501) staff       (20)      625 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/src/flask_caching/backends/nullcache.py
--rw-r--r--   0 gfvante    (501) staff       (20)     9485 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/src/flask_caching/backends/rediscache.py
--rw-r--r--   0 gfvante    (501) staff       (20)     2065 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/src/flask_caching/backends/simplecache.py
--rw-r--r--   0 gfvante    (501) staff       (20)      429 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/src/flask_caching/backends/uwsgicache.py
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2023-10-08 14:15:45.172736 Flask-Caching-2.1.0/src/flask_caching/contrib/
--rw-r--r--   0 gfvante    (501) staff       (20)        0 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/src/flask_caching/contrib/__init__.py
--rw-r--r--   0 gfvante    (501) staff       (20)     7527 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/src/flask_caching/contrib/googlecloudstoragecache.py
--rw-r--r--   0 gfvante    (501) staff       (20)     2295 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/src/flask_caching/contrib/uwsgicache.py
--rw-r--r--   0 gfvante    (501) staff       (20)     2919 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/src/flask_caching/jinja2ext.py
--rw-r--r--   0 gfvante    (501) staff       (20)        0 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/src/flask_caching/py.typed
--rw-r--r--   0 gfvante    (501) staff       (20)     3238 2023-10-07 22:16:15.000000 Flask-Caching-2.1.0/src/flask_caching/utils.py
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2023-10-08 14:15:45.174213 Flask-Caching-2.1.0/tests/
--rw-r--r--   0 gfvante    (501) staff       (20)     2298 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/tests/conftest.py
--rw-r--r--   0 gfvante    (501) staff       (20)     7899 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/tests/test_backend_cache.py
--rw-r--r--   0 gfvante    (501) staff       (20)     3840 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/tests/test_basic_app.py
--rw-r--r--   0 gfvante    (501) staff       (20)     9536 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/tests/test_cache.py
--rw-r--r--   0 gfvante    (501) staff       (20)     1329 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/tests/test_init.py
--rw-r--r--   0 gfvante    (501) staff       (20)    22816 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/tests/test_memoize.py
--rw-r--r--   0 gfvante    (501) staff       (20)      242 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/tests/test_template.html
--rw-r--r--   0 gfvante    (501) staff       (20)     1940 2023-01-12 15:56:37.000000 Flask-Caching-2.1.0/tests/test_templates.py
--rw-r--r--   0 gfvante    (501) staff       (20)    16728 2023-01-12 17:17:51.000000 Flask-Caching-2.1.0/tests/test_view.py
--rw-r--r--   0 gfvante    (501) staff       (20)      554 2023-10-07 22:16:15.000000 Flask-Caching-2.1.0/tox.ini
+drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-04-27 16:05:14.224943 flask_caching-2.2.0/
+-rw-r--r--   0 gfvante    (501) staff       (20)     3119 2023-01-12 15:56:37.000000 flask_caching-2.2.0/LICENSE
+-rw-r--r--   0 gfvante    (501) staff       (20)      260 2023-01-12 15:56:37.000000 flask_caching-2.2.0/MANIFEST.in
+-rw-r--r--   0 gfvante    (501) staff       (20)     2207 2024-04-27 16:05:14.224868 flask_caching-2.2.0/PKG-INFO
+-rw-r--r--   0 gfvante    (501) staff       (20)     1062 2023-01-12 15:56:37.000000 flask_caching-2.2.0/README.rst
+drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-04-27 16:05:14.219149 flask_caching-2.2.0/docs/
+-rw-r--r--   0 gfvante    (501) staff       (20)     7634 2023-01-12 15:56:37.000000 flask_caching-2.2.0/docs/Makefile
+drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-04-27 16:05:14.219339 flask_caching-2.2.0/docs/_static/
+-rw-r--r--   0 gfvante    (501) staff       (20)    14917 2023-01-12 15:56:37.000000 flask_caching-2.2.0/docs/_static/flask-cache.png
+drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-04-27 16:05:14.219550 flask_caching-2.2.0/docs/_templates/
+-rw-r--r--   0 gfvante    (501) staff       (20)      210 2023-01-12 15:56:37.000000 flask_caching-2.2.0/docs/_templates/sidebarintro.html
+-rw-r--r--   0 gfvante    (501) staff       (20)      697 2023-01-12 15:56:37.000000 flask_caching-2.2.0/docs/api.rst
+-rw-r--r--   0 gfvante    (501) staff       (20)       28 2023-01-12 15:56:37.000000 flask_caching-2.2.0/docs/changelog.rst
+-rw-r--r--   0 gfvante    (501) staff       (20)    10603 2023-10-08 13:54:02.000000 flask_caching-2.2.0/docs/conf.py
+-rw-r--r--   0 gfvante    (501) staff       (20)    26370 2024-04-27 15:47:35.000000 flask_caching-2.2.0/docs/index.rst
+-rw-r--r--   0 gfvante    (501) staff       (20)       67 2023-01-12 15:56:37.000000 flask_caching-2.2.0/docs/license.rst
+-rw-r--r--   0 gfvante    (501) staff       (20)     7465 2023-01-12 15:56:37.000000 flask_caching-2.2.0/docs/make.bat
+-rw-r--r--   0 gfvante    (501) staff       (20)     2075 2024-04-27 16:05:14.225510 flask_caching-2.2.0/setup.cfg
+-rwxr-xr-x   0 gfvante    (501) staff       (20)      204 2023-10-07 22:16:15.000000 flask_caching-2.2.0/setup.py
+drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-04-27 16:05:14.215939 flask_caching-2.2.0/src/
+drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-04-27 16:05:14.224593 flask_caching-2.2.0/src/Flask_Caching.egg-info/
+-rw-r--r--   0 gfvante    (501) staff       (20)     2207 2024-04-27 16:05:14.000000 flask_caching-2.2.0/src/Flask_Caching.egg-info/PKG-INFO
+-rw-r--r--   0 gfvante    (501) staff       (20)     1197 2024-04-27 16:05:14.000000 flask_caching-2.2.0/src/Flask_Caching.egg-info/SOURCES.txt
+-rw-r--r--   0 gfvante    (501) staff       (20)        1 2024-04-27 16:05:14.000000 flask_caching-2.2.0/src/Flask_Caching.egg-info/dependency_links.txt
+-rw-r--r--   0 gfvante    (501) staff       (20)       30 2024-04-27 16:05:14.000000 flask_caching-2.2.0/src/Flask_Caching.egg-info/requires.txt
+-rw-r--r--   0 gfvante    (501) staff       (20)       14 2024-04-27 16:05:14.000000 flask_caching-2.2.0/src/Flask_Caching.egg-info/top_level.txt
+drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-04-27 16:05:14.220889 flask_caching-2.2.0/src/flask_caching/
+-rw-r--r--   0 gfvante    (501) staff       (20)    41299 2024-04-27 15:58:21.000000 flask_caching-2.2.0/src/flask_caching/__init__.py
+drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-04-27 16:05:14.222134 flask_caching-2.2.0/src/flask_caching/backends/
+-rw-r--r--   0 gfvante    (501) staff       (20)     2215 2024-04-27 15:19:34.000000 flask_caching-2.2.0/src/flask_caching/backends/__init__.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     1501 2024-04-27 15:19:34.000000 flask_caching-2.2.0/src/flask_caching/backends/base.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     2680 2024-04-27 15:19:34.000000 flask_caching-2.2.0/src/flask_caching/backends/filesystemcache.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     7634 2024-04-27 15:19:34.000000 flask_caching-2.2.0/src/flask_caching/backends/memcache.py
+-rw-r--r--   0 gfvante    (501) staff       (20)      626 2024-04-27 15:19:34.000000 flask_caching-2.2.0/src/flask_caching/backends/nullcache.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     9344 2024-04-27 15:47:35.000000 flask_caching-2.2.0/src/flask_caching/backends/rediscache.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     2066 2024-04-27 15:19:34.000000 flask_caching-2.2.0/src/flask_caching/backends/simplecache.py
+-rw-r--r--   0 gfvante    (501) staff       (20)      455 2024-04-27 15:19:34.000000 flask_caching-2.2.0/src/flask_caching/backends/uwsgicache.py
+drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-04-27 16:05:14.222745 flask_caching-2.2.0/src/flask_caching/contrib/
+-rw-r--r--   0 gfvante    (501) staff       (20)        0 2023-01-12 15:56:37.000000 flask_caching-2.2.0/src/flask_caching/contrib/__init__.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     7527 2023-01-12 15:56:37.000000 flask_caching-2.2.0/src/flask_caching/contrib/googlecloudstoragecache.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     2296 2024-04-27 15:19:34.000000 flask_caching-2.2.0/src/flask_caching/contrib/uwsgicache.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     2920 2024-04-27 15:19:34.000000 flask_caching-2.2.0/src/flask_caching/jinja2ext.py
+-rw-r--r--   0 gfvante    (501) staff       (20)        0 2023-01-12 15:56:37.000000 flask_caching-2.2.0/src/flask_caching/py.typed
+-rw-r--r--   0 gfvante    (501) staff       (20)     3238 2023-10-07 22:16:15.000000 flask_caching-2.2.0/src/flask_caching/utils.py
+drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-04-27 16:05:14.224396 flask_caching-2.2.0/tests/
+-rw-r--r--   0 gfvante    (501) staff       (20)     2298 2023-01-12 15:56:37.000000 flask_caching-2.2.0/tests/conftest.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     7894 2024-04-27 15:47:35.000000 flask_caching-2.2.0/tests/test_backend_cache.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     3840 2023-01-12 15:56:37.000000 flask_caching-2.2.0/tests/test_basic_app.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     9536 2023-01-12 15:56:37.000000 flask_caching-2.2.0/tests/test_cache.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     1329 2023-01-12 15:56:37.000000 flask_caching-2.2.0/tests/test_init.py
+-rw-r--r--   0 gfvante    (501) staff       (20)    23087 2024-04-27 15:47:35.000000 flask_caching-2.2.0/tests/test_memoize.py
+-rw-r--r--   0 gfvante    (501) staff       (20)      242 2023-01-12 15:56:37.000000 flask_caching-2.2.0/tests/test_template.html
+-rw-r--r--   0 gfvante    (501) staff       (20)     1940 2023-01-12 15:56:37.000000 flask_caching-2.2.0/tests/test_templates.py
+-rw-r--r--   0 gfvante    (501) staff       (20)    16728 2024-04-27 15:19:34.000000 flask_caching-2.2.0/tests/test_view.py
+-rw-r--r--   0 gfvante    (501) staff       (20)      555 2024-04-27 15:19:34.000000 flask_caching-2.2.0/tox.ini
```

### Comparing `Flask-Caching-2.1.0/LICENSE` & `flask_caching-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-Caching-2.1.0/PKG-INFO` & `flask_caching-2.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: Flask-Caching
-Version: 2.1.0
+Version: 2.2.0
 Summary: Adds caching support to Flask applications.
 Home-page: https://github.com/pallets-eco/flask-caching
 Author: Peter Justin
 Author-email: peter.justin@outlook.com
 Maintainer: Pallets
 Maintainer-email: contact@palletsprojects.com
 License: BSD
 Project-URL: Donate, https://palletsprojects.com/donate
 Project-URL: Documentation, https://flask-caching.readthedocs.io
 Project-URL: Changes, https://flask-caching.readthedocs.io/en/latest/changelog.html
 Project-URL: Source Code, https://github.com/pallets-eco/flask-caching
 Project-URL: Issue Tracker, https://github.com/pallets-eco/flask-caching/issues
 Project-URL: Twitter, https://twitter.com/PalletsTeam
 Project-URL: Chat, https://discord.gg/pallets
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: cachelib<0.10.0,>=0.9.0
+Requires-Dist: Flask
 
 Flask-Caching
 =============
 
 A fork of the `Flask-cache`_ extension which adds easy cache support to Flask.
 
 .. _Flask-cache: https://github.com/thadeusb/flask-cache
@@ -62,9 +63,7 @@
 -   Documentation: https://flask-caching.readthedocs.io
 -   Changes: https://flask-caching.readthedocs.io/en/latest/changelog.html
 -   PyPI Releases: https://pypi.org/project/Flask-Caching/
 -   Source Code: https://github.com/pallets-eco/flask-caching
 -   Issue Tracker: https://github.com/pallets-eco/flask-caching/issues
 -   Twitter: https://twitter.com/PalletsTeam
 -   Chat: https://discord.gg/pallets
-
-
```

### Comparing `Flask-Caching-2.1.0/README.rst` & `flask_caching-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-Caching-2.1.0/docs/Makefile` & `flask_caching-2.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-Caching-2.1.0/docs/_static/flask-cache.png` & `flask_caching-2.2.0/docs/_static/flask-cache.png`

 * *Files identical despite different names*

### Comparing `Flask-Caching-2.1.0/docs/api.rst` & `flask_caching-2.2.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `Flask-Caching-2.1.0/docs/conf.py` & `flask_caching-2.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Flask-Caching-2.1.0/docs/index.rst` & `flask_caching-2.2.0/docs/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 Sometimes you want to define your cache key for each route. Using the same ``@cached``
 decorator you are able to specify how this key is generated. This might be useful when
 the key for cache is should not be just the default key_prefix, but has to be derived
 from other parameters in a request. An example usecase would be for caching POST routes.
 Where the cache key should be derived from the data in that request, rather than just the
 route/view itself.
 
-``make_cache_key`` can be used to specify such a function. The function should return a 
+``make_cache_key`` can be used to specify such a function. The function should return a
 string which should act like the key to the required value that is being cached::
 
    def make_key():
       """A function which is called to derive the key for a computed value.
          The key in this case is the concat value of all the json request
          parameters. Other strategy could to use any hashing function.
       :returns: unique string for which the value should be cached.
@@ -402,16 +402,16 @@
 ``CACHE_DEFAULT_TIMEOUT``       The timeout that is used if no other
                                 timeout is specified. Unit of time is
                                 seconds. Defaults to ``300``.
 ``CACHE_IGNORE_ERRORS``         If set to any errors that occurred during the
                                 deletion process will be ignored. However, if
                                 it is set to ``False`` it will stop on the
                                 first error. This option is only relevant for
-                                the backends **filesystem** and **simple**.
-                                Defaults to ``False``.
+                                the backends **FileSystemCache** and
+                                **SimpleCache**. Defaults to ``False``.
 ``CACHE_THRESHOLD``             The maximum number of items the cache
                                 will store before it starts deleting
                                 some. Used only for SimpleCache and
                                 FileSystemCache. Defaults to ``500``.
 ``CACHE_KEY_PREFIX``            A prefix that is added before all keys.
                                 This makes it possible to use the same
                                 memcached server for different apps.
```

### Comparing `Flask-Caching-2.1.0/docs/make.bat` & `flask_caching-2.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Flask-Caching-2.1.0/setup.cfg` & `flask_caching-2.2.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 	Operating System :: OS Independent
 	Programming Language :: Python
 
 [options]
 packages = find:
 package_dir = = src
 include_package_data = true
-python_requires = >= 3.7
+python_requires = >= 3.8
 
 [options.packages.find]
 where = src
 
 [build_sphinx]
 source-dir = docs/
 build-dir = docs/_build
@@ -46,14 +46,15 @@
 [flake8]
 select = B, E, F, W, B9, ISC
 ignore = 
 	E203
 	E501
 	E722
 	W503
+	B905
 max-line-length = 80
 
 [coverage:run]
 branch = True
 omit = 
 	src/flask_caching/contrib/*
 source = 
@@ -74,15 +75,15 @@
 disallow_subclassing_any = true
 disallow_untyped_decorators = true
 no_implicit_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 strict_equality = true
 strict_concatenate = true
-python_version = 3.7
+python_version = 3.8
 
 [mypy-uwsgi]
 ignore_missing_imports = True
 
 [mypy-rediscluster]
 ignore_missing_imports = True
```

### Comparing `Flask-Caching-2.1.0/src/Flask_Caching.egg-info/PKG-INFO` & `flask_caching-2.2.0/src/Flask_Caching.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: Flask-Caching
-Version: 2.1.0
+Version: 2.2.0
 Summary: Adds caching support to Flask applications.
 Home-page: https://github.com/pallets-eco/flask-caching
 Author: Peter Justin
 Author-email: peter.justin@outlook.com
 Maintainer: Pallets
 Maintainer-email: contact@palletsprojects.com
 License: BSD
 Project-URL: Donate, https://palletsprojects.com/donate
 Project-URL: Documentation, https://flask-caching.readthedocs.io
 Project-URL: Changes, https://flask-caching.readthedocs.io/en/latest/changelog.html
 Project-URL: Source Code, https://github.com/pallets-eco/flask-caching
 Project-URL: Issue Tracker, https://github.com/pallets-eco/flask-caching/issues
 Project-URL: Twitter, https://twitter.com/PalletsTeam
 Project-URL: Chat, https://discord.gg/pallets
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: cachelib<0.10.0,>=0.9.0
+Requires-Dist: Flask
 
 Flask-Caching
 =============
 
 A fork of the `Flask-cache`_ extension which adds easy cache support to Flask.
 
 .. _Flask-cache: https://github.com/thadeusb/flask-cache
@@ -62,9 +63,7 @@
 -   Documentation: https://flask-caching.readthedocs.io
 -   Changes: https://flask-caching.readthedocs.io/en/latest/changelog.html
 -   PyPI Releases: https://pypi.org/project/Flask-Caching/
 -   Source Code: https://github.com/pallets-eco/flask-caching
 -   Issue Tracker: https://github.com/pallets-eco/flask-caching/issues
 -   Twitter: https://twitter.com/PalletsTeam
 -   Chat: https://discord.gg/pallets
-
-
```

### Comparing `Flask-Caching-2.1.0/src/Flask_Caching.egg-info/SOURCES.txt` & `flask_caching-2.2.0/src/Flask_Caching.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-Caching-2.1.0/src/flask_caching/__init__.py` & `flask_caching-2.2.0/src/flask_caching/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,30 @@
     ~~~~~~~~~~~~~
 
     Adds cache support to your application.
 
     :copyright: (c) 2010 by Thadeus Burgess.
     :license: BSD, see LICENSE for more details.
 """
+
 import base64
 import functools
 import hashlib
 import inspect
 import logging
 import uuid
 import warnings
 from collections import OrderedDict
-from typing import Any, Dict, List, Callable, Optional, Tuple, Union
+from typing import Any
+from typing import Callable
+from typing import Dict
+from typing import List
+from typing import Optional
+from typing import Tuple
+from typing import Union
 
 from flask import current_app
 from flask import Flask
 from flask import request
 from flask import Response
 from flask import url_for
 from werkzeug.utils import import_string
@@ -29,15 +36,15 @@
 from flask_caching.utils import function_namespace
 from flask_caching.utils import get_arg_default
 from flask_caching.utils import get_arg_names
 from flask_caching.utils import get_id
 from flask_caching.utils import make_template_fragment_key  # noqa: F401
 from flask_caching.utils import wants_args
 
-__version__ = "2.1.0"
+__version__ = "2.2.0"
 
 logger = logging.getLogger(__name__)
 
 SUPPORTED_HASH_FUNCTIONS = [
     hashlib.sha1,
     hashlib.sha224,
     hashlib.sha256,
@@ -109,24 +116,26 @@
         config.setdefault("CACHE_TYPE", "null")
         config.setdefault("CACHE_NO_NULL_WARNING", False)
         config.setdefault("CACHE_SOURCE_CHECK", False)
 
         if config["CACHE_TYPE"] == "null" and not config["CACHE_NO_NULL_WARNING"]:
             warnings.warn(
                 "Flask-Caching: CACHE_TYPE is set to null, "
-                "caching is effectively disabled."
+                "caching is effectively disabled.",
+                stacklevel=2,
             )
 
         if (
             config["CACHE_TYPE"] in ["filesystem", "FileSystemCache"]
             and config["CACHE_DIR"] is None
         ):
             warnings.warn(
                 f"Flask-Caching: CACHE_TYPE is set to {config['CACHE_TYPE']} but no "
-                "CACHE_DIR is set."
+                "CACHE_DIR is set.",
+                stacklevel=2,
             )
 
         self.source_check = config["CACHE_SOURCE_CHECK"]
 
         if self.with_jinja2_ext:
             from .jinja2ext import CacheExtension, JINJA_CACHE_ATTR_NAME
 
@@ -151,14 +160,15 @@
             cache_factory = cache_factory.factory
         elif plain_name_used:
             warnings.warn(
                 "Using the initialization functions in flask_caching.backend "
                 "is deprecated.  Use the a full path to backend classes "
                 "directly.",
                 category=DeprecationWarning,
+                stacklevel=2,
             )
 
         if config["CACHE_OPTIONS"]:
             cache_options.update(config["CACHE_OPTIONS"])
 
         if not hasattr(app, "extensions"):
             app.extensions = {}
@@ -354,15 +364,17 @@
                 if source_check is None:
                     source_check = self.source_check
 
                 try:
                     if make_cache_key is not None and callable(make_cache_key):
                         cache_key = make_cache_key(*args, **kwargs)
                     else:
-                        cache_key = decorated_function.make_cache_key(*args, use_request=True, **kwargs)
+                        cache_key = decorated_function.make_cache_key(
+                            *args, use_request=True, **kwargs
+                        )
 
                     if (
                         callable(forced_update)
                         and (
                             forced_update(*args, **kwargs)
                             if wants_args(forced_update)
                             else forced_update()
@@ -421,15 +433,15 @@
                 # `make_cache_key` expects them) to keyword arguments
                 # (the way `url_for` expects them)
                 argspec_args = inspect.getfullargspec(f).args
 
                 for arg_name, arg in zip(argspec_args, args):
                     kwargs[arg_name] = arg
 
-                use_request = kwargs.pop('use_request', False)
+                use_request = kwargs.pop("use_request", False)
                 return _make_cache_key(args, kwargs, use_request=use_request)
 
             def _make_cache_key_query_string():
                 """Create consistent keys for query string arguments.
 
                 Produces the same cache key regardless of argument order, e.g.,
                 both `?limit=10&offset=20` and `?offset=20&limit=10` will
@@ -634,15 +646,15 @@
         #: 1, b=2 is equivalent to a=1, b=2, etc.
         new_args = []
         arg_num = 0
         args_to_ignore = kwargs.pop("args_to_ignore", None) or []
 
         # If the function uses VAR_KEYWORD type of parameters,
         # we need to pass these further
-        kw_keys_remaining = list(kwargs.keys())
+        kw_keys_remaining = [key for key in kwargs.keys() if key not in args_to_ignore]
         arg_names = get_arg_names(f)
         args_len = len(arg_names)
 
         for i in range(args_len):
             arg_default = get_arg_default(f, i)
             if arg_names[i] in args_to_ignore:
                 arg = None
```

### Comparing `Flask-Caching-2.1.0/src/flask_caching/backends/__init__.py` & `flask_caching-2.2.0/src/flask_caching/backends/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
     Various caching backends.
 
     :copyright: (c) 2018 by Peter Justin.
     :copyright: (c) 2010 by Thadeus Burgess.
     :license: BSD, see LICENSE for more details.
 """
+
 from flask_caching.backends.filesystemcache import FileSystemCache
 from flask_caching.backends.memcache import MemcachedCache
 from flask_caching.backends.memcache import SASLMemcachedCache
 from flask_caching.backends.memcache import SpreadSASLMemcachedCache
 from flask_caching.backends.nullcache import NullCache
 from flask_caching.backends.rediscache import RedisCache
 from flask_caching.backends.rediscache import RedisClusterCache
```

### Comparing `Flask-Caching-2.1.0/src/flask_caching/backends/base.py` & `flask_caching-2.2.0/src/flask_caching/backends/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     This module contains the BaseCache that other caching
     backends have to implement.
 
     :copyright: (c) 2018 by Peter Justin.
     :copyright: (c) 2010 by Thadeus Burgess.
     :license: BSD, see LICENSE for more details.
 """
+
 from cachelib import BaseCache as CachelibBaseCache
 
 
 class BaseCache(CachelibBaseCache):
     """Baseclass for the cache systems.  All the cache systems implement this
     API or a superset of it.
```

### Comparing `Flask-Caching-2.1.0/src/flask_caching/backends/filesystemcache.py` & `flask_caching-2.2.0/src/flask_caching/backends/filesystemcache.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 
     The filesystem caching backend.
 
     :copyright: (c) 2018 by Peter Justin.
     :copyright: (c) 2010 by Thadeus Burgess.
     :license: BSD, see LICENSE for more details.
 """
+
 import hashlib
 import logging
 
 from cachelib import FileSystemCache as CachelibFileSystemCache
 
 from flask_caching.backends.base import BaseCache
 
 logger = logging.getLogger(__name__)
 
 
 class FileSystemCache(BaseCache, CachelibFileSystemCache):
-
     """A cache that stores the items on the file system.  This cache depends
     on being the only user of the `cache_dir`.  Make absolutely sure that
     nobody but this cache stores files there or otherwise the cache will
     randomly delete files therein.
 
     :param cache_dir: the directory where cache files are stored.
     :param threshold: the maximum number of items the cache stores before
```

### Comparing `Flask-Caching-2.1.0/src/flask_caching/backends/memcache.py` & `flask_caching-2.2.0/src/flask_caching/backends/memcache.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
     The memcache caching backend.
 
     :copyright: (c) 2018 by Peter Justin.
     :copyright: (c) 2010 by Thadeus Burgess.
     :license: BSD, see LICENSE for more details.
 """
+
 import pickle
 import re
 
 from cachelib import MemcachedCache as CachelibMemcachedCache
 
 from flask_caching.backends.base import BaseCache
 
 
 _test_memcached_key = re.compile(r"[^\x00-\x21\xff]{1,250}$").match
 
 
 class MemcachedCache(BaseCache, CachelibMemcachedCache):
-
     """A cache that uses memcached as backend.
 
     The first argument can either be an object that resembles the API of a
     :class:`memcache.Client` or a tuple/list of server addresses. In the
     event that a tuple/list is passed, Werkzeug tries to import the best
     available memcache library.
```

### Comparing `Flask-Caching-2.1.0/src/flask_caching/backends/nullcache.py` & `flask_caching-2.2.0/src/flask_caching/backends/nullcache.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
     The null cache backend. A caching backend that doesn't cache.
 
     :copyright: (c) 2018 by Peter Justin.
     :copyright: (c) 2010 by Thadeus Burgess.
     :license: BSD, see LICENSE for more details.
 """
+
 from flask_caching.backends.base import BaseCache
 
 
 class NullCache(BaseCache):
     """A cache that doesn't cache. This can be useful for unit testing.
 
     :param default_timeout: a dummy parameter that is ignored but exists
```

### Comparing `Flask-Caching-2.1.0/src/flask_caching/backends/rediscache.py` & `flask_caching-2.2.0/src/flask_caching/backends/rediscache.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
     The redis caching backend.
 
     :copyright: (c) 2018 by Peter Justin.
     :copyright: (c) 2010 by Thadeus Burgess.
     :license: BSD, see LICENSE for more details.
 """
+
 import pickle
 
 from cachelib import RedisCache as CachelibRedisCache
 
 from flask_caching.backends.base import BaseCache
 
 
@@ -85,19 +86,14 @@
         if redis_url:
             kwargs["host"] = redis_from_url(redis_url, db=kwargs.pop("db", None))
 
         new_class = cls(*args, **kwargs)
 
         return new_class
 
-    def _get_prefix(self):
-        return (
-            self.key_prefix if isinstance(self.key_prefix, str) else self.key_prefix()
-        )
-
     def dump_object(self, value):
         """Dumps an object into a string for redis.  By default it serializes
         integers as regular string and pickle dumps everything else.
         """
         t = type(value)
         if t == int:
             return str(value).encode("ascii")
```

### Comparing `Flask-Caching-2.1.0/src/flask_caching/backends/simplecache.py` & `flask_caching-2.2.0/src/flask_caching/backends/simplecache.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
     The simple cache backend.
 
     :copyright: (c) 2018 by Peter Justin.
     :copyright: (c) 2010 by Thadeus Burgess.
     :license: BSD, see LICENSE for more details.
 """
+
 import logging
 
 from cachelib import SimpleCache as CachelibSimpleCache
 
 from flask_caching.backends.base import BaseCache
```

### Comparing `Flask-Caching-2.1.0/src/flask_caching/contrib/googlecloudstoragecache.py` & `flask_caching-2.2.0/src/flask_caching/contrib/googlecloudstoragecache.py`

 * *Files identical despite different names*

### Comparing `Flask-Caching-2.1.0/src/flask_caching/contrib/uwsgicache.py` & `flask_caching-2.2.0/src/flask_caching/contrib/uwsgicache.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
     The uWSGI caching backend.
 
     :copyright: (c) 2018 by Peter Justin.
     :copyright: (c) 2010 by Thadeus Burgess.
     :license: BSD, see LICENSE for more details.
 """
+
 from cachelib import UWSGICache as CachelibUWSGICache
 
 from flask_caching.backends.base import BaseCache
 
 
 class UWSGICache(BaseCache, CachelibUWSGICache):
     """Implements the cache using uWSGI's caching framework.
```

### Comparing `Flask-Caching-2.1.0/src/flask_caching/jinja2ext.py` & `flask_caching-2.2.0/src/flask_caching/jinja2ext.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
             </form>
         </div>
         {% endcache %}
 
     :copyright: (c) 2010 by Thadeus Burgess.
     :license: BSD, see LICENSE for more details.
 """
+
 from jinja2 import nodes
 from jinja2.ext import Extension
 
 from flask_caching import make_template_fragment_key
 
 JINJA_CACHE_ATTR_NAME = "_template_fragment_cache"
```

### Comparing `Flask-Caching-2.1.0/src/flask_caching/utils.py` & `flask_caching-2.2.0/src/flask_caching/utils.py`

 * *Files identical despite different names*

### Comparing `Flask-Caching-2.1.0/tests/conftest.py` & `flask_caching-2.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Flask-Caching-2.1.0/tests/test_backend_cache.py` & `flask_caching-2.2.0/tests/test_backend_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     ~~~~~~~~~~~
 
     Tests the cache system
 
     :copyright: (c) 2014 by Armin Ronacher.
     :license: BSD, see LICENSE for more details.
 """
+
 import pickle
 import time
 
 import pytest
 
 from flask_caching import backends
 from flask_caching.backends import RedisSentinelCache
@@ -185,17 +186,17 @@
             host = redis.Redis()
 
         c = backends.RedisCache(host=host, key_prefix=key_prefix)
         yield lambda: c
         c.clear()
 
     def test_compat(self, c):
-        assert c._write_client.set(c._get_prefix() + "foo", "Awesome")
+        assert c._write_client.set(c.key_prefix + "foo", "Awesome")
         assert c.get("foo") == b"Awesome"
-        assert c._write_client.set(c._get_prefix() + "foo", "42")
+        assert c._write_client.set(c.key_prefix + "foo", "42")
         assert c.get("foo") == 42
 
     def test_empty_host(self):
         with pytest.raises(ValueError) as exc_info:
             backends.RedisCache(host=None)
         assert str(exc_info.value) == "RedisCache host parameter may not be None"
```

### Comparing `Flask-Caching-2.1.0/tests/test_basic_app.py` & `flask_caching-2.2.0/tests/test_basic_app.py`

 * *Files identical despite different names*

### Comparing `Flask-Caching-2.1.0/tests/test_cache.py` & `flask_caching-2.2.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `Flask-Caching-2.1.0/tests/test_init.py` & `flask_caching-2.2.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `Flask-Caching-2.1.0/tests/test_memoize.py` & `flask_caching-2.2.0/tests/test_memoize.py`

 * *Files 1% similar despite different names*

```diff
@@ -830,7 +830,16 @@
 
         class Foo:
             @cache.memoize(50, args_to_ignore=["self"])
             def big_foo(self, a, b):
                 return a + b + random.randrange(0, 100000)
 
         assert Foo().big_foo(5, 2) == Foo().big_foo(5, 2)
+
+
+def test_memoize_function_ignore_kwarg(app, cache):
+    with app.test_request_context():
+        @cache.memoize(50, args_to_ignore=["b"])
+        def big_foo(a, b):
+            return a + b + random.randrange(0, 100000)
+
+        assert big_foo(5, 2) == big_foo(5, b=3)
```

### Comparing `Flask-Caching-2.1.0/tests/test_templates.py` & `flask_caching-2.2.0/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `Flask-Caching-2.1.0/tests/test_view.py` & `flask_caching-2.2.0/tests/test_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,15 @@
 
 def test_set_make_cache_key_property(app, cache):
     @app.route("/")
     @cache.cached(5)
     def cached_view():
         return str(time.time())
 
-    cached_view.make_cache_key = lambda *args, **kwargs: request.args['foo']
+    cached_view.make_cache_key = lambda *args, **kwargs: request.args["foo"]
 
     tc = app.test_client()
 
     rv = tc.get("/?foo=a")
     a = rv.data.decode("utf-8")
 
     rv = tc.get("/?foo=b")
```

### Comparing `Flask-Caching-2.1.0/tox.ini` & `flask_caching-2.2.0/tox.ini`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tox]
 envlist =
-    py{39,38,37,py3,310}
+    py{39,38,py3,310,311}
     style
     typing
     docs
 skip_missing_interpreters = true
 
 [testenv]
 setenv = TMPDIR={envtmpdir}
```

