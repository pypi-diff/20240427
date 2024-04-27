# Comparing `tmp/ng_data_pipelines_sdk-0.3.0.tar.gz` & `tmp/ng_data_pipelines_sdk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng_data_pipelines_sdk-0.3.0.tar", max compression
+gzip compressed data, was "ng_data_pipelines_sdk-0.4.0.tar", max compression
```

## Comparing `ng_data_pipelines_sdk-0.3.0.tar` & `ng_data_pipelines_sdk-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      106 2024-04-27 18:29:48.742626 ng_data_pipelines_sdk-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-04-27 18:29:48.768626 ng_data_pipelines_sdk-0.3.0/ng_data_pipelines_sdk/__init__.py
--rw-r--r--   0        0        0     9154 2024-04-27 18:29:48.742626 ng_data_pipelines_sdk-0.3.0/ng_data_pipelines_sdk/aws_interface.py
--rw-r--r--   0        0        0      231 2024-04-27 18:29:48.742626 ng_data_pipelines_sdk-0.3.0/ng_data_pipelines_sdk/custom_logger.py
--rw-r--r--   0        0        0    26473 2024-04-27 18:29:48.742626 ng_data_pipelines_sdk-0.3.0/ng_data_pipelines_sdk/dataframe_manager.py
--rw-r--r--   0        0        0    14940 2024-04-27 18:29:48.742626 ng_data_pipelines_sdk-0.3.0/ng_data_pipelines_sdk/interfaces.py
--rw-r--r--   0        0        0     4816 2024-04-27 18:29:48.742626 ng_data_pipelines_sdk-0.3.0/ng_data_pipelines_sdk/spark_manager.py
--rw-r--r--   0        0        0     1452 2024-04-27 18:29:48.742626 ng_data_pipelines_sdk-0.3.0/ng_data_pipelines_sdk/utils.py
--rw-r--r--   0        0        0      672 2024-04-27 18:29:48.744626 ng_data_pipelines_sdk-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-04-27 18:37:30.531740 ng_data_pipelines_sdk-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-27 18:37:30.555740 ng_data_pipelines_sdk-0.4.0/ng_data_pipelines_sdk/__init__.py
+-rw-r--r--   0        0        0     9154 2024-04-27 18:37:30.531740 ng_data_pipelines_sdk-0.4.0/ng_data_pipelines_sdk/aws_interface.py
+-rw-r--r--   0        0        0      231 2024-04-27 18:37:30.532740 ng_data_pipelines_sdk-0.4.0/ng_data_pipelines_sdk/custom_logger.py
+-rw-r--r--   0        0        0    26500 2024-04-27 18:37:30.532740 ng_data_pipelines_sdk-0.4.0/ng_data_pipelines_sdk/dataframe_manager.py
+-rw-r--r--   0        0        0    15191 2024-04-27 18:37:30.532740 ng_data_pipelines_sdk-0.4.0/ng_data_pipelines_sdk/interfaces.py
+-rw-r--r--   0        0        0     4816 2024-04-27 18:37:30.532740 ng_data_pipelines_sdk-0.4.0/ng_data_pipelines_sdk/spark_manager.py
+-rw-r--r--   0        0        0     1452 2024-04-27 18:37:30.532740 ng_data_pipelines_sdk-0.4.0/ng_data_pipelines_sdk/utils.py
+-rw-r--r--   0        0        0      672 2024-04-27 18:37:30.533740 ng_data_pipelines_sdk-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.4.0/PKG-INFO
```

### Comparing `ng_data_pipelines_sdk-0.3.0/ng_data_pipelines_sdk/aws_interface.py` & `ng_data_pipelines_sdk-0.4.0/ng_data_pipelines_sdk/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.3.0/ng_data_pipelines_sdk/dataframe_manager.py` & `ng_data_pipelines_sdk-0.4.0/ng_data_pipelines_sdk/dataframe_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -398,21 +398,21 @@
             dfs[df_name] = self.read_dataframe(df_params=input_df_params)
             logger.info(f"Dataframe '{df_name}' read successfully.\n")
 
         return dfs
 
     def _select_transformation_function(self, transform_params: TransformParams):
         """Select the transformation function based on direct or indirect reference."""
-        if transform_params.fn_direct:
-            return transform_params.fn_direct
+        if transform_params.transform_function:
+            return transform_params.transform_function
         elif transform_params.fn_indirect:
             raise NotImplementedError("Indirect function references are not supported.")
         else:
             raise ValueError(
-                "TransformParams must have either 'fn_direct' or 'fn_indirect' set."
+                "TransformParams must have either 'transform_function' or 'fn_indirect' set."
             )
 
     def apply_transform_to_df(
         self, df: DataFrame, transform_params: TransformParams
     ) -> DataFrame:
         """Apply transformation to a single DataFrame."""
         transform_fn = self._select_transformation_function(transform_params)
```

### Comparing `ng_data_pipelines_sdk-0.3.0/ng_data_pipelines_sdk/interfaces.py` & `ng_data_pipelines_sdk-0.4.0/ng_data_pipelines_sdk/interfaces.py`

 * *Files 10% similar despite different names*

```diff
@@ -348,51 +348,51 @@
 
 class TransformParams(BaseModelJsonDumps):
     """
     Represents the parameters for a data transformation.
 
     Attributes:
         transform_label (str): The label for the transformation.
-        fn_direct (Callable): The direct transformation function.
+        transform_function (Callable): The transformation function. Must have a (pyspark) DataFrame type hint as first parameter and return type hint, or a dict of [str, DataFrame] as first parameter hint and return type hint.
         fn_kwargs (Optional[dict]): Additional keyword arguments for the transformation function.
         apply_only_on (Optional[List[str]]): A list of target dataframes to apply the transformation on.
     """
     transform_label: str
-    fn_direct: Callable
-    fn_indirect: Optional[FnIndirect] = None
+    transform_function: Callable
     fn_kwargs: Optional[dict] = None
     apply_only_on: Optional[List[str]] = None
+    fn_indirect: Optional[FnIndirect] = None
     fn_kind: Optional[FnKind] = None
 
     @model_validator(mode="before")
-    def validate_fn_direct_indirect_and_apply_only_on(cls, data):
+    def validate_transform_function_indirect_and_apply_only_on(cls, data):
         fn_indirect = data.get("fn_indirect")
-        fn_direct = data.get("fn_direct")
+        transform_function = data.get("transform_function")
         apply_only_on = data.get("apply_only_on")
 
         def get_annotation_kind(annotation):
             origin = get_origin(annotation)
             args = get_args(annotation)
 
             if origin is dict and args[0] is str and issubclass(args[1], DataFrame):
                 return FnKind.BATCH
             elif issubclass(annotation, DataFrame):
                 return FnKind.SINGLE
             return None
 
-        if fn_indirect is not None and fn_direct is not None:
-            raise ValueError("'fn_indirect' and 'fn_direct' cannot be passed together")
+        if fn_indirect is not None and transform_function is not None:
+            raise ValueError("'fn_indirect' and 'transform_function' cannot be passed together")
 
-        if fn_indirect is None and fn_direct is None:
-            raise ValueError("Either 'fn_indirect' or 'fn_direct' should be passed")
+        if fn_indirect is None and transform_function is None:
+            raise ValueError("Either 'fn_indirect' or 'transform_function' should be passed")
 
         if fn_indirect:
             raise NotImplementedError("fn_indirect is not implemented yet")
 
-        signature = inspect.signature(fn_direct)
+        signature = inspect.signature(transform_function)
         parameters = signature.parameters
         first_param_annotation = (
             list(parameters.values())[0].annotation if parameters else None
         )
         return_annotation = signature.return_annotation
 
         first_param_kind = get_annotation_kind(first_param_annotation)
@@ -401,15 +401,15 @@
         if (first_param_kind is None or return_kind is None) or (first_param_kind != return_kind):
             raise ValueError(
                 "Function must have a DataFrame type hint as first parameter and return type hint, or a dict of [str, DataFrame] as first parameter hint and return type hint"
             )
 
         if first_param_kind != FnKind.SINGLE and apply_only_on is not None:
             raise ValueError(
-                "'apply_only_on' should be passed only when 'fn_direct' has a DataFrame as first parameter, not a list of DataFrames"
+                "'apply_only_on' should be passed only when 'transform_function' has a DataFrame as first parameter, not a list of DataFrames"
             )
 
         # If the function has a DataFrame as first parameter, then it is a single function. If it has a dict of [str, DataFrame] as first parameter, then it is a batch function
         # TODO: This should be a private attribute
         data["fn_kind"] = first_param_kind
 
         return data
```

### Comparing `ng_data_pipelines_sdk-0.3.0/ng_data_pipelines_sdk/spark_manager.py` & `ng_data_pipelines_sdk-0.4.0/ng_data_pipelines_sdk/spark_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.3.0/ng_data_pipelines_sdk/utils.py` & `ng_data_pipelines_sdk-0.4.0/ng_data_pipelines_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.3.0/pyproject.toml` & `ng_data_pipelines_sdk-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ng-data-pipelines-sdk"
-version = "0.3.0"
+version = "0.4.0"
 description = "A library for facilitating the development of data engineering pipelines using pyspark. Compatible with MWAA running airflow 2.8.1."
 authors = ["ng.cash"]
 readme = "README.md"
 exclude = [".git/", ".gitignore", "tests/", "docs/", "*.yml", "__pycache__/", "*.pyc", "*.ipynb", "playground/", "poetry.lock", "dist/", "build/"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
```

### Comparing `ng_data_pipelines_sdk-0.3.0/PKG-INFO` & `ng_data_pipelines_sdk-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ng-data-pipelines-sdk
-Version: 0.3.0
+Version: 0.4.0
 Summary: A library for facilitating the development of data engineering pipelines using pyspark. Compatible with MWAA running airflow 2.8.1.
 Author: ng.cash
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

