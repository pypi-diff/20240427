# Comparing `tmp/projen-0.81.1.tar.gz` & `tmp/projen-0.81.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projen-0.81.1.tar", last modified: Thu Apr 18 09:53:21 2024, max compression
+gzip compressed data, was "projen-0.81.2.tar", last modified: Fri Apr 26 17:27:43 2024, max compression
```

## Comparing `projen-0.81.1.tar` & `projen-0.81.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.281163 projen-0.81.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-18 09:53:10.000000 projen-0.81.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 09:53:10.000000 projen-0.81.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-04-18 09:53:21.281163 projen-0.81.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    78674 2024-04-18 09:53:10.000000 projen-0.81.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-18 09:53:10.000000 projen-0.81.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 09:53:21.281163 projen-0.81.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-18 09:53:10.000000 projen-0.81.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.261162 projen-0.81.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.265162 projen-0.81.1/src/projen/
--rw-r--r--   0 runner    (1001) docker     (127)   651984 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.265162 projen-0.81.1/src/projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.269162 projen-0.81.1/src/projen/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/_jsii/bin/projen
--rw-r--r--   0 runner    (1001) docker     (127)  2649940 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/_jsii/projen@0.81.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.269162 projen-0.81.1/src/projen/awscdk/
--rw-r--r--   0 runner    (1001) docker     (127)  1079302 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/awscdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.273162 projen-0.81.1/src/projen/build/
--rw-r--r--   0 runner    (1001) docker     (127)    52320 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.273162 projen-0.81.1/src/projen/cdk/
--rw-r--r--   0 runner    (1001) docker     (127)   510147 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.273162 projen-0.81.1/src/projen/cdk8s/
--rw-r--r--   0 runner    (1001) docker     (127)   597384 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/cdk8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.273162 projen-0.81.1/src/projen/cdktf/
--rw-r--r--   0 runner    (1001) docker     (127)   224466 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/cdktf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.277162 projen-0.81.1/src/projen/circleci/
--rw-r--r--   0 runner    (1001) docker     (127)    75913 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/circleci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.277162 projen-0.81.1/src/projen/github/
--rw-r--r--   0 runner    (1001) docker     (127)   407630 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.277162 projen-0.81.1/src/projen/github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)   250737 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/github/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.277162 projen-0.81.1/src/projen/gitlab/
--rw-r--r--   0 runner    (1001) docker     (127)   202810 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/gitlab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.277162 projen-0.81.1/src/projen/java/
--rw-r--r--   0 runner    (1001) docker     (127)   183709 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.277162 projen-0.81.1/src/projen/javascript/
--rw-r--r--   0 runner    (1001) docker     (127)   844523 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/javascript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.277162 projen-0.81.1/src/projen/python/
--rw-r--r--   0 runner    (1001) docker     (127)   213158 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.277162 projen-0.81.1/src/projen/release/
--rw-r--r--   0 runner    (1001) docker     (127)   285447 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/release/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.281163 projen-0.81.1/src/projen/typescript/
--rw-r--r--   0 runner    (1001) docker     (127)   474506 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/typescript/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.281163 projen-0.81.1/src/projen/vscode/
--rw-r--r--   0 runner    (1001) docker     (127)    69040 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/vscode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.281163 projen-0.81.1/src/projen/web/
--rw-r--r--   0 runner    (1001) docker     (127)   797444 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.265162 projen-0.81.1/src/projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-04-18 09:53:21.000000 projen-0.81.1/src/projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-18 09:53:21.000000 projen-0.81.1/src/projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:53:21.000000 projen-0.81.1/src/projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-18 09:53:21.000000 projen-0.81.1/src/projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 09:53:21.000000 projen-0.81.1/src/projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:27:43.104556 projen-0.81.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-26 17:27:30.000000 projen-0.81.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-26 17:27:30.000000 projen-0.81.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-04-26 17:27:43.104556 projen-0.81.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    78674 2024-04-26 17:27:30.000000 projen-0.81.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-26 17:27:30.000000 projen-0.81.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 17:27:43.104556 projen-0.81.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-26 17:27:30.000000 projen-0.81.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:27:43.084556 projen-0.81.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:27:43.088556 projen-0.81.2/src/projen/
+-rw-r--r--   0 runner    (1001) docker     (127)   651984 2024-04-26 17:27:30.000000 projen-0.81.2/src/projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:27:43.088556 projen-0.81.2/src/projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-26 17:27:30.000000 projen-0.81.2/src/projen/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:27:43.092556 projen-0.81.2/src/projen/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-26 17:27:30.000000 projen-0.81.2/src/projen/_jsii/bin/projen
+-rw-r--r--   0 runner    (1001) docker     (127)  2650275 2024-04-26 17:27:30.000000 projen-0.81.2/src/projen/_jsii/projen@0.81.2.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:27:43.092556 projen-0.81.2/src/projen/awscdk/
+-rw-r--r--   0 runner    (1001) docker     (127)  1079302 2024-04-26 17:27:30.000000 projen-0.81.2/src/projen/awscdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:27:43.096556 projen-0.81.2/src/projen/build/
+-rw-r--r--   0 runner    (1001) docker     (127)    52320 2024-04-26 17:27:30.000000 projen-0.81.2/src/projen/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:27:43.096556 projen-0.81.2/src/projen/cdk/
+-rw-r--r--   0 runner    (1001) docker     (127)   510147 2024-04-26 17:27:30.000000 projen-0.81.2/src/projen/cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:27:43.096556 projen-0.81.2/src/projen/cdk8s/
+-rw-r--r--   0 runner    (1001) docker     (127)   597384 2024-04-26 17:27:30.000000 projen-0.81.2/src/projen/cdk8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:27:43.096556 projen-0.81.2/src/projen/cdktf/
+-rw-r--r--   0 runner    (1001) docker     (127)   224466 2024-04-26 17:27:30.000000 projen-0.81.2/src/projen/cdktf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:27:43.096556 projen-0.81.2/src/projen/circleci/
+-rw-r--r--   0 runner    (1001) docker     (127)    75913 2024-04-26 17:27:30.000000 projen-0.81.2/src/projen/circleci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:27:43.096556 projen-0.81.2/src/projen/github/
+-rw-r--r--   0 runner    (1001) docker     (127)   409613 2024-04-26 17:27:30.000000 projen-0.81.2/src/projen/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:27:43.096556 projen-0.81.2/src/projen/github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)   250737 2024-04-26 17:27:30.000000 projen-0.81.2/src/projen/github/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:27:43.096556 projen-0.81.2/src/projen/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (127)   202810 2024-04-26 17:27:30.000000 projen-0.81.2/src/projen/gitlab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:27:43.100556 projen-0.81.2/src/projen/java/
+-rw-r--r--   0 runner    (1001) docker     (127)   183709 2024-04-26 17:27:30.000000 projen-0.81.2/src/projen/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:27:43.100556 projen-0.81.2/src/projen/javascript/
+-rw-r--r--   0 runner    (1001) docker     (127)   844523 2024-04-26 17:27:30.000000 projen-0.81.2/src/projen/javascript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 17:27:30.000000 projen-0.81.2/src/projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:27:43.100556 projen-0.81.2/src/projen/python/
+-rw-r--r--   0 runner    (1001) docker     (127)   213158 2024-04-26 17:27:30.000000 projen-0.81.2/src/projen/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:27:43.100556 projen-0.81.2/src/projen/release/
+-rw-r--r--   0 runner    (1001) docker     (127)   285447 2024-04-26 17:27:30.000000 projen-0.81.2/src/projen/release/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:27:43.100556 projen-0.81.2/src/projen/typescript/
+-rw-r--r--   0 runner    (1001) docker     (127)   474506 2024-04-26 17:27:30.000000 projen-0.81.2/src/projen/typescript/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:27:43.100556 projen-0.81.2/src/projen/vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)    69040 2024-04-26 17:27:30.000000 projen-0.81.2/src/projen/vscode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:27:43.100556 projen-0.81.2/src/projen/web/
+-rw-r--r--   0 runner    (1001) docker     (127)   797444 2024-04-26 17:27:30.000000 projen-0.81.2/src/projen/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:27:43.088556 projen-0.81.2/src/projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-04-26 17:27:43.000000 projen-0.81.2/src/projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-26 17:27:43.000000 projen-0.81.2/src/projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 17:27:43.000000 projen-0.81.2/src/projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-26 17:27:43.000000 projen-0.81.2/src/projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 17:27:43.000000 projen-0.81.2/src/projen.egg-info/top_level.txt
```

### Comparing `projen-0.81.1/LICENSE` & `projen-0.81.2/LICENSE`

 * *Files identical despite different names*

### Comparing `projen-0.81.1/PKG-INFO` & `projen-0.81.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.81.1
+Version: 0.81.2
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.81.1/README.md` & `projen-0.81.2/README.md`

 * *Files identical despite different names*

### Comparing `projen-0.81.1/setup.py` & `projen-0.81.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "projen",
-    "version": "0.81.1",
+    "version": "0.81.2",
     "description": "CDK for software projects",
     "license": "Apache-2.0",
     "url": "https://github.com/projen/projen.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -38,15 +38,15 @@
         "projen.release",
         "projen.typescript",
         "projen.vscode",
         "projen.web"
     ],
     "package_data": {
         "projen._jsii": [
-            "projen@0.81.1.jsii.tgz"
+            "projen@0.81.2.jsii.tgz"
         ],
         "projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `projen-0.81.1/src/projen/__init__.py` & `projen-0.81.2/src/projen/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.1/src/projen/awscdk/__init__.py` & `projen-0.81.2/src/projen/awscdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.1/src/projen/build/__init__.py` & `projen-0.81.2/src/projen/build/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.1/src/projen/cdk/__init__.py` & `projen-0.81.2/src/projen/cdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.1/src/projen/cdk8s/__init__.py` & `projen-0.81.2/src/projen/cdk8s/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.1/src/projen/cdktf/__init__.py` & `projen-0.81.2/src/projen/cdktf/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.1/src/projen/circleci/__init__.py` & `projen-0.81.2/src/projen/circleci/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.1/src/projen/github/__init__.py` & `projen-0.81.2/src/projen/github/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1189,28 +1189,30 @@
         ignore: typing.Optional[typing.Sequence[typing.Union["DependabotIgnore", typing.Dict[builtins.str, typing.Any]]]] = None,
         ignore_projen: typing.Optional[builtins.bool] = None,
         labels: typing.Optional[typing.Sequence[builtins.str]] = None,
         open_pull_requests_limit: typing.Optional[jsii.Number] = None,
         registries: typing.Optional[typing.Mapping[builtins.str, typing.Union["DependabotRegistry", typing.Dict[builtins.str, typing.Any]]]] = None,
         reviewers: typing.Optional[typing.Sequence[builtins.str]] = None,
         schedule_interval: typing.Optional["DependabotScheduleInterval"] = None,
+        target_branch: typing.Optional[builtins.str] = None,
         versioning_strategy: typing.Optional["VersioningStrategy"] = None,
     ) -> None:
         '''
         :param github: -
         :param allow: (experimental) https://docs.github.com/en/code-security/dependabot/dependabot-version-updates/configuration-options-for-the-dependabot.yml-file#allow. Use the allow option to customize which dependencies are updated. This applies to both version and security updates. Default: []
         :param assignees: (experimental) Specify individual assignees or teams of assignees for all pull requests raised for a package manager. Default: []
         :param groups: (experimental) https://docs.github.com/en/code-security/dependabot/dependabot-version-updates/configuration-options-for-the-dependabot.yml-file#groups. You can create groups to package dependency updates together into a single PR. Default: []
         :param ignore: (experimental) You can use the ``ignore`` option to customize which dependencies are updated. The ignore option supports the following options. Default: []
         :param ignore_projen: (experimental) Ignores updates to ``projen``. This is required since projen updates may cause changes in committed files and anti-tamper checks will fail. Projen upgrades are covered through the ``ProjenUpgrade`` class. Default: true
         :param labels: (experimental) List of labels to apply to the created PR's.
         :param open_pull_requests_limit: (experimental) Sets the maximum of pull requests Dependabot opens for version updates. Dependabot will not open any new requests until some of those open requests are merged or closed. Default: 5
         :param registries: (experimental) Map of package registries to use. Default: - use public registries
         :param reviewers: (experimental) Specify individual reviewers or teams of reviewers for all pull requests raised for a package manager. Default: []
         :param schedule_interval: (experimental) How often to check for new versions and raise pull requests. Default: ScheduleInterval.DAILY
+        :param target_branch: (experimental) https://docs.github.com/en/code-security/dependabot/dependabot-version-updates/configuration-options-for-the-dependabot.yml-file#target-branch You can configure the target branch for raising pull requests for version updates against.
         :param versioning_strategy: (experimental) The strategy to use when edits manifest and lock files. Default: VersioningStrategy.LOCKFILE_ONLY The default is to only update the lock file because package.json is controlled by projen and any outside updates will fail the build.
 
         :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2caae883697ce14c090e89c8fd0dbbab7e7c0f31d6d4d66311f05a6793bd9e92)
             check_type(argname="argument github", value=github, expected_type=type_hints["github"])
@@ -1221,14 +1223,15 @@
             ignore=ignore,
             ignore_projen=ignore_projen,
             labels=labels,
             open_pull_requests_limit=open_pull_requests_limit,
             registries=registries,
             reviewers=reviewers,
             schedule_interval=schedule_interval,
+            target_branch=target_branch,
             versioning_strategy=versioning_strategy,
         )
 
         jsii.create(self.__class__, self, [github, options])
 
     @jsii.member(jsii_name="addAllow")
     def add_allow(self, dependency_name: builtins.str) -> None:
@@ -1468,14 +1471,15 @@
         "ignore": "ignore",
         "ignore_projen": "ignoreProjen",
         "labels": "labels",
         "open_pull_requests_limit": "openPullRequestsLimit",
         "registries": "registries",
         "reviewers": "reviewers",
         "schedule_interval": "scheduleInterval",
+        "target_branch": "targetBranch",
         "versioning_strategy": "versioningStrategy",
     },
 )
 class DependabotOptions:
     def __init__(
         self,
         *,
@@ -1485,27 +1489,29 @@
         ignore: typing.Optional[typing.Sequence[typing.Union[DependabotIgnore, typing.Dict[builtins.str, typing.Any]]]] = None,
         ignore_projen: typing.Optional[builtins.bool] = None,
         labels: typing.Optional[typing.Sequence[builtins.str]] = None,
         open_pull_requests_limit: typing.Optional[jsii.Number] = None,
         registries: typing.Optional[typing.Mapping[builtins.str, typing.Union["DependabotRegistry", typing.Dict[builtins.str, typing.Any]]]] = None,
         reviewers: typing.Optional[typing.Sequence[builtins.str]] = None,
         schedule_interval: typing.Optional["DependabotScheduleInterval"] = None,
+        target_branch: typing.Optional[builtins.str] = None,
         versioning_strategy: typing.Optional["VersioningStrategy"] = None,
     ) -> None:
         '''
         :param allow: (experimental) https://docs.github.com/en/code-security/dependabot/dependabot-version-updates/configuration-options-for-the-dependabot.yml-file#allow. Use the allow option to customize which dependencies are updated. This applies to both version and security updates. Default: []
         :param assignees: (experimental) Specify individual assignees or teams of assignees for all pull requests raised for a package manager. Default: []
         :param groups: (experimental) https://docs.github.com/en/code-security/dependabot/dependabot-version-updates/configuration-options-for-the-dependabot.yml-file#groups. You can create groups to package dependency updates together into a single PR. Default: []
         :param ignore: (experimental) You can use the ``ignore`` option to customize which dependencies are updated. The ignore option supports the following options. Default: []
         :param ignore_projen: (experimental) Ignores updates to ``projen``. This is required since projen updates may cause changes in committed files and anti-tamper checks will fail. Projen upgrades are covered through the ``ProjenUpgrade`` class. Default: true
         :param labels: (experimental) List of labels to apply to the created PR's.
         :param open_pull_requests_limit: (experimental) Sets the maximum of pull requests Dependabot opens for version updates. Dependabot will not open any new requests until some of those open requests are merged or closed. Default: 5
         :param registries: (experimental) Map of package registries to use. Default: - use public registries
         :param reviewers: (experimental) Specify individual reviewers or teams of reviewers for all pull requests raised for a package manager. Default: []
         :param schedule_interval: (experimental) How often to check for new versions and raise pull requests. Default: ScheduleInterval.DAILY
+        :param target_branch: (experimental) https://docs.github.com/en/code-security/dependabot/dependabot-version-updates/configuration-options-for-the-dependabot.yml-file#target-branch You can configure the target branch for raising pull requests for version updates against.
         :param versioning_strategy: (experimental) The strategy to use when edits manifest and lock files. Default: VersioningStrategy.LOCKFILE_ONLY The default is to only update the lock file because package.json is controlled by projen and any outside updates will fail the build.
 
         :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d0078e67a79ce21c460b876a72b4fbd4a358306502062bdf9bdb13085805a3f2)
             check_type(argname="argument allow", value=allow, expected_type=type_hints["allow"])
@@ -1514,14 +1520,15 @@
             check_type(argname="argument ignore", value=ignore, expected_type=type_hints["ignore"])
             check_type(argname="argument ignore_projen", value=ignore_projen, expected_type=type_hints["ignore_projen"])
             check_type(argname="argument labels", value=labels, expected_type=type_hints["labels"])
             check_type(argname="argument open_pull_requests_limit", value=open_pull_requests_limit, expected_type=type_hints["open_pull_requests_limit"])
             check_type(argname="argument registries", value=registries, expected_type=type_hints["registries"])
             check_type(argname="argument reviewers", value=reviewers, expected_type=type_hints["reviewers"])
             check_type(argname="argument schedule_interval", value=schedule_interval, expected_type=type_hints["schedule_interval"])
+            check_type(argname="argument target_branch", value=target_branch, expected_type=type_hints["target_branch"])
             check_type(argname="argument versioning_strategy", value=versioning_strategy, expected_type=type_hints["versioning_strategy"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if allow is not None:
             self._values["allow"] = allow
         if assignees is not None:
             self._values["assignees"] = assignees
         if groups is not None:
@@ -1536,14 +1543,16 @@
             self._values["open_pull_requests_limit"] = open_pull_requests_limit
         if registries is not None:
             self._values["registries"] = registries
         if reviewers is not None:
             self._values["reviewers"] = reviewers
         if schedule_interval is not None:
             self._values["schedule_interval"] = schedule_interval
+        if target_branch is not None:
+            self._values["target_branch"] = target_branch
         if versioning_strategy is not None:
             self._values["versioning_strategy"] = versioning_strategy
 
     @builtins.property
     def allow(self) -> typing.Optional[typing.List[DependabotAllow]]:
         '''(experimental) https://docs.github.com/en/code-security/dependabot/dependabot-version-updates/configuration-options-for-the-dependabot.yml-file#allow.
 
@@ -1665,14 +1674,23 @@
 
         :stability: experimental
         '''
         result = self._values.get("schedule_interval")
         return typing.cast(typing.Optional["DependabotScheduleInterval"], result)
 
     @builtins.property
+    def target_branch(self) -> typing.Optional[builtins.str]:
+        '''(experimental) https://docs.github.com/en/code-security/dependabot/dependabot-version-updates/configuration-options-for-the-dependabot.yml-file#target-branch You can configure the target branch for raising pull requests for version updates against.
+
+        :stability: experimental
+        '''
+        result = self._values.get("target_branch")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def versioning_strategy(self) -> typing.Optional["VersioningStrategy"]:
         '''(experimental) The strategy to use when edits manifest and lock files.
 
         :default:
 
         VersioningStrategy.LOCKFILE_ONLY The default is to only update the
         lock file because package.json is controlled by projen and any outside
@@ -2356,27 +2374,29 @@
         ignore: typing.Optional[typing.Sequence[typing.Union[DependabotIgnore, typing.Dict[builtins.str, typing.Any]]]] = None,
         ignore_projen: typing.Optional[builtins.bool] = None,
         labels: typing.Optional[typing.Sequence[builtins.str]] = None,
         open_pull_requests_limit: typing.Optional[jsii.Number] = None,
         registries: typing.Optional[typing.Mapping[builtins.str, typing.Union[DependabotRegistry, typing.Dict[builtins.str, typing.Any]]]] = None,
         reviewers: typing.Optional[typing.Sequence[builtins.str]] = None,
         schedule_interval: typing.Optional[DependabotScheduleInterval] = None,
+        target_branch: typing.Optional[builtins.str] = None,
         versioning_strategy: typing.Optional["VersioningStrategy"] = None,
     ) -> Dependabot:
         '''
         :param allow: (experimental) https://docs.github.com/en/code-security/dependabot/dependabot-version-updates/configuration-options-for-the-dependabot.yml-file#allow. Use the allow option to customize which dependencies are updated. This applies to both version and security updates. Default: []
         :param assignees: (experimental) Specify individual assignees or teams of assignees for all pull requests raised for a package manager. Default: []
         :param groups: (experimental) https://docs.github.com/en/code-security/dependabot/dependabot-version-updates/configuration-options-for-the-dependabot.yml-file#groups. You can create groups to package dependency updates together into a single PR. Default: []
         :param ignore: (experimental) You can use the ``ignore`` option to customize which dependencies are updated. The ignore option supports the following options. Default: []
         :param ignore_projen: (experimental) Ignores updates to ``projen``. This is required since projen updates may cause changes in committed files and anti-tamper checks will fail. Projen upgrades are covered through the ``ProjenUpgrade`` class. Default: true
         :param labels: (experimental) List of labels to apply to the created PR's.
         :param open_pull_requests_limit: (experimental) Sets the maximum of pull requests Dependabot opens for version updates. Dependabot will not open any new requests until some of those open requests are merged or closed. Default: 5
         :param registries: (experimental) Map of package registries to use. Default: - use public registries
         :param reviewers: (experimental) Specify individual reviewers or teams of reviewers for all pull requests raised for a package manager. Default: []
         :param schedule_interval: (experimental) How often to check for new versions and raise pull requests. Default: ScheduleInterval.DAILY
+        :param target_branch: (experimental) https://docs.github.com/en/code-security/dependabot/dependabot-version-updates/configuration-options-for-the-dependabot.yml-file#target-branch You can configure the target branch for raising pull requests for version updates against.
         :param versioning_strategy: (experimental) The strategy to use when edits manifest and lock files. Default: VersioningStrategy.LOCKFILE_ONLY The default is to only update the lock file because package.json is controlled by projen and any outside updates will fail the build.
 
         :stability: experimental
         '''
         options = DependabotOptions(
             allow=allow,
             assignees=assignees,
@@ -2384,14 +2404,15 @@
             ignore=ignore,
             ignore_projen=ignore_projen,
             labels=labels,
             open_pull_requests_limit=open_pull_requests_limit,
             registries=registries,
             reviewers=reviewers,
             schedule_interval=schedule_interval,
+            target_branch=target_branch,
             versioning_strategy=versioning_strategy,
         )
 
         return typing.cast(Dependabot, jsii.invoke(self, "addDependabot", [options]))
 
     @jsii.member(jsii_name="addPullRequestTemplate")
     def add_pull_request_template(
@@ -8033,14 +8054,15 @@
     ignore: typing.Optional[typing.Sequence[typing.Union[DependabotIgnore, typing.Dict[builtins.str, typing.Any]]]] = None,
     ignore_projen: typing.Optional[builtins.bool] = None,
     labels: typing.Optional[typing.Sequence[builtins.str]] = None,
     open_pull_requests_limit: typing.Optional[jsii.Number] = None,
     registries: typing.Optional[typing.Mapping[builtins.str, typing.Union[DependabotRegistry, typing.Dict[builtins.str, typing.Any]]]] = None,
     reviewers: typing.Optional[typing.Sequence[builtins.str]] = None,
     schedule_interval: typing.Optional[DependabotScheduleInterval] = None,
+    target_branch: typing.Optional[builtins.str] = None,
     versioning_strategy: typing.Optional[VersioningStrategy] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__2f6be8925f643f55a433390fc13649104d3b8fc8654622add1c5222d49b92a79(
     dependency_name: builtins.str,
@@ -8086,14 +8108,15 @@
     ignore: typing.Optional[typing.Sequence[typing.Union[DependabotIgnore, typing.Dict[builtins.str, typing.Any]]]] = None,
     ignore_projen: typing.Optional[builtins.bool] = None,
     labels: typing.Optional[typing.Sequence[builtins.str]] = None,
     open_pull_requests_limit: typing.Optional[jsii.Number] = None,
     registries: typing.Optional[typing.Mapping[builtins.str, typing.Union[DependabotRegistry, typing.Dict[builtins.str, typing.Any]]]] = None,
     reviewers: typing.Optional[typing.Sequence[builtins.str]] = None,
     schedule_interval: typing.Optional[DependabotScheduleInterval] = None,
+    target_branch: typing.Optional[builtins.str] = None,
     versioning_strategy: typing.Optional[VersioningStrategy] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__71dcef0810bce091e26ea45c125fc125b6b541331dd4f1fa62466d1f52b108d4(
     *,
```

### Comparing `projen-0.81.1/src/projen/github/workflows/__init__.py` & `projen-0.81.2/src/projen/github/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.1/src/projen/gitlab/__init__.py` & `projen-0.81.2/src/projen/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.1/src/projen/java/__init__.py` & `projen-0.81.2/src/projen/java/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.1/src/projen/javascript/__init__.py` & `projen-0.81.2/src/projen/javascript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.1/src/projen/python/__init__.py` & `projen-0.81.2/src/projen/python/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.1/src/projen/release/__init__.py` & `projen-0.81.2/src/projen/release/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.1/src/projen/typescript/__init__.py` & `projen-0.81.2/src/projen/typescript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.1/src/projen/vscode/__init__.py` & `projen-0.81.2/src/projen/vscode/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.1/src/projen/web/__init__.py` & `projen-0.81.2/src/projen/web/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.1/src/projen.egg-info/PKG-INFO` & `projen-0.81.2/src/projen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.81.1
+Version: 0.81.2
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.81.1/src/projen.egg-info/SOURCES.txt` & `projen-0.81.2/src/projen.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/projen/py.typed
 src/projen.egg-info/PKG-INFO
 src/projen.egg-info/SOURCES.txt
 src/projen.egg-info/dependency_links.txt
 src/projen.egg-info/requires.txt
 src/projen.egg-info/top_level.txt
 src/projen/_jsii/__init__.py
-src/projen/_jsii/projen@0.81.1.jsii.tgz
+src/projen/_jsii/projen@0.81.2.jsii.tgz
 src/projen/_jsii/bin/projen
 src/projen/awscdk/__init__.py
 src/projen/build/__init__.py
 src/projen/cdk/__init__.py
 src/projen/cdk8s/__init__.py
 src/projen/cdktf/__init__.py
 src/projen/circleci/__init__.py
```

