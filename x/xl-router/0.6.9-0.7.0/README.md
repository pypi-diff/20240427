# Comparing `tmp/xl_router-0.6.9.tar.gz` & `tmp/xl_router-0.7.0.tar.gz`

## Comparing `xl_router-0.6.9.tar` & `xl_router-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 xl_router-0.6.9/src/xl_router/__init__.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 xl_router-0.6.9/src/xl_router/restful.py
--rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 xl_router-0.6.9/src/xl_router/router.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 xl_router-0.6.9/src/xl_router/decorators/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 xl_router-0.6.9/src/xl_router/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_router-0.6.9/src/xl_router/utils/log.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 xl_router-0.6.9/src/xl_router/utils/memory.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 xl_router-0.6.9/src/xl_router/utils/session.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 xl_router-0.6.9/src/xl_router/utils/base/json.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_router-0.6.9/src/xl_router/utils/database/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 xl_router-0.6.9/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 xl_router-0.6.9/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_router-0.6.9/README.md
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 xl_router-0.6.9/pyproject.toml
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 xl_router-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 xl_router-0.7.0/src/xl_router/__init__.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 xl_router-0.7.0/src/xl_router/restful.py
+-rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 xl_router-0.7.0/src/xl_router/router.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 xl_router-0.7.0/src/xl_router/decorators/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 xl_router-0.7.0/src/xl_router/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_router-0.7.0/src/xl_router/utils/log.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 xl_router-0.7.0/src/xl_router/utils/memory.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 xl_router-0.7.0/src/xl_router/utils/session.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 xl_router-0.7.0/src/xl_router/utils/base/json.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_router-0.7.0/src/xl_router/utils/database/__init__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 xl_router-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 xl_router-0.7.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_router-0.7.0/README.md
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 xl_router-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 xl_router-0.7.0/PKG-INFO
```

### Comparing `xl_router-0.6.9/src/xl_router/__init__.py` & `xl_router-0.7.0/src/xl_router/__init__.py`

 * *Files identical despite different names*

### Comparing `xl_router-0.6.9/src/xl_router/restful.py` & `xl_router-0.7.0/src/xl_router/restful.py`

 * *Files identical despite different names*

### Comparing `xl_router-0.6.9/src/xl_router/router.py` & `xl_router-0.7.0/src/xl_router/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 
 def get_resource_classes(resources_file):
     path = os.path.dirname(resources_file)
     resource_classes = []
     for root, dirs, files in os.walk(path):
         for file in files:
-            if file.endswith("resource.py"):
+            if file.endswith("resource.py") or file.startswith("resource"):
                 file_path = os.path.join(root, file)
                 spec = importlib.util.spec_from_file_location('module', file_path)
                 module = importlib.util.module_from_spec(spec)
                 spec.loader.exec_module(module)
                 resource_classes += get_resource_classes_from_module(module)
     return resource_classes
```

### Comparing `xl_router-0.6.9/src/xl_router/utils/memory.py` & `xl_router-0.7.0/src/xl_router/utils/memory.py`

 * *Files identical despite different names*

### Comparing `xl_router-0.6.9/src/xl_router/utils/session.py` & `xl_router-0.7.0/src/xl_router/utils/session.py`

 * *Files identical despite different names*

### Comparing `xl_router-0.6.9/src/xl_router/utils/base/json.py` & `xl_router-0.7.0/src/xl_router/utils/base/json.py`

 * *Files identical despite different names*

### Comparing `xl_router-0.6.9/LICENSE` & `xl_router-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xl_router-0.6.9/pyproject.toml` & `xl_router-0.7.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xl-router"
-version = "0.6.9"
+version = "0.7.0"
 authors = [
   { name="xilong", email="xilonglab@163.com" },
 ]
 description = "xilong router library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `xl_router-0.6.9/PKG-INFO` & `xl_router-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xl-router
-Version: 0.6.9
+Version: 0.7.0
 Summary: xilong router library
 Project-URL: Homepage, https://git.xilonglab.com/xilong/xl-router
 Project-URL: Bug Tracker, https://git.xilonglab.com/xilong/xl-router/issues
 Author-email: xilong <xilonglab@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

