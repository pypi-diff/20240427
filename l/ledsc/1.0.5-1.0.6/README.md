# Comparing `tmp/ledsc-1.0.5.tar.gz` & `tmp/ledsc-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ledsc-1.0.5.tar", last modified: Wed Apr 10 22:42:34 2024, max compression
+gzip compressed data, was "ledsc-1.0.6.tar", last modified: Sat Apr 27 13:44:29 2024, max compression
```

## Comparing `ledsc-1.0.5.tar` & `ledsc-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-04-10 22:42:34.755633 ledsc-1.0.5/
--rw-r--r--   0 hell      (1000) hell      (1000)      985 2024-04-10 22:42:34.755633 ledsc-1.0.5/PKG-INFO
--rw-r--r--   0 hell      (1000) hell      (1000)      558 2024-03-14 21:51:08.000000 ledsc-1.0.5/README.md
-drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-04-10 22:42:34.755633 ledsc-1.0.5/ledsc/
--rw-r--r--   0 hell      (1000) hell      (1000)       43 2024-04-10 22:42:30.000000 ledsc-1.0.5/ledsc/__init__.py
--rw-r--r--   0 hell      (1000) hell      (1000)     7788 2024-04-10 22:41:30.000000 ledsc-1.0.5/ledsc/ledsc.py
-drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-04-10 22:42:34.755633 ledsc-1.0.5/ledsc.egg-info/
--rw-r--r--   0 hell      (1000) hell      (1000)      985 2024-04-10 22:42:34.000000 ledsc-1.0.5/ledsc.egg-info/PKG-INFO
--rw-rw-r--   0 hell      (1000) hell      (1000)      201 2024-04-10 22:42:34.000000 ledsc-1.0.5/ledsc.egg-info/SOURCES.txt
--rw-rw-r--   0 hell      (1000) hell      (1000)        1 2024-04-10 22:42:34.000000 ledsc-1.0.5/ledsc.egg-info/dependency_links.txt
--rw-rw-r--   0 hell      (1000) hell      (1000)       30 2024-04-10 22:42:34.000000 ledsc-1.0.5/ledsc.egg-info/requires.txt
--rw-rw-r--   0 hell      (1000) hell      (1000)        6 2024-04-10 22:42:34.000000 ledsc-1.0.5/ledsc.egg-info/top_level.txt
--rw-r--r--   0 hell      (1000) hell      (1000)      437 2024-04-10 22:42:30.000000 ledsc-1.0.5/pyproject.toml
--rw-rw-r--   0 hell      (1000) hell      (1000)       38 2024-04-10 22:42:34.755633 ledsc-1.0.5/setup.cfg
+drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-04-27 13:44:29.588724 ledsc-1.0.6/
+-rw-r--r--   0 hell      (1000) hell      (1000)      985 2024-04-27 13:44:29.588724 ledsc-1.0.6/PKG-INFO
+-rw-r--r--   0 hell      (1000) hell      (1000)      558 2024-03-14 21:51:08.000000 ledsc-1.0.6/README.md
+drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-04-27 13:44:29.588724 ledsc-1.0.6/ledsc/
+-rw-r--r--   0 hell      (1000) hell      (1000)       43 2024-04-10 22:46:46.000000 ledsc-1.0.6/ledsc/__init__.py
+-rw-r--r--   0 hell      (1000) hell      (1000)     7773 2024-04-10 22:46:46.000000 ledsc-1.0.6/ledsc/ledsc.py
+drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-04-27 13:44:29.588724 ledsc-1.0.6/ledsc.egg-info/
+-rw-r--r--   0 hell      (1000) hell      (1000)      985 2024-04-27 13:44:29.000000 ledsc-1.0.6/ledsc.egg-info/PKG-INFO
+-rw-rw-r--   0 hell      (1000) hell      (1000)      201 2024-04-27 13:44:29.000000 ledsc-1.0.6/ledsc.egg-info/SOURCES.txt
+-rw-rw-r--   0 hell      (1000) hell      (1000)        1 2024-04-27 13:44:29.000000 ledsc-1.0.6/ledsc.egg-info/dependency_links.txt
+-rw-rw-r--   0 hell      (1000) hell      (1000)       30 2024-04-27 13:44:29.000000 ledsc-1.0.6/ledsc.egg-info/requires.txt
+-rw-rw-r--   0 hell      (1000) hell      (1000)        6 2024-04-27 13:44:29.000000 ledsc-1.0.6/ledsc.egg-info/top_level.txt
+-rw-r--r--   0 hell      (1000) hell      (1000)      437 2024-04-10 22:46:46.000000 ledsc-1.0.6/pyproject.toml
+-rw-rw-r--   0 hell      (1000) hell      (1000)       38 2024-04-27 13:44:29.588724 ledsc-1.0.6/setup.cfg
```

### Comparing `ledsc-1.0.5/PKG-INFO` & `ledsc-1.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledsc
-Version: 1.0.5
+Version: 1.0.6
 Summary: Library for communicate with led string controller
 Author-email: Patrik Kratochvil <info@ledsc.eu>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ledsc-1.0.5/README.md` & `ledsc-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ledsc-1.0.5/ledsc/ledsc.py` & `ledsc-1.0.6/ledsc/ledsc.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,23 +59,23 @@
             raise ValueError(f"Reading values is not available in BROADCAST mode!")
 
         resp = self.client.read_holding_registers(address=address, slave=self.slave_id, count=count)
         self.__response_check(resp)
         resp = resp.registers[0] if len(resp.registers) == 1 else resp.registers
         return resp
 
-    def __write(self, func: Callable[[], ModbusResponse]):
+    def __write(self, func):
         def wrapper(*args, **kwargs):
             is_broadcast = self.slave_id == 0
             if is_broadcast:
                 timeout = self.client.comm_params.timeout_connect
                 self.client.close()
                 self.client.comm_params.timeout_connect = 0.000001
 
-            resp = func()
+            resp = func(*args, **kwargs)
 
             if is_broadcast:
                 self.client.comm_params.timeout_connect = timeout  # noqa
             self.__response_check(resp)
         return wrapper
 
     def write_register(self, address: int, value: int) -> ModbusResponse:
```

### Comparing `ledsc-1.0.5/ledsc.egg-info/PKG-INFO` & `ledsc-1.0.6/ledsc.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledsc
-Version: 1.0.5
+Version: 1.0.6
 Summary: Library for communicate with led string controller
 Author-email: Patrik Kratochvil <info@ledsc.eu>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

