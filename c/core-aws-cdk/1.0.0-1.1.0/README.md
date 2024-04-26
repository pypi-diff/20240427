# Comparing `tmp/core-aws-cdk-1.0.0.tar.gz` & `tmp/core_aws_cdk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core-aws-cdk-1.0.0.tar", last modified: Mon Dec 25 14:46:07 2023, max compression
+gzip compressed data, was "core_aws_cdk-1.1.0.tar", last modified: Fri Apr 26 23:07:00 2024, max compression
```

## Comparing `core-aws-cdk-1.0.0.tar` & `core_aws_cdk-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-25 14:46:07.772653 core-aws-cdk-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1082 2023-12-25 14:45:47.000000 core-aws-cdk-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1639 2023-12-25 14:46:07.771653 core-aws-cdk-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      702 2023-12-25 14:45:47.000000 core-aws-cdk-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-25 14:46:07.769653 core-aws-cdk-1.0.0/core_aws_cdk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-25 14:45:47.000000 core-aws-cdk-1.0.0/core_aws_cdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-25 14:46:07.771653 core-aws-cdk-1.0.0/core_aws_cdk/stacks/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-12-25 14:45:47.000000 core-aws-cdk-1.0.0/core_aws_cdk/stacks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      837 2023-12-25 14:45:47.000000 core-aws-cdk-1.0.0/core_aws_cdk/stacks/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1589 2023-12-25 14:45:47.000000 core-aws-cdk-1.0.0/core_aws_cdk/stacks/functions.py
--rw-rw-rw-   0 root         (0) root         (0)     1149 2023-12-25 14:45:47.000000 core-aws-cdk-1.0.0/core_aws_cdk/stacks/s3.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-12-25 14:45:47.000000 core-aws-cdk-1.0.0/core_aws_cdk/stacks/sns.py
--rw-rw-rw-   0 root         (0) root         (0)     1551 2023-12-25 14:45:47.000000 core-aws-cdk-1.0.0/core_aws_cdk/stacks/sqs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-25 14:46:07.771653 core-aws-cdk-1.0.0/core_aws_cdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1639 2023-12-25 14:46:07.000000 core-aws-cdk-1.0.0/core_aws_cdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      418 2023-12-25 14:46:07.000000 core-aws-cdk-1.0.0/core_aws_cdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-25 14:46:07.000000 core-aws-cdk-1.0.0/core_aws_cdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       83 2023-12-25 14:46:07.000000 core-aws-cdk-1.0.0/core_aws_cdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-12-25 14:46:07.000000 core-aws-cdk-1.0.0/core_aws_cdk.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1317 2023-12-25 14:45:47.000000 core-aws-cdk-1.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-25 14:46:07.772653 core-aws-cdk-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-12-25 14:45:47.000000 core-aws-cdk-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 23:07:00.155951 core_aws_cdk-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2024-04-26 23:06:44.000000 core_aws_cdk-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1588 2024-04-26 23:07:00.155951 core_aws_cdk-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      702 2024-04-26 23:06:44.000000 core_aws_cdk-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 23:07:00.152951 core_aws_cdk-1.1.0/core_aws_cdk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 23:06:44.000000 core_aws_cdk-1.1.0/core_aws_cdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 23:07:00.154951 core_aws_cdk-1.1.0/core_aws_cdk/stacks/
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-26 23:06:44.000000 core_aws_cdk-1.1.0/core_aws_cdk/stacks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 23:07:00.154951 core_aws_cdk-1.1.0/core_aws_cdk/stacks/aws_lambda/
+-rw-rw-rw-   0 root         (0) root         (0)       59 2024-04-26 23:06:44.000000 core_aws_cdk-1.1.0/core_aws_cdk/stacks/aws_lambda/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5204 2024-04-26 23:06:44.000000 core_aws_cdk-1.1.0/core_aws_cdk/stacks/aws_lambda/assets.py
+-rw-rw-rw-   0 root         (0) root         (0)     3312 2024-04-26 23:06:44.000000 core_aws_cdk-1.1.0/core_aws_cdk/stacks/aws_lambda/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      837 2024-04-26 23:06:44.000000 core_aws_cdk-1.1.0/core_aws_cdk/stacks/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1149 2024-04-26 23:06:44.000000 core_aws_cdk-1.1.0/core_aws_cdk/stacks/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2024-04-26 23:06:44.000000 core_aws_cdk-1.1.0/core_aws_cdk/stacks/sns.py
+-rw-rw-rw-   0 root         (0) root         (0)     1551 2024-04-26 23:06:44.000000 core_aws_cdk-1.1.0/core_aws_cdk/stacks/sqs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 23:07:00.155951 core_aws_cdk-1.1.0/core_aws_cdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1588 2024-04-26 23:07:00.000000 core_aws_cdk-1.1.0/core_aws_cdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      508 2024-04-26 23:07:00.000000 core_aws_cdk-1.1.0/core_aws_cdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 23:07:00.000000 core_aws_cdk-1.1.0/core_aws_cdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-26 23:07:00.000000 core_aws_cdk-1.1.0/core_aws_cdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-26 23:07:00.000000 core_aws_cdk-1.1.0/core_aws_cdk.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1274 2024-04-26 23:06:44.000000 core_aws_cdk-1.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 23:07:00.155951 core_aws_cdk-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       64 2024-04-26 23:06:44.000000 core_aws_cdk-1.1.0/setup.py
```

### Comparing `core-aws-cdk-1.0.0/LICENSE` & `core_aws_cdk-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `core-aws-cdk-1.0.0/PKG-INFO` & `core_aws_cdk-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-aws-cdk
-Version: 1.0.0
+Version: 1.1.0
 Summary: This project contains the commons elements to create infrastructure in AWS using AWS CDK...
 Author-email: Alejandro Cora González <alek.cora.glez@gmail.com>
 Maintainer: Alejandro Cora González
 License: MIT
 Project-URL: Homepage, https://gitlab.com/bytecode-solutions/infrastructure/core-aws-cdk
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -12,17 +12,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aws-cdk-lib==2.110.0
-Requires-Dist: aws-cdk.aws-lambda-python-alpha==2.100.0a0
-Requires-Dist: core-tests
+Requires-Dist: aws-cdk-lib==2.139.0
+Requires-Dist: core-tests==1.0.3
 Provides-Extra: test
 
 # core-aws-cdk
 ___________________________________________________________________________________________________________________
 
 This project contains the commons elements to create infrastructure
 in AWS using AWS CDK...
```

### Comparing `core-aws-cdk-1.0.0/README.md` & `core_aws_cdk-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `core-aws-cdk-1.0.0/core_aws_cdk/stacks/base.py` & `core_aws_cdk-1.1.0/core_aws_cdk/stacks/base.py`

 * *Files identical despite different names*

### Comparing `core-aws-cdk-1.0.0/core_aws_cdk/stacks/s3.py` & `core_aws_cdk-1.1.0/core_aws_cdk/stacks/s3.py`

 * *Files identical despite different names*

### Comparing `core-aws-cdk-1.0.0/core_aws_cdk/stacks/sns.py` & `core_aws_cdk-1.1.0/core_aws_cdk/stacks/sns.py`

 * *Files identical despite different names*

### Comparing `core-aws-cdk-1.0.0/core_aws_cdk/stacks/sqs.py` & `core_aws_cdk-1.1.0/core_aws_cdk/stacks/sqs.py`

 * *Files identical despite different names*

### Comparing `core-aws-cdk-1.0.0/core_aws_cdk.egg-info/PKG-INFO` & `core_aws_cdk-1.1.0/core_aws_cdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-aws-cdk
-Version: 1.0.0
+Version: 1.1.0
 Summary: This project contains the commons elements to create infrastructure in AWS using AWS CDK...
 Author-email: Alejandro Cora González <alek.cora.glez@gmail.com>
 Maintainer: Alejandro Cora González
 License: MIT
 Project-URL: Homepage, https://gitlab.com/bytecode-solutions/infrastructure/core-aws-cdk
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -12,17 +12,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aws-cdk-lib==2.110.0
-Requires-Dist: aws-cdk.aws-lambda-python-alpha==2.100.0a0
-Requires-Dist: core-tests
+Requires-Dist: aws-cdk-lib==2.139.0
+Requires-Dist: core-tests==1.0.3
 Provides-Extra: test
 
 # core-aws-cdk
 ___________________________________________________________________________________________________________________
 
 This project contains the commons elements to create infrastructure
 in AWS using AWS CDK...
```

### Comparing `core-aws-cdk-1.0.0/pyproject.toml` & `core_aws_cdk-1.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "core-aws-cdk"
 description = "This project contains the commons elements to create infrastructure in AWS using AWS CDK..."
-version = "1.0.0"
+version = "1.1.0"
 
 authors = [
     {name = "Alejandro Cora González", email = "alek.cora.glez@gmail.com"}
 ]
 
 maintainers = [
     {name = "Alejandro Cora González"}
@@ -31,17 +31,16 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.11",
     "Intended Audience :: Developers",
     "Topic :: Utilities"
 ]
 
 dependencies = [
-    "aws-cdk-lib==2.110.0",
-    "aws-cdk.aws-lambda-python-alpha==2.100.0a0",
-    "core-tests",
+    "aws-cdk-lib==2.139.0",
+    "core-tests==1.0.3",
 ]
 
 [project.urls]
 Homepage = "https://gitlab.com/bytecode-solutions/infrastructure/core-aws-cdk"
 
 [project.optional-dependencies]
 test = []
```

