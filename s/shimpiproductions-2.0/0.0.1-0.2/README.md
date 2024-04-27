# Comparing `tmp/shimpiproductions-2.0-0.0.1.tar.gz` & `tmp/shimpiproductions-2.0-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shimpiproductions-2.0-0.0.1.tar", last modified: Sat Apr 27 11:22:40 2024, max compression
+gzip compressed data, was "shimpiproductions-2.0-0.2.tar", last modified: Sat Apr 27 11:48:00 2024, max compression
```

## Comparing `shimpiproductions-2.0-0.0.1.tar` & `shimpiproductions-2.0-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 11:22:40.179824 shimpiproductions-2.0-0.0.1/
--rw-rw-rw-   0        0        0     1078 2024-04-27 10:14:02.000000 shimpiproductions-2.0-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      691 2024-04-27 11:22:40.171829 shimpiproductions-2.0-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     8101 2024-04-27 10:00:51.000000 shimpiproductions-2.0-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 11:22:40.131850 shimpiproductions-2.0-0.0.1/lib/
--rw-rw-rw-   0        0        0        0 2024-04-27 11:13:32.000000 shimpiproductions-2.0-0.0.1/lib/__init__.py
--rw-rw-rw-   0        0        0     8095 2024-04-27 09:56:23.000000 shimpiproductions-2.0-0.0.1/lib/main.py
--rw-rw-rw-   0        0        0       42 2024-04-27 11:22:40.180822 shimpiproductions-2.0-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      977 2024-04-27 11:22:35.000000 shimpiproductions-2.0-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:22:40.166830 shimpiproductions-2.0-0.0.1/shimpiproductions_2.0.egg-info/
--rw-rw-rw-   0        0        0      691 2024-04-27 11:22:39.000000 shimpiproductions-2.0-0.0.1/shimpiproductions_2.0.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2024-04-27 11:22:39.000000 shimpiproductions-2.0-0.0.1/shimpiproductions_2.0.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 11:22:39.000000 shimpiproductions-2.0-0.0.1/shimpiproductions_2.0.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-27 11:22:39.000000 shimpiproductions-2.0-0.0.1/shimpiproductions_2.0.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       62 2024-04-27 11:22:39.000000 shimpiproductions-2.0-0.0.1/shimpiproductions_2.0.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-27 11:22:39.000000 shimpiproductions-2.0-0.0.1/shimpiproductions_2.0.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 11:48:00.220637 shimpiproductions-2.0-0.2/
+-rw-rw-rw-   0        0        0     1078 2024-04-27 10:14:02.000000 shimpiproductions-2.0-0.2/LICENSE
+-rw-rw-rw-   0        0        0     8808 2024-04-27 11:48:00.212642 shimpiproductions-2.0-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8101 2024-04-27 10:00:51.000000 shimpiproductions-2.0-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 11:48:00.176684 shimpiproductions-2.0-0.2/lib/
+-rw-rw-rw-   0        0        0        0 2024-04-27 11:13:32.000000 shimpiproductions-2.0-0.2/lib/__init__.py
+-rw-rw-rw-   0        0        0     8095 2024-04-27 09:56:23.000000 shimpiproductions-2.0-0.2/lib/main.py
+-rw-rw-rw-   0        0        0       42 2024-04-27 11:48:00.221637 shimpiproductions-2.0-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      994 2024-04-27 11:47:55.000000 shimpiproductions-2.0-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:48:00.207645 shimpiproductions-2.0-0.2/shimpiproductions_2.0.egg-info/
+-rw-rw-rw-   0        0        0     8808 2024-04-27 11:47:59.000000 shimpiproductions-2.0-0.2/shimpiproductions_2.0.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2024-04-27 11:47:59.000000 shimpiproductions-2.0-0.2/shimpiproductions_2.0.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 11:47:59.000000 shimpiproductions-2.0-0.2/shimpiproductions_2.0.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-27 11:47:59.000000 shimpiproductions-2.0-0.2/shimpiproductions_2.0.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       62 2024-04-27 11:47:59.000000 shimpiproductions-2.0-0.2/shimpiproductions_2.0.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-27 11:47:59.000000 shimpiproductions-2.0-0.2/shimpiproductions_2.0.egg-info/top_level.txt
```

### Comparing `shimpiproductions-2.0-0.0.1/LICENSE` & `shimpiproductions-2.0-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shimpiproductions-2.0-0.0.1/README.md` & `shimpiproductions-2.0-0.2/README.md`

 * *Files identical despite different names*

### Comparing `shimpiproductions-2.0-0.0.1/lib/main.py` & `shimpiproductions-2.0-0.2/lib/main.py`

 * *Files identical despite different names*

### Comparing `shimpiproductions-2.0-0.0.1/setup.py` & `shimpiproductions-2.0-0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 from setuptools import setup, find_packages
-import codecs
-import os
 
+with open("README.md", 'r') as f:
+    DESCRIPTION = f.read()
 
+VERSION = '0.2'
 
-VERSION = '0.0.1'
-DESCRIPTION = 'CODING MADE EASY'
-
-
-# Setting up
 setup(
     name="shimpiproductions-2.0",
     version=VERSION,
     author="Sarvesh Shimpi",
     author_email="sarveshshimpi18@gmail.com",
-    description=DESCRIPTION,
-    
+    long_description=DESCRIPTION,
+    long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=['numpy', 'matplotlib', 'scikit-learn', 'opencv-python', 'pyautogui', 'pyaudio'],
     keywords=['python', 'video', 'stream', 'video stream', 'camera stream', 'sockets'],
-    entry_points={"console_scripts":[
-        "shimpi=shimpi:hi",
-    ],
-                  
-                  },
+    entry_points={
+        "console_scripts": [
+            "shimpi=shimpi:hi",
+        ],
+    },
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
-
```

