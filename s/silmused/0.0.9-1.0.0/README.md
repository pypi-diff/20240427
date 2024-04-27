# Comparing `tmp/silmused-0.0.9.tar.gz` & `tmp/silmused-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silmused-0.0.9.tar", last modified: Sun Jan  7 11:56:09 2024, max compression
+gzip compressed data, was "silmused-1.0.0.tar", last modified: Sat Apr 27 11:49:34 2024, max compression
```

## Comparing `silmused-0.0.9.tar` & `silmused-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 11:56:09.624387 silmused-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-01-07 11:55:54.000000 silmused-0.0.9/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-01-07 11:56:09.624387 silmused-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-01-07 11:55:54.000000 silmused-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-07 11:56:09.624387 silmused-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-01-07 11:55:54.000000 silmused-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 11:56:09.620387 silmused-0.0.9/silmused/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/ExecuteLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/Runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/TitleLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 11:56:09.624387 silmused-0.0.9/silmused/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/tests/ConstraintTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/tests/DataTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/tests/FunctionTest.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/tests/IndexTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/tests/ProcedureTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/tests/StructureTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/tests/TestDefinition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/tests/TriggerTest.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/tests/ViewTest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 11:56:09.620387 silmused-0.0.9/silmused.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-01-07 11:56:09.000000 silmused-0.0.9/silmused.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-01-07 11:56:09.000000 silmused-0.0.9/silmused.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-07 11:56:09.000000 silmused-0.0.9/silmused.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-07 11:56:09.000000 silmused-0.0.9/silmused.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-07 11:56:09.000000 silmused-0.0.9/silmused.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 11:49:34.020912 silmused-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-27 11:49:17.000000 silmused-1.0.0/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-27 11:49:34.020912 silmused-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-27 11:49:17.000000 silmused-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 11:49:34.020912 silmused-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-27 11:49:17.000000 silmused-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 11:49:34.012912 silmused-1.0.0/silmused/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/ChecksLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/ExecuteLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10976 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/Runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/TitleLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/Translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 11:49:34.016912 silmused-1.0.0/silmused/locale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/locale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18201 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/locale/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17065 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/locale/et.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 11:49:34.016912 silmused-1.0.0/silmused/test_cases/
+-rw-r--r--   0 runner    (1001) docker     (127)    18420 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/test_cases/demo_test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/test_cases/feedback_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19234 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/test_cases/kodutood_koik.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/test_cases/paring_koik.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52754 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/test_cases/praksid_koik.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12983 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/test_cases/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 11:49:34.020912 silmused-1.0.0/silmused/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14223 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/tests/ConstraintTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10867 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/tests/DataTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/tests/FunctionTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/tests/IndexTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/tests/ProcedureTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/tests/QueryDataTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/tests/QueryStructureTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/tests/StructureTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/tests/TestDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/tests/TriggerTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/tests/ViewTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-27 11:49:17.000000 silmused-1.0.0/silmused/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 11:49:34.016912 silmused-1.0.0/silmused.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-27 11:49:33.000000 silmused-1.0.0/silmused.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-27 11:49:33.000000 silmused-1.0.0/silmused.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 11:49:33.000000 silmused-1.0.0/silmused.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-27 11:49:33.000000 silmused-1.0.0/silmused.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-27 11:49:33.000000 silmused-1.0.0/silmused.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-27 11:49:33.000000 silmused-1.0.0/silmused.egg-info/top_level.txt
```

### Comparing `silmused-0.0.9/LICENCE.txt` & `silmused-1.0.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `silmused-0.0.9/silmused/ExecuteLayer.py` & `silmused-1.0.0/silmused/ExecuteLayer.py`

 * *Files identical despite different names*

### Comparing `silmused-0.0.9/silmused/__init__.py` & `silmused-1.0.0/silmused/__init__.py`

 * *Files identical despite different names*

### Comparing `silmused-0.0.9/silmused/tests/TriggerTest.py` & `silmused-1.0.0/silmused/tests/TriggerTest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,69 @@
 from silmused.tests.TestDefinition import TestDefinition
 
 
 class TriggerTest(TestDefinition):
-    def __init__(self, name, description=None, points=0, arguments=None, action_timing=None):
+    def __init__(self, name, title=None, description=None, points=0, arguments=None, action_timing=None):
         super().__init__(
             name=name,
+            title=title,
             points=points,
             description=description,
             arguments=arguments,
             query=f"SELECT * FROM information_schema.views WHERE table_name = '{name}'",
         )
 
         self.action_timing = action_timing
 
     def execute(self, cursor):
-        # TODO small tests in separate functions
+
+        # Check that trigger name exists
+        test_trigger_exists_result = self.test_trigger_exists(cursor)
+        if test_trigger_exists_result is not None:
+            return test_trigger_exists_result
+
+        # Check trigger event manipulation on arguments and trigger action timing
+        errors = self.test_trigger_manipulation(cursor) if len(self.arguments) > 0 else []
+
+        return super().response(
+            len(errors) == 0,
+            {"test_type": "trigger_test",
+             "test_key": "trigger_definition_positive_feedback",
+             "params": [self.name]},
+            {"test_type": "trigger_test",
+             "test_key": "trigger_definition_negative_feedback",
+             "params": [self.name, {', '.join(errors)}]},  # TODO errorid on hetkel inglise keeles
+        )
+
+    def test_trigger_exists(self, cursor):
         cursor.execute(f"SELECT trigger_name FROM information_schema.triggers WHERE trigger_name = '{self.name}'")
 
         if len(cursor.fetchall()) <= 0:
             return super().response(
                 False,
-                ''
-                f"Trigger {self.name} was not found",
+                {"test_type": "trigger_test",
+                 "test_key": "trigger_exists_positive_feedback",
+                 "params": [self.name]},
+                {"test_type": "trigger_test",
+                 "test_key": "trigger_exists_negative_feedback",
+                 "params": [self.name]},
             )
+        return None
 
+    def test_trigger_manipulation(self, cursor):
         errors = []
+        for manipulation in self.arguments:
+            cursor.execute(
+                f"SELECT trigger_name FROM information_schema.triggers WHERE trigger_name = '{self.name}' "
+                f"AND event_manipulation = '{manipulation}'")
+
+            if len(cursor.fetchall()) <= 0:
+                errors.append(f"manipulation {manipulation} was not found")
+
+        cursor.execute(
+            f"SELECT trigger_name FROM information_schema.triggers WHERE trigger_name = '{self.name}' "
+            f"AND action_timing = '{self.action_timing}'")
 
-        if len(self.arguments) > 0:
-            for manipulation in self.arguments:
-                cursor.execute(
-                    f"SELECT trigger_name FROM information_schema.triggers WHERE trigger_name = '{self.name}' AND event_manipulation = '{manipulation}'")
-                if len(cursor.fetchall()) <= 0:
-                    errors.append(f"manipulation {manipulation} was not found")
-
-        # TODO this is a bit of a copy-paste
-        cursor.execute(f"SELECT trigger_name FROM information_schema.triggers WHERE trigger_name = '{self.name}' AND action_timing = '{self.action_timing}'")
         if len(cursor.fetchall()) <= 0:
             errors.append(f"action timing {self.action_timing} was not found")
 
-        return super().response(
-            len(errors) == 0,
-            f"Correct, trigger {self.name} definition is correct",
-            f"Trigger {self.name} had the following errors: {', '.join(errors)}",
-        )
+        return errors
```

