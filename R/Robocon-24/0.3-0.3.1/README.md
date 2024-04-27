# Comparing `tmp/Robocon_24-0.3.tar.gz` & `tmp/Robocon_24-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Robocon_24-0.3.tar", last modified: Sat Apr 27 20:05:42 2024, max compression
+gzip compressed data, was "Robocon_24-0.3.1.tar", last modified: Sat Apr 27 20:18:29 2024, max compression
```

## Comparing `Robocon_24-0.3.tar` & `Robocon_24-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 20:05:42.965884 Robocon_24-0.3/
--rw-rw-rw-   0        0        0     1092 2024-04-11 16:42:04.000000 Robocon_24-0.3/LICENSE
--rw-rw-rw-   0        0        0     2879 2024-04-27 20:05:42.965884 Robocon_24-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1610 2024-04-11 16:47:32.000000 Robocon_24-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 20:05:42.933592 Robocon_24-0.3/Robocon_24/
--rw-rw-rw-   0        0        0     5031 2024-04-11 14:54:25.000000 Robocon_24-0.3/Robocon_24/Robocon_24.py
--rw-rw-rw-   0        0        0       82 2024-04-27 19:50:44.000000 Robocon_24-0.3/Robocon_24/__init__.py
--rw-rw-rw-   0        0        0      239 2024-04-27 19:55:37.000000 Robocon_24-0.3/Robocon_24/ball_detection.py
-drwxrwxrwx   0        0        0        0 2024-04-27 20:05:42.965884 Robocon_24-0.3/Robocon_24.egg-info/
--rw-rw-rw-   0        0        0     2879 2024-04-27 20:05:42.000000 Robocon_24-0.3/Robocon_24.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-04-27 20:05:42.000000 Robocon_24-0.3/Robocon_24.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 20:05:42.000000 Robocon_24-0.3/Robocon_24.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-27 20:05:42.000000 Robocon_24-0.3/Robocon_24.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-27 20:05:42.000000 Robocon_24-0.3/Robocon_24.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 20:05:42.970964 Robocon_24-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1922 2024-04-27 20:01:46.000000 Robocon_24-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 20:18:29.481308 Robocon_24-0.3.1/
+-rw-rw-rw-   0        0        0     1092 2024-04-11 16:42:04.000000 Robocon_24-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     2881 2024-04-27 20:18:29.481308 Robocon_24-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1610 2024-04-11 16:47:32.000000 Robocon_24-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 20:18:29.446245 Robocon_24-0.3.1/Robocon_24/
+-rw-rw-rw-   0        0        0     5029 2024-04-27 20:16:08.000000 Robocon_24-0.3.1/Robocon_24/Robocon_24.py
+-rw-rw-rw-   0        0        0       82 2024-04-27 19:50:44.000000 Robocon_24-0.3.1/Robocon_24/__init__.py
+-rw-rw-rw-   0        0        0      237 2024-04-27 20:16:15.000000 Robocon_24-0.3.1/Robocon_24/ball_detection.py
+drwxrwxrwx   0        0        0        0 2024-04-27 20:18:29.479585 Robocon_24-0.3.1/Robocon_24.egg-info/
+-rw-rw-rw-   0        0        0     2881 2024-04-27 20:18:29.000000 Robocon_24-0.3.1/Robocon_24.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-04-27 20:18:29.000000 Robocon_24-0.3.1/Robocon_24.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 20:18:29.000000 Robocon_24-0.3.1/Robocon_24.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-27 20:18:29.000000 Robocon_24-0.3.1/Robocon_24.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-27 20:18:29.000000 Robocon_24-0.3.1/Robocon_24.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 20:18:29.481308 Robocon_24-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1924 2024-04-27 20:17:15.000000 Robocon_24-0.3.1/setup.py
```

### Comparing `Robocon_24-0.3/LICENSE` & `Robocon_24-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Robocon_24-0.3/PKG-INFO` & `Robocon_24-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Robocon_24
-Version: 0.3
+Version: 0.3.1
 Summary: This project is designed to detect balls and make decisions based on their positions in the context of a Robocon competition.
 Home-page: https://github.com/mariswarycharan/Robocon_24_version
 Author: Charan A A
 Author-email: mariswarycharan@gmail.com
 Project-URL: Homepage, https://github.com/mariswarycharan/Robocon_24_version
 Project-URL: Download, https://github.com/mariswarycharan/Robocon_24_version.git
 Project-URL: Documentation, https://github.com/mariswarycharan/Robocon_24_version/blob/main/README.md
```

### Comparing `Robocon_24-0.3/README.md` & `Robocon_24-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `Robocon_24-0.3/Robocon_24/Robocon_24.py` & `Robocon_24-0.3.1/Robocon_24/Robocon_24.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ultralytics import YOLO
 import cv2
 
-model = YOLO(r"models\best_2.pt")
+model = YOLO(r"models\best.pt")
 
 def point_inside(rectangle, entire_coordinates):    
     x1, y1 ,x2, y2 , _ , _ = rectangle
     return (entire_coordinates[0] <= x1 <= entire_coordinates[2] and entire_coordinates[1] <= y1 <= entire_coordinates[3]) or (entire_coordinates[0] <= x2 <= entire_coordinates[2] and entire_coordinates[1] <= y2 <= entire_coordinates[3])
 
 def decision_maker(image_input_def):
     global model
```

### Comparing `Robocon_24-0.3/Robocon_24.egg-info/PKG-INFO` & `Robocon_24-0.3.1/Robocon_24.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Robocon-24
-Version: 0.3
+Version: 0.3.1
 Summary: This project is designed to detect balls and make decisions based on their positions in the context of a Robocon competition.
 Home-page: https://github.com/mariswarycharan/Robocon_24_version
 Author: Charan A A
 Author-email: mariswarycharan@gmail.com
 Project-URL: Homepage, https://github.com/mariswarycharan/Robocon_24_version
 Project-URL: Download, https://github.com/mariswarycharan/Robocon_24_version.git
 Project-URL: Documentation, https://github.com/mariswarycharan/Robocon_24_version/blob/main/README.md
```

### Comparing `Robocon_24-0.3/setup.py` & `Robocon_24-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='Robocon_24',
-    version='0.3',
+    version='0.3.1',
     author='Charan A A',
     author_email='mariswarycharan@gmail.com',
     description='This project is designed to detect balls and make decisions based on their positions in the context of a Robocon competition.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/mariswarycharan/Robocon_24_version',  # Update with your GitHub repository URL
     packages=find_packages(),
```

