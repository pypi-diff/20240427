# Comparing `tmp/xmonkey_namonica-0.1.0.tar.gz` & `tmp/xmonkey_namonica-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmonkey_namonica-0.1.0.tar", last modified: Thu Apr 25 23:58:55 2024, max compression
+gzip compressed data, was "xmonkey_namonica-0.1.1.tar", last modified: Fri Apr 26 18:37:39 2024, max compression
```

## Comparing `xmonkey_namonica-0.1.0.tar` & `xmonkey_namonica-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 23:58:55.807602 xmonkey_namonica-0.1.0/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11357 2024-04-25 02:09:33.000000 xmonkey_namonica-0.1.0/LICENSE
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       82 2024-04-25 23:58:55.807441 xmonkey_namonica-0.1.0/PKG-INFO
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       18 2024-04-25 02:09:33.000000 xmonkey_namonica-0.1.0/README.md
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       38 2024-04-25 23:58:55.807656 xmonkey_namonica-0.1.0/setup.cfg
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      352 2024-04-25 06:46:13.000000 xmonkey_namonica-0.1.0/setup.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 23:58:55.805617 xmonkey_namonica-0.1.0/xmonkey_namonica/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:08.000000 xmonkey_namonica-0.1.0/xmonkey_namonica/__init__.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1804 2024-04-25 23:53:32.000000 xmonkey_namonica-0.1.0/xmonkey_namonica/cli.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3769 2024-04-25 23:05:14.000000 xmonkey_namonica-0.1.0/xmonkey_namonica/common.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 23:58:55.807018 xmonkey_namonica-0.1.0/xmonkey_namonica/handlers/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:41.000000 xmonkey_namonica-0.1.0/xmonkey_namonica/handlers/__init__.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      956 2024-04-25 07:37:41.000000 xmonkey_namonica-0.1.0/xmonkey_namonica/handlers/base_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2173 2024-04-25 23:56:19.000000 xmonkey_namonica-0.1.0/xmonkey_namonica/handlers/cargo_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2157 2024-04-25 08:32:55.000000 xmonkey_namonica-0.1.0/xmonkey_namonica/handlers/npm_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2180 2024-04-25 23:58:52.000000 xmonkey_namonica-0.1.0/xmonkey_namonica/handlers/nuget_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2252 2024-04-25 23:56:07.000000 xmonkey_namonica-0.1.0/xmonkey_namonica/handlers/pypi_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1608 2024-04-25 07:37:29.000000 xmonkey_namonica-0.1.0/xmonkey_namonica/utils.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 23:58:55.807279 xmonkey_namonica-0.1.0/xmonkey_namonica.egg-info/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       82 2024-04-25 23:58:55.000000 xmonkey_namonica-0.1.0/xmonkey_namonica.egg-info/PKG-INFO
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      584 2024-04-25 23:58:55.000000 xmonkey_namonica-0.1.0/xmonkey_namonica.egg-info/SOURCES.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        1 2024-04-25 23:58:55.000000 xmonkey_namonica-0.1.0/xmonkey_namonica.egg-info/dependency_links.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       63 2024-04-25 23:58:55.000000 xmonkey_namonica-0.1.0/xmonkey_namonica.egg-info/entry_points.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       17 2024-04-25 23:58:55.000000 xmonkey_namonica-0.1.0/xmonkey_namonica.egg-info/top_level.txt
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-26 18:37:39.108389 xmonkey_namonica-0.1.1/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11357 2024-04-25 02:09:33.000000 xmonkey_namonica-0.1.1/LICENSE
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       82 2024-04-26 18:37:39.108226 xmonkey_namonica-0.1.1/PKG-INFO
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      174 2024-04-26 18:19:26.000000 xmonkey_namonica-0.1.1/README.md
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       38 2024-04-26 18:37:39.108426 xmonkey_namonica-0.1.1/setup.cfg
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      352 2024-04-26 18:35:21.000000 xmonkey_namonica-0.1.1/setup.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-26 18:37:39.104441 xmonkey_namonica-0.1.1/xmonkey_namonica/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:08.000000 xmonkey_namonica-0.1.1/xmonkey_namonica/__init__.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1804 2024-04-25 23:53:32.000000 xmonkey_namonica-0.1.1/xmonkey_namonica/cli.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3716 2024-04-26 18:36:04.000000 xmonkey_namonica-0.1.1/xmonkey_namonica/common.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-26 18:37:39.107731 xmonkey_namonica-0.1.1/xmonkey_namonica/handlers/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:41.000000 xmonkey_namonica-0.1.1/xmonkey_namonica/handlers/__init__.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      956 2024-04-25 07:37:41.000000 xmonkey_namonica-0.1.1/xmonkey_namonica/handlers/base_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2152 2024-04-26 17:48:14.000000 xmonkey_namonica-0.1.1/xmonkey_namonica/handlers/cargo_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2188 2024-04-26 18:32:41.000000 xmonkey_namonica-0.1.1/xmonkey_namonica/handlers/npm_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2148 2024-04-26 17:48:03.000000 xmonkey_namonica-0.1.1/xmonkey_namonica/handlers/nuget_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2218 2024-04-26 17:49:28.000000 xmonkey_namonica-0.1.1/xmonkey_namonica/handlers/pypi_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1608 2024-04-26 17:39:40.000000 xmonkey_namonica-0.1.1/xmonkey_namonica/utils.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-26 18:37:39.108062 xmonkey_namonica-0.1.1/xmonkey_namonica.egg-info/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       82 2024-04-26 18:37:39.000000 xmonkey_namonica-0.1.1/xmonkey_namonica.egg-info/PKG-INFO
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      584 2024-04-26 18:37:39.000000 xmonkey_namonica-0.1.1/xmonkey_namonica.egg-info/SOURCES.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        1 2024-04-26 18:37:39.000000 xmonkey_namonica-0.1.1/xmonkey_namonica.egg-info/dependency_links.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       63 2024-04-26 18:37:39.000000 xmonkey_namonica-0.1.1/xmonkey_namonica.egg-info/entry_points.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       17 2024-04-26 18:37:39.000000 xmonkey_namonica-0.1.1/xmonkey_namonica.egg-info/top_level.txt
```

### Comparing `xmonkey_namonica-0.1.0/LICENSE` & `xmonkey_namonica-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.0/xmonkey_namonica/cli.py` & `xmonkey_namonica-0.1.1/xmonkey_namonica/cli.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.0/xmonkey_namonica/common.py` & `xmonkey_namonica-0.1.1/xmonkey_namonica/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import os
-import json
 import re
+import json
 from urllib.parse import unquote, urlparse, parse_qs
-from .utils import download_file, temp_directory, extract_zip, extract_tar
 from urllib.parse import urlparse, parse_qs, unquote
+from .utils import download_file, temp_directory, extract_zip, extract_tar
 
 
 class PackageManager:
     @staticmethod
     def parse_purl(purl):
         result = {}
         url = urlparse(purl)
         if url.scheme != 'pkg':
             raise ValueError("Invalid PURL scheme")
         path_parts = url.path.strip('/').split('/')
         if len(path_parts) < 2:
             raise ValueError(
                 "Invalid PURL format. Expected at least pkg:type/name@version"
             )
-        result['type'] = path_parts[1]
+        result['type'] = path_parts[0]
         name_with_version = path_parts[-1]
-        if len(path_parts) == 4:
-            result['namespace'] = unquote(path_parts[2])
+        if len(path_parts) == 3:
+            result['namespace'] = unquote(path_parts[1])
         else:
             result['namespace'] = None
         name_version = name_with_version.split('@', 1)
         result['name'] = unquote(name_version[0])
         if len(name_version) > 1:
             result['version'] = name_version[1]
         else:
@@ -80,17 +80,16 @@
         pattern = "[^0-9<>,.()@a-zA-Z-\s]+"
         for root, _, files in os.walk(temp_dir):
             for file in files:
                 file_path = os.path.join(root, file)
                 try:
                     with open(file_path, 'r', encoding='utf-8') as f:
                         for line in f:
-                            if "copyright" in line.lower() and any(
-                                char.isdigit() for char in line.lower()
-                            ):
+                            if ("copyright" in line.lower() and
+                                    len(line) <= 50):
                                 copyhit = line.strip()
                                 copyhit = re.sub(pattern, "", line.strip())
                                 copyrights.append({
                                     "file": file_path,
                                     "line": copyhit.strip()
                                 })
                 except UnicodeDecodeError:
```

### Comparing `xmonkey_namonica-0.1.0/xmonkey_namonica/handlers/base_handler.py` & `xmonkey_namonica-0.1.1/xmonkey_namonica/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.0/xmonkey_namonica/handlers/cargo_handler.py` & `xmonkey_namonica-0.1.1/xmonkey_namonica/handlers/pypi_handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from ..utils import download_file, temp_directory, extract_tar
-from ..utils import download_file, temp_directory, extract_tar
+import os
+import logging
 from .base_handler import BaseHandler
 from ..common import PackageManager, temp_directory
-import os
+from ..utils import download_file, temp_directory, extract_tar
 
 
-class CargoHandler(BaseHandler):
+class PypiHandler(BaseHandler):
     def fetch(self):
         download_url = self.construct_download_url()
         with temp_directory() as temp_dir:
             filename = (
                 f"{self.purl_details['name']}-"
                 f"{self.purl_details['version']}.tgz"
             )
             package_file_path = os.path.join(
                 temp_dir,
                 filename
             )
             download_file(download_url, package_file_path)
-            print(f"Downloaded RUST package to {package_file_path}")
+            logging.info(f"Downloaded package to {package_file_path}")
             self.temp_dir = temp_dir
             self.unpack()
             self.scan()
 
     def unpack(self):
         if self.temp_dir:
             filename = (
@@ -30,35 +30,36 @@
                 f"{self.purl_details['version']}.tgz"
             )
             package_file_path = os.path.join(
                 self.temp_dir,
                 filename
             )
             extract_tar(package_file_path, self.temp_dir)
-            print(f"Unpacked RUST package in {self.temp_dir}")
+            logging.info(f"Unpacked package in {self.temp_dir}")
 
     def scan(self):
         results = {}
-        print("Scanning package contents...")
+        logging.info("Scanning package contents...")
         files = PackageManager.scan_for_files(
-            self.temp_dir, ['.txt', '.md', 'LICENSE']
+            self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE']
         )
         results['license_files'] = files
         copyhits = PackageManager.scan_for_copyright(self.temp_dir)
         results['copyrights'] = copyhits
         self.results = results
 
     def generate_report(self):
-        print("Generating report based on the scanned data...")
+        logging.info("Generating report based on the scanned data...")
         return self.results
 
     def construct_download_url(self):
         namespace = (
             self.purl_details['namespace'].replace('%40', '@')
             if self.purl_details['namespace']
             else self.purl_details['name']
         )
+        iniName = namespace[0].lower()
         return (
-            f"https://crates.io/api/v1/crates/"
-            f"{self.purl_details['name']}/"
-            f"{self.purl_details['version']}/download"
+            f"https://pypi.python.org/packages/source/{iniName}/{namespace}/"
+            f"{self.purl_details['name']}-"
+            f"{self.purl_details['version']}.tar.gz"
         )
```

### Comparing `xmonkey_namonica-0.1.0/xmonkey_namonica/handlers/npm_handler.py` & `xmonkey_namonica-0.1.1/xmonkey_namonica/handlers/nuget_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,64 @@
-from ..utils import download_file, temp_directory, extract_tar
-from ..utils import download_file, temp_directory, extract_tar
+import os
+import logging
 from .base_handler import BaseHandler
 from ..common import PackageManager, temp_directory
-import os
+from ..utils import download_file, temp_directory, extract_zip
 
 
-class NpmHandler(BaseHandler):
+class NugetHandler(BaseHandler):
     def fetch(self):
         download_url = self.construct_download_url()
         with temp_directory() as temp_dir:
             filename = (
                 f"{self.purl_details['name']}-"
-                f"{self.purl_details['version']}.tgz"
+                f"{self.purl_details['version']}.zip"
             )
             package_file_path = os.path.join(
                 temp_dir,
                 filename
             )
             download_file(download_url, package_file_path)
-            print(f"Downloaded NPM package to {package_file_path}")
+            logging.info(f"Downloaded package to {package_file_path}")
             self.temp_dir = temp_dir
             self.unpack()
             self.scan()
 
     def unpack(self):
         if self.temp_dir:
             filename = (
                 f"{self.purl_details['name']}-"
-                f"{self.purl_details['version']}.tgz"
+                f"{self.purl_details['version']}.zip"
             )
             package_file_path = os.path.join(
                 self.temp_dir,
                 filename
             )
-            extract_tar(package_file_path, self.temp_dir)
-            print(f"Unpacked NPM package in {self.temp_dir}")
+            extract_zip(package_file_path, self.temp_dir)
+            logging.info(f"Unpacked package in {self.temp_dir}")
 
     def scan(self):
         results = {}
-        print("Scanning package contents...")
+        logging.info("Scanning package contents...")
         files = PackageManager.scan_for_files(
-            self.temp_dir, ['.txt', '.md', 'LICENSE']
+            self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE']
         )
         results['license_files'] = files
         copyhits = PackageManager.scan_for_copyright(self.temp_dir)
         results['copyrights'] = copyhits
         self.results = results
 
     def generate_report(self):
-        print("Generating report based on the scanned data...")
+        logging.info("Generating report based on the scanned data...")
         return self.results
 
     def construct_download_url(self):
         namespace = (
             self.purl_details['namespace'].replace('%40', '@')
             if self.purl_details['namespace']
             else self.purl_details['name']
         )
         return (
-            f"https://registry.npmjs.org/{namespace}/-/"
-            f"{self.purl_details['name']}-{self.purl_details['version']}.tgz"
+            f"https://www.nuget.org/api/v2/package/"
+            f"{self.purl_details['name']}/"
+            f"{self.purl_details['version']}"
         )
```

### Comparing `xmonkey_namonica-0.1.0/xmonkey_namonica/handlers/nuget_handler.py` & `xmonkey_namonica-0.1.1/xmonkey_namonica/handlers/cargo_handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-from ..utils import download_file, temp_directory, extract_zip
-from ..utils import download_file, temp_directory, extract_zip
+import os
+import logging
 from .base_handler import BaseHandler
 from ..common import PackageManager, temp_directory
-import os
+from ..utils import download_file, temp_directory, extract_tar
 
 
-class NugetHandler(BaseHandler):
+class CargoHandler(BaseHandler):
     def fetch(self):
         download_url = self.construct_download_url()
         with temp_directory() as temp_dir:
             filename = (
                 f"{self.purl_details['name']}-"
-                f"{self.purl_details['version']}.zip"
+                f"{self.purl_details['version']}.tgz"
             )
             package_file_path = os.path.join(
                 temp_dir,
                 filename
             )
             download_file(download_url, package_file_path)
-            print(f"Downloaded NUGET package to {package_file_path}")
+            logging.info(f"Unpacked package in {self.temp_dir}")
             self.temp_dir = temp_dir
             self.unpack()
             self.scan()
 
     def unpack(self):
         if self.temp_dir:
             filename = (
                 f"{self.purl_details['name']}-"
-                f"{self.purl_details['version']}.zip"
+                f"{self.purl_details['version']}.tgz"
             )
             package_file_path = os.path.join(
                 self.temp_dir,
                 filename
             )
-            extract_zip(package_file_path, self.temp_dir)
-            print(f"Unpacked NUGET package in {self.temp_dir}")
+            extract_tar(package_file_path, self.temp_dir)
+            logging.info(f"Unpacked NUGET package in {self.temp_dir}")
 
     def scan(self):
         results = {}
-        print("Scanning package contents...")
+        logging.info("Scanning package contents...")
         files = PackageManager.scan_for_files(
             self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE']
         )
         results['license_files'] = files
         copyhits = PackageManager.scan_for_copyright(self.temp_dir)
         results['copyrights'] = copyhits
         self.results = results
 
     def generate_report(self):
-        print("Generating report based on the scanned data...")
+        logging.info("Generating report based on the scanned data...")
         return self.results
 
     def construct_download_url(self):
         namespace = (
             self.purl_details['namespace'].replace('%40', '@')
             if self.purl_details['namespace']
             else self.purl_details['name']
         )
         return (
-            f"https://www.nuget.org/api/v2/package/"
+            f"https://crates.io/api/v1/crates/"
             f"{self.purl_details['name']}/"
-            f"{self.purl_details['version']}"
+            f"{self.purl_details['version']}/download"
         )
```

### Comparing `xmonkey_namonica-0.1.0/xmonkey_namonica/handlers/pypi_handler.py` & `xmonkey_namonica-0.1.1/xmonkey_namonica/handlers/npm_handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from ..utils import download_file, temp_directory, extract_tar
-from ..utils import download_file, temp_directory, extract_tar
+import os
+import logging
 from .base_handler import BaseHandler
 from ..common import PackageManager, temp_directory
-import os
+from ..utils import download_file, temp_directory, extract_tar
 
 
-class PypiHandler(BaseHandler):
+class NpmHandler(BaseHandler):
     def fetch(self):
         download_url = self.construct_download_url()
         with temp_directory() as temp_dir:
             filename = (
                 f"{self.purl_details['name']}-"
                 f"{self.purl_details['version']}.tgz"
             )
             package_file_path = os.path.join(
                 temp_dir,
                 filename
             )
             download_file(download_url, package_file_path)
-            print(f"Downloaded Python package to {package_file_path}")
+            logging.info(f"Downloaded package to {package_file_path}")
             self.temp_dir = temp_dir
             self.unpack()
             self.scan()
 
     def unpack(self):
         if self.temp_dir:
             filename = (
@@ -30,36 +30,35 @@
                 f"{self.purl_details['version']}.tgz"
             )
             package_file_path = os.path.join(
                 self.temp_dir,
                 filename
             )
             extract_tar(package_file_path, self.temp_dir)
-            print(f"Unpacked Python package in {self.temp_dir}")
+            logging.info(f"Unpacked package in {self.temp_dir}")
 
     def scan(self):
         results = {}
-        print("Scanning package contents...")
+        logging.info("Scanning package contents...")
         files = PackageManager.scan_for_files(
             self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE']
         )
         results['license_files'] = files
         copyhits = PackageManager.scan_for_copyright(self.temp_dir)
         results['copyrights'] = copyhits
         self.results = results
 
     def generate_report(self):
-        print("Generating report based on the scanned data...")
+        logging.info("Generating report based on the scanned data...")
         return self.results
 
     def construct_download_url(self):
         namespace = (
-            self.purl_details['namespace'].replace('%40', '@')
+            self.purl_details['namespace'].replace('%40', '@') + '/' + self.purl_details['name']
             if self.purl_details['namespace']
             else self.purl_details['name']
         )
-        iniName = namespace[0].lower()
         return (
-            f"https://pypi.python.org/packages/source/{iniName}/{namespace}/"
-            f"{self.purl_details['name']}-"
-            f"{self.purl_details['version']}.tar.gz"
+            f"https://registry.npmjs.org/"
+            f"{namespace}/-/"
+            f"{self.purl_details['name']}-{self.purl_details['version']}.tgz"
         )
```

### Comparing `xmonkey_namonica-0.1.0/xmonkey_namonica/utils.py` & `xmonkey_namonica-0.1.1/xmonkey_namonica/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+import os
 import requests
 import logging
 import zipfile
 import tarfile
-import os
 import tempfile
 import shutil
 from contextlib import contextmanager
 
 
 logging.basicConfig(
     level=logging.INFO,
```

### Comparing `xmonkey_namonica-0.1.0/xmonkey_namonica.egg-info/SOURCES.txt` & `xmonkey_namonica-0.1.1/xmonkey_namonica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

