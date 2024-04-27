# Comparing `tmp/smp-0.3.4.tar.gz` & `tmp/smp-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smp-0.3.4.tar", max compression
+gzip compressed data, was "smp-1.0.0.tar", max compression
```

## Comparing `smp-0.3.4.tar` & `smp-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11365 2024-04-24 23:26:42.128815 smp-0.3.4/LICENSE
--rw-r--r--   0        0        0     2243 2024-04-24 23:26:42.128815 smp-0.3.4/README.md
--rw-r--r--   0        0        0      953 2024-04-24 23:26:42.128815 smp-0.3.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 23:26:42.128815 smp-0.3.4/smp/__init__.py
--rw-r--r--   0        0        0      659 2024-04-24 23:26:42.128815 smp-0.3.4/smp/error.py
--rw-r--r--   0        0        0      471 2024-04-24 23:26:42.128815 smp-0.3.4/smp/exceptions.py
--rw-r--r--   0        0        0     4905 2024-04-24 23:26:42.128815 smp-0.3.4/smp/header.py
--rw-r--r--   0        0        0     6149 2024-04-24 23:26:42.128815 smp-0.3.4/smp/image_management.py
--rw-r--r--   0        0        0     4822 2024-04-24 23:26:42.128815 smp-0.3.4/smp/message.py
--rw-r--r--   0        0        0     6761 2024-04-24 23:26:42.128815 smp-0.3.4/smp/os_management.py
--rw-r--r--   0        0        0     3135 2024-04-24 23:26:42.128815 smp-0.3.4/smp/packet.py
--rw-r--r--   0        0        0        0 2024-04-24 23:26:42.128815 smp-0.3.4/smp/py.typed
--rw-r--r--   0        0        0     1071 2024-04-24 23:26:42.128815 smp-0.3.4/smp/shell_management.py
--rw-r--r--   0        0        0        0 2024-04-24 23:26:42.128815 smp-0.3.4/smp/user/__init__.py
--rw-r--r--   0        0        0     1359 2024-04-24 23:26:42.128815 smp-0.3.4/smp/user/intercreate.py
--rw-r--r--   0        0        0     2894 1970-01-01 00:00:00.000000 smp-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0    11365 2024-04-27 18:16:42.546318 smp-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2243 2024-04-27 18:16:42.546318 smp-1.0.0/README.md
+-rw-r--r--   0        0        0      953 2024-04-27 18:16:42.546318 smp-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-27 18:16:42.546318 smp-1.0.0/smp/__init__.py
+-rw-r--r--   0        0        0      659 2024-04-27 18:16:42.546318 smp-1.0.0/smp/error.py
+-rw-r--r--   0        0        0      471 2024-04-27 18:16:42.546318 smp-1.0.0/smp/exceptions.py
+-rw-r--r--   0        0        0     4978 2024-04-27 18:16:42.546318 smp-1.0.0/smp/header.py
+-rw-r--r--   0        0        0     6149 2024-04-27 18:16:42.546318 smp-1.0.0/smp/image_management.py
+-rw-r--r--   0        0        0     4846 2024-04-27 18:16:42.546318 smp-1.0.0/smp/message.py
+-rw-r--r--   0        0        0     6761 2024-04-27 18:16:42.546318 smp-1.0.0/smp/os_management.py
+-rw-r--r--   0        0        0     3135 2024-04-27 18:16:42.546318 smp-1.0.0/smp/packet.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:16:42.546318 smp-1.0.0/smp/py.typed
+-rw-r--r--   0        0        0     1071 2024-04-27 18:16:42.546318 smp-1.0.0/smp/shell_management.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:16:42.546318 smp-1.0.0/smp/user/__init__.py
+-rw-r--r--   0        0        0     1371 2024-04-27 18:16:42.546318 smp-1.0.0/smp/user/intercreate.py
+-rw-r--r--   0        0        0     2894 1970-01-01 00:00:00.000000 smp-1.0.0/PKG-INFO
```

### Comparing `smp-0.3.4/LICENSE` & `smp-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smp-0.3.4/README.md` & `smp-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `smp-0.3.4/pyproject.toml` & `smp-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smp-0.3.4/smp/error.py` & `smp-1.0.0/smp/error.py`

 * *Files identical despite different names*

### Comparing `smp-0.3.4/smp/header.py` & `smp-1.0.0/smp/header.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,27 +36,34 @@
     class Intercreate(IntEnum):
         UPLOAD = 1
 
 
 AnyCommandId: TypeAlias = IntEnum | int
 
 
+@unique
 class GroupId(IntEnum):
     OS_MANAGEMENT = 0
     IMAGE_MANAGEMENT = 1
     STATISTICS_MANAGEMENT = 2
     SETTINGS_MANAGEMENT = 3
     LOG_MANAGEMENT = 4
     RUNTIME_TESTS = 5
     SPLIT_IMAGE_MANAGEMENT = 6
     TEST_CRASH = 7
     FILE_MANAGEMENT = 8
     SHELL_MANAGEMENT = 9
     ZEPHYR = 63
-    _APPLICATIION_CUSTOM_MIN = 64
+
+
+class UserGroupId(IntEnum):
+    """Users may define their own Group IDs starting at 64.
+
+    It is optional to register them here."""
+
     INTERCREATE = 64
 
 
 AnyGroupId: TypeAlias = IntEnum | int
 
 
 @unique
@@ -90,29 +97,28 @@
 
 @dataclass(frozen=True)
 class Header:
     op: OP
     version: Version
     flags: Flag
     length: int
-    group_id: AnyGroupId | GroupId
+    group_id: AnyGroupId | GroupId | UserGroupId
     sequence: int
     command_id: (
         AnyCommandId
         | CommandId.OSManagement
         | CommandId.ImageManagement
         | CommandId.ShellManagement
         | CommandId.Intercreate
     )
 
     _MAP_GROUP_ID_TO_COMMAND_ID_ENUM: ClassVar[Dict[int, Type[IntEnum]]] = {
         GroupId.OS_MANAGEMENT: CommandId.OSManagement,
         GroupId.IMAGE_MANAGEMENT: CommandId.ImageManagement,
         GroupId.SHELL_MANAGEMENT: CommandId.ShellManagement,
-        GroupId.INTERCREATE: CommandId.Intercreate,
     }
     _STRUCT: ClassVar = struct.Struct("!BBHHBB")
     SIZE: ClassVar = _STRUCT.size
 
     @staticmethod
     def _pack_op(op: OP) -> int:
         """The value to be packed into the byte."""
```

### Comparing `smp-0.3.4/smp/image_management.py` & `smp-1.0.0/smp/image_management.py`

 * *Files identical despite different names*

### Comparing `smp-0.3.4/smp/message.py` & `smp-1.0.0/smp/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class _MessageBase(ABC, BaseModel):
     model_config = ConfigDict(extra="forbid", frozen=True)
 
     _OP: ClassVar[smpheader.OP]
     _VERSION: ClassVar[smpheader.Version] = smpheader.Version.V0
     _FLAGS: ClassVar[smpheader.Flag] = smpheader.Flag(0)
-    _GROUP_ID: ClassVar[smpheader.GroupId | smpheader.AnyGroupId]
+    _GROUP_ID: ClassVar[smpheader.GroupId | smpheader.UserGroupId | smpheader.AnyGroupId]
     _COMMAND_ID: ClassVar[
         smpheader.AnyCommandId
         | smpheader.CommandId.ImageManagement
         | smpheader.CommandId.OSManagement
         | smpheader.CommandId.ShellManagement
         | smpheader.CommandId.Intercreate
     ]
```

### Comparing `smp-0.3.4/smp/os_management.py` & `smp-1.0.0/smp/os_management.py`

 * *Files identical despite different names*

### Comparing `smp-0.3.4/smp/packet.py` & `smp-1.0.0/smp/packet.py`

 * *Files identical despite different names*

### Comparing `smp-0.3.4/smp/shell_management.py` & `smp-1.0.0/smp/shell_management.py`

 * *Files identical despite different names*

### Comparing `smp-0.3.4/smp/user/intercreate.py` & `smp-1.0.0/smp/user/intercreate.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from enum import IntEnum, auto, unique
 from typing import ClassVar
 
 from smp import error, header, message
 
 
 class _IntercreateManagementGroup:
-    _GROUP_ID: ClassVar = header.GroupId.INTERCREATE
+    _GROUP_ID: ClassVar = header.UserGroupId.INTERCREATE
 
 
 class ImageUploadWriteRequest(_IntercreateManagementGroup, message.WriteRequest):
     _COMMAND_ID = header.CommandId.Intercreate.UPLOAD
 
     off: int
     """The offset in the image to write to."""
@@ -42,12 +42,12 @@
     """No error."""
 
     INVALID_IMAGE = auto()
     """No image matched the image provided."""
 
 
 class ErrorV0(error.ErrorV0[IC_MGMT_ERR]):
-    _GROUP_ID = header.GroupId.INTERCREATE
+    _GROUP_ID = header.UserGroupId.INTERCREATE
 
 
 class ErrorV1(error.ErrorV1[IC_MGMT_ERR]):
-    _GROUP_ID = header.GroupId.INTERCREATE
+    _GROUP_ID = header.UserGroupId.INTERCREATE
```

### Comparing `smp-0.3.4/PKG-INFO` & `smp-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smp
-Version: 0.3.4
+Version: 1.0.0
 Summary: Simple Management Protocol (SMP) for remotely managing MCU firmware
 License: Apache-2.0
 Author: J.P. Hutchins
 Author-email: jphutchins@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

