# Comparing `tmp/toggl-track-0.5.0.tar.gz` & `tmp/toggl_track-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toggl-track-0.5.0.tar", last modified: Mon Apr 17 22:49:47 2023, max compression
+gzip compressed data, was "toggl_track-0.5.1.tar", last modified: Sat Apr 27 05:29:14 2024, max compression
```

## Comparing `toggl-track-0.5.0.tar` & `toggl_track-0.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:49:47.029955 toggl-track-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 22:49:27.000000 toggl-track-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-04-17 22:49:47.029955 toggl-track-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-04-17 22:49:27.000000 toggl-track-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 22:49:47.029955 toggl-track-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-17 22:49:27.000000 toggl-track-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:49:47.025954 toggl-track-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-04-17 22:49:27.000000 toggl-track-0.5.0/tests/test_entries_group_by.py
--rw-r--r--   0 runner    (1001) docker     (123)    19564 2023-04-17 22:49:27.000000 toggl-track-0.5.0/tests/test_entries_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-17 22:49:27.000000 toggl-track-0.5.0/tests/test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-17 22:49:27.000000 toggl-track-0.5.0/tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:49:47.029955 toggl-track-0.5.0/toggl_track/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:49:27.000000 toggl-track-0.5.0/toggl_track/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-17 22:49:27.000000 toggl-track-0.5.0/toggl_track/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-17 22:49:27.000000 toggl-track-0.5.0/toggl_track/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-04-17 22:49:27.000000 toggl-track-0.5.0/toggl_track/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-17 22:49:27.000000 toggl-track-0.5.0/toggl_track/toggl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:49:47.029955 toggl-track-0.5.0/toggl_track.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-04-17 22:49:47.000000 toggl-track-0.5.0/toggl_track.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-17 22:49:47.000000 toggl-track-0.5.0/toggl_track.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 22:49:47.000000 toggl-track-0.5.0/toggl_track.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-17 22:49:47.000000 toggl-track-0.5.0/toggl_track.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-17 22:49:47.000000 toggl-track-0.5.0/toggl_track.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 22:49:47.000000 toggl-track-0.5.0/toggl_track.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 05:29:14.731431 toggl_track-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-27 05:29:06.000000 toggl_track-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11541 2024-04-27 05:29:14.731431 toggl_track-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-04-27 05:29:06.000000 toggl_track-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 05:29:14.731431 toggl_track-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-27 05:29:06.000000 toggl_track-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 05:29:14.727431 toggl_track-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-27 05:29:06.000000 toggl_track-0.5.1/tests/test_entries_group_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-04-27 05:29:06.000000 toggl_track-0.5.1/tests/test_entries_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-04-27 05:29:06.000000 toggl_track-0.5.1/tests/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-27 05:29:06.000000 toggl_track-0.5.1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 05:29:14.727431 toggl_track-0.5.1/toggl_track/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 05:29:06.000000 toggl_track-0.5.1/toggl_track/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-27 05:29:06.000000 toggl_track-0.5.1/toggl_track/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-27 05:29:06.000000 toggl_track-0.5.1/toggl_track/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-27 05:29:06.000000 toggl_track-0.5.1/toggl_track/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-27 05:29:06.000000 toggl_track-0.5.1/toggl_track/toggl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 05:29:14.731431 toggl_track-0.5.1/toggl_track.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11541 2024-04-27 05:29:14.000000 toggl_track-0.5.1/toggl_track.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-27 05:29:14.000000 toggl_track-0.5.1/toggl_track.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 05:29:14.000000 toggl_track-0.5.1/toggl_track.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-27 05:29:14.000000 toggl_track-0.5.1/toggl_track.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-27 05:29:14.000000 toggl_track-0.5.1/toggl_track.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-27 05:29:14.000000 toggl_track-0.5.1/toggl_track.egg-info/top_level.txt
```

### Comparing `toggl-track-0.5.0/LICENSE` & `toggl_track-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `toggl-track-0.5.0/PKG-INFO` & `toggl_track-0.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: toggl-track
-Version: 0.5.0
+Version: 0.5.1
 Summary: CLI tool and Python library to access Toggl Track https://toggl.com/track/
 Home-page: https://github.com/zmoog/toggl-track
 Author: Maurizio Branca
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/zmoog/toggl-track/issues
 Project-URL: CI, https://github.com/zmoog/toggl-track/actions
 Project-URL: Changelog, https://github.com/zmoog/toggl-track/releases
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: click==8.1.7
+Requires-Dist: pydantic<2
+Requires-Dist: requests==2.31.0
+Requires-Dist: rich==13.7.1
+Provides-Extra: test
+Requires-Dist: pytest==7.4.4; extra == "test"
+Requires-Dist: pytest-recording==0.13.1; extra == "test"
 
 # toggl-track
 
 [![PyPI](https://img.shields.io/pypi/v/toggl-track.svg)](https://pypi.org/project/toggl-track/)
 [![Changelog](https://img.shields.io/github/v/release/zmoog/toggl-track?include_prereleases&label=changelog)](https://github.com/zmoog/toggl-track/releases)
 [![Tests](https://github.com/zmoog/toggl-track/workflows/Test/badge.svg)](https://github.com/zmoog/toggl-track/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/zmoog/toggl-track/blob/master/LICENSE)
```

### Comparing `toggl-track-0.5.0/README.md` & `toggl_track-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `toggl-track-0.5.0/setup.py` & `toggl_track-0.5.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.5.0"
+VERSION = "0.5.1"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
@@ -28,20 +28,20 @@
     version=VERSION,
     packages=["toggl_track"],
     entry_points="""
         [console_scripts]
         tgl=toggl_track.cli:cli
     """,
     install_requires=[
-        "click",
-        "pydantic",
-        "requests",
-        "rich",
+        "click == 8.1.7",
+        "pydantic < 2",
+        "requests == 2.31.0",
+        "rich == 13.7.1",
         ],
     extras_require={
         "test": [
-            "pytest",
-            "pytest-recording",
+            "pytest == 7.4.4",
+            "pytest-recording == 0.13.1",
             ]
     },
     python_requires=">=3.7",
 )
```

### Comparing `toggl-track-0.5.0/tests/test_result.py` & `toggl_track-0.5.1/tests/test_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def test_empty_timeentrieslistresult_as_str():
     entries = []
     result = TimeEntriesListResult(entries)
 
     assert str(result) == "No time entries found."
 
 
-def test_empty_timeentrieslistresult_as_str(save_to_tmp):
+def test_timeentrieslistresult_as_str(save_to_tmp):
     entries = [TimeEntry(
         id=1,
         workspace_id=1,
         user_id=1,
         project_id=1,
         task_id=None,
         billable=False,
@@ -37,15 +37,15 @@
   2021-01-25   community:    11:04 PM   11:27 PM   0:22       type:support  
  ────────────────────────────────────────────────────────────────────────── 
                                         Total      0:22                     
                                                                             
 """
 
 
-def test_empty_timeentrieslistresult_as_json(save_to_tmp):
+def test_timeentrieslistresult_as_json(save_to_tmp):
     entries = [TimeEntry(
         id=1,
         workspace_id=1,
         user_id=1,
         project_id=1,
         task_id=None,
         billable=False,
@@ -60,15 +60,15 @@
 
     json_result = result.json()
     save_to_tmp(json_result, "test_empty_timeentrieslistresult_as_json")
 
     assert json_result == """[{"id": 1, "workspace_id": 1, "user_id": 1, "project_id": 1, "task_id": null, "billable": false, "at": "2021-01-25T00:00:00", "description": "community:", "start": "2021-01-25T23:04:00", "stop": "2021-01-25T23:27:00", "duration": 1379, "tags": ["type:support"]}]"""
 
 
-def test_empty_timeentrieslistresult_as_json_with_root(save_to_tmp):
+def test_timeentrieslistresult_as_json_with_root(save_to_tmp):
     entries = [TimeEntry(
         id=1,
         workspace_id=1,
         user_id=1,
         project_id=1,
         task_id=None,
         billable=False,
```

### Comparing `toggl-track-0.5.0/toggl_track/cli.py` & `toggl_track-0.5.1/toggl_track/cli.py`

 * *Files identical despite different names*

### Comparing `toggl-track-0.5.0/toggl_track/result.py` & `toggl_track-0.5.1/toggl_track/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import io
 import json
-import datetime as dt
 from itertools import groupby
 from typing import Any, Iterator, List
 
 from pydantic.json import pydantic_encoder
 from rich import box
 from rich.console import Console
 from rich.table import Table
```

### Comparing `toggl-track-0.5.0/toggl_track/toggl.py` & `toggl_track-0.5.1/toggl_track/toggl.py`

 * *Files identical despite different names*

### Comparing `toggl-track-0.5.0/toggl_track.egg-info/PKG-INFO` & `toggl_track-0.5.1/toggl_track.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: toggl-track
-Version: 0.5.0
+Version: 0.5.1
 Summary: CLI tool and Python library to access Toggl Track https://toggl.com/track/
 Home-page: https://github.com/zmoog/toggl-track
 Author: Maurizio Branca
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/zmoog/toggl-track/issues
 Project-URL: CI, https://github.com/zmoog/toggl-track/actions
 Project-URL: Changelog, https://github.com/zmoog/toggl-track/releases
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: click==8.1.7
+Requires-Dist: pydantic<2
+Requires-Dist: requests==2.31.0
+Requires-Dist: rich==13.7.1
+Provides-Extra: test
+Requires-Dist: pytest==7.4.4; extra == "test"
+Requires-Dist: pytest-recording==0.13.1; extra == "test"
 
 # toggl-track
 
 [![PyPI](https://img.shields.io/pypi/v/toggl-track.svg)](https://pypi.org/project/toggl-track/)
 [![Changelog](https://img.shields.io/github/v/release/zmoog/toggl-track?include_prereleases&label=changelog)](https://github.com/zmoog/toggl-track/releases)
 [![Tests](https://github.com/zmoog/toggl-track/workflows/Test/badge.svg)](https://github.com/zmoog/toggl-track/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/zmoog/toggl-track/blob/master/LICENSE)
```

