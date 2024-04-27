# Comparing `tmp/FrustrationDynamiX-0.2.4.tar.gz` & `tmp/FrustrationDynamiX-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FrustrationDynamiX-0.2.4.tar", last modified: Sat Apr 27 18:51:03 2024, max compression
+gzip compressed data, was "FrustrationDynamiX-0.2.5.tar", last modified: Sat Apr 27 18:59:05 2024, max compression
```

## Comparing `FrustrationDynamiX-0.2.4.tar` & `FrustrationDynamiX-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 18:51:03.116439 FrustrationDynamiX-0.2.4/
-drwxrwxrwx   0        0        0        0 2024-04-27 18:51:03.086192 FrustrationDynamiX-0.2.4/FrustrationDynamiX/
--rw-rw-rw-   0        0        0       36 2024-04-19 23:23:05.000000 FrustrationDynamiX-0.2.4/FrustrationDynamiX/__init__.py
--rw-rw-rw-   0        0        0    25681 2024-04-27 18:50:19.000000 FrustrationDynamiX-0.2.4/FrustrationDynamiX/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 18:51:03.114433 FrustrationDynamiX-0.2.4/FrustrationDynamiX.egg-info/
--rw-rw-rw-   0        0        0     1370 2024-04-27 18:51:02.000000 FrustrationDynamiX-0.2.4/FrustrationDynamiX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2024-04-27 18:51:03.000000 FrustrationDynamiX-0.2.4/FrustrationDynamiX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 18:51:02.000000 FrustrationDynamiX-0.2.4/FrustrationDynamiX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-04-27 18:51:02.000000 FrustrationDynamiX-0.2.4/FrustrationDynamiX.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-27 18:51:02.000000 FrustrationDynamiX-0.2.4/FrustrationDynamiX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1094 2024-04-20 20:30:54.000000 FrustrationDynamiX-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     1370 2024-04-27 18:51:03.116439 FrustrationDynamiX-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      600 2024-04-20 20:05:17.000000 FrustrationDynamiX-0.2.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 18:51:03.117661 FrustrationDynamiX-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1125 2024-04-27 18:50:41.000000 FrustrationDynamiX-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 18:59:05.702332 FrustrationDynamiX-0.2.5/
+drwxrwxrwx   0        0        0        0 2024-04-27 18:59:05.673335 FrustrationDynamiX-0.2.5/FrustrationDynamiX/
+-rw-rw-rw-   0        0        0       36 2024-04-19 23:23:05.000000 FrustrationDynamiX-0.2.5/FrustrationDynamiX/__init__.py
+-rw-rw-rw-   0        0        0    25680 2024-04-27 18:58:56.000000 FrustrationDynamiX-0.2.5/FrustrationDynamiX/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 18:59:05.700336 FrustrationDynamiX-0.2.5/FrustrationDynamiX.egg-info/
+-rw-rw-rw-   0        0        0     1370 2024-04-27 18:59:05.000000 FrustrationDynamiX-0.2.5/FrustrationDynamiX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-04-27 18:59:05.000000 FrustrationDynamiX-0.2.5/FrustrationDynamiX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 18:59:05.000000 FrustrationDynamiX-0.2.5/FrustrationDynamiX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-04-27 18:59:05.000000 FrustrationDynamiX-0.2.5/FrustrationDynamiX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-27 18:59:05.000000 FrustrationDynamiX-0.2.5/FrustrationDynamiX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1094 2024-04-20 20:30:54.000000 FrustrationDynamiX-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0     1370 2024-04-27 18:59:05.702332 FrustrationDynamiX-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      600 2024-04-20 20:05:17.000000 FrustrationDynamiX-0.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 18:59:05.703330 FrustrationDynamiX-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1125 2024-04-27 18:59:02.000000 FrustrationDynamiX-0.2.5/setup.py
```

### Comparing `FrustrationDynamiX-0.2.4/FrustrationDynamiX/core.py` & `FrustrationDynamiX-0.2.5/FrustrationDynamiX/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
         list_var = df.columns.to_list()
         self.time_series = df
         self.duration = len(df)
         self.num_var = len(list_var) - 1
         self.time_var = list_var[0]
         self.dynamic_var = list_var[1:]
         self.time = df[self.time_var]
-        self.time_index = range(duration)
         self.time_vector = None
         self.is_normalized = is_normalized
         self.triadic_balance = None
         self.balanced_triangles = None
         self.unbalanced_triangles = None
         self.edge_deletion = None
         self.frustration = None
@@ -116,15 +115,16 @@
                 var = result['coefficients'].columns[2:]
                 for v in range(len(var)):
                     if u != v:
                         J[u,v,T_ind] = result['coefficients'][var[v]][window_size//2]
                         
             #Update iterators
             T_ind += 1
-            time_instants += [self.time_index[t + window_size//2]]
+            time_index = range(self.duration)
+            time_instants += [time_index[t + window_size//2]]
             time_vector = self.time[time_instants]
 
         return np.nan_to_num(J), time_vector
    
     @staticmethod
     def saveas_coo(jacobian_matrix, path):
         """
```

### Comparing `FrustrationDynamiX-0.2.4/FrustrationDynamiX.egg-info/PKG-INFO` & `FrustrationDynamiX-0.2.5/FrustrationDynamiX.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FrustrationDynamiX
-Version: 0.2.4
+Version: 0.2.5
 Summary: A package for handling computing frustration in dynamical systems
 Home-page: https://github.com/asb24repo/FrustrationDynamiX
 Author: Ali S. Badereddine
 Author-email: asb24@mail.aub.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `FrustrationDynamiX-0.2.4/LICENSE` & `FrustrationDynamiX-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `FrustrationDynamiX-0.2.4/PKG-INFO` & `FrustrationDynamiX-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FrustrationDynamiX
-Version: 0.2.4
+Version: 0.2.5
 Summary: A package for handling computing frustration in dynamical systems
 Home-page: https://github.com/asb24repo/FrustrationDynamiX
 Author: Ali S. Badereddine
 Author-email: asb24@mail.aub.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `FrustrationDynamiX-0.2.4/README.md` & `FrustrationDynamiX-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `FrustrationDynamiX-0.2.4/setup.py` & `FrustrationDynamiX-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FrustrationDynamiX',
-    version='0.2.4',
+    version='0.2.5',
     packages=find_packages(),
     description='A package for handling computing frustration in dynamical systems',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Ali S. Badereddine',
     author_email='asb24@mail.aub.edu',
     license='MIT',
```

