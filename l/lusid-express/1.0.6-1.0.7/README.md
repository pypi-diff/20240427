# Comparing `tmp/lusid_express-1.0.6.tar.gz` & `tmp/lusid_express-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_express-1.0.6.tar", last modified: Sat Apr 27 19:32:59 2024, max compression
+gzip compressed data, was "lusid_express-1.0.7.tar", last modified: Sat Apr 27 19:37:26 2024, max compression
```

## Comparing `lusid_express-1.0.6.tar` & `lusid_express-1.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:32:59.427700 lusid_express-1.0.6/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-27 19:32:21.000000 lusid_express-1.0.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-27 19:32:21.000000 lusid_express-1.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6659 2024-04-27 19:32:59.427700 lusid_express-1.0.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6019 2024-04-27 19:32:21.000000 lusid_express-1.0.6/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 19:32:59.427700 lusid_express-1.0.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-27 19:32:21.000000 lusid_express-1.0.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:32:59.421700 lusid_express-1.0.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:32:59.423700 lusid_express-1.0.6/src/lusid_express/
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-27 19:32:21.000000 lusid_express-1.0.6/src/lusid_express/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5616 2024-04-27 19:32:21.000000 lusid_express-1.0.6/src/lusid_express/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:32:59.425700 lusid_express-1.0.6/src/lusid_express/apis/
--rw-rw-rw-   0 root         (0) root         (0)  2240138 2024-04-27 19:32:59.000000 lusid_express-1.0.6/src/lusid_express/apis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:32:59.426700 lusid_express-1.0.6/src/lusid_express/config/
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-27 19:32:21.000000 lusid_express-1.0.6/src/lusid_express/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:32:59.427700 lusid_express-1.0.6/src/lusid_express/display/
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-27 19:32:21.000000 lusid_express-1.0.6/src/lusid_express/display/PRELOADED_VARS.md
--rw-rw-rw-   0 root         (0) root         (0)    10715 2024-04-27 19:32:21.000000 lusid_express-1.0.6/src/lusid_express/display/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2352 2024-04-27 19:32:21.000000 lusid_express-1.0.6/src/lusid_express/load.le
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:32:59.424700 lusid_express-1.0.6/src/lusid_express.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6659 2024-04-27 19:32:59.000000 lusid_express-1.0.6/src/lusid_express.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      482 2024-04-27 19:32:59.000000 lusid_express-1.0.6/src/lusid_express.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 19:32:59.000000 lusid_express-1.0.6/src/lusid_express.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-27 19:32:59.000000 lusid_express-1.0.6/src/lusid_express.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-27 19:32:59.000000 lusid_express-1.0.6/src/lusid_express.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:37:26.164184 lusid_express-1.0.7/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-27 19:36:46.000000 lusid_express-1.0.7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-27 19:36:46.000000 lusid_express-1.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6659 2024-04-27 19:37:26.164184 lusid_express-1.0.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6019 2024-04-27 19:36:46.000000 lusid_express-1.0.7/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 19:37:26.164184 lusid_express-1.0.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-27 19:36:46.000000 lusid_express-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:37:26.158186 lusid_express-1.0.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:37:26.160185 lusid_express-1.0.7/src/lusid_express/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-27 19:36:46.000000 lusid_express-1.0.7/src/lusid_express/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5616 2024-04-27 19:36:46.000000 lusid_express-1.0.7/src/lusid_express/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:37:26.161185 lusid_express-1.0.7/src/lusid_express/apis/
+-rw-rw-rw-   0 root         (0) root         (0)  2240138 2024-04-27 19:37:25.000000 lusid_express-1.0.7/src/lusid_express/apis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:37:26.163184 lusid_express-1.0.7/src/lusid_express/config/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-27 19:36:46.000000 lusid_express-1.0.7/src/lusid_express/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:37:26.164184 lusid_express-1.0.7/src/lusid_express/display/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-27 19:36:46.000000 lusid_express-1.0.7/src/lusid_express/display/PRELOADED_VARS.md
+-rw-rw-rw-   0 root         (0) root         (0)    10739 2024-04-27 19:36:46.000000 lusid_express-1.0.7/src/lusid_express/display/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2352 2024-04-27 19:36:46.000000 lusid_express-1.0.7/src/lusid_express/load.le
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:37:26.161185 lusid_express-1.0.7/src/lusid_express.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6659 2024-04-27 19:37:26.000000 lusid_express-1.0.7/src/lusid_express.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      482 2024-04-27 19:37:26.000000 lusid_express-1.0.7/src/lusid_express.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 19:37:26.000000 lusid_express-1.0.7/src/lusid_express.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-27 19:37:26.000000 lusid_express-1.0.7/src/lusid_express.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-27 19:37:26.000000 lusid_express-1.0.7/src/lusid_express.egg-info/top_level.txt
```

### Comparing `lusid_express-1.0.6/LICENSE` & `lusid_express-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.6/PKG-INFO` & `lusid_express-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid_express
-Version: 1.0.6
+Version: 1.0.7
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_express-1.0.6/README.md` & `lusid_express-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.6/setup.py` & `lusid_express-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ]
 
 
 
 
 setup(
     name='lusid_express',
-    version='1.0.6',
+    version='1.0.7',
     package_dir={'': 'src'},  # tells setuptools that packages are under src
     packages=find_packages(where='src'),  # tells setuptools to look for packages in src
     install_requires=requirements,
     description='lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.',
     long_description=open('README.md').read(),
     include_package_data=True,  
     long_description_content_type='text/markdown',
```

### Comparing `lusid_express-1.0.6/src/lusid_express/__main__.py` & `lusid_express-1.0.7/src/lusid_express/__main__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.6/src/lusid_express/apis/__init__.py` & `lusid_express-1.0.7/src/lusid_express/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.6/src/lusid_express/display/PRELOADED_VARS.md` & `lusid_express-1.0.7/src/lusid_express/display/PRELOADED_VARS.md`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.6/src/lusid_express/display/__init__.py` & `lusid_express-1.0.7/src/lusid_express/display/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,17 +42,17 @@
   background-color: #FFFFFF;
   border: 1px solid rgb(209,213,219);
   border-radius: .5rem;
   box-sizing: border-box;
   color: #111827;
   font-family: "Inter var",ui-sans-serif,system-ui,-apple-system,system-ui,"Segoe UI",Roboto,"Helvetica Neue",Arial,"Noto Sans",sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol","Noto Color Emoji";
   font-size: .875rem;
-  font-weight: 600;
+  font-weight: 300 !important;
   line-height: 1.25rem;
-  padding: .75rem 1rem;
+  padding: .25rem 0.5rem !important;
   text-align: center;
   text-decoration: none #D1D5DB solid;
   text-decoration-thickness: auto;
   box-shadow: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
   cursor: pointer;
   user-select: none;
   -webkit-user-select: none;
```

### Comparing `lusid_express-1.0.6/src/lusid_express/load.le` & `lusid_express-1.0.7/src/lusid_express/load.le`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.6/src/lusid_express.egg-info/PKG-INFO` & `lusid_express-1.0.7/src/lusid_express.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-express
-Version: 1.0.6
+Version: 1.0.7
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

