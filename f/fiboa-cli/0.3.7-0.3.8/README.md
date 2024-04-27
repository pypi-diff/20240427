# Comparing `tmp/fiboa_cli-0.3.7.tar.gz` & `tmp/fiboa_cli-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiboa_cli-0.3.7.tar", last modified: Thu Apr 25 15:45:31 2024, max compression
+gzip compressed data, was "fiboa_cli-0.3.8.tar", last modified: Sat Apr 27 20:21:36 2024, max compression
```

## Comparing `fiboa_cli-0.3.7.tar` & `fiboa_cli-0.3.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:45:31.340370 fiboa_cli-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 15:45:27.000000 fiboa_cli-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-04-25 15:45:31.340370 fiboa_cli-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-04-25 15:45:27.000000 fiboa_cli-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:45:31.340370 fiboa_cli-0.3.7/fiboa_cli/
--rw-r--r--   0 runner    (1001) docker     (127)    12187 2024-04-25 15:45:27.000000 fiboa_cli-0.3.7/fiboa_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-25 15:45:27.000000 fiboa_cli-0.3.7/fiboa_cli/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-25 15:45:27.000000 fiboa_cli-0.3.7/fiboa_cli/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-04-25 15:45:27.000000 fiboa_cli-0.3.7/fiboa_cli/convert_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-25 15:45:27.000000 fiboa_cli-0.3.7/fiboa_cli/create_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-25 15:45:27.000000 fiboa_cli-0.3.7/fiboa_cli/create_geoparquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-25 15:45:27.000000 fiboa_cli-0.3.7/fiboa_cli/describe.py
--rw-r--r--   0 runner    (1001) docker     (127)     9751 2024-04-25 15:45:27.000000 fiboa_cli-0.3.7/fiboa_cli/geopandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-04-25 15:45:27.000000 fiboa_cli-0.3.7/fiboa_cli/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-25 15:45:27.000000 fiboa_cli-0.3.7/fiboa_cli/jsonschema_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-25 15:45:27.000000 fiboa_cli-0.3.7/fiboa_cli/parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-25 15:45:27.000000 fiboa_cli-0.3.7/fiboa_cli/rename_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-25 15:45:27.000000 fiboa_cli-0.3.7/fiboa_cli/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-04-25 15:45:27.000000 fiboa_cli-0.3.7/fiboa_cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-04-25 15:45:27.000000 fiboa_cli-0.3.7/fiboa_cli/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-25 15:45:27.000000 fiboa_cli-0.3.7/fiboa_cli/validate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-25 15:45:27.000000 fiboa_cli-0.3.7/fiboa_cli/validate_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 15:45:27.000000 fiboa_cli-0.3.7/fiboa_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:45:31.340370 fiboa_cli-0.3.7/fiboa_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-04-25 15:45:31.000000 fiboa_cli-0.3.7/fiboa_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-25 15:45:31.000000 fiboa_cli-0.3.7/fiboa_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:45:31.000000 fiboa_cli-0.3.7/fiboa_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-25 15:45:31.000000 fiboa_cli-0.3.7/fiboa_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-25 15:45:31.000000 fiboa_cli-0.3.7/fiboa_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 15:45:31.000000 fiboa_cli-0.3.7/fiboa_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:45:31.340370 fiboa_cli-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-25 15:45:27.000000 fiboa_cli-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:45:31.340370 fiboa_cli-0.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-25 15:45:27.000000 fiboa_cli-0.3.7/tests/test_jsonschema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:21:36.363953 fiboa_cli-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-04-27 20:21:36.363953 fiboa_cli-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:21:36.363953 fiboa_cli-0.3.8/fiboa_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    12187 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/convert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/create_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/create_geoparquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/describe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9751 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/geopandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/jsonschema_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/rename_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/validate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/validate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:21:36.363953 fiboa_cli-0.3.8/fiboa_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-04-27 20:21:36.000000 fiboa_cli-0.3.8/fiboa_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-27 20:21:36.000000 fiboa_cli-0.3.8/fiboa_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 20:21:36.000000 fiboa_cli-0.3.8/fiboa_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-27 20:21:36.000000 fiboa_cli-0.3.8/fiboa_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-27 20:21:36.000000 fiboa_cli-0.3.8/fiboa_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-27 20:21:36.000000 fiboa_cli-0.3.8/fiboa_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 20:21:36.363953 fiboa_cli-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:21:36.363953 fiboa_cli-0.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/tests/test_jsonschema.py
```

### Comparing `fiboa_cli-0.3.7/LICENSE` & `fiboa_cli-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.7/PKG-INFO` & `fiboa_cli-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiboa-cli
-Version: 0.3.7
+Version: 0.3.8
 Summary: CLI tools such as validation and file format conversion for fiboa.
 Home-page: https://github.com/fiboa/cli
 Author: Matthias Mohr
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `fiboa_cli-0.3.7/README.md` & `fiboa_cli-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.7/fiboa_cli/__init__.py` & `fiboa_cli-0.3.8/fiboa_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.7/fiboa_cli/convert.py` & `fiboa_cli-0.3.8/fiboa_cli/convert.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.7/fiboa_cli/convert_utils.py` & `fiboa_cli-0.3.8/fiboa_cli/convert_utils.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.7/fiboa_cli/create_geojson.py` & `fiboa_cli-0.3.8/fiboa_cli/create_geojson.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.7/fiboa_cli/create_geoparquet.py` & `fiboa_cli-0.3.8/fiboa_cli/create_geoparquet.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.7/fiboa_cli/describe.py` & `fiboa_cli-0.3.8/fiboa_cli/describe.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.7/fiboa_cli/geopandas.py` & `fiboa_cli-0.3.8/fiboa_cli/geopandas.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.7/fiboa_cli/jsonschema.py` & `fiboa_cli-0.3.8/fiboa_cli/jsonschema.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.7/fiboa_cli/jsonschema_template.py` & `fiboa_cli-0.3.8/fiboa_cli/jsonschema_template.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.7/fiboa_cli/parquet.py` & `fiboa_cli-0.3.8/fiboa_cli/parquet.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.7/fiboa_cli/rename_extension.py` & `fiboa_cli-0.3.8/fiboa_cli/rename_extension.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.7/fiboa_cli/types.py` & `fiboa_cli-0.3.8/fiboa_cli/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,17 +75,15 @@
             return "str"
         else:
             return "string"
     elif type == "array":
         return lambda series: series.apply(lambda x: np.array(x))
     elif type == "object":
         return "object"
-    elif type == "date":
-        return "datetime64[D]"
-    elif type == "date-time":
+    elif type == "date" or type == "date-time":
         return lambda series: pd.to_datetime(series)
     elif type == "geometry":
         return None, # not a column, don't convert geometry
     elif type == "bounding-box":
         raise Exception("Bounding boxes are not supported yet") # todo
     else:
         return None
@@ -152,14 +150,15 @@
     elif dtype.startswith("int") or dtype.startswith("uint") or dtype.startswith("float"): # float16/32/64
         return getattr(pa, dtype)()
     elif dtype == "object":
         return pa.string() # todo
     elif dtype == "datetime64":
         return pa.timestamp("ms", tz="UTC")
     else:
+        print(dtype)
         return None
 
 
 # checks pyarrow datatypes
 PA_TYPE_CHECK = {
     "boolean": pat.is_boolean,
     "int8": pat.is_int8,
```

### Comparing `fiboa_cli-0.3.7/fiboa_cli/util.py` & `fiboa_cli-0.3.8/fiboa_cli/util.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.7/fiboa_cli/validate.py` & `fiboa_cli-0.3.8/fiboa_cli/validate.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.7/fiboa_cli/validate_data.py` & `fiboa_cli-0.3.8/fiboa_cli/validate_data.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.7/fiboa_cli/validate_schema.py` & `fiboa_cli-0.3.8/fiboa_cli/validate_schema.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.7/fiboa_cli.egg-info/PKG-INFO` & `fiboa_cli-0.3.8/fiboa_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiboa-cli
-Version: 0.3.7
+Version: 0.3.8
 Summary: CLI tools such as validation and file format conversion for fiboa.
 Home-page: https://github.com/fiboa/cli
 Author: Matthias Mohr
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `fiboa_cli-0.3.7/fiboa_cli.egg-info/SOURCES.txt` & `fiboa_cli-0.3.8/fiboa_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.7/setup.py` & `fiboa_cli-0.3.8/setup.py`

 * *Files identical despite different names*

