# Comparing `tmp/hosted-flasks-0.0.1.tar.gz` & `tmp/hosted-flasks-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hosted-flasks-0.0.1.tar", last modified: Wed Mar 13 15:41:49 2024, max compression
+gzip compressed data, was "hosted-flasks-0.0.2.tar", last modified: Sat Apr 27 13:25:22 2024, max compression
```

## Comparing `hosted-flasks-0.0.1.tar` & `hosted-flasks-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-03-13 15:41:49.902824 hosted-flasks-0.0.1/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-03-13 15:41:49.901019 hosted-flasks-0.0.1/.github/
--rw-r--r--   0 xtof       (501) staff       (20)     1033 2024-03-13 07:52:10.000000 hosted-flasks-0.0.1/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)     1057 2024-03-13 07:52:10.000000 hosted-flasks-0.0.1/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)       77 2024-03-13 07:52:10.000000 hosted-flasks-0.0.1/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-03-13 15:41:49.902714 hosted-flasks-0.0.1/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-03-13 15:41:49.901207 hosted-flasks-0.0.1/docs/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.1/docs/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1149 2024-03-13 07:52:10.000000 hosted-flasks-0.0.1/docs/conf.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-03-13 15:41:49.901833 hosted-flasks-0.0.1/hosted_flasks/
--rw-r--r--   0 xtof       (501) staff       (20)       22 2024-03-13 12:59:34.000000 hosted-flasks-0.0.1/hosted_flasks/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      161 2024-03-13 15:36:53.000000 hosted-flasks-0.0.1/hosted_flasks/__main__.py
--rw-r--r--   0 xtof       (501) staff       (20)      476 2024-03-13 12:31:07.000000 hosted-flasks-0.0.1/hosted_flasks/frontpage.py
--rw-r--r--   0 xtof       (501) staff       (20)      403 2024-03-13 12:18:19.000000 hosted-flasks-0.0.1/hosted_flasks/log_setup.py
--rw-r--r--   0 xtof       (501) staff       (20)      929 2024-03-13 12:54:51.000000 hosted-flasks-0.0.1/hosted_flasks/scanner.py
--rw-r--r--   0 xtof       (501) staff       (20)      485 2024-03-13 12:30:48.000000 hosted-flasks-0.0.1/hosted_flasks/server.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-03-13 15:41:49.902368 hosted-flasks-0.0.1/hosted_flasks.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-03-13 15:41:49.000000 hosted-flasks-0.0.1/hosted_flasks.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)      459 2024-03-13 15:41:49.000000 hosted-flasks-0.0.1/hosted_flasks.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2024-03-13 15:41:49.000000 hosted-flasks-0.0.1/hosted_flasks.egg-info/dependency_links.txt
--rw-r--r--   0 xtof       (501) staff       (20)        6 2024-03-13 15:41:49.000000 hosted-flasks-0.0.1/hosted_flasks.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)       25 2024-03-13 15:41:49.000000 hosted-flasks-0.0.1/hosted_flasks.egg-info/top_level.txt
--rw-r--r--   0 xtof       (501) staff       (20)       38 2024-03-13 15:41:49.902867 hosted-flasks-0.0.1/setup.cfg
--rw-r--r--   0 xtof       (501) staff       (20)     1516 2024-03-13 07:52:10.000000 hosted-flasks-0.0.1/setup.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-03-13 15:41:49.902568 hosted-flasks-0.0.1/tests/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.1/tests/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      942 2024-03-13 12:59:11.000000 hosted-flasks-0.0.1/tests/test_example.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 13:25:22.291883 hosted-flasks-0.0.2/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 13:25:22.289802 hosted-flasks-0.0.2/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)     1033 2024-03-13 07:52:10.000000 hosted-flasks-0.0.2/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1057 2024-03-13 07:52:10.000000 hosted-flasks-0.0.2/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       77 2024-03-13 07:52:10.000000 hosted-flasks-0.0.2/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-04-27 13:25:22.291756 hosted-flasks-0.0.2/PKG-INFO
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 13:25:22.290013 hosted-flasks-0.0.2/docs/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.2/docs/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1149 2024-03-13 07:52:10.000000 hosted-flasks-0.0.2/docs/conf.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 13:25:22.290577 hosted-flasks-0.0.2/hosted_flasks/
+-rw-r--r--   0 xtof       (501) staff       (20)       22 2024-04-27 13:24:42.000000 hosted-flasks-0.0.2/hosted_flasks/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      686 2024-04-27 09:34:49.000000 hosted-flasks-0.0.2/hosted_flasks/__main__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      859 2024-04-27 13:12:57.000000 hosted-flasks-0.0.2/hosted_flasks/frontpage.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1562 2024-04-27 09:44:37.000000 hosted-flasks-0.0.2/hosted_flasks/scanner.py
+-rw-r--r--   0 xtof       (501) staff       (20)      796 2024-04-27 13:00:13.000000 hosted-flasks-0.0.2/hosted_flasks/server.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 13:25:22.291272 hosted-flasks-0.0.2/hosted_flasks.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-04-27 13:25:22.000000 hosted-flasks-0.0.2/hosted_flasks.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)      493 2024-04-27 13:25:22.000000 hosted-flasks-0.0.2/hosted_flasks.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2024-04-27 13:25:22.000000 hosted-flasks-0.0.2/hosted_flasks.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       62 2024-04-27 13:25:22.000000 hosted-flasks-0.0.2/hosted_flasks.egg-info/entry_points.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       20 2024-04-27 13:25:22.000000 hosted-flasks-0.0.2/hosted_flasks.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       25 2024-04-27 13:25:22.000000 hosted-flasks-0.0.2/hosted_flasks.egg-info/top_level.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2024-04-27 13:25:22.291937 hosted-flasks-0.0.2/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1613 2024-04-27 08:20:07.000000 hosted-flasks-0.0.2/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 13:25:22.291580 hosted-flasks-0.0.2/tests/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.2/tests/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      651 2024-04-25 19:07:50.000000 hosted-flasks-0.0.2/tests/test_config.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1440 2024-04-27 09:44:49.000000 hosted-flasks-0.0.2/tests/test_scanner.py
```

### Comparing `hosted-flasks-0.0.1/.github/README.md` & `hosted-flasks-0.0.2/.github/README.md`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.1/LICENSE.txt` & `hosted-flasks-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.1/PKG-INFO` & `hosted-flasks-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hosted-flasks
-Version: 0.0.1
+Version: 0.0.2
 Summary: serve flask apps side by side
 Home-page: https://github.com/christophevg/hosted-flasks
 Author: Christophe VG
 License: MIT
 Description: # Hosted Flasks
         
         > serve flask apps side by side
```

### Comparing `hosted-flasks-0.0.1/docs/conf.py` & `hosted-flasks-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.1/hosted_flasks.egg-info/PKG-INFO` & `hosted-flasks-0.0.2/hosted_flasks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hosted-flasks
-Version: 0.0.1
+Version: 0.0.2
 Summary: serve flask apps side by side
 Home-page: https://github.com/christophevg/hosted-flasks
 Author: Christophe VG
 License: MIT
 Description: # Hosted Flasks
         
         > serve flask apps side by side
```

### Comparing `hosted-flasks-0.0.1/setup.py` & `hosted-flasks-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,18 +18,22 @@
   "Environment :: Web Environment",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   
 ]
 INSTALL_REQUIRES = [
   "Flask",
+  "python-dotenv",
   
 ]
 ENTRY_POINTS = {
-  
+  "console_scripts" : [
+    "hosted-flasks=hosted_flasks.__main__:cli",
+    
+  ]
 }
 SCRIPTS = [
   
 ]
 
 HERE = os.path.dirname(__file__)
```

