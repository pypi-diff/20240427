# Comparing `tmp/tga_data_analysis-2.0.8.tar.gz` & `tmp/tga_data_analysis-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tga_data_analysis-2.0.8.tar", last modified: Wed Apr 24 01:56:50 2024, max compression
+gzip compressed data, was "tga_data_analysis-2.0.9.tar", last modified: Sat Apr 27 13:16:55 2024, max compression
```

## Comparing `tga_data_analysis-2.0.8.tar` & `tga_data_analysis-2.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:56:50.232911 tga_data_analysis-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-04-24 01:56:50.232911 tga_data_analysis-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-24 01:56:44.000000 tga_data_analysis-2.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-24 01:56:44.000000 tga_data_analysis-2.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 01:56:50.232911 tga_data_analysis-2.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:56:50.228911 tga_data_analysis-2.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:56:50.232911 tga_data_analysis-2.0.8/src/tga_data_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 01:56:44.000000 tga_data_analysis-2.0.8/src/tga_data_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-24 01:56:44.000000 tga_data_analysis-2.0.8/src/tga_data_analysis/kas_kinetics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-24 01:56:44.000000 tga_data_analysis-2.0.8/src/tga_data_analysis/measure.py
--rw-r--r--   0 runner    (1001) docker     (127)    27504 2024-04-24 01:56:44.000000 tga_data_analysis-2.0.8/src/tga_data_analysis/myfigure.py
--rw-r--r--   0 runner    (1001) docker     (127)    64541 2024-04-24 01:56:44.000000 tga_data_analysis-2.0.8/src/tga_data_analysis/tga.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:56:50.232911 tga_data_analysis-2.0.8/src/tga_data_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-04-24 01:56:50.000000 tga_data_analysis-2.0.8/src/tga_data_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-24 01:56:50.000000 tga_data_analysis-2.0.8/src/tga_data_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 01:56:50.000000 tga_data_analysis-2.0.8/src/tga_data_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-24 01:56:50.000000 tga_data_analysis-2.0.8/src/tga_data_analysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 01:56:50.000000 tga_data_analysis-2.0.8/src/tga_data_analysis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:56:50.232911 tga_data_analysis-2.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-24 01:56:44.000000 tga_data_analysis-2.0.8/tests/test_deconvolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-24 01:56:44.000000 tga_data_analysis-2.0.8/tests/test_kas_kinetics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-24 01:56:44.000000 tga_data_analysis-2.0.8/tests/test_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-24 01:56:44.000000 tga_data_analysis-2.0.8/tests/test_my_figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-24 01:56:44.000000 tga_data_analysis-2.0.8/tests/test_oxidation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-24 01:56:44.000000 tga_data_analysis-2.0.8/tests/test_proximate.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-24 01:56:44.000000 tga_data_analysis-2.0.8/tests/test_soliddist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:16:55.417639 tga_data_analysis-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-04-27 13:16:55.417639 tga_data_analysis-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 13:16:55.417639 tga_data_analysis-2.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:16:55.413639 tga_data_analysis-2.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:16:55.413639 tga_data_analysis-2.0.9/src/tga_data_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/src/tga_data_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/src/tga_data_analysis/kas_kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/src/tga_data_analysis/measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27504 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/src/tga_data_analysis/myfigure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64570 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/src/tga_data_analysis/tga.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:16:55.417639 tga_data_analysis-2.0.9/src/tga_data_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-04-27 13:16:55.000000 tga_data_analysis-2.0.9/src/tga_data_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-27 13:16:55.000000 tga_data_analysis-2.0.9/src/tga_data_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 13:16:55.000000 tga_data_analysis-2.0.9/src/tga_data_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-27 13:16:55.000000 tga_data_analysis-2.0.9/src/tga_data_analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 13:16:55.000000 tga_data_analysis-2.0.9/src/tga_data_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:16:55.417639 tga_data_analysis-2.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/tests/test_deconvolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/tests/test_kas_kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/tests/test_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/tests/test_my_figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/tests/test_oxidation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/tests/test_proximate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/tests/test_soliddist.py
```

### Comparing `tga_data_analysis-2.0.8/PKG-INFO` & `tga_data_analysis-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tga_data_analysis
-Version: 2.0.8
+Version: 2.0.9
 Summary: Tool for automatic analysis of multiple TGA results
 Author: Matteo Pecchi
 License: MIT
 Project-URL: Homepage, https://github.com/mpecchi/tga_data_analysis
 Project-URL: Documentation, https://tga-data-analysis.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tga_data_analysis-2.0.8/README.md` & `tga_data_analysis-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.8/pyproject.toml` & `tga_data_analysis-2.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tga_data_analysis"
-version = "2.0.8"
+version = "2.0.9"
 authors = [
     { name = "Matteo Pecchi"}
 ]
 description = "Tool for automatic analysis of multiple TGA results"
 readme = "README.md"
 license = { text = "MIT" }
 classifiers = [
```

### Comparing `tga_data_analysis-2.0.8/src/tga_data_analysis/kas_kinetics.py` & `tga_data_analysis-2.0.9/src/tga_data_analysis/kas_kinetics.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.8/src/tga_data_analysis/measure.py` & `tga_data_analysis-2.0.9/src/tga_data_analysis/measure.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.8/src/tga_data_analysis/myfigure.py` & `tga_data_analysis-2.0.9/src/tga_data_analysis/myfigure.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.8/src/tga_data_analysis/tga.py` & `tga_data_analysis-2.0.9/src/tga_data_analysis/tga.py`

 * *Files 1% similar despite different names*

```diff
@@ -418,15 +418,14 @@
             "out_path": out_path,
             "height": 3.2,
             "width": 3.2,
             "grid": self.plot_grid,
             "text_font": self.plot_font,
             "x_lab": f"T [{self.temp_symbol}]",
             "y_lab": self.tg_label,
-            "x_lim": self.temp_lim_dtg,
         }
         # Update kwargs with the default key-value pairs if the key is not present in kwargs
         kwargs = {**default_kwargs, **kwargs}
 
         myfig = MyFigure(
             rows=1,
             cols=1,
@@ -1345,15 +1344,16 @@
                 self.time.stk(f)[self.idx_moist.stk(f)],
                 self.mp_ar.stk(f)[self.idx_moist.stk(f)] - 5,
                 self.mp_ar.stk(f)[self.idx_moist.stk(f)] + 5,
                 linestyle=linestyles[f],
                 color=colors[f],
             )
 
-            if self.vm_db() < 99:
+            # only try to plot VM is the analysis includes it
+            if self.time_vm is not None:
                 mf.axs[0].vlines(
                     self.time.stk(f)[self.idx_vm.stk(f)],
                     self.temp.stk(f)[self.idx_vm.stk(f)] - 50,
                     self.temp.stk(f)[self.idx_vm.stk(f)] + 50,
                     linestyle=linestyles[f],
                     color=colors[f],
                 )
```

### Comparing `tga_data_analysis-2.0.8/src/tga_data_analysis.egg-info/PKG-INFO` & `tga_data_analysis-2.0.9/src/tga_data_analysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tga_data_analysis
-Version: 2.0.8
+Version: 2.0.9
 Summary: Tool for automatic analysis of multiple TGA results
 Author: Matteo Pecchi
 License: MIT
 Project-URL: Homepage, https://github.com/mpecchi/tga_data_analysis
 Project-URL: Documentation, https://tga-data-analysis.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tga_data_analysis-2.0.8/src/tga_data_analysis.egg-info/SOURCES.txt` & `tga_data_analysis-2.0.9/src/tga_data_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.8/tests/test_deconvolution.py` & `tga_data_analysis-2.0.9/tests/test_deconvolution.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.8/tests/test_kas_kinetics.py` & `tga_data_analysis-2.0.9/tests/test_kas_kinetics.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.8/tests/test_measure.py` & `tga_data_analysis-2.0.9/tests/test_measure.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.8/tests/test_my_figure.py` & `tga_data_analysis-2.0.9/tests/test_my_figure.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.8/tests/test_oxidation.py` & `tga_data_analysis-2.0.9/tests/test_oxidation.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.8/tests/test_proximate.py` & `tga_data_analysis-2.0.9/tests/test_proximate.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.8/tests/test_soliddist.py` & `tga_data_analysis-2.0.9/tests/test_soliddist.py`

 * *Files identical despite different names*

