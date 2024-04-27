# Comparing `tmp/mlops_api_gemstack-0.3.7.tar.gz` & `tmp/mlops_api_gemstack-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlops_api_gemstack-0.3.7.tar", last modified: Sat Apr 27 16:49:14 2024, max compression
+gzip compressed data, was "mlops_api_gemstack-0.3.8.tar", last modified: Sat Apr 27 16:58:54 2024, max compression
```

## Comparing `mlops_api_gemstack-0.3.7.tar` & `mlops_api_gemstack-0.3.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 16:49:14.388461 mlops_api_gemstack-0.3.7/
--rw-r--r--   0 ricardosun   (501) staff       (20)     1071 2024-04-22 05:08:20.000000 mlops_api_gemstack-0.3.7/LICENSE
--rw-r--r--   0 ricardosun   (501) staff       (20)     4206 2024-04-27 16:49:14.387557 mlops_api_gemstack-0.3.7/PKG-INFO
--rw-r--r--   0 ricardosun   (501) staff       (20)     3807 2024-04-23 07:20:14.000000 mlops_api_gemstack-0.3.7/README.md
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 16:49:14.365920 mlops_api_gemstack-0.3.7/mlops_api_gemstack/
--rw-r--r--   0 ricardosun   (501) staff       (20)       18 2024-04-20 05:10:06.000000 mlops_api_gemstack-0.3.7/mlops_api_gemstack/__init__.py
--rw-r--r--   0 ricardosun   (501) staff       (20)    12233 2024-04-27 16:49:02.000000 mlops_api_gemstack-0.3.7/mlops_api_gemstack/api.py
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 16:49:14.378346 mlops_api_gemstack-0.3.7/mlops_api_gemstack.egg-info/
--rw-r--r--   0 ricardosun   (501) staff       (20)     4206 2024-04-27 16:49:14.000000 mlops_api_gemstack-0.3.7/mlops_api_gemstack.egg-info/PKG-INFO
--rw-r--r--   0 ricardosun   (501) staff       (20)      337 2024-04-27 16:49:14.000000 mlops_api_gemstack-0.3.7/mlops_api_gemstack.egg-info/SOURCES.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)        1 2024-04-27 16:49:14.000000 mlops_api_gemstack-0.3.7/mlops_api_gemstack.egg-info/dependency_links.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       50 2024-04-27 16:49:14.000000 mlops_api_gemstack-0.3.7/mlops_api_gemstack.egg-info/entry_points.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       37 2024-04-27 16:49:14.000000 mlops_api_gemstack-0.3.7/mlops_api_gemstack.egg-info/requires.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       19 2024-04-27 16:49:14.000000 mlops_api_gemstack-0.3.7/mlops_api_gemstack.egg-info/top_level.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       38 2024-04-27 16:49:14.388728 mlops_api_gemstack-0.3.7/setup.cfg
--rw-r--r--   0 ricardosun   (501) staff       (20)      770 2024-04-27 16:49:10.000000 mlops_api_gemstack-0.3.7/setup.py
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 16:58:54.771034 mlops_api_gemstack-0.3.8/
+-rw-r--r--   0 ricardosun   (501) staff       (20)     1071 2024-04-22 05:08:20.000000 mlops_api_gemstack-0.3.8/LICENSE
+-rw-r--r--   0 ricardosun   (501) staff       (20)     4206 2024-04-27 16:58:54.770347 mlops_api_gemstack-0.3.8/PKG-INFO
+-rw-r--r--   0 ricardosun   (501) staff       (20)     3807 2024-04-23 07:20:14.000000 mlops_api_gemstack-0.3.8/README.md
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 16:58:54.764213 mlops_api_gemstack-0.3.8/mlops_api_gemstack/
+-rw-r--r--   0 ricardosun   (501) staff       (20)       18 2024-04-20 05:10:06.000000 mlops_api_gemstack-0.3.8/mlops_api_gemstack/__init__.py
+-rw-r--r--   0 ricardosun   (501) staff       (20)    12224 2024-04-27 16:57:47.000000 mlops_api_gemstack-0.3.8/mlops_api_gemstack/api.py
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 16:58:54.769400 mlops_api_gemstack-0.3.8/mlops_api_gemstack.egg-info/
+-rw-r--r--   0 ricardosun   (501) staff       (20)     4206 2024-04-27 16:58:54.000000 mlops_api_gemstack-0.3.8/mlops_api_gemstack.egg-info/PKG-INFO
+-rw-r--r--   0 ricardosun   (501) staff       (20)      337 2024-04-27 16:58:54.000000 mlops_api_gemstack-0.3.8/mlops_api_gemstack.egg-info/SOURCES.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)        1 2024-04-27 16:58:54.000000 mlops_api_gemstack-0.3.8/mlops_api_gemstack.egg-info/dependency_links.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       50 2024-04-27 16:58:54.000000 mlops_api_gemstack-0.3.8/mlops_api_gemstack.egg-info/entry_points.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       42 2024-04-27 16:58:54.000000 mlops_api_gemstack-0.3.8/mlops_api_gemstack.egg-info/requires.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       19 2024-04-27 16:58:54.000000 mlops_api_gemstack-0.3.8/mlops_api_gemstack.egg-info/top_level.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       38 2024-04-27 16:58:54.771288 mlops_api_gemstack-0.3.8/setup.cfg
+-rw-r--r--   0 ricardosun   (501) staff       (20)      786 2024-04-27 16:58:48.000000 mlops_api_gemstack-0.3.8/setup.py
```

### Comparing `mlops_api_gemstack-0.3.7/LICENSE` & `mlops_api_gemstack-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mlops_api_gemstack-0.3.7/PKG-INFO` & `mlops_api_gemstack-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlops_api_gemstack
-Version: 0.3.7
+Version: 0.3.8
 Summary: An API package connect to a MLops server relating to the GEMstack project.
 Home-page: https://github.com/krishauser/GEMstack/tree/s2024_MLops/MLops/mlops_api_gemstack
 Author: Haoming Sun
 Author-email: ricardosun990122@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `mlops_api_gemstack-0.3.7/README.md` & `mlops_api_gemstack-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `mlops_api_gemstack-0.3.7/mlops_api_gemstack/api.py` & `mlops_api_gemstack-0.3.8/mlops_api_gemstack/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import time
 import requests
 import click
 import os
 import subprocess
 import signal
-import sys
 from tqdm import tqdm
 from pprint import pprint
 from urllib.parse import unquote
 
 base_url='http://10.195.159.3:5000'
 save_directory = os.getcwd()
 
@@ -257,15 +256,15 @@
         else:
             click.echo(f"Failed to upload the file. Status code: {response.status_code}")
 
 @cli.command()
 @click.argument('topics_file', type=click.Path(exists=True))
 @click.argument('rosbag_file_name')
 @click.argument('source')
-@click.option('--delete_rosbag', is_flag=True, default=False, help='Keep the rosbag file after recording')
+@click.option('--delete_rosbag', is_flag=True, default=True, help='Keep the rosbag file after recording')
 def record_rosbag(topics_file, rosbag_file_name, source, delete_rosbag):
 
     with open(topics_file) as f:
         topics = [line.strip() for line in f.readlines()]
 
     if not topics:
         print(f"No topics found in {topics_file}")
@@ -289,15 +288,15 @@
         path = os.path.join(pwd, rosbag_file_name)
         print(f"Recording saved at: {path}")
 
         time.sleep(2)
 
         # check connection
         net = "IllinoisNet"
-        while(process.check_output("iwgetid -r", shell=True).decode().strip() != net):
+        while(subprocess.check_output("iwgetid -r", shell=True).decode().strip() != net):
             print("Not connected to IllinoisNet. Retrying in 1 second")
             time.sleep(1)
 
         # send rosbag file through api
         print("Uploading rosbag file")
         upload_bag(path, source)
```

### Comparing `mlops_api_gemstack-0.3.7/mlops_api_gemstack.egg-info/PKG-INFO` & `mlops_api_gemstack-0.3.8/mlops_api_gemstack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlops-api-gemstack
-Version: 0.3.7
+Version: 0.3.8
 Summary: An API package connect to a MLops server relating to the GEMstack project.
 Home-page: https://github.com/krishauser/GEMstack/tree/s2024_MLops/MLops/mlops_api_gemstack
 Author: Haoming Sun
 Author-email: ricardosun990122@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `mlops_api_gemstack-0.3.7/setup.py` & `mlops_api_gemstack-0.3.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     description = f.read()
 
 setup(
     name='mlops_api_gemstack',
-    version='0.3.7',
+    version='0.3.8',
     description='An API package connect to a MLops server relating to the GEMstack project.',
     author='Haoming Sun',
     author_email='ricardosun990122@gmail.com',
     url='https://github.com/krishauser/GEMstack/tree/s2024_MLops/MLops/mlops_api_gemstack',
     packages=find_packages(),
     install_requires=[
         'requests',
         'tqdm',
         'pprintpp',
         'urllib3',
-        'click'
+        'click',
+        'time'
     ],
     entry_points={
         'console_scripts': [
             'mlops=mlops_api_gemstack:cli'
         ]
     },
     long_description=description,
```

