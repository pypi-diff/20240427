# Comparing `tmp/xl_router-0.7.1.tar.gz` & `tmp/xl_router-0.7.3.tar.gz`

## Comparing `xl_router-0.7.1.tar` & `xl_router-0.7.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 xl_router-0.7.1/src/xl_router/__init__.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 xl_router-0.7.1/src/xl_router/restful.py
--rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 xl_router-0.7.1/src/xl_router/router.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 xl_router-0.7.1/src/xl_router/decorators/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 xl_router-0.7.1/src/xl_router/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_router-0.7.1/src/xl_router/utils/log.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 xl_router-0.7.1/src/xl_router/utils/memory.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 xl_router-0.7.1/src/xl_router/utils/session.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 xl_router-0.7.1/src/xl_router/utils/base/json.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_router-0.7.1/src/xl_router/utils/database/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 xl_router-0.7.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 xl_router-0.7.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_router-0.7.1/README.md
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 xl_router-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 xl_router-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 xl_router-0.7.3/src/xl_router/__init__.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 xl_router-0.7.3/src/xl_router/restful.py
+-rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 xl_router-0.7.3/src/xl_router/router.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 xl_router-0.7.3/src/xl_router/decorators/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 xl_router-0.7.3/src/xl_router/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_router-0.7.3/src/xl_router/utils/log.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 xl_router-0.7.3/src/xl_router/utils/memory.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 xl_router-0.7.3/src/xl_router/utils/session.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 xl_router-0.7.3/src/xl_router/utils/base/json.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_router-0.7.3/src/xl_router/utils/database/__init__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 xl_router-0.7.3/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 xl_router-0.7.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_router-0.7.3/README.md
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 xl_router-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 xl_router-0.7.3/PKG-INFO
```

### Comparing `xl_router-0.7.1/src/xl_router/__init__.py` & `xl_router-0.7.3/src/xl_router/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             self.config.from_pyfile(config)
 
     def register_extensions(self):
         pass
 
     def register_resources(self):
         for module_name in self.resources:
-            module = import_module('app.{}'.format(module_name))
+            module = import_module('app.{}.resources'.format(module_name))
             self.register_blueprint(module.router)
 
 
 def get_user_agent():
     return request.user_agent.string.lower()
```

### Comparing `xl_router-0.7.1/src/xl_router/restful.py` & `xl_router-0.7.3/src/xl_router/restful.py`

 * *Files identical despite different names*

### Comparing `xl_router-0.7.1/src/xl_router/router.py` & `xl_router-0.7.3/src/xl_router/router.py`

 * *Files identical despite different names*

### Comparing `xl_router-0.7.1/src/xl_router/utils/memory.py` & `xl_router-0.7.3/src/xl_router/utils/memory.py`

 * *Files identical despite different names*

### Comparing `xl_router-0.7.1/src/xl_router/utils/session.py` & `xl_router-0.7.3/src/xl_router/utils/session.py`

 * *Files identical despite different names*

### Comparing `xl_router-0.7.1/src/xl_router/utils/base/json.py` & `xl_router-0.7.3/src/xl_router/utils/base/json.py`

 * *Files identical despite different names*

### Comparing `xl_router-0.7.1/LICENSE` & `xl_router-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xl_router-0.7.1/pyproject.toml` & `xl_router-0.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xl-router"
-version = "0.7.1"
+version = "0.7.3"
 authors = [
   { name="xilong", email="xilonglab@163.com" },
 ]
 description = "xilong router library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `xl_router-0.7.1/PKG-INFO` & `xl_router-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xl-router
-Version: 0.7.1
+Version: 0.7.3
 Summary: xilong router library
 Project-URL: Homepage, https://git.xilonglab.com/xilong/xl-router
 Project-URL: Bug Tracker, https://git.xilonglab.com/xilong/xl-router/issues
 Author-email: xilong <xilonglab@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

