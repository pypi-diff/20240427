# Comparing `tmp/pyblu-0.3.5.tar.gz` & `tmp/pyblu-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyblu-0.3.5.tar", max compression
+gzip compressed data, was "pyblu-0.3.6.tar", max compression
```

## Comparing `pyblu-0.3.5.tar` & `pyblu-0.3.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2024-03-09 09:45:55.409568 pyblu-0.3.5/LICENSE
--rw-r--r--   0        0        0      873 2024-04-12 16:28:03.088001 pyblu-0.3.5/README.md
--rw-r--r--   0        0        0      921 2024-04-27 10:23:15.060754 pyblu-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      277 2024-04-14 21:03:17.059292 pyblu-0.3.5/src/pyblu/__init__.py
--rw-r--r--   0        0        0     4373 2024-04-27 10:19:51.746277 pyblu-0.3.5/src/pyblu/_entities.py
--rw-r--r--   0        0        0     6039 2024-04-27 09:57:31.749983 pyblu-0.3.5/src/pyblu/_parse.py
--rw-r--r--   0        0        0    14367 2024-04-20 09:50:30.350831 pyblu-0.3.5/src/pyblu/_player.py
--rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 pyblu-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-09 09:45:55.409568 pyblu-0.3.6/LICENSE
+-rw-r--r--   0        0        0      873 2024-04-12 16:28:03.088001 pyblu-0.3.6/README.md
+-rw-r--r--   0        0        0      921 2024-04-27 10:38:11.092700 pyblu-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      277 2024-04-14 21:03:17.059292 pyblu-0.3.6/src/pyblu/__init__.py
+-rw-r--r--   0        0        0     4605 2024-04-27 10:36:10.024239 pyblu-0.3.6/src/pyblu/_entities.py
+-rw-r--r--   0        0        0     6109 2024-04-27 10:36:10.043239 pyblu-0.3.6/src/pyblu/_parse.py
+-rw-r--r--   0        0        0    14367 2024-04-20 09:50:30.350831 pyblu-0.3.6/src/pyblu/_player.py
+-rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 pyblu-0.3.6/PKG-INFO
```

### Comparing `pyblu-0.3.5/LICENSE` & `pyblu-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyblu-0.3.5/README.md` & `pyblu-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pyblu-0.3.5/pyproject.toml` & `pyblu-0.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyblu"
-version = "0.3.5"
+version = "0.3.6"
 description = ""
 authors = ["Louis Christ <mail@louischrist.de>"]
 repository = "https://github.com/LouisChrist/pyblu"
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "pyblu", from = "src" },
```

### Comparing `pyblu-0.3.5/src/pyblu/_entities.py` & `pyblu-0.3.6/src/pyblu/_entities.py`

 * *Files 16% similar despite different names*

```diff
@@ -51,14 +51,18 @@
     """Name of the group the player is in. Only present on master."""
     group_volume: int | None
     """Volume level of the group. Only present on master. Range is 0-100."""
 
     indexing: bool
     """True if the player is currently indexing."""
 
+    stream_url: str | None
+    """The presence of this element should be treated as a flag and its contents as an opaque value. 
+    Seems to be present for radio stations and to be the same as the url from the matching preset."""
+
 
 @dataclass
 class PairedPlayer:
     ip: str
     """IP address of the player"""
     port: int
     """Port of the player"""
```

### Comparing `pyblu-0.3.5/src/pyblu/_parse.py` & `pyblu-0.3.6/src/pyblu/_parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
         seconds=chained_get(response_dict, "status", "secs", _map=int),
         total_seconds=chained_get(response_dict, "status", "totlen", _map=float),
         can_seek=chained_get(response_dict, "status", "canSeek") == "1",
         sleep=chained_get(response_dict, "status", "sleep", _map=int, default=0),
         group_name=chained_get(response_dict, "status", "groupName"),
         group_volume=chained_get(response_dict, "status", "groupVolume", _map=int),
         indexing=chained_get(response_dict, "status", "indexing") == "1",
+        stream_url=chained_get(response_dict, "status", "streamUrl"),
     )
 
     return status
 
 
 def parse_volume(response_dict: dict[str, Any]) -> Volume:
     volume = Volume(
```

### Comparing `pyblu-0.3.5/src/pyblu/_player.py` & `pyblu-0.3.6/src/pyblu/_player.py`

 * *Files identical despite different names*

### Comparing `pyblu-0.3.5/PKG-INFO` & `pyblu-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyblu
-Version: 0.3.5
+Version: 0.3.6
 Summary: 
 Home-page: https://github.com/LouisChrist/pyblu
 License: MIT
 Author: Louis Christ
 Author-email: mail@louischrist.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

