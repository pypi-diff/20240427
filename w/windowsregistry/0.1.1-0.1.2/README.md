# Comparing `tmp/windowsregistry-0.1.1.tar.gz` & `tmp/windowsregistry-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windowsregistry-0.1.1.tar", max compression
+gzip compressed data, was "windowsregistry-0.1.2.tar", max compression
```

## Comparing `windowsregistry-0.1.1.tar` & `windowsregistry-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1120 2024-04-05 12:39:11.058256 windowsregistry-0.1.1/LICENSE
--rw-r--r--   0        0        0      464 2024-04-05 12:39:11.059283 windowsregistry-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-20 15:48:08.622855 windowsregistry-0.1.1/README.md
--rw-r--r--   0        0        0      476 2024-04-05 12:39:11.060258 windowsregistry-0.1.1/windowsregistry/__init__.py
--rw-r--r--   0        0        0     4284 2024-04-03 15:01:34.954247 windowsregistry-0.1.1/windowsregistry/_backend.py
--rw-r--r--   0        0        0     1510 2024-04-03 15:02:11.711534 windowsregistry-0.1.1/windowsregistry/_lowlevel.py
--rw-r--r--   0        0        0     5146 2024-04-04 15:00:34.353575 windowsregistry-0.1.1/windowsregistry/core.py
--rw-r--r--   0        0        0       50 2024-01-20 16:09:24.321620 windowsregistry-0.1.1/windowsregistry/errors.py
--rw-r--r--   0        0        0      522 2024-04-02 10:07:41.474792 windowsregistry-0.1.1/windowsregistry/models/__init__.py
--rw-r--r--   0        0        0      434 2024-04-02 10:07:41.476324 windowsregistry-0.1.1/windowsregistry/models/data.py
--rw-r--r--   0        0        0     2777 2024-04-01 13:51:14.444092 windowsregistry-0.1.1/windowsregistry/models/enums.py
--rw-r--r--   0        0        0     2300 2024-04-03 12:33:54.931151 windowsregistry-0.1.1/windowsregistry/regpath.py
--rw-r--r--   0        0        0      377 2024-04-02 15:35:52.786369 windowsregistry-0.1.1/windowsregistry/utils.py
--rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 windowsregistry-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1120 2024-04-05 12:39:11.058256 windowsregistry-0.1.2/LICENSE
+-rw-r--r--   0        0        0      464 2024-04-27 11:46:24.587809 windowsregistry-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-20 15:48:08.622855 windowsregistry-0.1.2/README.md
+-rw-r--r--   0        0        0      476 2024-04-05 12:39:11.060258 windowsregistry-0.1.2/windowsregistry/__init__.py
+-rw-r--r--   0        0        0     4456 2024-04-27 11:46:24.589820 windowsregistry-0.1.2/windowsregistry/_backend.py
+-rw-r--r--   0        0        0     1510 2024-04-24 11:39:24.667624 windowsregistry-0.1.2/windowsregistry/_lowlevel.py
+-rw-r--r--   0        0        0     5719 2024-04-27 11:46:24.590783 windowsregistry-0.1.2/windowsregistry/core.py
+-rw-r--r--   0        0        0       50 2024-01-20 16:09:24.321620 windowsregistry-0.1.2/windowsregistry/errors.py
+-rw-r--r--   0        0        0      562 2024-04-27 11:46:24.591781 windowsregistry-0.1.2/windowsregistry/models/__init__.py
+-rw-r--r--   0        0        0      684 2024-04-27 11:46:24.592780 windowsregistry-0.1.2/windowsregistry/models/data.py
+-rw-r--r--   0        0        0     2777 2024-04-01 13:51:14.444092 windowsregistry-0.1.2/windowsregistry/models/enums.py
+-rw-r--r--   0        0        0     2302 2024-04-27 11:46:24.593779 windowsregistry-0.1.2/windowsregistry/regpath.py
+-rw-r--r--   0        0        0      447 2024-04-27 11:46:24.593779 windowsregistry-0.1.2/windowsregistry/utils.py
+-rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 windowsregistry-0.1.2/PKG-INFO
```

### Comparing `windowsregistry-0.1.1/LICENSE` & `windowsregistry-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `windowsregistry-0.1.1/windowsregistry/_backend.py` & `windowsregistry-0.1.2/windowsregistry/_backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,27 +19,30 @@
 
 class WindowsRegistryHandler:
     def __init__(
         self,
         subkey: Union[str, Sequence[str], None] = None,
         *,
         root_key: Optional[RegistryHKEYEnum] = None,
-        permission: Optional[RegistryKeyPermissionType] = None,
+        permission: Optional[Union[RegistryKeyPermissionType, Sequence[RegistryKeyPermissionType]]] = None,
         wow64_32key_access: bool = False,
     ) -> None:
         if subkey is None:
             subkey = []
         elif isinstance(subkey, str):
             subkey = [subkey]
         if permission is None:
             permission = RegistryKeyPermissionType.KEY_READ
+        if isinstance(permission, RegistryKeyPermissionType):
+            permission = [permission]
         self._regpath = RegistryPathString(*subkey, root_key=root_key)
         self._ll = lowlevel(
             permconf=RegistryPermissionConfig(
-                permission=permission, wow64_32key_access=wow64_32key_access
+                permissions=tuple(permission),
+                wow64_32key_access=wow64_32key_access
             )
         )
         self._winreg_handler = self._ll.open_subkey(
             self._regpath.root_key.value, self._regpath.path
         )
         self._winreg_query = RegistryInfoKey(
             *self._ll.query_subkey(self._winreg_handler)
@@ -67,15 +70,15 @@
 
     def new_handler_from_path(
         self, subkey_parts: Sequence[str]
     ) -> "WindowsRegistryHandler":
         return self.__class__(
             subkey=subkey_parts,
             root_key=self._regpath.root_key,
-            permission=self._ll._permconf.permission,
+            permission=self._ll._permconf.permissions,
             wow64_32key_access=self._ll._permconf.wow64_32key_access,
         )
 
     def subkey_exists(self, subkey: str):
         try:
             self._ll.open_subkey(self.winreg_handler, subkey)
             return True
```

### Comparing `windowsregistry-0.1.1/windowsregistry/_lowlevel.py` & `windowsregistry-0.1.2/windowsregistry/_lowlevel.py`

 * *Files identical despite different names*

### Comparing `windowsregistry-0.1.1/windowsregistry/core.py` & `windowsregistry-0.1.2/windowsregistry/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from collections import deque
 from typing import Any, Iterator, Optional, Sequence, Union
 
-from windowsregistry.regpath import RegistryPathString
 
+from .regpath import RegistryPathString
 from ._backend import WindowsRegistryHandler
 from .errors import WindowsRegistryError
 from .models import (
     RegistryHKEYEnum,
     RegistryKeyPermissionType,
     RegistryValue,
     RegistryValueType,
+    RegistryInfoKey,
+    RegistrySize
 )
 
 
 class RegistryPath:
     def __init__(
         self,
         subkey: Union[None, str, Sequence[str]] = None,
@@ -30,15 +32,15 @@
         )
 
     def _sanargs(self, perm, w64):
         return (
             (
                 perm
                 if perm is not None
-                else self._backend._ll._permconf.permission
+                else self._backend._ll._permconf.permissions
             ),
             (
                 w64
                 if w64 is not None
                 else self._backend._ll._permconf.wow64_32key_access
             )
         )
@@ -53,14 +55,18 @@
         )
 
     @property
     def regpath(self) -> RegistryPathString:
         return self._backend._regpath
 
     @property
+    def query_info(self) -> RegistryInfoKey:
+        return self._backend.winreg_query
+
+    @property
     def parent(self) -> "RegistryPath":
         return self._internal_open_subkey(self.regpath.parent)
 
     def open_subkey(
         self,
         *paths: str,
         permission: Optional[RegistryKeyPermissionType] = None,
@@ -129,14 +135,26 @@
         while stacks:
             curr = stacks.popleft()
             subkeys_in_curr = tuple(curr.subkeys())
             values_in_curr = tuple(curr.values())
             yield curr, subkeys_in_curr, values_in_curr
             stacks.extend(subkeys_in_curr)
 
+    def sizeof(self) -> RegistrySize:
+        cached = getattr(self, "__cached_sizeof", None)
+        if cached is not None:
+            return cached
+        sub, val = 0, 0
+        for r, _, _ in self.traverse():
+            sub += r.query_info.total_subkeys
+            val += r.query_info.total_values
+        final = RegistrySize(self.regpath, sub, val)
+        setattr(self, "__cached_sizeof", final)
+        return final
+
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__}: {self.regpath.fullpath} at {hex(id(self))}>"
 
 
 def open_subkey(
     *path: str,
     root_key: Optional[RegistryHKEYEnum] = None,
```

### Comparing `windowsregistry-0.1.1/windowsregistry/models/__init__.py` & `windowsregistry-0.1.2/windowsregistry/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,21 +4,23 @@
     RegistryAlternateViewType,
     OtherRegistryType
 )
 from .data import (
     RegistryInfoKey,
     RegistryValue,
     RegistryValueType,
-    RegistryPermissionConfig
+    RegistryPermissionConfig,
+    RegistrySize
 )
 
 __all__ = [
     "RegistryHKEYEnum",
     "RegistryKeyPermissionType",
     "RegistryAlternateViewType",
     "RegistryValueType",
     "RegistryPermissionConfig",
+    "RegistrySize",
     "OtherRegistryType",
     "RegistryInfoKey",
     "RegistryValue",
     "RegistryValueType"
 ]
```

### Comparing `windowsregistry-0.1.1/windowsregistry/models/enums.py` & `windowsregistry-0.1.2/windowsregistry/models/enums.py`

 * *Files identical despite different names*

### Comparing `windowsregistry-0.1.1/windowsregistry/regpath.py` & `windowsregistry-0.1.2/windowsregistry/regpath.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,11 +72,11 @@
         return self.parts[-1]
     
     def joinpath(self, *paths: str) -> "RegistryPathString":
         parts = [*self.parts, *_parse_parts(paths)]
         return self.__class__(*parts, root_key=self.root_key)
     
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}({self.fullpath})"
+        return f"{self.__class__.__name__}({self.fullpath!r})"
     
     def __str__(self) -> str:
         return self.fullpath
```

### Comparing `windowsregistry-0.1.1/PKG-INFO` & `windowsregistry-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windowsregistry
-Version: 0.1.1
+Version: 0.1.2
 Summary: Windows Registry Editor with Pythonic interface
 Home-page: https://github.com/DinhHuy2010/windowsregistry.py
 License: MIT
 Author: DinhHuy2010
 Author-email: huy04052010@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

