# Comparing `tmp/hurray-1.0.0.tar.gz` & `tmp/hurray-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hurray-1.0.0.tar", last modified: Thu Aug 31 09:09:34 2023, max compression
+gzip compressed data, was "hurray-1.1.0.tar", last modified: Sat Apr 27 11:02:29 2024, max compression
```

## Comparing `hurray-1.0.0.tar` & `hurray-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 09:09:34.973180 hurray-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (999)     1064 2023-08-31 09:09:23.000000 hurray-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     3289 2023-08-31 09:09:34.969180 hurray-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1158 2023-08-31 09:09:23.000000 hurray-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 09:09:34.969180 hurray-1.0.0/hurray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     3289 2023-08-31 09:09:34.000000 hurray-1.0.0/hurray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      162 2023-08-31 09:09:34.000000 hurray-1.0.0/hurray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-31 09:09:34.000000 hurray-1.0.0/hurray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)        7 2023-08-31 09:09:34.000000 hurray-1.0.0/hurray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)     2639 2023-08-31 09:09:23.000000 hurray-1.0.0/hurray.py
--rw-r--r--   0 runner    (1001) docker     (999)     1137 2023-08-31 09:09:23.000000 hurray-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-31 09:09:34.973180 hurray-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 11:02:29.448619 hurray-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-27 11:02:23.000000 hurray-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-27 11:02:29.448619 hurray-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-27 11:02:23.000000 hurray-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 11:02:29.448619 hurray-1.1.0/hurray/
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-27 11:02:23.000000 hurray-1.1.0/hurray/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 11:02:29.448619 hurray-1.1.0/hurray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-27 11:02:29.000000 hurray-1.1.0/hurray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-27 11:02:29.000000 hurray-1.1.0/hurray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 11:02:29.000000 hurray-1.1.0/hurray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-27 11:02:29.000000 hurray-1.1.0/hurray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-27 11:02:23.000000 hurray-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 11:02:29.448619 hurray-1.1.0/setup.cfg
```

### Comparing `hurray-1.0.0/LICENSE` & `hurray-1.1.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 SyberiaK
+Copyright (c) 2024 SyberiaK
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `hurray-1.0.0/PKG-INFO` & `hurray-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: hurray
-Version: 1.0.0
+Version: 1.1.0
 Summary: Simple collection of wrappers around Python's builtin 'array' module
 Author: SyberiaK, trag1c, CircuitSacul, Micael Jarniac, bswck
 License: MIT License
         
-        Copyright (c) 2023 SyberiaK
+        Copyright (c) 2024 SyberiaK
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -31,14 +31,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hurray
```

### Comparing `hurray-1.0.0/README.md` & `hurray-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `hurray-1.0.0/hurray.egg-info/PKG-INFO` & `hurray-1.1.0/hurray.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: hurray
-Version: 1.0.0
+Version: 1.1.0
 Summary: Simple collection of wrappers around Python's builtin 'array' module
 Author: SyberiaK, trag1c, CircuitSacul, Micael Jarniac, bswck
 License: MIT License
         
-        Copyright (c) 2023 SyberiaK
+        Copyright (c) 2024 SyberiaK
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -31,14 +31,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hurray
```

### Comparing `hurray-1.0.0/hurray.py` & `hurray-1.1.0/hurray/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from array import array as _array, typecodes
 from typing import Generic, Iterable, TypeVar
+import sys
 
-__version__ = '1.0.0'
+__version__ = '1.1.0'
 __all__ = ('SByteArray', 'ByteArray',
            'CharArray', 'UCharArray',  # aliases for byte arrays
            'UnicodeArray',
            'ShortArray', 'UShortArray',
            'IntArray', 'UIntArray',
            'LongArray', 'ULongArray',
            'LongLongArray', 'ULongLongArray',
@@ -27,35 +28,39 @@
         return _array(self.typecode, initializer)
 
 
 SByteArray = ArrayType('b', int)
 """Stores signed chars (signed bytes). [-128; 127]"""
 ByteArray = ArrayType('B', int)
 """Stores unsigned chars (unsigned bytes). [0; 255]"""
-UnicodeArray = ArrayType('u', str)
-"""Stores Unicode strings."""
+if sys.version_info >= (3, 13):
+    UnicodeArray = ArrayType('w', str)
+    """Stores Unicode strings."""
+else:
+    UnicodeArray = ArrayType('u', str)
+    """Stores Unicode strings."""
 ShortArray = ArrayType('h', int)
 """Stores signed 16-bit integers. [-32768; 32767]"""
 UShortArray = ArrayType('H', int)
 """Stores unsigned 16-bit integers. [0; 65535]"""
 IntArray = ArrayType('i', int)
 """
 Stores *at least* signed 16-bit integers. [-32768; 32767]
 
 Note:
-    Python documentation states that ``array('i')`` elements *minimal* size is **2 bytes**.
+    Python documentation states that ``array('i')`` elements *minimal* size is **2 bytes** (**16 bits**).
 
     However, in most cases you deal with **32-bit** integers. [-2147483648; 2147483647]
 """
 UIntArray = ArrayType('I', int)
 """
     Stores at least unsigned 16-bit integers. [0; 65535]
 
 Note:
-    Python documentation states that ``array('I')`` elements *minimal* size is **2 bytes**.
+    Python documentation states that ``array('I')`` elements *minimal* size is **2 bytes** (**16 bits**).
 
     However, in most cases you deal with **32-bit** integers. [0; 4294967295]
 """
 LongArray = ArrayType('l', int)
 """Stores signed 32-bit integers. [-2147483648; 2147483647]"""
 ULongArray = ArrayType('L', int)
 """Stores unsigned 32-bit integers. [0; 4294967295]"""
```

### Comparing `hurray-1.0.0/pyproject.toml` & `hurray-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.13",
     "Topic :: Utilities",
     "Typing :: Typed"
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/SyberiaK/hurray"
```

