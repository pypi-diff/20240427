# Comparing `tmp/csxhair-1.0.0.tar.gz` & `tmp/csxhair-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csxhair-1.0.0.tar", last modified: Sat Sep  9 12:10:03 2023, max compression
+gzip compressed data, was "csxhair-1.0.1.tar", last modified: Sat Apr 27 04:18:02 2024, max compression
```

## Comparing `csxhair-1.0.0.tar` & `csxhair-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-09 12:10:03.848132 csxhair-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-09-09 12:09:49.000000 csxhair-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2023-09-09 12:10:03.848132 csxhair-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      990 2023-09-09 12:09:49.000000 csxhair-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-09 12:10:03.848132 csxhair-1.0.0/csxhair.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2023-09-09 12:10:03.000000 csxhair-1.0.0/csxhair.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-09-09 12:10:03.000000 csxhair-1.0.0/csxhair.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-09 12:10:03.000000 csxhair-1.0.0/csxhair.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-09-09 12:10:03.000000 csxhair-1.0.0/csxhair.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-09-09 12:10:03.000000 csxhair-1.0.0/csxhair.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10849 2023-09-09 12:09:49.000000 csxhair-1.0.0/csxhair.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-09-09 12:09:49.000000 csxhair-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-09 12:10:03.848132 csxhair-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:18:02.551555 csxhair-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-27 04:17:55.000000 csxhair-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-27 04:18:02.551555 csxhair-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-27 04:17:55.000000 csxhair-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:18:02.551555 csxhair-1.0.1/csxhair/
+-rw-r--r--   0 runner    (1001) docker     (127)    10919 2024-04-27 04:17:55.000000 csxhair-1.0.1/csxhair/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:18:02.551555 csxhair-1.0.1/csxhair.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-27 04:18:02.000000 csxhair-1.0.1/csxhair.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-27 04:18:02.000000 csxhair-1.0.1/csxhair.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 04:18:02.000000 csxhair-1.0.1/csxhair.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-27 04:18:02.000000 csxhair-1.0.1/csxhair.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-27 04:18:02.000000 csxhair-1.0.1/csxhair.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-27 04:17:55.000000 csxhair-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 04:18:02.551555 csxhair-1.0.1/setup.cfg
```

### Comparing `csxhair-1.0.0/LICENSE` & `csxhair-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `csxhair-1.0.0/PKG-INFO` & `csxhair-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csxhair
-Version: 1.0.0
+Version: 1.0.1
 Summary: Decode, edit and encode CS:GO/CS2 crosshairs easily.
 Author: SyberiaK
 License: MIT License
         
         Copyright (c) 2023 SyberiaK
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,15 +44,16 @@
 
 # CSXhair
 
 [![PyPI release]][pypi] 
 [![Python supported versions]][pypi]
 [![License]](./LICENSE)
 
-CSXhair is a simple package for decoding/encoding CS:GO (and CS2!) crosshairs using share codes.
+CSXhair is a simple package for decoding/encoding CS:GO (and CS2!) crosshairs using game share codes. \
+All share codes are fully compatible with CS:GO/CS2.
 
 ```python
 from csxhair import Crosshair
 
 my_crosshair = Crosshair.decode('CSGO-ZEw8O-KGXNu-4TTUU-VyXbD-SBCtG')
 print(my_crosshair.gap)  # -3.0
 
@@ -64,7 +65,9 @@
 print(my_crosshair.cs2_commands)  # ['cl_crosshairgap -3.0', ..., 'cl_crosshairdot false', ...]
 ```
 
 [pypi]: https://pypi.org/project/csxhair/
 [PyPI Release]: https://img.shields.io/pypi/v/csxhair.svg?label=pypi&color=green
 [Python supported versions]: https://img.shields.io/pypi/pyversions/csxhair.svg?label=%20&logo=python&logoColor=white
 [License]: https://img.shields.io/pypi/l/csxhair.svg?style=flat&label=license
+
+*Special thanks to [Aquarius](https://github.com/aquaismissing) for making a rough implementation led to this package.*
```

### Comparing `csxhair-1.0.0/csxhair.egg-info/PKG-INFO` & `csxhair-1.0.1/csxhair.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csxhair
-Version: 1.0.0
+Version: 1.0.1
 Summary: Decode, edit and encode CS:GO/CS2 crosshairs easily.
 Author: SyberiaK
 License: MIT License
         
         Copyright (c) 2023 SyberiaK
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,15 +44,16 @@
 
 # CSXhair
 
 [![PyPI release]][pypi] 
 [![Python supported versions]][pypi]
 [![License]](./LICENSE)
 
-CSXhair is a simple package for decoding/encoding CS:GO (and CS2!) crosshairs using share codes.
+CSXhair is a simple package for decoding/encoding CS:GO (and CS2!) crosshairs using game share codes. \
+All share codes are fully compatible with CS:GO/CS2.
 
 ```python
 from csxhair import Crosshair
 
 my_crosshair = Crosshair.decode('CSGO-ZEw8O-KGXNu-4TTUU-VyXbD-SBCtG')
 print(my_crosshair.gap)  # -3.0
 
@@ -64,7 +65,9 @@
 print(my_crosshair.cs2_commands)  # ['cl_crosshairgap -3.0', ..., 'cl_crosshairdot false', ...]
 ```
 
 [pypi]: https://pypi.org/project/csxhair/
 [PyPI Release]: https://img.shields.io/pypi/v/csxhair.svg?label=pypi&color=green
 [Python supported versions]: https://img.shields.io/pypi/pyversions/csxhair.svg?label=%20&logo=python&logoColor=white
 [License]: https://img.shields.io/pypi/l/csxhair.svg?style=flat&label=license
+
+*Special thanks to [Aquarius](https://github.com/aquaismissing) for making a rough implementation led to this package.*
```

### Comparing `csxhair-1.0.0/csxhair.py` & `csxhair-1.0.1/csxhair/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 from __future__ import annotations
 
 import re
 
-from attrs import define, field, validators
+from attrs import Attribute, define, field, validators
 
-__version__ = '1.0.0'
+
+__version__ = '1.0.1'
 __all__ = ('Crosshair',)
 
 DICTIONARY = 'ABCDEFGHJKLMNOPQRSTUVWXYZabcdefhijkmnopqrstuvwxyz23456789'
 DICTIONARY_LENGTH = len(DICTIONARY)
 CODE_PATTERN = re.compile(r'CSGO(-[{%s}]{5}){5}$' % DICTIONARY)
 
 
-def signed_byte(x, /) -> int:
+def signed_byte(x: int, /) -> int:
     """Converts an unsigned byte to a signed one."""
 
     return (x ^ 0x80) - 0x80  # https://stackoverflow.com/a/37095855
 
 
-def lowercase_bool(x, /) -> str:
+def lowercase_bool(x: bool, /) -> str:
     """For the sake of values unifying - returns a lowercase string of bool (``'True'`` -> ``'true'``)."""
 
     if type(x) is bool:
         return str(x).lower()
 
     raise ValueError(f'Expected bool, got {x}')
 
 
-def _validate_bounds(lower_bound, upper_bound, /):
-    def inner(_, attribute, value):
+def _validate_bounds(lower_bound: int | float, upper_bound: int | float, /):
+    def inner(_, attribute: Attribute, value: int):
         if not (lower_bound <= value <= upper_bound):
-            raise ValueError(f"'{attribute}' has to be in range [{lower_bound}; {upper_bound}].")
+            raise ValueError(f"'{attribute.name}' has to be in range [{lower_bound}; {upper_bound}].")
 
     return inner
 
 
 @define
 class Crosshair:
     """Represents a CS:GO/CS2 crosshair."""
```

### Comparing `csxhair-1.0.0/pyproject.toml` & `csxhair-1.0.1/pyproject.toml`

 * *Files identical despite different names*

