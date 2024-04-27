# Comparing `tmp/SimpleTKMessageBox-0.2.2.tar.gz` & `tmp/SimpleTKMessageBox-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleTKMessageBox-0.2.2.tar", last modified: Sat Apr 27 11:59:45 2024, max compression
+gzip compressed data, was "SimpleTKMessageBox-0.2.3.tar", last modified: Sat Apr 27 12:02:14 2024, max compression
```

## Comparing `SimpleTKMessageBox-0.2.2.tar` & `SimpleTKMessageBox-0.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 11:59:45.977463 SimpleTKMessageBox-0.2.2/
--rw-rw-rw-   0        0        0       25 2024-04-27 11:31:25.000000 SimpleTKMessageBox-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0      400 2024-04-27 11:59:45.974464 SimpleTKMessageBox-0.2.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-27 11:59:45.971464 SimpleTKMessageBox-0.2.2/SimpleTKMessageBox.egg-info/
--rw-rw-rw-   0        0        0      400 2024-04-27 11:59:45.000000 SimpleTKMessageBox-0.2.2/SimpleTKMessageBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      821 2024-04-27 11:59:45.000000 SimpleTKMessageBox-0.2.2/SimpleTKMessageBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 11:59:45.000000 SimpleTKMessageBox-0.2.2/SimpleTKMessageBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-27 11:59:45.000000 SimpleTKMessageBox-0.2.2/SimpleTKMessageBox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-27 11:59:45.770584 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/
--rw-rw-rw-   0        0        0     3558 2024-04-27 11:59:39.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/SimpleTkMessageBox.py
--rw-rw-rw-   0        0        0       59 2024-04-27 10:36:23.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:59:45.783572 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/
-drwxrwxrwx   0        0        0        0 2024-04-27 11:59:45.846536 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W10/
--rw-rw-rw-   0        0        0     1051 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W10/1.png
--rw-rw-rw-   0        0        0     1395 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W10/2.png
--rw-rw-rw-   0        0        0      725 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W10/3.png
--rw-rw-rw-   0        0        0     1423 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W10/4.png
--rw-rw-rw-   0        0        0     1145 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W10/5.png
-drwxrwxrwx   0        0        0        0 2024-04-27 11:59:45.900506 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W11/
--rw-rw-rw-   0        0        0     3154 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W11/1.png
--rw-rw-rw-   0        0        0     1847 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W11/2.png
--rw-rw-rw-   0        0        0     3264 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W11/3.png
--rw-rw-rw-   0        0        0     4962 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W11/4.png
--rw-rw-rw-   0        0        0     4565 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W11/5.png
-drwxrwxrwx   0        0        0        0 2024-04-27 11:59:45.967469 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W7/
--rw-rw-rw-   0        0        0     6639 2024-04-23 17:03:58.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W7/1.png
--rw-rw-rw-   0        0        0     2797 2024-04-23 17:01:54.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W7/2.png
--rw-rw-rw-   0        0        0     5154 2024-04-23 17:01:56.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W7/3.png
--rw-rw-rw-   0        0        0     6070 2024-04-23 17:01:59.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W7/4.png
--rw-rw-rw-   0        0        0     5708 2024-04-23 17:02:02.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W7/5.png
--rw-rw-rw-   0        0        0     1406 2024-04-24 08:46:15.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/transparent.ico
--rw-rw-rw-   0        0        0       42 2024-04-27 11:59:45.978461 SimpleTKMessageBox-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1305 2024-04-27 11:58:22.000000 SimpleTKMessageBox-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 12:02:14.451526 SimpleTKMessageBox-0.2.3/
+-rw-rw-rw-   0        0        0       25 2024-04-27 11:31:25.000000 SimpleTKMessageBox-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      400 2024-04-27 12:02:14.448530 SimpleTKMessageBox-0.2.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-27 12:02:14.445530 SimpleTKMessageBox-0.2.3/SimpleTKMessageBox.egg-info/
+-rw-rw-rw-   0        0        0      400 2024-04-27 12:02:14.000000 SimpleTKMessageBox-0.2.3/SimpleTKMessageBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      821 2024-04-27 12:02:14.000000 SimpleTKMessageBox-0.2.3/SimpleTKMessageBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 12:02:14.000000 SimpleTKMessageBox-0.2.3/SimpleTKMessageBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-27 12:02:14.000000 SimpleTKMessageBox-0.2.3/SimpleTKMessageBox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 12:02:14.392560 SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/
+-rw-rw-rw-   0        0        0     3558 2024-04-27 11:59:39.000000 SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/SimpleTkMessageBox.py
+-rw-rw-rw-   0        0        0       59 2024-04-27 10:36:23.000000 SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 12:02:14.395562 SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/
+drwxrwxrwx   0        0        0        0 2024-04-27 12:02:14.410550 SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W10/
+-rw-rw-rw-   0        0        0     1051 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W10/1.png
+-rw-rw-rw-   0        0        0     1395 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W10/2.png
+-rw-rw-rw-   0        0        0      725 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W10/3.png
+-rw-rw-rw-   0        0        0     1423 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W10/4.png
+-rw-rw-rw-   0        0        0     1145 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W10/5.png
+drwxrwxrwx   0        0        0        0 2024-04-27 12:02:14.425542 SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W11/
+-rw-rw-rw-   0        0        0     3154 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W11/1.png
+-rw-rw-rw-   0        0        0     1847 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W11/2.png
+-rw-rw-rw-   0        0        0     3264 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W11/3.png
+-rw-rw-rw-   0        0        0     4962 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W11/4.png
+-rw-rw-rw-   0        0        0     4565 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W11/5.png
+drwxrwxrwx   0        0        0        0 2024-04-27 12:02:14.440534 SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W7/
+-rw-rw-rw-   0        0        0     6639 2024-04-23 17:03:58.000000 SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W7/1.png
+-rw-rw-rw-   0        0        0     2797 2024-04-23 17:01:54.000000 SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W7/2.png
+-rw-rw-rw-   0        0        0     5154 2024-04-23 17:01:56.000000 SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W7/3.png
+-rw-rw-rw-   0        0        0     6070 2024-04-23 17:01:59.000000 SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W7/4.png
+-rw-rw-rw-   0        0        0     5708 2024-04-23 17:02:02.000000 SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W7/5.png
+-rw-rw-rw-   0        0        0     1406 2024-04-24 08:46:15.000000 SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/transparent.ico
+-rw-rw-rw-   0        0        0       42 2024-04-27 12:02:14.451526 SimpleTKMessageBox-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1304 2024-04-27 12:02:08.000000 SimpleTKMessageBox-0.2.3/setup.py
```

### Comparing `SimpleTKMessageBox-0.2.2/SimpleTKMessageBox.egg-info/SOURCES.txt` & `SimpleTKMessageBox-0.2.3/SimpleTKMessageBox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/SimpleTkMessageBox.py` & `SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/SimpleTkMessageBox.py`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W10/1.png` & `SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W10/1.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W10/2.png` & `SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W10/2.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W10/3.png` & `SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W10/3.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W10/4.png` & `SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W10/4.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W10/5.png` & `SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W10/5.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W11/1.png` & `SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W11/1.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W11/2.png` & `SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W11/2.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W11/3.png` & `SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W11/3.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W11/4.png` & `SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W11/4.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W11/5.png` & `SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W11/5.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W7/1.png` & `SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W7/1.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W7/2.png` & `SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W7/2.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W7/3.png` & `SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W7/3.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W7/4.png` & `SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W7/4.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W7/5.png` & `SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/W7/5.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/transparent.ico` & `SimpleTKMessageBox-0.2.3/SimpleTkMessageBox/icons/transparent.ico`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.2/setup.py` & `SimpleTKMessageBox-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 setup(
 name='SimpleTKMessageBox',
-version='0.2.2',
+version='0.2.3',
 author='Gustoon',
 author_email='no.email@gmail.com',
 description='A simple tkinter message box',
 long_description="""
 See documentation at https://github.com/Gustoon/SimpleTkMessageBox
 """,
 packages=find_packages(),
 include_package_data=True,
 data_files=[
-    ('SimpleTkMessageBox/icons/', ['SimpleTkMessageBox/icons/transparent.ico']),
+    ('SimpleTkMessageBox/icons', ['SimpleTkMessageBox/icons/transparent.ico']),
     ('SimpleTkMessageBox/icons/W11', ['SimpleTkMessageBox/icons/W11/1.png', 'SimpleTkMessageBox/icons/W11/2.png', 'SimpleTkMessageBox/icons/W11/3.png', 'SimpleTkMessageBox/icons/W11/4.png', 'SimpleTkMessageBox/icons/W11/5.png']),
     ('SimpleTkMessageBox/icons/W10', ['SimpleTkMessageBox/icons/W10/1.png', 'SimpleTkMessageBox/icons/W10/2.png', 'SimpleTkMessageBox/icons/W10/3.png', 'SimpleTkMessageBox/icons/W10/4.png', 'SimpleTkMessageBox/icons/W10/5.png']),
     ('SimpleTkMessageBox/icons/W7', ['SimpleTkMessageBox/icons/W7/1.png', 'SimpleTkMessageBox/icons/W7/2.png', 'SimpleTkMessageBox/icons/W7/3.png', 'SimpleTkMessageBox/icons/W7/4.png', 'SimpleTkMessageBox/icons/W7/5.png']),
 ],
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
```

