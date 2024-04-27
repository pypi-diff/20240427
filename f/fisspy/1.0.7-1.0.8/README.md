# Comparing `tmp/fisspy-1.0.7.tar.gz` & `tmp/fisspy-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fisspy-1.0.7.tar", last modified: Thu Apr 25 12:05:08 2024, max compression
+gzip compressed data, was "fisspy-1.0.8.tar", last modified: Fri Apr 26 10:47:37 2024, max compression
```

## Comparing `fisspy-1.0.7.tar` & `fisspy-1.0.8.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.288168 fisspy-1.0.7/
--rw-r--r--   0 jhkang     (501) staff       (20)     1305 2023-07-14 01:35:52.000000 fisspy-1.0.7/LICENSE.txt
--rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-04-25 12:05:08.287978 fisspy-1.0.7/PKG-INFO
--rw-r--r--   0 jhkang     (501) staff       (20)     1988 2024-04-23 12:48:39.000000 fisspy-1.0.7/README.md
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.276972 fisspy-1.0.7/fisspy/
--rw-r--r--   0 jhkang     (501) staff       (20)      430 2024-04-25 12:04:23.000000 fisspy-1.0.7/fisspy/__init__.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.278411 fisspy-1.0.7/fisspy/align/
--rw-r--r--   0 jhkang     (501) staff       (20)       44 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/align/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15179 2024-04-24 08:05:01.000000 fisspy-1.0.7/fisspy/align/alignment.py
--rw-r--r--   0 jhkang     (501) staff       (20)    11470 2024-04-25 11:40:56.000000 fisspy-1.0.7/fisspy/align/base.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.280809 fisspy-1.0.7/fisspy/analysis/
--rw-r--r--   0 jhkang     (501) staff       (20)      317 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/analysis/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    12577 2024-04-25 11:37:49.000000 fisspy-1.0.7/fisspy/analysis/doppler.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1030 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/analysis/filter.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2988 2024-04-25 11:30:36.000000 fisspy-1.0.7/fisspy/analysis/forecast.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15224 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/analysis/ofe.py
--rw-r--r--   0 jhkang     (501) staff       (20)    35498 2024-04-25 11:29:47.000000 fisspy-1.0.7/fisspy/analysis/tdmap.py
--rw-r--r--   0 jhkang     (501) staff       (20)    33907 2024-04-25 11:35:30.000000 fisspy-1.0.7/fisspy/analysis/wavelet.py
--rw-r--r--   0 jhkang     (501) staff       (20)    19011 2023-07-14 01:35:52.000000 fisspy-1.0.7/fisspy/cm.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.281818 fisspy-1.0.7/fisspy/correction/
--rw-r--r--   0 jhkang     (501) staff       (20)       51 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/correction/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    11372 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/correction/correction.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2337 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/correction/get_inform.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.282734 fisspy-1.0.7/fisspy/data/
--rw-r--r--   0 jhkang     (501) staff       (20)       64 2023-07-25 08:49:17.000000 fisspy-1.0.7/fisspy/data/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1072 2023-07-25 08:49:17.000000 fisspy-1.0.7/fisspy/data/_sample.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2965 2023-07-25 08:49:17.000000 fisspy-1.0.7/fisspy/data/download.py
--rw-r--r--   0 jhkang     (501) staff       (20)      394 2023-07-14 01:35:52.000000 fisspy-1.0.7/fisspy/data/sample.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.283446 fisspy-1.0.7/fisspy/image/
--rw-r--r--   0 jhkang     (501) staff       (20)       73 2024-04-25 10:45:58.000000 fisspy-1.0.7/fisspy/image/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    29769 2024-04-25 11:21:02.000000 fisspy-1.0.7/fisspy/image/interactive_image.py
--rw-r--r--   0 jhkang     (501) staff       (20)    11315 2024-04-25 12:04:09.000000 fisspy-1.0.7/fisspy/image/raster_set.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.283755 fisspy-1.0.7/fisspy/inversion/
--rw-r--r--   0 jhkang     (501) staff       (20)        0 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/inversion/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)      181 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/inversion/_mlsi.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.284182 fisspy-1.0.7/fisspy/io/
--rw-r--r--   0 jhkang     (501) staff       (20)      320 2023-07-14 01:35:52.000000 fisspy-1.0.7/fisspy/io/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15840 2023-07-14 01:35:52.000000 fisspy-1.0.7/fisspy/io/read.py
--rw-r--r--   0 jhkang     (501) staff       (20)     4974 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/makevideo.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.285837 fisspy-1.0.7/fisspy/preprocess/
--rw-r--r--   0 jhkang     (501) staff       (20)       29 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/preprocess/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    52443 2024-04-25 11:18:41.000000 fisspy-1.0.7/fisspy/preprocess/proc_base.py
--rw-r--r--   0 jhkang     (501) staff       (20)   143266 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/preprocess/proc_gui.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1685 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/preprocess/t_y_sh.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.287580 fisspy-1.0.7/fisspy/read/
--rw-r--r--   0 jhkang     (501) staff       (20)      195 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/read/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    49069 2024-04-25 11:24:21.000000 fisspy-1.0.7/fisspy/read/read_factory.py
--rw-r--r--   0 jhkang     (501) staff       (20)     6847 2024-04-25 06:03:54.000000 fisspy-1.0.7/fisspy/read/readbase.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.277787 fisspy-1.0.7/fisspy.egg-info/
--rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-04-25 12:05:08.000000 fisspy-1.0.7/fisspy.egg-info/PKG-INFO
--rw-r--r--   0 jhkang     (501) staff       (20)     1079 2024-04-25 12:05:08.000000 fisspy-1.0.7/fisspy.egg-info/SOURCES.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-25 12:05:08.000000 fisspy-1.0.7/fisspy.egg-info/dependency_links.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-25 12:05:08.000000 fisspy-1.0.7/fisspy.egg-info/not-zip-safe
--rw-r--r--   0 jhkang     (501) staff       (20)      137 2024-04-25 12:05:08.000000 fisspy-1.0.7/fisspy.egg-info/requires.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        7 2024-04-25 12:05:08.000000 fisspy-1.0.7/fisspy.egg-info/top_level.txt
--rw-r--r--   0 jhkang     (501) staff       (20)       38 2024-04-25 12:05:08.288209 fisspy-1.0.7/setup.cfg
--rw-r--r--   0 jhkang     (501) staff       (20)      582 2024-04-25 12:04:40.000000 fisspy-1.0.7/setup.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-26 10:47:37.064443 fisspy-1.0.8/
+-rw-r--r--   0 jhkang     (501) staff       (20)     1305 2023-07-14 01:35:52.000000 fisspy-1.0.8/LICENSE.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-04-26 10:47:37.064245 fisspy-1.0.8/PKG-INFO
+-rw-r--r--   0 jhkang     (501) staff       (20)     1988 2024-04-23 12:48:39.000000 fisspy-1.0.8/README.md
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-26 10:47:37.056470 fisspy-1.0.8/fisspy/
+-rw-r--r--   0 jhkang     (501) staff       (20)      430 2024-04-26 10:04:56.000000 fisspy-1.0.8/fisspy/__init__.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-26 10:47:37.057775 fisspy-1.0.8/fisspy/align/
+-rw-r--r--   0 jhkang     (501) staff       (20)       44 2024-04-20 02:57:09.000000 fisspy-1.0.8/fisspy/align/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15179 2024-04-24 08:05:01.000000 fisspy-1.0.8/fisspy/align/alignment.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11470 2024-04-25 11:40:56.000000 fisspy-1.0.8/fisspy/align/base.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-26 10:47:37.059414 fisspy-1.0.8/fisspy/analysis/
+-rw-r--r--   0 jhkang     (501) staff       (20)      317 2024-04-20 02:57:09.000000 fisspy-1.0.8/fisspy/analysis/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    12577 2024-04-25 11:37:49.000000 fisspy-1.0.8/fisspy/analysis/doppler.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1030 2024-04-20 02:57:09.000000 fisspy-1.0.8/fisspy/analysis/filter.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2988 2024-04-25 11:30:36.000000 fisspy-1.0.8/fisspy/analysis/forecast.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15224 2024-04-20 02:57:09.000000 fisspy-1.0.8/fisspy/analysis/ofe.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    35498 2024-04-25 11:29:47.000000 fisspy-1.0.8/fisspy/analysis/tdmap.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    33907 2024-04-25 11:35:30.000000 fisspy-1.0.8/fisspy/analysis/wavelet.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    19011 2023-07-14 01:35:52.000000 fisspy-1.0.8/fisspy/cm.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-26 10:47:37.059824 fisspy-1.0.8/fisspy/correction/
+-rw-r--r--   0 jhkang     (501) staff       (20)       51 2024-04-20 02:57:09.000000 fisspy-1.0.8/fisspy/correction/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11372 2024-04-20 02:57:09.000000 fisspy-1.0.8/fisspy/correction/correction.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2337 2024-04-20 02:57:09.000000 fisspy-1.0.8/fisspy/correction/get_inform.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-26 10:47:37.060418 fisspy-1.0.8/fisspy/data/
+-rw-r--r--   0 jhkang     (501) staff       (20)       64 2023-07-25 08:49:17.000000 fisspy-1.0.8/fisspy/data/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1072 2023-07-25 08:49:17.000000 fisspy-1.0.8/fisspy/data/_sample.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2965 2023-07-25 08:49:17.000000 fisspy-1.0.8/fisspy/data/download.py
+-rw-r--r--   0 jhkang     (501) staff       (20)      394 2023-07-14 01:35:52.000000 fisspy-1.0.8/fisspy/data/sample.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-26 10:47:37.060918 fisspy-1.0.8/fisspy/image/
+-rw-r--r--   0 jhkang     (501) staff       (20)       73 2024-04-25 10:45:58.000000 fisspy-1.0.8/fisspy/image/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    29769 2024-04-25 11:21:02.000000 fisspy-1.0.8/fisspy/image/interactive_image.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11762 2024-04-26 09:44:52.000000 fisspy-1.0.8/fisspy/image/raster_set.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-26 10:47:37.061185 fisspy-1.0.8/fisspy/inversion/
+-rw-r--r--   0 jhkang     (501) staff       (20)        0 2024-04-20 02:57:09.000000 fisspy-1.0.8/fisspy/inversion/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)      181 2024-04-20 02:57:09.000000 fisspy-1.0.8/fisspy/inversion/_mlsi.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-26 10:47:37.061666 fisspy-1.0.8/fisspy/io/
+-rw-r--r--   0 jhkang     (501) staff       (20)      320 2023-07-14 01:35:52.000000 fisspy-1.0.8/fisspy/io/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15840 2023-07-14 01:35:52.000000 fisspy-1.0.8/fisspy/io/read.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     4974 2024-04-20 02:57:09.000000 fisspy-1.0.8/fisspy/makevideo.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-26 10:47:37.062403 fisspy-1.0.8/fisspy/preprocess/
+-rw-r--r--   0 jhkang     (501) staff       (20)       29 2024-04-20 02:57:09.000000 fisspy-1.0.8/fisspy/preprocess/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    52443 2024-04-25 11:18:41.000000 fisspy-1.0.8/fisspy/preprocess/proc_base.py
+-rw-r--r--   0 jhkang     (501) staff       (20)   144078 2024-04-26 10:31:20.000000 fisspy-1.0.8/fisspy/preprocess/proc_gui.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1685 2024-04-20 02:57:09.000000 fisspy-1.0.8/fisspy/preprocess/t_y_sh.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-26 10:47:37.063622 fisspy-1.0.8/fisspy/read/
+-rw-r--r--   0 jhkang     (501) staff       (20)      195 2024-04-20 02:57:09.000000 fisspy-1.0.8/fisspy/read/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    49241 2024-04-26 03:08:29.000000 fisspy-1.0.8/fisspy/read/read_factory.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     6847 2024-04-25 06:03:54.000000 fisspy-1.0.8/fisspy/read/readbase.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-26 10:47:37.057352 fisspy-1.0.8/fisspy.egg-info/
+-rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-04-26 10:47:37.000000 fisspy-1.0.8/fisspy.egg-info/PKG-INFO
+-rw-r--r--   0 jhkang     (501) staff       (20)     1079 2024-04-26 10:47:37.000000 fisspy-1.0.8/fisspy.egg-info/SOURCES.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-26 10:47:37.000000 fisspy-1.0.8/fisspy.egg-info/dependency_links.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-26 10:47:37.000000 fisspy-1.0.8/fisspy.egg-info/not-zip-safe
+-rw-r--r--   0 jhkang     (501) staff       (20)      137 2024-04-26 10:47:37.000000 fisspy-1.0.8/fisspy.egg-info/requires.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        7 2024-04-26 10:47:37.000000 fisspy-1.0.8/fisspy.egg-info/top_level.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)       38 2024-04-26 10:47:37.064482 fisspy-1.0.8/setup.cfg
+-rw-r--r--   0 jhkang     (501) staff       (20)      582 2024-04-26 10:04:44.000000 fisspy-1.0.8/setup.py
```

### Comparing `fisspy-1.0.7/LICENSE.txt` & `fisspy-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.7/PKG-INFO` & `fisspy-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fisspy
-Version: 1.0.7
+Version: 1.0.8
 Summary: fisspy: Python analysis tools for GST/FISS
 Home-page: http://fiss.snu.ac.kr
 Author: Juhyung Kang
 Author-email: jhkang@astro.snu.ac.kr
 License: BSD-2
 Requires-Python: >=3.6
 License-File: LICENSE.txt
```

### Comparing `fisspy-1.0.7/README.md` & `fisspy-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.7/fisspy/align/alignment.py` & `fisspy-1.0.8/fisspy/align/alignment.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.7/fisspy/align/base.py` & `fisspy-1.0.8/fisspy/align/base.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.7/fisspy/analysis/doppler.py` & `fisspy-1.0.8/fisspy/analysis/doppler.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.7/fisspy/analysis/filter.py` & `fisspy-1.0.8/fisspy/analysis/filter.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.7/fisspy/analysis/forecast.py` & `fisspy-1.0.8/fisspy/analysis/forecast.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.7/fisspy/analysis/ofe.py` & `fisspy-1.0.8/fisspy/analysis/ofe.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.7/fisspy/analysis/tdmap.py` & `fisspy-1.0.8/fisspy/analysis/tdmap.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.7/fisspy/analysis/wavelet.py` & `fisspy-1.0.8/fisspy/analysis/wavelet.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.7/fisspy/cm.py` & `fisspy-1.0.8/fisspy/cm.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.7/fisspy/correction/correction.py` & `fisspy-1.0.8/fisspy/correction/correction.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.7/fisspy/correction/get_inform.py` & `fisspy-1.0.8/fisspy/correction/get_inform.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.7/fisspy/data/_sample.py` & `fisspy-1.0.8/fisspy/data/_sample.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.7/fisspy/data/download.py` & `fisspy-1.0.8/fisspy/data/download.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.7/fisspy/image/interactive_image.py` & `fisspy-1.0.8/fisspy/image/interactive_image.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.7/fisspy/image/raster_set.py` & `fisspy-1.0.8/fisspy/image/raster_set.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         bg_second = "#484c4f"
         fontcolor = "#adb5bd"
         titlecolor = "#ffda6a"
         self.time = np.zeros(self.nf, dtype=float)
         self.anx = np.zeros(self.nf, dtype=int)
 
         A, B, time = self.loadData(ii)
+        self.rh = A.header
         cwvA = A.centralWavelength
         cwvB = B.centralWavelength
 
         if wvset is None:
             wvSet = np.array([-4, -0.7, -0.5, -0.2, 0, 0.2, 0.5, 0.7])
         else:
             wvSet = wvset
@@ -247,14 +248,15 @@
 
         Returns
         -------
         None
         """
         self.ani = FuncAnimation(self.fig, self.chData, frames=np.arange(self.nf), interval=interval)
         self.fig.canvas.draw_idle()
+            
 
     def saveAnimation(self, dirn):
         """
         Save animation
         
         Parameters
         ----------
@@ -263,17 +265,23 @@
         
         Returns
         -------
         None
         """
         if self.ani is None:
             self.animation()
-        mname = join(dirn, f'{self.stT.isot}.mp4')
+        tmp = self.rh['target'].replace(' ', '')
+        mname = join(dirn, tmp+'_01.mp4')
+        if isfile(mname):
+            lf = len(glob(join(dirn, tmp+'*.mp4')))
+            mname = mname.replace("01.mp4", f"{lf+1:02}.mp4")
         self.ani.save(mname)
         self.fname_movie = mname
+        if not self.show:
+            plt.close(self.fig)
 
     def makeCatalogFiles(self, dirn):
         """
         Make JSON file for the data catalog
 
         Parameters
         ----------
@@ -293,15 +301,20 @@
         ddir = join(bdir, 'data')
         if not isdir(mdir):
             mkdir(mdir)
         if not isdir(idir):
             mkdir(idir)
         if not isdir(ddir):
             mkdir(ddir)
-        move(self.fname_movie, join(mdir, basename(self.fname_movie)))
+
+        amname = basename(self.fname_movie)
+        if isfile(join(mdir,amname)):
+            lf = len(glob(join(mdir, amname[:-6]+'*.mp4')))
+            amname = amname.replace(amname[-6:], f"{lf+1:02}.mp4")
+        move(self.fname_movie, join(mdir, amname))
 
         # make image
         A, B, time = self.loadData(self.nf//2)
         h = A.header
         ifname = self.title.get_text().replace(':','_').replace('-','_')+'.png'
         self.saveImage(join(idir, ifname), i=self.nf//2)
 
@@ -343,18 +356,18 @@
             k = glob(join(bdir,f'*_{date}.json'))
             nk = len(k)
             fjson = join(bdir, f"{nk+1:02}_{date}.json")
 
         opn = open(fjson, 'w')
         opn.write('{\n')
         opn.write(f"""  "observer": "{observer}",\n""")
-        opn.write(f"""  "observer": "{obstime}",\n""")
+        opn.write(f"""  "obstime": "{obstime}",\n""")
         opn.write(f"""  "target": "{target}",\n""")
         opn.write(f"""  "position": {position},\n""")
         opn.write(f"""  "cadence": "{dt:.2f}",\n""")
         opn.write(f"""  "obsarea": ["{ax:.0f}", "{ay:.0f}"],\n""")
         opn.write(f"""  "imgA": "{ifname}",\n""")
         opn.write(f"""  "imgB": "",\n""")
-        opn.write(f"""  "movie": ["{basename(self.fname_movie)}"],\n""")
+        opn.write(f"""  "movie": ["{amname}"],\n""")
         opn.write(f"""  "data": ["{basename(zipname)}"]\n""")
         opn.write('}')
         opn.close()
```

### Comparing `fisspy-1.0.7/fisspy/io/read.py` & `fisspy-1.0.8/fisspy/io/read.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.7/fisspy/makevideo.py` & `fisspy-1.0.8/fisspy/makevideo.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.7/fisspy/preprocess/proc_base.py` & `fisspy-1.0.8/fisspy/preprocess/proc_base.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.7/fisspy/preprocess/proc_gui.py` & `fisspy-1.0.8/fisspy/preprocess/proc_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -3137,14 +3137,15 @@
                         hdu.header['STRTIME'] = (h['STRTIME'], 'Scan Start Time')
                         hdu.header['ENDTIME'] = (h['ENDTIME'], 'Scan Finish Time')
                         hdu.header['HBINNING'] = (h['HBINNING'], 'Horizontal Binning')
                         hdu.header['VBINNING'] = (h['VBINNING'], 'Vertical Binning')
                         hdu.header['OBSERVER'] = (h['OBSERVER'], 'The name of main observer')
                         hdu.header['TEL_XPOS'] = (h['TEL_XPOS'], 'X position of Telescope on the Sun')
                         hdu.header['TEL_YPOS'] = (h['TEL_YPOS'], 'X position of Telescope on the Sun')
+                        hdu.header['TARGET'] = (h['TARGET'], 'Observation Target')
                         hdu.header['TILT'] = (ch['tilt'], 'Degree')
                         hdu.header['COEF1_0'] = (ch['coef1_0'], 'Curvature correction coeff p0')
                         hdu.header['COEF1_1'] = (ch['coef1_1'], 'Curvature correction coeff p1')
                         hdu.header['COEF1_2'] = (ch['coef1_2'], 'Curvature correction coeff p2')
                         hdu.header['COEF2_0'] = (ch['coef2_0'], '2nd Curvature correction coeff p0')
                         hdu.header['COEF2_1'] = (ch['coef2_1'], '2nd Curvature correction coeff p1')
                         hdu.header['COEF2_2'] = (ch['coef2_2'], '2nd Curvature correction coeff p2')
@@ -3153,14 +3154,22 @@
                             hdu.header['WAVELEN'] = (ch['WAVELEN'], 'Angstrom')
                         except:
                             pass
                         try:
                             hdu.header['GRATWVLN'] = (ch['GRATWVLN'], 'Angstrom')
                         except:
                             pass
+                        hdu.header['GRATSTEP'] = (ch['GRATSTEP'], 'Grating step count')
+                        hdu.header['GRATANGL'] = (ch['GRATANGL'], 'Grating angle')
+                        hdu.header['CCDTEMP'] = (ch['CCDTEMP'], 'Cooling Temperature of CCD')
+                        hdu.header['STEPSIZE'] = (ch['STEPSIZE'], 'Step size to move scanner (um)')
+                        hdu.header['STEPTIME'] = (ch['STEPTIME'], 'Step duration time (ms)')
+                        hdu.header['ELAPTIME'] = (ch['ELAPTIME'], 'Elapse time during scanning (s)')
+                        hdu.header['PAMPGAIN'] = (ch['PAMPGAIN'], 'Value Range: 0-2')
+                        hdu.header['EMGAIN'] = (ch['EMGAIN'], 'Value Range: 0-255')
                         hdu.header.add_comment('Tilt Corrected')
                         hdu.header.add_comment('1st Curvature Corrected')
                         hdu.header.add_comment('2nd Curvature Corrected')
                         if len(tlfYF[idx]):
                             hdu.header.add_comment('y-dir Fringe Subtractd')
                         if len(tlfXF[idx]):
                             hdu.header.add_comment('x-dir Fringe Subtractd')
```

### Comparing `fisspy-1.0.7/fisspy/preprocess/t_y_sh.py` & `fisspy-1.0.8/fisspy/preprocess/t_y_sh.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.7/fisspy/read/read_factory.py` & `fisspy-1.0.8/fisspy/read/read_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
     Examples
     --------
     >>> from fisspy import read
     >>> import fisspy.data.sample
     >>> fiss = read.FISS(fisspy.data.sample.FISS_IMAGE)
     """
 
-    def __init__(self, file, x1=0, x2=None, y1=0, y2=None, ncoeff=False, smoothingMethod=None, wvCalibMethod='photo', **kwargs):
+    def __init__(self, file, x1=0, x2=None, y1=0, y2=None, ncoeff=False, smoothingMethod=None, wvCalibMethod='simple', **kwargs):
         if file.find('1.fts') != -1:
             self.ftype = 'proc'
         elif file.find('c.fts') != -1:
             self.ftype = 'comp'
 
         if self.ftype != 'proc' and self.ftype != 'comp':
             raise ValueError("Input file is neither proc nor comp data")
@@ -352,15 +352,19 @@
         wv: `~numpy.ndarray`
             Wavelength.
         """
         if profile is None:
             pf = self.refProfile
         else:
             pf = profile
-        return wvCalib(pf, self.header, method=method)
+        try:
+            wv = wvCalib(pf, self.header, method=method)
+        except:
+            raise ValueError(f"Please change the wvCalibMethod among 'simple', 'center', and 'photo'. Current: {method}")
+        return wv
 
     def CorSLA(self, refProf=None, pure=None, eps=0.027, zeta=0.055):
         """
         Correction of spectral line(s) profile for stray linght and far wing red-blue asymmetry.
 
         Parameters
         ----------
```

### Comparing `fisspy-1.0.7/fisspy/read/readbase.py` & `fisspy-1.0.8/fisspy/read/readbase.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.7/fisspy.egg-info/PKG-INFO` & `fisspy-1.0.8/fisspy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fisspy
-Version: 1.0.7
+Version: 1.0.8
 Summary: fisspy: Python analysis tools for GST/FISS
 Home-page: http://fiss.snu.ac.kr
 Author: Juhyung Kang
 Author-email: jhkang@astro.snu.ac.kr
 License: BSD-2
 Requires-Python: >=3.6
 License-File: LICENSE.txt
```

### Comparing `fisspy-1.0.7/fisspy.egg-info/SOURCES.txt` & `fisspy-1.0.8/fisspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.7/setup.py` & `fisspy-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fisspy',
-    version='1.0.7',
+    version='1.0.8',
     description='fisspy: Python analysis tools for GST/FISS',
     url='http://fiss.snu.ac.kr',
     author='Juhyung Kang',
     author_email='jhkang@astro.snu.ac.kr',
     license='BSD-2',
     python_requires='>=3.6',
     packages=find_packages(exclude=['docs', 'logo']),
```

