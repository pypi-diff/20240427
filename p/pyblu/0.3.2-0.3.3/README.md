# Comparing `tmp/pyblu-0.3.2.tar.gz` & `tmp/pyblu-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyblu-0.3.2.tar", max compression
+gzip compressed data, was "pyblu-0.3.3.tar", max compression
```

## Comparing `pyblu-0.3.2.tar` & `pyblu-0.3.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2024-03-09 09:45:55.409568 pyblu-0.3.2/LICENSE
--rw-r--r--   0        0        0      873 2024-04-12 16:28:03.088001 pyblu-0.3.2/README.md
--rw-r--r--   0        0        0      921 2024-04-22 18:22:23.807364 pyblu-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      277 2024-04-14 21:03:17.059292 pyblu-0.3.2/src/pyblu/__init__.py
--rw-r--r--   0        0        0     4330 2024-04-22 18:21:45.409156 pyblu-0.3.2/src/pyblu/_entities.py
--rw-r--r--   0        0        0     6031 2024-04-22 18:21:45.442156 pyblu-0.3.2/src/pyblu/_parse.py
--rw-r--r--   0        0        0    14367 2024-04-20 09:50:30.350831 pyblu-0.3.2/src/pyblu/_player.py
--rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 pyblu-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-09 09:45:55.409568 pyblu-0.3.3/LICENSE
+-rw-r--r--   0        0        0      873 2024-04-12 16:28:03.088001 pyblu-0.3.3/README.md
+-rw-r--r--   0        0        0      921 2024-04-27 09:52:27.298810 pyblu-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      277 2024-04-14 21:03:17.059292 pyblu-0.3.3/src/pyblu/__init__.py
+-rw-r--r--   0        0        0     4334 2024-04-27 09:49:20.789539 pyblu-0.3.3/src/pyblu/_entities.py
+-rw-r--r--   0        0        0     6035 2024-04-27 09:49:20.798539 pyblu-0.3.3/src/pyblu/_parse.py
+-rw-r--r--   0        0        0    14367 2024-04-20 09:50:30.350831 pyblu-0.3.3/src/pyblu/_player.py
+-rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 pyblu-0.3.3/PKG-INFO
```

### Comparing `pyblu-0.3.2/LICENSE` & `pyblu-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyblu-0.3.2/README.md` & `pyblu-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pyblu-0.3.2/pyproject.toml` & `pyblu-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyblu"
-version = "0.3.2"
+version = "0.3.3"
 description = ""
 authors = ["Louis Christ <mail@louischrist.de>"]
 repository = "https://github.com/LouisChrist/pyblu"
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "pyblu", from = "src" },
```

### Comparing `pyblu-0.3.2/src/pyblu/_entities.py` & `pyblu-0.3.3/src/pyblu/_entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,22 +23,22 @@
     name: str
     """Track name"""
     image: str
     """URL of the album art"""
 
     volume: int
     """Volume level with a range of 0-100"""
-    volume_db: int
+    volume_db: float
     """Volume level in dB"""
 
     mute: bool
     """Mute status"""
     mute_volume: int | None
     """If the player is muted, then this is the unmuted volume level. Absent if the player is not muted."""
-    mute_volume_db: int | None
+    mute_volume_db: float | None
     """If the player is muted, then this is the unmuted volume level in dB. Absent if the player is not muted."""
 
     seconds: int
     """Current playback position in seconds"""
     total_seconds: float
     """Total track length in seconds"""
     can_seek: bool
```

### Comparing `pyblu-0.3.2/src/pyblu/_parse.py` & `pyblu-0.3.3/src/pyblu/_parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,18 +81,18 @@
         state=chained_get(response_dict, "status", "state"),
         shuffle=chained_get(response_dict, "status", "shuffle") == "1",
         album=album,
         artist=artist,
         name=name,
         image=chained_get(response_dict, "status", "image"),
         volume=chained_get(response_dict, "status", "volume", _map=int),
-        volume_db=chained_get(response_dict, "status", "db", _map=int),
+        volume_db=chained_get(response_dict, "status", "db", _map=float),
         mute=chained_get(response_dict, "status", "mute") == "1",
         mute_volume=chained_get(response_dict, "status", "muteVolume", _map=int),
-        mute_volume_db=chained_get(response_dict, "status", "muteDb", _map=int),
+        mute_volume_db=chained_get(response_dict, "status", "muteDb", _map=float),
         seconds=chained_get(response_dict, "status", "secs", _map=int),
         total_seconds=chained_get(response_dict, "status", "totlen", _map=float),
         can_seek=chained_get(response_dict, "status", "canSeek") == "1",
         sleep=chained_get(response_dict, "status", "sleep", _map=int, default=0),
         group_name=chained_get(response_dict, "status", "groupName"),
         group_volume=chained_get(response_dict, "status", "groupVolume", _map=int),
         indexing=chained_get(response_dict, "status", "indexing") == "1",
```

### Comparing `pyblu-0.3.2/src/pyblu/_player.py` & `pyblu-0.3.3/src/pyblu/_player.py`

 * *Files identical despite different names*

### Comparing `pyblu-0.3.2/PKG-INFO` & `pyblu-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyblu
-Version: 0.3.2
+Version: 0.3.3
 Summary: 
 Home-page: https://github.com/LouisChrist/pyblu
 License: MIT
 Author: Louis Christ
 Author-email: mail@louischrist.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

