# Comparing `tmp/netsome-0.3.3.tar.gz` & `tmp/netsome-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsome-0.3.3.tar", max compression
+gzip compressed data, was "netsome-0.3.4.tar", max compression
```

## Comparing `netsome-0.3.3.tar` & `netsome-0.3.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1286 2024-04-11 18:59:46.819718 netsome-0.3.3/LICENSE
--rw-r--r--   0        0        0      355 2024-04-15 07:10:06.582777 netsome-0.3.3/README.md
--rw-r--r--   0        0        0        0 2024-04-11 18:59:46.820411 netsome-0.3.3/netsome/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 18:59:46.820647 netsome-0.3.3/netsome/_converters/__init__.py
--rw-r--r--   0        0        0      967 2024-04-15 07:10:54.993891 netsome-0.3.3/netsome/_converters/bgp.py
--rw-r--r--   0        0        0      343 2024-04-15 07:10:54.994197 netsome-0.3.3/netsome/_converters/ipv4.py
--rw-r--r--   0        0        0      662 2024-04-15 18:22:42.950755 netsome-0.3.3/netsome/constants.py
--rw-r--r--   0        0        0        0 2024-04-11 18:59:46.823365 netsome-0.3.3/netsome/types/__init__.py
--rw-r--r--   0        0        0     2219 2024-04-15 07:10:54.995099 netsome-0.3.3/netsome/types/bgp.py
--rw-r--r--   0        0        0     4510 2024-04-15 07:10:55.013884 netsome-0.3.3/netsome/types/ipv4.py
--rw-r--r--   0        0        0      906 2024-04-15 07:10:55.014565 netsome-0.3.3/netsome/types/vlans.py
--rw-r--r--   0        0        0        0 2024-04-11 18:59:46.824730 netsome-0.3.3/netsome/validators/__init__.py
--rw-r--r--   0        0        0     2022 2024-04-15 18:35:57.465187 netsome-0.3.3/netsome/validators/bgp.py
--rw-r--r--   0        0        0     2112 2024-04-15 19:18:19.904520 netsome-0.3.3/netsome/validators/ipv4.py
--rw-r--r--   0        0        0      381 2024-04-15 07:10:55.016488 netsome-0.3.3/netsome/validators/vlans.py
--rw-r--r--   0        0        0     1234 2024-04-17 18:11:35.677357 netsome-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 netsome-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1286 2024-04-11 18:59:46.819718 netsome-0.3.4/LICENSE
+-rw-r--r--   0        0        0      355 2024-04-15 07:10:06.582777 netsome-0.3.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 18:59:46.820411 netsome-0.3.4/netsome/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:59:46.820647 netsome-0.3.4/netsome/_converters/__init__.py
+-rw-r--r--   0        0        0      967 2024-04-20 09:23:59.212783 netsome-0.3.4/netsome/_converters/bgp.py
+-rw-r--r--   0        0        0      343 2024-04-20 09:23:59.213195 netsome-0.3.4/netsome/_converters/ipv4.py
+-rw-r--r--   0        0        0     1056 2024-04-21 19:30:32.626766 netsome-0.3.4/netsome/constants.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:59:46.823365 netsome-0.3.4/netsome/types/__init__.py
+-rw-r--r--   0        0        0     2219 2024-04-20 09:23:59.214154 netsome-0.3.4/netsome/types/bgp.py
+-rw-r--r--   0        0        0     4510 2024-04-21 19:30:32.627924 netsome-0.3.4/netsome/types/ipv4.py
+-rw-r--r--   0        0        0     3629 2024-04-27 09:10:55.543541 netsome-0.3.4/netsome/types/mac.py
+-rw-r--r--   0        0        0      906 2024-04-20 09:23:59.215917 netsome-0.3.4/netsome/types/vlans.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:59:46.824730 netsome-0.3.4/netsome/validators/__init__.py
+-rw-r--r--   0        0        0     2022 2024-04-20 09:23:59.216841 netsome-0.3.4/netsome/validators/bgp.py
+-rw-r--r--   0        0        0     2112 2024-04-20 09:23:59.217488 netsome-0.3.4/netsome/validators/ipv4.py
+-rw-r--r--   0        0        0      381 2024-04-20 09:23:59.218189 netsome-0.3.4/netsome/validators/vlans.py
+-rw-r--r--   0        0        0     1234 2024-04-27 09:11:32.080276 netsome-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 netsome-0.3.4/PKG-INFO
```

### Comparing `netsome-0.3.3/LICENSE` & `netsome-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `netsome-0.3.3/netsome/_converters/bgp.py` & `netsome-0.3.4/netsome/_converters/bgp.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.3/netsome/constants.py` & `netsome-0.3.4/netsome/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 import enum
 
 
+class NUMERALSYSTEMS(enum.IntEnum):
+    BIN = 2
+    DEC = 10
+    HEX = 16
+
+
 class BYTES(enum.IntEnum):
 
     ZERO = 0
     ONE = 2**8
-    TWO = ONE**2
-    FOUR = TWO**2
+    TWO = 2 ** (8 * 2)
+    THREE = 2 ** (8 * 3)
+    FOUR = 2 ** (8 * 4)
+    FIVE = 2 ** (8 * 5)
+    SIX = 2 ** (8 * 6)
+    EIGHT = 2 ** (8 * 8)
 
 
 class DELIMITERS(str, enum.Enum):
 
     DASH = "-"
     DOT = "."
     COLON = ":"
@@ -41,7 +51,19 @@
 
 
 class BGP(enum.IntEnum):
 
     ASN_MIN = 0
     ASN_MAX = BYTES.FOUR - 1
     ASN_ORDER_MAX = BYTES.TWO - 1
+
+
+class MAC(enum.IntEnum):
+
+    ADDRESS_MIN = 0
+    ADDRESS_MAX = BYTES.SIX - 1
+
+    OUI_MAX = BYTES.THREE - 1
+    NIC_MAX = BYTES.THREE - 1
+
+    NIC64_MAX = BYTES.FIVE - 1
+    ADDRESS64_MAX = BYTES.EIGHT - 1
```

### Comparing `netsome-0.3.3/netsome/types/bgp.py` & `netsome-0.3.4/netsome/types/bgp.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.3/netsome/types/ipv4.py` & `netsome-0.3.4/netsome/types/ipv4.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.3/netsome/types/vlans.py` & `netsome-0.3.4/netsome/types/vlans.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.3/netsome/validators/bgp.py` & `netsome-0.3.4/netsome/validators/bgp.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.3/netsome/validators/ipv4.py` & `netsome-0.3.4/netsome/validators/ipv4.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.3/pyproject.toml` & `netsome-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ]
 description = "The one and only library to make your network code handsome"
 keywords = ["library", "network"]
 license = "X11 License Distribution Modification Variant"
 name = "netsome"
 readme = "README.md"
 repository = "https://github.com/kuderr/netsome"
-version = "0.3.3"
+version = "0.3.4"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
 poethepoet = "^0.25.0"
 pytest = "^8.1.1"
```

### Comparing `netsome-0.3.3/PKG-INFO` & `netsome-0.3.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsome
-Version: 0.3.3
+Version: 0.3.4
 Summary: The one and only library to make your network code handsome
 Home-page: https://github.com/kuderr/netsome
 License: X11-distribute-modifications-variant
 Keywords: library,network
 Author: kuderr
 Author-email: dakudryavcev@gmail.com
 Requires-Python: >=3.10,<4.0
```

