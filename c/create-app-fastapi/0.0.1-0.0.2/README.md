# Comparing `tmp/create-app-fastapi-0.0.1.tar.gz` & `tmp/create-app-fastapi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "create-app-fastapi-0.0.1.tar", last modified: Sat Apr 27 10:19:54 2024, max compression
+gzip compressed data, was "create-app-fastapi-0.0.2.tar", last modified: Sat Apr 27 10:24:30 2024, max compression
```

## Comparing `create-app-fastapi-0.0.1.tar` & `create-app-fastapi-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-04-27 10:19:54.946858 create-app-fastapi-0.0.1/
--rw-rw-r--   0 bosco     (1000) bosco     (1000)      468 2024-04-27 10:19:54.946858 create-app-fastapi-0.0.1/PKG-INFO
-drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-04-27 10:19:54.942858 create-app-fastapi-0.0.1/create_app_fastapi.egg-info/
--rw-rw-r--   0 bosco     (1000) bosco     (1000)      468 2024-04-27 10:19:54.000000 create-app-fastapi-0.0.1/create_app_fastapi.egg-info/PKG-INFO
--rw-rw-r--   0 bosco     (1000) bosco     (1000)      296 2024-04-27 10:19:54.000000 create-app-fastapi-0.0.1/create_app_fastapi.egg-info/SOURCES.txt
--rw-rw-r--   0 bosco     (1000) bosco     (1000)        1 2024-04-27 10:19:54.000000 create-app-fastapi-0.0.1/create_app_fastapi.egg-info/dependency_links.txt
--rw-rw-r--   0 bosco     (1000) bosco     (1000)       61 2024-04-27 10:19:54.000000 create-app-fastapi-0.0.1/create_app_fastapi.egg-info/entry_points.txt
--rw-rw-r--   0 bosco     (1000) bosco     (1000)       15 2024-04-27 10:19:54.000000 create-app-fastapi-0.0.1/create_app_fastapi.egg-info/top_level.txt
-drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-04-27 10:19:54.942858 create-app-fastapi-0.0.1/projectfastapi/
--rw-rw-r--   0 bosco     (1000) bosco     (1000)        0 2024-04-27 10:16:31.000000 create-app-fastapi-0.0.1/projectfastapi/__init__.py
--rw-rw-r--   0 bosco     (1000) bosco     (1000)     3550 2024-04-27 10:16:56.000000 create-app-fastapi-0.0.1/projectfastapi/main.py
--rw-rw-r--   0 bosco     (1000) bosco     (1000)     2202 2024-04-26 13:06:58.000000 create-app-fastapi-0.0.1/projectfastapi/source.py
--rw-rw-r--   0 bosco     (1000) bosco     (1000)       38 2024-04-27 10:19:54.946858 create-app-fastapi-0.0.1/setup.cfg
--rw-rw-r--   0 bosco     (1000) bosco     (1000)      668 2024-04-27 10:19:45.000000 create-app-fastapi-0.0.1/setup.py
+drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-04-27 10:24:30.061327 create-app-fastapi-0.0.2/
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)      468 2024-04-27 10:24:30.061327 create-app-fastapi-0.0.2/PKG-INFO
+drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-04-27 10:24:30.061327 create-app-fastapi-0.0.2/create_app_fastapi.egg-info/
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)      468 2024-04-27 10:24:30.000000 create-app-fastapi-0.0.2/create_app_fastapi.egg-info/PKG-INFO
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)      296 2024-04-27 10:24:30.000000 create-app-fastapi-0.0.2/create_app_fastapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)        1 2024-04-27 10:24:30.000000 create-app-fastapi-0.0.2/create_app_fastapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)       65 2024-04-27 10:24:30.000000 create-app-fastapi-0.0.2/create_app_fastapi.egg-info/entry_points.txt
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)       15 2024-04-27 10:24:30.000000 create-app-fastapi-0.0.2/create_app_fastapi.egg-info/top_level.txt
+drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-04-27 10:24:30.061327 create-app-fastapi-0.0.2/projectfastapi/
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)        0 2024-04-27 10:16:31.000000 create-app-fastapi-0.0.2/projectfastapi/__init__.py
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)     3551 2024-04-27 10:22:13.000000 create-app-fastapi-0.0.2/projectfastapi/main.py
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)     2202 2024-04-26 13:06:58.000000 create-app-fastapi-0.0.2/projectfastapi/source.py
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)       38 2024-04-27 10:24:30.061327 create-app-fastapi-0.0.2/setup.cfg
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)      672 2024-04-27 10:23:13.000000 create-app-fastapi-0.0.2/setup.py
```

### Comparing `create-app-fastapi-0.0.1/projectfastapi/main.py` & `create-app-fastapi-0.0.2/projectfastapi/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os, platform, sys, subprocess, threading, time
-from source import getFileData
+from .source import getFileData
 
 curdir= os.getcwd()
 platformOS= platform.system()
 threadStop= False
 
 # terminal color code
 RED = "\033[31m"
```

### Comparing `create-app-fastapi-0.0.1/projectfastapi/source.py` & `create-app-fastapi-0.0.2/projectfastapi/source.py`

 * *Files identical despite different names*

### Comparing `create-app-fastapi-0.0.1/setup.py` & `create-app-fastapi-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup( 
 	name="create-app-fastapi", 
-	version="0.0.1", 
+	version="0.0.2", 
 	author="Ravishnu", 
 	author_email="ravishnu60@gmail.com", 
 	packages=find_packages(), 
 	description="Package to create fastapi project", 
 	long_description="A package used to create fastAPI project structure with virtual environment and dependencies", 
 	long_description_content_type="text/markdown", 
 	python_requires='>=3.9', 
 	install_requires=[],
 	entry_points ={ 
 		'console_scripts': [ 
-			'create-fastapi=projectfastapi.main:main'
+			'create-app-fastapi=projectfastapi.main:main'
 		] 
 	},
     keywords=['fastapi', 'fastapi project','project structure','api structure', 'python fastapi project structure']
 )
```

