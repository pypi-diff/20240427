# Comparing `tmp/mlops_api_gemstack-0.3.5.tar.gz` & `tmp/mlops_api_gemstack-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlops_api_gemstack-0.3.5.tar", last modified: Sat Apr 27 16:14:36 2024, max compression
+gzip compressed data, was "mlops_api_gemstack-0.3.6.tar", last modified: Sat Apr 27 16:20:42 2024, max compression
```

## Comparing `mlops_api_gemstack-0.3.5.tar` & `mlops_api_gemstack-0.3.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 16:14:36.545481 mlops_api_gemstack-0.3.5/
--rw-r--r--   0 ricardosun   (501) staff       (20)     1071 2024-04-22 05:08:20.000000 mlops_api_gemstack-0.3.5/LICENSE
--rw-r--r--   0 ricardosun   (501) staff       (20)     4206 2024-04-27 16:14:36.544282 mlops_api_gemstack-0.3.5/PKG-INFO
--rw-r--r--   0 ricardosun   (501) staff       (20)     3807 2024-04-23 07:20:14.000000 mlops_api_gemstack-0.3.5/README.md
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 16:14:36.537112 mlops_api_gemstack-0.3.5/mlops_api_gemstack/
--rw-r--r--   0 ricardosun   (501) staff       (20)       18 2024-04-20 05:10:06.000000 mlops_api_gemstack-0.3.5/mlops_api_gemstack/__init__.py
--rw-r--r--   0 ricardosun   (501) staff       (20)    11858 2024-04-27 16:12:50.000000 mlops_api_gemstack-0.3.5/mlops_api_gemstack/api.py
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 16:14:36.543370 mlops_api_gemstack-0.3.5/mlops_api_gemstack.egg-info/
--rw-r--r--   0 ricardosun   (501) staff       (20)     4206 2024-04-27 16:14:36.000000 mlops_api_gemstack-0.3.5/mlops_api_gemstack.egg-info/PKG-INFO
--rw-r--r--   0 ricardosun   (501) staff       (20)      337 2024-04-27 16:14:36.000000 mlops_api_gemstack-0.3.5/mlops_api_gemstack.egg-info/SOURCES.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)        1 2024-04-27 16:14:36.000000 mlops_api_gemstack-0.3.5/mlops_api_gemstack.egg-info/dependency_links.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       50 2024-04-27 16:14:36.000000 mlops_api_gemstack-0.3.5/mlops_api_gemstack.egg-info/entry_points.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       37 2024-04-27 16:14:36.000000 mlops_api_gemstack-0.3.5/mlops_api_gemstack.egg-info/requires.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       19 2024-04-27 16:14:36.000000 mlops_api_gemstack-0.3.5/mlops_api_gemstack.egg-info/top_level.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       38 2024-04-27 16:14:36.545733 mlops_api_gemstack-0.3.5/setup.cfg
--rw-r--r--   0 ricardosun   (501) staff       (20)      770 2024-04-27 16:13:00.000000 mlops_api_gemstack-0.3.5/setup.py
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 16:20:42.213467 mlops_api_gemstack-0.3.6/
+-rw-r--r--   0 ricardosun   (501) staff       (20)     1071 2024-04-22 05:08:20.000000 mlops_api_gemstack-0.3.6/LICENSE
+-rw-r--r--   0 ricardosun   (501) staff       (20)     4206 2024-04-27 16:20:42.207017 mlops_api_gemstack-0.3.6/PKG-INFO
+-rw-r--r--   0 ricardosun   (501) staff       (20)     3807 2024-04-23 07:20:14.000000 mlops_api_gemstack-0.3.6/README.md
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 16:20:42.198870 mlops_api_gemstack-0.3.6/mlops_api_gemstack/
+-rw-r--r--   0 ricardosun   (501) staff       (20)       18 2024-04-20 05:10:06.000000 mlops_api_gemstack-0.3.6/mlops_api_gemstack/__init__.py
+-rw-r--r--   0 ricardosun   (501) staff       (20)    11998 2024-04-27 16:19:50.000000 mlops_api_gemstack-0.3.6/mlops_api_gemstack/api.py
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 16:20:42.205525 mlops_api_gemstack-0.3.6/mlops_api_gemstack.egg-info/
+-rw-r--r--   0 ricardosun   (501) staff       (20)     4206 2024-04-27 16:20:42.000000 mlops_api_gemstack-0.3.6/mlops_api_gemstack.egg-info/PKG-INFO
+-rw-r--r--   0 ricardosun   (501) staff       (20)      337 2024-04-27 16:20:42.000000 mlops_api_gemstack-0.3.6/mlops_api_gemstack.egg-info/SOURCES.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)        1 2024-04-27 16:20:42.000000 mlops_api_gemstack-0.3.6/mlops_api_gemstack.egg-info/dependency_links.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       50 2024-04-27 16:20:42.000000 mlops_api_gemstack-0.3.6/mlops_api_gemstack.egg-info/entry_points.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       37 2024-04-27 16:20:42.000000 mlops_api_gemstack-0.3.6/mlops_api_gemstack.egg-info/requires.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       19 2024-04-27 16:20:42.000000 mlops_api_gemstack-0.3.6/mlops_api_gemstack.egg-info/top_level.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       38 2024-04-27 16:20:42.213663 mlops_api_gemstack-0.3.6/setup.cfg
+-rw-r--r--   0 ricardosun   (501) staff       (20)      770 2024-04-27 16:20:38.000000 mlops_api_gemstack-0.3.6/setup.py
```

### Comparing `mlops_api_gemstack-0.3.5/LICENSE` & `mlops_api_gemstack-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mlops_api_gemstack-0.3.5/PKG-INFO` & `mlops_api_gemstack-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlops_api_gemstack
-Version: 0.3.5
+Version: 0.3.6
 Summary: An API package connect to a MLops server relating to the GEMstack project.
 Home-page: https://github.com/krishauser/GEMstack/tree/s2024_MLops/MLops/mlops_api_gemstack
 Author: Haoming Sun
 Author-email: ricardosun990122@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `mlops_api_gemstack-0.3.5/README.md` & `mlops_api_gemstack-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `mlops_api_gemstack-0.3.5/mlops_api_gemstack/api.py` & `mlops_api_gemstack-0.3.6/mlops_api_gemstack/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import time
 import requests
 import click
 import os
 import subprocess
 import signal
 import sys
 from tqdm import tqdm
@@ -281,17 +282,22 @@
 
     def stop_recording(sig, frame):
         print("Stopping rosbag recording")
         process.terminate()
         print("Recording stopped")
 
         pwd = os.getcwd()
+        print(f"Current working directory: {pwd}")
         path = os.path.join(pwd, rosbag_file_name)
+        print(f"Recording saved at: {path}")
+
+        time.sleep(5)
 
         # send rosbag file through api
+        
         upload_bag(path, source)
        
         if delete_rosbag:
             print("Removing rosbag file")
             subprocess.run(f"rm {rosbag_file_name}", shell=True)
         exit(0)
```

### Comparing `mlops_api_gemstack-0.3.5/mlops_api_gemstack.egg-info/PKG-INFO` & `mlops_api_gemstack-0.3.6/mlops_api_gemstack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlops-api-gemstack
-Version: 0.3.5
+Version: 0.3.6
 Summary: An API package connect to a MLops server relating to the GEMstack project.
 Home-page: https://github.com/krishauser/GEMstack/tree/s2024_MLops/MLops/mlops_api_gemstack
 Author: Haoming Sun
 Author-email: ricardosun990122@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `mlops_api_gemstack-0.3.5/setup.py` & `mlops_api_gemstack-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     description = f.read()
 
 setup(
     name='mlops_api_gemstack',
-    version='0.3.5',
+    version='0.3.6',
     description='An API package connect to a MLops server relating to the GEMstack project.',
     author='Haoming Sun',
     author_email='ricardosun990122@gmail.com',
     url='https://github.com/krishauser/GEMstack/tree/s2024_MLops/MLops/mlops_api_gemstack',
     packages=find_packages(),
     install_requires=[
         'requests',
```
