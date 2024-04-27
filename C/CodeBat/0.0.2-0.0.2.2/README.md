# Comparing `tmp/codebat-0.0.2.tar.gz` & `tmp/codebat-0.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codebat-0.0.2.tar", last modified: Sat Apr 27 03:48:58 2024, max compression
+gzip compressed data, was "codebat-0.0.2.2.tar", last modified: Sat Apr 27 03:56:17 2024, max compression
```

## Comparing `codebat-0.0.2.tar` & `codebat-0.0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 03:48:58.971039 codebat-0.0.2/
-drwxrwxrwx   0        0        0        0 2024-04-27 03:48:58.966698 codebat-0.0.2/CodeBat.egg-info/
--rw-rw-rw-   0        0        0      538 2024-04-27 03:48:58.000000 codebat-0.0.2/CodeBat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2024-04-27 03:48:58.000000 codebat-0.0.2/CodeBat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 03:48:58.000000 codebat-0.0.2/CodeBat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-27 03:48:58.000000 codebat-0.0.2/CodeBat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 03:48:58.000000 codebat-0.0.2/CodeBat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11357 2024-04-27 00:32:34.000000 codebat-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      538 2024-04-27 03:48:58.968897 codebat-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       51 2024-04-27 00:41:07.000000 codebat-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 03:48:58.972122 codebat-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      731 2024-04-27 03:48:34.000000 codebat-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:56:17.038292 codebat-0.0.2.2/
+drwxrwxrwx   0        0        0        0 2024-04-27 03:56:17.031752 codebat-0.0.2.2/CodeBat.egg-info/
+-rw-rw-rw-   0        0        0      540 2024-04-27 03:56:16.000000 codebat-0.0.2.2/CodeBat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2024-04-27 03:56:16.000000 codebat-0.0.2.2/CodeBat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 03:56:16.000000 codebat-0.0.2.2/CodeBat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-27 03:56:16.000000 codebat-0.0.2.2/CodeBat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 03:56:16.000000 codebat-0.0.2.2/CodeBat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11357 2024-04-27 00:32:34.000000 codebat-0.0.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      540 2024-04-27 03:56:17.034965 codebat-0.0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2024-04-27 00:41:07.000000 codebat-0.0.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 03:56:17.039404 codebat-0.0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      719 2024-04-27 03:56:05.000000 codebat-0.0.2.2/setup.py
```

### Comparing `codebat-0.0.2/CodeBat.egg-info/PKG-INFO` & `codebat-0.0.2.2/CodeBat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodeBat
-Version: 0.0.2
+Version: 0.0.2.2
 Summary: A Python Library for CodeMao API.
 Home-page: https://github.com/ShawnMerryCode/CodeBat
 Author: ShawnMerry
 Author-email: merrybili@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `codebat-0.0.2/LICENSE.txt` & `codebat-0.0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `codebat-0.0.2/PKG-INFO` & `codebat-0.0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodeBat
-Version: 0.0.2
+Version: 0.0.2.2
 Summary: A Python Library for CodeMao API.
 Home-page: https://github.com/ShawnMerryCode/CodeBat
 Author: ShawnMerry
 Author-email: merrybili@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `codebat-0.0.2/setup.py` & `codebat-0.0.2.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="CodeBat",
-    version="0.0.2",
+    version="0.0.2.02",
     author="ShawnMerry",
     author_email="merrybili@163.com",
     description="A Python Library for CodeMao API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ShawnMerryCode/CodeBat",
-    packages=find_packages("./src/CodeBat"),
+    packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.12",
     install_requires=['requests>=2.31.0']
```

