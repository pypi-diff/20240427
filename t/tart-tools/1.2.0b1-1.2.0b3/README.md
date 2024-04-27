# Comparing `tmp/tart_tools-1.2.0b1.tar.gz` & `tmp/tart_tools-1.2.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tart_tools-1.2.0b1.tar", last modified: Sat Dec  2 11:59:27 2023, max compression
+gzip compressed data, was "tart_tools-1.2.0b3.tar", last modified: Sat Apr 27 19:54:34 2024, max compression
```

## Comparing `tart_tools-1.2.0b1.tar` & `tart_tools-1.2.0b3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 11:59:27.414440 tart_tools-1.2.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2023-12-02 11:59:17.000000 tart_tools-1.2.0b1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-02 11:59:17.000000 tart_tools-1.2.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2023-12-02 11:59:27.414440 tart_tools-1.2.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2023-12-02 11:59:17.000000 tart_tools-1.2.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 11:59:27.410440 tart_tools-1.2.0b1/bin/
--rw-r--r--   0 runner    (1001) docker     (127)    13381 2023-12-02 11:59:17.000000 tart_tools-1.2.0b1/bin/tart_calibrate
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2023-12-02 11:59:17.000000 tart_tools-1.2.0b1/bin/tart_calibration_data
--rw-r--r--   0 runner    (1001) docker     (127)      998 2023-12-02 11:59:17.000000 tart_tools-1.2.0b1/bin/tart_download_antenna_positions
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2023-12-02 11:59:17.000000 tart_tools-1.2.0b1/bin/tart_download_data
--rw-r--r--   0 runner    (1001) docker     (127)      934 2023-12-02 11:59:17.000000 tart_tools-1.2.0b1/bin/tart_download_gains
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2023-12-02 11:59:17.000000 tart_tools-1.2.0b1/bin/tart_get_archive_data
--rw-r--r--   0 runner    (1001) docker     (127)    14359 2023-12-02 11:59:17.000000 tart_tools-1.2.0b1/bin/tart_image
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2023-12-02 11:59:17.000000 tart_tools-1.2.0b1/bin/tart_set_mode
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2023-12-02 11:59:17.000000 tart_tools-1.2.0b1/bin/tart_upload_antenna_positions
--rw-r--r--   0 runner    (1001) docker     (127)      978 2023-12-02 11:59:17.000000 tart_tools-1.2.0b1/bin/tart_upload_gains
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2023-12-02 11:59:17.000000 tart_tools-1.2.0b1/bin/tart_vis2json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-02 11:59:27.414440 tart_tools-1.2.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2023-12-02 11:59:17.000000 tart_tools-1.2.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 11:59:27.414440 tart_tools-1.2.0b1/tart_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-12-02 11:59:17.000000 tart_tools-1.2.0b1/tart_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2023-12-02 11:59:17.000000 tart_tools-1.2.0b1/tart_tools/api_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12887 2023-12-02 11:59:17.000000 tart_tools-1.2.0b1/tart_tools/api_imaging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 11:59:27.414440 tart_tools-1.2.0b1/tart_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2023-12-02 11:59:27.000000 tart_tools-1.2.0b1/tart_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      547 2023-12-02 11:59:27.000000 tart_tools-1.2.0b1/tart_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-02 11:59:27.000000 tart_tools-1.2.0b1/tart_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-02 11:59:27.000000 tart_tools-1.2.0b1/tart_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-02 11:59:27.000000 tart_tools-1.2.0b1/tart_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:54:34.586775 tart_tools-1.2.0b3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-27 19:54:30.000000 tart_tools-1.2.0b3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 19:54:30.000000 tart_tools-1.2.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-27 19:54:34.586775 tart_tools-1.2.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-27 19:54:30.000000 tart_tools-1.2.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:54:34.582775 tart_tools-1.2.0b3/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)    13381 2024-04-27 19:54:30.000000 tart_tools-1.2.0b3/bin/tart_calibrate
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-27 19:54:30.000000 tart_tools-1.2.0b3/bin/tart_calibration_data
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-27 19:54:30.000000 tart_tools-1.2.0b3/bin/tart_download_antenna_positions
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-27 19:54:30.000000 tart_tools-1.2.0b3/bin/tart_download_data
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-27 19:54:30.000000 tart_tools-1.2.0b3/bin/tart_download_gains
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-27 19:54:30.000000 tart_tools-1.2.0b3/bin/tart_get_archive_data
+-rw-r--r--   0 runner    (1001) docker     (127)    14359 2024-04-27 19:54:30.000000 tart_tools-1.2.0b3/bin/tart_image
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-27 19:54:30.000000 tart_tools-1.2.0b3/bin/tart_set_mode
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-27 19:54:30.000000 tart_tools-1.2.0b3/bin/tart_upload_antenna_positions
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-27 19:54:30.000000 tart_tools-1.2.0b3/bin/tart_upload_gains
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-27 19:54:30.000000 tart_tools-1.2.0b3/bin/tart_vis2json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 19:54:34.586775 tart_tools-1.2.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-27 19:54:30.000000 tart_tools-1.2.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:54:34.582775 tart_tools-1.2.0b3/tart_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-27 19:54:30.000000 tart_tools-1.2.0b3/tart_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-04-27 19:54:30.000000 tart_tools-1.2.0b3/tart_tools/api_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-04-27 19:54:30.000000 tart_tools-1.2.0b3/tart_tools/api_imaging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:54:34.586775 tart_tools-1.2.0b3/tart_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-27 19:54:34.000000 tart_tools-1.2.0b3/tart_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-27 19:54:34.000000 tart_tools-1.2.0b3/tart_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 19:54:34.000000 tart_tools-1.2.0b3/tart_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-27 19:54:34.000000 tart_tools-1.2.0b3/tart_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-27 19:54:34.000000 tart_tools-1.2.0b3/tart_tools.egg-info/top_level.txt
```

### Comparing `tart_tools-1.2.0b1/LICENSE.txt` & `tart_tools-1.2.0b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tart_tools-1.2.0b1/PKG-INFO` & `tart_tools-1.2.0b3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: tart_tools
-Version: 1.2.0b1
+Version: 1.2.0b3
 Summary: Transient Array Radio Telescope Command Line Tools
-Home-page: http://github.com/tmolteno/TART
+Home-page: http://github.com/tmolteno/tart_tools
 Author: Tim Molteno
 Author-email: tim@elec.ac.nz
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Communications :: Ham Radio
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -27,28 +27,29 @@
     
 This module provides command line tools for operating Transient Array Radio Telescope (TART). These tools are
 
 * tart_calibrate
 * tart_calibration_data
 * tart_download_antenna_positions
 * tart_upload_antenna_positions
+* tart_get_archive_data
 * tart_download_data
 * tart_download_gains
 * tart_image
 * tart_upload_gains
 * tart_set_mode
 * tart_vis2json
 
 
 To generate an image from a telescope, try the following command which should display the current view from a telescope
 on top of Signal-Hill near Dunedin New Zealand.
 
     tart_image --api https://tart.elec.ac.nz/signal --display
 
-For more information see the [TART Github repository](https://github.com/tmolteno/TART)
+For more information see the [TART website](https://tart.elec.ac.nz)
 
 ## Install Instructions
 
 tart_tools is available from standard python package repositories. Try:
 
     pip3 install tart_tools
 
@@ -65,14 +66,17 @@
 	make develop
 ```
 in which case changes to the source-code will be immediately available to projects using it.
 
     
 ## NEWS
 
+* 1.2.0b3 Update links to the github repository.
+* 1.2.0b2 tart_get_archive_data: Use a five digit leading-zeros number for multiple downloads, 
+          default to all data if --n is not specified
 * 1.2.0b1 new tool: tart_get_archive_data super convenient to query the AWS cloud archive of TART data.
 * 1.1.2b8 Add an argument --rotate to tart_upload_antenna_positions (for first stage of calibration)
 * 1.1.2b7 Handle expiration of JWT tokens better (in tart_tools)
 * 1.1.2b7 TART tools update. Add a command line switch to specify output file for tart_download_data'
 * 1.1.2b6 Pass the lat and lon to catalog_url
 * 1.1.2b5 Require the python-dateutil library
 * 1.1.2b4 Require the requests library
```

### Comparing `tart_tools-1.2.0b1/README.md` & `tart_tools-1.2.0b3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,28 +2,29 @@
     
 This module provides command line tools for operating Transient Array Radio Telescope (TART). These tools are
 
 * tart_calibrate
 * tart_calibration_data
 * tart_download_antenna_positions
 * tart_upload_antenna_positions
+* tart_get_archive_data
 * tart_download_data
 * tart_download_gains
 * tart_image
 * tart_upload_gains
 * tart_set_mode
 * tart_vis2json
 
 
 To generate an image from a telescope, try the following command which should display the current view from a telescope
 on top of Signal-Hill near Dunedin New Zealand.
 
     tart_image --api https://tart.elec.ac.nz/signal --display
 
-For more information see the [TART Github repository](https://github.com/tmolteno/TART)
+For more information see the [TART website](https://tart.elec.ac.nz)
 
 ## Install Instructions
 
 tart_tools is available from standard python package repositories. Try:
 
     pip3 install tart_tools
 
@@ -40,14 +41,17 @@
 	make develop
 ```
 in which case changes to the source-code will be immediately available to projects using it.
 
     
 ## NEWS
 
+* 1.2.0b3 Update links to the github repository.
+* 1.2.0b2 tart_get_archive_data: Use a five digit leading-zeros number for multiple downloads, 
+          default to all data if --n is not specified
 * 1.2.0b1 new tool: tart_get_archive_data super convenient to query the AWS cloud archive of TART data.
 * 1.1.2b8 Add an argument --rotate to tart_upload_antenna_positions (for first stage of calibration)
 * 1.1.2b7 Handle expiration of JWT tokens better (in tart_tools)
 * 1.1.2b7 TART tools update. Add a command line switch to specify output file for tart_download_data'
 * 1.1.2b6 Pass the lat and lon to catalog_url
 * 1.1.2b5 Require the python-dateutil library
 * 1.1.2b4 Require the requests library
```

### Comparing `tart_tools-1.2.0b1/bin/tart_calibrate` & `tart_tools-1.2.0b3/bin/tart_calibrate`

 * *Files identical despite different names*

### Comparing `tart_tools-1.2.0b1/bin/tart_calibration_data` & `tart_tools-1.2.0b3/bin/tart_calibration_data`

 * *Files identical despite different names*

### Comparing `tart_tools-1.2.0b1/bin/tart_download_antenna_positions` & `tart_tools-1.2.0b3/bin/tart_download_antenna_positions`

 * *Files identical despite different names*

### Comparing `tart_tools-1.2.0b1/bin/tart_download_data` & `tart_tools-1.2.0b3/bin/tart_download_data`

 * *Files identical despite different names*

### Comparing `tart_tools-1.2.0b1/bin/tart_download_gains` & `tart_tools-1.2.0b3/bin/tart_download_gains`

 * *Files identical despite different names*

### Comparing `tart_tools-1.2.0b1/bin/tart_get_archive_data` & `tart_tools-1.2.0b3/bin/tart_get_archive_data`

 * *Files 14% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     parser.add_argument('--target', required=False,
                         default='signal', help="Telescope name in s3 bucket.")
 
     parser.add_argument('--catalog', required=False,
                         default='https://tart.elec.ac.nz/catalog', help="Catalog API URL.")
 
     parser.add_argument('--n', required=False, type=int,
-                        default=1, help="Number of HDF vis files. (-1 means all)")
+                        default=-1, help="Number of HDF vis files. (-1 means all)")
     
     parser.add_argument('--start', required=False, default="-60", help="Start time (negative means offset from now).")
     parser.add_argument('--duration', required=False,  default="0", help="Number of minutes to sample for")
 
 
     ARGS = parser.parse_args()
 
@@ -46,15 +46,14 @@
 
 
     # for o in objects:
     #     print(vars(o))
     #     print(dir(o))
     #     break
 
-    N = ARGS.n
     
     start = ARGS.start
     duration_str = ARGS.duration
     duration = float(duration_str)
     duration_dt = datetime.timedelta(days = 0, hours=0, \
                         minutes=duration, seconds=0)
 
@@ -89,18 +88,24 @@
 
 
     desired_objects = []
     for o in objects:
         if (o.last_modified >= start_datetime) and (o.last_modified <= stop_datetime):
             desired_objects.append(o)
 
-    steps = max(len(desired_objects) // N, 1)
-
-    index = 1
-    for item in tqdm(list(desired_objects)[::steps]):
+    N = ARGS.n
+    if N > 0:
+        steps = max(len(desired_objects) // N, 1)
+        data_to_get = list(desired_objects)[::steps]
+    else:
+        data_to_get = list(desired_objects)
+        
+    n = len(data_to_get)
+    index = 0
+    for item in tqdm(data_to_get):
 
         dirname, fname = os.path.split(item.object_name)
-        fname = f"obs_{index}.hdf"
+        fname = f"obs_{index:05d}.hdf"
         fname_out = os.path.join(output, fname)
         index = index+1
         client.fget_object(BUCKET_NAME, item.object_name, fname_out)
         # print(fname_out)
```

### Comparing `tart_tools-1.2.0b1/bin/tart_image` & `tart_tools-1.2.0b3/bin/tart_image`

 * *Files identical despite different names*

### Comparing `tart_tools-1.2.0b1/bin/tart_set_mode` & `tart_tools-1.2.0b3/bin/tart_set_mode`

 * *Files identical despite different names*

### Comparing `tart_tools-1.2.0b1/bin/tart_upload_antenna_positions` & `tart_tools-1.2.0b3/bin/tart_upload_antenna_positions`

 * *Files identical despite different names*

### Comparing `tart_tools-1.2.0b1/bin/tart_upload_gains` & `tart_tools-1.2.0b3/bin/tart_upload_gains`

 * *Files identical despite different names*

### Comparing `tart_tools-1.2.0b1/bin/tart_vis2json` & `tart_tools-1.2.0b3/bin/tart_vis2json`

 * *Files identical despite different names*

### Comparing `tart_tools-1.2.0b1/setup.py` & `tart_tools-1.2.0b3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(name='tart_tools',
-    version='1.2.0b1',
+    version='1.2.0b3',
     description='Transient Array Radio Telescope Command Line Tools',
     long_description=readme,
     long_description_content_type="text/markdown",
-    url='http://github.com/tmolteno/TART',
+    url='http://github.com/tmolteno/tart_tools',
     author='Tim Molteno',
     author_email='tim@elec.ac.nz',
     license='GPLv3',
     install_requires=['numpy', 'matplotlib', 'healpy', 'astropy', 'tart', 'requests', 'tqdm', 'minio'],
     packages=['tart_tools'],
     scripts=['bin/tart_image',
              'bin/tart_calibrate',
```

### Comparing `tart_tools-1.2.0b1/tart_tools/api_handler.py` & `tart_tools-1.2.0b3/tart_tools/api_handler.py`

 * *Files identical despite different names*

### Comparing `tart_tools-1.2.0b1/tart_tools/api_imaging.py` & `tart_tools-1.2.0b3/tart_tools/api_imaging.py`

 * *Files identical despite different names*

### Comparing `tart_tools-1.2.0b1/tart_tools.egg-info/PKG-INFO` & `tart_tools-1.2.0b3/tart_tools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: tart-tools
-Version: 1.2.0b1
+Name: tart_tools
+Version: 1.2.0b3
 Summary: Transient Array Radio Telescope Command Line Tools
-Home-page: http://github.com/tmolteno/TART
+Home-page: http://github.com/tmolteno/tart_tools
 Author: Tim Molteno
 Author-email: tim@elec.ac.nz
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Communications :: Ham Radio
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -27,28 +27,29 @@
     
 This module provides command line tools for operating Transient Array Radio Telescope (TART). These tools are
 
 * tart_calibrate
 * tart_calibration_data
 * tart_download_antenna_positions
 * tart_upload_antenna_positions
+* tart_get_archive_data
 * tart_download_data
 * tart_download_gains
 * tart_image
 * tart_upload_gains
 * tart_set_mode
 * tart_vis2json
 
 
 To generate an image from a telescope, try the following command which should display the current view from a telescope
 on top of Signal-Hill near Dunedin New Zealand.
 
     tart_image --api https://tart.elec.ac.nz/signal --display
 
-For more information see the [TART Github repository](https://github.com/tmolteno/TART)
+For more information see the [TART website](https://tart.elec.ac.nz)
 
 ## Install Instructions
 
 tart_tools is available from standard python package repositories. Try:
 
     pip3 install tart_tools
 
@@ -65,14 +66,17 @@
 	make develop
 ```
 in which case changes to the source-code will be immediately available to projects using it.
 
     
 ## NEWS
 
+* 1.2.0b3 Update links to the github repository.
+* 1.2.0b2 tart_get_archive_data: Use a five digit leading-zeros number for multiple downloads, 
+          default to all data if --n is not specified
 * 1.2.0b1 new tool: tart_get_archive_data super convenient to query the AWS cloud archive of TART data.
 * 1.1.2b8 Add an argument --rotate to tart_upload_antenna_positions (for first stage of calibration)
 * 1.1.2b7 Handle expiration of JWT tokens better (in tart_tools)
 * 1.1.2b7 TART tools update. Add a command line switch to specify output file for tart_download_data'
 * 1.1.2b6 Pass the lat and lon to catalog_url
 * 1.1.2b5 Require the python-dateutil library
 * 1.1.2b4 Require the requests library
```

### Comparing `tart_tools-1.2.0b1/tart_tools.egg-info/SOURCES.txt` & `tart_tools-1.2.0b3/tart_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

