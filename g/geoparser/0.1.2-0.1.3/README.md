# Comparing `tmp/geoparser-0.1.2.tar.gz` & `tmp/geoparser-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoparser-0.1.2.tar", last modified: Fri Apr 26 20:25:05 2024, max compression
+gzip compressed data, was "geoparser-0.1.3.tar", last modified: Sat Apr 27 13:22:14 2024, max compression
```

## Comparing `geoparser-0.1.2.tar` & `geoparser-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 20:25:05.322834 geoparser-0.1.2/
--rw-rw-rw-   0        0        0     1083 2024-04-26 20:12:16.000000 geoparser-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      455 2024-04-26 20:25:05.322332 geoparser-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       53 2024-04-26 20:12:16.000000 geoparser-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 20:25:05.307334 geoparser-0.1.2/geoparser/
--rw-rw-rw-   0        0        0       34 2024-04-26 20:12:16.000000 geoparser-0.1.2/geoparser/__init__.py
--rw-rw-rw-   0        0        0     1515 2024-04-26 20:12:16.000000 geoparser-0.1.2/geoparser/entities.py
--rw-rw-rw-   0        0        0     5647 2024-04-26 20:12:16.000000 geoparser-0.1.2/geoparser/gazetteer.py
--rw-rw-rw-   0        0        0     9241 2024-04-26 20:12:16.000000 geoparser-0.1.2/geoparser/geoparser.py
-drwxrwxrwx   0        0        0        0 2024-04-26 20:25:05.321333 geoparser-0.1.2/geoparser.egg-info/
--rw-rw-rw-   0        0        0      455 2024-04-26 20:25:05.000000 geoparser-0.1.2/geoparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-04-26 20:25:05.000000 geoparser-0.1.2/geoparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 20:25:05.000000 geoparser-0.1.2/geoparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-04-26 20:25:05.000000 geoparser-0.1.2/geoparser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-26 20:25:05.000000 geoparser-0.1.2/geoparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 20:25:05.322834 geoparser-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2421 2024-04-26 20:24:11.000000 geoparser-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 13:22:14.597037 geoparser-0.1.3/
+-rw-rw-rw-   0        0        0     1083 2024-04-27 11:43:17.000000 geoparser-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      455 2024-04-27 13:22:14.596037 geoparser-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       53 2024-04-27 11:43:17.000000 geoparser-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 13:22:14.587036 geoparser-0.1.3/geoparser/
+-rw-rw-rw-   0        0        0       34 2024-04-27 12:54:59.000000 geoparser-0.1.3/geoparser/__init__.py
+-rw-rw-rw-   0        0        0      232 2024-04-27 12:54:57.000000 geoparser-0.1.3/geoparser/__main__.py
+-rw-rw-rw-   0        0        0     3977 2024-04-27 13:12:31.000000 geoparser-0.1.3/geoparser/downloader.py
+-rw-rw-rw-   0        0        0     1525 2024-04-27 12:55:09.000000 geoparser-0.1.3/geoparser/entities.py
+-rw-rw-rw-   0        0        0     5583 2024-04-27 12:55:13.000000 geoparser-0.1.3/geoparser/gazetteer.py
+-rw-rw-rw-   0        0        0     8415 2024-04-27 12:55:18.000000 geoparser-0.1.3/geoparser/geoparser.py
+drwxrwxrwx   0        0        0        0 2024-04-27 13:22:14.596037 geoparser-0.1.3/geoparser.egg-info/
+-rw-rw-rw-   0        0        0      455 2024-04-27 13:22:14.000000 geoparser-0.1.3/geoparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2024-04-27 13:22:14.000000 geoparser-0.1.3/geoparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 13:22:14.000000 geoparser-0.1.3/geoparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-04-27 13:22:14.000000 geoparser-0.1.3/geoparser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-27 13:22:14.000000 geoparser-0.1.3/geoparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 13:22:14.597037 geoparser-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      763 2024-04-27 12:56:34.000000 geoparser-0.1.3/setup.py
```

### Comparing `geoparser-0.1.2/LICENSE` & `geoparser-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geoparser-0.1.2/geoparser/entities.py` & `geoparser-0.1.3/geoparser/entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,8 +35,9 @@
 
 class Document:
     def __init__(self, text: str):
         self.text = text
         self.toponyms: List[Toponym] = []
 
     def __str__(self):
-        return self.text
+        return self.text
+
```

### Comparing `geoparser-0.1.2/geoparser/gazetteer.py` & `geoparser-0.1.3/geoparser/gazetteer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-import pkg_resources
+import os
+from appdirs import user_data_dir
 import pandas as pd
 import numpy as np
 
 class Gazetteer:
     def __init__(self):
-        self.geonames_file = pkg_resources.resource_filename('geoparser', 'geonames/allCountries.txt')
-        self.admin1_file = pkg_resources.resource_filename('geoparser', 'geonames/admin1CodesASCII.txt')
-        self.admin2_file = pkg_resources.resource_filename('geoparser', 'geonames/admin2Codes.txt')
-        self.country_info_file = pkg_resources.resource_filename('geoparser', 'geonames/countryInfo.txt')
-        self.feature_codes_file = pkg_resources.resource_filename('geoparser', 'geonames/featureCodes_en.txt')
+        data_dir = user_data_dir('geoparser')
+        
+        self.geonames_file = os.path.join(data_dir, 'allCountries.txt')
+        self.admin1_file = os.path.join(data_dir, 'admin1CodesASCII.txt')
+        self.admin2_file = os.path.join(data_dir, 'admin2Codes.txt')
+        self.country_info_file = os.path.join(data_dir, 'countryInfo.txt')
+        self.feature_codes_file = os.path.join(data_dir, 'featureCodes_en.txt')
         self.data = None
 
     def load(self, all_candidates):
         
         cols = ['geonameid', 'name', 'asciiname', 'alternatenames', 'latitude', 'longitude', 
                  'feature_class', 'feature_code', 'country_code', 'cc2', 'admin1_code', 'admin2_code', 
                  'admin3_code', 'admin4_code', 'population', 'elevation', 'dem', 'timezone', 
@@ -94,8 +97,9 @@
         components = [row['name']]
         for field in ['admin2_name', 'admin1_name', 'country_name']:
             if pd.notna(row[field]):
                 components.append(row[field])
         location_str = " in " + ", ".join(components[1:]) if len(components) > 1 else ""
         feature_str = f" ({row['feature_name']})" if pd.notna(row['feature_name']) else ""
     
-        return f"{components[0]}{feature_str}{location_str}"
+        return f"{components[0]}{feature_str}{location_str}"
+
```

### Comparing `geoparser-0.1.2/geoparser/geoparser.py` & `geoparser-0.1.3/geoparser/geoparser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 import os
 import re
 import pickle
 import unicodedata
 import logging
-import pkg_resources
 import spacy
 from tqdm.auto import tqdm
 from typing import List, Set
 from sentence_transformers import SentenceTransformer, util
+from appdirs import user_data_dir
 import torch
 
 from .entities import Document, Toponym, Location
 from .gazetteer import Gazetteer
 
 # Suppress token length warnings from transformers
 logging.getLogger("transformers.tokenization_utils_base").setLevel(logging.ERROR)
 
 class Geoparser:
     def __init__(self, spacy_model='en_core_web_trf', transformer_model='dguzh/geo-all-distilroberta-v1'):
         self.ensure_spacy_model(spacy_model)
         self.nlp = spacy.load(spacy_model)
         self.transformer = SentenceTransformer(transformer_model)
-        self.index_file = pkg_resources.resource_filename('geoparser', 'index.pkl')
-        self.geonames_file = pkg_resources.resource_filename('geoparser', 'geonames/allCountries.txt')
+        
+        data_dir = user_data_dir('geoparser')
+        self.index_file = os.path.join(data_dir, 'index.pkl')
+        self.geonames_file = os.path.join(data_dir, 'allCountries.txt')
+        
         self.index = self.load_index()
         self.tokenizer = self.transformer.tokenizer
         self.model_max_length = self.tokenizer.model_max_length
 
     def ensure_spacy_model(self, model_name):
         if not spacy.util.is_package(model_name):
             print(f"Downloading spaCy model '{model_name}'...")
@@ -39,35 +42,15 @@
         return name.lower()  # convert to lowercase
 
     def load_index(self):
         if os.path.exists(self.index_file):
             with open(self.index_file, 'rb') as file:
                 return pickle.load(file)
         else:
-            index = self.build_index()
-            with open(self.index_file, 'wb') as file:
-                pickle.dump(index, file)
-            return index
-
-    def build_index(self):
-        index = {}
-        with open(self.geonames_file, 'r', encoding='utf-8') as file:
-            total_lines = sum(1 for line in file)
-        with open(self.geonames_file, 'r', encoding='utf-8') as file:
-            for line in tqdm(file, total=total_lines, desc="Building index", unit=" lines"):
-                columns = line.strip().split('\t')
-                geonameid = int(columns[0])
-                names = [columns[1]] + columns[3].split(',')
-                for name in names:
-                    normalized_name = self.normalize_name(name)
-                    if normalized_name:
-                        if normalized_name not in index:
-                            index[normalized_name] = set()
-                        index[normalized_name].add(geonameid)
-        return index
+            raise FileNotFoundError("GeoNames index file not found. Please run 'python -m geoparser download' to generate it.")
 
     def parse(self, texts: List[str]):
         documents = [Document(text) for text in texts]
         for document in documents:
             self.extract_toponyms(document)
         self.resolve_toponyms(documents)
         return documents
@@ -192,8 +175,9 @@
                             country_name=predicted_location['country_name'],
                             feature_name=predicted_location['feature_name'],
                             latitude=predicted_location['latitude'],
                             longitude=predicted_location['longitude'],
                             elevation=predicted_location['elevation'],
                             population=predicted_location['population']
                         )
-                    toponym_index += 1
+                    toponym_index += 1
+
```

