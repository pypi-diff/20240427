# Comparing `tmp/hydro_raster-0.0.8.tar.gz` & `tmp/hydro_raster-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hydro_raster-0.0.8.tar", last modified: Wed Oct 11 22:17:46 2023, max compression
+gzip compressed data, was "dist/hydro_raster-0.0.9.tar", last modified: Wed Oct 25 09:43:56 2023, max compression
```

## Comparing `hydro_raster-0.0.8.tar` & `hydro_raster-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 ming       (502) staff       (20)        0 2023-10-11 22:17:46.000000 hydro_raster-0.0.8/
--rw-r--r--   0 ming       (502) staff       (20)      168 2022-04-01 15:19:17.000000 hydro_raster-0.0.8/MANIFEST.in
--rw-r--r--   0 ming       (502) staff       (20)     3757 2023-10-11 22:17:46.000000 hydro_raster-0.0.8/PKG-INFO
--rw-r--r--   0 ming       (502) staff       (20)     2545 2023-10-11 18:05:54.000000 hydro_raster-0.0.8/README.md
-drwxr-xr-x   0 ming       (502) staff       (20)        0 2023-10-11 22:17:46.000000 hydro_raster-0.0.8/hydro_raster/
--rw-r--r--   0 ming       (502) staff       (20)    34553 2023-10-11 22:16:51.000000 hydro_raster-0.0.8/hydro_raster/Raster.py
--rwxr-xr-x   0 ming       (502) staff       (20)      855 2023-09-26 21:02:30.000000 hydro_raster-0.0.8/hydro_raster/__init__.py
--rw-r--r--   0 ming       (502) staff       (20)    15398 2023-10-11 22:02:23.000000 hydro_raster-0.0.8/hydro_raster/grid_show.py
-drwxr-xr-x   0 ming       (502) staff       (20)        0 2023-10-11 22:17:46.000000 hydro_raster-0.0.8/hydro_raster/sample/
--rw-r--r--   0 ming       (502) staff       (20)  6300262 2021-05-26 13:44:17.000000 hydro_raster-0.0.8/hydro_raster/sample/CA1_5m.tif
--rw-r--r--   0 ming       (502) staff       (20)        5 2022-03-08 17:05:24.000000 hydro_raster-0.0.8/hydro_raster/sample/CA1_overhead_features.cpg
--rw-r--r--   0 ming       (502) staff       (20)      226 2022-03-08 17:47:50.000000 hydro_raster-0.0.8/hydro_raster/sample/CA1_overhead_features.dbf
--rw-r--r--   0 ming       (502) staff       (20)      417 2022-03-08 17:05:24.000000 hydro_raster-0.0.8/hydro_raster/sample/CA1_overhead_features.prj
--rw-r--r--   0 ming       (502) staff       (20)      659 2022-03-08 17:05:24.000000 hydro_raster-0.0.8/hydro_raster/sample/CA1_overhead_features.qmd
--rw-r--r--   0 ming       (502) staff       (20)      644 2022-03-08 17:47:50.000000 hydro_raster-0.0.8/hydro_raster/sample/CA1_overhead_features.shp
--rw-r--r--   0 ming       (502) staff       (20)      132 2022-03-08 17:47:50.000000 hydro_raster-0.0.8/hydro_raster/sample/CA1_overhead_features.shx
--rw-r--r--   0 ming       (502) staff       (20)    17052 2023-10-11 18:05:54.000000 hydro_raster-0.0.8/hydro_raster/spatial_analysis.py
-drwxr-xr-x   0 ming       (502) staff       (20)        0 2023-10-11 22:17:46.000000 hydro_raster-0.0.8/hydro_raster.egg-info/
--rw-r--r--   0 ming       (502) staff       (20)     3757 2023-10-11 22:17:46.000000 hydro_raster-0.0.8/hydro_raster.egg-info/PKG-INFO
--rw-r--r--   0 ming       (502) staff       (20)      623 2023-10-11 22:17:46.000000 hydro_raster-0.0.8/hydro_raster.egg-info/SOURCES.txt
--rw-r--r--   0 ming       (502) staff       (20)        1 2023-10-11 22:17:46.000000 hydro_raster-0.0.8/hydro_raster.egg-info/dependency_links.txt
--rw-r--r--   0 ming       (502) staff       (20)       71 2023-10-11 22:17:46.000000 hydro_raster-0.0.8/hydro_raster.egg-info/requires.txt
--rw-r--r--   0 ming       (502) staff       (20)       13 2023-10-11 22:17:46.000000 hydro_raster-0.0.8/hydro_raster.egg-info/top_level.txt
--rw-r--r--   0 ming       (502) staff       (20)       38 2023-10-11 22:17:46.000000 hydro_raster-0.0.8/setup.cfg
--rwxr-xr-x   0 ming       (502) staff       (20)     2100 2023-10-11 18:22:13.000000 hydro_raster-0.0.8/setup.py
+drwxr-xr-x   0 ming       (502) staff       (20)        0 2023-10-25 09:43:56.000000 hydro_raster-0.0.9/
+-rw-r--r--   0 ming       (502) staff       (20)      168 2022-04-01 15:19:17.000000 hydro_raster-0.0.9/MANIFEST.in
+-rw-r--r--   0 ming       (502) staff       (20)     3794 2023-10-25 09:43:56.000000 hydro_raster-0.0.9/PKG-INFO
+-rw-r--r--   0 ming       (502) staff       (20)     2574 2023-10-11 22:19:50.000000 hydro_raster-0.0.9/README.md
+drwxr-xr-x   0 ming       (502) staff       (20)        0 2023-10-25 09:43:56.000000 hydro_raster-0.0.9/hydro_raster/
+-rw-r--r--   0 ming       (502) staff       (20)    34746 2023-10-25 09:32:14.000000 hydro_raster-0.0.9/hydro_raster/Raster.py
+-rwxr-xr-x   0 ming       (502) staff       (20)      855 2023-09-26 21:02:30.000000 hydro_raster-0.0.9/hydro_raster/__init__.py
+-rw-r--r--   0 ming       (502) staff       (20)    15398 2023-10-11 22:02:23.000000 hydro_raster-0.0.9/hydro_raster/grid_show.py
+drwxr-xr-x   0 ming       (502) staff       (20)        0 2023-10-25 09:43:56.000000 hydro_raster-0.0.9/hydro_raster/sample/
+-rw-r--r--   0 ming       (502) staff       (20)  6300262 2021-05-26 13:44:17.000000 hydro_raster-0.0.9/hydro_raster/sample/CA1_5m.tif
+-rw-r--r--   0 ming       (502) staff       (20)        5 2022-03-08 17:05:24.000000 hydro_raster-0.0.9/hydro_raster/sample/CA1_overhead_features.cpg
+-rw-r--r--   0 ming       (502) staff       (20)      226 2022-03-08 17:47:50.000000 hydro_raster-0.0.9/hydro_raster/sample/CA1_overhead_features.dbf
+-rw-r--r--   0 ming       (502) staff       (20)      417 2022-03-08 17:05:24.000000 hydro_raster-0.0.9/hydro_raster/sample/CA1_overhead_features.prj
+-rw-r--r--   0 ming       (502) staff       (20)      659 2022-03-08 17:05:24.000000 hydro_raster-0.0.9/hydro_raster/sample/CA1_overhead_features.qmd
+-rw-r--r--   0 ming       (502) staff       (20)      644 2022-03-08 17:47:50.000000 hydro_raster-0.0.9/hydro_raster/sample/CA1_overhead_features.shp
+-rw-r--r--   0 ming       (502) staff       (20)      132 2022-03-08 17:47:50.000000 hydro_raster-0.0.9/hydro_raster/sample/CA1_overhead_features.shx
+-rw-r--r--   0 ming       (502) staff       (20)    18006 2023-10-25 09:33:52.000000 hydro_raster-0.0.9/hydro_raster/spatial_analysis.py
+drwxr-xr-x   0 ming       (502) staff       (20)        0 2023-10-25 09:43:56.000000 hydro_raster-0.0.9/hydro_raster.egg-info/
+-rw-r--r--   0 ming       (502) staff       (20)     3794 2023-10-25 09:43:55.000000 hydro_raster-0.0.9/hydro_raster.egg-info/PKG-INFO
+-rw-r--r--   0 ming       (502) staff       (20)      623 2023-10-25 09:43:55.000000 hydro_raster-0.0.9/hydro_raster.egg-info/SOURCES.txt
+-rw-r--r--   0 ming       (502) staff       (20)        1 2023-10-25 09:43:55.000000 hydro_raster-0.0.9/hydro_raster.egg-info/dependency_links.txt
+-rw-r--r--   0 ming       (502) staff       (20)       71 2023-10-25 09:43:55.000000 hydro_raster-0.0.9/hydro_raster.egg-info/requires.txt
+-rw-r--r--   0 ming       (502) staff       (20)       13 2023-10-25 09:43:55.000000 hydro_raster-0.0.9/hydro_raster.egg-info/top_level.txt
+-rw-r--r--   0 ming       (502) staff       (20)       38 2023-10-25 09:43:56.000000 hydro_raster-0.0.9/setup.cfg
+-rwxr-xr-x   0 ming       (502) staff       (20)     2100 2023-10-25 09:43:38.000000 hydro_raster-0.0.9/setup.py
```

### Comparing `hydro_raster-0.0.8/PKG-INFO` & `hydro_raster-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydro_raster
-Version: 0.0.8
+Version: 0.0.9
 Summary: To process raster data for hydrological/hydrodynamic modelling
 Home-page: https://github.com/mingxiaodong/hydro-raster
 Author: Xiaodong Ming
 Author-email: x.ming@lboro.ac.uk
 License: LICENSE.txt
 Description: hydro_raster
         --------
@@ -57,14 +57,15 @@
         ras_obj_cut = ras_obj.rect_clip(clip_extent) # raster can aslo be cut by a shapfile using 'clip' function
         ras_obj_cut.mapshow()
         ```
         3. Rasterize polygons on a raster and return an index array with the same dimension of the raster array
         ```
         shp_file_name = get_sample_data('shp')
         index_array = ras_obj_cut.rasterize(shp_file_name)
+        index_array = index_array>=0
         ```
         4. Change raster cell values within the polygons by adding a fixed value
         ```
         ras_obj_new = ras_obj_cut.duplicate()
         ras_obj_new.array[index_array] = ras_obj_cut.array[index_array]+20
         ```
         5. Show the edited raster with the shapefile polygons
```

### Comparing `hydro_raster-0.0.8/README.md` & `hydro_raster-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 ras_obj_cut = ras_obj.rect_clip(clip_extent) # raster can aslo be cut by a shapfile using 'clip' function
 ras_obj_cut.mapshow()
 ```
 3. Rasterize polygons on a raster and return an index array with the same dimension of the raster array
 ```
 shp_file_name = get_sample_data('shp')
 index_array = ras_obj_cut.rasterize(shp_file_name)
+index_array = index_array>=0
 ```
 4. Change raster cell values within the polygons by adding a fixed value
 ```
 ras_obj_new = ras_obj_cut.duplicate()
 ras_obj_new.array[index_array] = ras_obj_cut.array[index_array]+20
 ```
 5. Show the edited raster with the shapefile polygons
```

### Comparing `hydro_raster-0.0.8/hydro_raster/Raster.py` & `hydro_raster-0.0.9/hydro_raster/Raster.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,39 +47,41 @@
         extent_dict: a dictionary storing outline limits of the raster  
         wkt: (string) the Well-Known_Text (wkt) projection information  
         
     """
 #%%======================== initialization function ===========================   
     def __init__(self, source_file=None, array=None, header=None, 
                  xllcorner=0, yllcorner=0, cellsize=100, NODATA_value=-9999,
-                 crs=None, num_header_rows=6):
+                 crs=None, num_header_rows=6, read_extent=None):
         """Initialise the object
 
         Args:
             source_file: name of a asc/tif file if a file read is needed
             array: values in each raster cell [a numpy array]
             header: georeference of the raster [a dictionary containing 6 keys]
                 nrows, nclos [int]
                 cellsize, xllcorner, yllcorner
                 NODATA_value
             crs: coordinate reference system, either epsg(epsg code, int) or
                 wkt(string), or a rasterio.crs object
+            read_extent (dict, optional): extent window (left, right, bottom, top 
+                in map coordinates) to read part of the tif. Defaults to None.
         Example: define a raster object with a random array
             array = np.random.rand(10, 10)
             header = {'ncols':array.shape[1], 'nrows':array.shape[0],
                       'xllcorner':0, 'yllcorner':1,
                       'cellsize':100, 'NODATA_value':-9999}
             obj_ras = Raster(array=array, header=header)
             obj_ras.mapshow() %plot map
 
         """
         # get data from file or arguments
         if type(source_file) is str: # tif, txt, asc, or gz file
             if source_file.endswith('.tif'): # only read the first band
-                array, header, crs, ras_meta = sp.tif_read(source_file)
+                array, header, crs, ras_meta = sp.tif_read(source_file, read_extent)
                 self.meta = ras_meta
             else:
                 array, header, crs = sp.arcgridread(source_file,
                                                     num_header_rows)                
             self.source_file = source_file
         elif type(source_file) is bytes:  # try a binary file-like object
             array, header = sp.byte_file_read(source_file)
```

### Comparing `hydro_raster-0.0.8/hydro_raster/__init__.py` & `hydro_raster-0.0.9/hydro_raster/__init__.py`

 * *Files identical despite different names*

### Comparing `hydro_raster-0.0.8/hydro_raster/grid_show.py` & `hydro_raster-0.0.9/hydro_raster/grid_show.py`

 * *Files identical despite different names*

### Comparing `hydro_raster-0.0.8/hydro_raster/sample/CA1_5m.tif` & `hydro_raster-0.0.9/hydro_raster/sample/CA1_5m.tif`

 * *Files identical despite different names*

### Comparing `hydro_raster-0.0.8/hydro_raster/sample/CA1_overhead_features.qmd` & `hydro_raster-0.0.9/hydro_raster/sample/CA1_overhead_features.qmd`

 * *Files identical despite different names*

### Comparing `hydro_raster-0.0.8/hydro_raster/sample/CA1_overhead_features.shp` & `hydro_raster-0.0.9/hydro_raster/sample/CA1_overhead_features.shp`

 * *Files identical despite different names*

### Comparing `hydro_raster-0.0.8/hydro_raster/spatial_analysis.py` & `hydro_raster-0.0.9/hydro_raster/spatial_analysis.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import os
 import gzip
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.colors as colors
 import rasterio as rio
 import shapefile
+from rasterio.windows import Window
 from matplotlib import cm
 from matplotlib.colors import ListedColormap
 from matplotlib.patches import Patch
 from matplotlib.colors import LightSource
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 #%%
 def arc_header_read(file_name, header_rows=6):
@@ -166,33 +167,48 @@
     file_h.write(b"cellsize    %g\n" % header['cellsize'])
     file_h.write(b"NODATA_value    %g\n" % header['NODATA_value'])
     array[np.isnan(array)] = header['NODATA_value']
     np.savetxt(file_h, array, fmt='%g', delimiter=' ')
     file_h.close()
     print(file_name + ' created')
 
-def tif_read(file_name):
-    """read tif file (only the 1st band) and return array, header, crs
+def tif_read(file_name, read_extent=None):
+    """read tif file (only the 1st band) and return array, header, crs and meta
+
+    Args:
+        file_name (str): tif file name
+        read_extent (dict, optional): extent window (left, right, bottom, top 
+            in map coordinates) to read part of the raster. Defaults to None.
+
+    Returns:
+        _type_: _description_
     """
     with rio.open(file_name) as src:
-        masked_array = src.read(1, masked=True)
         ras_meta = src.meta
+    if read_extent is None:
+        with rio.open(file_name) as src:
+            masked_array = src.read(1, masked=True)
+    else:
+        X = np.array(read_extent[:2])
+        Y = np.array(read_extent[2:])
+        geo_transform = ras_meta['transform']
+        rows, cols = map2sub(X, Y, geo_transform)
+        slice_r = slice(rows.min(), rows.max())
+        slice_c = slice(cols.min(), cols.max())
+        window = Window.from_slices(slice_r, slice_c)
+        with rio.open(file_name) as src:
+            masked_array = src.read(1, masked=True, 
+                                    window=window)
+            win_transform = src.window_transform(window)
+        ras_meta['height'] = masked_array.data.shape[0]
+        ras_meta['width'] = masked_array.data.shape[1]
+        ras_meta['transform'] = win_transform 
     array = masked_array.data+0.0
     array[array == masked_array.fill_value] = np.nan
-    ncols = ras_meta['width']
-    nrows = ras_meta['height']
-    geo_transform = ras_meta['transform']
-    cellsize = geo_transform[0]
-    x_min = geo_transform[2]
-    y_max = geo_transform[5]
-    xllcorner = x_min
-    yllcorner = y_max-nrows*cellsize
-    header = {'ncols':ncols, 'nrows':nrows,
-              'xllcorner':xllcorner, 'yllcorner':yllcorner,
-              'cellsize':cellsize, 'NODATA_value':ras_meta['nodata']}     
+    header = meta2header(ras_meta)   
     crs = ras_meta['crs']
     return array, header, crs, ras_meta
 
 def byte_file_read(file_name):
     """ Read file from a bytes object
     """
     # read header
@@ -333,36 +349,45 @@
         raise ValueError('extent produces different cellsize in x and y')
     cellsize = cellsize_x
     header = {'ncols':ncols, 'nrows':nrows,
               'xllcorner':xllcorner, 'yllcorner':yllcorner,
               'cellsize':cellsize, 'NODATA_value':nan_value}
     return header
 
-def map2sub(X, Y, header):
-    """ convert map coordinates to subscripts of an array
-
-        array is defined by a geo-reference header
+def map2sub(X, Y, geo_ref):
+    """convert map coordinates to subscripts of the raster 
+    array according to geo_ref which is either a header or
+    a geo_transform object from raster
 
-    Args: 
-        X: a scalar or numpy array of coordinate values
-        Y: a scalar or numpy array of coordinate values
+    Args:
+        X (scalar or numpy.ndarray): Input X coordinate
+        Y (scalar or numpy.ndarray): Input Y coordinate
+        geo_ref (_type_): _description_
 
-    Return: 
-        numpy array: rows and cols in the array
+    Returns:
+        tuple (int, int): rows and cols in the array
     """
-    # X and Y coordinate of the centre of the first cell in the array
     X = np.array(X)
     Y = np.array(Y)
-    x0 = header['xllcorner']+0.5*header['cellsize']
-    y0 = header['yllcorner']+(header['nrows']-0.5)*header['cellsize']
-    rows = (y0-Y)/header['cellsize'] # row and col number starts from 0
-    cols = (X-x0)/header['cellsize']
+    if type(geo_ref) is dict: #header
+        cellsize = geo_ref['cellsize']
+        x0 = geo_ref['xllcorner']+0.5*cellsize
+        y0 = geo_ref['yllcorner']+(geo_ref['nrows']-0.5)*cellsize
+        rows = (y0-Y)/cellsize # row and col number starts from 0
+        cols = (X-x0)/cellsize
+    else: # geo_transform
+        cellsize = geo_ref[0]
+        x_ulcorner = geo_ref[2]
+        y_ulcorner = geo_ref[5]
+        cols = (X-x_ulcorner)/cellsize-0.5
+        rows = (y_ulcorner-Y)/cellsize-0.5
+
     if isinstance(rows, np.ndarray):
         rows = np.round(rows).astype('int64')
-        cols = np.round(cols).astype('int64') #.astype('int64')
+        cols = np.round(cols).astype('int64')
     else:
         rows = int(rows)
         cols = int(cols)
     return rows, cols
 
 def sub2map(rows, cols, header):
     """convert subscripts of a matrix to map coordinates rows,
```

### Comparing `hydro_raster-0.0.8/hydro_raster.egg-info/PKG-INFO` & `hydro_raster-0.0.9/hydro_raster.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydro-raster
-Version: 0.0.8
+Version: 0.0.9
 Summary: To process raster data for hydrological/hydrodynamic modelling
 Home-page: https://github.com/mingxiaodong/hydro-raster
 Author: Xiaodong Ming
 Author-email: x.ming@lboro.ac.uk
 License: LICENSE.txt
 Description: hydro_raster
         --------
@@ -57,14 +57,15 @@
         ras_obj_cut = ras_obj.rect_clip(clip_extent) # raster can aslo be cut by a shapfile using 'clip' function
         ras_obj_cut.mapshow()
         ```
         3. Rasterize polygons on a raster and return an index array with the same dimension of the raster array
         ```
         shp_file_name = get_sample_data('shp')
         index_array = ras_obj_cut.rasterize(shp_file_name)
+        index_array = index_array>=0
         ```
         4. Change raster cell values within the polygons by adding a fixed value
         ```
         ras_obj_new = ras_obj_cut.duplicate()
         ras_obj_new.array[index_array] = ras_obj_cut.array[index_array]+20
         ```
         5. Show the edited raster with the shapefile polygons
```

### Comparing `hydro_raster-0.0.8/hydro_raster.egg-info/SOURCES.txt` & `hydro_raster-0.0.9/hydro_raster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hydro_raster-0.0.8/setup.py` & `hydro_raster-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from os import path
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
       name='hydro_raster',
-      version='0.0.8',
+      version='0.0.9',
       description='To process raster data for hydrological/hydrodynamic modelling',
       url='https://github.com/mingxiaodong/hydro-raster',
       author='Xiaodong Ming',
       author_email='x.ming@lboro.ac.uk',
       long_description=long_description,
       long_description_content_type='text/markdown',
       classifiers=['Development Status :: 3 - Alpha',
```

