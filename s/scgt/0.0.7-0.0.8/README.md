# Comparing `tmp/scgt-0.0.7.tar.gz` & `tmp/scgt-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scgt-0.0.7.tar", last modified: Thu Apr 18 20:00:40 2024, max compression
+gzip compressed data, was "scgt-0.0.8.tar", last modified: Fri Apr 26 22:31:15 2024, max compression
```

## Comparing `scgt-0.0.7.tar` & `scgt-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 20:00:40.488186 scgt-0.0.7/
--rw-rw-rw-   0        0        0     1314 2023-09-24 05:16:05.000000 scgt-0.0.7/LICENSE.md
--rw-rw-rw-   0        0        0     3128 2024-04-18 20:00:40.433415 scgt-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      743 2023-09-24 05:16:05.000000 scgt-0.0.7/README.md
--rw-rw-rw-   0        0        0     1107 2024-04-18 19:45:15.000000 scgt-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       79 2023-09-24 05:16:05.000000 scgt-0.0.7/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-18 20:00:40.242657 scgt-0.0.7/scgt/
--rw-rw-rw-   0        0        0       41 2023-09-24 05:16:05.000000 scgt-0.0.7/scgt/__init__.py
--rw-rw-rw-   0        0        0    31983 2024-04-18 19:59:25.000000 scgt-0.0.7/scgt/scgt.py
-drwxrwxrwx   0        0        0        0 2024-04-18 20:00:40.429412 scgt-0.0.7/scgt.egg-info/
--rw-rw-rw-   0        0        0     3128 2024-04-18 20:00:39.000000 scgt-0.0.7/scgt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-04-18 20:00:40.000000 scgt-0.0.7/scgt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 20:00:39.000000 scgt-0.0.7/scgt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2024-04-18 20:00:39.000000 scgt-0.0.7/scgt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-18 20:00:39.000000 scgt-0.0.7/scgt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 20:00:40.490187 scgt-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 22:31:15.356454 scgt-0.0.8/
+-rw-rw-rw-   0        0        0     1314 2023-09-24 05:16:05.000000 scgt-0.0.8/LICENSE.md
+-rw-rw-rw-   0        0        0     3128 2024-04-26 22:31:15.353315 scgt-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      743 2023-09-24 05:16:05.000000 scgt-0.0.8/README.md
+-rw-rw-rw-   0        0        0     1107 2024-04-26 22:30:46.000000 scgt-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       79 2023-09-24 05:16:05.000000 scgt-0.0.8/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 22:31:15.251877 scgt-0.0.8/scgt/
+-rw-rw-rw-   0        0        0       41 2023-09-24 05:16:05.000000 scgt-0.0.8/scgt/__init__.py
+-rw-rw-rw-   0        0        0    32109 2024-04-26 22:27:15.000000 scgt-0.0.8/scgt/scgt.py
+drwxrwxrwx   0        0        0        0 2024-04-26 22:31:15.350611 scgt-0.0.8/scgt.egg-info/
+-rw-rw-rw-   0        0        0     3128 2024-04-26 22:31:14.000000 scgt-0.0.8/scgt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2024-04-26 22:31:15.000000 scgt-0.0.8/scgt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 22:31:15.000000 scgt-0.0.8/scgt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2024-04-26 22:31:15.000000 scgt-0.0.8/scgt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-26 22:31:15.000000 scgt-0.0.8/scgt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 22:31:15.363431 scgt-0.0.8/setup.cfg
```

### Comparing `scgt-0.0.7/LICENSE.md` & `scgt-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scgt-0.0.7/PKG-INFO` & `scgt-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scgt
-Version: 0.0.7
+Version: 0.0.8
 Summary: UC Santa Cruz Geographical Toolkit
 Author-email: Jasmine Tai <jctai@ucsc.edu>, Natalie Valett <nvalett@ucsc.edu>, Luca de Alfaro <luca@dealfaro.com>
 License: Copyright 2023, The Regents of the University of California. 
         
         Redistribution and use in source and binary forms, with or without modification, 
         are permitted provided that the following conditions are met:
```

### Comparing `scgt-0.0.7/README.md` & `scgt-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `scgt-0.0.7/pyproject.toml` & `scgt-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scgt"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
         {name="Jasmine Tai", email="jctai@ucsc.edu"},
         {name="Natalie Valett", email="nvalett@ucsc.edu"},
         {name="Luca de Alfaro", email="luca@dealfaro.com"}]
 description = "UC Santa Cruz Geographical Toolkit"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `scgt-0.0.7/scgt/scgt.py` & `scgt-0.0.8/scgt/scgt.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 import sys
 import numpy as np
 import matplotlib.pyplot as plt
 import math
 from osgeo import gdal
 import scipy.ndimage as nd
 
+# Tell GDAL to raise exceptions on errors
+gdal.UseExceptions()
+
 class GeoTiff(object):
     """A GeoTiff object provides an interface to reading/writing geotiffs in
     a tiled fashion, and to many other additional operations."""
     
     def __init__(self, file=None, memory_file=None):
         """
         Initializes a GeoTiff object.
@@ -58,15 +61,16 @@
 
     def __exit__(self, type, value, traceback):
         """Context manager exit."""
         # closes the dataset at the conclusion of a with statement
         if self.memory_file is not None:
             self.close_memory_file()
         else:
-            self.getAttributeTable()
+            if np.issubdtype(self.profile['dtype'], np.integer):
+                self.getAttributeTable()
             self.dataset.close()
 
     @classmethod
     def from_file(cls, filename):
         """
         Creates a GeoTiff object from a filename.
         :param filename: filename to open in read mode.
@@ -97,15 +101,15 @@
         # sets no_data (transparent value)
         if no_data_value is not None:
             with rasterio.open(filename, "r+") as dataset:
                 dataset.nodata = no_data_value
                 nodata_mask = np.ones((dataset.width, dataset.height)) * no_data_value
                 dataset.write(nodata_mask.astype(profile['dtype']), 1)
 
-        open_file = rasterio.open(filename, 'r+', **profile)
+        open_file = rasterio.open(filename, 'r+')
         if not open_file:
             sys.exit("GeoTiff Error: copy_to_new_file() being called with invalid Geotiff data or filepath")
         
         # return GeoTiff obj with open file
         return cls(open_file)
 
     @classmethod
```

### Comparing `scgt-0.0.7/scgt.egg-info/PKG-INFO` & `scgt-0.0.8/scgt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scgt
-Version: 0.0.7
+Version: 0.0.8
 Summary: UC Santa Cruz Geographical Toolkit
 Author-email: Jasmine Tai <jctai@ucsc.edu>, Natalie Valett <nvalett@ucsc.edu>, Luca de Alfaro <luca@dealfaro.com>
 License: Copyright 2023, The Regents of the University of California. 
         
         Redistribution and use in source and binary forms, with or without modification, 
         are permitted provided that the following conditions are met:
```

