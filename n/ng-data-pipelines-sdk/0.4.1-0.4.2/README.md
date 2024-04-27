# Comparing `tmp/ng_data_pipelines_sdk-0.4.1.tar.gz` & `tmp/ng_data_pipelines_sdk-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng_data_pipelines_sdk-0.4.1.tar", max compression
+gzip compressed data, was "ng_data_pipelines_sdk-0.4.2.tar", max compression
```

## Comparing `ng_data_pipelines_sdk-0.4.1.tar` & `ng_data_pipelines_sdk-0.4.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      106 2024-04-27 18:54:03.234672 ng_data_pipelines_sdk-0.4.1/README.md
--rw-r--r--   0        0        0        0 2024-04-27 18:54:03.261672 ng_data_pipelines_sdk-0.4.1/ng_data_pipelines_sdk/__init__.py
--rw-r--r--   0        0        0     9155 2024-04-27 18:54:03.235672 ng_data_pipelines_sdk-0.4.1/ng_data_pipelines_sdk/aws_interface.py
--rw-r--r--   0        0        0      231 2024-04-27 18:54:03.235672 ng_data_pipelines_sdk-0.4.1/ng_data_pipelines_sdk/custom_logger.py
--rw-r--r--   0        0        0    26500 2024-04-27 18:54:03.235672 ng_data_pipelines_sdk-0.4.1/ng_data_pipelines_sdk/dataframe_manager.py
--rw-r--r--   0        0        0    15307 2024-04-27 18:54:03.235672 ng_data_pipelines_sdk-0.4.1/ng_data_pipelines_sdk/interfaces.py
--rw-r--r--   0        0        0     4648 2024-04-27 18:54:03.235672 ng_data_pipelines_sdk-0.4.1/ng_data_pipelines_sdk/spark_manager.py
--rw-r--r--   0        0        0     1453 2024-04-27 18:54:03.235672 ng_data_pipelines_sdk-0.4.1/ng_data_pipelines_sdk/utils.py
--rw-r--r--   0        0        0      672 2024-04-27 18:54:03.236672 ng_data_pipelines_sdk-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-04-27 19:06:03.389718 ng_data_pipelines_sdk-0.4.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-27 19:06:03.413718 ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/__init__.py
+-rw-r--r--   0        0        0     9155 2024-04-27 19:06:03.389718 ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/aws_interface.py
+-rw-r--r--   0        0        0      231 2024-04-27 19:06:03.389718 ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/custom_logger.py
+-rw-r--r--   0        0        0    26500 2024-04-27 19:06:03.389718 ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/dataframe_manager.py
+-rw-r--r--   0        0        0    15377 2024-04-27 19:06:03.389718 ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/interfaces.py
+-rw-r--r--   0        0        0     4648 2024-04-27 19:06:03.389718 ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/spark_manager.py
+-rw-r--r--   0        0        0     1453 2024-04-27 19:06:03.389718 ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/utils.py
+-rw-r--r--   0        0        0      672 2024-04-27 19:06:03.391718 ng_data_pipelines_sdk-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.4.2/PKG-INFO
```

### Comparing `ng_data_pipelines_sdk-0.4.1/ng_data_pipelines_sdk/aws_interface.py` & `ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.4.1/ng_data_pipelines_sdk/dataframe_manager.py` & `ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/dataframe_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.4.1/ng_data_pipelines_sdk/interfaces.py` & `ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -412,15 +412,15 @@
         ):
             raise ValueError(
                 "Function must have a DataFrame type hint as first parameter and return type hint, or a dict of [str, DataFrame] as first parameter hint and return type hint"
             )
 
         if first_param_kind != FnKind.SINGLE and apply_only_on is not None:
             raise ValueError(
-                "'apply_only_on' should be passed only when 'transform_function' has a DataFrame as first parameter, not a list of DataFrames"
+                "'apply_only_on' is only accepted when 'transform_function' is of type 'single', that is, when the first parameter is a DataFrame type hint and the return type hint is also a DataFrame type hint."
             )
 
         # If the function has a DataFrame as first parameter, then it is a single function. If it has a dict of [str, DataFrame] as first parameter, then it is a batch function
         # TODO: This should be a private attribute
         data["fn_kind"] = first_param_kind
 
         return data
```

### Comparing `ng_data_pipelines_sdk-0.4.1/ng_data_pipelines_sdk/spark_manager.py` & `ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/spark_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.4.1/ng_data_pipelines_sdk/utils.py` & `ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.4.1/pyproject.toml` & `ng_data_pipelines_sdk-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ng-data-pipelines-sdk"
-version = "0.4.1"
+version = "0.4.2"
 description = "A library for facilitating the development of data engineering pipelines using pyspark. Compatible with MWAA running airflow 2.8.1."
 authors = ["ng.cash"]
 readme = "README.md"
 exclude = [".git/", ".gitignore", "tests/", "docs/", "*.yml", "__pycache__/", "*.pyc", "*.ipynb", "playground/", "poetry.lock", "dist/", "build/"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
```

### Comparing `ng_data_pipelines_sdk-0.4.1/PKG-INFO` & `ng_data_pipelines_sdk-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ng-data-pipelines-sdk
-Version: 0.4.1
+Version: 0.4.2
 Summary: A library for facilitating the development of data engineering pipelines using pyspark. Compatible with MWAA running airflow 2.8.1.
 Author: ng.cash
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

