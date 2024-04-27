# Comparing `tmp/thunderlab-1.1.0.tar.gz` & `tmp/thunderlab-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunderlab-1.1.0.tar", last modified: Wed Apr 24 09:54:28 2024, max compression
+gzip compressed data, was "thunderlab-1.2.0.tar", last modified: Sat Apr 27 15:48:56 2024, max compression
```

## Comparing `thunderlab-1.1.0.tar` & `thunderlab-1.2.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-24 09:54:28.170182 thunderlab-1.1.0/
--rw-rw-r--   0 benda     (1001) benda     (1001)    35149 2024-04-23 21:40:14.000000 thunderlab-1.1.0/LICENSE
--rw-r--r--   0 benda     (1001) benda     (1001)    45560 2024-04-24 09:54:28.170182 thunderlab-1.1.0/PKG-INFO
--rw-rw-r--   0 benda     (1001) benda     (1001)     3625 2024-04-24 09:52:26.000000 thunderlab-1.1.0/README.md
--rw-rw-r--   0 benda     (1001) benda     (1001)     1631 2024-04-23 21:40:14.000000 thunderlab-1.1.0/pyproject.toml
--rw-rw-r--   0 benda     (1001) benda     (1001)       38 2024-04-24 09:54:28.170182 thunderlab-1.1.0/setup.cfg
-drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-24 09:54:28.166182 thunderlab-1.1.0/src/
-drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-24 09:54:28.170182 thunderlab-1.1.0/src/thunderlab/
--rw-rw-r--   0 benda     (1001) benda     (1001)       80 2024-04-24 09:52:26.000000 thunderlab-1.1.0/src/thunderlab/__init__.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    13663 2024-04-23 21:40:14.000000 thunderlab-1.1.0/src/thunderlab/configfile.py
--rw-rw-r--   0 benda     (1001) benda     (1001)     3649 2024-04-23 21:40:14.000000 thunderlab-1.1.0/src/thunderlab/consoleinput.py
--rw-rw-r--   0 benda     (1001) benda     (1001)     8968 2024-04-23 21:40:14.000000 thunderlab-1.1.0/src/thunderlab/convertdata.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    66045 2024-04-23 21:40:14.000000 thunderlab-1.1.0/src/thunderlab/dataloader.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    38986 2024-04-23 21:40:14.000000 thunderlab-1.1.0/src/thunderlab/datawriter.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    50112 2024-04-23 21:40:14.000000 thunderlab-1.1.0/src/thunderlab/eventdetection.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    57140 2024-04-23 21:40:14.000000 thunderlab-1.1.0/src/thunderlab/multivariateexplorer.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    20137 2024-04-23 21:40:14.000000 thunderlab-1.1.0/src/thunderlab/powerspectrum.py
--rw-rw-r--   0 benda     (1001) benda     (1001)   112826 2024-04-23 21:40:14.000000 thunderlab-1.1.0/src/thunderlab/tabledata.py
--rw-rw-r--   0 benda     (1001) benda     (1001)      205 2024-04-24 09:53:13.000000 thunderlab-1.1.0/src/thunderlab/version.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    43812 2024-04-23 21:40:14.000000 thunderlab-1.1.0/src/thunderlab/voronoi.py
-drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-24 09:54:28.170182 thunderlab-1.1.0/src/thunderlab.egg-info/
--rw-r--r--   0 benda     (1001) benda     (1001)    45560 2024-04-24 09:54:28.000000 thunderlab-1.1.0/src/thunderlab.egg-info/PKG-INFO
--rw-rw-r--   0 benda     (1001) benda     (1001)      852 2024-04-24 09:54:28.000000 thunderlab-1.1.0/src/thunderlab.egg-info/SOURCES.txt
--rw-rw-r--   0 benda     (1001) benda     (1001)        1 2024-04-24 09:54:28.000000 thunderlab-1.1.0/src/thunderlab.egg-info/dependency_links.txt
--rw-rw-r--   0 benda     (1001) benda     (1001)       60 2024-04-24 09:54:28.000000 thunderlab-1.1.0/src/thunderlab.egg-info/entry_points.txt
--rw-rw-r--   0 benda     (1001) benda     (1001)       55 2024-04-24 09:54:28.000000 thunderlab-1.1.0/src/thunderlab.egg-info/requires.txt
--rw-rw-r--   0 benda     (1001) benda     (1001)       11 2024-04-24 09:54:28.000000 thunderlab-1.1.0/src/thunderlab.egg-info/top_level.txt
-drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-24 09:54:28.170182 thunderlab-1.1.0/tests/
--rw-rw-r--   0 benda     (1001) benda     (1001)     1384 2024-04-23 21:40:14.000000 thunderlab-1.1.0/tests/test_configfile.py
--rw-rw-r--   0 benda     (1001) benda     (1001)     1363 2024-04-23 21:40:14.000000 thunderlab-1.1.0/tests/test_consoleinput.py
--rw-rw-r--   0 benda     (1001) benda     (1001)     3780 2024-04-23 21:40:14.000000 thunderlab-1.1.0/tests/test_convertdata.py
--rw-rw-r--   0 benda     (1001) benda     (1001)     9017 2024-04-23 21:40:14.000000 thunderlab-1.1.0/tests/test_dataloader.py
--rw-rw-r--   0 benda     (1001) benda     (1001)     1708 2024-04-23 21:40:14.000000 thunderlab-1.1.0/tests/test_datawriter.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    20229 2024-04-23 21:40:14.000000 thunderlab-1.1.0/tests/test_eventdetection.py
--rw-rw-r--   0 benda     (1001) benda     (1001)     5738 2024-04-23 21:40:14.000000 thunderlab-1.1.0/tests/test_powerspectrum.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    14927 2024-04-23 21:40:14.000000 thunderlab-1.1.0/tests/test_tabledata.py
--rw-rw-r--   0 benda     (1001) benda     (1001)     3671 2024-04-23 21:40:14.000000 thunderlab-1.1.0/tests/test_voronoi.py
+drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-27 15:48:56.869375 thunderlab-1.2.0/
+-rw-rw-r--   0 benda     (1001) benda     (1001)    35149 2024-04-23 21:40:14.000000 thunderlab-1.2.0/LICENSE
+-rw-r--r--   0 benda     (1001) benda     (1001)    45604 2024-04-27 15:48:56.869375 thunderlab-1.2.0/PKG-INFO
+-rw-rw-r--   0 benda     (1001) benda     (1001)     3669 2024-04-27 15:48:07.000000 thunderlab-1.2.0/README.md
+-rw-rw-r--   0 benda     (1001) benda     (1001)     1693 2024-04-27 15:48:07.000000 thunderlab-1.2.0/pyproject.toml
+-rw-rw-r--   0 benda     (1001) benda     (1001)       38 2024-04-27 15:48:56.869375 thunderlab-1.2.0/setup.cfg
+drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-27 15:48:56.837374 thunderlab-1.2.0/src/
+drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-27 15:48:56.865375 thunderlab-1.2.0/src/thunderlab/
+-rw-rw-r--   0 benda     (1001) benda     (1001)       80 2024-04-24 09:52:26.000000 thunderlab-1.2.0/src/thunderlab/__init__.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    13663 2024-04-23 21:40:14.000000 thunderlab-1.2.0/src/thunderlab/configfile.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     3649 2024-04-23 21:40:14.000000 thunderlab-1.2.0/src/thunderlab/consoleinput.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     8968 2024-04-23 21:40:14.000000 thunderlab-1.2.0/src/thunderlab/convertdata.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    66045 2024-04-23 21:40:14.000000 thunderlab-1.2.0/src/thunderlab/dataloader.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    38986 2024-04-23 21:40:14.000000 thunderlab-1.2.0/src/thunderlab/datawriter.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    50112 2024-04-23 21:40:14.000000 thunderlab-1.2.0/src/thunderlab/eventdetection.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    68697 2024-04-27 15:48:07.000000 thunderlab-1.2.0/src/thunderlab/multivariateexplorer.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    20137 2024-04-23 21:40:14.000000 thunderlab-1.2.0/src/thunderlab/powerspectrum.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)   113968 2024-04-27 15:48:07.000000 thunderlab-1.2.0/src/thunderlab/tabledata.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)      205 2024-04-27 15:48:07.000000 thunderlab-1.2.0/src/thunderlab/version.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    43812 2024-04-23 21:40:14.000000 thunderlab-1.2.0/src/thunderlab/voronoi.py
+drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-27 15:48:56.865375 thunderlab-1.2.0/src/thunderlab.egg-info/
+-rw-r--r--   0 benda     (1001) benda     (1001)    45604 2024-04-27 15:48:56.000000 thunderlab-1.2.0/src/thunderlab.egg-info/PKG-INFO
+-rw-rw-r--   0 benda     (1001) benda     (1001)      887 2024-04-27 15:48:56.000000 thunderlab-1.2.0/src/thunderlab.egg-info/SOURCES.txt
+-rw-rw-r--   0 benda     (1001) benda     (1001)        1 2024-04-27 15:48:56.000000 thunderlab-1.2.0/src/thunderlab.egg-info/dependency_links.txt
+-rw-rw-r--   0 benda     (1001) benda     (1001)      120 2024-04-27 15:48:56.000000 thunderlab-1.2.0/src/thunderlab.egg-info/entry_points.txt
+-rw-rw-r--   0 benda     (1001) benda     (1001)       55 2024-04-27 15:48:56.000000 thunderlab-1.2.0/src/thunderlab.egg-info/requires.txt
+-rw-rw-r--   0 benda     (1001) benda     (1001)       11 2024-04-27 15:48:56.000000 thunderlab-1.2.0/src/thunderlab.egg-info/top_level.txt
+drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-27 15:48:56.865375 thunderlab-1.2.0/tests/
+-rw-rw-r--   0 benda     (1001) benda     (1001)     1384 2024-04-23 21:40:14.000000 thunderlab-1.2.0/tests/test_configfile.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     1363 2024-04-23 21:40:14.000000 thunderlab-1.2.0/tests/test_consoleinput.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     3780 2024-04-23 21:40:14.000000 thunderlab-1.2.0/tests/test_convertdata.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     9017 2024-04-23 21:40:14.000000 thunderlab-1.2.0/tests/test_dataloader.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     1708 2024-04-23 21:40:14.000000 thunderlab-1.2.0/tests/test_datawriter.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    20229 2024-04-23 21:40:14.000000 thunderlab-1.2.0/tests/test_eventdetection.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     2337 2024-04-25 07:51:35.000000 thunderlab-1.2.0/tests/test_multivariateexplorer.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     5738 2024-04-23 21:40:14.000000 thunderlab-1.2.0/tests/test_powerspectrum.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    14927 2024-04-23 21:40:14.000000 thunderlab-1.2.0/tests/test_tabledata.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     3671 2024-04-23 21:40:14.000000 thunderlab-1.2.0/tests/test_voronoi.py
```

### Comparing `thunderlab-1.1.0/LICENSE` & `thunderlab-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thunderlab-1.1.0/PKG-INFO` & `thunderlab-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thunderlab
-Version: 1.1.0
+Version: 1.2.0
 Summary: Algorithms and scripts for analyzing recordings of electric fish waveforms.
 Author: Jörg Henninger, Jan Grewe, Fabian Sinz
 Author-email: Jan Benda <jan.benda@uni-tuebingen.de>
 Maintainer-email: Jan Benda <jan.benda@uni-tuebingen.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -744,15 +744,15 @@
 
 
 ## Software
 
 The ThunderLab package provides the following software:
 
 - [`convertdata`](https://bendalab.github.io/thunderlab/api/convertdata/): Convert data from various file formats to audio files.
-
+- [`multivariateexplorer`](https://bendalab.github.io/thunderlab/api/multivariateexplorer.html): Simple GUI for viewing and exploring multivariate data. [More](docs/multivariateexplorer/index.html)
 
 
 ## Algorithms
 
 Click on the modules for more information.
 
 ### Input/output
@@ -764,15 +764,14 @@
 - [`consoleinput`](https://bendalab.github.io/thunderlab/api/consoleinput.html): User input from console.
 
 ### Basic data analysis
 
 - [`eventdetection`](https://bendalab.github.io/thunderlab/api/eventdetection.html): Detect and hande peaks and troughs as well as threshold crossings in data arrays.
 - [`powerspectrum`](https://bendalab.github.io/thunderlab/api/powerspectrum.html): Compute and plot powerspectra and spectrograms for a given minimum frequency resolution.
 - [`voronoi`](https://bendalab.github.io/thunderlab/api/voronoi.html): Analyse Voronoi diagrams based on scipy.spatial.
-- [`multivariateexplorer`](https://bendalab.github.io/thunderlab/api/multivariateexplorer.html): Simple GUI for viewing and exploring multivariate data.
 
 
 ## Used by
 
 - [thunderfish](https://github.com/bendalab/thunderfish): Algorithms and programs for analysing electric field recordings of weakly electric fish.
 - [audian](https://github.com/bendalab/audian) Python-based GUI for
 viewing and analyzing recordings of animal vocalizations.
```

### Comparing `thunderlab-1.1.0/README.md` & `thunderlab-1.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 ## Software
 
 The ThunderLab package provides the following software:
 
 - [`convertdata`](https://bendalab.github.io/thunderlab/api/convertdata/): Convert data from various file formats to audio files.
-
+- [`multivariateexplorer`](https://bendalab.github.io/thunderlab/api/multivariateexplorer.html): Simple GUI for viewing and exploring multivariate data. [More](docs/multivariateexplorer/index.html)
 
 
 ## Algorithms
 
 Click on the modules for more information.
 
 ### Input/output
@@ -56,15 +56,14 @@
 - [`consoleinput`](https://bendalab.github.io/thunderlab/api/consoleinput.html): User input from console.
 
 ### Basic data analysis
 
 - [`eventdetection`](https://bendalab.github.io/thunderlab/api/eventdetection.html): Detect and hande peaks and troughs as well as threshold crossings in data arrays.
 - [`powerspectrum`](https://bendalab.github.io/thunderlab/api/powerspectrum.html): Compute and plot powerspectra and spectrograms for a given minimum frequency resolution.
 - [`voronoi`](https://bendalab.github.io/thunderlab/api/voronoi.html): Analyse Voronoi diagrams based on scipy.spatial.
-- [`multivariateexplorer`](https://bendalab.github.io/thunderlab/api/multivariateexplorer.html): Simple GUI for viewing and exploring multivariate data.
 
 
 ## Used by
 
 - [thunderfish](https://github.com/bendalab/thunderfish): Algorithms and programs for analysing electric field recordings of weakly electric fish.
 - [audian](https://github.com/bendalab/audian) Python-based GUI for
 viewing and analyzing recordings of animal vocalizations.
```

### Comparing `thunderlab-1.1.0/pyproject.toml` & `thunderlab-1.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -45,13 +45,14 @@
 
 [project.urls]
 Repository    = "https://github.com/bendalab/thunderlab"
 Documentation = "https://bendalab.github.io/thunderlab"
 
 [project.scripts]
 convertdata = "thunderlab.convertdata:main"
+multivariateexplorer = "thunderlab.multivariateexplorer:main"
 
 [tool.setuptools.dynamic]
 version = {attr = "thunderlab.version.__version__"}
 
 [tool.pytest.ini_options]
 pythonpath = "src"
```

### Comparing `thunderlab-1.1.0/src/thunderlab/configfile.py` & `thunderlab-1.2.0/src/thunderlab/configfile.py`

 * *Files identical despite different names*

### Comparing `thunderlab-1.1.0/src/thunderlab/consoleinput.py` & `thunderlab-1.2.0/src/thunderlab/consoleinput.py`

 * *Files identical despite different names*

### Comparing `thunderlab-1.1.0/src/thunderlab/convertdata.py` & `thunderlab-1.2.0/src/thunderlab/convertdata.py`

 * *Files identical despite different names*

### Comparing `thunderlab-1.1.0/src/thunderlab/dataloader.py` & `thunderlab-1.2.0/src/thunderlab/dataloader.py`

 * *Files identical despite different names*

### Comparing `thunderlab-1.1.0/src/thunderlab/datawriter.py` & `thunderlab-1.2.0/src/thunderlab/datawriter.py`

 * *Files identical despite different names*

### Comparing `thunderlab-1.1.0/src/thunderlab/eventdetection.py` & `thunderlab-1.2.0/src/thunderlab/eventdetection.py`

 * *Files identical despite different names*

### Comparing `thunderlab-1.1.0/src/thunderlab/multivariateexplorer.py` & `thunderlab-1.2.0/src/thunderlab/multivariateexplorer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """Simple GUI for viewing and exploring multivariate data.
 
 - `class MultiVariateExplorer`: simple matplotlib-based GUI for viewing and exploring multivariate data.
 - `categorize()`: convert categorial string data into integer categories.
+- `select_features()`: assemble list of column indices.
+- `select_coloring()`: select column from data table for colorizing the data.
+- `list_available_features()`: print available features on console.
 """
 
+import sys
 import numpy as np
+from scipy.stats import pearsonr
 from sklearn import decomposition
 from sklearn import preprocessing
 import matplotlib.pyplot as plt
 import matplotlib.patches as patches
 import matplotlib.widgets as widgets
 import argparse
 from .version import __version__, __year__
@@ -40,157 +45,187 @@
     - fix_scatter_plot()
     - fix_waveform_plot()
     - list_selection()
     - analyze_selection()
     See the documentation of these functions for details.
     """
 
-    mouse_actions = (('left click', 'select data points'),
-                     ('left and drag', 'rectangular selection and zoom of data points'),
-                     ('shift + left click/drag', 'add data points to selection'),
-                     ('ctrl + left click/drag',  'remove data points from selection'))
+    mouse_actions = [
+        ('left click', 'select sample'),
+        ('left and drag', 'rectangular selection of samples and/or zoom'),
+        ('shift + left click/drag', 'add samples to selection'),
+        ('ctrl + left click/drag',  'remove samples from selection')
+    ]
+    """List of tuples with mouse actions and a description of their action."""
         
-    key_actions = (('l', 'list selected EOD waveforms on console'),
-                   ('p,P', 'toggle between data columns, PC, and scaled PC axis'),
-                   ('<, pageup', 'decrease number of displayed data columns/PC axis'),
-                   ('>, pagedown', 'increase number of displayed data columns/PC axis'),
-                   ('w',  'toggle maximized waveform plot'),
-                   ('o, z',  'toggle zoom mode on or off'),
-                   ('backspace', 'zoom back'),
-                   ('ctrl + a', 'select all'),
-                   ('+, -', 'increase, decrease pick radius'),
-                   ('0', 'reset pick radius'),
-                   ('n, N', 'decrease, increase number of bins of histograms'),
-                   ('h', 'toggle between scatter plot and 2D histogram'),
-                   ('c, C', 'cycle color map trough data columns'),
-                   ('left, right, up, down', 'show and move magnified scatter plot'),
-                   ('escape', 'close magnified scatter plot'))
+    key_actions = [
+        ('c, C', 'cycle color map trough data columns'),
+        ('p,P', 'toggle between features, PCs, and scaled PCs'),
+        ('<, pageup', 'decrease number of displayed featured/PCs'),
+        ('>, pagedown', 'increase number of displayed features/PCs'),
+        ('o, z',  'toggle zoom mode on or off'),
+        ('backspace', 'zoom back'),
+        ('n, N', 'decrease, increase number of bins of histograms'),
+        ('H', 'toggle between scatter plot and 2D histogram'),
+        ('left, right, up, down', 'show and move magnified scatter plot'),
+        ('escape', 'close magnified scatter plot'),
+        ('ctrl + a', 'select all'),
+        ('+, -', 'increase, decrease pick radius'),
+        ('0', 'reset pick radius'),
+        ('l', 'list selection on console'),
+        ('w',  'toggle maximized waveform plot'),
+        ('h',  'toggle help window'),
+    ]
+    """List of tuples with key shortcuts and a description of their action."""
     
     def __init__(self, data, labels=None, title=None):
         """Initialize explorer with scatter-plot data.
 
         Parameters
         ----------
         data: TableData, 2D array, or list of 1D arrays
             The data to be explored. Each column is a variable.
             For the 2D array the columns are the second dimension,
             for a list of 1D arrays, the list goes over columns,
             i.e. each 1D array is one column.
-        labels: list of string
+        labels: list of str
             If data is not a TableData, then this provides labels
             for the data columns.
-        title: string
+        title: str
             Title for the window.
         """
-        # data and labels:
+        # data. categories and labels:
+        self.raw_data = None     # original data table as 2D numpy array (samples x features)
+        self.raw_labels = None   # for each feature a label, optional with unit
+        self.categories = []     # for each feature None or list of categories
         if isinstance(data, TableData):
-            self.categories = []
             for c, col in enumerate(data):
                 if not isinstance(col[0], (int, float,
                                            np.integer, np.floating)):
                     # categorial data:
+                    #print(data[:,c])
                     cats, data[:,c] = categorize(col)
                     self.categories.append(cats)
                 else:
                     self.categories.append(None)
             self.raw_data = data.array()
             if labels is None:
                 self.raw_labels = []
                 for c in range(len(data)):
                     if len(data.unit(c)) > 0 and not data.unit(c) in ['-', '1']:
-                        self.raw_labels.append('%s [%s]' % (data.label(c), data.unit(c)))
+                        self.raw_labels.append(f'{data.label(c)} [{data.unit(c)}]')
                     else:
                         self.raw_labels.append(data.label(c))
             else:
                 self.raw_labels = labels
         else:
             if isinstance(data, np.ndarray):
                 self.raw_data = data
+                self.categories = [None] * data.shape[1]
             else:
-                self.categories = []
                 for c, col in enumerate(data):
                     if not isinstance(col[0], (int, float,
                                                np.integer, np.floating)):
                         # categorial data:
                         cats, data[c] = categorize(col)
                         self.categories.append(cats)
                     else:
                         self.categories.append(None)
                 self.raw_data = np.asarray(data).T
             self.raw_labels = labels
+        # remove columns containing only invalid numbers:
+        cols = np.all(~np.isfinite(self.raw_data), 0)
+        if np.sum(cols) > 0:
+            print('removed columns containing no numbers:',
+                  [l for l, c in zip(self.raw_labels, cols) if c])
+        self.raw_data = self.raw_data[:, ~cols]
+        self.raw_labels = [l for l, c in zip(self.raw_labels, cols) if not c]
+        # remove rows containing invalid numbers:
+        self.valid_samples = ~np.any(~np.isfinite(self.raw_data), 1)
+        self.raw_data = self.raw_data[self.valid_samples, :]
+        if np.sum(~self.valid_samples) > 0:
+            print(f'removed {np.sum(~self.valid_samples)} rows containing invalid numbers:')
+            for k in range(len(self.valid_samples)):
+                if not self.valid_samples[k]:
+                    print(k)
+        self.valid_rows = [k for k in range(len(self.valid_samples))
+                           if self.valid_samples[k]]
+        # title for the window:
         self.title = title if title is not None else 'MultivariateExplorer'
-        # no pca data yet:
+        # data, pca-data, scaled-pca data (no pca data yet):
         self.all_data = [self.raw_data, None, None]
         self.all_labels = [self.raw_labels, None, None]
         self.all_maxcols = [self.raw_data.shape[1], None, None]
-        self.all_titles = ['data', 'PCA', 'scaled PCA']
+        self.all_titles = ['data', 'PCA', 'scaled PCA'] # added to window title 
         # pca:
-        self.pca_tables = [None, None]
-        self._pca_header(data, labels)
+        self.pca_tables = [None, None]  # raw and scaled pca coefficients
+        self._pca_header(self.raw_data, self.raw_labels)  # prepare header of the pca tables
         # start showing raw data:
-        self.show_mode = 0
-        self.data = self.all_data[self.show_mode]
-        self.labels = self.all_labels[self.show_mode]
-        self.maxcols = self.all_maxcols[self.show_mode]
+        self.show_mode = 0                       # show data, pca or scaled pca
+        self.data = self.all_data[self.show_mode]       # the data shown
+        self.labels = self.all_labels[self.show_mode]   # the feature labels shown
+        self.maxcols = self.all_maxcols[self.show_mode] # maximum number of features currently shown
         if self.maxcols > 6:
             self.maxcols = 6
         # waveform data:
         self.wave_data = []
         self.wave_nested = False
         self.wave_has_xticks = []
         self.wave_xlabels = []
         self.wave_ylabels = []
         self.wave_title = False
         # colors:
         self.color_map = plt.get_cmap('jet')
-        self.extra_colors = None
-        self.extra_color_label = None
-        self.extra_categories = None
-        self.color_values = None
-        self.color_set_index = 0
-        self.color_index = 0
-        self.color_label = None
-        self.color_set_index = 0
-        self.color_index = 0
-        self.data_colors = None
+        self.extra_colors = None         # additional data column to be used for coloring
+        self.extra_color_label = None    # label for extra_colors
+        self.extra_categories = None     # category name for extra_colors if needed
+        self.color_set_index = 0         # -1: rows and extra_colors, 0: data, 1: pca, 2: scaled pca
+        self.color_index = 0             # column used for coloring with color_set_index
+        self.color_values = None         # data column currently used for coloring as specified by color_set_index and color_index
+        self.color_label = None          # label of data currently used for coloring
+        self.data_colors = None          # actual colors for color_values
         self.color_vmin = None
         self.color_vmax = None
         self.color_ticks = None
-        self.cbax = None
+        self.cbax = None                 # axes of color bar
         # figure variables:
         self.plt_params = {}
         for k in ['toolbar', 'keymap.quit', 'keymap.back', 'keymap.forward',
                   'keymap.zoom', 'keymap.pan', 'keymap.xscale', 'keymap.yscale']:
             self.plt_params[k] = plt.rcParams[k]
             if k != 'toolbar':
                 plt.rcParams[k] = ''
-        self.xborder = 70.0  # pixel for ylabels
-        self.yborder = 50.0  # pixel for xlabels
-        self.spacing = 10.0  # pixel between plots
+        self.xborder = 100.0       # pixel for ylabels
+        self.yborder = 50.0        # pixel for xlabels
+        self.spacing = 10.0        # pixel between plots
+        self.mborder = 20.0        # pixel around magnified plot
         self.pick_radius = 4.0
         # histogram plots:
-        self.hist_ax = []
-        self.hist_indices = []
-        self.hist_selector = []
-        self.hist_nbins = 30
+        self.hist_ax = []          # list of histogram axes
+        self.hist_indices = []     # feature index of the histogram axes
+        self.hist_selector = []    # for each histogram axes a selector
+        self.hist_nbins = 30       # number of bins for computing histograms
         # scatter plots:
-        self.scatter_ax = []
-        self.scatter_indices = []
-        self.scatter_artists = []
-        self.scatter_selector = []
-        self.scatter = True
-        self.mark_data = []
+        self.scatter_ax = []       # list of axes with scatter plots (1D)
+        self.scatter_indices = []  # for each axes a tuple of the column and row index
+        self.scatter_artists = []  # artists of selected scatter points
+        self.scatter_selector = [] # selector for each axes
+        self.scatter = True        # scatter (True) or density (False)
+        self.mark_data = []        # list of indices of selected data
+        self.significance_level = 0.05 # r is bold if p is below
         self.select_zooms = False
         self.zoom_stack = []
         # magnified scatter plot:
         self.magnified_on = False
         self.magnified_backdrop = None
-        self.magnified_size = np.array([0.5, 0.5])
+        self.magnified_size = np.array([0.6, 0.6])
         # waveform plots:
         self.wave_ax = []
+        # help window:
+        self.help_ax = None
 
 
     def set_wave_data(self, data, xlabels='', ylabels=[], title=False):
         """Add waveform data to explorer.
 
         Parameters
         ----------
@@ -199,22 +234,22 @@
             Elements of the outer list correspond to the rows of the data.
             The inner 2D arrays contain a common x-axes (first column)
             and one or more corresponding y-values (second and optional higher columns).
             Each column for y-values is plotted in its own axes on top of each other,
             from top to bottom.
             The optional inner list of 2D arrays contains several 2D arrays as ascribed above
             each with its own common x-axes.
-        xlabel: string or list of strings
+        xlabel: str or list of str
             The xlabels for the waveform plots. If only a string is given, then
             there will be a common xaxis for all the plots, and only the lowest
             one gets a labeled xaxis. If a list of strings is given, each waveform
             plot gets its own labeled x-axis.
-        ylabels: list of strings
+        ylabels: list of str
             The ylabels for each of the waveform plots.
-        title: bool or string
+        title: bool or str
             If True or a string, povide space on top of the waveform plots for a title.
             If string, set this as the title for the waveform plots.
         """
         self.wave_data = []
         if data is not None and len(data) > 0:
             self.wave_data = data
             self.wave_has_xticks = []
@@ -242,18 +277,18 @@
         
         Parameters
         ----------
         colors: int or 1D array
            Index to colum in data to be used for coloring scatter plots.
            -2 for coloring row index of data.
            Or data array used to color scalar plots.
-        color_label: string
+        color_label: str
            If colors is an array, this is a label describing the data.
            It is used to label the color bar.
-        color_map: string or None
+        color_map: str or None
             Name of a matplotlib color map.
             If None 'jet' is used.
         """
         if isinstance(colors, (np.integer, int)):
             if colors < 0:
                 self.color_set_index = -1
                 self.color_index = 0
@@ -263,81 +298,89 @@
         else:
             if not isinstance(colors[0], (int, float,
                                           np.integer, np.floating)):
                 # categorial data:
                 self.extra_categories, self.extra_colors = categorize(colors)
             else:
                 self.extra_colors = colors
+            self.extra_colors = self.extra_colors[self.valid_samples]
             self.extra_color_label = color_label
             self.color_set_index = -1
             self.color_index = 1
         self.color_map = plt.get_cmap(color_map if color_map else 'jet')
 
         
-    def show(self):
+    def show(self, ioff=True):
         """Show interactive scatter plots for exploration.
         """
-        plt.ioff()
+        if ioff:
+            plt.ioff()
+        else:
+            plt.ion()
         plt.rcParams['toolbar'] = 'None'
-        plt.rcParams['keymap.quit'] = 'ctrl+w, alt+q, q'
-        self.fig = plt.figure(facecolor='white')
+        plt.rcParams['keymap.quit'] = 'ctrl+w, alt+q, ctrl+q, q'
+        plt.rcParams['font.size'] = 12
+        self.fig = plt.figure(facecolor='white', figsize=(10, 8))
         self.fig.canvas.manager.set_window_title(self.title + ': ' + self.all_titles[self.show_mode])
         self.fig.canvas.mpl_connect('key_press_event', self._on_key)
         self.fig.canvas.mpl_connect('resize_event', self._on_resize)
         self.fig.canvas.mpl_connect('pick_event', self._on_pick)
         if self.color_map is None:
             self.color_map = plt.get_cmap('jet')
         self._set_color_column()
         self._init_hist_plots()
         self._init_scatter_plots()
         self.wave_ax = []
         if self.wave_data is not None and len(self.wave_data) > 0:
             axx = None
             xi = 0
             for k, has_xticks in enumerate(self.wave_has_xticks):
-                ax = self.fig.add_subplot(1, len(self.wave_has_xticks), 1+k, sharex=axx)
+                ax = self.fig.add_subplot(1, len(self.wave_has_xticks),
+                                          1+k, sharex=axx)
                 self.wave_ax.append(ax)
                 if has_xticks:
                     if xi >= len(self.wave_xlabels):
                         self.wave_xlabels.append('')
                     ax.set_xlabel(self.wave_xlabels[xi])
                     xi += 1
                     axx = None
                 else:
-                    plt.setp(ax.get_xticklabels(), visible=False)
+                    #ax.xaxis.set_major_formatter(plt.NullFormatter())
                     if axx is None:
                         axx = ax
             for ax, ylabel in zip(self.wave_ax, self.wave_ylabels):
                 ax.set_ylabel(ylabel)
             if not isinstance(self.wave_title, bool) and self.wave_title:
                 self.wave_ax[0].set_title(self.wave_title)
             self.fix_waveform_plot(self.wave_ax, self.mark_data)
         self._plot_magnified_scatter()
+        self._plot_help()
         plt.show()
 
 
     def _pca_header(self, data, labels):
-        """Set up header for the table of principal components. """
-        if isinstance(data, TableData):
-            header = data.table_header()
-            for c in reversed(range(data.columns())):
-                if not np.all(np.isfinite(data[:,c])):
-                    header.remove(c)
-        else:
-            lbs = []
-            for l, d in zip(labels, data):
-                if not np.all(np.isfinite(d)):
-                    continue
-                if '[' in l:
-                    lbs.append(l.split('[')[0].strip())
-                elif '/' in l:
-                    lbs.append(l.split('/')[0].strip())
-                else:
-                    lbs.append(l)
-            header = TableData(header=lbs)
+        """Set up header for the table of principal components.
+
+        Parameters
+        ----------
+        data: ndarray of float
+            The data (samples x features) without invalid (infinite or
+            NaN) numbers.
+        labels: list of str
+            Labels of the features.
+        """
+        lbs = []
+        for l, d in zip(labels, data):
+            if '[' in l:
+                lbs.append(l.split('[')[0].strip())
+            elif '/' in l:
+                lbs.append(l.split('/')[0].strip())
+            else:
+                lbs.append(l)
+        header = TableData(header=lbs)
         header.set_formats('%.3f')
         header.insert(0, ['PC'] + ['-']*header.nsecs, '', '%d')
         header.insert(1, 'variance', '%', '%.3f')
         for k in range(len(self.pca_tables)):
             self.pca_tables[k] = TableData(header)
 
                 
@@ -348,32 +391,29 @@
         ----------
         scale: boolean
             If True standardize data before computing PCA, i.e. remove mean
             of each variabel and divide by its standard deviation.
         write: boolean
             If True write PCA components to standard out.
         """
-        # select columns without NANs:
-        idxs = [i for i in range(self.raw_data.shape[1]) if np.all(np.isfinite(self.raw_data[:,i]))]
-        data = self.raw_data[:,idxs]
         # pca:
         pca = decomposition.PCA()
         if scale:
             scaler = preprocessing.StandardScaler()
-            scaler.fit(data)
-            pca.fit(scaler.transform(data))
+            scaler.fit(self.raw_data)
+            pca.fit(scaler.transform(self.raw_data))
             pca_label = 'sPC'
         else:
-            pca.fit(data)
+            pca.fit(self.raw_data)
             pca_label = 'PC'
         for k in range(len(pca.components_)):
             if np.abs(np.min(pca.components_[k])) > np.max(pca.components_[k]):
                 pca.components_[k] *= -1.0
-        pca_data = pca.transform(data)
-        pca_labels = [('%s%d (%.1f%%)' if v > 0.01 else '%s%d (%.2f%%)') % (pca_label, k+1, 100.0*v)
+        pca_data = pca.transform(self.raw_data)
+        pca_labels = [f'{pca_label}{k+1} ' + (f'({100*v:.1f}%)' if v > 0.01 else (f'{100*v:.2f}%'))
                            for k, v in enumerate(pca.explained_variance_ratio_)]
         if np.min(pca.explained_variance_ratio_) >= 0.01:
             pca_maxcols = pca_data.shape[1]
         else:
             pca_maxcols = np.argmax(pca.explained_variance_ratio_ < 0.01)
         if pca_maxcols < 2:
             pca_maxcols = 2
@@ -401,15 +441,15 @@
 
             
     def save_pca(self, file_name, scale, **kwargs):
         """Write PCA data to file.
 
         Parameters
         ----------
-        file_name: string
+        file_name: str
             Name of ouput file.
         scale: boolean
             If True write PCA components of standardized PCA.
         kwargs: dict
             Additional parameter for TableData.write()
         """
         if scale:
@@ -428,226 +468,291 @@
 
             
     def _set_color_column(self):
         """Initialize variables used for colorization of scatter points."""
         if self.color_set_index == -1:
             if self.color_index == 0:
                 self.color_values = np.arange(self.data.shape[0], dtype=float)
-                self.color_label = 'row'
+                self.color_label = 'sample'
             elif self.color_index == 1:
                 self.color_values = self.extra_colors
                 self.color_label = self.extra_color_label
         else:
             self.color_values = self.all_data[self.color_set_index][:,self.color_index]
             self.color_label = self.all_labels[self.color_set_index][self.color_index]
         self.color_vmin, self.color_vmax, self.color_ticks = \
-          self.fix_scatter_plot(self.cbax, self.color_values, self.color_label, 'c')
+          self.fix_scatter_plot(self.cbax, self.color_values,
+                                self.color_label, 'c')
         if self.color_ticks is None:
             if self.color_set_index == 0 and \
                self.categories[self.color_index] is not None:
                 self.color_ticks = np.arange(len(self.categories[self.color_index]))
             elif self.color_set_index == -1 and \
                  self.color_index == 1 and \
                  self.extra_categories is not None:
                 self.color_ticks = np.arange(len(self.extra_categories))
         self.data_colors = self.color_map((self.color_values - self.color_vmin)/(self.color_vmax - self.color_vmin))
 
+
+    def _add_backdrop(self, ax):
+        bbox = ax.get_tightbbox(self.fig.canvas.get_renderer())
+        if bbox is not None:
+            self.magnified_backdrop = \
+                patches.Rectangle((bbox.x0 - self.mborder,
+                                   bbox.y0 - self.mborder),
+                                  bbox.width + 2*self.mborder,
+                                  bbox.height + 2*self.mborder,
+                                  transform=None, clip_on=False,
+                                  facecolor='#f7f7f7', edgecolor='none',
+                                  zorder=-5)
+            ax.add_patch(self.magnified_backdrop)
+
+            
+    def _create_selector(self, ax):
+        try:
+            selector = \
+                widgets.RectangleSelector(ax, self._on_select,
+                                          useblit=True, button=1,
+                                          minspanx=0, minspany=0,
+                                          spancoords='pixels',
+                                          props=dict(facecolor='gray',
+                                                     edgecolor='gray',
+                                                     alpha=0.2,
+                                                     fill=True),
+                                          state_modifier_keys=dict(move='',
+                                                                   clear='',
+                                                                   square='',
+                                                                   center='ctrl'))
+        except TypeError:
+            # old matplotlib:
+            selector = widgets.RectangleSelector(ax, self._on_select,
+                                                 useblit=True, button=1)
+        return selector
+    
                             
-    def _plot_hist(self, ax, magnifiedax, keep_lims):
+    def _plot_hist(self, ax, magnifiedax):
         """Plot and label a histogram."""
-        ax_xlim = ax.get_xlim()
-        ax_ylim = ax.get_ylim()
         try:
             idx = self.hist_ax.index(ax)
             c = self.hist_indices[idx]
             in_hist = True
         except ValueError:
             idx = self.scatter_ax.index(ax)
-            c = self.scatter_indices[-1][0]
+            c = self.scatter_indices[idx][0]
             in_hist = False
         ax.clear()
-        ax.relim()
-        ax.autoscale(True)
+        #ax.relim()
+        #ax.autoscale(True)
         x = self.data[:,c]
-        ax.hist(x[np.isfinite(x)], self.hist_nbins)
+        ax.hist(x, self.hist_nbins)
+        #ax.autoscale(False)
         ax.set_xlabel(self.labels[c])
-        if self.categories[c] is not None:
-            ax.set_xticks(np.arange(len(self.categories[c])))
-            ax.set_xticklabels(self.categories[c])
-        self.fix_scatter_plot(ax, self.data[:,c], self.labels[c], 'x')
+        ax.xaxis.set_major_locator(plt.AutoLocator())
+        ax.xaxis.set_major_formatter(plt.ScalarFormatter())
+        if self.show_mode == 0:
+            if self.categories[c] is not None:
+                ax.set_xticks(np.arange(len(self.categories[c])))
+                ax.set_xticklabels(self.categories[c])
+            self.fix_scatter_plot(ax, self.data[:,c], self.labels[c], 'x')
         if magnifiedax:
+            ax.text(0.05, 0.9, f'n={len(self.data)}',
+                    transform=ax.transAxes, zorder=100)
             ax.set_ylabel('count')
             cax = self.hist_ax[self.scatter_indices[-1][0]]
             ax.set_xlim(cax.get_xlim())
         else:
             if c == 0:
+                ax.text(0.05, 0.9, f'n={len(self.data)}',
+                        transform=ax.transAxes, zorder=100)
                 ax.set_ylabel('count')
             else:
-                plt.setp(ax.get_yticklabels(), visible=False)
-        if keep_lims:
-            ax.set_xlim(*ax_xlim)
-            ax.set_ylim(*ax_ylim)
-        try:
-            selector = widgets.RectangleSelector(ax, self._on_select, useblit=True, button=1,
-                                                 props=dict(facecolor='gray', edgecolor='gray', alpha=0.2, fill=True),
-                                                 state_modifier_keys=dict(move='', clear='', square='', center=''))
-        except TypeError:
-            selector = widgets.RectangleSelector(ax, self._on_select, useblit=True, button=1)
+                ax.yaxis.set_major_formatter(plt.NullFormatter())
+        selector = self._create_selector(ax)
         if in_hist:
             self.hist_selector[idx] = selector
         else:
             self.scatter_selector[idx] = selector
             self.scatter_artists[idx] = None
+        ax.relim(True)
         if magnifiedax:
-            bbox = ax.get_tightbbox(self.fig.canvas.get_renderer())
-            if bbox is not None:
-                self.magnified_backdrop = patches.Rectangle((bbox.x0, bbox.y0),
-                                                            bbox.width, bbox.height,
-                                                            transform=None, clip_on=False,
-                                                            facecolor='white', edgecolor='none', zorder=-5)
-                ax.add_patch(self.magnified_backdrop)
+            self._add_backdrop(ax)
+            
+
+    def _set_hist_ylim(self):
+        ymax = np.max([ax.get_ylim() for ax in self.hist_ax[:self.maxcols]], 0)[1]
+        for ax in self.hist_ax:
+            ax.set_ylim(0, ymax)
 
                         
     def _init_hist_plots(self):
         """Initial plots of the histograms."""
         n = self.data.shape[1]
-        yax = None
         self.hist_ax = []
         for r in range(n):
-            ax = self.fig.add_subplot(n, n, (n-1)*n+r+1, sharey=yax)
+            ax = self.fig.add_subplot(n, n, (n-1)*n+r+1)
             self.hist_ax.append(ax)
             self.hist_indices.append(r)
             self.hist_selector.append(None)
-            self._plot_hist(ax, False, False)
-            yax = ax
+            self._plot_hist(ax, False)
+        self._set_hist_ylim()
 
                         
-    def _plot_scatter(self, ax, magnifiedax, keep_lims, cax=None):
+    def _plot_scatter(self, ax, magnifiedax, cax=None):
         """Plot a scatter plot."""
-        ax_xlim = ax.get_xlim()
-        ax_ylim = ax.get_ylim()
         idx = self.scatter_ax.index(ax)
         c, r = self.scatter_indices[idx]
-        sel = np.isfinite(self.data[:,c]) & np.isfinite(self.data[:,r])
-        if self.scatter:
+        if self.scatter: # scatter plot
             ax.clear()
-            ax.relim()
-            ax.autoscale(True)
-            a = ax.scatter(self.data[sel,c], self.data[sel,r], c=self.color_values[sel],
-                           cmap=self.color_map, vmin=self.color_vmin, vmax=self.color_vmax,
-                           s=50, edgecolors='none', zorder=10)
+            a = ax.scatter(self.data[:,c], self.data[:,r], s=50,
+                           edgecolors='white', linewidths=0.5,
+                           picker=self.pick_radius, zorder=10)
+            a.set_facecolor(self.data_colors)
+            pr, pp = pearsonr(self.data[:,c], self.data[:,r])
+            fw = 'bold' if pp < self.significance_level/self.data.shape[1] else 'normal'
+            if pr < 0:
+                ax.text(0.95, 0.9, f'r={pr:.2f}, p={pp:.3f}', fontweight=fw,
+                        transform=ax.transAxes, ha='right', zorder=100)
+            else:
+                ax.text(0.05, 0.9, f'r={pr:.2f}, p={pp:.3f}', fontweight=fw,
+                        transform=ax.transAxes, zorder=100)
+            # color bar:
             if cax is not None:
+                a = ax.scatter(self.data[:, c], self.data[:, r],
+                               c=self.color_values, cmap=self.color_map)
                 self.fig.colorbar(a, cax=cax, ticks=self.color_ticks)
+                a.remove()
                 cax.set_ylabel(self.color_label)
                 self.color_vmin, self.color_vmax, self.color_ticks = \
-                  self.fix_scatter_plot(self.cbax, self.color_values, self.color_label, 'c')
+                  self.fix_scatter_plot(self.cbax, self.color_values,
+                                        self.color_label, 'c')
                 if self.color_ticks is None:
                     if self.color_set_index == 0 and \
                        self.categories[self.color_index] is not None:
                         cax.set_yticklabels(self.categories[self.color_index])
                     elif self.color_set_index == -1 and \
                          self.color_index == 1 and \
                          self.extra_categories is not None:
                         cax.set_yticklabels(self.extra_categories)
-        else:
-            ax.autoscale(True)
-            self.fix_scatter_plot(ax, self.data[sel,c], self.labels[c], 'x')
-            self.fix_scatter_plot(ax, self.data[sel,r], self.labels[r], 'y')
+        else: # histogram
+            if self.show_mode == 0:
+                self.fix_scatter_plot(ax, self.data[:,c], self.labels[c], 'x')
+                self.fix_scatter_plot(ax, self.data[:,r], self.labels[r], 'y')
             axrange = [ax.get_xlim(), ax.get_ylim()]
             ax.clear()
-            ax.hist2d(self.data[sel,c], self.data[sel,r], self.hist_nbins, range=axrange,
-                      cmap=plt.get_cmap('Greys'))
-        md = [m for m in self.mark_data if np.isfinite(self.data[m,c]) and
-                                           np.isfinite(self.data[m,r])]
-        a = ax.scatter(self.data[md,c], self.data[md,r], c=self.data_colors[md],
-                       s=80, zorder=11)
+            ax.hist2d(self.data[:,c], self.data[:,r], self.hist_nbins,
+                      range=axrange, cmap=plt.get_cmap('Greys'))
+        # selected data:
+        a = ax.scatter(self.data[self.mark_data, c],
+                       self.data[self.mark_data, r], s=100,
+                       edgecolors='black', linewidths=0.5,
+                       picker=self.pick_radius, zorder=11)
+        a.set_facecolor(self.data_colors[self.mark_data])
         self.scatter_artists[idx] = a
-        if self.categories[c] is not None:
-            ax.set_xticks(np.arange(len(self.categories[c])))
-            ax.set_xticklabels(self.categories[c])
-        if self.categories[r] is not None:
-            ax.set_yticks(np.arange(len(self.categories[r])))
-            ax.set_yticklabels(self.categories[r])
+        ax.xaxis.set_major_locator(plt.AutoLocator())
+        ax.yaxis.set_major_locator(plt.AutoLocator())
+        ax.xaxis.set_major_formatter(plt.ScalarFormatter())
+        ax.yaxis.set_major_formatter(plt.ScalarFormatter())
+        if self.show_mode == 0:
+            if self.categories[c] is not None:
+                ax.set_xticks(np.arange(len(self.categories[c])))
+                ax.set_xticklabels(self.categories[c])
+            if self.categories[r] is not None:
+                ax.set_yticks(np.arange(len(self.categories[r])))
+                ax.set_yticklabels(self.categories[r])
         if magnifiedax:
             ax.set_xlabel(self.labels[c])
             ax.set_ylabel(self.labels[r])
             cax = self.scatter_ax[self.scatter_indices[:-1].index(self.scatter_indices[-1])]
             ax.set_xlim(cax.get_xlim())
             ax.set_ylim(cax.get_ylim())
         else:
             if c == 0:
                 ax.set_ylabel(self.labels[r])
-        self.fix_scatter_plot(ax, self.data[sel,c], self.labels[c], 'x')
-        self.fix_scatter_plot(ax, self.data[sel,r], self.labels[r], 'y')
+        if self.show_mode == 0:
+            self.fix_scatter_plot(ax, self.data[:, c], self.labels[c], 'x')
+            self.fix_scatter_plot(ax, self.data[:, r], self.labels[r], 'y')
         if not magnifiedax:
-            plt.setp(ax.get_xticklabels(), visible=False)
+            ax.xaxis.set_major_formatter(plt.NullFormatter())
             if c > 0:
-                plt.setp(ax.get_yticklabels(), visible=False)
-        if keep_lims:
-            ax.set_xlim(*ax_xlim)
-            ax.set_ylim(*ax_ylim)
+                ax.yaxis.set_major_formatter(plt.NullFormatter())
+        ax.set_xlim(*self.hist_ax[c].get_xlim())
+        ax.set_ylim(*self.hist_ax[r].get_xlim())
         if magnifiedax:
-            bbox = ax.get_tightbbox(self.fig.canvas.get_renderer())
-            if bbox is not None:
-                self.magnified_backdrop = patches.Rectangle((bbox.x0, bbox.y0),
-                                                            bbox.width, bbox.height,
-                                                            transform=None, clip_on=False,
-                                                            facecolor='white', edgecolor='none', zorder=-5)
-                ax.add_patch(self.magnified_backdrop)
-        try:
-            selector = widgets.RectangleSelector(ax, self._on_select, useblit=True, button=1,
-                                                 props=dict(facecolor='gray', edgecolor='gray', alpha=0.2, fill=True),
-                                                 state_modifier_keys=dict(move='', clear='', square='', center=''))
-        except TypeError:
-            selector = widgets.RectangleSelector(ax, self._on_select, useblit=True, button=1)
+            self._add_backdrop(ax)
+        selector = self._create_selector(ax)
         self.scatter_selector[idx] = selector
+        ax.relim(True)
 
         
     def _init_scatter_plots(self):
         """Initial plots of scatter plots."""
         self.cbax = self.fig.add_axes([0.5, 0.5, 0.1, 0.5])
         cbax = self.cbax
         n = self.data.shape[1]
         for r in range(1, n):
-            yax = None
             for c in range(r):
-                ax = self.fig.add_subplot(n, n, (r-1)*n+c+1, sharex=self.hist_ax[c], sharey=yax)
+                ax = self.fig.add_subplot(n, n, (r-1)*n+c+1)
                 self.scatter_ax.append(ax)
                 self.scatter_indices.append([c, r])
                 self.scatter_artists.append(None)
                 self.scatter_selector.append(None)
-                self._plot_scatter(ax, False, False, cbax)
-                yax = ax
+                self._plot_scatter(ax, False, cbax)
                 cbax = None
 
                 
     def _plot_magnified_scatter(self):
         """Initial plot of the magnified scatter plot."""
         ax = self.fig.add_axes([0.5, 0.9, 0.05, 0.05])
         ax.set_visible(False)
         self.magnified_on = False
         c = 0
         r = 1
-        sel = np.isfinite(self.data[:,c]) & np.isfinite(self.data[:,r])
-        ax.scatter(self.data[sel,c], self.data[sel,r], c=self.data_colors[sel],
-                   s=50, edgecolors='none')
-        md = [m for m in self.mark_data if np.isfinite(self.data[m,c]) and
-                                           np.isfinite(self.data[m,r])]
-        a = ax.scatter(self.data[md,c], self.data[md,r],
-                       c=self.data_colors[md], s=80)
+        a = ax.scatter(self.data[:, c], self.data[:, r],
+                       s=50, edgecolors='none')
+        a.set_facecolor(self.data_colors)
+        a = ax.scatter(self.data[self.mark_data, c],
+                       self.data[self.mark_data, r], s=80)
+        a.set_facecolor(self.data_colors[self.mark_data])
         ax.set_xlabel(self.labels[c])
         ax.set_ylabel(self.labels[r])
-        self.fix_scatter_plot(ax, self.data[sel,c], self.labels[c], 'x')
-        self.fix_scatter_plot(ax, self.data[sel,r], self.labels[r], 'y')
+        self.fix_scatter_plot(ax, self.data[:, c], self.labels[c], 'x')
+        self.fix_scatter_plot(ax, self.data[:, r], self.labels[r], 'y')
         self.scatter_ax.append(ax)
         self.scatter_indices.append([c, r])
         self.scatter_artists.append(a)
         self.scatter_selector.append(None)
 
         
+    def _plot_help(self):
+        ax = self.fig.add_subplot(1, 1, 1)
+        ax.set_position([0.02, 0.02, 0.96, 0.96])
+        ax.xaxis.set_major_locator(plt.NullLocator())
+        ax.yaxis.set_major_locator(plt.NullLocator())
+        n = len(self.mouse_actions) + len(self.key_actions) + 4
+        dy = 1/n
+        y = 1 - 1.5*dy
+        ax.text(0.05, y, 'Key shortcuts', transform=ax.transAxes,
+                fontweight='bold')
+        y -= dy
+        for a, d in self.key_actions:
+            ax.text(0.05, y, a, transform=ax.transAxes)
+            ax.text(0.3, y, d, transform=ax.transAxes)
+            y -= dy
+        y -= dy
+        ax.text(0.05, y, 'Mouse actions', transform=ax.transAxes,
+                fontweight='bold')
+        y -= dy
+        for a, d in self.mouse_actions:
+            ax.text(0.05, y, a, transform=ax.transAxes)
+            ax.text(0.3, y, d, transform=ax.transAxes)
+            y -= dy
+        ax.set_visible(False)
+        self.help_ax = ax
+        
+        
     def fix_scatter_plot(self, ax, data, label, axis):
         """Customize an axes of a scatter plot.
 
         This function is called after a scatter plot has been plotted.
         Once for the x axes, once for the y axis and once for the color bar.
         Reimplement this function to set appropriate limits and ticks.
 
@@ -666,29 +771,29 @@
         
         Parameters
         ----------
         ax: matplotlib axes
             Axes of the scatter plot or color bar to be worked on.
         data: 1D array
             Data array of the axes.
-        label: string
+        label: str
             Label coresponding to the data array.
         axis: str
             'x', 'y': set properties of x or y axes of ax.
             'c': set properies of color bar axes (note that ax can be None!)
                  and return vmin, vmax, and ticks.
 
         Returns
         -------
-            min: float
-                minimum value of color bar axis
-            max: float
-                maximum value of color bar axis
-            ticks: list of float
-                position of ticks for color bar axis
+        min: float
+            minimum value of color bar axis
+        max: float
+            maximum value of color bar axis
+        ticks: list of float
+            position of ticks for color bar axis
         """
         return np.nanmin(data), np.nanmax(data), None
 
     
     def fix_waveform_plot(self, axs, indices):
         """Customize waveform plots.
 
@@ -743,24 +848,26 @@
 
     
     def list_selection(self, indices):
         """List information about the current selection of data points.
 
         This function is called when 'l' is pressed.  Reimplement this
         function, for example, to print some meaningfull information
-        about the current selection of data points on console. You nay
+        about the current selection of data points on console. You may
         do, however, whatever you want in this function.
 
         Parameters
         ----------
         indices: list of int
             Indices of the data points that have been selected.
         """
+        print('')
+        print('selected rows in data table:')
         for i in indices:
-            print(i)
+            print(self.valid_rows[i])
 
             
     def analyze_selection(self, index):
         """Provide further information about a single selected data point.
 
         This function is called when a single data item was double
         clicked.  Reimplement this function to provide some further
@@ -807,246 +914,289 @@
             self.mark_data = []
         try:
             axi = self.scatter_ax.index(ax)
             # from scatter plots:
             c, r = self.scatter_indices[axi]
             if r < self.data.shape[1]:
                 # from scatter:
-                for ind, (x, y) in enumerate(zip(self.data[:,c], self.data[:,r])):
-                    if np.isfinite(x) and np.isfinite(y) and \
-                       x >= x0 and x <= x1 and y >= y0 and y <= y1:
+                for ind, (x, y) in enumerate(zip(self.data[:, c], self.data[:, r])):
+                    if x >= x0 and x <= x1 and y >= y0 and y <= y1:
                         if ind in self.mark_data:
                             if key == 'control':
                                 self.mark_data.remove(ind)
                         elif key != 'control':
                             self.mark_data.append(ind)
             else:
                 # from histogram:
-                for ind, x in enumerate(self.data[:,c]):
-                    if np.isfinite(x) and x >= x0 and x <= x1:
+                for ind, x in enumerate(self.data[:, c]):
+                    if x >= x0 and x <= x1:
                         if ind in self.mark_data:
                             if key == 'control':
                                 self.mark_data.remove(ind)
                         elif key != 'control':
                             self.mark_data.append(ind)
         except ValueError:
             try:
-                r = self.hist_ax.index(ax)
+                r = self.hist_indices[self.hist_ax.index(ax)]
                 # from histogram:
-                for ind, x in enumerate(self.data[:,r]):
-                    if np.isfinite(x) and x >= x0 and x <= x1:
+                for ind, x in enumerate(self.data[:, r]):
+                    if x >= x0 and x <= x1:
                         if ind in self.mark_data:
                             if key == 'control':
                                 self.mark_data.remove(ind)
                         elif key != 'control':
                             self.mark_data.append(ind)
             except ValueError:
                 return
 
                         
     def _update_selection(self):
-        """Highlight select points in the scatter plots and plot corresponding waveforms."""
+        """Highlight selected points in the scatter plots and plot corresponding waveforms."""
         # update scatter plots:
         for artist, (c, r) in zip(self.scatter_artists, self.scatter_indices):
             if artist is not None:
-                md = [m for m in self.mark_data if np.isfinite(self.data[m,c]) and
-                                                   np.isfinite(self.data[m,r])]
-                artist.set_offsets(list(zip(self.data[md,c], self.data[md,r])))
-                artist.set_facecolors(self.data_colors[md])
+                if len(self.mark_data) == 0:
+                    artist.set_offsets(np.zeros((0, 2)))
+                else:
+                    artist.set_offsets(list(zip(self.data[self.mark_data, c],
+                                                self.data[self.mark_data, r])))
+                    artist.set_facecolors(self.data_colors[self.mark_data])
         # waveform plots:
         if len(self.wave_ax) > 0:
             axdi = 0
             axti = 1
             for xi, ax in enumerate(self.wave_ax):
                 ax.clear()
                 if len(self.mark_data) > 0:
                     for idx in self.mark_data:
                         if self.wave_nested:
                             data = self.wave_data[idx][axdi]
                         else:
                             data = self.wave_data[idx]
                         if data is not None:
-                            ax.plot(data[:,0], data[:,axti], c=self.data_colors[idx],
+                            ax.plot(data[:, 0], data[:, axti],
+                                    c=self.data_colors[idx],
                                     picker=self.pick_radius)
                 axti += 1
                 if self.wave_has_xticks[xi]:
                     ax.set_xlabel(self.wave_xlabels[axdi])
                     axti = 1
                     axdi += 1
-                else:
-                    plt.setp(ax.get_xticklabels(), visible=False)
+                #else:
+                #    ax.xaxis.set_major_formatter(plt.NullFormatter())
             for ax, ylabel in zip(self.wave_ax, self.wave_ylabels):
                 ax.set_ylabel(ylabel)
             if not isinstance(self.wave_title, bool) and self.wave_title:
                 self.wave_ax[0].set_title(self.wave_title)
             self.fix_waveform_plot(self.wave_ax, self.mark_data)
         self.fig.canvas.draw()
 
         
+    def _set_limits(self, ax, x0, x1, y0, y1):
+        if ax in self.hist_ax:
+            ax.set_xlim(x0, x1)
+            for hax in self.hist_ax:
+                hax.set_ylim(y0, y1)
+            cc = self.hist_indices[self.hist_ax.index(ax)]
+            for sax, (c, r) in zip(self.scatter_ax, self.scatter_indices):
+                if c == cc:
+                    sax.set_xlim(x0, x1)
+                if r == cc:
+                    sax.set_ylim(x0, x1)
+        if ax in self.scatter_ax:
+            idx = self.scatter_ax.index(ax)
+            cc, rr = self.scatter_indices[idx]
+            self.hist_ax[cc].set_xlim(x0, x1)
+            self.hist_ax[rr].set_xlim(y0, y1)
+            for sax, (c, r) in zip(self.scatter_ax, self.scatter_indices):
+                if c == cc:
+                    sax.set_xlim(x0, x1)
+                if c == rr:
+                    sax.set_xlim(y0, y1)
+                if r == cc:
+                    sax.set_ylim(x0, x1)
+                if r == rr:
+                    sax.set_ylim(y0, y1)
+
+                    
     def _on_key(self, event):
         """Handle key events."""
         #print('pressed', event.key)
-        plot_zoom = True
         if event.key in ['left', 'right', 'up', 'down']:
             if self.magnified_on:
+                mc, mr = self.scatter_indices[-1]
                 if event.key == 'left':
-                    if self.scatter_indices[-1][0] > 0:
+                    if mc > 0:
                         self.scatter_indices[-1][0] -= 1
+                    elif mr > 1:
+                        if mr >= self.data.shape[1]:
+                            self.scatter_indices[-1][1] = self.maxcols - 1
+                        else:
+                            self.scatter_indices[-1][1] -= 1
+                        self.scatter_indices[-1][0] = self.scatter_indices[-1][1] - 1
                     else:
-                        plot_zoom = False
+                        self.scatter_indices[-1][0] = self.data.shape[1] - 1
+                        self.scatter_indices[-1][1] = self.data.shape[1]
                 elif event.key == 'right':
-                    if self.scatter_indices[-1][0] < self.scatter_indices[-1][1]-1 and \
-                       self.scatter_indices[-1][0] < self.maxcols-1:
+                    if mc < mr - 1 and mc < self.maxcols - 1:
                         self.scatter_indices[-1][0] += 1
+                    elif mr < self.maxcols:
+                        self.scatter_indices[-1][0] = 0
+                        self.scatter_indices[-1][1] += 1
+                        if mr >= self.maxcols:
+                            self.scatter_indices[-1][1] = self.data.shape[1]
                     else:
-                        plot_zoom = False
+                        self.scatter_indices[-1][0] = 0
+                        self.scatter_indices[-1][1] = 1
                 elif event.key == 'up':
-                    if self.scatter_indices[-1][1] > 1:
-                        if self.scatter_indices[-1][1] >= self.data.shape[1]:
-                            self.scatter_indices[-1][1] = self.maxcols-1
+                    if mr > mc + 1:
+                        if mr >= self.data.shape[1]:
+                            self.scatter_indices[-1][1] = self.maxcols - 1
                         else:
                             self.scatter_indices[-1][1] -= 1
-                        if self.scatter_indices[-1][0] >= self.scatter_indices[-1][1]:
-                            self.scatter_indices[-1][0] = self.scatter_indices[-1][1]-1
+                    elif mc > 0:
+                        self.scatter_indices[-1][0] -= 1
+                        self.scatter_indices[-1][1] = self.data.shape[1]
                     else:
-                        plot_zoom = False
+                        self.scatter_indices[-1][0] = self.data.shape[1] - 1
+                        self.scatter_indices[-1][1] = self.data.shape[1]
                 elif event.key == 'down':
-                    if self.scatter_indices[-1][1] < self.maxcols:
+                    if mr < self.maxcols:
                         self.scatter_indices[-1][1] += 1
+                        if mr >= self.maxcols:
+                            self.scatter_indices[-1][1] = self.data.shape[1]
+                    elif mc < self.maxcols - 1:
+                        self.scatter_indices[-1][0] += 1
+                        self.scatter_indices[-1][1] = mc + 2
                         if self.scatter_indices[-1][1] >= self.maxcols:
                             self.scatter_indices[-1][1] = self.data.shape[1]
                     else:
-                        plot_zoom = False
+                        self.scatter_indices[-1][0] = 0
+                        self.scatter_indices[-1][1] = 1
+            for k in reversed(range(len(self.zoom_stack))):
+                if self.zoom_stack[k][0] == self.scatter_ax[-1]:
+                    del self.zoom_stack[k]
+            self.scatter_ax[-1].clear()
+            self.scatter_ax[-1].set_visible(True)
+            self.magnified_on = True
+            self._set_magnified_pos(self.fig.get_window_extent().width,
+                                    self.fig.get_window_extent().height)
+            if self.scatter_indices[-1][1] < self.data.shape[1]:
+                self._plot_scatter(self.scatter_ax[-1], True)
+            else:
+                self._plot_hist(self.scatter_ax[-1], True)
+            self.fig.canvas.draw()
         else:
-            plot_zoom = False
             if event.key == 'escape':
                 self.scatter_ax[-1].set_position([0.5, 0.9, 0.05, 0.05])
                 self.magnified_on = False
                 self.scatter_ax[-1].set_visible(False)
                 self.fig.canvas.draw()
             elif event.key in 'oz':
                 self.select_zooms = not self.select_zooms
             elif event.key == 'backspace':
                 if len(self.zoom_stack) > 0:
-                    ax, xmin, xmax, ymin, ymax = self.zoom_stack.pop()
-                    ax.set_xlim(xmin, xmax)
-                    ax.set_ylim(ymin, ymax)
-                    if ax in self.scatter_ax[:-1]:
-                        axidx = self.scatter_ax[:-1].index(ax)
-                        if self.scatter_indices[axidx][0] == self.scatter_indices[-1][0]:
-                            self.scatter_ax[-1].set_xlim(xmin, xmax)
-                        if self.scatter_indices[axidx][1] == self.scatter_indices[-1][1]:
-                            self.scatter_ax[-1].set_ylim(ymin, ymax)
-                    elif ax in self.hist_ax:
-                        if self.scatter_indices[-1][1] == self.data.shape[1] and \
-                           self.scatter_indices[-1][0] == self.hist_ax.index(ax):
-                            self.scatter_ax[-1].set_xlim(xmin, xmax)
-                            self.scatter_ax[-1].set_ylim(ymin, ymax)
+                    self._set_limits(*self.zoom_stack.pop())
                     self.fig.canvas.draw()
             elif event.key in '+=':
                 self.pick_radius *= 1.5
             elif event.key in '-':
                 if self.pick_radius > 5.0:
                     self.pick_radius /= 1.5
             elif event.key in '0':
                 self.pick_radius = 4.0
             elif event.key in ['pageup', 'pagedown', '<', '>']:
                 if event.key in ['pageup', '<'] and self.maxcols > 2:
                     self.maxcols -= 1
                 elif event.key in ['pagedown', '>'] and self.maxcols < self.raw_data.shape[1]:
                     self.maxcols += 1
+                for ax in self.hist_ax:
+                    self._plot_hist(ax, False)
                 self._update_layout()
             elif event.key == 'w':
-                if self.maxcols > 0:
-                    self.all_maxcols[self.show_mode] = self.maxcols
-                    self.maxcols = 0
-                else:
-                    self.maxcols = self.all_maxcols[self.show_mode]
-                self._set_layout(self.fig.get_window_extent().width,
-                                 self.fig.get_window_extent().height)
-                self.fig.canvas.draw()
+                if len(self.wave_data) > 0:
+                    if self.maxcols > 0:
+                        self.all_maxcols[self.show_mode] = self.maxcols
+                        self.maxcols = 0
+                    else:
+                        self.maxcols = self.all_maxcols[self.show_mode]
+                    self._set_layout(self.fig.get_window_extent().width,
+                                     self.fig.get_window_extent().height)
+                    self.fig.canvas.draw()
             elif event.key == 'ctrl+a':
-                self.mark_data = range(len(self.data))
+                self.mark_data = list(range(len(self.data)))
                 self._update_selection()
             elif event.key in 'cC':
                 if event.key in 'c':
-                    first = True
-                    while first or not np.all(np.isfinite(self.color_values)):
-                        self.color_index -= 1
-                        if self.color_index < 0:
-                            self.color_set_index -= 1
-                            if self.color_set_index < -1:
-                                self.color_set_index = len(self.all_data)-1
-                            if self.color_set_index >= 0:
-                                if self.all_data[self.color_set_index] is None:
-                                    self.compute_pca(self.color_set_index>1, True)
-                                self.color_index = self.all_data[self.color_set_index].shape[1]-1
-                            else:
-                                self.color_index = 0 if self.extra_colors is None else 1
-                        self._set_color_column()
-                        first = False
-                else:
-                    first = True
-                    while first or not np.all(np.isfinite(self.color_values)):
-                        self.color_index += 1
-                        if (self.color_set_index >= 0 and \
-                            self.color_index >= self.all_data[self.color_set_index].shape[1]) or \
-                            (self.color_set_index < 0 and \
-                             self.color_index >= (1 if self.extra_colors is None else 2)):
-                            self.color_index = 0
-                            self.color_set_index += 1
-                            if self.color_set_index >= len(self.all_data):
-                                self.color_set_index = -1
-                            elif self.all_data[self.color_set_index] is None:
+                    self.color_index -= 1
+                    if self.color_index < 0:
+                        self.color_set_index -= 1
+                        if self.color_set_index < -1:
+                            self.color_set_index = len(self.all_data)-1
+                        if self.color_set_index >= 0:
+                            if self.all_data[self.color_set_index] is None:
                                 self.compute_pca(self.color_set_index>1, True)
-                        self._set_color_column()
-                        first = False
+                            self.color_index = self.all_data[self.color_set_index].shape[1]-1
+                        else:
+                            self.color_index = 0 if self.extra_colors is None else 1
+                    self._set_color_column()
+                else:
+                    self.color_index += 1
+                    if (self.color_set_index >= 0 and \
+                        self.color_index >= self.all_data[self.color_set_index].shape[1]) or \
+                        (self.color_set_index < 0 and \
+                         self.color_index >= (1 if self.extra_colors is None else 2)):
+                        self.color_index = 0
+                        self.color_set_index += 1
+                        if self.color_set_index >= len(self.all_data):
+                            self.color_set_index = -1
+                        elif self.all_data[self.color_set_index] is None:
+                            self.compute_pca(self.color_set_index>1, True)
+                    self._set_color_column()
                 for ax in self.scatter_ax:
-                    if len(ax.collections) > 0:
-                        idx = self.scatter_ax.index(ax)
-                        c, r = self.scatter_indices[idx]
-                        ax.collections[0].set_facecolors(self.data_colors[np.isfinite(self.data[:,c]) & np.isfinite(self.data[:,r])])
-                for a, (c, r) in zip(self.scatter_artists, self.scatter_indices):
+                    ax.collections[0].set_facecolors(self.data_colors)
+                for a in self.scatter_artists:
                     if a is not None:
-                        md = [m for m in self.mark_data if np.isfinite(self.data[m,c]) and
-                                                           np.isfinite(self.data[m,r])]
-                        a.set_facecolors(self.data_colors[md])
+                        a.set_facecolors(self.data_colors[self.mark_data])
                 for ax in self.wave_ax:
                     for l, c in zip(ax.lines, self.data_colors[self.mark_data]):
                         l.set_color(c)
                         l.set_markerfacecolor(c)
-                self._plot_scatter(self.scatter_ax[0], False, True, self.cbax)
+                self._plot_scatter(self.scatter_ax[0], False, self.cbax)
                 self.fix_scatter_plot(self.cbax, self.color_values,
                                       self.color_label, 'c')
                 self.fig.canvas.draw()
             elif event.key in 'nN':
                 if event.key in 'N':
                     self.hist_nbins = (self.hist_nbins*3)//2
                 elif self.hist_nbins >= 15:
                     self.hist_nbins = (self.hist_nbins*2)//3
+                else:
+                    self.hist_nbins = 10
                 for ax in self.hist_ax:
-                    self._plot_hist(ax, False, True)
+                    self._plot_hist(ax, False)
+                self._set_hist_ylim()
                 if self.scatter_indices[-1][1] >= self.data.shape[1]:
                     self._plot_hist(self.scatter_ax[-1], True, True)
                 elif not self.scatter:
-                    self._plot_scatter(self.scatter_ax[-1], True, True)
+                    self._plot_scatter(self.scatter_ax[-1], True)
                 if not self.scatter:
                     for ax in self.scatter_ax[:-1]:
-                        self._plot_scatter(ax, False, True)
+                        self._plot_scatter(ax, False)
                 self.fig.canvas.draw()
-            elif event.key in 'h':
+            elif event.key in 'H':
                 self.scatter = not self.scatter
                 for ax in self.scatter_ax[:-1]:
-                    self._plot_scatter(ax, False, True)
+                    self._plot_scatter(ax, False)
                 if self.scatter_indices[-1][1] < self.data.shape[1]:
-                    self._plot_scatter(self.scatter_ax[-1], True, True)
+                    self._plot_scatter(self.scatter_ax[-1], True)
                 self.fig.canvas.draw()
             elif event.key in 'pP':
                 self.all_maxcols[self.show_mode] = self.maxcols
-                if event.key == 'p':
+                if event.key == 'P':
                     self.show_mode += 1
                     if self.show_mode >= len(self.all_data):
                         self.show_mode = 0
                 else:
                     self.show_mode -= 1
                     if self.show_mode < 0:
                         self.show_mode = len(self.all_data)-1
@@ -1059,38 +1209,26 @@
                 if self.all_data[self.show_mode] is None:
                     self.compute_pca(self.show_mode>1, True)
                 self.data = self.all_data[self.show_mode]
                 self.labels = self.all_labels[self.show_mode]
                 self.maxcols = self.all_maxcols[self.show_mode]
                 self.zoom_stack = []
                 self.fig.canvas.manager.set_window_title(self.title + ': ' + self.all_titles[self.show_mode])
-                for ax in self.hist_ax[:self.maxcols]:
-                    self._plot_hist(ax, False, False)
-                for ax in self.scatter_ax[:self.maxcols]:
-                    self._plot_scatter(ax, False, False)
+                for ax in self.hist_ax:
+                    self._plot_hist(ax, False)
+                self._set_hist_ylim()
+                for ax in self.scatter_ax:
+                    self._plot_scatter(ax, False)
                 self._update_layout()
             elif event.key in 'l':
                 if len(self.mark_data) > 0:
-                    print('')
-                    print('selected:')
                     self.list_selection(self.mark_data)
-        if plot_zoom:
-            for k in reversed(range(len(self.zoom_stack))):
-                if self.zoom_stack[k][0] == self.scatter_ax[-1]:
-                    del self.zoom_stack[k]
-            self.scatter_ax[-1].clear()
-            self.scatter_ax[-1].set_visible(True)
-            self.magnified_on = True
-            self._set_magnified_pos(self.fig.get_window_extent().width,
-                                    self.fig.get_window_extent().height)
-            if self.scatter_indices[-1][1] < self.data.shape[1]:
-                self._plot_scatter(self.scatter_ax[-1], True, False)
-            else:
-                self._plot_hist(self.scatter_ax[-1], True, False)
-            self.fig.canvas.draw()
+            elif event.key in 'h':
+                self.help_ax.set_visible(not self.help_ax.get_visible())
+                self.fig.canvas.draw()
 
             
     def _on_select(self, eclick, erelease):
         """Handle selection events."""
         if eclick.dblclick:
             if len(self.mark_data) > 0:
                 self.analyze_selection(self.mark_data[-1])
@@ -1115,26 +1253,28 @@
             dy = self.pick_radius*(ymax-ymin)/height
             x0 = erelease.xdata - dx
             x1 = erelease.xdata + dx
             y0 = erelease.ydata - dy
             y1 = erelease.ydata + dy
         elif self.select_zooms:
             self.zoom_stack.append((ax, xmin, xmax, ymin, ymax))
-            ax.set_xlim(x0, x1)
-            ax.set_ylim(y0, y1)
+            self._set_limits(ax, x0, x1, y0, y1)
         self._make_selection(ax, erelease.key, x0, x1, y0, y1)
         self._update_selection()
 
         
     def _on_pick(self, event):
-        """Handle pick events on waveforms."""
+        """Handle pick events."""
         for ax in self.wave_ax:
             for k, l in enumerate(ax.lines):
                 if l is event.artist:
                     self.mark_data = [self.mark_data[k]]
+        for ax in self.scatter_ax:
+            if ax.collections[0] is event.artist:
+                self.mark_data = event.ind
         self._update_selection()
         if event.mouseevent.dblclick:
             if len(self.mark_data) > 0:
                 self.analyze_selection(self.mark_data[-1])
 
                     
     def _set_layout(self, width, height):
@@ -1173,15 +1313,18 @@
             self.cbax.set_position([0.99, 0.01, 0.01, 0.01])
         # magnified plot:
         if self.maxcols > 0:
             self._set_magnified_pos(width, height)
             if self.magnified_backdrop is not None:
                 bbox = self.scatter_ax[-1].get_tightbbox(self.fig.canvas.get_renderer())
                 if bbox is not None:
-                    self.magnified_backdrop.set_bounds(bbox.x0, bbox.y0, bbox.width, bbox.height)
+                    self.magnified_backdrop.set_bounds(bbox.x0 - self.mborder,
+                                                       bbox.y0 - self.mborder,
+                                                       bbox.width + 2*self.mborder,
+                                                       bbox.height + 2*self.mborder)
         else:
             self.scatter_ax[-1].set_position([0.5, 0.9, 0.05, 0.05])
             self.scatter_ax[-1].set_visible(False)
         # waveform plots:
         if len(self.wave_ax) > 0:
             if self.maxcols > 0:
                 x0 = xoffs+((self.maxcols+1)//2)*dx
@@ -1215,19 +1358,20 @@
     def _update_layout(self):
         """Update content and position of magnified plot."""
         if self.scatter_indices[-1][1] < self.data.shape[1]:
             if self.scatter_indices[-1][1] >= self.maxcols:
                 self.scatter_indices[-1][1] = self.maxcols-1
             if self.scatter_indices[-1][0] >= self.scatter_indices[-1][1]:
                 self.scatter_indices[-1][0] = self.scatter_indices[-1][1]-1
-            self._plot_scatter(self.scatter_ax[-1], True, False)
+            self._plot_scatter(self.scatter_ax[-1], True)
         else:
             if self.scatter_indices[-1][0] >= self.maxcols:
                 self.scatter_indices[-1][0] = self.maxcols-1
-                self._plot_hist(self.scatter_ax[-1], True, False)
+                self._plot_hist(self.scatter_ax[-1], True)
+        self._set_hist_ylim()
         self._set_layout(self.fig.get_window_extent().width,
                          self.fig.get_window_extent().height)
         self.fig.canvas.draw()
 
         
     def _on_resize(self, event):
         """Adapt layout of plots to new figure size."""
@@ -1235,66 +1379,220 @@
 
 
 def categorize(data):
     """Convert categorial string data into integer categories.
 
     Parameters
     ----------
-    data: list of string
-        A list of textual categories.
+    data: list or ndarray of str
+        Data with textual categories.
 
     Returns
     -------
-    categories: list of strings
-        A sorted unique list of the strings in data.
-    cdata: list of integers
+    categories: list of str
+        A sorted unique list of the strings in `data`,
+        that is the names of the categories.
+    cdata: ndarray of int
         A copy of the input `data` where each string value is replaced
-        by an integer number that is an index into the reurned `categories`.
+        by an integer number that is an index into the returned `categories`.
     """
     cats = sorted(set(data))
     cdata = np.array([cats.index(x) for x in data], dtype=int)
     return cats, cdata
+
+
+def select_features(data, columns):
+    """Assemble list of column indices.
+
+    Parameters
+    ----------
+    data: TableData
+        The table from which to select features.
+    columns: list of str
+        Feature names (column headers) to be selected from the data.
+        If a column is listed twice (even times) it is not added.
+
+    Returns
+    -------
+    data_cols: list of int
+        List of indices into data columns for selecting features.
+    """
+    if len(columns) == 0:
+        data_cols = list(np.arange(len(data)))
+    else:
+        data_cols = []
+        for c in columns:
+            idx = data.index(c)
+            if idx is None:
+                print(f'"{c}" is not a valid data column')
+            elif idx in data_cols:
+                data_cols.remove(idx)
+            else:
+                data_cols.append(idx)
+    return data_cols
+
+
+def select_coloring(data, data_cols, color_col):
+    """Select column from data table for colorizing the data.
+
+    Pass the output of this function on to MultivariateExplorer.set_colors().
+
+    Parameters
+    ----------
+    data: TableData
+        Table with all EOD properties from which columns are selected.
+    data_cols: list of int
+        List of columns selected to be explored.
+    color_col: str or int
+        Column to be selected for coloring the data.
+        If 'row' then use the row index of the data in the table for coloring.
+
+    Returns
+    -------
+    colors: int or list of values or None
+        Either index of `data_cols` or additional data from the data table
+        to be used for coloring.
+    color_label: str or None
+        Label for labeling the color bar.
+    color_idx: int or None
+        Index of color column in `data`.
+    error: None or str
+        In case an invalid column is selected, an error string.
+    """
+    color_idx = data.index(color_col)
+    colors = None
+    color_label = None
+    if color_idx is None and color_col != 'row':
+        return None, None, None, f'"{color_col}" is not a valid column for color code'
+    if color_idx is None:
+        colors = -2
+    elif color_idx in data_cols:
+        colors = data_cols.index(color_idx)
+    else:
+        if len(data.unit(color_idx)) > 0 and not data.unit(color_idx) in ['-', '1']:
+            color_label = f'{data.label(color_idx)} [{data.unit(color_idx)}]'
+        else:
+            color_label = data.label(color_idx)
+        colors = data[:, color_idx]
+    return colors, color_label, color_idx, None
+
+
+def list_available_features(data, data_cols=[], color_col=None):
+    """Print available features on console.
+
+    Parameters
+    ----------
+    data: TableData
+        The full data table.
+    data_cols: list of int
+        List of indices of columns (features) in the table
+        that are passed on to the MultivariateExplorer.
+    color_col: int or None
+        Index of columns (feature) in the table
+        that is initially used for color coding the data.
+    """
+    print('available features:')
+    for k, c in enumerate(data.keys()):
+        s = [' '] * 3
+        if k in data_cols:
+            s[1] = '*'
+        if color_col is not None and k == color_col:
+            s[0] = 'C'
+        print(''.join(s) + c)
+    if len(data_cols) > 0:
+        print('*: feature selected for exploration')
+    if color_col is not None:
+        print('C: feature selected for color coding the data')
+
+
+class PrintHelp(argparse.Action):
+    def __call__(self, parser, namespace, values, option_string):
+        parser.print_help()
+        print('')
+        print('mouse:')
+        for ma in MultivariateExplorer.mouse_actions:
+            print('%-23s %s' % ma)
+        print('%-23s %s' % ('double left click', 'run thunderfish on selected EOD waveform'))
+        print('')
+        print('key shortcuts:')
+        for ka in MultivariateExplorer.key_actions:
+            print('%-23s %s' % ka)
+        parser.exit()      
+
+
+def demo():
+    """Run the multivariate explorer with a random test data set.
+    """
+    # generate data:
+    n = 100
+    data = []
+    data.append(np.random.randn(n) + 2.0)
+    data.append(1.0+0.1*data[0] + 1.5*np.random.randn(n))
+    data.append(10*(-3.0*data[0] + 2.0*data[1] + 1.8*np.random.randn(n)))
+    idx = np.random.randint(0, 3, n)
+    names = ['aaa', 'bbb', 'ccc']
+    data.append([names[i] for i in idx])
+    # generate waveforms:
+    waveforms = []
+    time = np.arange(0.0, 10.0, 0.01)
+    for r in range(len(data[0])):
+        x = data[0][r]*np.sin(2.0*np.pi*data[1][r]*time + data[2][r])
+        y = data[0][r]*np.exp(-0.5*((time-data[1][r])/(0.2*data[2][r]))**2.0)
+        waveforms.append(np.column_stack((time, x, y)))
+        #waveforms.append([np.column_stack((time, x)), np.column_stack((time, y))])
+    # initialize explorer:
+    expl = MultivariateExplorer(data,
+                                list(map(chr, np.arange(len(data))+ord('A'))),
+                                'Explorer')
+    expl.set_wave_data(waveforms, 'Time', ['Sine', 'Gauss'])
+    # explore data:
+    expl.set_colors()
+    expl.show()
         
 
-def main():
+def main(*cargs):
     # parse command line:
-    parser = argparse.ArgumentParser(add_help=True,
+    parser = argparse.ArgumentParser(add_help=False,
         description='View and explore multivariate data.',
-        epilog='version %s by Benda-Lab (2019-%s)' % (__version__, __year__))
+        epilog = f'version {__version__} by Benda-Lab (2019-{__year__})')
+    parser.add_argument('-h', '--help', nargs=0, action=PrintHelp,
+                        help='show this help message and exit')
+    parser.add_argument('--version', action='version', version=__version__)
+    parser.add_argument('-l', dest='list_features', action='store_true',
+                        help='list all available data columns (features) and exit')
+    parser.add_argument('-d', dest='data_cols', action='append',
+                        default=[], metavar='COLUMN',
+                        help='data columns (features) to be explored')
+    parser.add_argument('-c', dest='color_col', default=None,
+                        type=str, metavar='COLUMN',
+                        help='data column to be used for color code or "row"')
+    parser.add_argument('-m', dest='color_map', default='jet',
+                        type=str, metavar='CMAP',
+                        help='name of color map to be used')
     parser.add_argument('file', nargs='?', default='', type=str,
                         help='a file containing a table of data (csv file or similar)')
-    args = parser.parse_args()
+    if len(cargs) == 0:
+        cargs = None
+    args = parser.parse_args(cargs)
     if args.file:
         # load data:
         data = TableData(args.file)
-        # initialize explorer:
-        expl = MultivariateExplorer(data)
+        data_cols = select_features(data, args.data_cols)
+        # select column used for coloring the data:
+        colors, color_label, color_col, error = \
+          select_coloring(data, data_cols, args.color_col)
+        if error:
+            parser.error(error)
+        # list features:
+        if args.list_features:
+            list_available_features(data, data_cols, color_col)
+            parser.exit()
+        # explore data:
+        expl = MultivariateExplorer(data[:, data_cols])
+        expl.set_colors(colors, color_label, args.color_map)
+        expl.show()
     else:
-        # generate data:
-        n = 100
-        data = []
-        data.append(np.random.randn(n) + 2.0)
-        data.append(1.0+0.1*data[0] + 1.5*np.random.randn(n))
-        data.append(-3.0*data[0] - 2.0*data[1] + 1.8*np.random.randn(n))
-        idx = np.random.randint(0, 3, n)
-        names = ['aaa', 'bbb', 'ccc']
-        data.append([names[i] for i in idx])
-        # generate waveforms:
-        waveforms = []
-        time = np.arange(0.0, 10.0, 0.01)
-        for r in range(len(data[0])):
-            x = data[0][r]*np.sin(2.0*np.pi*data[1][r]*time + data[2][r])
-            y = data[0][r]*np.exp(-0.5*((time-data[1][r])/(0.2*data[2][r]))**2.0)
-            waveforms.append(np.column_stack((time, x, y)))
-            #waveforms.append([np.column_stack((time, x)), np.column_stack((time, y))])
-        # initialize explorer:
-        expl = MultivariateExplorer(data,
-                                    list(map(chr, np.arange(len(data))+ord('A'))),
-                                    'Explorer')
-        expl.set_wave_data(waveforms, 'Time', ['Sine', 'Gauss'])
-    # explore data:
-    expl.set_colors()
-    expl.show()
+        demo()
 
 
 if __name__ == '__main__':
-    main()
+    main(*sys.argv[1:])
```

### Comparing `thunderlab-1.1.0/src/thunderlab/powerspectrum.py` & `thunderlab-1.2.0/src/thunderlab/powerspectrum.py`

 * *Files identical despite different names*

### Comparing `thunderlab-1.1.0/src/thunderlab/tabledata.py` & `thunderlab-1.2.0/src/thunderlab/tabledata.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,33 +44,40 @@
 __pdoc__['TableData.__call__'] = True
 __pdoc__['TableData.__getitem__'] = True
 __pdoc__['TableData.__setitem__'] = True
 __pdoc__['TableData.__delitem__'] = True
 __pdoc__['TableData.__str__'] = True
 
 
+default_missing_str = '-'
+"""Default string indicating nan data elements whne outputting data."""
+
+default_missing_inputs = ['na', 'NA', 'nan', 'NAN', '-']
+"""Default strings that are translated to nan when loading table data."""
+
+
 class TableData(object):
     """Table with numpy-style indexing and a rich hierarchical header including units and formats.
     
     Parameters
     ----------
-    data: string, stream, array
+    data: str, stream, ndarray
         - a filename: load table from file with name `data`.
         - a stream/file handle: load table from that stream.
-        - 1-D or 2-D array of data: the data of the table.
+        - 1-D or 2-D ndarray of data: the data of the table.
           Requires als a specified `header`.
-    header: list of string
+    header: list of str
         Header labels for each column.
-    units: list of string, optional
+    units: list of str, optional
         Unit strings for each column.
-    formats: string or list of string, optional
+    formats: str or list of str, optional
         Format strings for each column. If only a single format string is
         given, then all columns are initialized with this format string.
-    missing: string
-        Missing data are indicated by this string.
+    missing: list of str
+        Missing data are indicated by one of these strings.
 
     Manipulate table header
     -----------------------
 
     Each column of the table has a label (the name of the column), a
     unit, and a format specifier. Sections group columns into a hierarchy.
 
@@ -216,33 +223,34 @@
     [23, 45, 3405]
     [1.234, 123.5, 0.0001235]
     ```
 
     Accessing data
     --------------
 
-    In contrast to the iterator functions the [] operator treats the table as a
-    2D-array where the first index indicates the row and the second index the column.
+    In contrast to the iterator functions the [] operator treats the
+    table as a 2D-array where the first index indicates the row and
+    the second index the column.
 
     Like a numpy aray the table can be sliced, and logical indexing can
     be used to select specific parts of the table.
     
     As for any function, columns can be specified as indices or strings.
     
     - `rows()`: the number of rows.
     - `columns()`: the number of columns.
     - `shape`: number of rows and columns.
     - `row()`: a single row of the table as TableData.
     - `row_dict()`: a single row of the table as dictionary.
     - `col()`: a single column of the table as TableData.
-    - `__call__()`: a single column of the table as numpy array.
+    - `__call__()`: a single column of the table as ndarray.
     - `__getitem__()`: data elements specified by slice.
     - `__setitem__()`: assign values to data elements specified by slice.
     - `__delitem__()`: delete data elements or whole columns or rows.
-    - `array()`: the table data as a numpy array.
+    - `array()`: the table data as a ndarray.
     - `data_frame()`: the table data as a pandas DataFrame.
     - `dicts()`: the table as a list of dictionaries.
     - `dict()`: the table as a dictionary.
     - `append_data()`: append data elements to successive columns.
     - `append_data_column()`: append data elements to a column.
     - `set_column()`: set the column where to add data.
     - `fill_data()`: fill up all columns with missing data.
@@ -251,25 +259,25 @@
     
     - `sort()`: sort the table rows in place.
     - `statistics()`: descriptive statistics of each column.
 
     For example:
     ```
     # single column:    
-    df('size')     # data of 'size' column as numpy array
-    df[:,'size']   # data of 'size' column as numpy array
+    df('size')     # data of 'size' column as ndarray
+    df[:,'size']   # data of 'size' column as ndarray
     df.col('size') # table with the single column 'size'
 
     # single row:    
     df[2,:]    # table with data of only the third row
     df.row(2)  # table with data of only the third row
 
     # slices:
     df[2:5,['size','jitter']]          # sub-table
-    df[2:5,['size','jitter']].array()  # numpy array with data only
+    df[2:5,['size','jitter']].array()  # ndarray with data only
 
     # logical indexing:
     df[df('speed') > 100.0, 'size'] = 0.0 # set size to 0 if speed is > 100
 
     # delete:
     del df[3:6, 'weight']  # delete rows 3-6 from column 'weight'
     del df[3:5,:]          # delete rows 3-5 completeley
@@ -315,14 +323,15 @@
     - `load()`: load table from file or stream.
     - `formats`: list of supported file formats for writing.
     - `descriptions`: dictionary with descriptions of the supported file formats.
     - `extensions`: dictionary with default filename extensions for each of the file formats.
     - `ext_formats`: dictionary mapping filename extensions to file formats.
 
     See documentation of the `write()` function for examples of the supported file formats.
+
     """
     
     formats = ['dat', 'ascii', 'csv', 'rtai', 'md', 'tex', 'html']
     """list of strings: Supported output formats."""
     descriptions = {'dat': 'data text file', 'ascii': 'ascii-art table',
                     'csv': 'comma separated values', 'rtai': 'rtai-style table',
                     'md': 'markdown', 'tex': 'latex tabular',
@@ -333,15 +342,15 @@
     """dict: Default file extensions for the output `formats`. """
     ext_formats = {'dat': 'dat', 'DAT': 'dat', 'txt': 'dat', 'TXT': 'dat',
                    'csv': 'csv', 'CSV': 'csv', 'md': 'md', 'MD': 'md',
                    'tex': 'tex', 'TEX': 'tex', 'html': 'html', 'HTML': 'html'}
     """dict: Mapping of file extensions to the output formats."""
 
     def __init__(self, data=None, header=None, units=None, formats=None,
-                 missing='-'):
+                 missing=default_missing_inputs):
         self.data = []
         self.shape = (0, 0)
         self.header = []
         self.nsecs = 0
         self.units = []
         self.formats = []
         self.hidden = []
@@ -387,23 +396,23 @@
         
     def append(self, label, unit=None, formats=None, value=None,
                fac=None, key=None):
         """Append column to the table.
 
         Parameters
         ----------
-        label: string or list of string
+        label: str or list of str
             Optional section titles and the name of the column.
-        unit: string or None
+        unit: str or None
             The unit of the column contents.
-        formats: string or None
+        formats: str or None
             The C-style format string used for printing out the column content, e.g.
             '%g', '%.2f', '%s', etc.
             If None, the format is set to '%g'.
-        value: None, float, int, string, etc. or list thereof, or list of dict
+        value: None, float, int, str, etc. or list thereof, or list of dict
             If not None, data for the column.
             If list of dictionaries, extract from each dictionary in the list
             the value specified by `key`. If `key` is `None` use `label` as
             the key.
         fac: float
             If not None, multiply the data values by this number.
         key: None or key of a dictionary
@@ -458,27 +467,27 @@
         """Insert a table column at a given position.
 
         .. WARNING::
            If no `value` is given, the inserted column is an empty list.
 
         Parameters
         ----------
-        columns int or string
+        columns int or str
             Column before which to insert the new column.
             Column can be specified by index or name,
             see `index()` for details.
-        label: string or list of string
+        label: str or list of str
             Optional section titles and the name of the column.
-        unit: string or None
+        unit: str or None
             The unit of the column contents.
-        formats: string or None
+        formats: str or None
             The C-style format string used for printing out the column content, e.g.
             '%g', '%.2f', '%s', etc.
             If None, the format is set to '%g'.
-        value: None, float, int, string, etc. or list thereof
+        value: None, float, int, str, etc. or list thereof
             If not None, data for the column.
 
         Returns
         -------
         index: int
             The index of the inserted column.
             
@@ -512,15 +521,15 @@
         return col
 
     def remove(self, columns):
         """Remove columns from the table.
 
         Parameters
         -----------
-        columns: int or string or list of int or string
+        columns: int or str or list of int of str
             Columns can be specified by index or name,
             see `index()` for details.
 
         Raises
         ------
         IndexError:
             If an invalid column was specified.
@@ -550,26 +559,28 @@
         self.shape = (self.rows(), self.columns())
 
     def section(self, column, level):
         """The section name of a specified column.
 
         Parameters
         ----------
-        column: None, int, or string
+        column: None, int, or str
             A specification of a column.
             See self.index() for more information on how to specify a column.
         level: int
             The level of the section to be returned. The column label itself is level=0.
 
         Returns
         -------
-        name: string
-            The name of the section at the specified level containing the column.
+        name: str
+            The name of the section at the specified level containing
+            the column.
         index: int
-            The column index that contains this section (equal or smaller thant `column`).
+            The column index that contains this section
+            (equal or smaller thant `column`).
 
         Raises
         ------
         IndexError:
             If `level` exceeds the maximum possible level.
         """
         if level < 0 or level > self.nsecs:
@@ -580,17 +591,17 @@
         return self.header[column][level], column
     
     def set_section(self, label, column, level):
         """Set a section name.
 
         Parameters
         ----------
-        label: string
+        label: str
             The new name to be used for the section.
-        column: None, int, or string
+        column: None, int, or str
             A specification of a column.
             See self.index() for more information on how to specify a column.
         level: int
             The level of the section to be set. The column label itself is level=0.
         """
         column = self.index(column)
         self.header[column][level] = label
@@ -600,15 +611,15 @@
         """Add sections to the table header.
 
         Each column of the table has a header label. Columns can be
         grouped into sections. Sections can be nested arbitrarily.
 
         Parameters
         ----------
-        label: string or list of string
+        label: stri or list of str
             The name(s) of the section(s).
 
         Returns
         -------
         index: int
             The column index where the section was appended.
         """
@@ -633,19 +644,19 @@
         return self.addcol
         
     def insert_section(self, column, section):
         """Insert a section at a given position of the table header.
 
         Parameters
         ----------
-        columns int or string
+        columns int or str
             Column before which to insert the new section.
             Column can be specified by index or name,
             see `index()` for details.
-        section: string
+        section: str
             The name of the section.
 
         Returns
         -------
         index: int
             The index of the column where the section was inserted.
             
@@ -665,122 +676,122 @@
         return col
 
     def label(self, column):
         """The name of a column.
 
         Parameters
         ----------
-        column: None, int, or string
+        column: None, int, or str
             A specification of a column.
             See self.index() for more information on how to specify a column.
 
         Returns
         -------
-        name: string
+        name: str
             The column label.
         """
         column = self.index(column)
         return self.header[column][0]
 
     def set_label(self, label, column):
         """Set the name of a column.
 
         Parameters
         ----------
-        label: string
+        label: str
             The new name to be used for the column.
-        column: None, int, or string
+        column: None, int, or str
             A specification of a column.
             See self.index() for more information on how to specify a column.
         """        
         column = self.index(column)
         self.header[column][0] = label
         return column
 
     def unit(self, column):
         """The unit of a column.
 
         Parameters
         ----------
-        column: None, int, or string
+        column: None, int, or str
             A specification of a column.
             See self.index() for more information on how to specify a column.
 
         Returns
         -------
-        unit: string
+        unit: str
             The unit.
         """
         column = self.index(column)
         return self.units[column]
 
     def set_unit(self, unit, column):
         """Set the unit of a column.
 
         Parameters
         ----------
-        unit: string
+        unit: str
             The new unit to be used for the column.
-        column: None, int, or string
+        column: None, int, or str
             A specification of a column.
             See self.index() for more information on how to specify a column.
         """
         column = self.index(column)
         self.units[column] = unit
         return column
 
     def set_units(self, units):
         """Set the units of all columns.
 
         Parameters
         ----------
-        units: list of string
+        units: list of str
             The new units to be used.
         """
         for c, u in enumerate(units):
             self.units[c] = u
 
     def format(self, column):
         """The format string of the column.
 
         Parameters
         ----------
-        column: None, int, or string
+        column: None, int, or str
             A specification of a column.
             See self.index() for more information on how to specify a column.
 
         Returns
         -------
-        format: string
+        format: str
             The format string.
         """
         column = self.index(column)
         return self.formats[column]
 
     def set_format(self, format, column):
         """Set the format string of a column.
 
         Parameters
         ----------
-        format: string
+        format: str
             The new format string to be used for the column.
-        column: None, int, or string
+        column: None, int, or str
             A specification of a column.
             See self.index() for more information on how to specify a column.
         """
         column = self.index(column)
         self.formats[column] = format
         return column
 
     def set_formats(self, formats):
         """Set the format strings of all columns.
 
         Parameters
         ----------
-        formats: string or list of string
+        formats: str or list of str
             The new format strings to be used.
             If only a single format is specified,
             then all columns get the same format.
         """
         if isinstance(formats, (list, tuple, np.ndarray)):
             for c, f in enumerate(formats):
                 self.formats[c] = f or '%g'
@@ -809,56 +820,56 @@
         return data
 
     def column_head(self, column):
         """The name, unit, and format of a column.
 
         Parameters
         ----------
-        column: None, int, or string
+        column: None, int, or str
             A specification of a column.
             See self.index() for more information on how to specify a column.
 
         Returns
         -------
-        name: string
+        name: str
             The column label.
-        unit: string
+        unit: str
             The unit.
-        format: string
+        format: str
             The format string.
         """
         column = self.index(column)
         return self.header[column][0], self.units[column], self.formats[column]
 
     def column_spec(self, column):
         """Full specification of a column with all its section names.
 
         Parameters
         ----------
-        column: int or string
+        column: int or str
             Specifies the column.
             See self.index() for more information on how to specify a column.
 
         Returns
         -------
-        s: string
+        s: str
             Full specification of the column by all its section names and its header name.
         """
         c = self.index(column)
         fh = [self.header[c][0]]
         for l in range(self.nsecs):
             fh.append(self.section(c, l+1)[0])
         return '>'.join(reversed(fh))
     
     def find_col(self, column):
         """Find the start and end index of a column specification.
         
         Parameters
         ----------
-        column: None, int, or string
+        column: None, int, or str
             A specification of a column.
             See self.index() for more information on how to specify a column.
 
         Returns
         -------
         c0: int or None
             A valid column index or None that is specified by `column`.
@@ -918,15 +929,15 @@
         return c0, c1
 
     def index(self, column):
         """The index of a column.
         
         Parameters
         ----------
-        column: None, int, or string
+        column: None, int, or str
             A specification of a column.
             - None: no column is specified
             - int: the index of the column (first column is zero), e.g. `index(2)`.
             - a string representing an integer is converted into the column index,
               e.g. `index('2')`
             - a string specifying a column by its header.
               Header names of descending hierarchy are separated by '>'.
@@ -940,15 +951,15 @@
         return c0
 
     def __contains__(self, column):
         """Check for existence of a column.
 
         Parameters
         ----------
-        column: None, int, or string
+        column: None, int, or str
             The column to be checked.
             See self.index() for more information on how to specify a column.
 
         Returns
         -------
         contains: bool
             True if `column` specifies an existing column key.
@@ -956,15 +967,15 @@
         return self.index(column) is not None
 
     def keys(self):
         """List of unique column keys for all available columns.
 
         Returns
         -------
-        keys: list of strings
+        keys: list of str
             List of unique column specifications.
         """
         return [self.column_spec(c) for c in range(self.columns())]
 
     def values(self):
         """List of column data corresponding to keys().
 
@@ -1090,15 +1101,15 @@
         return data
 
     def col(self, column):
         """A single column of the table.
 
         Parameters
         ----------
-        column: None, int, or string
+        column: None, int, or str
             The column to be returned.
             See self.index() for more information on how to specify a column.
 
         Returns
         -------
         table: TableData
             A TableData object with a single column.
@@ -1107,26 +1118,26 @@
         c = self.index(column)
         data.append(*self.column_head(c))
         data.data = [self.data[c]]
         data.nsecs = 0
         return data
 
     def __call__(self, column):
-        """A single column of the table as a numpy array.
+        """A single column of the table as a ndarray.
 
         Parameters
         ----------
-        column: None, int, or string
+        column: None, int, or str
             The column to be returned.
             See self.index() for more information on how to specify a column.
 
         Returns
         -------
-        data: 1-D array
-            Content of the specified column as a numpy array.
+        data: 1-D ndarray
+            Content of the specified column as a ndarray.
         """
         c = self.index(column)
         return np.asarray(self.data[c])
 
     def __setupkey(self, key):
         """Helper function that turns a key into row and column indices.
 
@@ -1184,15 +1195,15 @@
             Columns can be specified by index or name,
             see `index()` for details.
 
         Returns
         -------
         data:
             - A single data value if a single row and a single column is specified.
-            - An array of data elements if a single single column is specified.
+            - A ndarray of data elements if a single single column is specified.
             - A TableData object for multiple columns.
             - None if no row is selected (e.g. by a logical index that nowhere is True)
 
         Raises
         ------
         IndexError:
             If an invalid column was specified.
@@ -1323,27 +1334,27 @@
                 self.shape = (self.rows(), self.columns())
         else:
             for c in cols:
                 del self.data[c][row_indices]
             self.shape = (self.rows(), self.columns())
 
     def array(self, row=None):
-        """The table data as a numpy array.
+        """The table data as a ndarray.
 
         Parameters
         ----------
         row: int or None
-            If specified, a 1D array of that row will be returned.
+            If specified, a 1D ndarray of that row will be returned.
 
         Returns
         -------
         data: 2D or 1D ndarray
             If no row is specified, the data content of the entire table
-            as a 2D numpy array (rows first).
-            If a row is specified, a 1D array of that row.
+            as a 2D ndarray (rows first).
+            If a row is specified, a 1D ndarray of that row.
         """
         if row is None:
             return np.array(self.data).T
         else:
             return np.array([d[row] for d in self.data])
 
     def data_frame(self):
@@ -1352,23 +1363,23 @@
         Returns
         -------
         data: pandas.DataFrame
             A pandas DataFrame of the whole table.
         """
         return pd.DataFrame(self.dict())
 
-    def dicts(self, raw_values=True, missing='-'):
+    def dicts(self, raw_values=True, missing=default_missing_str):
         """The table as a list of dictionaries.
 
         Parameters
         ----------
         raw_values: bool
             If True, use raw table values as values,
             else format the values and add unit string.
-        missing: string
+        missing: str
             String indicating non-existing data elements.
 
         Returns
         -------
         table: list of dict
             For each row of the table a dictionary with header as key.
         """
@@ -1405,22 +1416,22 @@
     def append_data(self, data, column=None):
         """Append data elements to successive columns.
 
         The current column is set behid the added columns.
 
         Parameters
         ----------
-        data: float, int, string, etc. or list thereof or list of list thereof
+        data: float, int, str, etc. or list thereof or list of list thereof
             Data values to be appended to successive column.
             - A single value is simply appened to the specified column of the table.
             - A 1D-list of values is appended to successive columns of the table
               starting with the specified column.
             - The columns of a 2D-list of values (second index) are appended
               to successive columns of the table starting with the specified column.
-        column: None, int, or string
+        column: None, int, or str
             The first column to which the data should be appended.
             If None, append to the current column.
             See self.index() for more information on how to specify a column.
         """
         column = self.index(column)
         if column is None:
             column = self.setcol
@@ -1446,17 +1457,17 @@
     def append_data_column(self, data, column=None):
         """Append data elements to a column.
 
         The current column is incremented by one.
 
         Parameters
         ----------
-        data: float, int, string, etc. or list thereof
+        data: float, int, str, etc. or list thereof
             Data values to be appended to a column.
-        column: None, int, or string
+        column: None, int, or str
             The column to which the data should be appended.
             If None, append to the current column.
             See self.index() for more information on how to specify a column.
         """
         column = self.index(column)
         if column is None:
             column = self.setcol
@@ -1470,15 +1481,15 @@
         self.shape = (self.rows(), self.columns())
 
     def set_column(self, column):
         """Set the column where to add data.
 
         Parameters
         ----------
-        column: int or string
+        column: int or str
             The column to which data elements should be appended.
             See self.index() for more information on how to specify a column.
 
         Raises
         ------
         IndexError:
             If an invalid column was specified.
@@ -1513,15 +1524,15 @@
         self.shape = (self.rows(), self.columns())
                 
     def sort(self, columns, reverse=False):
         """Sort the table rows in place.
 
         Parameters
         ----------
-        columns: int or string or list of int or string
+        columns: int or str or list of int or str
             A column specifier or a list of column specifiers of the columns
             to be sorted.
         reverse: boolean
             If `True` sort in descending order.
 
         Raises
         ------
@@ -1602,32 +1613,32 @@
                 ds.append_data(np.max(data), dc)
                 ds.append_data(len(data), dc)
                 dc += 1
         ds.nsecs = self.nsecs
         ds.shape = (ds.rows(), ds.columns())
         return ds
 
-    def key_value(self, row, col, missing='-'):
+    def key_value(self, row, col, missing=default_missing_str):
         """A data element returned as a key-value pair.
 
         Parameters
         ----------
         row: int
             Specifies the row from which the data element should be retrieved.
-        col: None, int, or string
+        col: None, int, or str
             A specification of a column.
             See self.index() for more information on how to specify a column.
-        missing: string
+        missing: str
             String indicating non-existing data elements.
 
         Returns
         -------
-        key: string
+        key: str
             Header label of the column
-        value: string
+        value: str
             A textual representation of the data element according to the format
             of the column, followed by the unit of the column.
         """
         col = self.index(col)
         if col is None:
             return ''
         if isinstance(self.data[col][row], (float, np.floating)) and m.isnan(self.data[col][row]):
@@ -1642,15 +1653,15 @@
     def hide(self, column):
         """Hide a column or a range of columns.
 
         Hidden columns will not be printed out by the write() function.
 
         Parameters
         ----------
-        column: int or string
+        column: int or str
             The column to be hidden.
             See self.index() for more information on how to specify a column.
         """
         c0, c1 = self.find_col(column)
         if c0 is not None:
             for c in range(c0, c1):
                 self.hidden[c] = True
@@ -1659,82 +1670,83 @@
         """Hide all columns.
 
         Hidden columns will not be printed out by the write() function.
         """
         for c in range(len(self.hidden)):
             self.hidden[c] = True
 
-    def hide_empty_columns(self, missing='-'):
+    def hide_empty_columns(self, missing=default_missing_inputs):
         """Hide all columns that do not contain data.
 
         Hidden columns will not be printed out by the write() function.
 
         Parameters
         ----------
-        missing: string
-            String indicating missing data.
+        missing: list of str
+            Strings indicating missing data.
         """
         for c in range(len(self.data)):
             # check for empty column:
             isempty = True
             for v in self.data[c]:
                 if isinstance(v, (float, np.floating)):
                     if not m.isnan(v):
                         isempty = False
                         break
                 else:
-                    if v != missing:
+                    if not v in missing:
                         isempty = False
                         break
             if isempty:
                 self.hidden[c] = True
 
     def show(self, column):
         """Show a column or a range of columns.
 
         Undoes hiding of a column.
 
         Parameters
         ----------
-        column: int or string
+        column: int or str
             The column to be shown.
             See self.index() for more information on how to specify a column.
         """
         c0, c1 = self.find_col(column)
         if c0 is not None:
             for c in range(c0, c1):
                 self.hidden[c] = False
 
     def write(self, fh=sys.stdout, table_format=None, delimiter=None,
               unit_style=None, column_numbers=None, sections=None,
-              align_columns=None, shrink_width=True, missing='-',
-              center_columns=False, latex_label_command='', latex_merge_std=False):
+              align_columns=None, shrink_width=True,
+              missing=default_missing_str, center_columns=False,
+              latex_label_command='', latex_merge_std=False):
         """Write the table to a file or stream.
 
         Parameters
         ----------
         fh: filename or stream
             If not a stream, the file with name `fh` is opened.
             If `fh` does not have an extension,
             the `table_format` is appended as an extension.
             Otherwise `fh` is used as a stream for writing.
-        table_format: None or string
+        table_format: None or str
             The format to be used for output.
             One of 'out', 'dat', 'ascii', 'csv', 'rtai', 'md', 'tex', 'html'.
             If None or 'auto' then the format is set to the extension of the filename given by `fh`.
             If `fh` is a stream the format is set to 'dat'.
-        delimiter: string
+        delimiter: str
             String or character separating columns, if supported by the `table_format`.
             If None or 'auto' use the default for the specified `table_format`.
-        unit_style: None or string
+        unit_style: None or str
             - None or 'auto': use default of the specified `table_format`.
             - 'row': write an extra row to the table header specifying the units of the columns.
             - 'header': add the units to the column headers.
             - 'none': do not specify the units.
-        column_numbers: string or None
+        column_numbers: str or None
             Add a row specifying the column index:
             - 'index': indices are integers, first column is 0.
             - 'num': indices are integers, first column is 1.
             - 'aa': use 'a', 'b', 'c', ..., 'z', 'aa', 'ab', ... for indexing
             - 'aa': use 'A', 'B', 'C', ..., 'Z', 'AA', 'AB', ... for indexing
             - None or 'none': do not add a row with column indices
             TableData.column_numbering is a list with the supported styles.
@@ -1744,28 +1756,28 @@
         align_columns: boolean
             - `True`: set width of column formats to make them align.
             - `False`: set width of column formats to 0 - no unnecessary spaces.
             - None or 'auto': Use default of the selected `table_format`.
         shrink_width: boolean
             If `True` disregard width specified by the format strings,
             such that columns can become narrower.
-        missing: string
+        missing: str
             Indicate missing data by this string.
         center_columns: boolean
             If True center all columns (markdown, html, and latex).
-        latex_label_command: string
+        latex_label_command: str
             LaTeX command for formatting header labels.
             E.g. 'textbf' for making the header labels bold.
-        latex_merge_std: string
+        latex_merge_std: str
             Merge header of columns with standard deviations with previous column
             (LaTeX tables only).
 
         Returns
         -------
-        file_name: string or None
+        file_name: str or None
             The full name of the file into which the data were written.
 
         Supported file formats
         ----------------------
         
         ## `dat`: data text file
         ``` plain
@@ -2429,28 +2441,28 @@
 
 
     def write_file_stream(self, basename, file_name, **kwargs):
         """Write table to file or stream and return appropriate file name.
 
         Parameters
         ----------
-        basename: string or stream
-            If string, path and basename of file.
+        basename: str or stream
+            If str, path and basename of file.
             `file_name` and an extension are appended.
             If stream, write table data into this stream.
-        file_name: string
+        file_name: str
             Name of file that is appended to a base path or `basename`.
         kwargs:
             Arguments passed on to `TableData.write()`.
             In particular, 'table_format' is used to the set the file extension
             that is appended to the returned `file_name`.
 
         Returns
         -------
-        file_name: string
+        file_name: str
             Path and full name of the written file in case of `basename`
             being a string. Otherwise, the file name and extension that
             should be appended to a base path.
         """
         if hasattr(basename, 'write'):
             table_format = kwargs.get('table_format', None)
             if table_format is None or table_format == 'auto':
@@ -2467,25 +2479,26 @@
         """Write table to a string.
         """
         stream = StringIO()
         self.write(stream, table_format='out')
         return stream.getvalue()
                 
 
-    def load(self, fh, missing='-'):
+    def load(self, fh, missing=default_missing_inputs):
         """Load table from file or stream.
 
         File type and properties are automatically inferred.
 
         Parameters
         ----------
-        fh: filename or stream
+        fh: str or stream
             If not a stream, the file with name `fh` is opened for reading.
-        missing: string
-            Missing data are indicated by this string.
+        missing: str or list of str
+            Missing data are indicated by this string and
+            are translated to np.nan.
 
         Raises
         ------
         FileNotFoundError:
             If `fh` is a path that does not exist.
         """
 
@@ -2520,28 +2533,36 @@
                     if k == len(cols)-1:
                         c = c.rstrip('|')
                     cs = c.strip()
                     colss.append(cs)
                     indicess.append(i)
             return colss, indicess
 
-        def read_data_line(line, sep, post, precd, alld, numc, exped, fixed, strf, missing):
+        def read_data_line(line, sep, post, precd, alld, numc, exped,
+                           fixed, strf, missing, nans):
             # read line:
             cols = []
             if sep is None:
                 cols = [m.group(0) for m in re.finditer(r'\S+', line.strip())]
             else:
-                seps = r'[^'+re.escape(sep)+']+'
-                cols = [m.group(0).strip() for m in re.finditer(seps, line.strip())]
-                cols[0] = cols[0].lstrip('|').lstrip()
-                cols[-1] = cols[-1].rstrip('|').rstrip()
-            cols = [c for c in cols if c not in '|']
+                if sep.isspace():
+                    seps = r'[^'+re.escape(sep)+']+'
+                    cols = [m.group(0) for m in re.finditer(seps, line.strip())]
+                else:
+                    cols = line.split(sep)
+                    if len(cols) > 0 and len(cols[0]) == 0:
+                        cols = cols[1:]
+                    if len(cols) > 0 and len(cols[-1]) == 0:
+                        cols = cols[:-1]
+                if len(cols) > 0:
+                    cols[0] = cols[0].lstrip('|').lstrip()
+                    cols[-1] = cols[-1].rstrip('|').rstrip()
+            cols = [c.strip() for c in cols if c != '|']
             # read columns:
             for k, c in enumerate(cols):
-                c = c.strip()
                 try:
                     v = float(c)
                     ad = 0
                     ve = c.split('e')
                     if len(ve) <= 1:
                         exped[k] = False
                     else:
@@ -2558,24 +2579,27 @@
                         prec += len(vc[1].rstrip('0'))
                     if precd[k] < prec:
                         precd[k] = prec
                     if alld[k] < ad:
                         alld[k] = ad
                     numc[k] = True
                 except ValueError:
-                    if c == missing:
+                    if c in missing:
                         v = np.nan
+                        nans[k] = c
                     else:
                         strf[k] = True
                         if alld[k] < len(c):
                             alld[k] = len(c)
                         v = c
                 self.append_data(v, k)
 
         # initialize:
+        if isinstance(missing, str):
+            missing = [missing]
         self.data = []
         self.shape = (0, 0)
         self.header = []
         self.nsecs = 0
         self.units = []
         self.formats = []
         self.hidden = []
@@ -2768,86 +2792,102 @@
         post = np.zeros(colnum)
         precd = np.zeros(colnum)
         alld = np.zeros(colnum)
         numc = [False] * colnum
         exped = [True] * colnum
         fixed = [True] * colnum
         strf = [False] * colnum
+        nans = [None] * colnum
         for line in data:
-            read_data_line(line, sep, post, precd, alld, numc, exped, fixed, strf, missing)
+            read_data_line(line, sep, post, precd, alld, numc, exped, fixed,
+                           strf, missing, nans)
         # read remaining data:
         for line in fh:
             line = line.rstrip()
             if table_format == 'tex':
                 if r'\end{tabular' in line or r'\hline' in line:
                     break
                 line = line.rstrip(r'\\')
             if (line[0:3] == '|--' or line[0:3] == '|:-') and \
                 (line[-3:] == '--|' or line[-3:] == '-:|'):
                 break
             if line[0:3] == 'RTD':
                 line = line[3:]
-            read_data_line(line, sep, post, precd, alld, numc, exped, fixed, strf, missing)
+            read_data_line(line, sep, post, precd, alld, numc, exped, fixed,
+                           strf, missing, nans)
         # set formats:
         for k in range(len(alld)):
             if strf[k]:
                 self.set_format('%%-%ds' % alld[k], k)
+                # make sure all elements are strings:
+                for i in range(len(self.data[k])):
+                    if self.data[k][i] is np.nan:
+                        self.data[k][i] = nans[k]
+                    else:
+                        self.data[k][i] = str(self.data[k][i])
             elif exped[k]:
                 self.set_format('%%%d.%de' % (alld[k], post[k]), k)
             elif fixed[k]:
                 self.set_format('%%%d.%df' % (alld[k], post[k]), k)
             else:
                 self.set_format('%%%d.%dg' % (alld[k], precd[k]), k)
         # close file:
         if own_file:
             fh.close()
 
 
-def write(fh, data, header, units=None, formats=None, table_format=None, delimiter=None,
-              unit_style=None, column_numbers=None, sections=None,
-              align_columns=None, shrink_width=True, missing='-',
-              center_columns=False, latex_label_command='', latex_merge_std=False):
+def write(fh, data, header, units=None, formats=None,
+          table_format=None, delimiter=None, unit_style=None,
+          column_numbers=None, sections=None, align_columns=None,
+          shrink_width=True, missing=default_missing_str,
+          center_columns=False, latex_label_command='',
+          latex_merge_std=False):
     """Construct table and write to file.
 
     Parameters
     ----------
     fh: filename or stream
         If not a stream, the file with name `fh` is opened.
         If `fh` does not have an extension,
         the `table_format` is appended as an extension.
         Otherwise `fh` is used as a stream for writing.
-    data: 1-D or 2-D array of data
+    data: 1-D or 2-D ndarray of data
           The data of the table.
-    header: list of string
+    header: list of str
         Header labels for each column.
-    units: list of string, optional
+    units: list of str, optional
         Unit strings for each column.
-    formats: string or list of string, optional
+    formats: str or list of str, optional
         Format strings for each column. If only a single format string is
         given, then all columns are initialized with this format string.
 
     See `TableData.write()` for a description of all other parameters.
 
     Example
     -------
     ```
     write(sys.stdout, np.random.randn(4,3), ['aaa', 'bbb', 'ccc'], units=['m', 's', 'g'], formats='%.2f')
     ```
     """
     td = TableData(data, header, units, formats)
     td.write(fh, table_format=table_format, unit_style=unit_style,
-             column_numbers=column_numbers, missing=missing, shrink_width=shrink_width,
-             delimiter=delimiter, align_columns=align_columns, sections=sections,
-             latex_label_command=latex_label_command, latex_merge_std=latex_merge_std)
+             column_numbers=column_numbers, missing=missing,
+             shrink_width=shrink_width, delimiter=delimiter,
+             align_columns=align_columns, sections=sections,
+             latex_label_command=latex_label_command,
+             latex_merge_std=latex_merge_std)
 
     
 def add_write_table_config(cfg, table_format=None, delimiter=None,
-                           unit_style=None, column_numbers=None, sections=None,
-                           align_columns=None, shrink_width=True, missing='-',
-                           center_columns=False, latex_label_command='', latex_merge_std=False):
+                           unit_style=None, column_numbers=None,
+                           sections=None, align_columns=None,
+                           shrink_width=True, missing='-',
+                           center_columns=False,
+                           latex_label_command='',
+                           latex_merge_std=False):
     """Add parameter specifying how to write a table to a file as a new
 section to a configuration.
 
     Parameters
     ----------
     cfg: ConfigFile
         The configuration.
@@ -2902,20 +2942,20 @@
 
 
 def latex_unit(unit):
     """Translate unit string into SIunit LaTeX code.
     
     Parameters
     ----------
-    unit: string
+    unit: str
         String enoting a unit.
         
     Returns
     -------
-    unit: string
+    unit: str
         Unit string as valid LaTeX code.
     """
     si_prefixes = {'y': '\\yocto',
                   'z': '\\zepto',
                   'a': '\\atto',
                   'f': '\\femto',
                   'p': '\\pico',
@@ -3019,20 +3059,20 @@
 
     Inspired by https://stackoverflow.com/a/37604105
 
     Parameters
     ----------
     n: int
         An integer to be converted into alphabetical representation.
-    a: string ('a' or 'A')
+    a: str ('a' or 'A')
         Use upper or lower case characters.
 
     Returns
     -------
-    ns: string
+    ns: str
         Alphabetical represtnation of an integer.
     """
     d, m = divmod(n, 26)
     bm = chr(ord(a)+m)
     return index2aa(d-1, a) + bm if d else bm
 
 
@@ -3041,15 +3081,15 @@
 
     The alphabetical representation 'a', 'b', 'c', ..., 'z',
     'aa', 'ab', 'ac', ..., 'az', 'ba', 'bb', ...
     is converted to an index starting with 0.
 
     Parameters
     ----------
-    s: string
+    s: str
         Alphabetical representation of an index.
 
     Returns
     -------
     index: int
         The corresponding index.
```

### Comparing `thunderlab-1.1.0/src/thunderlab/voronoi.py` & `thunderlab-1.2.0/src/thunderlab/voronoi.py`

 * *Files identical despite different names*

### Comparing `thunderlab-1.1.0/src/thunderlab.egg-info/PKG-INFO` & `thunderlab-1.2.0/src/thunderlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thunderlab
-Version: 1.1.0
+Version: 1.2.0
 Summary: Algorithms and scripts for analyzing recordings of electric fish waveforms.
 Author: Jörg Henninger, Jan Grewe, Fabian Sinz
 Author-email: Jan Benda <jan.benda@uni-tuebingen.de>
 Maintainer-email: Jan Benda <jan.benda@uni-tuebingen.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -744,15 +744,15 @@
 
 
 ## Software
 
 The ThunderLab package provides the following software:
 
 - [`convertdata`](https://bendalab.github.io/thunderlab/api/convertdata/): Convert data from various file formats to audio files.
-
+- [`multivariateexplorer`](https://bendalab.github.io/thunderlab/api/multivariateexplorer.html): Simple GUI for viewing and exploring multivariate data. [More](docs/multivariateexplorer/index.html)
 
 
 ## Algorithms
 
 Click on the modules for more information.
 
 ### Input/output
@@ -764,15 +764,14 @@
 - [`consoleinput`](https://bendalab.github.io/thunderlab/api/consoleinput.html): User input from console.
 
 ### Basic data analysis
 
 - [`eventdetection`](https://bendalab.github.io/thunderlab/api/eventdetection.html): Detect and hande peaks and troughs as well as threshold crossings in data arrays.
 - [`powerspectrum`](https://bendalab.github.io/thunderlab/api/powerspectrum.html): Compute and plot powerspectra and spectrograms for a given minimum frequency resolution.
 - [`voronoi`](https://bendalab.github.io/thunderlab/api/voronoi.html): Analyse Voronoi diagrams based on scipy.spatial.
-- [`multivariateexplorer`](https://bendalab.github.io/thunderlab/api/multivariateexplorer.html): Simple GUI for viewing and exploring multivariate data.
 
 
 ## Used by
 
 - [thunderfish](https://github.com/bendalab/thunderfish): Algorithms and programs for analysing electric field recordings of weakly electric fish.
 - [audian](https://github.com/bendalab/audian) Python-based GUI for
 viewing and analyzing recordings of animal vocalizations.
```

### Comparing `thunderlab-1.1.0/src/thunderlab.egg-info/SOURCES.txt` & `thunderlab-1.2.0/src/thunderlab.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -21,10 +21,11 @@
 src/thunderlab.egg-info/top_level.txt
 tests/test_configfile.py
 tests/test_consoleinput.py
 tests/test_convertdata.py
 tests/test_dataloader.py
 tests/test_datawriter.py
 tests/test_eventdetection.py
+tests/test_multivariateexplorer.py
 tests/test_powerspectrum.py
 tests/test_tabledata.py
 tests/test_voronoi.py
```

### Comparing `thunderlab-1.1.0/tests/test_configfile.py` & `thunderlab-1.2.0/tests/test_configfile.py`

 * *Files identical despite different names*

### Comparing `thunderlab-1.1.0/tests/test_consoleinput.py` & `thunderlab-1.2.0/tests/test_consoleinput.py`

 * *Files identical despite different names*

### Comparing `thunderlab-1.1.0/tests/test_convertdata.py` & `thunderlab-1.2.0/tests/test_convertdata.py`

 * *Files identical despite different names*

### Comparing `thunderlab-1.1.0/tests/test_dataloader.py` & `thunderlab-1.2.0/tests/test_dataloader.py`

 * *Files identical despite different names*

### Comparing `thunderlab-1.1.0/tests/test_datawriter.py` & `thunderlab-1.2.0/tests/test_datawriter.py`

 * *Files identical despite different names*

### Comparing `thunderlab-1.1.0/tests/test_eventdetection.py` & `thunderlab-1.2.0/tests/test_eventdetection.py`

 * *Files identical despite different names*

### Comparing `thunderlab-1.1.0/tests/test_powerspectrum.py` & `thunderlab-1.2.0/tests/test_powerspectrum.py`

 * *Files identical despite different names*

### Comparing `thunderlab-1.1.0/tests/test_tabledata.py` & `thunderlab-1.2.0/tests/test_tabledata.py`

 * *Files identical despite different names*

### Comparing `thunderlab-1.1.0/tests/test_voronoi.py` & `thunderlab-1.2.0/tests/test_voronoi.py`

 * *Files identical despite different names*

