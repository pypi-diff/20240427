# Comparing `tmp/tailucas_pylib-0.2.7.tar.gz` & `tmp/tailucas_pylib-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailucas_pylib-0.2.7.tar", max compression
+gzip compressed data, was "tailucas_pylib-0.2.8.tar", max compression
```

## Comparing `tailucas_pylib-0.2.7.tar` & `tailucas_pylib-0.2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1066 2023-08-31 19:44:41.375775 tailucas_pylib-0.2.7/LICENSE
--rw-r--r--   0        0        0    11403 2023-11-25 09:06:51.036540 tailucas_pylib-0.2.7/README.md
--rw-r--r--   0        0        0      571 2024-04-22 09:53:00.569504 tailucas_pylib-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     5454 2024-01-07 20:24:45.999553 tailucas_pylib-0.2.7/tailucas_pylib/__init__.py
--rw-r--r--   0        0        0     2148 2023-09-10 09:39:25.219973 tailucas_pylib-0.2.7/tailucas_pylib/app.py
--rw-r--r--   0        0        0     1218 2023-09-10 09:33:16.369962 tailucas_pylib-0.2.7/tailucas_pylib/aws/__init__.py
--rw-r--r--   0        0        0     1455 2023-09-10 09:49:11.549965 tailucas_pylib-0.2.7/tailucas_pylib/aws/metrics.py
--rw-r--r--   0        0        0     8727 2024-02-25 13:23:22.241361 tailucas_pylib-0.2.7/tailucas_pylib/aws/swf.py
--rw-r--r--   0        0        0     2427 2023-08-31 19:44:41.385775 tailucas_pylib-0.2.7/tailucas_pylib/bluetooth.py
--rw-r--r--   0        0        0      725 2023-12-29 14:58:54.907113 tailucas_pylib-0.2.7/tailucas_pylib/data.py
--rw-r--r--   0        0        0     3147 2023-08-31 19:44:41.385775 tailucas_pylib-0.2.7/tailucas_pylib/datetime.py
--rw-r--r--   0        0        0     3112 2023-09-10 09:47:03.819967 tailucas_pylib-0.2.7/tailucas_pylib/handler.py
--rw-r--r--   0        0        0     1009 2023-08-31 19:44:41.385775 tailucas_pylib-0.2.7/tailucas_pylib/process.py
--rw-r--r--   0        0        0     9521 2023-09-03 07:12:39.509088 tailucas_pylib-0.2.7/tailucas_pylib/rabbit.py
--rw-r--r--   0        0        0     5225 2024-04-22 09:52:31.109505 tailucas_pylib-0.2.7/tailucas_pylib/threads.py
--rw-r--r--   0        0        0     3387 2024-04-21 11:13:24.751872 tailucas_pylib-0.2.7/tailucas_pylib/zmq.py
--rw-r--r--   0        0        0    12344 1970-01-01 00:00:00.000000 tailucas_pylib-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-08-31 19:44:41.375775 tailucas_pylib-0.2.8/LICENSE
+-rw-r--r--   0        0        0    11403 2023-11-25 09:06:51.036540 tailucas_pylib-0.2.8/README.md
+-rw-r--r--   0        0        0      570 2024-04-27 06:25:58.535854 tailucas_pylib-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     5454 2024-01-07 20:24:45.999553 tailucas_pylib-0.2.8/tailucas_pylib/__init__.py
+-rw-r--r--   0        0        0     2148 2023-09-10 09:39:25.219973 tailucas_pylib-0.2.8/tailucas_pylib/app.py
+-rw-r--r--   0        0        0     1218 2023-09-10 09:33:16.369962 tailucas_pylib-0.2.8/tailucas_pylib/aws/__init__.py
+-rw-r--r--   0        0        0     1455 2023-09-10 09:49:11.549965 tailucas_pylib-0.2.8/tailucas_pylib/aws/metrics.py
+-rw-r--r--   0        0        0     8727 2024-02-25 13:23:22.241361 tailucas_pylib-0.2.8/tailucas_pylib/aws/swf.py
+-rw-r--r--   0        0        0     2427 2023-08-31 19:44:41.385775 tailucas_pylib-0.2.8/tailucas_pylib/bluetooth.py
+-rw-r--r--   0        0        0      725 2023-12-29 14:58:54.907113 tailucas_pylib-0.2.8/tailucas_pylib/data.py
+-rw-r--r--   0        0        0     3147 2023-08-31 19:44:41.385775 tailucas_pylib-0.2.8/tailucas_pylib/datetime.py
+-rw-r--r--   0        0        0     3112 2023-09-10 09:47:03.819967 tailucas_pylib-0.2.8/tailucas_pylib/handler.py
+-rw-r--r--   0        0        0     1009 2023-08-31 19:44:41.385775 tailucas_pylib-0.2.8/tailucas_pylib/process.py
+-rw-r--r--   0        0        0     9521 2023-09-03 07:12:39.509088 tailucas_pylib-0.2.8/tailucas_pylib/rabbit.py
+-rw-r--r--   0        0        0     5225 2024-04-22 09:52:31.109505 tailucas_pylib-0.2.8/tailucas_pylib/threads.py
+-rw-r--r--   0        0        0     3387 2024-04-21 11:13:24.751872 tailucas_pylib-0.2.8/tailucas_pylib/zmq.py
+-rw-r--r--   0        0        0    12343 1970-01-01 00:00:00.000000 tailucas_pylib-0.2.8/PKG-INFO
```

### Comparing `tailucas_pylib-0.2.7/LICENSE` & `tailucas_pylib-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.7/README.md` & `tailucas_pylib-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.7/pyproject.toml` & `tailucas_pylib-0.2.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "tailucas-pylib"
-version = "0.2.7"
+version = "0.2.8"
 description = "Common Python utility modules"
 authors = ["Tai Lucas <tglucas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 botoflow = "^0.8"
-boto3 = "^1.34.88"
+boto3 = "^1.34.93"
 cronitor = "^4.7.1"
 msgpack = "^1.0.8"
 onepasswordconnectsdk = "^1.5.1"
 pika = "^1.3.2"
 python-dateutil = "^2.9.0.post0"
 pytz = "^2024.1"
 pyzmq = "^26.0.2"
-sentry-sdk = "^1.45.0"
+sentry-sdk = "^2.0.1"
 simplejson = "^3.19.2"
 pyyaml = "^6.0.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tailucas_pylib-0.2.7/tailucas_pylib/__init__.py` & `tailucas_pylib-0.2.8/tailucas_pylib/__init__.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.7/tailucas_pylib/app.py` & `tailucas_pylib-0.2.8/tailucas_pylib/app.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.7/tailucas_pylib/aws/__init__.py` & `tailucas_pylib-0.2.8/tailucas_pylib/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.7/tailucas_pylib/aws/metrics.py` & `tailucas_pylib-0.2.8/tailucas_pylib/aws/metrics.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.7/tailucas_pylib/aws/swf.py` & `tailucas_pylib-0.2.8/tailucas_pylib/aws/swf.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.7/tailucas_pylib/bluetooth.py` & `tailucas_pylib-0.2.8/tailucas_pylib/bluetooth.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.7/tailucas_pylib/data.py` & `tailucas_pylib-0.2.8/tailucas_pylib/data.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.7/tailucas_pylib/datetime.py` & `tailucas_pylib-0.2.8/tailucas_pylib/datetime.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.7/tailucas_pylib/handler.py` & `tailucas_pylib-0.2.8/tailucas_pylib/handler.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.7/tailucas_pylib/process.py` & `tailucas_pylib-0.2.8/tailucas_pylib/process.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.7/tailucas_pylib/rabbit.py` & `tailucas_pylib-0.2.8/tailucas_pylib/rabbit.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.7/tailucas_pylib/threads.py` & `tailucas_pylib-0.2.8/tailucas_pylib/threads.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.7/tailucas_pylib/zmq.py` & `tailucas_pylib-0.2.8/tailucas_pylib/zmq.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.7/PKG-INFO` & `tailucas_pylib-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: tailucas-pylib
-Version: 0.2.7
+Version: 0.2.8
 Summary: Common Python utility modules
 License: MIT
 Author: Tai Lucas
 Author-email: tglucas@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: boto3 (>=1.34.88,<2.0.0)
+Requires-Dist: boto3 (>=1.34.93,<2.0.0)
 Requires-Dist: botoflow (>=0.8,<0.9)
 Requires-Dist: cronitor (>=4.7.1,<5.0.0)
 Requires-Dist: msgpack (>=1.0.8,<2.0.0)
 Requires-Dist: onepasswordconnectsdk (>=1.5.1,<2.0.0)
 Requires-Dist: pika (>=1.3.2,<2.0.0)
 Requires-Dist: python-dateutil (>=2.9.0.post0,<3.0.0)
 Requires-Dist: pytz (>=2024.1,<2025.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: pyzmq (>=26.0.2,<27.0.0)
-Requires-Dist: sentry-sdk (>=1.45.0,<2.0.0)
+Requires-Dist: sentry-sdk (>=2.0.1,<3.0.0)
 Requires-Dist: simplejson (>=3.19.2,<4.0.0)
 Description-Content-Type: text/markdown
 
 <a name="readme-top"></a>
 
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
```

