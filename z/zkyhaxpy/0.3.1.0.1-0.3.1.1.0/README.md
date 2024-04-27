# Comparing `tmp/zkyhaxpy-0.3.1.0.1.tar.gz` & `tmp/zkyhaxpy-0.3.1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zkyhaxpy-0.3.1.0.1.tar", last modified: Sun Apr 14 16:07:11 2024, max compression
+gzip compressed data, was "zkyhaxpy-0.3.1.1.0.tar", last modified: Sat Apr 27 10:54:12 2024, max compression
```

## Comparing `zkyhaxpy-0.3.1.0.1.tar` & `zkyhaxpy-0.3.1.1.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 16:07:11.873611 zkyhaxpy-0.3.1.0.1/
--rw-rw-rw-   0        0        0     1088 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/LICENSE
--rw-rw-rw-   0        0        0      616 2024-04-14 16:07:11.873611 zkyhaxpy-0.3.1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      141 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-14 16:07:11.874611 zkyhaxpy-0.3.1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      703 2024-04-14 14:46:44.000000 zkyhaxpy-0.3.1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 16:07:11.861611 zkyhaxpy-0.3.1.0.1/zkyhaxpy/
--rw-rw-rw-   0        0        0        0 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/__init__.py
--rw-rw-rw-   0        0        0     1651 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/aws_tools.py
--rw-rw-rw-   0        0        0     2929 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/colab_tools.py
--rw-rw-rw-   0        0        0      875 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/console_tools.py
--rw-rw-rw-   0        0        0      623 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/dict_tools.py
--rw-rw-rw-   0        0        0     5115 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/dttm_tools.py
--rw-rw-rw-   0        0        0     3411 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/ftp_tools.py
--rw-rw-rw-   0        0        0      614 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/gcp_tools.py
--rw-rw-rw-   0        0        0    41927 2024-04-14 14:46:31.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/gis_tools.py
--rw-rw-rw-   0        0        0      348 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/hash_tools.py
--rw-rw-rw-   0        0        0      664 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/http_tools.py
--rw-rw-rw-   0        0        0     1280 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/img_tools.py
--rw-rw-rw-   0        0        0    13142 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/io_tools.py
--rw-rw-rw-   0        0        0     3515 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/json_tools.py
--rw-rw-rw-   0        0        0      179 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/jupyter_tools.py
--rw-rw-rw-   0        0        0     2002 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/log_tools.py
--rw-rw-rw-   0        0        0     6360 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/ml_tools.py
--rw-rw-rw-   0        0        0      281 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/mpl_tools.py
--rw-rw-rw-   0        0        0      652 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/multitask_tools.py
--rw-rw-rw-   0        0        0     2396 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/np_tools.py
--rw-rw-rw-   0        0        0     6709 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/pd_tools.py
--rw-rw-rw-   0        0        0     1822 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/skopt_tools.py
--rw-rw-rw-   0        0        0     1130 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/snippet_tools.py
--rw-rw-rw-   0        0        0      463 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/str_tools.py
--rw-rw-rw-   0        0        0     1838 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/timer_tools.py
--rw-rw-rw-   0        0        0      663 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/util_tools.py
-drwxrwxrwx   0        0        0        0 2024-04-14 16:07:11.872611 zkyhaxpy-0.3.1.0.1/zkyhaxpy.egg-info/
--rw-rw-rw-   0        0        0      616 2024-04-14 16:07:11.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      751 2024-04-14 16:07:11.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 16:07:11.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-14 16:07:11.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 10:54:12.246289 zkyhaxpy-0.3.1.1.0/
+-rw-rw-rw-   0        0        0     1088 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      616 2024-04-27 10:54:12.245289 zkyhaxpy-0.3.1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      141 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 10:54:12.246289 zkyhaxpy-0.3.1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      703 2024-04-27 10:52:31.000000 zkyhaxpy-0.3.1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:54:12.234289 zkyhaxpy-0.3.1.1.0/zkyhaxpy/
+-rw-rw-rw-   0        0        0        0 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/__init__.py
+-rw-rw-rw-   0        0        0     1651 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/aws_tools.py
+-rw-rw-rw-   0        0        0     2929 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/colab_tools.py
+-rw-rw-rw-   0        0        0      875 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/console_tools.py
+-rw-rw-rw-   0        0        0      623 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/dict_tools.py
+-rw-rw-rw-   0        0        0     5115 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/dttm_tools.py
+-rw-rw-rw-   0        0        0     3411 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/ftp_tools.py
+-rw-rw-rw-   0        0        0      614 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/gcp_tools.py
+-rw-rw-rw-   0        0        0    42777 2024-04-27 10:49:55.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/gis_tools.py
+-rw-rw-rw-   0        0        0      348 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/hash_tools.py
+-rw-rw-rw-   0        0        0      664 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/http_tools.py
+-rw-rw-rw-   0        0        0     1280 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/img_tools.py
+-rw-rw-rw-   0        0        0    13142 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/io_tools.py
+-rw-rw-rw-   0        0        0     3515 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/json_tools.py
+-rw-rw-rw-   0        0        0      179 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/jupyter_tools.py
+-rw-rw-rw-   0        0        0     2002 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/log_tools.py
+-rw-rw-rw-   0        0        0     6360 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/ml_tools.py
+-rw-rw-rw-   0        0        0      281 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/mpl_tools.py
+-rw-rw-rw-   0        0        0      652 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/multitask_tools.py
+-rw-rw-rw-   0        0        0     2396 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/np_tools.py
+-rw-rw-rw-   0        0        0     6709 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/pd_tools.py
+-rw-rw-rw-   0        0        0     1822 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/skopt_tools.py
+-rw-rw-rw-   0        0        0     1130 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/snippet_tools.py
+-rw-rw-rw-   0        0        0      463 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/str_tools.py
+-rw-rw-rw-   0        0        0     1838 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/timer_tools.py
+-rw-rw-rw-   0        0        0      663 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy/util_tools.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:54:12.245289 zkyhaxpy-0.3.1.1.0/zkyhaxpy.egg-info/
+-rw-rw-rw-   0        0        0      616 2024-04-27 10:54:12.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      751 2024-04-27 10:54:12.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 10:54:12.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-27 10:54:12.000000 zkyhaxpy-0.3.1.1.0/zkyhaxpy.egg-info/top_level.txt
```

### Comparing `zkyhaxpy-0.3.1.0.1/LICENSE` & `zkyhaxpy-0.3.1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.1.0.1/PKG-INFO` & `zkyhaxpy-0.3.1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zkyhaxpy
-Version: 0.3.1.0.1
+Version: 0.3.1.1.0
 Summary: A swiss-knife Data Science package for python
 Home-page: https://github.com/surasakcho/zkyhaxpy
 Author: Surasak Choedpasuporn
 Author-email: surasak.cho@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `zkyhaxpy-0.3.1.0.1/setup.py` & `zkyhaxpy-0.3.1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="zkyhaxpy",
-    version="0.3.1.0.1",
+    version="0.3.1.1.0",
     author="Surasak Choedpasuporn",
     author_email="surasak.cho@gmail.com",
     description="A swiss-knife Data Science package for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/surasakcho/zkyhaxpy",
     packages=setuptools.find_packages(),
```

### Comparing `zkyhaxpy-0.3.1.0.1/zkyhaxpy/aws_tools.py` & `zkyhaxpy-0.3.1.1.0/zkyhaxpy/aws_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.1.0.1/zkyhaxpy/colab_tools.py` & `zkyhaxpy-0.3.1.1.0/zkyhaxpy/colab_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.1.0.1/zkyhaxpy/console_tools.py` & `zkyhaxpy-0.3.1.1.0/zkyhaxpy/console_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.1.0.1/zkyhaxpy/dict_tools.py` & `zkyhaxpy-0.3.1.1.0/zkyhaxpy/dict_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.1.0.1/zkyhaxpy/dttm_tools.py` & `zkyhaxpy-0.3.1.1.0/zkyhaxpy/dttm_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.1.0.1/zkyhaxpy/ftp_tools.py` & `zkyhaxpy-0.3.1.1.0/zkyhaxpy/ftp_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.1.0.1/zkyhaxpy/gcp_tools.py` & `zkyhaxpy-0.3.1.1.0/zkyhaxpy/gcp_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.1.0.1/zkyhaxpy/gis_tools.py` & `zkyhaxpy-0.3.1.1.0/zkyhaxpy/gis_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -666,15 +666,15 @@
 
             
         elif (out_mem==False) & (out_raster_path==None):
             if tmp_folder==None:                                                
                 if os.path.exists('/tmp'):
                     out_raster_folder = os.path.join('/tmp', uuid.uuid4().hex)
                 else:
-                    out_raster_folder = os.path.join('c:', 'tmp', uuid.uuid4().hex)
+                    out_raster_folder = os.path.join(r'c:/tmp', uuid.uuid4().hex)
             else:                
                 out_raster_folder = os.path.join(tmp_folder, uuid.uuid4().hex)
             out_raster_path = os.path.join(out_raster_folder, f'rowcol_map_{os.path.basename(in_raster)}')
             io_tools.create_folders(out_raster_path)
             with rasterio.open(out_raster_path, 'w', **profile) as dst:
                 #row
                 dst.write(tmp_arr_row_col[0], 1)
@@ -1277,8 +1277,29 @@
             compress='lzw'
         )
 
         with rasterio.open(path_out, 'w', **profile) as ds_out:
             ds_out.write(arr_out, 1)
         print(f'{path_out} has been saved')
     return arr_out
-    
+    
+    
+    
+    
+def generate_grid(lat_min, lat_max, lon_min, lon_max, step_size_km=1):
+    '''
+    Generates a regular grid of latitude and longitude coordinates within the specified bounding box.
+    :param lat_min: Minimum latitude
+    :param lat_max: Maximum latitude
+    :param lon_min: Minimum longitude
+    :param lon_max: Maximum longitude
+    :param step_size_km: Spacing between grid points (default: 1 km)
+    :return: List of (latitude, longitude) pairs
+    '''
+    grid_points = []
+    step_size_deg = step_size_km / 111.32  # Approximate conversion from km to degrees
+    
+    for lat in np.arange(lat_min, lat_max, step_size_deg):
+        for lon in np.arange(lon_min, lon_max, step_size_deg):
+            grid_points.append((round(lat, 4), round(lon, 4)))  # Convert back to decimal degrees
+
+    return grid_points
```

### Comparing `zkyhaxpy-0.3.1.0.1/zkyhaxpy/http_tools.py` & `zkyhaxpy-0.3.1.1.0/zkyhaxpy/http_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.1.0.1/zkyhaxpy/img_tools.py` & `zkyhaxpy-0.3.1.1.0/zkyhaxpy/img_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.1.0.1/zkyhaxpy/io_tools.py` & `zkyhaxpy-0.3.1.1.0/zkyhaxpy/io_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.1.0.1/zkyhaxpy/json_tools.py` & `zkyhaxpy-0.3.1.1.0/zkyhaxpy/json_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.1.0.1/zkyhaxpy/log_tools.py` & `zkyhaxpy-0.3.1.1.0/zkyhaxpy/log_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.1.0.1/zkyhaxpy/ml_tools.py` & `zkyhaxpy-0.3.1.1.0/zkyhaxpy/ml_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.1.0.1/zkyhaxpy/multitask_tools.py` & `zkyhaxpy-0.3.1.1.0/zkyhaxpy/multitask_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.1.0.1/zkyhaxpy/np_tools.py` & `zkyhaxpy-0.3.1.1.0/zkyhaxpy/np_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.1.0.1/zkyhaxpy/pd_tools.py` & `zkyhaxpy-0.3.1.1.0/zkyhaxpy/pd_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.1.0.1/zkyhaxpy/skopt_tools.py` & `zkyhaxpy-0.3.1.1.0/zkyhaxpy/skopt_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.1.0.1/zkyhaxpy/snippet_tools.py` & `zkyhaxpy-0.3.1.1.0/zkyhaxpy/snippet_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.1.0.1/zkyhaxpy/timer_tools.py` & `zkyhaxpy-0.3.1.1.0/zkyhaxpy/timer_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.1.0.1/zkyhaxpy/util_tools.py` & `zkyhaxpy-0.3.1.1.0/zkyhaxpy/util_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.1.0.1/zkyhaxpy.egg-info/PKG-INFO` & `zkyhaxpy-0.3.1.1.0/zkyhaxpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zkyhaxpy
-Version: 0.3.1.0.1
+Version: 0.3.1.1.0
 Summary: A swiss-knife Data Science package for python
 Home-page: https://github.com/surasakcho/zkyhaxpy
 Author: Surasak Choedpasuporn
 Author-email: surasak.cho@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `zkyhaxpy-0.3.1.0.1/zkyhaxpy.egg-info/SOURCES.txt` & `zkyhaxpy-0.3.1.1.0/zkyhaxpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

