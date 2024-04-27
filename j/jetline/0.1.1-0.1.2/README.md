# Comparing `tmp/jetline-0.1.1.tar.gz` & `tmp/jetline-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jetline-0.1.1.tar", last modified: Fri Apr 26 06:01:45 2024, max compression
+gzip compressed data, was "jetline-0.1.2.tar", last modified: Fri Apr 26 11:12:52 2024, max compression
```

## Comparing `jetline-0.1.1.tar` & `jetline-0.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-26 06:01:45.435387 jetline-0.1.1/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-26 06:01:45.435168 jetline-0.1.1/PKG-INFO
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1103 2024-04-25 16:42:38.000000 jetline-0.1.1/README.md
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-26 06:01:45.430188 jetline-0.1.1/jetline/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.1/jetline/__init__.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-26 06:01:45.432945 jetline-0.1.1/jetline/commands/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.1/jetline/commands/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1998 2024-04-25 16:41:25.000000 jetline-0.1.1/jetline/commands/_helper.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)    10737 2024-04-25 16:41:25.000000 jetline-0.1.1/jetline/commands/analyze_project.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     4122 2024-04-26 06:00:11.000000 jetline-0.1.1/jetline/commands/create_pipe.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     2086 2024-04-25 16:41:25.000000 jetline-0.1.1/jetline/commands/info.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     2866 2024-04-25 16:41:25.000000 jetline-0.1.1/jetline/commands/installer.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1134 2024-04-26 06:01:00.000000 jetline-0.1.1/jetline/commands/run_pipeline.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)    13304 2024-04-25 16:41:25.000000 jetline-0.1.1/jetline/commands/to_exe.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-26 06:01:45.433354 jetline-0.1.1/jetline/data/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.1/jetline/data/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     5221 2024-04-25 16:41:25.000000 jetline-0.1.1/jetline/data/data.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     3222 2024-04-26 05:41:26.000000 jetline-0.1.1/jetline/data/helper.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      127 2024-04-26 05:52:47.000000 jetline-0.1.1/jetline/logging.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-26 06:01:45.433828 jetline-0.1.1/jetline/pipeline/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.1/jetline/pipeline/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1684 2024-04-25 16:41:25.000000 jetline-0.1.1/jetline/pipeline/node.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     6038 2024-04-26 05:59:24.000000 jetline-0.1.1/jetline/pipeline/pipeline.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-26 06:01:45.434679 jetline-0.1.1/jetline/templates/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.1/jetline/templates/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      709 2024-04-25 16:41:25.000000 jetline-0.1.1/jetline/templates/data.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      664 2024-04-25 16:41:25.000000 jetline-0.1.1/jetline/templates/main.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      603 2024-04-25 16:41:25.000000 jetline-0.1.1/jetline/templates/nodes.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      804 2024-04-25 16:41:25.000000 jetline-0.1.1/jetline/templates/pipeline.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-26 06:01:45.434904 jetline-0.1.1/jetline.egg-info/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-26 06:01:45.000000 jetline-0.1.1/jetline.egg-info/PKG-INFO
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      776 2024-04-26 06:01:45.000000 jetline-0.1.1/jetline.egg-info/SOURCES.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        1 2024-04-26 06:01:45.000000 jetline-0.1.1/jetline.egg-info/dependency_links.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      317 2024-04-26 06:01:45.000000 jetline-0.1.1/jetline.egg-info/entry_points.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      117 2024-04-26 06:01:45.000000 jetline-0.1.1/jetline.egg-info/requires.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        8 2024-04-26 06:01:45.000000 jetline-0.1.1/jetline.egg-info/top_level.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)       38 2024-04-26 06:01:45.435434 jetline-0.1.1/setup.cfg
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1639 2024-04-26 06:01:18.000000 jetline-0.1.1/setup.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-26 11:12:52.354077 jetline-0.1.2/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-26 11:12:52.353816 jetline-0.1.2/PKG-INFO
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1103 2024-04-25 16:42:38.000000 jetline-0.1.2/README.md
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-26 11:12:52.329724 jetline-0.1.2/jetline/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.2/jetline/__init__.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-26 11:12:52.343384 jetline-0.1.2/jetline/commands/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.2/jetline/commands/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1998 2024-04-25 16:41:25.000000 jetline-0.1.2/jetline/commands/_helper.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)    10737 2024-04-25 16:41:25.000000 jetline-0.1.2/jetline/commands/analyze_project.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     4122 2024-04-26 06:00:11.000000 jetline-0.1.2/jetline/commands/create_pipe.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     2086 2024-04-25 16:41:25.000000 jetline-0.1.2/jetline/commands/info.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     2866 2024-04-25 16:41:25.000000 jetline-0.1.2/jetline/commands/installer.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1134 2024-04-26 06:01:00.000000 jetline-0.1.2/jetline/commands/run_pipeline.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)    13304 2024-04-25 16:41:25.000000 jetline-0.1.2/jetline/commands/to_exe.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-26 11:12:52.347336 jetline-0.1.2/jetline/data/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.2/jetline/data/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     5221 2024-04-25 16:41:25.000000 jetline-0.1.2/jetline/data/data.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     3222 2024-04-26 05:41:26.000000 jetline-0.1.2/jetline/data/helper.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      127 2024-04-26 05:52:47.000000 jetline-0.1.2/jetline/logging.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-26 11:12:52.350821 jetline-0.1.2/jetline/pipeline/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.2/jetline/pipeline/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1684 2024-04-25 16:41:25.000000 jetline-0.1.2/jetline/pipeline/node.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     6038 2024-04-26 05:59:24.000000 jetline-0.1.2/jetline/pipeline/pipeline.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-26 11:12:52.353171 jetline-0.1.2/jetline/templates/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.2/jetline/templates/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      709 2024-04-25 16:41:25.000000 jetline-0.1.2/jetline/templates/data.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      664 2024-04-25 16:41:25.000000 jetline-0.1.2/jetline/templates/main.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      603 2024-04-25 16:41:25.000000 jetline-0.1.2/jetline/templates/nodes.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      804 2024-04-25 16:41:25.000000 jetline-0.1.2/jetline/templates/pipeline.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-26 11:12:52.353447 jetline-0.1.2/jetline.egg-info/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-26 11:12:52.000000 jetline-0.1.2/jetline.egg-info/PKG-INFO
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      776 2024-04-26 11:12:52.000000 jetline-0.1.2/jetline.egg-info/SOURCES.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        1 2024-04-26 11:12:52.000000 jetline-0.1.2/jetline.egg-info/dependency_links.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      317 2024-04-26 11:12:52.000000 jetline-0.1.2/jetline.egg-info/entry_points.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      117 2024-04-26 11:12:52.000000 jetline-0.1.2/jetline.egg-info/requires.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        8 2024-04-26 11:12:52.000000 jetline-0.1.2/jetline.egg-info/top_level.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)       38 2024-04-26 11:12:52.354143 jetline-0.1.2/setup.cfg
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1639 2024-04-26 11:12:36.000000 jetline-0.1.2/setup.py
```

### Comparing `jetline-0.1.1/PKG-INFO` & `jetline-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetline
-Version: 0.1.1
+Version: 0.1.2
 Summary: Automated Pipeline Builder
 Home-page: https://github.com/your_username/jetline
 Author: Johannes Kanthak
 Author-email: johannes.kanthak@kdc-solutions.de
 License: MIT
 Keywords: pipeline automation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `jetline-0.1.1/README.md` & `jetline-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `jetline-0.1.1/jetline/commands/_helper.py` & `jetline-0.1.2/jetline/commands/_helper.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.1/jetline/commands/analyze_project.py` & `jetline-0.1.2/jetline/commands/analyze_project.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.1/jetline/commands/create_pipe.py` & `jetline-0.1.2/jetline/commands/create_pipe.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.1/jetline/commands/info.py` & `jetline-0.1.2/jetline/commands/info.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.1/jetline/commands/installer.py` & `jetline-0.1.2/jetline/commands/installer.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.1/jetline/commands/run_pipeline.py` & `jetline-0.1.2/jetline/commands/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.1/jetline/commands/to_exe.py` & `jetline-0.1.2/jetline/commands/to_exe.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.1/jetline/data/data.py` & `jetline-0.1.2/jetline/data/data.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.1/jetline/data/helper.py` & `jetline-0.1.2/jetline/data/helper.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.1/jetline/pipeline/node.py` & `jetline-0.1.2/jetline/pipeline/node.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.1/jetline/pipeline/pipeline.py` & `jetline-0.1.2/jetline/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.1/jetline/templates/data.py` & `jetline-0.1.2/jetline/templates/data.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.1/jetline/templates/main.py` & `jetline-0.1.2/jetline/templates/main.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.1/jetline/templates/nodes.py` & `jetline-0.1.2/jetline/templates/nodes.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.1/jetline/templates/pipeline.py` & `jetline-0.1.2/jetline/templates/pipeline.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.1/jetline.egg-info/PKG-INFO` & `jetline-0.1.2/jetline.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetline
-Version: 0.1.1
+Version: 0.1.2
 Summary: Automated Pipeline Builder
 Home-page: https://github.com/your_username/jetline
 Author: Johannes Kanthak
 Author-email: johannes.kanthak@kdc-solutions.de
 License: MIT
 Keywords: pipeline automation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `jetline-0.1.1/jetline.egg-info/SOURCES.txt` & `jetline-0.1.2/jetline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jetline-0.1.1/setup.py` & `jetline-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     'vulture'
     
 
 ]
 
 setup(
     name='jetline',
-    version='0.1.1',
+    version='0.1.2',
     description='Automated Pipeline Builder',
     url='https://github.com/your_username/jetline',
     author='Johannes Kanthak',
     author_email='johannes.kanthak@kdc-solutions.de',
     license='MIT',
     classifiers=classifiers,
     keywords='pipeline automation',
```

