# Comparing `tmp/FrustrationDynamiX-0.2.6.tar.gz` & `tmp/FrustrationDynamiX-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FrustrationDynamiX-0.2.6.tar", last modified: Sat Apr 27 19:02:05 2024, max compression
+gzip compressed data, was "FrustrationDynamiX-0.2.7.tar", last modified: Sat Apr 27 19:07:04 2024, max compression
```

## Comparing `FrustrationDynamiX-0.2.6.tar` & `FrustrationDynamiX-0.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 19:02:05.730994 FrustrationDynamiX-0.2.6/
-drwxrwxrwx   0        0        0        0 2024-04-27 19:02:05.700834 FrustrationDynamiX-0.2.6/FrustrationDynamiX/
--rw-rw-rw-   0        0        0       36 2024-04-19 23:23:05.000000 FrustrationDynamiX-0.2.6/FrustrationDynamiX/__init__.py
--rw-rw-rw-   0        0        0    25668 2024-04-27 19:01:54.000000 FrustrationDynamiX-0.2.6/FrustrationDynamiX/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:02:05.728431 FrustrationDynamiX-0.2.6/FrustrationDynamiX.egg-info/
--rw-rw-rw-   0        0        0     1370 2024-04-27 19:02:05.000000 FrustrationDynamiX-0.2.6/FrustrationDynamiX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2024-04-27 19:02:05.000000 FrustrationDynamiX-0.2.6/FrustrationDynamiX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 19:02:05.000000 FrustrationDynamiX-0.2.6/FrustrationDynamiX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-04-27 19:02:05.000000 FrustrationDynamiX-0.2.6/FrustrationDynamiX.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-27 19:02:05.000000 FrustrationDynamiX-0.2.6/FrustrationDynamiX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1094 2024-04-20 20:30:54.000000 FrustrationDynamiX-0.2.6/LICENSE
--rw-rw-rw-   0        0        0     1370 2024-04-27 19:02:05.730994 FrustrationDynamiX-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      600 2024-04-20 20:05:17.000000 FrustrationDynamiX-0.2.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 19:02:05.732007 FrustrationDynamiX-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1125 2024-04-27 19:02:03.000000 FrustrationDynamiX-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:07:04.040248 FrustrationDynamiX-0.2.7/
+drwxrwxrwx   0        0        0        0 2024-04-27 19:07:04.010253 FrustrationDynamiX-0.2.7/FrustrationDynamiX/
+-rw-rw-rw-   0        0        0       36 2024-04-19 23:23:05.000000 FrustrationDynamiX-0.2.7/FrustrationDynamiX/__init__.py
+-rw-rw-rw-   0        0        0    25696 2024-04-27 19:06:52.000000 FrustrationDynamiX-0.2.7/FrustrationDynamiX/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:07:04.037252 FrustrationDynamiX-0.2.7/FrustrationDynamiX.egg-info/
+-rw-rw-rw-   0        0        0     1370 2024-04-27 19:07:03.000000 FrustrationDynamiX-0.2.7/FrustrationDynamiX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-04-27 19:07:03.000000 FrustrationDynamiX-0.2.7/FrustrationDynamiX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 19:07:03.000000 FrustrationDynamiX-0.2.7/FrustrationDynamiX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-04-27 19:07:03.000000 FrustrationDynamiX-0.2.7/FrustrationDynamiX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-27 19:07:03.000000 FrustrationDynamiX-0.2.7/FrustrationDynamiX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1094 2024-04-20 20:30:54.000000 FrustrationDynamiX-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0     1370 2024-04-27 19:07:04.039250 FrustrationDynamiX-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      600 2024-04-20 20:05:17.000000 FrustrationDynamiX-0.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 19:07:04.040248 FrustrationDynamiX-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1125 2024-04-27 19:06:57.000000 FrustrationDynamiX-0.2.7/setup.py
```

### Comparing `FrustrationDynamiX-0.2.6/FrustrationDynamiX/core.py` & `FrustrationDynamiX-0.2.7/FrustrationDynamiX/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,15 @@
         if window_size == None:
             window_size = self.num_var + 2
         J = np.zeros((self.num_var,self.num_var,len(range(1,self.duration-window_size,window_size)))) #Define empty jacobian
         
         #Define the empty variables
         T_ind = 0
         time_vector = []
+        time_instants = []
         time_index = range(self.duration)
 
         #Loop over variables
         for t in tqdm(range(1,self.duration-window_size,window_size)):
             for u in range(self.num_var): #1 loop for each variable
                 result = pyEDM.SMap(dataFrame = self.time_series, lib = [t,t+window_size], pred = [t,t+window_size], 
                                     embedded = True, columns = self.dynamic_var, target = self.dynamic_var[u], showPlot= showPlot)
```

### Comparing `FrustrationDynamiX-0.2.6/FrustrationDynamiX.egg-info/PKG-INFO` & `FrustrationDynamiX-0.2.7/FrustrationDynamiX.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FrustrationDynamiX
-Version: 0.2.6
+Version: 0.2.7
 Summary: A package for handling computing frustration in dynamical systems
 Home-page: https://github.com/asb24repo/FrustrationDynamiX
 Author: Ali S. Badereddine
 Author-email: asb24@mail.aub.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `FrustrationDynamiX-0.2.6/LICENSE` & `FrustrationDynamiX-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `FrustrationDynamiX-0.2.6/PKG-INFO` & `FrustrationDynamiX-0.2.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FrustrationDynamiX
-Version: 0.2.6
+Version: 0.2.7
 Summary: A package for handling computing frustration in dynamical systems
 Home-page: https://github.com/asb24repo/FrustrationDynamiX
 Author: Ali S. Badereddine
 Author-email: asb24@mail.aub.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `FrustrationDynamiX-0.2.6/README.md` & `FrustrationDynamiX-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `FrustrationDynamiX-0.2.6/setup.py` & `FrustrationDynamiX-0.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FrustrationDynamiX',
-    version='0.2.6',
+    version='0.2.7',
     packages=find_packages(),
     description='A package for handling computing frustration in dynamical systems',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Ali S. Badereddine',
     author_email='asb24@mail.aub.edu',
     license='MIT',
```

