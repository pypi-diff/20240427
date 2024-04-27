# Comparing `tmp/Robocon_24-0.2.tar.gz` & `tmp/Robocon_24-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Robocon_24-0.2.tar", last modified: Tue Apr 23 07:46:52 2024, max compression
+gzip compressed data, was "Robocon_24-0.3.tar", last modified: Sat Apr 27 20:05:42 2024, max compression
```

## Comparing `Robocon_24-0.2.tar` & `Robocon_24-0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 07:46:52.822558 Robocon_24-0.2/
--rw-rw-rw-   0        0        0     1092 2024-04-11 16:42:04.000000 Robocon_24-0.2/LICENSE
--rw-rw-rw-   0        0        0     2358 2024-04-23 07:46:52.817964 Robocon_24-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1610 2024-04-11 16:47:32.000000 Robocon_24-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 07:46:52.789665 Robocon_24-0.2/Robocon_24/
--rw-rw-rw-   0        0        0     5031 2024-04-11 14:54:25.000000 Robocon_24-0.2/Robocon_24/Robocon_24.py
--rw-rw-rw-   0        0        0       38 2024-04-11 18:15:36.000000 Robocon_24-0.2/Robocon_24/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:46:52.817964 Robocon_24-0.2/Robocon_24.egg-info/
--rw-rw-rw-   0        0        0     2358 2024-04-23 07:46:52.000000 Robocon_24-0.2/Robocon_24.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2024-04-23 07:46:52.000000 Robocon_24-0.2/Robocon_24.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 07:46:52.000000 Robocon_24-0.2/Robocon_24.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-23 07:46:52.000000 Robocon_24-0.2/Robocon_24.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-23 07:46:52.000000 Robocon_24-0.2/Robocon_24.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 07:46:52.825241 Robocon_24-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1144 2024-04-23 07:46:04.000000 Robocon_24-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 20:05:42.965884 Robocon_24-0.3/
+-rw-rw-rw-   0        0        0     1092 2024-04-11 16:42:04.000000 Robocon_24-0.3/LICENSE
+-rw-rw-rw-   0        0        0     2879 2024-04-27 20:05:42.965884 Robocon_24-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1610 2024-04-11 16:47:32.000000 Robocon_24-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 20:05:42.933592 Robocon_24-0.3/Robocon_24/
+-rw-rw-rw-   0        0        0     5031 2024-04-11 14:54:25.000000 Robocon_24-0.3/Robocon_24/Robocon_24.py
+-rw-rw-rw-   0        0        0       82 2024-04-27 19:50:44.000000 Robocon_24-0.3/Robocon_24/__init__.py
+-rw-rw-rw-   0        0        0      239 2024-04-27 19:55:37.000000 Robocon_24-0.3/Robocon_24/ball_detection.py
+drwxrwxrwx   0        0        0        0 2024-04-27 20:05:42.965884 Robocon_24-0.3/Robocon_24.egg-info/
+-rw-rw-rw-   0        0        0     2879 2024-04-27 20:05:42.000000 Robocon_24-0.3/Robocon_24.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-04-27 20:05:42.000000 Robocon_24-0.3/Robocon_24.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 20:05:42.000000 Robocon_24-0.3/Robocon_24.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-27 20:05:42.000000 Robocon_24-0.3/Robocon_24.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-27 20:05:42.000000 Robocon_24-0.3/Robocon_24.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 20:05:42.970964 Robocon_24-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1922 2024-04-27 20:01:46.000000 Robocon_24-0.3/setup.py
```

### Comparing `Robocon_24-0.2/LICENSE` & `Robocon_24-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Robocon_24-0.2/PKG-INFO` & `Robocon_24-0.3/Robocon_24.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 Metadata-Version: 2.1
-Name: Robocon_24
-Version: 0.2
+Name: Robocon-24
+Version: 0.3
 Summary: This project is designed to detect balls and make decisions based on their positions in the context of a Robocon competition.
 Home-page: https://github.com/mariswarycharan/Robocon_24_version
 Author: Charan A A
 Author-email: mariswarycharan@gmail.com
+Project-URL: Homepage, https://github.com/mariswarycharan/Robocon_24_version
+Project-URL: Download, https://github.com/mariswarycharan/Robocon_24_version.git
+Project-URL: Documentation, https://github.com/mariswarycharan/Robocon_24_version/blob/main/README.md
+Project-URL: Issue tracker, https://github.com/mariswarycharan/Robocon_24_version/issues
+Project-URL: Source code, https://github.com/mariswarycharan/Robocon_24_version
+Project-URL: GitHub Statistics, https://github.com/mariswarycharan/Robocon_24_version
 Keywords: Robocon,Ball,Detection,Decision,Making,Computer Vision,YOLO,Ultralytics,OpenCV,Python,Ball Detection,Ball Decision Making,Robocon 2024,Robocon 24
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: opencv-python
```

### Comparing `Robocon_24-0.2/README.md` & `Robocon_24-0.3/README.md`

 * *Files identical despite different names*

### Comparing `Robocon_24-0.2/Robocon_24/Robocon_24.py` & `Robocon_24-0.3/Robocon_24/Robocon_24.py`

 * *Files identical despite different names*

### Comparing `Robocon_24-0.2/Robocon_24.egg-info/PKG-INFO` & `Robocon_24-0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 Metadata-Version: 2.1
-Name: Robocon-24
-Version: 0.2
+Name: Robocon_24
+Version: 0.3
 Summary: This project is designed to detect balls and make decisions based on their positions in the context of a Robocon competition.
 Home-page: https://github.com/mariswarycharan/Robocon_24_version
 Author: Charan A A
 Author-email: mariswarycharan@gmail.com
+Project-URL: Homepage, https://github.com/mariswarycharan/Robocon_24_version
+Project-URL: Download, https://github.com/mariswarycharan/Robocon_24_version.git
+Project-URL: Documentation, https://github.com/mariswarycharan/Robocon_24_version/blob/main/README.md
+Project-URL: Issue tracker, https://github.com/mariswarycharan/Robocon_24_version/issues
+Project-URL: Source code, https://github.com/mariswarycharan/Robocon_24_version
+Project-URL: GitHub Statistics, https://github.com/mariswarycharan/Robocon_24_version
 Keywords: Robocon,Ball,Detection,Decision,Making,Computer Vision,YOLO,Ultralytics,OpenCV,Python,Ball Detection,Ball Decision Making,Robocon 2024,Robocon 24
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: opencv-python
```

