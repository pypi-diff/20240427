# Comparing `tmp/instaOS-0.0.1.tar.gz` & `tmp/instaOS-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instaOS-0.0.1.tar", last modified: Sat Apr 27 17:02:50 2024, max compression
+gzip compressed data, was "instaOS-0.0.2.tar", last modified: Sat Apr 27 17:16:40 2024, max compression
```

## Comparing `instaOS-0.0.1.tar` & `instaOS-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 umitkoc   (1000) umitkoc   (1000)        0 2024-04-27 17:02:50.930033 instaOS-0.0.1/
--rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)     1067 2024-04-27 16:50:46.000000 instaOS-0.0.1/LICENSE
--rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)      820 2024-04-27 17:02:50.930033 instaOS-0.0.1/PKG-INFO
--rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)      211 2024-04-27 16:45:54.000000 instaOS-0.0.1/README.md
-drwxrwxr-x   0 umitkoc   (1000) umitkoc   (1000)        0 2024-04-27 17:02:50.926033 instaOS-0.0.1/instaOS/
--rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)       39 2024-04-27 16:51:36.000000 instaOS-0.0.1/instaOS/__init__.py
--rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)     6123 2024-04-27 16:56:34.000000 instaOS-0.0.1/instaOS/instagram.py
-drwxrwxr-x   0 umitkoc   (1000) umitkoc   (1000)        0 2024-04-27 17:02:50.930033 instaOS-0.0.1/instaOS.egg-info/
--rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)      820 2024-04-27 17:02:50.000000 instaOS-0.0.1/instaOS.egg-info/PKG-INFO
--rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)      221 2024-04-27 17:02:50.000000 instaOS-0.0.1/instaOS.egg-info/SOURCES.txt
--rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)        1 2024-04-27 17:02:50.000000 instaOS-0.0.1/instaOS.egg-info/dependency_links.txt
--rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)       87 2024-04-27 17:02:50.000000 instaOS-0.0.1/instaOS.egg-info/requires.txt
--rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)        8 2024-04-27 17:02:50.000000 instaOS-0.0.1/instaOS.egg-info/top_level.txt
--rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)       38 2024-04-27 17:02:50.930033 instaOS-0.0.1/setup.cfg
--rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)     1106 2024-04-27 16:55:21.000000 instaOS-0.0.1/setup.py
+drwxrwxr-x   0 umitkoc   (1000) umitkoc   (1000)        0 2024-04-27 17:16:39.999117 instaOS-0.0.2/
+-rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)     1067 2024-04-27 16:50:46.000000 instaOS-0.0.2/LICENSE
+-rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)      820 2024-04-27 17:16:39.999117 instaOS-0.0.2/PKG-INFO
+-rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)      211 2024-04-27 16:45:54.000000 instaOS-0.0.2/README.md
+drwxrwxr-x   0 umitkoc   (1000) umitkoc   (1000)        0 2024-04-27 17:16:39.999117 instaOS-0.0.2/instaOS/
+-rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)       39 2024-04-27 16:51:36.000000 instaOS-0.0.2/instaOS/__init__.py
+-rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)     6122 2024-04-27 17:15:11.000000 instaOS-0.0.2/instaOS/instagram.py
+drwxrwxr-x   0 umitkoc   (1000) umitkoc   (1000)        0 2024-04-27 17:16:39.999117 instaOS-0.0.2/instaOS.egg-info/
+-rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)      820 2024-04-27 17:16:39.000000 instaOS-0.0.2/instaOS.egg-info/PKG-INFO
+-rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)      221 2024-04-27 17:16:39.000000 instaOS-0.0.2/instaOS.egg-info/SOURCES.txt
+-rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)        1 2024-04-27 17:16:39.000000 instaOS-0.0.2/instaOS.egg-info/dependency_links.txt
+-rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)       87 2024-04-27 17:16:39.000000 instaOS-0.0.2/instaOS.egg-info/requires.txt
+-rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)        8 2024-04-27 17:16:39.000000 instaOS-0.0.2/instaOS.egg-info/top_level.txt
+-rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)       38 2024-04-27 17:16:39.999117 instaOS-0.0.2/setup.cfg
+-rw-rw-r--   0 umitkoc   (1000) umitkoc   (1000)     1106 2024-04-27 17:15:31.000000 instaOS-0.0.2/setup.py
```

### Comparing `instaOS-0.0.1/LICENSE` & `instaOS-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `instaOS-0.0.1/PKG-INFO` & `instaOS-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instaOS
-Version: 0.0.1
+Version: 0.0.2
 Summary: Instagram followers list and following list
 Home-page: UNKNOWN
 Author: Umit KOC
 Author-email: umitkoc.com@gmail.com
 License: UNKNOWN
 Keywords: instagram,followers,following,not following
 Platform: UNKNOWN
```

### Comparing `instaOS-0.0.1/instaOS/instagram.py` & `instaOS-0.0.2/instaOS/instagram.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.get_following(user_input=users)
         self.logger.info("__init__ func:finished")
         self.exit()
 
     def header(self):
         self.logger.info("header func:started")
         self.TIMEOUT = 15
-        service = Service(executable_path="../chromedriver")
+        service = Service(executable_path="./chromedriver")
         options = webdriver.ChromeOptions()
         #options.add_argument("--headless")
         options.add_argument('--no-sandbox')
         options.add_argument("--log-level=3")
         mobile_emulation = {
         "deviceMetrics": { "width": 360, "height": 640, "pixelRatio": 3.0 },
         "userAgent": "Mozilla/5.0 (Linux; Android 4.2.1; en-us; Nexus 5 Build/JOP40D) AppleWebKit/535.19 (KHTML, like Gecko) Chrome/124.0.6367.91 Mobile Safari/535.19","clientHints": {"platform": "Android", "mobile": True} }
```

### Comparing `instaOS-0.0.1/instaOS.egg-info/PKG-INFO` & `instaOS-0.0.2/instaOS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instaOS
-Version: 0.0.1
+Version: 0.0.2
 Summary: Instagram followers list and following list
 Home-page: UNKNOWN
 Author: Umit KOC
 Author-email: umitkoc.com@gmail.com
 License: UNKNOWN
 Keywords: instagram,followers,following,not following
 Platform: UNKNOWN
```

### Comparing `instaOS-0.0.1/setup.py` & `instaOS-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 
 with codecs.open(path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Instagram followers list and following list'
 LONG_DESCRIPTION = ''
 
 # Setting up
 setup(
     name="instaOS",
     version=VERSION,
```

