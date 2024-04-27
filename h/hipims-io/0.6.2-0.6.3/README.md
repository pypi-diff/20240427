# Comparing `tmp/hipims_io-0.6.2.tar.gz` & `tmp/hipims_io-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hipims_io-0.6.2.tar", last modified: Tue May 17 17:32:28 2022, max compression
+gzip compressed data, was "dist/hipims_io-0.6.3.tar", last modified: Sat Apr 27 15:05:05 2024, max compression
```

## Comparing `hipims_io-0.6.2.tar` & `hipims_io-0.6.3.tar`

### file list

```diff
@@ -1,24 +1,29 @@
-drwxr-xr-x   0 ming       (502) staff       (20)        0 2022-05-17 17:32:28.000000 hipims_io-0.6.2/
--rw-r--r--   0 ming       (502) staff       (20)     1073 2020-04-01 16:52:05.000000 hipims_io-0.6.2/LICENSE.txt
--rw-r--r--   0 ming       (502) staff       (20)      157 2020-04-16 11:34:13.000000 hipims_io-0.6.2/MANIFEST.in
--rw-r--r--   0 ming       (502) staff       (20)     4425 2022-05-17 17:32:28.000000 hipims_io-0.6.2/PKG-INFO
--rw-r--r--   0 ming       (502) staff       (20)     3134 2022-03-24 17:16:29.000000 hipims_io-0.6.2/README.md
-drwxr-xr-x   0 ming       (502) staff       (20)        0 2022-05-17 17:32:28.000000 hipims_io-0.6.2/hipims_io/
--rw-r--r--   0 ming       (502) staff       (20)    19532 2022-03-22 14:31:04.000000 hipims_io-0.6.2/hipims_io/Boundary.py
--rw-r--r--   0 ming       (502) staff       (20)    52898 2022-05-17 15:53:33.000000 hipims_io-0.6.2/hipims_io/InputHipims.py
--rw-r--r--   0 ming       (502) staff       (20)     2345 2022-03-22 14:31:47.000000 hipims_io-0.6.2/hipims_io/Landcover.py
--rw-r--r--   0 ming       (502) staff       (20)    23916 2022-03-28 16:50:03.000000 hipims_io-0.6.2/hipims_io/OutputHipims.py
--rw-r--r--   0 ming       (502) staff       (20)    10938 2022-03-22 14:30:23.000000 hipims_io-0.6.2/hipims_io/Rainfall.py
--rw-r--r--   0 ming       (502) staff       (20)    11331 2022-03-24 17:16:29.000000 hipims_io-0.6.2/hipims_io/Summary.py
--rw-r--r--   0 ming       (502) staff       (20)      587 2022-03-22 14:41:38.000000 hipims_io-0.6.2/hipims_io/__init__.py
--rw-r--r--   0 ming       (502) staff       (20)     3841 2022-03-22 14:41:57.000000 hipims_io-0.6.2/hipims_io/demo_functions.py
--rw-r--r--   0 ming       (502) staff       (20)    18000 2022-05-17 17:17:00.000000 hipims_io-0.6.2/hipims_io/indep_functions.py
--rw-r--r--   0 ming       (502) staff       (20)    10023 2022-03-22 14:45:15.000000 hipims_io-0.6.2/hipims_io/rainfall_processing.py
-drwxr-xr-x   0 ming       (502) staff       (20)        0 2022-05-17 17:32:28.000000 hipims_io-0.6.2/hipims_io.egg-info/
--rw-r--r--   0 ming       (502) staff       (20)     4425 2022-05-17 17:32:27.000000 hipims_io-0.6.2/hipims_io.egg-info/PKG-INFO
--rw-r--r--   0 ming       (502) staff       (20)      457 2022-05-17 17:32:27.000000 hipims_io-0.6.2/hipims_io.egg-info/SOURCES.txt
--rw-r--r--   0 ming       (502) staff       (20)        1 2022-05-17 17:32:27.000000 hipims_io-0.6.2/hipims_io.egg-info/dependency_links.txt
--rw-r--r--   0 ming       (502) staff       (20)       72 2022-05-17 17:32:27.000000 hipims_io-0.6.2/hipims_io.egg-info/requires.txt
--rw-r--r--   0 ming       (502) staff       (20)       10 2022-05-17 17:32:27.000000 hipims_io-0.6.2/hipims_io.egg-info/top_level.txt
--rw-r--r--   0 ming       (502) staff       (20)       38 2022-05-17 17:32:28.000000 hipims_io-0.6.2/setup.cfg
--rw-r--r--   0 ming       (502) staff       (20)     2387 2022-05-17 17:26:30.000000 hipims_io-0.6.2/setup.py
+drwxr-xr-x   0 ming       (502) staff       (20)        0 2024-04-27 15:05:05.457329 hipims_io-0.6.3/
+-rw-r--r--   0 ming       (502) staff       (20)     1073 2020-04-01 16:52:05.000000 hipims_io-0.6.3/LICENSE.txt
+-rw-r--r--   0 ming       (502) staff       (20)      157 2020-04-16 11:34:13.000000 hipims_io-0.6.3/MANIFEST.in
+-rw-r--r--   0 ming       (502) staff       (20)     4425 2024-04-27 15:05:05.456848 hipims_io-0.6.3/PKG-INFO
+-rw-r--r--   0 ming       (502) staff       (20)     3134 2022-03-24 17:16:29.000000 hipims_io-0.6.3/README.md
+drwxr-xr-x   0 ming       (502) staff       (20)        0 2024-04-27 15:05:05.450790 hipims_io-0.6.3/hipims_io/
+-rw-r--r--   0 ming       (502) staff       (20)    19602 2024-04-27 15:02:46.000000 hipims_io-0.6.3/hipims_io/Boundary.py
+-rw-r--r--   0 ming       (502) staff       (20)    52898 2022-05-17 15:53:33.000000 hipims_io-0.6.3/hipims_io/InputHipims.py
+-rw-r--r--   0 ming       (502) staff       (20)     2345 2022-03-22 14:31:47.000000 hipims_io-0.6.3/hipims_io/Landcover.py
+-rw-r--r--   0 ming       (502) staff       (20)    23916 2022-03-28 16:50:03.000000 hipims_io-0.6.3/hipims_io/OutputHipims.py
+-rw-r--r--   0 ming       (502) staff       (20)    10990 2024-04-27 14:19:04.000000 hipims_io-0.6.3/hipims_io/Rainfall.py
+-rw-r--r--   0 ming       (502) staff       (20)    11331 2022-03-24 17:16:29.000000 hipims_io-0.6.3/hipims_io/Summary.py
+-rw-r--r--   0 ming       (502) staff       (20)      587 2022-03-22 14:41:38.000000 hipims_io-0.6.3/hipims_io/__init__.py
+-rw-r--r--   0 ming       (502) staff       (20)     3841 2022-03-22 14:41:57.000000 hipims_io-0.6.3/hipims_io/demo_functions.py
+-rw-r--r--   0 ming       (502) staff       (20)    18000 2022-05-17 17:17:00.000000 hipims_io-0.6.3/hipims_io/indep_functions.py
+-rw-r--r--   0 ming       (502) staff       (20)    10023 2022-03-22 14:45:15.000000 hipims_io-0.6.3/hipims_io/rainfall_processing.py
+drwxr-xr-x   0 ming       (502) staff       (20)        0 2024-04-27 15:05:05.456000 hipims_io-0.6.3/hipims_io/sample/
+-rw-r--r--   0 ming       (502) staff       (20)    98722 2021-02-19 00:03:41.000000 hipims_io-0.6.3/hipims_io/sample/DEM.gz
+-rw-r--r--   0 ming       (502) staff       (20)      813 2021-02-19 00:03:41.000000 hipims_io-0.6.3/hipims_io/sample/landcover.gz
+-rw-r--r--   0 ming       (502) staff       (20)      813 2021-02-19 00:03:41.000000 hipims_io-0.6.3/hipims_io/sample/rain_mask.gz
+-rw-r--r--   0 ming       (502) staff       (20)      325 2021-02-19 00:03:41.000000 hipims_io-0.6.3/hipims_io/sample/rain_source.csv
+drwxr-xr-x   0 ming       (502) staff       (20)        0 2024-04-27 15:05:05.453185 hipims_io-0.6.3/hipims_io.egg-info/
+-rw-r--r--   0 ming       (502) staff       (20)     4425 2024-04-27 15:05:05.000000 hipims_io-0.6.3/hipims_io.egg-info/PKG-INFO
+-rw-r--r--   0 ming       (502) staff       (20)      574 2024-04-27 15:05:05.000000 hipims_io-0.6.3/hipims_io.egg-info/SOURCES.txt
+-rw-r--r--   0 ming       (502) staff       (20)        1 2024-04-27 15:05:05.000000 hipims_io-0.6.3/hipims_io.egg-info/dependency_links.txt
+-rw-r--r--   0 ming       (502) staff       (20)       72 2024-04-27 15:05:05.000000 hipims_io-0.6.3/hipims_io.egg-info/requires.txt
+-rw-r--r--   0 ming       (502) staff       (20)       10 2024-04-27 15:05:05.000000 hipims_io-0.6.3/hipims_io.egg-info/top_level.txt
+-rw-r--r--   0 ming       (502) staff       (20)       38 2024-04-27 15:05:05.457480 hipims_io-0.6.3/setup.cfg
+-rw-r--r--   0 ming       (502) staff       (20)     2387 2024-04-27 14:10:13.000000 hipims_io-0.6.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hipims_io-0.6.2/LICENSE.txt` & `hipims_io-0.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hipims_io-0.6.2/PKG-INFO` & `hipims_io-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipims_io
-Version: 0.6.2
+Version: 0.6.3
 Summary: To process input and output files of the HiPIMS model
 Home-page: https://github.com/mingxiaodong/hipims_io_python
 Author: Xiaodong Ming
 Author-email: x.ming@lboro.ac.uk
 License: LICENSE.txt
 Description: hipims_io
         --------
```

### Comparing `hipims_io-0.6.2/README.md` & `hipims_io-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `hipims_io-0.6.2/hipims_io/Boundary.py` & `hipims_io-0.6.3/hipims_io/Boundary.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,41 +239,45 @@
     data_table = pd.DataFrame(columns=['type', 'extent',
                                        'hSources', 'hUSources',
                                        'h_code', 'hU_code', 'name'])
     # set default outline boundary [0]
     if outline_boundary == 'fall':
         hSources = np.array([[0, 0], [1, 0]])
         hUSources = np.array([[0, 0, 0], [1, 0, 0]])
-        data_table = data_table.append({'type':'fall', 'extent':None,
-                                        'hSources':hSources,
-                                        'hUSources':hUSources},
-                                       ignore_index=True)
+        new_row = pd.DataFrame({'type':['fall'], 
+                                'extent':[None],
+                                'hSources':[hSources],
+                                'hUSources':[hUSources]})
     elif outline_boundary == 'rigid':
-        data_table = data_table.append({'type':'rigid', 'extent':None,
-                                        'hSources':None, 'hUSources':None},
-                                       ignore_index=True)
+        new_row = pd.DataFrame({'type':['rigid'], 
+                                'extent':[None],
+                                'hSources':[None], 
+                                'hUSources':[None]})
     elif outline_boundary == 'open':
-        data_table = data_table.append({'type':'open', 'extent':None,
-                                        'hSources':None, 'hUSources':None},
-                                       ignore_index=True)
+        new_row = pd.DataFrame({'type':['open'], 
+                                'extent':[None],
+                                'hSources':[None],
+                                'hUSources':[None]})
     else:
         raise ValueError("outline_boundary must be fall, open or rigid!")
+    data_table = pd.concat([data_table, new_row], ignore_index=True)
     data_table.name[0] = 'Outline boundary'
     # convert boundary_list to a dataframe
     if boundary_list is None:
         boundary_list = []
     for one_bound in boundary_list:
         # Only a bound with polyPoints can be regarded as a boundary
         # Otherwise it will be treated as the outline boundary
         bound_ind = data_table.shape[0]  # bound index
             # set extent
         if 'polyPoints' in one_bound.keys():
             bound_extent = np.array(one_bound['polyPoints'])
-            data_table = data_table.append({'extent':bound_extent, }, 
-                                           ignore_index=True)
+            new_row = pd.DataFrame({'extent':[bound_extent]})
+            data_table = pd.concat([data_table, new_row], 
+                                    ignore_index=True)
         else:
             bound_ind = 0
             print('polyPoints is not given in boundary_list[0],'
                   'set as outline boundary')
         if 'type' in one_bound.keys():
             bound_type = one_bound['type']
         else:
```

### Comparing `hipims_io-0.6.2/hipims_io/InputHipims.py` & `hipims_io-0.6.3/hipims_io/InputHipims.py`

 * *Files identical despite different names*

### Comparing `hipims_io-0.6.2/hipims_io/Landcover.py` & `hipims_io-0.6.3/hipims_io/Landcover.py`

 * *Files identical despite different names*

### Comparing `hipims_io-0.6.2/hipims_io/OutputHipims.py` & `hipims_io-0.6.3/hipims_io/OutputHipims.py`

 * *Files identical despite different names*

### Comparing `hipims_io-0.6.2/hipims_io/Rainfall.py` & `hipims_io-0.6.3/hipims_io/Rainfall.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,16 +193,17 @@
         """
         rain_rate_valid, mask_valid = self.get_valid_rain_rate()
         time_s = self.time_s
         cellsize = self.mask_header['cellsize']
         temporal_res = (time_s.max()-time_s.min())/(time_s.size-1) # seconds
         source_uniq, source_counts = np.unique(mask_valid, return_counts=True)
         num_source = source_uniq.size
-        mode_value = stats.mode(source_counts)
-        spatial_res = np.sqrt(mode_value[0][0])*cellsize
+        mode_value = stats.mode(source_counts)[0]
+        mode_value = np.array(mode_value).flatten()
+        spatial_res = np.sqrt(mode_value[0])*cellsize
         cell_mean = np.mean(rain_rate_valid, axis=1)
         # total value along time axis for a cell
         rain_total = np.trapz(cell_mean, x=time_s, axis=0)*1000 # mm
         rain_mean = rain_total/(time_s.max()-time_s.min())*3600 # mm/h
         cell_max = np.max(rain_rate_valid, axis=1)*3600*1000
         attrs = {}
         attrs['num_source'] = num_source
```

### Comparing `hipims_io-0.6.2/hipims_io/Summary.py` & `hipims_io-0.6.3/hipims_io/Summary.py`

 * *Files identical despite different names*

### Comparing `hipims_io-0.6.2/hipims_io/__init__.py` & `hipims_io-0.6.3/hipims_io/__init__.py`

 * *Files identical despite different names*

### Comparing `hipims_io-0.6.2/hipims_io/demo_functions.py` & `hipims_io-0.6.3/hipims_io/demo_functions.py`

 * *Files identical despite different names*

### Comparing `hipims_io-0.6.2/hipims_io/indep_functions.py` & `hipims_io-0.6.3/hipims_io/indep_functions.py`

 * *Files identical despite different names*

### Comparing `hipims_io-0.6.2/hipims_io/rainfall_processing.py` & `hipims_io-0.6.3/hipims_io/rainfall_processing.py`

 * *Files identical despite different names*

### Comparing `hipims_io-0.6.2/hipims_io.egg-info/PKG-INFO` & `hipims_io-0.6.3/hipims_io.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipims-io
-Version: 0.6.2
+Version: 0.6.3
 Summary: To process input and output files of the HiPIMS model
 Home-page: https://github.com/mingxiaodong/hipims_io_python
 Author: Xiaodong Ming
 Author-email: x.ming@lboro.ac.uk
 License: LICENSE.txt
 Description: hipims_io
         --------
```

### Comparing `hipims_io-0.6.2/setup.py` & `hipims_io-0.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from os import path
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
       name='hipims_io',
-      version='0.6.2',
+      version='0.6.3',
       description='To process input and output files of the HiPIMS model',
       url='https://github.com/mingxiaodong/hipims_io_python',
       author='Xiaodong Ming',
       author_email='x.ming@lboro.ac.uk',
       long_description=long_description,
       long_description_content_type='text/markdown',
       classifiers=['Development Status :: 3 - Alpha',
```

