# Comparing `tmp/computer_vision_design_patterns-0.1.1.tar.gz` & `tmp/computer_vision_design_patterns-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computer_vision_design_patterns-0.1.1.tar", max compression
+gzip compressed data, was "computer_vision_design_patterns-0.1.2.tar", max compression
```

## Comparing `computer_vision_design_patterns-0.1.1.tar` & `computer_vision_design_patterns-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-03-15 19:53:30.502092 computer_vision_design_patterns-0.1.1/computer_vision_design_patterns/__init__.py
--rw-r--r--   0        0        0        0 2024-03-15 19:53:30.503135 computer_vision_design_patterns-0.1.1/computer_vision_design_patterns/alarm.py
--rw-r--r--   0        0        0     1070 2024-03-15 23:43:16.152608 computer_vision_design_patterns-0.1.1/computer_vision_design_patterns/counter.py
--rw-r--r--   0        0        0     1179 2024-03-15 23:43:16.153610 computer_vision_design_patterns-0.1.1/computer_vision_design_patterns/event.py
--rw-r--r--   0        0        0      445 2024-03-15 23:43:16.156608 computer_vision_design_patterns-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       35 2023-12-04 17:12:59.778488 computer_vision_design_patterns-0.1.1/README.md
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 computer_vision_design_patterns-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-15 19:53:30.502092 computer_vision_design_patterns-0.1.2/computer_vision_design_patterns/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-15 19:53:30.503135 computer_vision_design_patterns-0.1.2/computer_vision_design_patterns/alarm.py
+-rw-r--r--   0        0        0     1070 2024-03-15 23:43:16.152608 computer_vision_design_patterns-0.1.2/computer_vision_design_patterns/counter.py
+-rw-r--r--   0        0        0     1353 2024-04-26 23:53:10.802100 computer_vision_design_patterns-0.1.2/computer_vision_design_patterns/event.py
+-rw-r--r--   0        0        0      445 2024-04-26 23:51:17.739966 computer_vision_design_patterns-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       35 2024-04-26 23:53:08.561056 computer_vision_design_patterns-0.1.2/README.md
+-rw-r--r--   0        0        0      603 1970-01-01 00:00:00.000000 computer_vision_design_patterns-0.1.2/PKG-INFO
```

### Comparing `computer_vision_design_patterns-0.1.1/computer_vision_design_patterns/counter.py` & `computer_vision_design_patterns-0.1.2/computer_vision_design_patterns/counter.py`

 * *Files identical despite different names*

### Comparing `computer_vision_design_patterns-0.1.1/computer_vision_design_patterns/event.py` & `computer_vision_design_patterns-0.1.2/computer_vision_design_patterns/event.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,12 +32,21 @@
         self._event_seconds_duration = event_seconds_duration
         self._last_call_time = None
 
     def trigger(self):
         self._last_call_time = time.time()
         self.activate()
 
-    def update_state(self):
+    def _update_timer(self):
         if self._last_call_time is not None:
             if time.time() - self._last_call_time > self._event_seconds_duration:
                 self.deactivate()
                 self._last_call_time = None
+
+    def retrive_state(self):
+        self._update_timer()
+
+        return self.state
+
+    def is_active(self):
+        self._update_timer()
+        return self.is_active()
```

### Comparing `computer_vision_design_patterns-0.1.1/PKG-INFO` & `computer_vision_design_patterns-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: computer-vision-design-patterns
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Federico Lanzani
 Author-email: federico@federicolanzani.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: transitions (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
```

