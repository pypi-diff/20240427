# Comparing `tmp/robotframework_rpycremote-0.0.3.tar.gz` & `tmp/robotframework_rpycremote-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_rpycremote-0.0.3.tar", last modified: Wed Apr 24 21:14:26 2024, max compression
+gzip compressed data, was "robotframework_rpycremote-0.0.4.tar", last modified: Sat Apr 27 06:30:40 2024, max compression
```

## Comparing `robotframework_rpycremote-0.0.3.tar` & `robotframework_rpycremote-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:14:26.417055 robotframework_rpycremote-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:14:26.413055 robotframework_rpycremote-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:14:26.417055 robotframework_rpycremote-0.0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:14:26.417055 robotframework_rpycremote-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/.github/workflows/pipeline.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-24 21:14:26.417055 robotframework_rpycremote-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:14:26.417055 robotframework_rpycremote-0.0.3/RPyCRobotRemote/
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/RPyCRobotRemote/RPyCRobotRemoteClient.py
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/RPyCRobotRemote/RPyCRobotRemoteServer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/RPyCRobotRemote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-24 21:14:26.000000 robotframework_rpycremote-0.0.3/RPyCRobotRemote/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:14:26.417055 robotframework_rpycremote-0.0.3/robotframework_rpycremote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-24 21:14:26.000000 robotframework_rpycremote-0.0.3/robotframework_rpycremote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-24 21:14:26.000000 robotframework_rpycremote-0.0.3/robotframework_rpycremote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 21:14:26.000000 robotframework_rpycremote-0.0.3/robotframework_rpycremote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-24 21:14:26.000000 robotframework_rpycremote-0.0.3/robotframework_rpycremote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 21:14:26.000000 robotframework_rpycremote-0.0.3/robotframework_rpycremote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 21:14:26.417055 robotframework_rpycremote-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:14:26.417055 robotframework_rpycremote-0.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/test/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/test/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/test/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/test/test.robot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:30:40.748729 robotframework_rpycremote-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:30:40.744729 robotframework_rpycremote-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:30:40.744729 robotframework_rpycremote-0.0.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:30:40.744729 robotframework_rpycremote-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/.github/workflows/pipeline.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-27 06:30:40.748729 robotframework_rpycremote-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:30:40.744729 robotframework_rpycremote-0.0.4/RPyCRobotRemote/
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/RPyCRobotRemote/RPyCRobotRemoteClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/RPyCRobotRemote/RPyCRobotRemoteServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/RPyCRobotRemote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-27 06:30:40.000000 robotframework_rpycremote-0.0.4/RPyCRobotRemote/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:30:40.748729 robotframework_rpycremote-0.0.4/robotframework_rpycremote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-27 06:30:40.000000 robotframework_rpycremote-0.0.4/robotframework_rpycremote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-27 06:30:40.000000 robotframework_rpycremote-0.0.4/robotframework_rpycremote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 06:30:40.000000 robotframework_rpycremote-0.0.4/robotframework_rpycremote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-27 06:30:40.000000 robotframework_rpycremote-0.0.4/robotframework_rpycremote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-27 06:30:40.000000 robotframework_rpycremote-0.0.4/robotframework_rpycremote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 06:30:40.748729 robotframework_rpycremote-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:30:40.748729 robotframework_rpycremote-0.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/test/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/test/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/test/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/test/test.robot
```

### Comparing `robotframework_rpycremote-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md` & `robotframework_rpycremote-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md` & `robotframework_rpycremote-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.3/.github/workflows/pipeline.yml` & `robotframework_rpycremote-0.0.4/.github/workflows/pipeline.yml`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.3/.github/workflows/publish-to-pypi.yml` & `robotframework_rpycremote-0.0.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.3/LICENSE.txt` & `robotframework_rpycremote-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.3/PKG-INFO` & `robotframework_rpycremote-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-rpycremote
-Version: 0.0.3
+Version: 0.0.4
 Summary: Robot Framework Remote Library based on RPyC
 Author-email: René Lehfeld <54720674+rlehfeld@users.noreply.github.com>
 License: MIT
 Project-URL: Homepage, https://github.com/rlehfeld/robotframework-rpycremote
 Project-URL: Bug Reports, https://github.com/rlehfeld/robotframework-rpycremote/issues
 Project-URL: Source, https://github.com/rlehfeld/robotframework-rpycremote/
 Keywords: robotframework,robot-framework,rpyc
```

### Comparing `robotframework_rpycremote-0.0.3/README.rst` & `robotframework_rpycremote-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.3/RPyCRobotRemote/RPyCRobotRemoteClient.py` & `robotframework_rpycremote-0.0.4/RPyCRobotRemote/RPyCRobotRemoteClient.py`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.3/RPyCRobotRemote/RPyCRobotRemoteServer.py` & `robotframework_rpycremote-0.0.4/RPyCRobotRemote/RPyCRobotRemoteServer.py`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.3/RPyCRobotRemote/__init__.py` & `robotframework_rpycremote-0.0.4/RPyCRobotRemote/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -73,55 +73,59 @@
         space or is a netref. A netref in the local cache could be from a
         chained-connection. To handle type related behavior properly, the
         attribute `__class__` is a descriptor for netrefs.
 
         So, check thy assumptions regarding the given object when creating
         `id_pack`.
         """
-        if hasattr(obj, '____id_pack__'):
-            # netrefs are handled first since __class__ is a descriptor
-            return obj.____id_pack__
+        undef = object()
+        name_pack = getattr(obj, '____id_pack__', undef)
+        if name_pack is not undef:
+            return name_pack
 
-        if (inspect.ismodule(obj) or
-                getattr(obj, '__name__', None) == 'module'):
+        obj_name = getattr(obj, '__name__', None)
+        if (inspect.ismodule(obj) or obj_name == 'module'):
             if isinstance(obj, type):  # module
                 obj_cls = type(obj)
                 name_pack = (
                     f'{obj_cls.__module__}.{obj_cls.__name__}'
                 )
                 return (name_pack, id(type(obj)), id(obj))
 
-            if inspect.ismodule(obj) and obj.__name__ != 'module':
-                if obj.__name__ in sys.modules:
-                    name_pack = obj.__name__
+            if inspect.ismodule(obj) and obj_name != 'module':
+                if obj_name in sys.modules:
+                    name_pack = obj_name
                 else:
+                    obj_cls = getattr(obj, '__class__', type(obj))
                     name_pack = (
-                        f'{type(obj).__module__}.{obj.__name__}'
+                        f'{obj_cls.__module__}.{obj_name}'
                     )
             elif inspect.ismodule(obj):
                 name_pack = (
-                    f'{obj.__module__}.{obj.__name__}'
-                )
-            elif hasattr(obj, '__module__'):
-                name_pack = (
-                    f'{obj.__module__}.{obj.__name__}'
+                    f'{obj.__module__}.{obj_name}'
                 )
             else:
-                obj_cls = type(obj)
-                name_pack = f'{obj.__name__}'
+                obj_module = getattr(obj, '__module__', undef)
+                if obj_module is not undef:
+                    name_pack = (
+                        f'{obj.__module__}.{obj_name}'
+                    )
+                else:
+                    name_pack = obj_name
             return (name_pack, id(type(obj)), id(obj))
 
         if not inspect.isclass(obj):
+            obj_cls = getattr(obj, '__class__', type(obj))
             name_pack = (
-                f'{type(obj).__module__}.{type(obj).__name__}'
+                f'{obj_cls.__module__}.{obj_cls.__name__}'
             )
             return (name_pack, id(type(obj)), id(obj))
 
         name_pack = (
-            f'{obj.__module__}.{obj.__name__}'
+            f'{obj.__module__}.{obj_name}'
         )
         return (name_pack, id(obj), 0)
 
     func.__code__ = get_id_pack.__code__
 
 
 patch_get_id_pack(rpyc.lib.get_id_pack)
```

### Comparing `robotframework_rpycremote-0.0.3/pyproject.toml` & `robotframework_rpycremote-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.3/robotframework_rpycremote.egg-info/PKG-INFO` & `robotframework_rpycremote-0.0.4/robotframework_rpycremote.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-rpycremote
-Version: 0.0.3
+Version: 0.0.4
 Summary: Robot Framework Remote Library based on RPyC
 Author-email: René Lehfeld <54720674+rlehfeld@users.noreply.github.com>
 License: MIT
 Project-URL: Homepage, https://github.com/rlehfeld/robotframework-rpycremote
 Project-URL: Bug Reports, https://github.com/rlehfeld/robotframework-rpycremote/issues
 Project-URL: Source, https://github.com/rlehfeld/robotframework-rpycremote/
 Keywords: robotframework,robot-framework,rpyc
```

### Comparing `robotframework_rpycremote-0.0.3/robotframework_rpycremote.egg-info/SOURCES.txt` & `robotframework_rpycremote-0.0.4/robotframework_rpycremote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.3/test/provider.py` & `robotframework_rpycremote-0.0.4/test/provider.py`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.3/test/server.py` & `robotframework_rpycremote-0.0.4/test/server.py`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.3/test/test.robot` & `robotframework_rpycremote-0.0.4/test/test.robot`

 * *Files identical despite different names*

