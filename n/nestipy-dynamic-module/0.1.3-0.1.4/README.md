# Comparing `tmp/nestipy_dynamic_module-0.1.3.tar.gz` & `tmp/nestipy_dynamic_module-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy_dynamic_module-0.1.3.tar", max compression
+gzip compressed data, was "nestipy_dynamic_module-0.1.4.tar", max compression
```

## Comparing `nestipy_dynamic_module-0.1.3.tar` & `nestipy_dynamic_module-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-22 14:55:15.443739 nestipy_dynamic_module-0.1.3/README.md
--rw-r--r--   0        0        0      399 2024-04-25 14:50:30.994478 nestipy_dynamic_module-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      231 2024-04-24 07:15:09.916835 nestipy_dynamic_module-0.1.3/src/nestipy_dynamic_module/__init__.py
--rw-r--r--   0        0        0     2421 2024-04-25 14:50:00.330266 nestipy_dynamic_module-0.1.3/src/nestipy_dynamic_module/builder.py
--rw-r--r--   0        0        0      139 2024-04-24 07:14:46.993633 nestipy_dynamic_module-0.1.3/src/nestipy_dynamic_module/module/__init__.py
--rw-r--r--   0        0        0      517 2024-04-24 07:08:05.538940 nestipy_dynamic_module-0.1.3/src/nestipy_dynamic_module/module/consumer.py
--rw-r--r--   0        0        0      251 2024-04-24 07:14:10.682894 nestipy_dynamic_module-0.1.3/src/nestipy_dynamic_module/module/interface.py
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 nestipy_dynamic_module-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy_dynamic_module-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1906 2024-04-26 13:39:21.397719 nestipy_dynamic_module-0.1.4/README.md
+-rw-r--r--   0        0        0      399 2024-04-27 06:18:19.307796 nestipy_dynamic_module-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-04-24 07:15:09.916835 nestipy_dynamic_module-0.1.4/src/nestipy_dynamic_module/__init__.py
+-rw-r--r--   0        0        0     2544 2024-04-27 06:16:16.063842 nestipy_dynamic_module-0.1.4/src/nestipy_dynamic_module/builder.py
+-rw-r--r--   0        0        0      139 2024-04-24 07:14:46.993633 nestipy_dynamic_module-0.1.4/src/nestipy_dynamic_module/module/__init__.py
+-rw-r--r--   0        0        0      517 2024-04-24 07:08:05.538940 nestipy_dynamic_module-0.1.4/src/nestipy_dynamic_module/module/consumer.py
+-rw-r--r--   0        0        0      251 2024-04-24 07:14:10.682894 nestipy_dynamic_module-0.1.4/src/nestipy_dynamic_module/module/interface.py
+-rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 nestipy_dynamic_module-0.1.4/PKG-INFO
```

### Comparing `nestipy_dynamic_module-0.1.3/src/nestipy_dynamic_module/builder.py` & `nestipy_dynamic_module-0.1.4/src/nestipy_dynamic_module/builder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import uuid
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import TypeVar, Generic, Optional, Any, Callable, Union, Type, Awaitable
 
 from nestipy_ioc import ModuleProviderDict
 from nestipy_metadata import ModuleMetadata, Reflect
 
 T = TypeVar('T')
 
 
 @dataclass
 class DynamicModule:
     module: Any
-    exports: list = None
-    imports: list = None
-    providers: list = None
-    controllers: list = None
+    exports: list = field(default_factory=lambda: [])
+    imports: list = field(default_factory=lambda: [])
+    providers: list = field(default_factory=lambda: [])
+    controllers: list = field(default_factory=lambda: [])
     is_global: bool = False
 
 
 class ConfigurableModuleBuilder(Generic[T]):
     def __init__(self):
         self._method_name = 'register'
```

### Comparing `nestipy_dynamic_module-0.1.3/src/nestipy_dynamic_module/module/consumer.py` & `nestipy_dynamic_module-0.1.4/src/nestipy_dynamic_module/module/consumer.py`

 * *Files identical despite different names*

