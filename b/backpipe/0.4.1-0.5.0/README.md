# Comparing `tmp/backpipe-0.4.1.tar.gz` & `tmp/backpipe-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backpipe-0.4.1.tar", last modified: Sun Apr 14 10:33:54 2024, max compression
+gzip compressed data, was "backpipe-0.5.0.tar", last modified: Sat Apr 27 10:38:53 2024, max compression
```

## Comparing `backpipe-0.4.1.tar` & `backpipe-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,60 @@
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-14 10:33:54.507292 backpipe-0.4.1/
--rw-r--r--   0 simon     (1000) simon     (1000)    35129 2023-11-04 20:14:40.000000 backpipe-0.4.1/LICENSE
--rw-r--r--   0 simon     (1000) simon     (1000)     3353 2024-04-14 10:33:54.507292 backpipe-0.4.1/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)     2700 2024-04-03 20:39:35.000000 backpipe-0.4.1/README.md
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-14 10:33:54.506292 backpipe-0.4.1/backpipe/
--rw-r--r--   0 simon     (1000) simon     (1000)      458 2024-04-14 10:27:00.000000 backpipe-0.4.1/backpipe/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     6194 2024-04-14 10:30:45.000000 backpipe-0.4.1/backpipe/__main__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     6095 2024-04-14 09:49:40.000000 backpipe-0.4.1/backpipe/app.py
--rw-r--r--   0 simon     (1000) simon     (1000)     3244 2024-03-30 02:36:58.000000 backpipe-0.4.1/backpipe/builder.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1257 2024-03-28 19:06:16.000000 backpipe-0.4.1/backpipe/config.py
--rw-r--r--   0 simon     (1000) simon     (1000)      364 2024-03-29 01:51:22.000000 backpipe-0.4.1/backpipe/defaults.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1916 2024-03-30 04:22:44.000000 backpipe-0.4.1/backpipe/host.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1233 2024-04-14 09:53:29.000000 backpipe-0.4.1/backpipe/rq.py
--rw-r--r--   0 simon     (1000) simon     (1000)     6476 2024-03-30 04:30:41.000000 backpipe-0.4.1/backpipe/server.py
--rw-r--r--   0 simon     (1000) simon     (1000)      137 2023-11-14 15:08:41.000000 backpipe-0.4.1/backpipe/uptime.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-14 10:33:54.507292 backpipe-0.4.1/backpipe.egg-info/
--rw-r--r--   0 simon     (1000) simon     (1000)     3353 2024-04-14 10:33:54.000000 backpipe-0.4.1/backpipe.egg-info/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)      408 2024-04-14 10:33:54.000000 backpipe-0.4.1/backpipe.egg-info/SOURCES.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        1 2024-04-14 10:33:54.000000 backpipe-0.4.1/backpipe.egg-info/dependency_links.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       52 2024-04-14 10:33:54.000000 backpipe-0.4.1/backpipe.egg-info/entry_points.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       19 2024-04-14 10:33:54.000000 backpipe-0.4.1/backpipe.egg-info/requires.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        9 2024-04-14 10:33:54.000000 backpipe-0.4.1/backpipe.egg-info/top_level.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       38 2024-04-14 10:33:54.507292 backpipe-0.4.1/setup.cfg
--rw-r--r--   0 simon     (1000) simon     (1000)     1277 2024-03-28 17:08:11.000000 backpipe-0.4.1/setup.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 10:38:53.645433 backpipe-0.5.0/
+-rw-r--r--   0 simon     (1000) simon     (1000)    35129 2023-11-04 20:14:40.000000 backpipe-0.5.0/LICENSE
+-rw-r--r--   0 simon     (1000) simon     (1000)      176 2024-04-22 18:38:17.000000 backpipe-0.5.0/MANIFEST.in
+-rw-r--r--   0 simon     (1000) simon     (1000)     3513 2024-04-27 10:38:53.645433 backpipe-0.5.0/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)     2860 2024-04-15 19:20:17.000000 backpipe-0.5.0/README.md
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 10:38:53.641433 backpipe-0.5.0/backpipe/
+-rw-r--r--   0 simon     (1000) simon     (1000)      490 2024-04-27 10:25:27.000000 backpipe-0.5.0/backpipe/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     5172 2024-04-26 15:29:12.000000 backpipe-0.5.0/backpipe/__main__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     6095 2024-04-14 09:49:40.000000 backpipe-0.5.0/backpipe/app.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     3244 2024-03-30 02:36:58.000000 backpipe-0.5.0/backpipe/builder.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1257 2024-03-28 19:06:16.000000 backpipe-0.5.0/backpipe/config.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      364 2024-03-29 01:51:22.000000 backpipe-0.5.0/backpipe/defaults.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1916 2024-03-30 04:22:44.000000 backpipe-0.5.0/backpipe/host.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 10:38:53.642433 backpipe-0.5.0/backpipe/presets/
+-rw-r--r--   0 simon     (1000) simon     (1000)      522 2024-04-26 19:42:58.000000 backpipe-0.5.0/backpipe/presets/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1434 2024-04-26 20:01:59.000000 backpipe-0.5.0/backpipe/presets/file.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      425 2024-04-26 19:39:30.000000 backpipe-0.5.0/backpipe/presets/ipaddr.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1233 2024-04-14 09:53:29.000000 backpipe-0.5.0/backpipe/rq.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     6476 2024-03-30 04:30:41.000000 backpipe-0.5.0/backpipe/server.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 10:38:53.642433 backpipe-0.5.0/backpipe/tools/
+-rw-r--r--   0 simon     (1000) simon     (1000)      178 2024-04-22 17:36:44.000000 backpipe-0.5.0/backpipe/tools/__init__.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 10:38:53.642433 backpipe-0.5.0/backpipe/tools/base64/
+-rw-r--r--   0 simon     (1000) simon     (1000)       95 2024-04-15 14:45:34.000000 backpipe-0.5.0/backpipe/tools/base64/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      177 2024-04-15 14:45:00.000000 backpipe-0.5.0/backpipe/tools/base64/decode.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      177 2024-04-15 14:43:40.000000 backpipe-0.5.0/backpipe/tools/base64/encode.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      398 2024-04-15 15:05:34.000000 backpipe-0.5.0/backpipe/tools/check_type.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 10:38:53.643433 backpipe-0.5.0/backpipe/tools/file/
+-rw-r--r--   0 simon     (1000) simon     (1000)      181 2024-04-22 17:06:34.000000 backpipe-0.5.0/backpipe/tools/file/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      464 2024-04-22 17:03:16.000000 backpipe-0.5.0/backpipe/tools/file/append.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      301 2024-04-22 16:26:18.000000 backpipe-0.5.0/backpipe/tools/file/create.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      388 2024-04-22 16:51:25.000000 backpipe-0.5.0/backpipe/tools/file/delete.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      463 2024-04-22 16:39:25.000000 backpipe-0.5.0/backpipe/tools/file/write.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 10:38:53.644433 backpipe-0.5.0/backpipe/tools/hash/
+-rw-r--r--   0 simon     (1000) simon     (1000)      265 2024-04-22 17:45:34.000000 backpipe-0.5.0/backpipe/tools/hash/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      284 2024-04-22 17:41:35.000000 backpipe-0.5.0/backpipe/tools/hash/md5.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      286 2024-04-22 17:41:54.000000 backpipe-0.5.0/backpipe/tools/hash/sha1.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:42:44.000000 backpipe-0.5.0/backpipe/tools/hash/sha224.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:42:57.000000 backpipe-0.5.0/backpipe/tools/hash/sha256.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:44:00.000000 backpipe-0.5.0/backpipe/tools/hash/sha384.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:44:07.000000 backpipe-0.5.0/backpipe/tools/hash/sha512.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 10:38:53.644433 backpipe-0.5.0/backpipe/tools/html/
+-rw-r--r--   0 simon     (1000) simon     (1000)       41 2024-04-14 18:21:28.000000 backpipe-0.5.0/backpipe/tools/html/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      212 2024-04-14 20:54:18.000000 backpipe-0.5.0/backpipe/tools/html/addMeta.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      130 2024-04-14 20:54:11.000000 backpipe-0.5.0/backpipe/tools/html/addStyle.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      346 2024-04-27 09:07:22.000000 backpipe-0.5.0/backpipe/tools/html/addTag.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1176 2024-04-27 09:10:21.000000 backpipe-0.5.0/backpipe/tools/html/html.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 10:38:53.645433 backpipe-0.5.0/backpipe/tools/json/
+-rw-r--r--   0 simon     (1000) simon     (1000)      107 2024-04-14 16:06:07.000000 backpipe-0.5.0/backpipe/tools/json/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      184 2024-04-15 14:42:14.000000 backpipe-0.5.0/backpipe/tools/json/deserialize.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      262 2024-04-15 14:42:48.000000 backpipe-0.5.0/backpipe/tools/json/serialize.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      137 2023-11-14 15:08:41.000000 backpipe-0.5.0/backpipe/uptime.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 10:38:53.642433 backpipe-0.5.0/backpipe.egg-info/
+-rw-r--r--   0 simon     (1000) simon     (1000)     3513 2024-04-27 10:38:53.000000 backpipe-0.5.0/backpipe.egg-info/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)     1266 2024-04-27 10:38:53.000000 backpipe-0.5.0/backpipe.egg-info/SOURCES.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)        1 2024-04-27 10:38:53.000000 backpipe-0.5.0/backpipe.egg-info/dependency_links.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       52 2024-04-27 10:38:53.000000 backpipe-0.5.0/backpipe.egg-info/entry_points.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       19 2024-04-27 10:38:53.000000 backpipe-0.5.0/backpipe.egg-info/requires.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)        9 2024-04-27 10:38:53.000000 backpipe-0.5.0/backpipe.egg-info/top_level.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       38 2024-04-27 10:38:53.645433 backpipe-0.5.0/setup.cfg
+-rw-r--r--   0 simon     (1000) simon     (1000)     1532 2024-04-26 16:49:47.000000 backpipe-0.5.0/setup.py
```

### Comparing `backpipe-0.4.1/LICENSE` & `backpipe-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `backpipe-0.4.1/PKG-INFO` & `backpipe-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backpipe
-Version: 0.4.1
+Version: 0.5.0
 Summary: A backend HTTP framework for Python.
 Home-page: https://github.com/Simoso68/backpipe
 Author: Simoso68
 Maintainer: Simoso68
 License: GNU GPL v3
 Keywords: framework,http,web,api,server
 Classifier: Development Status :: 4 - Beta
@@ -25,18 +25,17 @@
 <img src="https://img.shields.io/pypi/v/backpipe?color=blue">
 <img src='https://static.pepy.tech/badge/backpipe'>
 <img src="https://img.shields.io/pypi/l/backpipe?color=yellow">
 <img src="https://img.shields.io/github/repo-size/Simoso68/backpipe?color=green">
 <img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.github.com%2Frepos%2FSimoso68%2Fbackpipe%2Flanguages&query=Python&label=characters&color=green">
 
 <br>
+<pre><code>pip install backpipe</code></pre>
 </div>
 
-<div align=center><pre><code>pip install backpipe</code></pre></div>
-
 ## Info
 
 Backpipe tries to support all operating systems. \
 But its primary focus lies on Linux support, \
 as it is the main choice for website hosting. \
 \
 Running it on Windows might lead to issues and is not recommended.
@@ -129,10 +128,15 @@
 When activating HTTPS, you need to sign your certificate file \
 with a key provided by a trusted authority. \
 \
 Self-signing your certificate will make tools such as \
 CURL, your Browser, etc. raise a warning, \
 that the website may be unsafe.
 
+## Documentation for dummies
+
+Read through the [Documentation for Dummies](https://github.com/Simoso68/backpipe/blob/main/DOCUMENTATION_FOR_DUMMIES.md), \
+to get started with backpipe
+
 ## License
 
 Backpipe is licensed under the GNU GPL v3.
```

### Comparing `backpipe-0.4.1/README.md` & `backpipe-0.5.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -6,18 +6,17 @@
 <img src="https://img.shields.io/pypi/v/backpipe?color=blue">
 <img src='https://static.pepy.tech/badge/backpipe'>
 <img src="https://img.shields.io/pypi/l/backpipe?color=yellow">
 <img src="https://img.shields.io/github/repo-size/Simoso68/backpipe?color=green">
 <img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.github.com%2Frepos%2FSimoso68%2Fbackpipe%2Flanguages&query=Python&label=characters&color=green">
 
 <br>
+<pre><code>pip install backpipe</code></pre>
 </div>
 
-<div align=center><pre><code>pip install backpipe</code></pre></div>
-
 ## Info
 
 Backpipe tries to support all operating systems. \
 But its primary focus lies on Linux support, \
 as it is the main choice for website hosting. \
 \
 Running it on Windows might lead to issues and is not recommended.
@@ -110,10 +109,15 @@
 When activating HTTPS, you need to sign your certificate file \
 with a key provided by a trusted authority. \
 \
 Self-signing your certificate will make tools such as \
 CURL, your Browser, etc. raise a warning, \
 that the website may be unsafe.
 
+## Documentation for dummies
+
+Read through the [Documentation for Dummies](https://github.com/Simoso68/backpipe/blob/main/DOCUMENTATION_FOR_DUMMIES.md), \
+to get started with backpipe
+
 ## License
 
 Backpipe is licensed under the GNU GPL v3.
```

### Comparing `backpipe-0.4.1/backpipe/__main__.py` & `backpipe-0.5.0/backpipe/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from sys import argv, exit
 from os import mkdir, path
 from subprocess import run
 from json import loads
 from packaging.version import Version
 
 from backpipe import __version__
+from backpipe.presets import PRESET_MNGR
 
 init()
 
 def info(msg):
     print(f"{Back.LIGHTGREEN_EX}{Fore.BLACK} INFO {Back.RESET}{Fore.RESET} {msg}")
 
 def err(msg, t="ERROR"):
@@ -19,89 +20,51 @@
 
 def warn(msg):
     print(f"{Back.LIGHTYELLOW_EX}{Fore.BLACK} WARN {Back.RESET}{Fore.RESET} {msg}")
 
 def crash(exc):
     print(f"\r{Back.LIGHTRED_EX}{Fore.BLACK} CRASH {Back.RESET}{Fore.RESET} {Fore.BLUE}{type(exc).__name__}{Fore.RESET}: {Fore.LIGHTBLUE_EX}{exc}{Fore.RESET}")
 
-def file_hoster(addr, port):
-    # Give Root/Admin Permissions for full access
-    # This script uses newer F-String features provided by Python 3.12
-
-    import backpipe
-    import os
-    import platform
-    import urllib
-
-    server = backpipe.BackPipe(addr, port)
-
-    @server.get
-    def respond(r: backpipe.Request):
-        try: 
-            if platform.system() == "Windows":
-                PATH = urllib.parse.unquote(f"C:{r.path}")
-            else:
-                PATH = urllib.parse.unquote(r.path)
-
-            if not os.path.exists(PATH):
-                return (404, "File not found.")
-    
-            if os.path.isdir(PATH):
-                HTML = "<!DOCTYPE html>\n"
-
-                if r.path == "/":
-                    CURRENT_DIR = r.path[:-1]
-                else:
-                    CURRENT_DIR = r.path
-
-                for o in os.listdir(PATH):
-                    HTML += f"<a href='{CURRENT_DIR + f"/{o}"}'>{o}</a><br>"
-                return (200, HTML)
-            else:
-                return (200, open(PATH, "rb").read())
-        except PermissionError:
-            return (403, "Can not access object")
-    
-    server.run()
-
 def main():
     if "-v" in argv[1:] or "--version" in argv[1:]:
         print(f"BackPipe {__version__}")
         exit()
 
     elif "-h" in argv[1:] or "--help" in argv[1:]:
         print("""BackPipe Help
 backpipe -h / --help        This message.
 backpipe -v / --version     Display the current version of backpipe.
 backpipe new                BackPipe project template.
 backpipe exec               Executes your BackPipe project.
-backpipe update             Update backpipe using pip.""")
+backpipe update             Update backpipe using pip.
+backpipe host               Host a preset server.""")
         exit()
     
     elif "host" in argv[1:]:
         print("Available presets: ")
-        for preset in ("file",): # More will be added soon
+        for preset in PRESET_MNGR.listPresets():
             print(f"- {preset}")
         TYPE = input("What server preset do you want to host?: ")
-        if TYPE == "file":
-            SERVER = file_hoster
+        if TYPE in PRESET_MNGR.listPresets():
+            info("preset found")
         else:
             err("preset does not exist", "UNKNOWN")
             return
         
         ADDR = input("server address (leave empty for default): ")
         PORT = input("server port: ")
 
         try:
             int(PORT)
         except ValueError:
             err("port must be a number")
+            return
 
         try:
-            SERVER(ADDR, int(PORT))
+            PRESET_MNGR.execPreset(TYPE, ADDR, int(PORT))
             return
         except Exception as server_exc:
             crash(server_exc)
             return
 
     elif "new" in argv[1:]:
         try:
```

### Comparing `backpipe-0.4.1/backpipe/app.py` & `backpipe-0.5.0/backpipe/app.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.4.1/backpipe/builder.py` & `backpipe-0.5.0/backpipe/builder.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.4.1/backpipe/config.py` & `backpipe-0.5.0/backpipe/config.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.4.1/backpipe/host.py` & `backpipe-0.5.0/backpipe/host.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.4.1/backpipe/rq.py` & `backpipe-0.5.0/backpipe/rq.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.4.1/backpipe/server.py` & `backpipe-0.5.0/backpipe/server.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.4.1/backpipe.egg-info/PKG-INFO` & `backpipe-0.5.0/backpipe.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backpipe
-Version: 0.4.1
+Version: 0.5.0
 Summary: A backend HTTP framework for Python.
 Home-page: https://github.com/Simoso68/backpipe
 Author: Simoso68
 Maintainer: Simoso68
 License: GNU GPL v3
 Keywords: framework,http,web,api,server
 Classifier: Development Status :: 4 - Beta
@@ -25,18 +25,17 @@
 <img src="https://img.shields.io/pypi/v/backpipe?color=blue">
 <img src='https://static.pepy.tech/badge/backpipe'>
 <img src="https://img.shields.io/pypi/l/backpipe?color=yellow">
 <img src="https://img.shields.io/github/repo-size/Simoso68/backpipe?color=green">
 <img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.github.com%2Frepos%2FSimoso68%2Fbackpipe%2Flanguages&query=Python&label=characters&color=green">
 
 <br>
+<pre><code>pip install backpipe</code></pre>
 </div>
 
-<div align=center><pre><code>pip install backpipe</code></pre></div>
-
 ## Info
 
 Backpipe tries to support all operating systems. \
 But its primary focus lies on Linux support, \
 as it is the main choice for website hosting. \
 \
 Running it on Windows might lead to issues and is not recommended.
@@ -129,10 +128,15 @@
 When activating HTTPS, you need to sign your certificate file \
 with a key provided by a trusted authority. \
 \
 Self-signing your certificate will make tools such as \
 CURL, your Browser, etc. raise a warning, \
 that the website may be unsafe.
 
+## Documentation for dummies
+
+Read through the [Documentation for Dummies](https://github.com/Simoso68/backpipe/blob/main/DOCUMENTATION_FOR_DUMMIES.md), \
+to get started with backpipe
+
 ## License
 
 Backpipe is licensed under the GNU GPL v3.
```

