# Comparing `tmp/webdriver_cache_manager-0.0.4.tar.gz` & `tmp/webdriver_cache_manager-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webdriver_cache_manager-0.0.4.tar", last modified: Fri Apr 26 17:04:45 2024, max compression
+gzip compressed data, was "webdriver_cache_manager-0.0.5.tar", last modified: Sat Apr 27 19:53:14 2024, max compression
```

## Comparing `webdriver_cache_manager-0.0.4.tar` & `webdriver_cache_manager-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:04:45.655012 webdriver_cache_manager-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-26 17:04:41.000000 webdriver_cache_manager-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-26 17:04:45.655012 webdriver_cache_manager-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-26 17:04:41.000000 webdriver_cache_manager-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-26 17:04:41.000000 webdriver_cache_manager-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 17:04:45.655012 webdriver_cache_manager-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:04:45.651012 webdriver_cache_manager-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:04:45.655012 webdriver_cache_manager-0.0.4/src/webdriver_cache_manager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:04:41.000000 webdriver_cache_manager-0.0.4/src/webdriver_cache_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-26 17:04:41.000000 webdriver_cache_manager-0.0.4/src/webdriver_cache_manager/webdriver_cache_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:04:45.655012 webdriver_cache_manager-0.0.4/src/webdriver_cache_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-26 17:04:45.000000 webdriver_cache_manager-0.0.4/src/webdriver_cache_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-26 17:04:45.000000 webdriver_cache_manager-0.0.4/src/webdriver_cache_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 17:04:45.000000 webdriver_cache_manager-0.0.4/src/webdriver_cache_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 17:04:45.000000 webdriver_cache_manager-0.0.4/src/webdriver_cache_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:53:14.430691 webdriver_cache_manager-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-27 19:53:10.000000 webdriver_cache_manager-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-27 19:53:14.430691 webdriver_cache_manager-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-27 19:53:10.000000 webdriver_cache_manager-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-27 19:53:10.000000 webdriver_cache_manager-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 19:53:14.430691 webdriver_cache_manager-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:53:14.430691 webdriver_cache_manager-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:53:14.430691 webdriver_cache_manager-0.0.5/src/webdriver_cache_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 19:53:10.000000 webdriver_cache_manager-0.0.5/src/webdriver_cache_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-27 19:53:10.000000 webdriver_cache_manager-0.0.5/src/webdriver_cache_manager/webdriver_cache_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:53:14.430691 webdriver_cache_manager-0.0.5/src/webdriver_cache_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-27 19:53:14.000000 webdriver_cache_manager-0.0.5/src/webdriver_cache_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-27 19:53:14.000000 webdriver_cache_manager-0.0.5/src/webdriver_cache_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 19:53:14.000000 webdriver_cache_manager-0.0.5/src/webdriver_cache_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-27 19:53:14.000000 webdriver_cache_manager-0.0.5/src/webdriver_cache_manager.egg-info/top_level.txt
```

### Comparing `webdriver_cache_manager-0.0.4/LICENSE` & `webdriver_cache_manager-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `webdriver_cache_manager-0.0.4/PKG-INFO` & `webdriver_cache_manager-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdriver_cache_manager
-Version: 0.0.4
+Version: 0.0.5
 Summary: Optimize WebDriver usage in Selenium with Python. Manage processes, terminate efficiently, and handle PIDs using CSV. Simplify automation!
 Author-email: Muhammad Nawaz <MNawaz6935@gmail.com>
 Project-URL: Homepage, https://github.com/mnawaz6935/webdriver_cache_manager
 Project-URL: Issues, https://github.com/mnawaz6935/webdriver_cache_manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `webdriver_cache_manager-0.0.4/README.md` & `webdriver_cache_manager-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `webdriver_cache_manager-0.0.4/pyproject.toml` & `webdriver_cache_manager-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "webdriver_cache_manager"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Muhammad Nawaz", email="MNawaz6935@gmail.com" },
 ]
 description = "Optimize WebDriver usage in Selenium with Python. Manage processes, terminate efficiently, and handle PIDs using CSV. Simplify automation!"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `webdriver_cache_manager-0.0.4/src/webdriver_cache_manager.egg-info/PKG-INFO` & `webdriver_cache_manager-0.0.5/src/webdriver_cache_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdriver_cache_manager
-Version: 0.0.4
+Version: 0.0.5
 Summary: Optimize WebDriver usage in Selenium with Python. Manage processes, terminate efficiently, and handle PIDs using CSV. Simplify automation!
 Author-email: Muhammad Nawaz <MNawaz6935@gmail.com>
 Project-URL: Homepage, https://github.com/mnawaz6935/webdriver_cache_manager
 Project-URL: Issues, https://github.com/mnawaz6935/webdriver_cache_manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

