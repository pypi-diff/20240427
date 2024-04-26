# Comparing `tmp/openmindat-0.0.5.tar.gz` & `tmp/openmindat-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmindat-0.0.5.tar", last modified: Fri Apr 26 17:48:24 2024, max compression
+gzip compressed data, was "openmindat-0.0.6.tar", last modified: Fri Apr 26 17:56:52 2024, max compression
```

## Comparing `openmindat-0.0.5.tar` & `openmindat-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 blc        (501) staff       (20)        0 2024-04-26 17:48:24.532507 openmindat-0.0.5/
--rw-r--r--   0 blc        (501) staff       (20)    11357 2023-09-28 23:58:40.000000 openmindat-0.0.5/LICENSE
--rw-r--r--   0 blc        (501) staff       (20)      136 2024-04-09 06:30:41.000000 openmindat-0.0.5/MANIFEST.in
--rw-r--r--   0 blc        (501) staff       (20)     6247 2024-04-26 17:48:24.532266 openmindat-0.0.5/PKG-INFO
--rw-r--r--   0 blc        (501) staff       (20)     5741 2024-04-26 17:47:50.000000 openmindat-0.0.5/README.md
-drwxr-xr-x   0 blc        (501) staff       (20)        0 2024-04-26 17:48:24.530653 openmindat-0.0.5/openmindat/
--rw-r--r--   0 blc        (501) staff       (20)     6087 2024-04-25 18:17:20.000000 openmindat-0.0.5/openmindat/__init__.py
--rw-r--r--   0 blc        (501) staff       (20)     8320 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/countries.py
--rw-r--r--   0 blc        (501) staff       (20)     5656 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/dana8.py
--rw-r--r--   0 blc        (501) staff       (20)    47522 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/geomaterials.py
--rw-r--r--   0 blc        (501) staff       (20)     4207 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/geomaterials_search.py
--rw-r--r--   0 blc        (501) staff       (20)    20573 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/localities.py
--rw-r--r--   0 blc        (501) staff       (20)     8378 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/localities_age.py
--rw-r--r--   0 blc        (501) staff       (20)     8578 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/localities_status.py
--rw-r--r--   0 blc        (501) staff       (20)     8535 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/localities_type.py
--rw-r--r--   0 blc        (501) staff       (20)     4215 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/locgeoregion2.py
--rw-r--r--   0 blc        (501) staff       (20)     3775 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/locobject.py
--rw-r--r--   0 blc        (501) staff       (20)     9166 2024-04-25 17:55:43.000000 openmindat-0.0.5/openmindat/mindat_api.py
--rw-r--r--   0 blc        (501) staff       (20)    13796 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/minerals_ima.py
--rw-r--r--   0 blc        (501) staff       (20)     6120 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/nickel_strunz.py
--rw-r--r--   0 blc        (501) staff       (20)     3496 2024-04-26 17:35:31.000000 openmindat-0.0.5/openmindat/photo_count.py
-drwxr-xr-x   0 blc        (501) staff       (20)        0 2024-04-26 17:48:24.531961 openmindat-0.0.5/openmindat.egg-info/
--rw-r--r--   0 blc        (501) staff       (20)     6247 2024-04-26 17:48:24.000000 openmindat-0.0.5/openmindat.egg-info/PKG-INFO
--rw-r--r--   0 blc        (501) staff       (20)      642 2024-04-26 17:48:24.000000 openmindat-0.0.5/openmindat.egg-info/SOURCES.txt
--rw-r--r--   0 blc        (501) staff       (20)        1 2024-04-26 17:48:24.000000 openmindat-0.0.5/openmindat.egg-info/dependency_links.txt
--rw-r--r--   0 blc        (501) staff       (20)        1 2024-03-09 23:51:57.000000 openmindat-0.0.5/openmindat.egg-info/not-zip-safe
--rw-r--r--   0 blc        (501) staff       (20)       21 2024-04-26 17:48:24.000000 openmindat-0.0.5/openmindat.egg-info/requires.txt
--rw-r--r--   0 blc        (501) staff       (20)       11 2024-04-26 17:48:24.000000 openmindat-0.0.5/openmindat.egg-info/top_level.txt
--rw-r--r--   0 blc        (501) staff       (20)       38 2024-04-26 17:48:24.532572 openmindat-0.0.5/setup.cfg
--rw-r--r--   0 blc        (501) staff       (20)     1076 2024-04-26 17:38:02.000000 openmindat-0.0.5/setup.py
+drwxr-xr-x   0 blc        (501) staff       (20)        0 2024-04-26 17:56:52.531605 openmindat-0.0.6/
+-rw-r--r--   0 blc        (501) staff       (20)    11357 2023-09-28 23:58:40.000000 openmindat-0.0.6/LICENSE
+-rw-r--r--   0 blc        (501) staff       (20)      136 2024-04-09 06:30:41.000000 openmindat-0.0.6/MANIFEST.in
+-rw-r--r--   0 blc        (501) staff       (20)     6344 2024-04-26 17:56:52.531372 openmindat-0.0.6/PKG-INFO
+-rw-r--r--   0 blc        (501) staff       (20)     5843 2024-04-26 17:56:02.000000 openmindat-0.0.6/README.md
+drwxr-xr-x   0 blc        (501) staff       (20)        0 2024-04-26 17:56:52.529703 openmindat-0.0.6/openmindat/
+-rw-r--r--   0 blc        (501) staff       (20)     6087 2024-04-25 18:17:20.000000 openmindat-0.0.6/openmindat/__init__.py
+-rw-r--r--   0 blc        (501) staff       (20)     8203 2024-04-26 17:53:48.000000 openmindat-0.0.6/openmindat/countries.py
+-rw-r--r--   0 blc        (501) staff       (20)     5656 2024-04-26 17:35:31.000000 openmindat-0.0.6/openmindat/dana8.py
+-rw-r--r--   0 blc        (501) staff       (20)    47522 2024-04-26 17:35:31.000000 openmindat-0.0.6/openmindat/geomaterials.py
+-rw-r--r--   0 blc        (501) staff       (20)     4207 2024-04-26 17:35:31.000000 openmindat-0.0.6/openmindat/geomaterials_search.py
+-rw-r--r--   0 blc        (501) staff       (20)    20573 2024-04-26 17:35:31.000000 openmindat-0.0.6/openmindat/localities.py
+-rw-r--r--   0 blc        (501) staff       (20)     8378 2024-04-26 17:35:31.000000 openmindat-0.0.6/openmindat/localities_age.py
+-rw-r--r--   0 blc        (501) staff       (20)     8578 2024-04-26 17:35:31.000000 openmindat-0.0.6/openmindat/localities_status.py
+-rw-r--r--   0 blc        (501) staff       (20)     8535 2024-04-26 17:35:31.000000 openmindat-0.0.6/openmindat/localities_type.py
+-rw-r--r--   0 blc        (501) staff       (20)     4215 2024-04-26 17:35:31.000000 openmindat-0.0.6/openmindat/locgeoregion2.py
+-rw-r--r--   0 blc        (501) staff       (20)     3775 2024-04-26 17:35:31.000000 openmindat-0.0.6/openmindat/locobject.py
+-rw-r--r--   0 blc        (501) staff       (20)     9166 2024-04-25 17:55:43.000000 openmindat-0.0.6/openmindat/mindat_api.py
+-rw-r--r--   0 blc        (501) staff       (20)    13796 2024-04-26 17:35:31.000000 openmindat-0.0.6/openmindat/minerals_ima.py
+-rw-r--r--   0 blc        (501) staff       (20)     6120 2024-04-26 17:35:31.000000 openmindat-0.0.6/openmindat/nickel_strunz.py
+-rw-r--r--   0 blc        (501) staff       (20)     3496 2024-04-26 17:35:31.000000 openmindat-0.0.6/openmindat/photo_count.py
+drwxr-xr-x   0 blc        (501) staff       (20)        0 2024-04-26 17:56:52.531109 openmindat-0.0.6/openmindat.egg-info/
+-rw-r--r--   0 blc        (501) staff       (20)     6344 2024-04-26 17:56:52.000000 openmindat-0.0.6/openmindat.egg-info/PKG-INFO
+-rw-r--r--   0 blc        (501) staff       (20)      642 2024-04-26 17:56:52.000000 openmindat-0.0.6/openmindat.egg-info/SOURCES.txt
+-rw-r--r--   0 blc        (501) staff       (20)        1 2024-04-26 17:56:52.000000 openmindat-0.0.6/openmindat.egg-info/dependency_links.txt
+-rw-r--r--   0 blc        (501) staff       (20)        1 2024-03-09 23:51:57.000000 openmindat-0.0.6/openmindat.egg-info/not-zip-safe
+-rw-r--r--   0 blc        (501) staff       (20)       21 2024-04-26 17:56:52.000000 openmindat-0.0.6/openmindat.egg-info/requires.txt
+-rw-r--r--   0 blc        (501) staff       (20)       11 2024-04-26 17:56:52.000000 openmindat-0.0.6/openmindat.egg-info/top_level.txt
+-rw-r--r--   0 blc        (501) staff       (20)       38 2024-04-26 17:56:52.531663 openmindat-0.0.6/setup.cfg
+-rw-r--r--   0 blc        (501) staff       (20)     1076 2024-04-26 17:54:37.000000 openmindat-0.0.6/setup.py
```

### Comparing `openmindat-0.0.5/LICENSE` & `openmindat-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openmindat-0.0.5/PKG-INFO` & `openmindat-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmindat
-Version: 0.0.5
+Version: 0.0.6
 Summary: An alpha version for OpenMindat package
 Home-page: https://github.com/ChuBL/OpenMindat
 Author: Jiyin Zhang
 Author-email: jiyinz@uidaho.edu
 License: Apache Software License
 Keywords: mindat openmindat mineral data python api
 Classifier: Development Status :: 3 - Alpha
@@ -177,14 +177,19 @@
         <img src="https://github.com/ChuBL/OpenMindat/blob/main/Logo/NSF_Official_logo_Low_Res.png?raw=true"  width="10%">
 </p>
 
 - This work is supported by NSF, Award #2126315.
 
 ## Upgrading Logs
 
+### 0.0.6
+**Released:** Apr 26, 2024
+
+- Revised a neglected get function for country endpoints.
+
 ### 0.0.5
 **Released:** Apr 26, 2024
 
 - The `Internal Server Error` issue in v0.0.4 is fixed from the server side.
 - The get functions are now changed to `get_dict`.
 - Added progress bars for multiple-page queries.
 - Some other minor updates.
```

### Comparing `openmindat-0.0.5/README.md` & `openmindat-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,19 @@
         <img src="https://github.com/ChuBL/OpenMindat/blob/main/Logo/NSF_Official_logo_Low_Res.png?raw=true"  width="10%">
 </p>
 
 - This work is supported by NSF, Award #2126315.
 
 ## Upgrading Logs
 
+### 0.0.6
+**Released:** Apr 26, 2024
+
+- Revised a neglected get function for country endpoints.
+
 ### 0.0.5
 **Released:** Apr 26, 2024
 
 - The `Internal Server Error` issue in v0.0.4 is fixed from the server side.
 - The get functions are now changed to `get_dict`.
 - Added progress bars for multiple-page queries.
 - Some other minor updates.
```

### Comparing `openmindat-0.0.5/openmindat/__init__.py` & `openmindat-0.0.6/openmindat/__init__.py`

 * *Files identical despite different names*

### Comparing `openmindat-0.0.5/openmindat/countries.py` & `openmindat-0.0.6/openmindat/countries.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,39 +117,35 @@
                 >>> cr = CountriesListRetriever()
                 >>> cr.page(2).save()
         '''
         file_name = FILE_NAME
         
         self.saveto('', file_name)
         
-    def get_list(self):
+    def get_dict(self):
         '''
         Executes the query to retrieve the country data as a dictionary.
 
         Returns:
             list of dictionaries.
 
         Example:
             >>> cr = CountriesListRetriever()
-            >>> france = cr.page(2).get_list()
+            >>> france = cr.page(2).get_dict()
 
         '''
        
         params = self._params
         end_point = self.end_point
         
         ma = mindat_api.MindatApi()        
         #clears params for next get statement     
 
-        if "page" in params:
-            results = [ma.get_mindat_json(params, end_point)]
-        else:
-            results = ma.get_mindat_json(params, end_point)
-        
-        
+        results = ma.get_mindat_json(params, end_point)
+           
         self._init_params()
         return results
             
             
         
 
 class CountriesIdRetriever:
@@ -271,32 +267,32 @@
                 >>> cidr = countriesIdRetriever()
                 >>> cidr.id(2).save()
         '''
         file_name = FILE_NAME
         
         self.saveto('', file_name)
         
-    def get_list(self):
+    def get_dict(self):
         '''
         Executes the query to retrieve the country data as a dictionary.
 
         Returns:
             list of dictionaries.
 
         Example:
             >>> cidr = countriesIdRetriever()
-            >>> france = cidr.id(2).get_liat()
+            >>> france = cidr.id(2).get_dict()
 
         '''
        
         params = self._params
         end_point = self.end_point    
         
         ma = mindat_api.MindatApi()
-        results = [ma.get_mindat_json(params, end_point)]
+        results = ma.get_mindat_json(params, end_point)
         
         self._init_params()
         return results
 
 if __name__ == '__main__':
     cidr = CountriesIdRetriever()
     cidr.id(2).save()
```

### Comparing `openmindat-0.0.5/openmindat/dana8.py` & `openmindat-0.0.6/openmindat/dana8.py`

 * *Files identical despite different names*

### Comparing `openmindat-0.0.5/openmindat/geomaterials.py` & `openmindat-0.0.6/openmindat/geomaterials.py`

 * *Files identical despite different names*

### Comparing `openmindat-0.0.5/openmindat/geomaterials_search.py` & `openmindat-0.0.6/openmindat/geomaterials_search.py`

 * *Files identical despite different names*

### Comparing `openmindat-0.0.5/openmindat/localities.py` & `openmindat-0.0.6/openmindat/localities.py`

 * *Files identical despite different names*

### Comparing `openmindat-0.0.5/openmindat/localities_age.py` & `openmindat-0.0.6/openmindat/localities_age.py`

 * *Files identical despite different names*

### Comparing `openmindat-0.0.5/openmindat/localities_status.py` & `openmindat-0.0.6/openmindat/localities_status.py`

 * *Files identical despite different names*

### Comparing `openmindat-0.0.5/openmindat/localities_type.py` & `openmindat-0.0.6/openmindat/localities_type.py`

 * *Files identical despite different names*

### Comparing `openmindat-0.0.5/openmindat/locgeoregion2.py` & `openmindat-0.0.6/openmindat/locgeoregion2.py`

 * *Files identical despite different names*

### Comparing `openmindat-0.0.5/openmindat/locobject.py` & `openmindat-0.0.6/openmindat/locobject.py`

 * *Files identical despite different names*

### Comparing `openmindat-0.0.5/openmindat/mindat_api.py` & `openmindat-0.0.6/openmindat/mindat_api.py`

 * *Files identical despite different names*

### Comparing `openmindat-0.0.5/openmindat/minerals_ima.py` & `openmindat-0.0.6/openmindat/minerals_ima.py`

 * *Files identical despite different names*

### Comparing `openmindat-0.0.5/openmindat/nickel_strunz.py` & `openmindat-0.0.6/openmindat/nickel_strunz.py`

 * *Files identical despite different names*

### Comparing `openmindat-0.0.5/openmindat/photo_count.py` & `openmindat-0.0.6/openmindat/photo_count.py`

 * *Files identical despite different names*

### Comparing `openmindat-0.0.5/openmindat.egg-info/PKG-INFO` & `openmindat-0.0.6/openmindat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmindat
-Version: 0.0.5
+Version: 0.0.6
 Summary: An alpha version for OpenMindat package
 Home-page: https://github.com/ChuBL/OpenMindat
 Author: Jiyin Zhang
 Author-email: jiyinz@uidaho.edu
 License: Apache Software License
 Keywords: mindat openmindat mineral data python api
 Classifier: Development Status :: 3 - Alpha
@@ -177,14 +177,19 @@
         <img src="https://github.com/ChuBL/OpenMindat/blob/main/Logo/NSF_Official_logo_Low_Res.png?raw=true"  width="10%">
 </p>
 
 - This work is supported by NSF, Award #2126315.
 
 ## Upgrading Logs
 
+### 0.0.6
+**Released:** Apr 26, 2024
+
+- Revised a neglected get function for country endpoints.
+
 ### 0.0.5
 **Released:** Apr 26, 2024
 
 - The `Internal Server Error` issue in v0.0.4 is fixed from the server side.
 - The get functions are now changed to `get_dict`.
 - Added progress bars for multiple-page queries.
 - Some other minor updates.
```

### Comparing `openmindat-0.0.5/openmindat.egg-info/SOURCES.txt` & `openmindat-0.0.6/openmindat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openmindat-0.0.5/setup.py` & `openmindat-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(name='openmindat',
-      version='0.0.5',
+      version='0.0.6',
       description='An alpha version for OpenMindat package',
       long_description=open('README.md').read(),
       long_description_content_type='text/markdown',
       classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: Apache Software License',
         "Programming Language :: Python :: 3",
```

