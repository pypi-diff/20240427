# Comparing `tmp/truefoundry-0.2.0rc7.tar.gz` & `tmp/truefoundry-0.2.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truefoundry-0.2.0rc7.tar", max compression
+gzip compressed data, was "truefoundry-0.2.0rc8.tar", max compression
```

## Comparing `truefoundry-0.2.0rc7.tar` & `truefoundry-0.2.0rc8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      871 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/README.md
--rw-r--r--   0        0        0     1170 2024-04-23 09:54:31.265832 truefoundry-0.2.0rc7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/autodeploy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/autodeploy/agents/__init__.py
--rw-r--r--   0        0        0     6405 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/autodeploy/agents/base.py
--rw-r--r--   0        0        0     4126 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/autodeploy/agents/developer.py
--rw-r--r--   0        0        0     4438 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/autodeploy/agents/project_identifier.py
--rw-r--r--   0        0        0     2352 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/autodeploy/agents/tester.py
--rw-r--r--   0        0        0    12317 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/autodeploy/cli.py
--rw-r--r--   0        0        0     1111 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/autodeploy/constants.py
--rw-r--r--   0        0        0       54 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/autodeploy/exception.py
--rw-r--r--   0        0        0      325 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/autodeploy/logger.py
--rw-r--r--   0        0        0      875 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/autodeploy/tools/__init__.py
--rw-r--r--   0        0        0      856 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/autodeploy/tools/ask.py
--rw-r--r--   0        0        0      665 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/autodeploy/tools/base.py
--rw-r--r--   0        0        0     5892 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/autodeploy/tools/commit.py
--rw-r--r--   0        0        0     3931 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/autodeploy/tools/docker_build.py
--rw-r--r--   0        0        0     5078 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/autodeploy/tools/docker_run.py
--rw-r--r--   0        0        0     2288 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/autodeploy/tools/file_type_counts.py
--rw-r--r--   0        0        0     2577 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/autodeploy/tools/list_files.py
--rw-r--r--   0        0        0     1751 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/autodeploy/tools/read_file.py
--rw-r--r--   0        0        0     1614 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/autodeploy/tools/send_request.py
--rw-r--r--   0        0        0     3130 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/autodeploy/tools/write_file.py
--rw-r--r--   0        0        0     5358 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/autodeploy/utils/diff.py
--rw-r--r--   0        0        0      412 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/autodeploy/utils/pydantic_compat.py
--rw-r--r--   0        0        0        0 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/cli/__init__.py
--rw-r--r--   0        0        0      916 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/cli/__main__.py
--rw-r--r--   0        0        0       43 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/deploy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/deploy/cli/__init__.py
--rw-r--r--   0        0        0     2994 2024-04-23 09:54:17.129713 truefoundry-0.2.0rc7/truefoundry/deploy/cli/cli.py
--rw-r--r--   0        0        0     5524 2024-04-23 09:54:17.133713 truefoundry-0.2.0rc7/truefoundry/deploy/cli/deploy.py
--rw-r--r--   0        0        0       53 2024-04-23 09:54:17.133713 truefoundry-0.2.0rc7/truefoundry/langchain/__init__.py
--rw-r--r--   0        0        0      179 2024-04-23 09:54:17.133713 truefoundry-0.2.0rc7/truefoundry/ml/__init__.py
--rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 truefoundry-0.2.0rc7/PKG-INFO
+-rw-r--r--   0        0        0      871 2024-04-26 13:38:33.433473 truefoundry-0.2.0rc8/README.md
+-rw-r--r--   0        0        0     1170 2024-04-26 13:38:45.073514 truefoundry-0.2.0rc8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-26 13:38:33.433473 truefoundry-0.2.0rc8/truefoundry/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:38:33.433473 truefoundry-0.2.0rc8/truefoundry/autodeploy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:38:33.433473 truefoundry-0.2.0rc8/truefoundry/autodeploy/agents/__init__.py
+-rw-r--r--   0        0        0     6405 2024-04-26 13:38:33.433473 truefoundry-0.2.0rc8/truefoundry/autodeploy/agents/base.py
+-rw-r--r--   0        0        0     4126 2024-04-26 13:38:33.433473 truefoundry-0.2.0rc8/truefoundry/autodeploy/agents/developer.py
+-rw-r--r--   0        0        0     4438 2024-04-26 13:38:33.433473 truefoundry-0.2.0rc8/truefoundry/autodeploy/agents/project_identifier.py
+-rw-r--r--   0        0        0     2352 2024-04-26 13:38:33.433473 truefoundry-0.2.0rc8/truefoundry/autodeploy/agents/tester.py
+-rw-r--r--   0        0        0    12317 2024-04-26 13:38:33.433473 truefoundry-0.2.0rc8/truefoundry/autodeploy/cli.py
+-rw-r--r--   0        0        0     1111 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/constants.py
+-rw-r--r--   0        0        0       54 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/exception.py
+-rw-r--r--   0        0        0      325 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/logger.py
+-rw-r--r--   0        0        0      875 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/__init__.py
+-rw-r--r--   0        0        0      856 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/ask.py
+-rw-r--r--   0        0        0      665 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/base.py
+-rw-r--r--   0        0        0     5892 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/commit.py
+-rw-r--r--   0        0        0     3931 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/docker_build.py
+-rw-r--r--   0        0        0     5078 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/docker_run.py
+-rw-r--r--   0        0        0     2288 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/file_type_counts.py
+-rw-r--r--   0        0        0     2577 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/list_files.py
+-rw-r--r--   0        0        0     1751 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/read_file.py
+-rw-r--r--   0        0        0     1614 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/send_request.py
+-rw-r--r--   0        0        0     3130 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/write_file.py
+-rw-r--r--   0        0        0     5358 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/utils/diff.py
+-rw-r--r--   0        0        0      412 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/utils/pydantic_compat.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/cli/__init__.py
+-rw-r--r--   0        0        0      916 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/cli/__main__.py
+-rw-r--r--   0        0        0       43 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/deploy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/deploy/cli/__init__.py
+-rw-r--r--   0        0        0     2994 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/deploy/cli/cli.py
+-rw-r--r--   0        0        0     5524 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/deploy/cli/deploy.py
+-rw-r--r--   0        0        0       53 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/langchain/__init__.py
+-rw-r--r--   0        0        0      179 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/ml/__init__.py
+-rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 truefoundry-0.2.0rc8/PKG-INFO
```

### Comparing `truefoundry-0.2.0rc7/README.md` & `truefoundry-0.2.0rc8/README.md`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc7/pyproject.toml` & `truefoundry-0.2.0rc8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truefoundry"
-version = "0.2.0rc7"
+version = "0.2.0rc8"
 description = "Truefoundry CLI"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1,<3.13"
 servicefoundry = "0.10.10"
```

### Comparing `truefoundry-0.2.0rc7/truefoundry/autodeploy/agents/base.py` & `truefoundry-0.2.0rc8/truefoundry/autodeploy/agents/base.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc7/truefoundry/autodeploy/agents/developer.py` & `truefoundry-0.2.0rc8/truefoundry/autodeploy/agents/developer.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc7/truefoundry/autodeploy/agents/project_identifier.py` & `truefoundry-0.2.0rc8/truefoundry/autodeploy/agents/project_identifier.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc7/truefoundry/autodeploy/agents/tester.py` & `truefoundry-0.2.0rc8/truefoundry/autodeploy/agents/tester.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc7/truefoundry/autodeploy/cli.py` & `truefoundry-0.2.0rc8/truefoundry/autodeploy/cli.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc7/truefoundry/autodeploy/constants.py` & `truefoundry-0.2.0rc8/truefoundry/autodeploy/constants.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc7/truefoundry/autodeploy/tools/__init__.py` & `truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc7/truefoundry/autodeploy/tools/ask.py` & `truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/ask.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc7/truefoundry/autodeploy/tools/base.py` & `truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/base.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc7/truefoundry/autodeploy/tools/commit.py` & `truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/commit.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc7/truefoundry/autodeploy/tools/docker_build.py` & `truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/docker_build.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc7/truefoundry/autodeploy/tools/docker_run.py` & `truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/docker_run.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc7/truefoundry/autodeploy/tools/file_type_counts.py` & `truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/file_type_counts.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc7/truefoundry/autodeploy/tools/list_files.py` & `truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/list_files.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc7/truefoundry/autodeploy/tools/read_file.py` & `truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/read_file.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc7/truefoundry/autodeploy/tools/send_request.py` & `truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/send_request.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc7/truefoundry/autodeploy/tools/write_file.py` & `truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/write_file.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc7/truefoundry/autodeploy/utils/diff.py` & `truefoundry-0.2.0rc8/truefoundry/autodeploy/utils/diff.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc7/truefoundry/cli/__main__.py` & `truefoundry-0.2.0rc8/truefoundry/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc7/truefoundry/deploy/cli/cli.py` & `truefoundry-0.2.0rc8/truefoundry/deploy/cli/cli.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc7/truefoundry/deploy/cli/deploy.py` & `truefoundry-0.2.0rc8/truefoundry/deploy/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc7/PKG-INFO` & `truefoundry-0.2.0rc8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truefoundry
-Version: 0.2.0rc7
+Version: 0.2.0rc8
 Summary: Truefoundry CLI
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.8.1,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

