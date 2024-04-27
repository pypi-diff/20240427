# Comparing `tmp/systembridgebackend-4.2.4.tar.gz` & `tmp/systembridgebackend-4.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgebackend-4.2.4.tar", last modified: Sun Apr 14 12:23:05 2024, max compression
+gzip compressed data, was "systembridgebackend-4.2.5.tar", last modified: Sat Apr 27 12:24:58 2024, max compression
```

## Comparing `systembridgebackend-4.2.4.tar` & `systembridgebackend-4.2.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:23:05.046157 systembridgebackend-4.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-14 12:23:05.046157 systembridgebackend-4.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 12:23:05.046157 systembridgebackend-4.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:23:05.038157 systembridgebackend-4.2.4/systembridgebackend/
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-14 12:23:02.000000 systembridgebackend-4.2.4/systembridgebackend/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:23:05.042158 systembridgebackend-4.2.4/systembridgebackend/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/keyboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:23:05.042158 systembridgebackend-4.2.4/systembridgebackend/handlers/media/
--rw-r--r--   0 runner    (1001) docker     (127)    16367 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/media/windows.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/open.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/power.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:23:05.042158 systembridgebackend-4.2.4/systembridgebackend/handlers/threads/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/threads/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/threads/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/threads/update.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:23:05.046157 systembridgebackend-4.2.4/systembridgebackend/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)    14935 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/disks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/displays.py
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/gpus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/listeners.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:23:05.046157 systembridgebackend-4.2.4/systembridgebackend/server/
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/server/mdns.py
--rw-r--r--   0 runner    (1001) docker     (127)    36941 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/server/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:23:05.046157 systembridgebackend-4.2.4/systembridgebackend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-14 12:23:04.000000 systembridgebackend-4.2.4/systembridgebackend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-14 12:23:05.000000 systembridgebackend-4.2.4/systembridgebackend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 12:23:04.000000 systembridgebackend-4.2.4/systembridgebackend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-14 12:23:04.000000 systembridgebackend-4.2.4/systembridgebackend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-14 12:23:04.000000 systembridgebackend-4.2.4/systembridgebackend.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:23:05.046157 systembridgebackend-4.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/tests/test__version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:24:58.048166 systembridgebackend-4.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-27 12:24:58.048166 systembridgebackend-4.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 12:24:58.048166 systembridgebackend-4.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:24:58.040166 systembridgebackend-4.2.5/systembridgebackend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-27 12:24:55.000000 systembridgebackend-4.2.5/systembridgebackend/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:24:58.044166 systembridgebackend-4.2.5/systembridgebackend/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/handlers/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/handlers/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/handlers/keyboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:24:58.044166 systembridgebackend-4.2.5/systembridgebackend/handlers/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    16367 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/handlers/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/handlers/media/windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/handlers/open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/handlers/power.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:24:58.044166 systembridgebackend-4.2.5/systembridgebackend/handlers/threads/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/handlers/threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/handlers/threads/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/handlers/threads/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/handlers/threads/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/handlers/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:24:58.048166 systembridgebackend-4.2.5/systembridgebackend/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/modules/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/modules/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15765 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/modules/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/modules/disks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/modules/displays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/modules/gpus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/modules/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/modules/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/modules/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/modules/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/modules/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/modules/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13629 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/modules/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:24:58.048166 systembridgebackend-4.2.5/systembridgebackend/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/server/mdns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36941 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/systembridgebackend/server/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:24:58.048166 systembridgebackend-4.2.5/systembridgebackend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-27 12:24:57.000000 systembridgebackend-4.2.5/systembridgebackend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-27 12:24:58.000000 systembridgebackend-4.2.5/systembridgebackend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 12:24:57.000000 systembridgebackend-4.2.5/systembridgebackend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-27 12:24:57.000000 systembridgebackend-4.2.5/systembridgebackend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-27 12:24:57.000000 systembridgebackend-4.2.5/systembridgebackend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:24:58.048166 systembridgebackend-4.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-27 12:24:17.000000 systembridgebackend-4.2.5/tests/test__version.py
```

### Comparing `systembridgebackend-4.2.4/LICENSE` & `systembridgebackend-4.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/PKG-INFO` & `systembridgebackend-4.2.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: systembridgebackend
-Version: 4.2.4
+Version: 4.2.5
 Summary: System Bridge Backend
 Home-page: https://github.com/timmo001/system-bridge-backend
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp>=3.9.0b0
-Requires-Dist: fastapi==0.110.1
+Requires-Dist: fastapi==0.110.2
 Requires-Dist: incremental==22.10.0
 Requires-Dist: keyboard==0.13.5
 Requires-Dist: mutagen==1.47.0
 Requires-Dist: packaging>=24.0
 Requires-Dist: plyer==2.1.0
 Requires-Dist: psutil==5.9.8
 Requires-Dist: python-multipart==0.0.9
 Requires-Dist: screeninfo==0.8.1
 Requires-Dist: systembridgeconnector==4.1.2
 Requires-Dist: systembridgemodels==4.1.0
 Requires-Dist: systembridgeshared==4.0.4
 Requires-Dist: typer==0.12.3
 Requires-Dist: uvicorn[standard]==0.29.0
-Requires-Dist: zeroconf==0.132.0
+Requires-Dist: zeroconf==0.132.2
 
 # System Bridge - Backend
 
 This is the backend package for the [System Bridge](https://github.com/timmo001/system-bridge) project.
```

### Comparing `systembridgebackend-4.2.4/pyproject.toml` & `systembridgebackend-4.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/setup.py` & `systembridgebackend-4.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/__init__.py` & `systembridgebackend-4.2.5/systembridgebackend/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/__main__.py` & `systembridgebackend-4.2.5/systembridgebackend/__main__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/handlers/action.py` & `systembridgebackend-4.2.5/systembridgebackend/handlers/action.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/handlers/data.py` & `systembridgebackend-4.2.5/systembridgebackend/handlers/data.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/handlers/keyboard.py` & `systembridgebackend-4.2.5/systembridgebackend/handlers/keyboard.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/handlers/media/__init__.py` & `systembridgebackend-4.2.5/systembridgebackend/handlers/media/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/handlers/media/windows.py` & `systembridgebackend-4.2.5/systembridgebackend/handlers/media/windows.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/handlers/power.py` & `systembridgebackend-4.2.5/systembridgebackend/handlers/power.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/handlers/threads/__init__.py` & `systembridgebackend-4.2.5/systembridgebackend/handlers/threads/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/handlers/threads/data.py` & `systembridgebackend-4.2.5/systembridgebackend/handlers/threads/data.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/handlers/threads/media.py` & `systembridgebackend-4.2.5/systembridgebackend/handlers/threads/media.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/handlers/threads/update.py` & `systembridgebackend-4.2.5/systembridgebackend/handlers/threads/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/modules/__init__.py` & `systembridgebackend-4.2.5/systembridgebackend/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/modules/battery.py` & `systembridgebackend-4.2.5/systembridgebackend/modules/battery.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/modules/cpu.py` & `systembridgebackend-4.2.5/systembridgebackend/modules/cpu.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,14 +146,30 @@
                             or "Core 0" in sensor
                         ):
                             self._logger.debug(
                                 "Found CPU temperature (coretemp): %s",
                                 sensor,
                             )
                             return sensor.current
+                if "atk0110" in self.sensors.temperatures:
+                    for sensor in self.sensors.temperatures["atk0110"]:
+                        self._logger.debug("atk0110: %s", sensor)
+                        if "CPU" in sensor:
+                            self._logger.debug(
+                                "Found CPU temperature (atk0110): %s",
+                                sensor,
+                            )
+                            return sensor.current
+                # Use the first temperature sensor key
+                for key in temperatures:
+                    for sensor in temperatures[key]:
+                        self._logger.warning(
+                            "Unknown sensor used (may not be correct): %s", sensor
+                        )
+                        return sensor.current
             if (
                 self.sensors.windows_sensors is not None
                 and self.sensors.windows_sensors.hardware is not None
             ):
                 for hardware in self.sensors.windows_sensors.hardware:
                     # Find type "CPU"
                     if "CPU" not in hardware.type.upper():
```

### Comparing `systembridgebackend-4.2.4/systembridgebackend/modules/disks.py` & `systembridgebackend-4.2.5/systembridgebackend/modules/disks.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/modules/displays.py` & `systembridgebackend-4.2.5/systembridgebackend/modules/displays.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/modules/gpus.py` & `systembridgebackend-4.2.5/systembridgebackend/modules/gpus.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/modules/listeners.py` & `systembridgebackend-4.2.5/systembridgebackend/modules/listeners.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/modules/media.py` & `systembridgebackend-4.2.5/systembridgebackend/modules/media.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/modules/memory.py` & `systembridgebackend-4.2.5/systembridgebackend/modules/memory.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/modules/networks.py` & `systembridgebackend-4.2.5/systembridgebackend/modules/networks.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/modules/processes.py` & `systembridgebackend-4.2.5/systembridgebackend/modules/processes.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/modules/sensors.py` & `systembridgebackend-4.2.5/systembridgebackend/modules/sensors.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/modules/system.py` & `systembridgebackend-4.2.5/systembridgebackend/modules/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,16 +157,15 @@
             sock.connect(("2001:4860:4860::8888", 80))
             return sock.getsockname()[0]
         except OSError:
             return ""
 
     def _get_mac_address(self) -> str:
         """Get MAC address."""
-        # pylint: disable=consider-using-f-string
-        return ":".join(re.findall("..", "%012x" % uuid.getnode()))
+        return ":".join(re.findall("..", f"{uuid.getnode():012x}"))
 
     async def _get_pending_reboot(self) -> bool:
         """Check if there is a pending reboot."""
         if sys.platform == "win32":
             # Read from registry for pending reboot
             import winreg  # pylint: disable=import-error,import-outside-toplevel
```

### Comparing `systembridgebackend-4.2.4/systembridgebackend/server/__init__.py` & `systembridgebackend-4.2.5/systembridgebackend/server/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/server/api.py` & `systembridgebackend-4.2.5/systembridgebackend/server/api.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/server/mdns.py` & `systembridgebackend-4.2.5/systembridgebackend/server/mdns.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend/server/websocket.py` & `systembridgebackend-4.2.5/systembridgebackend/server/websocket.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.4/systembridgebackend.egg-info/PKG-INFO` & `systembridgebackend-4.2.5/systembridgebackend.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: systembridgebackend
-Version: 4.2.4
+Version: 4.2.5
 Summary: System Bridge Backend
 Home-page: https://github.com/timmo001/system-bridge-backend
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp>=3.9.0b0
-Requires-Dist: fastapi==0.110.1
+Requires-Dist: fastapi==0.110.2
 Requires-Dist: incremental==22.10.0
 Requires-Dist: keyboard==0.13.5
 Requires-Dist: mutagen==1.47.0
 Requires-Dist: packaging>=24.0
 Requires-Dist: plyer==2.1.0
 Requires-Dist: psutil==5.9.8
 Requires-Dist: python-multipart==0.0.9
 Requires-Dist: screeninfo==0.8.1
 Requires-Dist: systembridgeconnector==4.1.2
 Requires-Dist: systembridgemodels==4.1.0
 Requires-Dist: systembridgeshared==4.0.4
 Requires-Dist: typer==0.12.3
 Requires-Dist: uvicorn[standard]==0.29.0
-Requires-Dist: zeroconf==0.132.0
+Requires-Dist: zeroconf==0.132.2
 
 # System Bridge - Backend
 
 This is the backend package for the [System Bridge](https://github.com/timmo001/system-bridge) project.
```

### Comparing `systembridgebackend-4.2.4/systembridgebackend.egg-info/SOURCES.txt` & `systembridgebackend-4.2.5/systembridgebackend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

