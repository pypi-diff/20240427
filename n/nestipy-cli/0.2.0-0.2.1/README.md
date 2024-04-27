# Comparing `tmp/nestipy_cli-0.2.0.tar.gz` & `tmp/nestipy_cli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy_cli-0.2.0.tar", max compression
+gzip compressed data, was "nestipy_cli-0.2.1.tar", max compression
```

## Comparing `nestipy_cli-0.2.0.tar` & `nestipy_cli-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0        0 2024-04-15 07:59:02.892079 nestipy_cli-0.2.0/README.md
--rw-r--r--   0        0        0      647 2024-04-26 13:48:40.614231 nestipy_cli-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 17:11:04.969253 nestipy_cli-0.2.0/src/nestipy_cli/__init__.py
--rw-r--r--   0        0        0     2769 2024-04-26 12:11:10.721587 nestipy_cli-0.2.0/src/nestipy_cli/cli.py
--rw-r--r--   0        0        0     5054 2024-04-17 13:42:24.077471 nestipy_cli-0.2.0/src/nestipy_cli/handler.py
--rw-r--r--   0        0        0      502 2024-02-29 12:35:05.153461 nestipy_cli-0.2.0/src/nestipy_cli/style.py
--rw-r--r--   0        0        0        0 2024-04-13 17:11:04.977253 nestipy_cli-0.2.0/src/nestipy_cli/templates/__init__.py
--rw-r--r--   0        0        0      184 2024-04-17 12:09:31.875788 nestipy_cli-0.2.0/src/nestipy_cli/templates/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2906 2024-04-17 12:09:31.875788 nestipy_cli-0.2.0/src/nestipy_cli/templates/__pycache__/generator.cpython-311.pyc
--rw-r--r--   0        0        0     1068 2024-04-13 17:11:04.969253 nestipy_cli-0.2.0/src/nestipy_cli/templates/generator.py
--rw-r--r--   0        0        0      988 2024-04-26 13:46:00.142205 nestipy_cli-0.2.0/src/nestipy_cli/templates/project/README.md
--rw-r--r--   0        0        0        0 2024-04-13 17:11:04.977253 nestipy_cli-0.2.0/src/nestipy_cli/templates/project/__init__.py
--rw-r--r--   0        0        0      192 2024-04-22 08:09:23.913452 nestipy_cli-0.2.0/src/nestipy_cli/templates/project/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1301 2024-04-23 14:58:38.932547 nestipy_cli-0.2.0/src/nestipy_cli/templates/project/__pycache__/app_service.cpython-311.pyc
--rw-r--r--   0        0        0      694 2024-04-24 10:33:50.721429 nestipy_cli-0.2.0/src/nestipy_cli/templates/project/app_controller.py
--rw-r--r--   0        0        0      209 2024-04-24 10:34:01.977450 nestipy_cli-0.2.0/src/nestipy_cli/templates/project/app_module.py
--rw-r--r--   0        0        0      374 2024-04-24 10:34:09.977466 nestipy_cli-0.2.0/src/nestipy_cli/templates/project/app_service.py
--rw-r--r--   0        0        0      225 2024-04-24 10:34:14.393474 nestipy_cli-0.2.0/src/nestipy_cli/templates/project/main.py
--rw-r--r--   0        0        0       14 2024-04-26 13:43:35.466113 nestipy_cli-0.2.0/src/nestipy_cli/templates/project/requirements.txt
--rw-r--r--   0        0        0        0 2024-04-13 17:11:04.977253 nestipy_cli-0.2.0/src/nestipy_cli/templates/project/src/__init__.py
--rw-r--r--   0        0        0     1078 2024-04-24 10:34:41.397526 nestipy_cli-0.2.0/src/nestipy_cli/templates/views/controller.txt
--rw-r--r--   0        0        0      187 2024-04-13 17:11:04.969253 nestipy_cli-0.2.0/src/nestipy_cli/templates/views/dto.txt
--rw-r--r--   0        0        0      311 2024-04-13 17:11:04.969253 nestipy_cli-0.2.0/src/nestipy_cli/templates/views/graphql_module.txt
--rw-r--r--   0        0        0      294 2024-04-13 17:11:04.969253 nestipy_cli-0.2.0/src/nestipy_cli/templates/views/graphql_service.txt
--rw-r--r--   0        0        0      102 2024-04-26 08:24:54.367660 nestipy_cli-0.2.0/src/nestipy_cli/templates/views/input.txt
--rw-r--r--   0        0        0      312 2024-04-13 17:11:04.969253 nestipy_cli-0.2.0/src/nestipy_cli/templates/views/module.txt
--rw-r--r--   0        0        0      575 2024-04-26 08:22:46.303518 nestipy_cli-0.2.0/src/nestipy_cli/templates/views/resolver.txt
--rw-r--r--   0        0        0      471 2024-04-17 13:29:07.960343 nestipy_cli-0.2.0/src/nestipy_cli/templates/views/service.txt
--rw-r--r--   0        0        0      168 2024-04-13 17:11:04.969253 nestipy_cli-0.2.0/src/nestipy_cli/templates/views/single_controller.txt
--rw-r--r--   0        0        0       86 2024-04-13 17:11:04.969253 nestipy_cli-0.2.0/src/nestipy_cli/templates/views/single_module.txt
--rw-r--r--   0        0        0      303 2024-04-13 17:11:04.969253 nestipy_cli-0.2.0/src/nestipy_cli/templates/views/single_resolver.txt
--rw-r--r--   0        0        0      127 2024-04-13 17:11:04.969253 nestipy_cli-0.2.0/src/nestipy_cli/templates/views/single_service.txt
--rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 nestipy_cli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 07:59:02.892079 nestipy_cli-0.2.1/README.md
+-rw-r--r--   0        0        0      647 2024-04-27 15:47:45.800856 nestipy_cli-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-13 17:11:04.969253 nestipy_cli-0.2.1/src/nestipy_cli/__init__.py
+-rw-r--r--   0        0        0     2769 2024-04-26 12:11:10.721587 nestipy_cli-0.2.1/src/nestipy_cli/cli.py
+-rw-r--r--   0        0        0     5054 2024-04-17 13:42:24.077471 nestipy_cli-0.2.1/src/nestipy_cli/handler.py
+-rw-r--r--   0        0        0      502 2024-02-29 12:35:05.153461 nestipy_cli-0.2.1/src/nestipy_cli/style.py
+-rw-r--r--   0        0        0        0 2024-04-13 17:11:04.977253 nestipy_cli-0.2.1/src/nestipy_cli/templates/__init__.py
+-rw-r--r--   0        0        0      184 2024-04-17 12:09:31.875788 nestipy_cli-0.2.1/src/nestipy_cli/templates/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2906 2024-04-17 12:09:31.875788 nestipy_cli-0.2.1/src/nestipy_cli/templates/__pycache__/generator.cpython-311.pyc
+-rw-r--r--   0        0        0     1068 2024-04-13 17:11:04.969253 nestipy_cli-0.2.1/src/nestipy_cli/templates/generator.py
+-rw-r--r--   0        0        0      988 2024-04-26 13:46:00.142205 nestipy_cli-0.2.1/src/nestipy_cli/templates/project/README.md
+-rw-r--r--   0        0        0        0 2024-04-13 17:11:04.977253 nestipy_cli-0.2.1/src/nestipy_cli/templates/project/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-22 08:09:23.913452 nestipy_cli-0.2.1/src/nestipy_cli/templates/project/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1301 2024-04-23 14:58:38.932547 nestipy_cli-0.2.1/src/nestipy_cli/templates/project/__pycache__/app_service.cpython-311.pyc
+-rw-r--r--   0        0        0      694 2024-04-24 10:33:50.721429 nestipy_cli-0.2.1/src/nestipy_cli/templates/project/app_controller.py
+-rw-r--r--   0        0        0      209 2024-04-24 10:34:01.977450 nestipy_cli-0.2.1/src/nestipy_cli/templates/project/app_module.py
+-rw-r--r--   0        0        0      374 2024-04-24 10:34:09.977466 nestipy_cli-0.2.1/src/nestipy_cli/templates/project/app_service.py
+-rw-r--r--   0        0        0      225 2024-04-24 10:34:14.393474 nestipy_cli-0.2.1/src/nestipy_cli/templates/project/main.py
+-rw-r--r--   0        0        0       14 2024-04-26 13:43:35.466113 nestipy_cli-0.2.1/src/nestipy_cli/templates/project/requirements.txt
+-rw-r--r--   0        0        0        0 2024-04-13 17:11:04.977253 nestipy_cli-0.2.1/src/nestipy_cli/templates/project/src/__init__.py
+-rw-r--r--   0        0        0     1078 2024-04-24 10:34:41.397526 nestipy_cli-0.2.1/src/nestipy_cli/templates/views/controller.txt
+-rw-r--r--   0        0        0      187 2024-04-13 17:11:04.969253 nestipy_cli-0.2.1/src/nestipy_cli/templates/views/dto.txt
+-rw-r--r--   0        0        0      311 2024-04-13 17:11:04.969253 nestipy_cli-0.2.1/src/nestipy_cli/templates/views/graphql_module.txt
+-rw-r--r--   0        0        0      294 2024-04-13 17:11:04.969253 nestipy_cli-0.2.1/src/nestipy_cli/templates/views/graphql_service.txt
+-rw-r--r--   0        0        0      102 2024-04-26 08:24:54.367660 nestipy_cli-0.2.1/src/nestipy_cli/templates/views/input.txt
+-rw-r--r--   0        0        0      312 2024-04-13 17:11:04.969253 nestipy_cli-0.2.1/src/nestipy_cli/templates/views/module.txt
+-rw-r--r--   0        0        0      575 2024-04-26 08:22:46.303518 nestipy_cli-0.2.1/src/nestipy_cli/templates/views/resolver.txt
+-rw-r--r--   0        0        0      471 2024-04-17 13:29:07.960343 nestipy_cli-0.2.1/src/nestipy_cli/templates/views/service.txt
+-rw-r--r--   0        0        0      168 2024-04-13 17:11:04.969253 nestipy_cli-0.2.1/src/nestipy_cli/templates/views/single_controller.txt
+-rw-r--r--   0        0        0       86 2024-04-13 17:11:04.969253 nestipy_cli-0.2.1/src/nestipy_cli/templates/views/single_module.txt
+-rw-r--r--   0        0        0      303 2024-04-13 17:11:04.969253 nestipy_cli-0.2.1/src/nestipy_cli/templates/views/single_resolver.txt
+-rw-r--r--   0        0        0      127 2024-04-13 17:11:04.969253 nestipy_cli-0.2.1/src/nestipy_cli/templates/views/single_service.txt
+-rw-r--r--   0        0        0      827 1970-01-01 00:00:00.000000 nestipy_cli-0.2.1/PKG-INFO
```

### Comparing `nestipy_cli-0.2.0/pyproject.toml` & `nestipy_cli-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "nestipy-cli"
-version = "0.2.0"
+version = "0.2.1"
 description = "Nestipy is a Python framework built on top of FastAPI that follows the modular architecture of NestJS"
 authors = ["tsiresymila <tsiresymila@gmail.com>"]
 readme = "README.md"
 packages = [{include = "nestipy_cli", from = "src"}]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 click = "^8.1.7"
 minijinja = "^1.0.16"
 click-aliases = "^1.0.4"
 questionary = "^2.0.1"
 aiofile = "^3.8.8"
 autoflake = "^2.3.1"
 isort = "^5.13.2"
```

### Comparing `nestipy_cli-0.2.0/src/nestipy_cli/cli.py` & `nestipy_cli-0.2.1/src/nestipy_cli/cli.py`

 * *Files identical despite different names*

### Comparing `nestipy_cli-0.2.0/src/nestipy_cli/handler.py` & `nestipy_cli-0.2.1/src/nestipy_cli/handler.py`

 * *Files identical despite different names*

### Comparing `nestipy_cli-0.2.0/src/nestipy_cli/templates/__pycache__/generator.cpython-311.pyc` & `nestipy_cli-0.2.1/src/nestipy_cli/templates/__pycache__/generator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy_cli-0.2.0/src/nestipy_cli/templates/generator.py` & `nestipy_cli-0.2.1/src/nestipy_cli/templates/generator.py`

 * *Files identical despite different names*

### Comparing `nestipy_cli-0.2.0/src/nestipy_cli/templates/project/README.md` & `nestipy_cli-0.2.1/src/nestipy_cli/templates/project/README.md`

 * *Files identical despite different names*

### Comparing `nestipy_cli-0.2.0/src/nestipy_cli/templates/project/__pycache__/app_service.cpython-311.pyc` & `nestipy_cli-0.2.1/src/nestipy_cli/templates/project/__pycache__/app_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy_cli-0.2.0/src/nestipy_cli/templates/project/app_controller.py` & `nestipy_cli-0.2.1/src/nestipy_cli/templates/project/app_controller.py`

 * *Files identical despite different names*

### Comparing `nestipy_cli-0.2.0/src/nestipy_cli/templates/views/controller.txt` & `nestipy_cli-0.2.1/src/nestipy_cli/templates/views/controller.txt`

 * *Files identical despite different names*

### Comparing `nestipy_cli-0.2.0/src/nestipy_cli/templates/views/resolver.txt` & `nestipy_cli-0.2.1/src/nestipy_cli/templates/views/resolver.txt`

 * *Files identical despite different names*

### Comparing `nestipy_cli-0.2.0/PKG-INFO` & `nestipy_cli-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: nestipy-cli
-Version: 0.2.0
+Version: 0.2.1
 Summary: Nestipy is a Python framework built on top of FastAPI that follows the modular architecture of NestJS
 Author: tsiresymila
 Author-email: tsiresymila@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofile (>=3.8.8,<4.0.0)
 Requires-Dist: autoflake (>=2.3.1,<3.0.0)
 Requires-Dist: autopep8 (>=2.1.0,<3.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: click-aliases (>=1.0.4,<2.0.0)
```
