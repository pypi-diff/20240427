# Comparing `tmp/codebat-0.0.2.4.tar.gz` & `tmp/codebat-0.0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codebat-0.0.2.4.tar", last modified: Sat Apr 27 04:23:03 2024, max compression
+gzip compressed data, was "codebat-0.0.2.5.tar", last modified: Sat Apr 27 16:06:47 2024, max compression
```

## Comparing `codebat-0.0.2.4.tar` & `codebat-0.0.2.5.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 04:23:03.104285 codebat-0.0.2.4/
-drwxrwxrwx   0        0        0        0 2024-04-27 04:23:03.096465 codebat-0.0.2.4/CodeBat.egg-info/
--rw-rw-rw-   0        0        0      536 2024-04-27 04:23:02.000000 codebat-0.0.2.4/CodeBat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2024-04-27 04:23:02.000000 codebat-0.0.2.4/CodeBat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 04:23:02.000000 codebat-0.0.2.4/CodeBat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-27 04:23:02.000000 codebat-0.0.2.4/CodeBat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 04:23:02.000000 codebat-0.0.2.4/CodeBat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11357 2024-04-27 00:32:34.000000 codebat-0.0.2.4/LICENSE.txt
--rw-rw-rw-   0        0        0      536 2024-04-27 04:23:03.099890 codebat-0.0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-27 04:18:15.000000 codebat-0.0.2.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 04:23:03.105381 codebat-0.0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      720 2024-04-27 04:22:35.000000 codebat-0.0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 16:06:47.117408 codebat-0.0.2.5/
+drwxrwxrwx   0        0        0        0 2024-04-27 16:06:47.093020 codebat-0.0.2.5/CodeBat/
+-rw-rw-rw-   0        0        0     3892 2024-04-27 04:22:23.000000 codebat-0.0.2.5/CodeBat/CodeBat.py
+-rw-rw-rw-   0        0        0        0 2024-04-27 04:22:11.000000 codebat-0.0.2.5/CodeBat/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 16:06:47.110980 codebat-0.0.2.5/CodeBat.egg-info/
+-rw-rw-rw-   0        0        0      536 2024-04-27 16:06:46.000000 codebat-0.0.2.5/CodeBat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2024-04-27 16:06:46.000000 codebat-0.0.2.5/CodeBat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 16:06:46.000000 codebat-0.0.2.5/CodeBat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-27 16:06:46.000000 codebat-0.0.2.5/CodeBat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-27 16:06:46.000000 codebat-0.0.2.5/CodeBat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11357 2024-04-27 00:32:34.000000 codebat-0.0.2.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      536 2024-04-27 16:06:47.113136 codebat-0.0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-27 04:18:15.000000 codebat-0.0.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 16:06:47.117408 codebat-0.0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      720 2024-04-27 16:03:50.000000 codebat-0.0.2.5/setup.py
```

### Comparing `codebat-0.0.2.4/CodeBat.egg-info/PKG-INFO` & `codebat-0.0.2.5/CodeBat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodeBat
-Version: 0.0.2.4
+Version: 0.0.2.5
 Summary: A Python Library about Codemao API.
 Home-page: https://github.com/ShawnMerryCode/CodeBat
 Author: ShawnMerry
 Author-email: merrybili@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `codebat-0.0.2.4/LICENSE.txt` & `codebat-0.0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `codebat-0.0.2.4/PKG-INFO` & `codebat-0.0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodeBat
-Version: 0.0.2.4
+Version: 0.0.2.5
 Summary: A Python Library about Codemao API.
 Home-page: https://github.com/ShawnMerryCode/CodeBat
 Author: ShawnMerry
 Author-email: merrybili@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `codebat-0.0.2.4/setup.py` & `codebat-0.0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="CodeBat",
-    version="0.0.2.4",
+    version="0.0.2.5",
     author="ShawnMerry",
     author_email="merrybili@163.com",
     description="A Python Library about Codemao API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ShawnMerryCode/CodeBat",
     packages=find_packages(),
```

