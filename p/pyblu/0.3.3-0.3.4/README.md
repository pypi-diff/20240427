# Comparing `tmp/pyblu-0.3.3.tar.gz` & `tmp/pyblu-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyblu-0.3.3.tar", max compression
+gzip compressed data, was "pyblu-0.3.4.tar", max compression
```

## Comparing `pyblu-0.3.3.tar` & `pyblu-0.3.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2024-03-09 09:45:55.409568 pyblu-0.3.3/LICENSE
--rw-r--r--   0        0        0      873 2024-04-12 16:28:03.088001 pyblu-0.3.3/README.md
--rw-r--r--   0        0        0      921 2024-04-27 09:52:27.298810 pyblu-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      277 2024-04-14 21:03:17.059292 pyblu-0.3.3/src/pyblu/__init__.py
--rw-r--r--   0        0        0     4334 2024-04-27 09:49:20.789539 pyblu-0.3.3/src/pyblu/_entities.py
--rw-r--r--   0        0        0     6035 2024-04-27 09:49:20.798539 pyblu-0.3.3/src/pyblu/_parse.py
--rw-r--r--   0        0        0    14367 2024-04-20 09:50:30.350831 pyblu-0.3.3/src/pyblu/_player.py
--rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 pyblu-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-09 09:45:55.409568 pyblu-0.3.4/LICENSE
+-rw-r--r--   0        0        0      873 2024-04-12 16:28:03.088001 pyblu-0.3.4/README.md
+-rw-r--r--   0        0        0      921 2024-04-27 09:57:54.150415 pyblu-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      277 2024-04-14 21:03:17.059292 pyblu-0.3.4/src/pyblu/__init__.py
+-rw-r--r--   0        0        0     4338 2024-04-27 09:57:31.717983 pyblu-0.3.4/src/pyblu/_entities.py
+-rw-r--r--   0        0        0     6039 2024-04-27 09:57:31.749983 pyblu-0.3.4/src/pyblu/_parse.py
+-rw-r--r--   0        0        0    14367 2024-04-20 09:50:30.350831 pyblu-0.3.4/src/pyblu/_player.py
+-rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 pyblu-0.3.4/PKG-INFO
```

### Comparing `pyblu-0.3.3/LICENSE` & `pyblu-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyblu-0.3.3/README.md` & `pyblu-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pyblu-0.3.3/pyproject.toml` & `pyblu-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyblu"
-version = "0.3.3"
+version = "0.3.4"
 description = ""
 authors = ["Louis Christ <mail@louischrist.de>"]
 repository = "https://github.com/LouisChrist/pyblu"
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "pyblu", from = "src" },
```

### Comparing `pyblu-0.3.3/src/pyblu/_entities.py` & `pyblu-0.3.4/src/pyblu/_entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,20 +98,20 @@
     brand: str
     """Brand name of the player"""
     model: str
     """Model name of the player"""
     model_name: str
     """Model name of the player"""
 
-    mute_volume_db: int | None
+    mute_volume_db: float | None
     """If the player is muted, then this is the unmuted volume level in dB. Absent if the player is not muted."""
     mute_volume: int | None
     """If the player is muted, then this is the unmuted volume level. Absent if the player is not muted."""
 
-    volume_db: int
+    volume_db: float
     """Volume level in dB"""
     volume: int
     """Volume level with a range of 0-100. -1 means fixed volume."""
 
 
 @dataclass
 class Volume:
```

### Comparing `pyblu-0.3.3/src/pyblu/_parse.py` & `pyblu-0.3.4/src/pyblu/_parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,17 +50,17 @@
         slaves=slaves,
         zone=chained_get(response_dict, "SyncStatus", "@zone"),
         zone_master=chained_get(response_dict, "SyncStatus", "@zoneMaster") == "true",
         zone_slave=chained_get(response_dict, "SyncStatus", "@zoneSlave") == "true",
         brand=chained_get(response_dict, "SyncStatus", "@brand"),
         model=chained_get(response_dict, "SyncStatus", "@model"),
         model_name=chained_get(response_dict, "SyncStatus", "@modelName"),
-        mute_volume_db=chained_get(response_dict, "SyncStatus", "@muteDb", _map=int),
+        mute_volume_db=chained_get(response_dict, "SyncStatus", "@muteDb", _map=float),
         mute_volume=chained_get(response_dict, "SyncStatus", "@muteVolume", _map=int),
-        volume_db=chained_get(response_dict, "SyncStatus", "@db", _map=int),
+        volume_db=chained_get(response_dict, "SyncStatus", "@db", _map=float),
         volume=chained_get(response_dict, "SyncStatus", "@volume", _map=int),
     )
 
     return sync_status
 
 
 def parse_status(response_dict: dict[str, Any]) -> Status:
```

### Comparing `pyblu-0.3.3/src/pyblu/_player.py` & `pyblu-0.3.4/src/pyblu/_player.py`

 * *Files identical despite different names*

### Comparing `pyblu-0.3.3/PKG-INFO` & `pyblu-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyblu
-Version: 0.3.3
+Version: 0.3.4
 Summary: 
 Home-page: https://github.com/LouisChrist/pyblu
 License: MIT
 Author: Louis Christ
 Author-email: mail@louischrist.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

