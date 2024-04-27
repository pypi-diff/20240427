# Comparing `tmp/fastbench-0.1.1.tar.gz` & `tmp/fastbench-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastbench-0.1.1.tar", max compression
+gzip compressed data, was "fastbench-0.1.2.tar", max compression
```

## Comparing `fastbench-0.1.1.tar` & `fastbench-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1078 2024-04-27 10:59:06.527379 fastbench-0.1.1/LICENSE
--rw-r--r--   0        0        0     1913 2024-04-27 10:59:06.527379 fastbench-0.1.1/README.md
--rw-r--r--   0        0        0      670 2024-04-27 10:59:06.527379 fastbench-0.1.1/fastbench/__init__.py
--rw-r--r--   0        0        0      516 2024-04-27 10:59:06.527379 fastbench-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2256 1970-01-01 00:00:00.000000 fastbench-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-27 11:10:43.970360 fastbench-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1917 2024-04-27 11:10:43.970360 fastbench-0.1.2/README.md
+-rw-r--r--   0        0        0      670 2024-04-27 11:10:43.974360 fastbench-0.1.2/fastbench/__init__.py
+-rw-r--r--   0        0        0      516 2024-04-27 11:10:43.974360 fastbench-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2260 1970-01-01 00:00:00.000000 fastbench-0.1.2/PKG-INFO
```

### Comparing `fastbench-0.1.1/LICENSE` & `fastbench-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastbench-0.1.1/README.md` & `fastbench-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <h1 align="center">
   <br>
   <img src="https://raw.githubusercontent.com/itsmeadarsh2008/fastbench/main/truebench.svg" width="200" height="200">
   <br>
   TrueBench
-  
+  <br>
   <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/fastbench">
   <img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/itsmeadarsh2008/fastbench">
   <br>
 </h1>
 
 TrueBench is a high-performance Python package for benchmarking code execution time, CPU usage, and memory usage. It's implemented in Python for simplicity and provides a simple API for measuring the performance of your Python code.
```

### Comparing `fastbench-0.1.1/fastbench/__init__.py` & `fastbench-0.1.2/fastbench/__init__.py`

 * *Files identical despite different names*

### Comparing `fastbench-0.1.1/pyproject.toml` & `fastbench-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastbench"
-version = "0.1.1"
+version = "0.1.2"
 description = "A pure-python based benchmarking package for Python 🤪"
 authors = ["Adarsh Gourab Mahalik <gourabmahalikadarsh@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 psutil = "^5.9.8"
```

### Comparing `fastbench-0.1.1/PKG-INFO` & `fastbench-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: fastbench
-Version: 0.1.1
+Version: 0.1.2
 Summary: A pure-python based benchmarking package for Python 🤪
 Author: Adarsh Gourab Mahalik
 Author-email: gourabmahalikadarsh@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
   <img src="https://raw.githubusercontent.com/itsmeadarsh2008/fastbench/main/truebench.svg" width="200" height="200">
   <br>
   TrueBench
-  
+  <br>
   <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/fastbench">
   <img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/itsmeadarsh2008/fastbench">
   <br>
 </h1>
 
 TrueBench is a high-performance Python package for benchmarking code execution time, CPU usage, and memory usage. It's implemented in Python for simplicity and provides a simple API for measuring the performance of your Python code.
```

