# Comparing `tmp/mutechromecastads-0.1.0.tar.gz` & `tmp/mutechromecastads-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutechromecastads-0.1.0.tar", max compression
+gzip compressed data, was "mutechromecastads-0.1.1.tar", max compression
```

## Comparing `mutechromecastads-0.1.0.tar` & `mutechromecastads-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      976 2024-04-27 07:07:26.726900 mutechromecastads-0.1.0/README.md
--rw-r--r--   0        0        0     1868 2024-04-27 07:07:26.726900 mutechromecastads-0.1.0/mutechromecastads.py
--rw-r--r--   0        0        0      318 2024-04-27 07:07:26.726900 mutechromecastads-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 mutechromecastads-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      981 2024-04-27 07:21:32.604466 mutechromecastads-0.1.1/README.md
+-rw-r--r--   0        0        0     1868 2024-04-27 07:21:32.604466 mutechromecastads-0.1.1/mutechromecastads.py
+-rw-r--r--   0        0        0      386 2024-04-27 07:21:32.604466 mutechromecastads-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1450 1970-01-01 00:00:00.000000 mutechromecastads-0.1.1/PKG-INFO
```

### Comparing `mutechromecastads-0.1.0/README.md` & `mutechromecastads-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,13 +18,13 @@
 > ```
 >
 > where hostname is the hostname or the ip of the chromecast device
 
 ### podman
 
 > ```bash
-> podman run --env CHROMECAST_HOST=hostname ghcr.io/rikyiso01/mutechromecastads
+> podman run --rm --env CHROMECAST_HOST=hostname ghcr.io/rikyiso01/mutechromecastads
 > ```
 >
 > where hostname is the hostname or the ip of the chromecast device
 
 After doing this the program will start looping and will mute the device when the broadcasted song title is 'Advertisement'
```

### Comparing `mutechromecastads-0.1.0/mutechromecastads.py` & `mutechromecastads-0.1.1/mutechromecastads.py`

 * *Files identical despite different names*

### Comparing `mutechromecastads-0.1.0/PKG-INFO` & `mutechromecastads-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutechromecastads
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: rikyiso01
 Author-email: riky.isola@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -33,14 +33,14 @@
 > ```
 >
 > where hostname is the hostname or the ip of the chromecast device
 
 ### podman
 
 > ```bash
-> podman run --env CHROMECAST_HOST=hostname ghcr.io/rikyiso01/mutechromecastads
+> podman run --rm --env CHROMECAST_HOST=hostname ghcr.io/rikyiso01/mutechromecastads
 > ```
 >
 > where hostname is the hostname or the ip of the chromecast device
 
 After doing this the program will start looping and will mute the device when the broadcasted song title is 'Advertisement'
```

