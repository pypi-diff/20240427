# Comparing `tmp/mlops_api_gemstack-0.3.8.tar.gz` & `tmp/mlops_api_gemstack-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlops_api_gemstack-0.3.8.tar", last modified: Sat Apr 27 16:58:54 2024, max compression
+gzip compressed data, was "mlops_api_gemstack-0.3.9.tar", last modified: Sat Apr 27 17:06:28 2024, max compression
```

## Comparing `mlops_api_gemstack-0.3.8.tar` & `mlops_api_gemstack-0.3.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 16:58:54.771034 mlops_api_gemstack-0.3.8/
--rw-r--r--   0 ricardosun   (501) staff       (20)     1071 2024-04-22 05:08:20.000000 mlops_api_gemstack-0.3.8/LICENSE
--rw-r--r--   0 ricardosun   (501) staff       (20)     4206 2024-04-27 16:58:54.770347 mlops_api_gemstack-0.3.8/PKG-INFO
--rw-r--r--   0 ricardosun   (501) staff       (20)     3807 2024-04-23 07:20:14.000000 mlops_api_gemstack-0.3.8/README.md
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 16:58:54.764213 mlops_api_gemstack-0.3.8/mlops_api_gemstack/
--rw-r--r--   0 ricardosun   (501) staff       (20)       18 2024-04-20 05:10:06.000000 mlops_api_gemstack-0.3.8/mlops_api_gemstack/__init__.py
--rw-r--r--   0 ricardosun   (501) staff       (20)    12224 2024-04-27 16:57:47.000000 mlops_api_gemstack-0.3.8/mlops_api_gemstack/api.py
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 16:58:54.769400 mlops_api_gemstack-0.3.8/mlops_api_gemstack.egg-info/
--rw-r--r--   0 ricardosun   (501) staff       (20)     4206 2024-04-27 16:58:54.000000 mlops_api_gemstack-0.3.8/mlops_api_gemstack.egg-info/PKG-INFO
--rw-r--r--   0 ricardosun   (501) staff       (20)      337 2024-04-27 16:58:54.000000 mlops_api_gemstack-0.3.8/mlops_api_gemstack.egg-info/SOURCES.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)        1 2024-04-27 16:58:54.000000 mlops_api_gemstack-0.3.8/mlops_api_gemstack.egg-info/dependency_links.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       50 2024-04-27 16:58:54.000000 mlops_api_gemstack-0.3.8/mlops_api_gemstack.egg-info/entry_points.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       42 2024-04-27 16:58:54.000000 mlops_api_gemstack-0.3.8/mlops_api_gemstack.egg-info/requires.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       19 2024-04-27 16:58:54.000000 mlops_api_gemstack-0.3.8/mlops_api_gemstack.egg-info/top_level.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       38 2024-04-27 16:58:54.771288 mlops_api_gemstack-0.3.8/setup.cfg
--rw-r--r--   0 ricardosun   (501) staff       (20)      786 2024-04-27 16:58:48.000000 mlops_api_gemstack-0.3.8/setup.py
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 17:06:28.824855 mlops_api_gemstack-0.3.9/
+-rw-r--r--   0 ricardosun   (501) staff       (20)     1071 2024-04-22 05:08:20.000000 mlops_api_gemstack-0.3.9/LICENSE
+-rw-r--r--   0 ricardosun   (501) staff       (20)     4206 2024-04-27 17:06:28.824211 mlops_api_gemstack-0.3.9/PKG-INFO
+-rw-r--r--   0 ricardosun   (501) staff       (20)     3807 2024-04-23 07:20:14.000000 mlops_api_gemstack-0.3.9/README.md
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 17:06:28.814924 mlops_api_gemstack-0.3.9/mlops_api_gemstack/
+-rw-r--r--   0 ricardosun   (501) staff       (20)       18 2024-04-20 05:10:06.000000 mlops_api_gemstack-0.3.9/mlops_api_gemstack/__init__.py
+-rw-r--r--   0 ricardosun   (501) staff       (20)    12224 2024-04-27 17:06:20.000000 mlops_api_gemstack-0.3.9/mlops_api_gemstack/api.py
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 17:06:28.823366 mlops_api_gemstack-0.3.9/mlops_api_gemstack.egg-info/
+-rw-r--r--   0 ricardosun   (501) staff       (20)     4206 2024-04-27 17:06:28.000000 mlops_api_gemstack-0.3.9/mlops_api_gemstack.egg-info/PKG-INFO
+-rw-r--r--   0 ricardosun   (501) staff       (20)      337 2024-04-27 17:06:28.000000 mlops_api_gemstack-0.3.9/mlops_api_gemstack.egg-info/SOURCES.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)        1 2024-04-27 17:06:28.000000 mlops_api_gemstack-0.3.9/mlops_api_gemstack.egg-info/dependency_links.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       50 2024-04-27 17:06:28.000000 mlops_api_gemstack-0.3.9/mlops_api_gemstack.egg-info/entry_points.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       37 2024-04-27 17:06:28.000000 mlops_api_gemstack-0.3.9/mlops_api_gemstack.egg-info/requires.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       19 2024-04-27 17:06:28.000000 mlops_api_gemstack-0.3.9/mlops_api_gemstack.egg-info/top_level.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       38 2024-04-27 17:06:28.825109 mlops_api_gemstack-0.3.9/setup.cfg
+-rw-r--r--   0 ricardosun   (501) staff       (20)      770 2024-04-27 17:06:14.000000 mlops_api_gemstack-0.3.9/setup.py
```

### Comparing `mlops_api_gemstack-0.3.8/LICENSE` & `mlops_api_gemstack-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mlops_api_gemstack-0.3.8/PKG-INFO` & `mlops_api_gemstack-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlops_api_gemstack
-Version: 0.3.8
+Version: 0.3.9
 Summary: An API package connect to a MLops server relating to the GEMstack project.
 Home-page: https://github.com/krishauser/GEMstack/tree/s2024_MLops/MLops/mlops_api_gemstack
 Author: Haoming Sun
 Author-email: ricardosun990122@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `mlops_api_gemstack-0.3.8/README.md` & `mlops_api_gemstack-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `mlops_api_gemstack-0.3.8/mlops_api_gemstack/api.py` & `mlops_api_gemstack-0.3.9/mlops_api_gemstack/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,16 +289,16 @@
         print(f"Recording saved at: {path}")
 
         time.sleep(2)
 
         # check connection
         net = "IllinoisNet"
         while(subprocess.check_output("iwgetid -r", shell=True).decode().strip() != net):
-            print("Not connected to IllinoisNet. Retrying in 1 second")
-            time.sleep(1)
+            print("Not connected to IllinoisNet. Retrying in 5 second")
+            time.sleep(5)
 
         # send rosbag file through api
         print("Uploading rosbag file")
         upload_bag(path, source)
        
         if delete_rosbag:
             print("Removing rosbag file")
```

### Comparing `mlops_api_gemstack-0.3.8/mlops_api_gemstack.egg-info/PKG-INFO` & `mlops_api_gemstack-0.3.9/mlops_api_gemstack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlops-api-gemstack
-Version: 0.3.8
+Version: 0.3.9
 Summary: An API package connect to a MLops server relating to the GEMstack project.
 Home-page: https://github.com/krishauser/GEMstack/tree/s2024_MLops/MLops/mlops_api_gemstack
 Author: Haoming Sun
 Author-email: ricardosun990122@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `mlops_api_gemstack-0.3.8/setup.py` & `mlops_api_gemstack-0.3.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     description = f.read()
 
 setup(
     name='mlops_api_gemstack',
-    version='0.3.8',
+    version='0.3.9',
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
-        'click',
-        'time'
+        'click'
     ],
     entry_points={
         'console_scripts': [
             'mlops=mlops_api_gemstack:cli'
         ]
     },
     long_description=description,
```

