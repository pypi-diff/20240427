# Comparing `tmp/codebat-0.0.2.2.tar.gz` & `tmp/codebat-0.0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codebat-0.0.2.2.tar", last modified: Sat Apr 27 03:56:17 2024, max compression
+gzip compressed data, was "codebat-0.0.2.3.tar", last modified: Sat Apr 27 04:18:30 2024, max compression
```

## Comparing `codebat-0.0.2.2.tar` & `codebat-0.0.2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 03:56:17.038292 codebat-0.0.2.2/
-drwxrwxrwx   0        0        0        0 2024-04-27 03:56:17.031752 codebat-0.0.2.2/CodeBat.egg-info/
--rw-rw-rw-   0        0        0      540 2024-04-27 03:56:16.000000 codebat-0.0.2.2/CodeBat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2024-04-27 03:56:16.000000 codebat-0.0.2.2/CodeBat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 03:56:16.000000 codebat-0.0.2.2/CodeBat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-27 03:56:16.000000 codebat-0.0.2.2/CodeBat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 03:56:16.000000 codebat-0.0.2.2/CodeBat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11357 2024-04-27 00:32:34.000000 codebat-0.0.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0      540 2024-04-27 03:56:17.034965 codebat-0.0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       51 2024-04-27 00:41:07.000000 codebat-0.0.2.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 03:56:17.039404 codebat-0.0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      719 2024-04-27 03:56:05.000000 codebat-0.0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 04:18:30.070443 codebat-0.0.2.3/
+drwxrwxrwx   0        0        0        0 2024-04-27 04:18:30.064037 codebat-0.0.2.3/CodeBat.egg-info/
+-rw-rw-rw-   0        0        0      536 2024-04-27 04:18:29.000000 codebat-0.0.2.3/CodeBat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2024-04-27 04:18:29.000000 codebat-0.0.2.3/CodeBat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 04:18:29.000000 codebat-0.0.2.3/CodeBat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-27 04:18:29.000000 codebat-0.0.2.3/CodeBat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 04:18:29.000000 codebat-0.0.2.3/CodeBat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11357 2024-04-27 00:32:34.000000 codebat-0.0.2.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      536 2024-04-27 04:18:30.066166 codebat-0.0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-27 04:18:15.000000 codebat-0.0.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 04:18:30.070554 codebat-0.0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      721 2024-04-27 04:18:15.000000 codebat-0.0.2.3/setup.py
```

### Comparing `codebat-0.0.2.2/LICENSE.txt` & `codebat-0.0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `codebat-0.0.2.2/setup.py` & `codebat-0.0.2.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="CodeBat",
-    version="0.0.2.02",
+    version="0.0.2.03",
     author="ShawnMerry",
     author_email="merrybili@163.com",
-    description="A Python Library for CodeMao API.",
+    description="A Python Library about Codemao API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ShawnMerryCode/CodeBat",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

