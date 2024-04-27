# Comparing `tmp/jeedomdaemon-0.7.3.tar.gz` & `tmp/jeedomdaemon-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeedomdaemon-0.7.3.tar", last modified: Fri Apr 26 13:23:42 2024, max compression
+gzip compressed data, was "jeedomdaemon-0.7.4.tar", last modified: Fri Apr 26 13:39:20 2024, max compression
```

## Comparing `jeedomdaemon-0.7.3.tar` & `jeedomdaemon-0.7.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:23:42.885746 jeedomdaemon-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-26 13:23:38.000000 jeedomdaemon-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-26 13:23:42.885746 jeedomdaemon-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-26 13:23:38.000000 jeedomdaemon-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:23:42.881746 jeedomdaemon-0.7.3/jeedomdaemon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:23:38.000000 jeedomdaemon-0.7.3/jeedomdaemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-26 13:23:38.000000 jeedomdaemon-0.7.3/jeedomdaemon/aio_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-26 13:23:38.000000 jeedomdaemon-0.7.3/jeedomdaemon/base_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-26 13:23:38.000000 jeedomdaemon-0.7.3/jeedomdaemon/base_daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-26 13:23:38.000000 jeedomdaemon-0.7.3/jeedomdaemon/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:23:42.885746 jeedomdaemon-0.7.3/jeedomdaemon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-26 13:23:42.000000 jeedomdaemon-0.7.3/jeedomdaemon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-26 13:23:42.000000 jeedomdaemon-0.7.3/jeedomdaemon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 13:23:42.000000 jeedomdaemon-0.7.3/jeedomdaemon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 13:23:42.000000 jeedomdaemon-0.7.3/jeedomdaemon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 13:23:42.000000 jeedomdaemon-0.7.3/jeedomdaemon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 13:23:42.885746 jeedomdaemon-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-26 13:23:38.000000 jeedomdaemon-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:23:42.885746 jeedomdaemon-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:23:38.000000 jeedomdaemon-0.7.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-26 13:23:38.000000 jeedomdaemon-0.7.3/tests/base_config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-26 13:23:38.000000 jeedomdaemon-0.7.3/tests/base_daemon_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:39:20.332732 jeedomdaemon-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-26 13:39:15.000000 jeedomdaemon-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-26 13:39:20.332732 jeedomdaemon-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-26 13:39:15.000000 jeedomdaemon-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:39:20.328732 jeedomdaemon-0.7.4/jeedomdaemon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:39:15.000000 jeedomdaemon-0.7.4/jeedomdaemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-26 13:39:15.000000 jeedomdaemon-0.7.4/jeedomdaemon/aio_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-26 13:39:15.000000 jeedomdaemon-0.7.4/jeedomdaemon/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-26 13:39:15.000000 jeedomdaemon-0.7.4/jeedomdaemon/base_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-26 13:39:15.000000 jeedomdaemon-0.7.4/jeedomdaemon/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:39:20.332732 jeedomdaemon-0.7.4/jeedomdaemon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-26 13:39:20.000000 jeedomdaemon-0.7.4/jeedomdaemon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-26 13:39:20.000000 jeedomdaemon-0.7.4/jeedomdaemon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 13:39:20.000000 jeedomdaemon-0.7.4/jeedomdaemon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 13:39:20.000000 jeedomdaemon-0.7.4/jeedomdaemon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 13:39:20.000000 jeedomdaemon-0.7.4/jeedomdaemon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 13:39:20.332732 jeedomdaemon-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-26 13:39:15.000000 jeedomdaemon-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:39:20.332732 jeedomdaemon-0.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:39:15.000000 jeedomdaemon-0.7.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-26 13:39:15.000000 jeedomdaemon-0.7.4/tests/base_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-26 13:39:15.000000 jeedomdaemon-0.7.4/tests/base_daemon_test.py
```

### Comparing `jeedomdaemon-0.7.3/LICENSE` & `jeedomdaemon-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7.3/PKG-INFO` & `jeedomdaemon-0.7.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeedomdaemon
-Version: 0.7.3
+Version: 0.7.4
 Summary: A base to implement Jeedom daemon in python
 Home-page: https://github.com/Mips2648/jeedom-daemon-py
 Author: Mips
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
@@ -51,21 +51,25 @@
 
 ### Via requirements.txt
 
 ```txt
 jeedomdaemon~=0.7.3
 ```
 
-## Create a daemon skeleton
+## Quick start
 
 Create a file `myDaemon.py` and copy/past the 4 lines of code below and that's it, nothing else to do, your daemon is good to start.
 
 ```python
 from jeedomdaemon.base_daemon import BaseDaemon
 
 class myDaemon(BaseDaemon):
     pass
 
 myDaemon().run()
 ```
 
 Of course, this does nothing so far except starting, accepting incoming requests from your php code and stopping when it is needed.
+
+## What's next
+
+I suggest you to take a look at this [demo plugin](https://github.com/Mips2648/jeedom-aiodemo) which implement this library
```

### Comparing `jeedomdaemon-0.7.3/README.md` & `jeedomdaemon-0.7.4/jeedomdaemon.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: jeedomdaemon
+Version: 0.7.4
+Summary: A base to implement Jeedom daemon in python
+Home-page: https://github.com/Mips2648/jeedom-daemon-py
+Author: Mips
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp
+
 # jeedom-daemon-py
 
 ![pytest 3.9](https://github.com/Mips2648/jeedom-daemon-py/actions/workflows/pytest-3.9.yml/badge.svg)
 ![pytest 3.11](https://github.com/Mips2648/jeedom-daemon-py/actions/workflows/pytest-3.11.yml/badge.svg)
 
 ## Description
 
@@ -40,21 +51,25 @@
 
 ### Via requirements.txt
 
 ```txt
 jeedomdaemon~=0.7.3
 ```
 
-## Create a daemon skeleton
+## Quick start
 
 Create a file `myDaemon.py` and copy/past the 4 lines of code below and that's it, nothing else to do, your daemon is good to start.
 
 ```python
 from jeedomdaemon.base_daemon import BaseDaemon
 
 class myDaemon(BaseDaemon):
     pass
 
 myDaemon().run()
 ```
 
 Of course, this does nothing so far except starting, accepting incoming requests from your php code and stopping when it is needed.
+
+## What's next
+
+I suggest you to take a look at this [demo plugin](https://github.com/Mips2648/jeedom-aiodemo) which implement this library
```

### Comparing `jeedomdaemon-0.7.3/jeedomdaemon/aio_connector.py` & `jeedomdaemon-0.7.4/jeedomdaemon/aio_connector.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7.3/jeedomdaemon/base_config.py` & `jeedomdaemon-0.7.4/jeedomdaemon/base_config.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7.3/jeedomdaemon/base_daemon.py` & `jeedomdaemon-0.7.4/jeedomdaemon/base_daemon.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7.3/jeedomdaemon/utils.py` & `jeedomdaemon-0.7.4/jeedomdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7.3/jeedomdaemon.egg-info/PKG-INFO` & `jeedomdaemon-0.7.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: jeedomdaemon
-Version: 0.7.3
-Summary: A base to implement Jeedom daemon in python
-Home-page: https://github.com/Mips2648/jeedom-daemon-py
-Author: Mips
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiohttp
-
 # jeedom-daemon-py
 
 ![pytest 3.9](https://github.com/Mips2648/jeedom-daemon-py/actions/workflows/pytest-3.9.yml/badge.svg)
 ![pytest 3.11](https://github.com/Mips2648/jeedom-daemon-py/actions/workflows/pytest-3.11.yml/badge.svg)
 
 ## Description
 
@@ -51,21 +40,25 @@
 
 ### Via requirements.txt
 
 ```txt
 jeedomdaemon~=0.7.3
 ```
 
-## Create a daemon skeleton
+## Quick start
 
 Create a file `myDaemon.py` and copy/past the 4 lines of code below and that's it, nothing else to do, your daemon is good to start.
 
 ```python
 from jeedomdaemon.base_daemon import BaseDaemon
 
 class myDaemon(BaseDaemon):
     pass
 
 myDaemon().run()
 ```
 
 Of course, this does nothing so far except starting, accepting incoming requests from your php code and stopping when it is needed.
+
+## What's next
+
+I suggest you to take a look at this [demo plugin](https://github.com/Mips2648/jeedom-aiodemo) which implement this library
```

### Comparing `jeedomdaemon-0.7.3/setup.py` & `jeedomdaemon-0.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     author='Mips',
     # author_email='',
     # Needed to actually package something
     packages=find_packages(),
     # Needed for dependencies
     install_requires=['aiohttp'],
     # *strongly* suggested for sharing
-    version='0.7.3',
+    version='0.7.4',
     # The license can be anything you like
     license='MIT',
     description='A base to implement Jeedom daemon in python',
     # We will also need a readme eventually (there will be a warning)
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
 )
```

### Comparing `jeedomdaemon-0.7.3/tests/base_config_test.py` & `jeedomdaemon-0.7.4/tests/base_config_test.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7.3/tests/base_daemon_test.py` & `jeedomdaemon-0.7.4/tests/base_daemon_test.py`

 * *Files identical despite different names*

