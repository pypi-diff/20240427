# Comparing `tmp/hosted-flasks-0.0.3.tar.gz` & `tmp/hosted-flasks-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hosted-flasks-0.0.3.tar", last modified: Sat Apr 27 13:33:20 2024, max compression
+gzip compressed data, was "hosted-flasks-0.0.4.tar", last modified: Sat Apr 27 14:07:38 2024, max compression
```

## Comparing `hosted-flasks-0.0.3.tar` & `hosted-flasks-0.0.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 13:33:20.153212 hosted-flasks-0.0.3/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 13:33:20.149667 hosted-flasks-0.0.3/.github/
--rw-r--r--   0 xtof       (501) staff       (20)     1033 2024-03-13 07:52:10.000000 hosted-flasks-0.0.3/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)     1057 2024-03-13 07:52:10.000000 hosted-flasks-0.0.3/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)      121 2024-04-27 13:30:32.000000 hosted-flasks-0.0.3/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-04-27 13:33:20.153107 hosted-flasks-0.0.3/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 13:33:20.149871 hosted-flasks-0.0.3/docs/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.3/docs/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1149 2024-03-13 07:52:10.000000 hosted-flasks-0.0.3/docs/conf.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 13:33:20.150414 hosted-flasks-0.0.3/hosted_flasks/
--rw-r--r--   0 xtof       (501) staff       (20)       22 2024-04-27 13:31:32.000000 hosted-flasks-0.0.3/hosted_flasks/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      686 2024-04-27 09:34:49.000000 hosted-flasks-0.0.3/hosted_flasks/__main__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 13:33:20.151189 hosted-flasks-0.0.3/hosted_flasks/frontpage/
--rw-r--r--   0 xtof       (501) staff       (20)     1462 2024-04-27 13:00:36.000000 hosted-flasks-0.0.3/hosted_flasks/frontpage/index.html
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 13:33:20.152200 hosted-flasks-0.0.3/hosted_flasks/frontpage/static/
--rw-rw-r--   0 xtof       (501) staff       (20)    17742 2024-04-27 08:53:20.000000 hosted-flasks-0.0.3/hosted_flasks/frontpage/static/android-chrome-192x192.png
--rw-rw-r--   0 xtof       (501) staff       (20)    53448 2024-04-27 08:53:20.000000 hosted-flasks-0.0.3/hosted_flasks/frontpage/static/android-chrome-512x512.png
--rw-rw-r--   0 xtof       (501) staff       (20)    15929 2024-04-27 08:53:20.000000 hosted-flasks-0.0.3/hosted_flasks/frontpage/static/apple-touch-icon.png
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 13:33:20.152434 hosted-flasks-0.0.3/hosted_flasks/frontpage/static/css/
--rw-r--r--   0 xtof       (501) staff       (20)     5011 2023-12-06 14:26:46.000000 hosted-flasks-0.0.3/hosted_flasks/frontpage/static/css/default.css
--rw-r--r--   0 xtof       (501) staff       (20)     1216 2024-04-27 13:14:19.000000 hosted-flasks-0.0.3/hosted_flasks/frontpage/static/css/style.css
--rw-rw-r--   0 xtof       (501) staff       (20)      821 2024-04-27 08:53:20.000000 hosted-flasks-0.0.3/hosted_flasks/frontpage/static/favicon-16x16.png
--rw-rw-r--   0 xtof       (501) staff       (20)     1907 2024-04-27 08:53:20.000000 hosted-flasks-0.0.3/hosted_flasks/frontpage/static/favicon-32x32.png
--rw-rw-r--   0 xtof       (501) staff       (20)    15406 2024-04-27 08:53:20.000000 hosted-flasks-0.0.3/hosted_flasks/frontpage/static/favicon.ico
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 13:33:20.152624 hosted-flasks-0.0.3/hosted_flasks/frontpage/static/img/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-12-06 14:26:46.000000 hosted-flasks-0.0.3/hosted_flasks/frontpage/static/img/.gitkeep
--rw-r--r--   0 xtof       (501) staff       (20)    20142 2024-04-27 12:20:37.000000 hosted-flasks-0.0.3/hosted_flasks/frontpage/static/img/logo.svg
--rw-r--r--   0 xtof       (501) staff       (20)       78 2023-12-06 14:26:46.000000 hosted-flasks-0.0.3/hosted_flasks/frontpage/static/robots.txt
--rw-rw-r--   0 xtof       (501) staff       (20)      359 2024-04-27 13:15:48.000000 hosted-flasks-0.0.3/hosted_flasks/frontpage/static/site.webmanifest
--rw-r--r--   0 xtof       (501) staff       (20)      859 2024-04-27 13:12:57.000000 hosted-flasks-0.0.3/hosted_flasks/frontpage.py
--rw-r--r--   0 xtof       (501) staff       (20)     1562 2024-04-27 09:44:37.000000 hosted-flasks-0.0.3/hosted_flasks/scanner.py
--rw-r--r--   0 xtof       (501) staff       (20)      796 2024-04-27 13:00:13.000000 hosted-flasks-0.0.3/hosted_flasks/server.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 13:33:20.151072 hosted-flasks-0.0.3/hosted_flasks.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-04-27 13:33:20.000000 hosted-flasks-0.0.3/hosted_flasks.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)     1107 2024-04-27 13:33:20.000000 hosted-flasks-0.0.3/hosted_flasks.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2024-04-27 13:33:20.000000 hosted-flasks-0.0.3/hosted_flasks.egg-info/dependency_links.txt
--rw-r--r--   0 xtof       (501) staff       (20)       62 2024-04-27 13:33:20.000000 hosted-flasks-0.0.3/hosted_flasks.egg-info/entry_points.txt
--rw-r--r--   0 xtof       (501) staff       (20)       20 2024-04-27 13:33:20.000000 hosted-flasks-0.0.3/hosted_flasks.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)       25 2024-04-27 13:33:20.000000 hosted-flasks-0.0.3/hosted_flasks.egg-info/top_level.txt
--rw-r--r--   0 xtof       (501) staff       (20)       38 2024-04-27 13:33:20.153258 hosted-flasks-0.0.3/setup.cfg
--rw-r--r--   0 xtof       (501) staff       (20)     1613 2024-04-27 08:20:07.000000 hosted-flasks-0.0.3/setup.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 13:33:20.152943 hosted-flasks-0.0.3/tests/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.3/tests/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      651 2024-04-25 19:07:50.000000 hosted-flasks-0.0.3/tests/test_config.py
--rw-r--r--   0 xtof       (501) staff       (20)     1440 2024-04-27 09:44:49.000000 hosted-flasks-0.0.3/tests/test_scanner.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 14:07:38.036513 hosted-flasks-0.0.4/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 14:07:38.032906 hosted-flasks-0.0.4/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)     1033 2024-03-13 07:52:10.000000 hosted-flasks-0.0.4/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1057 2024-03-13 07:52:10.000000 hosted-flasks-0.0.4/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)      121 2024-04-27 13:30:32.000000 hosted-flasks-0.0.4/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-04-27 14:07:38.036401 hosted-flasks-0.0.4/PKG-INFO
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 14:07:38.033104 hosted-flasks-0.0.4/docs/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.4/docs/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1149 2024-03-13 07:52:10.000000 hosted-flasks-0.0.4/docs/conf.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 14:07:38.033660 hosted-flasks-0.0.4/hosted_flasks/
+-rw-r--r--   0 xtof       (501) staff       (20)       22 2024-04-27 14:06:27.000000 hosted-flasks-0.0.4/hosted_flasks/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      686 2024-04-27 09:34:49.000000 hosted-flasks-0.0.4/hosted_flasks/__main__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 14:07:38.034467 hosted-flasks-0.0.4/hosted_flasks/frontpage/
+-rw-r--r--   0 xtof       (501) staff       (20)     1462 2024-04-27 13:00:36.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/index.html
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 14:07:38.035489 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/
+-rw-rw-r--   0 xtof       (501) staff       (20)    17742 2024-04-27 08:53:20.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/android-chrome-192x192.png
+-rw-rw-r--   0 xtof       (501) staff       (20)    53448 2024-04-27 08:53:20.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/android-chrome-512x512.png
+-rw-rw-r--   0 xtof       (501) staff       (20)    15929 2024-04-27 08:53:20.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/apple-touch-icon.png
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 14:07:38.035731 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/css/
+-rw-r--r--   0 xtof       (501) staff       (20)     5011 2023-12-06 14:26:46.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/css/default.css
+-rw-r--r--   0 xtof       (501) staff       (20)     1216 2024-04-27 13:14:19.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/css/style.css
+-rw-rw-r--   0 xtof       (501) staff       (20)      821 2024-04-27 08:53:20.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/favicon-16x16.png
+-rw-rw-r--   0 xtof       (501) staff       (20)     1907 2024-04-27 08:53:20.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/favicon-32x32.png
+-rw-rw-r--   0 xtof       (501) staff       (20)    15406 2024-04-27 08:53:20.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/favicon.ico
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 14:07:38.035921 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/img/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-12-06 14:26:46.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/img/.gitkeep
+-rw-r--r--   0 xtof       (501) staff       (20)    20142 2024-04-27 12:20:37.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/img/logo.svg
+-rw-r--r--   0 xtof       (501) staff       (20)       78 2023-12-06 14:26:46.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/robots.txt
+-rw-rw-r--   0 xtof       (501) staff       (20)      359 2024-04-27 13:15:48.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/site.webmanifest
+-rw-r--r--   0 xtof       (501) staff       (20)      859 2024-04-27 13:12:57.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1696 2024-04-27 14:05:39.000000 hosted-flasks-0.0.4/hosted_flasks/scanner.py
+-rw-r--r--   0 xtof       (501) staff       (20)      796 2024-04-27 14:02:43.000000 hosted-flasks-0.0.4/hosted_flasks/server.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 14:07:38.034349 hosted-flasks-0.0.4/hosted_flasks.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-04-27 14:07:38.000000 hosted-flasks-0.0.4/hosted_flasks.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)     1107 2024-04-27 14:07:38.000000 hosted-flasks-0.0.4/hosted_flasks.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2024-04-27 14:07:38.000000 hosted-flasks-0.0.4/hosted_flasks.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       62 2024-04-27 14:07:38.000000 hosted-flasks-0.0.4/hosted_flasks.egg-info/entry_points.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       29 2024-04-27 14:07:38.000000 hosted-flasks-0.0.4/hosted_flasks.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       25 2024-04-27 14:07:38.000000 hosted-flasks-0.0.4/hosted_flasks.egg-info/top_level.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2024-04-27 14:07:38.036552 hosted-flasks-0.0.4/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1627 2024-04-27 14:06:16.000000 hosted-flasks-0.0.4/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 14:07:38.036240 hosted-flasks-0.0.4/tests/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.4/tests/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      651 2024-04-25 19:07:50.000000 hosted-flasks-0.0.4/tests/test_config.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1440 2024-04-27 09:44:49.000000 hosted-flasks-0.0.4/tests/test_scanner.py
```

### Comparing `hosted-flasks-0.0.3/.github/README.md` & `hosted-flasks-0.0.4/.github/README.md`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.3/LICENSE.txt` & `hosted-flasks-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.3/PKG-INFO` & `hosted-flasks-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hosted-flasks
-Version: 0.0.3
+Version: 0.0.4
 Summary: serve flask apps side by side
 Home-page: https://github.com/christophevg/hosted-flasks
 Author: Christophe VG
 License: MIT
 Description: # Hosted Flasks
         
         > serve flask apps side by side
```

### Comparing `hosted-flasks-0.0.3/docs/conf.py` & `hosted-flasks-0.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.3/hosted_flasks/__main__.py` & `hosted-flasks-0.0.4/hosted_flasks/__main__.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.3/hosted_flasks/frontpage/index.html` & `hosted-flasks-0.0.4/hosted_flasks/frontpage/index.html`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.3/hosted_flasks/frontpage/static/android-chrome-192x192.png` & `hosted-flasks-0.0.4/hosted_flasks/frontpage/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.3/hosted_flasks/frontpage/static/android-chrome-512x512.png` & `hosted-flasks-0.0.4/hosted_flasks/frontpage/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.3/hosted_flasks/frontpage/static/apple-touch-icon.png` & `hosted-flasks-0.0.4/hosted_flasks/frontpage/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.3/hosted_flasks/frontpage/static/css/default.css` & `hosted-flasks-0.0.4/hosted_flasks/frontpage/static/css/default.css`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.3/hosted_flasks/frontpage/static/css/style.css` & `hosted-flasks-0.0.4/hosted_flasks/frontpage/static/css/style.css`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.3/hosted_flasks/frontpage/static/favicon-16x16.png` & `hosted-flasks-0.0.4/hosted_flasks/frontpage/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.3/hosted_flasks/frontpage/static/favicon-32x32.png` & `hosted-flasks-0.0.4/hosted_flasks/frontpage/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.3/hosted_flasks/frontpage/static/favicon.ico` & `hosted-flasks-0.0.4/hosted_flasks/frontpage/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.3/hosted_flasks/frontpage/static/img/logo.svg` & `hosted-flasks-0.0.4/hosted_flasks/frontpage/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.3/hosted_flasks/frontpage.py` & `hosted-flasks-0.0.4/hosted_flasks/frontpage.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.3/hosted_flasks/scanner.py` & `hosted-flasks-0.0.4/hosted_flasks/scanner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# ruff: noqa: E402
+# needed to avoid
+# RuntimeError: Working outside of application context.
+import eventlet
+eventlet.monkey_patch()
+
 import logging
 
 import os
 
 from pathlib import Path
 import importlib.util
 import sys
```

### Comparing `hosted-flasks-0.0.3/hosted_flasks/server.py` & `hosted-flasks-0.0.4/hosted_flasks/server.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.3/hosted_flasks.egg-info/PKG-INFO` & `hosted-flasks-0.0.4/hosted_flasks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hosted-flasks
-Version: 0.0.3
+Version: 0.0.4
 Summary: serve flask apps side by side
 Home-page: https://github.com/christophevg/hosted-flasks
 Author: Christophe VG
 License: MIT
 Description: # Hosted Flasks
         
         > serve flask apps side by side
```

### Comparing `hosted-flasks-0.0.3/hosted_flasks.egg-info/SOURCES.txt` & `hosted-flasks-0.0.4/hosted_flasks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.3/setup.py` & `hosted-flasks-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   
 ]
 INSTALL_REQUIRES = [
   "Flask",
   "python-dotenv",
+  "eventlet",
   
 ]
 ENTRY_POINTS = {
   "console_scripts" : [
     "hosted-flasks=hosted_flasks.__main__:cli",
     
   ]
```

### Comparing `hosted-flasks-0.0.3/tests/test_config.py` & `hosted-flasks-0.0.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.3/tests/test_scanner.py` & `hosted-flasks-0.0.4/tests/test_scanner.py`

 * *Files identical despite different names*

