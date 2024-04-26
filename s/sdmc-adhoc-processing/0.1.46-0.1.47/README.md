# Comparing `tmp/sdmc_adhoc_processing-0.1.46.tar.gz` & `tmp/sdmc_adhoc_processing-0.1.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdmc_adhoc_processing-0.1.46.tar", last modified: Mon Apr 15 21:59:15 2024, max compression
+gzip compressed data, was "sdmc_adhoc_processing-0.1.47.tar", last modified: Fri Apr 26 22:55:30 2024, max compression
```

## Comparing `sdmc_adhoc_processing-0.1.46.tar` & `sdmc_adhoc_processing-0.1.47.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 bhaddock (80211) staff     (1000)        0 2024-04-15 21:59:15.561651 sdmc_adhoc_processing-0.1.46/
--rw-rw-r--   0 bhaddock (80211) staff     (1000)    35149 2024-03-01 20:01:53.000000 sdmc_adhoc_processing-0.1.46/LICENSE
--rw-r--r--   0 bhaddock (80211) staff     (1000)      619 2024-04-15 21:59:15.557654 sdmc_adhoc_processing-0.1.46/PKG-INFO
--rw-rw-r--   0 bhaddock (80211) staff     (1000)       69 2024-03-01 19:56:23.000000 sdmc_adhoc_processing-0.1.46/README.md
--rw-rw-r--   0 bhaddock (80211) staff     (1000)     1037 2024-04-15 21:56:29.000000 sdmc_adhoc_processing-0.1.46/pyproject.toml
--rw-rw-r--   0 bhaddock (80211) staff     (1000)       38 2024-04-15 21:59:15.561686 sdmc_adhoc_processing-0.1.46/setup.cfg
-drwxrwxr-x   0 bhaddock (80211) staff     (1000)        0 2024-04-15 21:59:15.486708 sdmc_adhoc_processing-0.1.46/src/
-drwxrwxr-x   0 bhaddock (80211) staff     (1000)        0 2024-04-15 21:59:15.526645 sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing/
--rw-rw-r--   0 bhaddock (80211) staff     (1000)      313 2024-03-15 23:09:53.000000 sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing/__init__.py
--rw-rw-r--   0 bhaddock (80211) staff     (1000)     3197 2024-04-10 20:42:00.000000 sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing/constants.py
--rwxrwx---   0 bhaddock (80211) staff     (1000)    12964 2024-03-22 18:48:38.000000 sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing/data_dictionary_TEMPLATE.xlsx
--rwxrwx---   0 bhaddock (80211) staff     (1000)    10205 2024-03-22 18:52:44.000000 sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing/data_dictionary_nonstandard_vars.xlsx
--rw-rw-r--   0 bhaddock (80211) staff     (1000)     6589 2024-04-15 20:00:36.000000 sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing/generate_README.py
--rwxrwx---   0 bhaddock (80211) staff     (1000)     5889 2024-04-15 18:59:57.000000 sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing/generate_dict.py
--rw-rw-r--   0 bhaddock (80211) staff     (1000)     9237 2024-04-11 19:14:15.000000 sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing/process.py
--rw-rw-r--   0 bhaddock (80211) staff     (1000)     1248 2024-04-15 20:06:25.000000 sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing/readme_template.md
--rw-rw-r--   0 bhaddock (80211) staff     (1000)      313 2024-04-10 18:40:18.000000 sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing/utilities.py
-drwxrwxr-x   0 bhaddock (80211) staff     (1000)        0 2024-04-15 21:59:15.553674 sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing.egg-info/
--rw-r--r--   0 bhaddock (80211) staff     (1000)      619 2024-04-15 21:59:15.000000 sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing.egg-info/PKG-INFO
--rw-rw-r--   0 bhaddock (80211) staff     (1000)      752 2024-04-15 21:59:15.000000 sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing.egg-info/SOURCES.txt
--rw-rw-r--   0 bhaddock (80211) staff     (1000)        1 2024-04-15 21:59:15.000000 sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing.egg-info/dependency_links.txt
--rw-rw-r--   0 bhaddock (80211) staff     (1000)      146 2024-04-15 21:59:15.000000 sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing.egg-info/entry_points.txt
--rw-rw-r--   0 bhaddock (80211) staff     (1000)       23 2024-04-15 21:59:15.000000 sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing.egg-info/requires.txt
--rw-rw-r--   0 bhaddock (80211) staff     (1000)       22 2024-04-15 21:59:15.000000 sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing.egg-info/top_level.txt
-drwxrwxr-x   0 bhaddock (80211) staff     (1000)        0 2024-04-15 21:59:15.549700 sdmc_adhoc_processing-0.1.46/tests/
--rw-rw-r--   0 bhaddock (80211) staff     (1000)      100 2024-03-01 19:54:57.000000 sdmc_adhoc_processing-0.1.46/tests/test_foo.py
+drwxrwxr-x   0 bhaddock (80211) staff     (1000)        0 2024-04-26 22:55:30.262785 sdmc_adhoc_processing-0.1.47/
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)    35149 2024-03-01 20:01:53.000000 sdmc_adhoc_processing-0.1.47/LICENSE
+-rw-r--r--   0 bhaddock (80211) staff     (1000)      619 2024-04-26 22:55:30.257791 sdmc_adhoc_processing-0.1.47/PKG-INFO
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)       69 2024-03-01 19:56:23.000000 sdmc_adhoc_processing-0.1.47/README.md
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)     1108 2024-04-26 22:51:21.000000 sdmc_adhoc_processing-0.1.47/pyproject.toml
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)       38 2024-04-26 22:55:30.262807 sdmc_adhoc_processing-0.1.47/setup.cfg
+drwxrwxr-x   0 bhaddock (80211) staff     (1000)        0 2024-04-26 22:55:30.163816 sdmc_adhoc_processing-0.1.47/src/
+drwxrwxr-x   0 bhaddock (80211) staff     (1000)        0 2024-04-26 22:55:30.223786 sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing/
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)      313 2024-03-15 23:09:53.000000 sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing/__init__.py
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)     3197 2024-04-10 20:42:00.000000 sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing/constants.py
+-rwxrwx---   0 bhaddock (80211) staff     (1000)    12964 2024-03-22 18:48:38.000000 sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing/data_dictionary_TEMPLATE.xlsx
+-rwxrwx---   0 bhaddock (80211) staff     (1000)    10205 2024-03-22 18:52:44.000000 sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing/data_dictionary_nonstandard_vars.xlsx
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)     6654 2024-04-26 22:24:36.000000 sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing/generate_README.py
+-rwxrwx---   0 bhaddock (80211) staff     (1000)     5889 2024-04-15 18:59:57.000000 sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing/generate_dict.py
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)     9237 2024-04-11 19:14:15.000000 sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing/process.py
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)     1248 2024-04-15 20:06:25.000000 sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing/readme_template.md
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)      661 2024-04-26 22:48:45.000000 sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing/regenerate_README.py
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)      313 2024-04-10 18:40:18.000000 sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing/utilities.py
+drwxrwxr-x   0 bhaddock (80211) staff     (1000)        0 2024-04-26 22:55:30.253783 sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing.egg-info/
+-rw-r--r--   0 bhaddock (80211) staff     (1000)      619 2024-04-26 22:55:30.000000 sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing.egg-info/PKG-INFO
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)      799 2024-04-26 22:55:30.000000 sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing.egg-info/SOURCES.txt
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)        1 2024-04-26 22:55:30.000000 sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing.egg-info/dependency_links.txt
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)      214 2024-04-26 22:55:30.000000 sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing.egg-info/entry_points.txt
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)       23 2024-04-26 22:55:30.000000 sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing.egg-info/requires.txt
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)       22 2024-04-26 22:55:30.000000 sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing.egg-info/top_level.txt
+drwxrwxr-x   0 bhaddock (80211) staff     (1000)        0 2024-04-26 22:55:30.247792 sdmc_adhoc_processing-0.1.47/tests/
+-rw-rw-r--   0 bhaddock (80211) staff     (1000)      100 2024-03-01 19:54:57.000000 sdmc_adhoc_processing-0.1.47/tests/test_foo.py
```

### Comparing `sdmc_adhoc_processing-0.1.46/LICENSE` & `sdmc_adhoc_processing-0.1.47/LICENSE`

 * *Files identical despite different names*

### Comparing `sdmc_adhoc_processing-0.1.46/PKG-INFO` & `sdmc_adhoc_processing-0.1.47/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdmc_adhoc_processing
-Version: 0.1.46
+Version: 0.1.47
 Summary: Helper utilities for SDMC ad-hoc data processing requests.
 Author-email: Beatrix Haddock <beatrix.haddock@gmail.com>
 Project-URL: Homepage, https://github.com/beatrixh/sdmc-adhoc-processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `sdmc_adhoc_processing-0.1.46/pyproject.toml` & `sdmc_adhoc_processing-0.1.47/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sdmc_adhoc_processing"
-version = "0.1.46"
+version = "0.1.47"
 authors = [
   { name="Beatrix Haddock", email="beatrix.haddock@gmail.com" },
 ]
 description = "Helper utilities for SDMC ad-hoc data processing requests."
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = ["docutils", "requires <= 0.4"]
@@ -36,8 +36,9 @@
 where = ["src"]
 
 [tool.setuptools.package-data]
 "*" = ["*.*"]
 
 [project.scripts]
 gen-readme = "sdmc_adhoc_processing.generate_README:gen_README"
+regen-readme = "sdmc_adhoc_processing.regenerate_README:regen_README"
 gen-data-dict = "sdmc_adhoc_processing.generate_dict:gen_data_dict"
```

### Comparing `sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing/constants.py` & `sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing/constants.py`

 * *Files identical despite different names*

### Comparing `sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing/data_dictionary_TEMPLATE.xlsx` & `sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing/data_dictionary_TEMPLATE.xlsx`

 * *Files identical despite different names*

### Comparing `sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing/data_dictionary_nonstandard_vars.xlsx` & `sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing/data_dictionary_nonstandard_vars.xlsx`

 * *Files identical despite different names*

### Comparing `sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing/generate_README.py` & `sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing/generate_README.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # OUTPUTS:  - README.html
 #           - README.md
 ## ---------------------------------------------------------------------------##
 import markdown
 import datetime
 import pandas as pd
+import numpy as np
 import os
 import sys
 import sdmc_adhoc_processing.constants as constants
 
 # read in settings, build vars -----------------------------------------------##
 OUTPUT_DIR = sys.argv[1]
 INPUT_DATA_PATH = sys.argv[2]
@@ -31,14 +32,15 @@
 
     print("The following were found in the output dir:")
     for file in os.listdir(OUTPUT_DIR):
         print(f"   - {file}")
 
     # build dict of filepaths in output dir --------------------------------------##
     USEPATHS = {}
+    files = np.sort(os.listdir(OUTPUT_DIR))
     for file in os.listdir(OUTPUT_DIR):
         if "process" in file and ".txt" in file:
             USEPATHS["output_data"] = file
         if "dict" in file and ".xlsx" in file:
             USEPATHS["dict"] = file
         if ".py" in file and "process" in file:
             USEPATHS["code"] = file
```

### Comparing `sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing/generate_dict.py` & `sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing/generate_dict.py`

 * *Files identical despite different names*

### Comparing `sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing/process.py` & `sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing/process.py`

 * *Files identical despite different names*

### Comparing `sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing/readme_template.md` & `sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing/readme_template.md`

 * *Files identical despite different names*

### Comparing `sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing.egg-info/PKG-INFO` & `sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdmc_adhoc_processing
-Version: 0.1.46
+Version: 0.1.47
 Summary: Helper utilities for SDMC ad-hoc data processing requests.
 Author-email: Beatrix Haddock <beatrix.haddock@gmail.com>
 Project-URL: Homepage, https://github.com/beatrixh/sdmc-adhoc-processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `sdmc_adhoc_processing-0.1.46/src/sdmc_adhoc_processing.egg-info/SOURCES.txt` & `sdmc_adhoc_processing-0.1.47/src/sdmc_adhoc_processing.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/sdmc_adhoc_processing/constants.py
 src/sdmc_adhoc_processing/data_dictionary_TEMPLATE.xlsx
 src/sdmc_adhoc_processing/data_dictionary_nonstandard_vars.xlsx
 src/sdmc_adhoc_processing/generate_README.py
 src/sdmc_adhoc_processing/generate_dict.py
 src/sdmc_adhoc_processing/process.py
 src/sdmc_adhoc_processing/readme_template.md
+src/sdmc_adhoc_processing/regenerate_README.py
 src/sdmc_adhoc_processing/utilities.py
 src/sdmc_adhoc_processing.egg-info/PKG-INFO
 src/sdmc_adhoc_processing.egg-info/SOURCES.txt
 src/sdmc_adhoc_processing.egg-info/dependency_links.txt
 src/sdmc_adhoc_processing.egg-info/entry_points.txt
 src/sdmc_adhoc_processing.egg-info/requires.txt
 src/sdmc_adhoc_processing.egg-info/top_level.txt
```

