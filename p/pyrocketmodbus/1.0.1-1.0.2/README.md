# Comparing `tmp/pyrocketmodbus-1.0.1.tar.gz` & `tmp/pyrocketmodbus-1.0.2.tar.gz`

## Comparing `pyrocketmodbus-1.0.1.tar` & `pyrocketmodbus-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pyrocketmodbus-1.0.1/requirements.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 pyrocketmodbus-1.0.1/src/__init__.py
--rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 pyrocketmodbus-1.0.1/src/pyrocketmodbus.py
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 pyrocketmodbus-1.0.1/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pyrocketmodbus-1.0.1/LICENSE
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pyrocketmodbus-1.0.1/README.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pyrocketmodbus-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 pyrocketmodbus-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pyrocketmodbus-1.0.2/requirements.txt
+-rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 pyrocketmodbus-1.0.2/src/pyrocketmodbus/__init__.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 pyrocketmodbus-1.0.2/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pyrocketmodbus-1.0.2/LICENSE
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pyrocketmodbus-1.0.2/README.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pyrocketmodbus-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 pyrocketmodbus-1.0.2/PKG-INFO
```

### Comparing `pyrocketmodbus-1.0.1/src/pyrocketmodbus.py` & `pyrocketmodbus-1.0.2/src/pyrocketmodbus/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+"""
+pyrocketmodbus.
+
+Python package for Modbus communication.
+"""
+
+__author__ = 'Giuliano Errico'
+
 from typing import Any
 import serial
 from subprocess import getstatusoutput as shell_command
 from logging import Logger
 
 
 class RocketModbusException(Exception):
```

### Comparing `pyrocketmodbus-1.0.1/.gitignore` & `pyrocketmodbus-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyrocketmodbus-1.0.1/LICENSE` & `pyrocketmodbus-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrocketmodbus-1.0.1/pyproject.toml` & `pyrocketmodbus-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyrocketmodbus"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Giuliano Errico", email="errgioul2@gmail.com" },
 ]
 description = "Python package for Modbus communication"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `pyrocketmodbus-1.0.1/PKG-INFO` & `pyrocketmodbus-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyrocketmodbus
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python package for Modbus communication
 Project-URL: Homepage, https://github.com/ciuliene/pyrocketmodbus
 Project-URL: Issues, https://github.com/ciuliene/pyrocketmodbus/issues
 Author-email: Giuliano Errico <errgioul2@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

