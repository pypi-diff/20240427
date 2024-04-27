# Comparing `tmp/xl_router-0.7.5.tar.gz` & `tmp/xl_router-0.7.6.tar.gz`

## Comparing `xl_router-0.7.5.tar` & `xl_router-0.7.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 xl_router-0.7.5/src/xl_router/__init__.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 xl_router-0.7.5/src/xl_router/restful.py
--rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 xl_router-0.7.5/src/xl_router/router.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 xl_router-0.7.5/src/xl_router/decorators/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 xl_router-0.7.5/src/xl_router/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_router-0.7.5/src/xl_router/utils/log.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 xl_router-0.7.5/src/xl_router/utils/memory.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 xl_router-0.7.5/src/xl_router/utils/session.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 xl_router-0.7.5/src/xl_router/utils/base/json.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_router-0.7.5/src/xl_router/utils/database/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 xl_router-0.7.5/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 xl_router-0.7.5/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_router-0.7.5/README.md
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 xl_router-0.7.5/pyproject.toml
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 xl_router-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 xl_router-0.7.6/src/xl_router/__init__.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 xl_router-0.7.6/src/xl_router/restful.py
+-rw-r--r--   0        0        0     9902 2020-02-02 00:00:00.000000 xl_router-0.7.6/src/xl_router/router.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 xl_router-0.7.6/src/xl_router/decorators/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 xl_router-0.7.6/src/xl_router/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_router-0.7.6/src/xl_router/utils/log.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 xl_router-0.7.6/src/xl_router/utils/memory.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 xl_router-0.7.6/src/xl_router/utils/session.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 xl_router-0.7.6/src/xl_router/utils/base/json.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_router-0.7.6/src/xl_router/utils/database/__init__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 xl_router-0.7.6/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 xl_router-0.7.6/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_router-0.7.6/README.md
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 xl_router-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 xl_router-0.7.6/PKG-INFO
```

### Comparing `xl_router-0.7.5/src/xl_router/__init__.py` & `xl_router-0.7.6/src/xl_router/__init__.py`

 * *Files identical despite different names*

### Comparing `xl_router-0.7.5/src/xl_router/restful.py` & `xl_router-0.7.6/src/xl_router/restful.py`

 * *Files identical despite different names*

### Comparing `xl_router-0.7.5/src/xl_router/router.py` & `xl_router-0.7.6/src/xl_router/router.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from flask import Blueprint, request
 from jsonschema.exceptions import ValidationError
 import functools
 import random
 import os
 import importlib
 import inspect
+import re
 
 
 class ParamMixin:
     @staticmethod
     def get_params():
         if request.method in ['GET', 'DELETE']:
             return to_lowcase({**request.args, **request.view_args})
@@ -40,17 +41,18 @@
             resource_classes.append(obj)
     return resource_classes
 
 
 def get_resource_classes(resources_file):
     path = os.path.dirname(resources_file)
     resource_classes = []
+    pattern = re.compile(r'.*resource(?!s).*\.py$')
     for root, dirs, files in os.walk(path):
         for file in files:
-            if file.endswith("resource.py") or file.startswith("resource_") or file=="resource.py":
+            if pattern.match(file):
                 file_path = os.path.join(root, file)
                 spec = importlib.util.spec_from_file_location('module', file_path)
                 module = importlib.util.module_from_spec(spec)
                 spec.loader.exec_module(module)
                 resource_classes += get_resource_classes_from_module(module)
     return resource_classes
 
@@ -126,8 +128,142 @@
         self.add_resources(resource_classes)
 
     def add(self, rule, public=False, **options):
         def decorator(f):
             endpoint = options.pop("endpoint", None)
             self.add_url_rule(rule, endpoint, self.wrap_view_func(
                 f, public=public,), **options)
-        return decorator
+        return decoratorfrom xl_router.exceptions import MessagePrompt
+from xl_router.utils.base.json import to_lowcase, iter_lowcase, iter_camel
+from flask import Blueprint, request
+from jsonschema.exceptions import ValidationError
+import functools
+import random
+import os
+import importlib
+import inspect
+import re
+
+
+class ParamMixin:
+    @staticmethod
+    def get_params():
+        if request.method in ['GET', 'DELETE']:
+            return to_lowcase({**request.args, **request.view_args})
+        elif 'multipart/form-data' in request.content_type:
+            return {
+                **request.files,
+                **to_lowcase(request.form.to_dict())
+            }
+        else:
+            try:
+                params = request.get_json()
+                return iter_lowcase(params)
+            except:
+                return {
+                    'data': request.get_data()
+                }
+
+    @staticmethod
+    def clean_params(params):
+        return {k: v for k, v in params.items() if v not in ('', 'null', None)}
+
+
+def get_resource_classes_from_module(module):
+    resource_classes = []
+    for name, obj in inspect.getmembers(module):
+        if inspect.isclass(obj) and name.endswith("Resource"):
+            resource_classes.append(obj)
+    return resource_classes
+
+
+def get_resource_classes(resources_file):
+    path = os.path.dirname(resources_file)
+    resource_classes = []
+    pattern = re.compile(r'.*resource(?!s).*\.py$')
+    for root, dirs, files in os.walk(path):
+        for file in files:
+            if pattern.match(file):
+                file_path = os.path.join(root, file)
+                spec = importlib.util.spec_from_file_location('module', file_path)
+                module = importlib.util.module_from_spec(spec)
+                spec.loader.exec_module(module)
+                resource_classes += get_resource_classes_from_module(module)
+    return resource_classes
+
+
+class Router(ParamMixin, Blueprint):
+    """路由"""
+
+    def __init__(self, *args, **kwargs):
+        Blueprint.__init__(self, *args, **kwargs)
+
+    def verify_user(self):
+        """用户验证，通过继承覆盖此方法实现具体逻辑"""
+        return True
+
+    def handle_error(self, e):
+        """错误处理，通过继承覆盖此方法实现具体逻辑"""
+        pass
+
+    @staticmethod
+    def decorator(func):
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+            return func(*args, **kwargs)
+        return wrapper
+
+    def wrap_view_func(self, func, public=False):
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+            params = self.clean_params(self.get_params())
+            if not self.verify_user() and not public:
+                return {'code': 401, 'msg': '用户无权限'}
+            try:
+                data = self.decorator(func)(**params)
+            except MessagePrompt as e:
+                return {'code': 500, 'msg': str(e)}
+            except ValidationError as e:
+                return {'code': 400, 'msg': str(e)}
+            except Exception as e:
+                self.handle_error(e)
+                raise e
+            if isinstance(data, dict):
+                data = iter_camel(data)
+            elif isinstance(data, list):
+                data = [iter_camel(item) if isinstance(item, dict) else item
+                        for item in data]
+            elif data is None:
+                pass
+            elif isinstance(data, str):
+                pass 
+            else:
+                return data
+            return {'code': 200, 'msg': '操作成功', 'data': data}
+        return wrapper
+
+    def add_resource(self, rule, resource_class):
+        http_methods = ['get', 'post', 'put', 'delete']
+
+        for method_name in http_methods:
+            if method_name in dir(resource_class):
+                method = getattr(resource_class, method_name)
+                public = getattr(method, 'public', False)
+                method = functools.partial(method)
+                endpoint = str(random.randint(10000000, 99999999))
+                self.add_url_rule(rule, endpoint, self.wrap_view_func(method,
+                                                                      public=public), methods=[method_name.upper()])
+
+    def add_resources(self, resource_classes):
+        for resource_class in resource_classes:
+            self.add_resource(resource_class.path, resource_class)
+
+    def auto_add_resources(self, resources_file):
+        resource_classes = get_resource_classes(resources_file)
+        self.add_resources(resource_classes)
+
+    def add(self, rule, public=False, **options):
+        def decorator(f):
+            endpoint = options.pop("endpoint", None)
+            self.add_url_rule(rule, endpoint, self.wrap_view_func(
+                f, public=public,), **options)
+        return decorator
```

### Comparing `xl_router-0.7.5/src/xl_router/utils/memory.py` & `xl_router-0.7.6/src/xl_router/utils/memory.py`

 * *Files identical despite different names*

### Comparing `xl_router-0.7.5/src/xl_router/utils/session.py` & `xl_router-0.7.6/src/xl_router/utils/session.py`

 * *Files identical despite different names*

### Comparing `xl_router-0.7.5/src/xl_router/utils/base/json.py` & `xl_router-0.7.6/src/xl_router/utils/base/json.py`

 * *Files identical despite different names*

### Comparing `xl_router-0.7.5/LICENSE` & `xl_router-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xl_router-0.7.5/pyproject.toml` & `xl_router-0.7.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xl-router"
-version = "0.7.5"
+version = "0.7.6"
 authors = [
   { name="xilong", email="xilonglab@163.com" },
 ]
 description = "xilong router library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `xl_router-0.7.5/PKG-INFO` & `xl_router-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xl-router
-Version: 0.7.5
+Version: 0.7.6
 Summary: xilong router library
 Project-URL: Homepage, https://git.xilonglab.com/xilong/xl-router
 Project-URL: Bug Tracker, https://git.xilonglab.com/xilong/xl-router/issues
 Author-email: xilong <xilonglab@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

