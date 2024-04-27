# Comparing `tmp/bluepy3-2.4.2.tar.gz` & `tmp/bluepy3-2.6.1.tar.gz`

## Comparing `bluepy3-2.4.2.tar` & `bluepy3-2.6.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 bluepy3-2.4.2/bluepy3/Makefile
--rwxr-xr-x   0        0        0      226 2020-02-02 00:00:00.000000 bluepy3-2.4.2/bluepy3/__init__.py
--rwxr-xr-x   0        0        0     5144 2020-02-02 00:00:00.000000 bluepy3-2.4.2/bluepy3/blescan.py
--rw-r--r--   0        0        0    58458 2020-02-02 00:00:00.000000 bluepy3-2.4.2/bluepy3/bluepy3-helper.c
--rwxr-xr-x   0        0        0    40792 2020-02-02 00:00:00.000000 bluepy3-2.4.2/bluepy3/btle.py
--rwxr-xr-x   0        0        0    10019 2020-02-02 00:00:00.000000 bluepy3-2.4.2/bluepy3/get_services.py
--rw-r--r--   0        0        0     7453 2020-02-02 00:00:00.000000 bluepy3-2.4.2/bluepy3/helpermaker.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 bluepy3-2.4.2/bluepy3/py.typed
--rw-r--r--   0        0        0    37880 2020-02-02 00:00:00.000000 bluepy3-2.4.2/bluepy3/uuids.json
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 bluepy3-2.4.2/bluepy3/version.h
--rw-r--r--   0        0        0     4210 2020-02-02 00:00:00.000000 bluepy3-2.4.2/bluepy3/config/config.5.47.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.4.2/bluepy3/config/config.5.50.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.4.2/bluepy3/config/config.5.60.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.4.2/bluepy3/config/config.5.66.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.4.2/bluepy3/config/config.5.68.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.4.2/bluepy3/config/config.5.70.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.4.2/bluepy3/config/config.5.71.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.4.2/bluepy3/config/config.5.72.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.4.2/bluepy3/config/config.5.73.h
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 bluepy3-2.4.2/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 bluepy3-2.4.2/LICENSE
--rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 bluepy3-2.4.2/README.md
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 bluepy3-2.4.2/pyproject.toml
--rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 bluepy3-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/Makefile
+-rwxr-xr-x   0        0        0      226 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/__init__.py
+-rwxr-xr-x   0        0        0     5144 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/blescan.py
+-rw-r--r--   0        0        0    58458 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/bluepy3-helper.c
+-rwxr-xr-x   0        0        0    40792 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/btle.py
+-rwxr-xr-x   0        0        0    10019 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/get_services.py
+-rw-r--r--   0        0        0     7453 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/helpermaker.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/py.typed
+-rw-r--r--   0        0        0    37880 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/uuids.json
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/version.h
+-rw-r--r--   0        0        0     4210 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/config/config.5.47.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/config/config.5.50.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/config/config.5.60.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/config/config.5.66.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/config/config.5.68.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/config/config.5.70.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/config/config.5.71.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/config/config.5.72.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/config/config.5.73.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/config/config.5.75.h
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 bluepy3-2.6.1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 bluepy3-2.6.1/LICENSE
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 bluepy3-2.6.1/README.md
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 bluepy3-2.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 bluepy3-2.6.1/PKG-INFO
```

### Comparing `bluepy3-2.4.2/bluepy3/Makefile` & `bluepy3-2.6.1/bluepy3/Makefile`

 * *Files identical despite different names*

### Comparing `bluepy3-2.4.2/bluepy3/blescan.py` & `bluepy3-2.6.1/bluepy3/blescan.py`

 * *Files identical despite different names*

### Comparing `bluepy3-2.4.2/bluepy3/bluepy3-helper.c` & `bluepy3-2.6.1/bluepy3/bluepy3-helper.c`

 * *Files identical despite different names*

### Comparing `bluepy3-2.4.2/bluepy3/btle.py` & `bluepy3-2.6.1/bluepy3/btle.py`

 * *Files identical despite different names*

### Comparing `bluepy3-2.4.2/bluepy3/get_services.py` & `bluepy3-2.6.1/bluepy3/get_services.py`

 * *Files identical despite different names*

### Comparing `bluepy3-2.4.2/bluepy3/helpermaker.py` & `bluepy3-2.6.1/bluepy3/helpermaker.py`

 * *Files identical despite different names*

### Comparing `bluepy3-2.4.2/bluepy3/uuids.json` & `bluepy3-2.6.1/bluepy3/uuids.json`

 * *Files identical despite different names*

### Comparing `bluepy3-2.4.2/bluepy3/config/config.5.47.h` & `bluepy3-2.6.1/bluepy3/config/config.5.47.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.4.2/bluepy3/config/config.5.50.h` & `bluepy3-2.6.1/bluepy3/config/config.5.50.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.4.2/bluepy3/config/config.5.60.h` & `bluepy3-2.6.1/bluepy3/config/config.5.60.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.4.2/bluepy3/config/config.5.66.h` & `bluepy3-2.6.1/bluepy3/config/config.5.66.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.4.2/bluepy3/config/config.5.68.h` & `bluepy3-2.6.1/bluepy3/config/config.5.68.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.4.2/bluepy3/config/config.5.70.h` & `bluepy3-2.6.1/bluepy3/config/config.5.70.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.4.2/bluepy3/config/config.5.71.h` & `bluepy3-2.6.1/bluepy3/config/config.5.71.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.4.2/bluepy3/config/config.5.72.h` & `bluepy3-2.6.1/bluepy3/config/config.5.72.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.4.2/bluepy3/config/config.5.73.h` & `bluepy3-2.6.1/bluepy3/config/config.5.73.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.4.2/.gitignore` & `bluepy3-2.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bluepy3-2.4.2/LICENSE` & `bluepy3-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bluepy3-2.4.2/README.md` & `bluepy3-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `bluepy3-2.4.2/pyproject.toml` & `bluepy3-2.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bluepy3"
-version = "2.4.2"  # latest/current distribution version
-# version = "2.3.4"  # latest test version
+version = "2.6.1"  # latest/current distribution version
+# version = "2.5.1"  # latest test version
 description = "A Python3 module for interfacing with Bluetooth LE devices on Linux."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 # license-files = { paths = ["LICENSE"] }
 authors = [
     { name="Mausy5043" },
```

### Comparing `bluepy3-2.4.2/PKG-INFO` & `bluepy3-2.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bluepy3
-Version: 2.4.2
+Version: 2.6.1
 Summary: A Python3 module for interfacing with Bluetooth LE devices on Linux.
 Project-URL: Homepage, https://github.com/Mausy5043/bluepy3
 Project-URL: Bug Tracker, https://github.com/Mausy5043/bluepy3/issues
 Author: Mausy5043
 License-Expression: MIT
 License-File: LICENSE
 Keywords: BLE,Bluetooth,Bluetooth Low Energy,Bluetooth Smart,Raspberry Pi
```

