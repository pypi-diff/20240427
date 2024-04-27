# Comparing `tmp/ng_data_pipelines_sdk-0.2.0.tar.gz` & `tmp/ng_data_pipelines_sdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng_data_pipelines_sdk-0.2.0.tar", max compression
+gzip compressed data, was "ng_data_pipelines_sdk-0.3.0.tar", max compression
```

## Comparing `ng_data_pipelines_sdk-0.2.0.tar` & `ng_data_pipelines_sdk-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      106 2024-04-26 14:50:23.986738 ng_data_pipelines_sdk-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-04-26 14:50:24.014738 ng_data_pipelines_sdk-0.2.0/ng_data_pipelines_sdk/__init__.py
--rw-r--r--   0        0        0     4932 2024-04-26 14:50:23.986738 ng_data_pipelines_sdk-0.2.0/ng_data_pipelines_sdk/aws_interface.py
--rw-r--r--   0        0        0      231 2024-04-26 14:50:23.986738 ng_data_pipelines_sdk-0.2.0/ng_data_pipelines_sdk/custom_logger.py
--rw-r--r--   0        0        0    25929 2024-04-26 14:50:23.986738 ng_data_pipelines_sdk-0.2.0/ng_data_pipelines_sdk/dataframe_manager.py
--rw-r--r--   0        0        0     8138 2024-04-26 14:50:23.986738 ng_data_pipelines_sdk-0.2.0/ng_data_pipelines_sdk/interfaces.py
--rw-r--r--   0        0        0     2878 2024-04-26 14:50:23.986738 ng_data_pipelines_sdk-0.2.0/ng_data_pipelines_sdk/spark_manager.py
--rw-r--r--   0        0        0     3498 2024-04-26 14:50:23.986738 ng_data_pipelines_sdk-0.2.0/ng_data_pipelines_sdk/utils.py
--rw-r--r--   0        0        0      672 2024-04-26 14:50:23.987738 ng_data_pipelines_sdk-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-04-27 18:29:48.742626 ng_data_pipelines_sdk-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-27 18:29:48.768626 ng_data_pipelines_sdk-0.3.0/ng_data_pipelines_sdk/__init__.py
+-rw-r--r--   0        0        0     9154 2024-04-27 18:29:48.742626 ng_data_pipelines_sdk-0.3.0/ng_data_pipelines_sdk/aws_interface.py
+-rw-r--r--   0        0        0      231 2024-04-27 18:29:48.742626 ng_data_pipelines_sdk-0.3.0/ng_data_pipelines_sdk/custom_logger.py
+-rw-r--r--   0        0        0    26473 2024-04-27 18:29:48.742626 ng_data_pipelines_sdk-0.3.0/ng_data_pipelines_sdk/dataframe_manager.py
+-rw-r--r--   0        0        0    14940 2024-04-27 18:29:48.742626 ng_data_pipelines_sdk-0.3.0/ng_data_pipelines_sdk/interfaces.py
+-rw-r--r--   0        0        0     4816 2024-04-27 18:29:48.742626 ng_data_pipelines_sdk-0.3.0/ng_data_pipelines_sdk/spark_manager.py
+-rw-r--r--   0        0        0     1452 2024-04-27 18:29:48.742626 ng_data_pipelines_sdk-0.3.0/ng_data_pipelines_sdk/utils.py
+-rw-r--r--   0        0        0      672 2024-04-27 18:29:48.744626 ng_data_pipelines_sdk-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.3.0/PKG-INFO
```

### Comparing `ng_data_pipelines_sdk-0.2.0/ng_data_pipelines_sdk/dataframe_manager.py` & `ng_data_pipelines_sdk-0.3.0/ng_data_pipelines_sdk/dataframe_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,14 +149,24 @@
             error_message = (
                 f"Error retrieving or handling schema from {full_s3_file_path}: {e}"
             )
             logger.error(error_message)
             raise ValueError(error_message)
 
     def read_dataframe(self, df_params: InputDataFrameParams) -> DataFrame:
+        """
+        Reads a DataFrame from a specified location.
+
+        Args:
+            df_params (InputDataFrameParams): The parameters for reading the DataFrame.
+
+        Returns:
+            DataFrame: The read DataFrame.
+
+        """
         read_params = df_params.df_params
         bucket_url = self._get_bucket_url(read_params.bucket_params)
         if read_params.specific_path:
             path = f"{bucket_url}/{read_params.specific_path}"
         else:
             path = f"{bucket_url}/{self._get_dataframe_path_with_date_partitions(read_params)}"
 
@@ -285,14 +295,24 @@
             or df_params.df_params.file_type != FileType.PARQUET
         ):
             self.write_schema(df, write_params)
 
         logger.info("Dataframe written successfully.\n")
 
     def write_dataframe(self, df: DataFrame, df_params: OutputDataFrameParams) -> None:
+        """
+        Writes a DataFrame to a specified location with optional date partitions.
+
+        Args:
+            df (DataFrame): The DataFrame to be written.
+            df_params (OutputDataFrameParams): The parameters for writing the DataFrame.
+
+        Returns:
+            None
+        """
         write_params = df_params.df_params
         bucket_url = self._get_bucket_url(write_params.bucket_params)
         write_path_url = f"{bucket_url}/{write_params.path_to_dataframe_root}"
         logger.debug(f"Write root path: {write_path_url}")
 
         partitions = self._get_partitions(write_params)
         logger.debug(f"Using partitions: {partitions}")
```

### Comparing `ng_data_pipelines_sdk-0.2.0/pyproject.toml` & `ng_data_pipelines_sdk-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ng-data-pipelines-sdk"
-version = "0.2.0"
+version = "0.3.0"
 description = "A library for facilitating the development of data engineering pipelines using pyspark. Compatible with MWAA running airflow 2.8.1."
 authors = ["ng.cash"]
 readme = "README.md"
 exclude = [".git/", ".gitignore", "tests/", "docs/", "*.yml", "__pycache__/", "*.pyc", "*.ipynb", "playground/", "poetry.lock", "dist/", "build/"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
```

### Comparing `ng_data_pipelines_sdk-0.2.0/PKG-INFO` & `ng_data_pipelines_sdk-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ng-data-pipelines-sdk
-Version: 0.2.0
+Version: 0.3.0
 Summary: A library for facilitating the development of data engineering pipelines using pyspark. Compatible with MWAA running airflow 2.8.1.
 Author: ng.cash
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

