# Comparing `tmp/MLXpress-0.1.9.0.tar.gz` & `tmp/MLXpress-0.1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLXpress-0.1.9.0.tar", last modified: Sat Apr 27 13:52:38 2024, max compression
+gzip compressed data, was "MLXpress-0.1.9.1.tar", last modified: Sat Apr 27 14:09:57 2024, max compression
```

## Comparing `MLXpress-0.1.9.0.tar` & `MLXpress-0.1.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 vinilg7    (501) staff       (20)        0 2024-04-27 13:52:38.528869 MLXpress-0.1.9.0/
-drwxr-xr-x   0 vinilg7    (501) staff       (20)        0 2024-04-27 13:52:38.527162 MLXpress-0.1.9.0/MLXpress/
--rw-rw-r--   0 vinilg7    (501) staff       (20)        0 2023-07-14 01:21:38.000000 MLXpress-0.1.9.0/MLXpress/__init__.py
--rw-r--r--   0 vinilg7    (501) staff       (20)     5478 2023-12-13 11:57:53.000000 MLXpress-0.1.9.0/MLXpress/bigdata.py
--rw-rw-r--   0 vinilg7    (501) staff       (20)     2338 2023-07-16 23:45:14.000000 MLXpress-0.1.9.0/MLXpress/diabetes.py
--rw-r--r--   0 vinilg7    (501) staff       (20)     6232 2024-04-14 12:01:28.000000 MLXpress-0.1.9.0/MLXpress/getdata.py
--rw-r--r--   0 vinilg7    (501) staff       (20)     3360 2023-12-14 13:36:32.000000 MLXpress-0.1.9.0/MLXpress/help.py
--rw-rw-r--   0 vinilg7    (501) staff       (20)     4011 2023-07-17 06:11:02.000000 MLXpress-0.1.9.0/MLXpress/iris.py
--rw-r--r--   0 vinilg7    (501) staff       (20)     3240 2023-12-13 09:58:20.000000 MLXpress-0.1.9.0/MLXpress/math.py
--rw-r--r--   0 vinilg7    (501) staff       (20)    28135 2023-12-13 09:58:20.000000 MLXpress-0.1.9.0/MLXpress/ml.py
--rw-rw-r--   0 vinilg7    (501) staff       (20)     5030 2023-07-17 05:03:38.000000 MLXpress-0.1.9.0/MLXpress/preprocessing.py
--rw-rw-r--   0 vinilg7    (501) staff       (20)     1870 2023-07-17 05:24:56.000000 MLXpress-0.1.9.0/MLXpress/stats.py
--rw-r--r--   0 vinilg7    (501) staff       (20)    11741 2024-04-27 13:48:43.000000 MLXpress-0.1.9.0/MLXpress/timeSeries.py
--rw-rw-r--   0 vinilg7    (501) staff       (20)     2733 2023-07-17 06:10:32.000000 MLXpress-0.1.9.0/MLXpress/wine.py
-drwxr-xr-x   0 vinilg7    (501) staff       (20)        0 2024-04-27 13:52:38.528196 MLXpress-0.1.9.0/MLXpress.egg-info/
--rw-r--r--   0 vinilg7    (501) staff       (20)     2461 2024-04-27 13:52:38.000000 MLXpress-0.1.9.0/MLXpress.egg-info/PKG-INFO
--rw-r--r--   0 vinilg7    (501) staff       (20)      409 2024-04-27 13:52:38.000000 MLXpress-0.1.9.0/MLXpress.egg-info/SOURCES.txt
--rw-rw-r--   0 vinilg7    (501) staff       (20)        1 2024-04-27 13:52:38.000000 MLXpress-0.1.9.0/MLXpress.egg-info/dependency_links.txt
--rw-rw-r--   0 vinilg7    (501) staff       (20)       97 2024-04-27 13:52:38.000000 MLXpress-0.1.9.0/MLXpress.egg-info/requires.txt
--rw-rw-r--   0 vinilg7    (501) staff       (20)        9 2024-04-27 13:52:38.000000 MLXpress-0.1.9.0/MLXpress.egg-info/top_level.txt
--rw-r--r--   0 vinilg7    (501) staff       (20)     2461 2024-04-27 13:52:38.528617 MLXpress-0.1.9.0/PKG-INFO
--rw-rw-r--   0 vinilg7    (501) staff       (20)     1718 2023-07-16 07:37:28.000000 MLXpress-0.1.9.0/README.md
--rw-r--r--   0 vinilg7    (501) staff       (20)       38 2024-04-27 13:52:38.528921 MLXpress-0.1.9.0/setup.cfg
--rw-r--r--   0 vinilg7    (501) staff       (20)      981 2024-04-27 13:50:40.000000 MLXpress-0.1.9.0/setup.py
+drwxr-xr-x   0 vinilg7    (501) staff       (20)        0 2024-04-27 14:09:57.904996 MLXpress-0.1.9.1/
+drwxr-xr-x   0 vinilg7    (501) staff       (20)        0 2024-04-27 14:09:57.902334 MLXpress-0.1.9.1/MLXpress/
+-rw-rw-r--   0 vinilg7    (501) staff       (20)        0 2023-07-14 01:21:38.000000 MLXpress-0.1.9.1/MLXpress/__init__.py
+-rw-r--r--   0 vinilg7    (501) staff       (20)     5478 2023-12-13 11:57:53.000000 MLXpress-0.1.9.1/MLXpress/bigdata.py
+-rw-rw-r--   0 vinilg7    (501) staff       (20)     2338 2023-07-16 23:45:14.000000 MLXpress-0.1.9.1/MLXpress/diabetes.py
+-rw-r--r--   0 vinilg7    (501) staff       (20)     6232 2024-04-14 12:01:28.000000 MLXpress-0.1.9.1/MLXpress/getdata.py
+-rw-r--r--   0 vinilg7    (501) staff       (20)     3360 2023-12-14 13:36:32.000000 MLXpress-0.1.9.1/MLXpress/help.py
+-rw-rw-r--   0 vinilg7    (501) staff       (20)     4011 2023-07-17 06:11:02.000000 MLXpress-0.1.9.1/MLXpress/iris.py
+-rw-r--r--   0 vinilg7    (501) staff       (20)     3240 2023-12-13 09:58:20.000000 MLXpress-0.1.9.1/MLXpress/math.py
+-rw-r--r--   0 vinilg7    (501) staff       (20)    28135 2023-12-13 09:58:20.000000 MLXpress-0.1.9.1/MLXpress/ml.py
+-rw-rw-r--   0 vinilg7    (501) staff       (20)     5030 2023-07-17 05:03:38.000000 MLXpress-0.1.9.1/MLXpress/preprocessing.py
+-rw-rw-r--   0 vinilg7    (501) staff       (20)     1870 2023-07-17 05:24:56.000000 MLXpress-0.1.9.1/MLXpress/stats.py
+-rw-r--r--   0 vinilg7    (501) staff       (20)    11741 2024-04-27 13:48:43.000000 MLXpress-0.1.9.1/MLXpress/timeSeries.py
+-rw-rw-r--   0 vinilg7    (501) staff       (20)     2733 2023-07-17 06:10:32.000000 MLXpress-0.1.9.1/MLXpress/wine.py
+drwxr-xr-x   0 vinilg7    (501) staff       (20)        0 2024-04-27 14:09:57.904317 MLXpress-0.1.9.1/MLXpress.egg-info/
+-rw-r--r--   0 vinilg7    (501) staff       (20)     2461 2024-04-27 14:09:57.000000 MLXpress-0.1.9.1/MLXpress.egg-info/PKG-INFO
+-rw-r--r--   0 vinilg7    (501) staff       (20)      409 2024-04-27 14:09:57.000000 MLXpress-0.1.9.1/MLXpress.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinilg7    (501) staff       (20)        1 2024-04-27 14:09:57.000000 MLXpress-0.1.9.1/MLXpress.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinilg7    (501) staff       (20)       97 2024-04-27 14:09:57.000000 MLXpress-0.1.9.1/MLXpress.egg-info/requires.txt
+-rw-rw-r--   0 vinilg7    (501) staff       (20)        9 2024-04-27 14:09:57.000000 MLXpress-0.1.9.1/MLXpress.egg-info/top_level.txt
+-rw-r--r--   0 vinilg7    (501) staff       (20)     2461 2024-04-27 14:09:57.904775 MLXpress-0.1.9.1/PKG-INFO
+-rw-rw-r--   0 vinilg7    (501) staff       (20)     1718 2023-07-16 07:37:28.000000 MLXpress-0.1.9.1/README.md
+-rw-r--r--   0 vinilg7    (501) staff       (20)       38 2024-04-27 14:09:57.905048 MLXpress-0.1.9.1/setup.cfg
+-rw-r--r--   0 vinilg7    (501) staff       (20)      981 2024-04-27 14:09:29.000000 MLXpress-0.1.9.1/setup.py
```

### Comparing `MLXpress-0.1.9.0/MLXpress/bigdata.py` & `MLXpress-0.1.9.1/MLXpress/bigdata.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.0/MLXpress/diabetes.py` & `MLXpress-0.1.9.1/MLXpress/diabetes.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.0/MLXpress/getdata.py` & `MLXpress-0.1.9.1/MLXpress/getdata.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.0/MLXpress/help.py` & `MLXpress-0.1.9.1/MLXpress/help.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.0/MLXpress/iris.py` & `MLXpress-0.1.9.1/MLXpress/iris.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.0/MLXpress/math.py` & `MLXpress-0.1.9.1/MLXpress/math.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.0/MLXpress/ml.py` & `MLXpress-0.1.9.1/MLXpress/ml.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.0/MLXpress/preprocessing.py` & `MLXpress-0.1.9.1/MLXpress/preprocessing.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.0/MLXpress/stats.py` & `MLXpress-0.1.9.1/MLXpress/stats.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.0/MLXpress/timeSeries.py` & `MLXpress-0.1.9.1/MLXpress/timeSeries.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.0/MLXpress/wine.py` & `MLXpress-0.1.9.1/MLXpress/wine.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.0/MLXpress.egg-info/PKG-INFO` & `MLXpress-0.1.9.1/MLXpress.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLXpress
-Version: 0.1.9.0
+Version: 0.1.9.1
 Summary: A powerful and user-friendly machine learning toolkit for data science and ML professionals to accelerate their workflow
 Author: vinilg7
 Author-email: vinilg7@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MLXpress-0.1.9.0/PKG-INFO` & `MLXpress-0.1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLXpress
-Version: 0.1.9.0
+Version: 0.1.9.1
 Summary: A powerful and user-friendly machine learning toolkit for data science and ML professionals to accelerate their workflow
 Author: vinilg7
 Author-email: vinilg7@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MLXpress-0.1.9.0/README.md` & `MLXpress-0.1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.0/setup.py` & `MLXpress-0.1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='MLXpress',
-    version='0.1.9.0',
+    version='0.1.9.1',
     author='vinilg7',
     author_email='vinilg7@gmail.com',
     description='A powerful and user-friendly machine learning toolkit for data science and ML professionals to accelerate their workflow',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

