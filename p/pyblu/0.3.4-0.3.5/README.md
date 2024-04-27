# Comparing `tmp/pyblu-0.3.4.tar.gz` & `tmp/pyblu-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyblu-0.3.4.tar", max compression
+gzip compressed data, was "pyblu-0.3.5.tar", max compression
```

## Comparing `pyblu-0.3.4.tar` & `pyblu-0.3.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2024-03-09 09:45:55.409568 pyblu-0.3.4/LICENSE
--rw-r--r--   0        0        0      873 2024-04-12 16:28:03.088001 pyblu-0.3.4/README.md
--rw-r--r--   0        0        0      921 2024-04-27 09:57:54.150415 pyblu-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      277 2024-04-14 21:03:17.059292 pyblu-0.3.4/src/pyblu/__init__.py
--rw-r--r--   0        0        0     4338 2024-04-27 09:57:31.717983 pyblu-0.3.4/src/pyblu/_entities.py
--rw-r--r--   0        0        0     6039 2024-04-27 09:57:31.749983 pyblu-0.3.4/src/pyblu/_parse.py
--rw-r--r--   0        0        0    14367 2024-04-20 09:50:30.350831 pyblu-0.3.4/src/pyblu/_player.py
--rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 pyblu-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-09 09:45:55.409568 pyblu-0.3.5/LICENSE
+-rw-r--r--   0        0        0      873 2024-04-12 16:28:03.088001 pyblu-0.3.5/README.md
+-rw-r--r--   0        0        0      921 2024-04-27 10:23:15.060754 pyblu-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      277 2024-04-14 21:03:17.059292 pyblu-0.3.5/src/pyblu/__init__.py
+-rw-r--r--   0        0        0     4373 2024-04-27 10:19:51.746277 pyblu-0.3.5/src/pyblu/_entities.py
+-rw-r--r--   0        0        0     6039 2024-04-27 09:57:31.749983 pyblu-0.3.5/src/pyblu/_parse.py
+-rw-r--r--   0        0        0    14367 2024-04-20 09:50:30.350831 pyblu-0.3.5/src/pyblu/_player.py
+-rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 pyblu-0.3.5/PKG-INFO
```

### Comparing `pyblu-0.3.4/LICENSE` & `pyblu-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyblu-0.3.4/README.md` & `pyblu-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pyblu-0.3.4/pyproject.toml` & `pyblu-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyblu"
-version = "0.3.4"
+version = "0.3.5"
 description = ""
 authors = ["Louis Christ <mail@louischrist.de>"]
 repository = "https://github.com/LouisChrist/pyblu"
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "pyblu", from = "src" },
```

### Comparing `pyblu-0.3.4/src/pyblu/_entities.py` & `pyblu-0.3.5/src/pyblu/_entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 @dataclass
 class Status:
     etag: str
     """Cursor for long polling requests. Can be passed to next status call."""
 
     input_id: str | None
     """Unique id of the input. Is not set for radio."""
-    service: str
+    service: str | None
     """Service id of current input. 'Capture' for regular inputs."""
 
     state: str
     """Playback state"""
     shuffle: bool
     """Shuffle enabled"""
 
-    album: str
+    album: str | None
     """Album name"""
-    artist: str
+    artist: str | None
     """Artist name"""
-    name: str
+    name: str | None
     """Track name"""
-    image: str
+    image: str | None
     """URL of the album art"""
 
     volume: int
     """Volume level with a range of 0-100"""
     volume_db: float
     """Volume level in dB"""
```

### Comparing `pyblu-0.3.4/src/pyblu/_parse.py` & `pyblu-0.3.5/src/pyblu/_parse.py`

 * *Files identical despite different names*

### Comparing `pyblu-0.3.4/src/pyblu/_player.py` & `pyblu-0.3.5/src/pyblu/_player.py`

 * *Files identical despite different names*

### Comparing `pyblu-0.3.4/PKG-INFO` & `pyblu-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyblu
-Version: 0.3.4
+Version: 0.3.5
 Summary: 
 Home-page: https://github.com/LouisChrist/pyblu
 License: MIT
 Author: Louis Christ
 Author-email: mail@louischrist.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

