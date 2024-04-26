# Comparing `tmp/knockofforigins-0.1.0.tar.gz` & `tmp/knockofforigins-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knockofforigins-0.1.0.tar", max compression
+gzip compressed data, was "knockofforigins-0.1.1.tar", max compression
```

## Comparing `knockofforigins-0.1.0.tar` & `knockofforigins-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1069 2024-04-26 20:50:14.680887 knockofforigins-0.1.0/LICENSE
--rw-r--r--   0        0        0     3669 2024-04-26 20:46:06.696480 knockofforigins-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-26 21:46:15.138438 knockofforigins-0.1.0/knockofforigins/__init__.py
--rw-r--r--   0        0        0     3555 2024-04-26 21:46:15.138438 knockofforigins-0.1.0/knockofforigins/data_gen.py
--rw-r--r--   0        0        0     2829 2024-04-26 21:46:15.138438 knockofforigins-0.1.0/knockofforigins/decompose.py
--rw-r--r--   0        0        0        0 2024-04-26 21:46:15.138438 knockofforigins-0.1.0/knockofforigins/evaluation.py
--rw-r--r--   0        0        0     1267 2024-04-26 21:46:15.138438 knockofforigins-0.1.0/knockofforigins/gram_matrix.py
--rw-r--r--   0        0        0        0 2024-04-26 21:46:15.139438 knockofforigins-0.1.0/knockofforigins/knockoff.py
--rw-r--r--   0        0        0     2659 2024-04-26 21:48:10.588247 knockofforigins-0.1.0/knockofforigins/knockoff_construct.py
--rw-r--r--   0        0        0     1499 2024-04-26 21:46:15.139438 knockofforigins-0.1.0/knockofforigins/lasso.py
--rw-r--r--   0        0        0        0 2024-04-26 21:46:15.139438 knockofforigins-0.1.0/knockofforigins/plots.py
--rw-r--r--   0        0        0        0 2024-04-26 21:46:15.139438 knockofforigins-0.1.0/knockofforigins/testatistics.py
--rw-r--r--   0        0        0        0 2024-04-26 21:46:15.139438 knockofforigins-0.1.0/knockofforigins/utils.py
--rw-r--r--   0        0        0      965 2024-04-26 21:48:09.077138 knockofforigins-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4855 1970-01-01 00:00:00.000000 knockofforigins-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-26 20:50:14.680887 knockofforigins-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3669 2024-04-26 20:46:06.696480 knockofforigins-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-26 21:46:15.138438 knockofforigins-0.1.1/knockofforigins/__init__.py
+-rw-r--r--   0        0        0     3555 2024-04-26 21:46:15.138438 knockofforigins-0.1.1/knockofforigins/data_gen.py
+-rw-r--r--   0        0        0     2829 2024-04-26 21:46:15.138438 knockofforigins-0.1.1/knockofforigins/decompose.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:46:15.138438 knockofforigins-0.1.1/knockofforigins/evaluation.py
+-rw-r--r--   0        0        0     1267 2024-04-26 21:46:15.138438 knockofforigins-0.1.1/knockofforigins/gram_matrix.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:46:15.139438 knockofforigins-0.1.1/knockofforigins/knockoff.py
+-rw-r--r--   0        0        0     2659 2024-04-26 21:48:10.588247 knockofforigins-0.1.1/knockofforigins/knockoff_construct.py
+-rw-r--r--   0        0        0     1499 2024-04-26 21:46:15.139438 knockofforigins-0.1.1/knockofforigins/lasso.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:46:15.139438 knockofforigins-0.1.1/knockofforigins/plots.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:46:15.139438 knockofforigins-0.1.1/knockofforigins/testatistics.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:46:15.139438 knockofforigins-0.1.1/knockofforigins/utils.py
+-rw-r--r--   0        0        0      965 2024-04-26 22:07:04.893770 knockofforigins-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4855 1970-01-01 00:00:00.000000 knockofforigins-0.1.1/PKG-INFO
```

### Comparing `knockofforigins-0.1.0/LICENSE` & `knockofforigins-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `knockofforigins-0.1.0/README.md` & `knockofforigins-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `knockofforigins-0.1.0/knockofforigins/data_gen.py` & `knockofforigins-0.1.1/knockofforigins/data_gen.py`

 * *Files identical despite different names*

### Comparing `knockofforigins-0.1.0/knockofforigins/decompose.py` & `knockofforigins-0.1.1/knockofforigins/decompose.py`

 * *Files identical despite different names*

### Comparing `knockofforigins-0.1.0/knockofforigins/gram_matrix.py` & `knockofforigins-0.1.1/knockofforigins/gram_matrix.py`

 * *Files identical despite different names*

### Comparing `knockofforigins-0.1.0/knockofforigins/knockoff_construct.py` & `knockofforigins-0.1.1/knockofforigins/knockoff_construct.py`

 * *Files identical despite different names*

### Comparing `knockofforigins-0.1.0/knockofforigins/lasso.py` & `knockofforigins-0.1.1/knockofforigins/lasso.py`

 * *Files identical despite different names*

### Comparing `knockofforigins-0.1.0/pyproject.toml` & `knockofforigins-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "KnockoffOrigins"
-version = "0.1.0"
+version = "0.1.1"
 description = "This repository is dedicated to implementing the methodologies from the 2015 paper \"False Discovery Rate via Knockoffs\". It provides code for generating knockoff features and applying selection procedures. The aim is to help users understand and apply the knockoff method for feature selection. Please refer to the original paper for a complete understanding."
 authors = ["Javad Razi <j.razi@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jrazi/KnockoffOrigins"
 
 [tool.poetry.dependencies]
```

### Comparing `knockofforigins-0.1.0/PKG-INFO` & `knockofforigins-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knockofforigins
-Version: 0.1.0
+Version: 0.1.1
 Summary: This repository is dedicated to implementing the methodologies from the 2015 paper "False Discovery Rate via Knockoffs". It provides code for generating knockoff features and applying selection procedures. The aim is to help users understand and apply the knockoff method for feature selection. Please refer to the original paper for a complete understanding.
 Home-page: https://github.com/jrazi/KnockoffOrigins
 License: MIT
 Author: Javad Razi
 Author-email: j.razi@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

