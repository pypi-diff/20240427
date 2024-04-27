# Comparing `tmp/geoparser-0.1.1.tar.gz` & `tmp/geoparser-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoparser-0.1.1.tar", last modified: Fri Apr 26 18:31:39 2024, max compression
+gzip compressed data, was "geoparser-0.1.2.tar", last modified: Fri Apr 26 20:25:05 2024, max compression
```

## Comparing `geoparser-0.1.1.tar` & `geoparser-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 18:31:39.755777 geoparser-0.1.1/
--rw-rw-rw-   0        0        0     1083 2024-04-26 18:30:53.000000 geoparser-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      455 2024-04-26 18:31:39.755777 geoparser-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       53 2024-04-26 18:30:53.000000 geoparser-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 18:31:39.742775 geoparser-0.1.1/geoparser/
--rw-rw-rw-   0        0        0       34 2024-04-26 18:30:53.000000 geoparser-0.1.1/geoparser/__init__.py
--rw-rw-rw-   0        0        0     1515 2024-04-26 18:30:53.000000 geoparser-0.1.1/geoparser/entities.py
--rw-rw-rw-   0        0        0     5647 2024-04-26 18:30:53.000000 geoparser-0.1.1/geoparser/gazetteer.py
--rw-rw-rw-   0        0        0     9241 2024-04-26 18:30:53.000000 geoparser-0.1.1/geoparser/geoparser.py
-drwxrwxrwx   0        0        0        0 2024-04-26 18:31:39.754777 geoparser-0.1.1/geoparser.egg-info/
--rw-rw-rw-   0        0        0      455 2024-04-26 18:31:39.000000 geoparser-0.1.1/geoparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-04-26 18:31:39.000000 geoparser-0.1.1/geoparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 18:31:39.000000 geoparser-0.1.1/geoparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-04-26 18:31:39.000000 geoparser-0.1.1/geoparser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-26 18:31:39.000000 geoparser-0.1.1/geoparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 18:31:39.755777 geoparser-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2413 2024-04-26 18:31:15.000000 geoparser-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 20:25:05.322834 geoparser-0.1.2/
+-rw-rw-rw-   0        0        0     1083 2024-04-26 20:12:16.000000 geoparser-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      455 2024-04-26 20:25:05.322332 geoparser-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       53 2024-04-26 20:12:16.000000 geoparser-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 20:25:05.307334 geoparser-0.1.2/geoparser/
+-rw-rw-rw-   0        0        0       34 2024-04-26 20:12:16.000000 geoparser-0.1.2/geoparser/__init__.py
+-rw-rw-rw-   0        0        0     1515 2024-04-26 20:12:16.000000 geoparser-0.1.2/geoparser/entities.py
+-rw-rw-rw-   0        0        0     5647 2024-04-26 20:12:16.000000 geoparser-0.1.2/geoparser/gazetteer.py
+-rw-rw-rw-   0        0        0     9241 2024-04-26 20:12:16.000000 geoparser-0.1.2/geoparser/geoparser.py
+drwxrwxrwx   0        0        0        0 2024-04-26 20:25:05.321333 geoparser-0.1.2/geoparser.egg-info/
+-rw-rw-rw-   0        0        0      455 2024-04-26 20:25:05.000000 geoparser-0.1.2/geoparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-04-26 20:25:05.000000 geoparser-0.1.2/geoparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 20:25:05.000000 geoparser-0.1.2/geoparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-04-26 20:25:05.000000 geoparser-0.1.2/geoparser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-26 20:25:05.000000 geoparser-0.1.2/geoparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 20:25:05.322834 geoparser-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2421 2024-04-26 20:24:11.000000 geoparser-0.1.2/setup.py
```

### Comparing `geoparser-0.1.1/LICENSE` & `geoparser-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geoparser-0.1.1/geoparser/entities.py` & `geoparser-0.1.2/geoparser/entities.py`

 * *Files identical despite different names*

### Comparing `geoparser-0.1.1/geoparser/gazetteer.py` & `geoparser-0.1.2/geoparser/gazetteer.py`

 * *Files identical despite different names*

### Comparing `geoparser-0.1.1/geoparser/geoparser.py` & `geoparser-0.1.2/geoparser/geoparser.py`

 * *Files identical despite different names*

### Comparing `geoparser-0.1.1/setup.py` & `geoparser-0.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pkg_resources
-import requests
 import zipfile
 import os
 import subprocess
 import sys
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
@@ -15,14 +14,15 @@
 
     def download_spacy(self):
         models = ["en_core_web_sm", "en_core_web_trf"]
         for model in models:
             subprocess.check_call([sys.executable, "-m", "spacy", "download", model])
 
     def download_geonames(self):
+        import requests
         site_packages = os.path.join(sys.prefix, 'lib', 'site-packages')
         data_dir = os.path.join(site_packages, 'geoparser', 'geonames')
         os.makedirs(data_dir, exist_ok=True)
 
         file_links = [
             "http://download.geonames.org/export/dump/allCountries.zip",
             "http://download.geonames.org/export/dump/admin1CodesASCII.txt",
@@ -42,15 +42,15 @@
             if filename.endswith('.zip'):
                 with zipfile.ZipFile(file_path, 'r') as zip_ref:
                     zip_ref.extractall(data_dir)
                 os.remove(file_path)
 
 setup(
     name='geoparser',
-    version='0.1.1',
+    version='0.1.2',
     author='Diego Gomes',
     author_email='diego.gomes@uzh.ch',
     packages=find_packages(),
     description='A geoparsing library for English texts',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
```

