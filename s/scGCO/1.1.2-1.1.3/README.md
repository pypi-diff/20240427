# Comparing `tmp/scGCO-1.1.2.tar.gz` & `tmp/scGCO-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scGCO-1.1.2.tar", last modified: Mon Sep  5 13:50:01 2022, max compression
+gzip compressed data, was "scGCO-1.1.3.tar", last modified: Sat Apr 27 11:01:52 2024, max compression
```

## Comparing `scGCO-1.1.2.tar` & `scGCO-1.1.3.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-09-05 13:50:01.526053 scGCO-1.1.2/
--rw-rw-rw-   0        0        0      214 2022-09-05 13:50:01.525054 scGCO-1.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-09-05 13:50:01.515082 scGCO-1.1.2/scGCO/
--rw-rw-rw-   0        0        0    26421 2021-12-28 14:16:10.000000 scGCO-1.1.2/scGCO/Calculate_dist.py
--rw-rw-rw-   0        0        0    14004 2021-12-28 14:16:10.000000 scGCO-1.1.2/scGCO/Clustering.py
--rw-rw-rw-   0        0        0     6219 2022-09-03 14:54:32.000000 scGCO-1.1.2/scGCO/GMM.py
--rw-rw-rw-   0        0        0    57659 2022-09-03 14:54:40.000000 scGCO-1.1.2/scGCO/Graph_cut.py
--rw-rw-rw-   0        0        0    15935 2021-12-28 14:16:10.000000 scGCO-1.1.2/scGCO/Preprocessing.py
--rw-rw-rw-   0        0        0    48741 2021-12-28 14:16:10.000000 scGCO-1.1.2/scGCO/Test_FPR.py
--rw-rw-rw-   0        0        0    30434 2021-12-28 14:16:10.000000 scGCO-1.1.2/scGCO/Visualization.py
--rw-rw-rw-   0        0        0      208 2021-12-28 14:16:10.000000 scGCO-1.1.2/scGCO/__init__.py
--rw-rw-rw-   0        0        0    25756 2022-09-05 13:48:14.000000 scGCO-1.1.2/scGCO/venn.py
-drwxrwxrwx   0        0        0        0 2022-09-05 13:50:01.524058 scGCO-1.1.2/scGCO.egg-info/
--rw-rw-rw-   0        0        0      214 2022-09-05 13:50:01.000000 scGCO-1.1.2/scGCO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2022-09-05 13:50:01.000000 scGCO-1.1.2/scGCO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-05 13:50:01.000000 scGCO-1.1.2/scGCO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      152 2022-09-05 13:50:01.000000 scGCO-1.1.2/scGCO.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-09-05 13:50:01.000000 scGCO-1.1.2/scGCO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-05 13:50:01.526053 scGCO-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      755 2022-09-03 14:57:50.000000 scGCO-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:01:52.396967 scGCO-1.1.3/
+-rw-rw-rw-   0        0        0      101 2024-04-27 09:17:30.000000 scGCO-1.1.3/AUTHORS
+-rw-rw-rw-   0        0        0     1111 2024-04-27 09:17:30.000000 scGCO-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0      267 2024-04-27 11:01:52.395968 scGCO-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6878 2024-04-27 10:10:08.000000 scGCO-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 11:01:52.380969 scGCO-1.1.3/scGCO/
+-rw-rw-rw-   0        0        0     6219 2022-09-03 14:54:32.000000 scGCO-1.1.3/scGCO/GMM.py
+-rw-rw-rw-   0        0        0    57679 2022-11-26 08:24:32.000000 scGCO-1.1.3/scGCO/Graph_cut.py
+-rw-rw-rw-   0        0        0    15935 2021-12-28 14:16:10.000000 scGCO-1.1.3/scGCO/Preprocessing.py
+-rw-rw-rw-   0        0        0    30434 2021-12-28 14:16:10.000000 scGCO-1.1.3/scGCO/Visualization.py
+-rw-rw-rw-   0        0        0      127 2024-04-27 08:50:04.000000 scGCO-1.1.3/scGCO/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:01:52.391967 scGCO-1.1.3/scGCO.egg-info/
+-rw-rw-rw-   0        0        0      267 2024-04-27 11:01:52.000000 scGCO-1.1.3/scGCO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-04-27 11:01:52.000000 scGCO-1.1.3/scGCO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 11:01:52.000000 scGCO-1.1.3/scGCO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      157 2024-04-27 11:01:52.000000 scGCO-1.1.3/scGCO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-27 11:01:52.000000 scGCO-1.1.3/scGCO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 11:01:52.396967 scGCO-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      767 2024-04-27 09:27:43.000000 scGCO-1.1.3/setup.py
```

### Comparing `scGCO-1.1.2/scGCO/GMM.py` & `scGCO-1.1.3/scGCO/GMM.py`

 * *Files identical despite different names*

### Comparing `scGCO-1.1.2/scGCO/Graph_cut.py` & `scGCO-1.1.3/scGCO/Graph_cut.py`

 * *Files 0% similar despite different names*

```diff
@@ -1217,15 +1217,15 @@
     
     :param points: count: shape (n,); gmm: gmm object; scale_factor: scalar
 
     :rtype: unary energy matrix.
     '''    
    
     labels_pred = np.zeros(count.shape[0])
-    if isinstance(thresholds, float):
+    if isinstance(thresholds, np.float32):
         labels_pred[np.where(count > thresholds)] = 1
         mid_points = np.zeros(1)
         temp_means = np.zeros(2)
         temp_covs = np.zeros(2)
     else:
         for i in np.arange(thresholds.shape[0]):
             labels_pred[np.where(count > thresholds[i])] = i + 1      
@@ -1272,15 +1272,15 @@
     
     :param points: count: shape (n,); gmm: gmm object; scale_factor: scalar
 
     :rtype: unary energy matrix.
     '''    
    
     labels_pred = np.zeros(count.shape[0])
-    if isinstance(thresholds, float):
+    if isinstance(thresholds, np.float32):
         labels_pred[np.where(count > thresholds)] = 1
         mid_points = np.zeros(1)
         temp_means = np.zeros(2)
     else:
         for i in np.arange(thresholds.shape[0]):
             labels_pred[np.where(count > thresholds[i])] = i + 1      
     
@@ -1306,15 +1306,15 @@
     Returns unary cost energy just use profile without exp.
     
     :param points: count: shape (n,); gmm: gmm object; scale_factor: scalar
 
     :rtype: unary energy matrix.
     '''    
     labels_pred = np.zeros(count.shape[0])
-    if isinstance(thresholds, float):
+    if isinstance(thresholds, np.float32):
         labels_pred[np.where(count > thresholds)] = 1       
     else:
         for i in np.arange(thresholds.shape[0]):
             labels_pred[np.where(count > thresholds[i])] = i + 1
 
     uniq, count = np.unique(labels_pred, return_counts = True)    
 
@@ -1338,15 +1338,15 @@
     :unary_scale_factor, scalar; smooth_factor, scalar; 
     :label_cost: scalar; algorithm='expansion'
     :rtype: label shape (n,); gmm object.
     '''
     count=exp
 #    thresholds = threshold_multiotsu(exp) #3D
     thresholds = threshold_otsu(count)  #2D
-    if isinstance(thresholds, float):
+    if isinstance(thresholds, np.float32):
         pair_size = 2
     else:
         pair_size = thresholds.shape[0] + 1
     smooth_factor = smooth_factor
     unary_scale_factor = unary_scale_factor
     label_cost = label_cost
     algorithm = algorithm
```

### Comparing `scGCO-1.1.2/scGCO/Preprocessing.py` & `scGCO-1.1.3/scGCO/Preprocessing.py`

 * *Files identical despite different names*

### Comparing `scGCO-1.1.2/scGCO/Visualization.py` & `scGCO-1.1.3/scGCO/Visualization.py`

 * *Files identical despite different names*

### Comparing `scGCO-1.1.2/setup.py` & `scGCO-1.1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 setup(
         name='scGCO',
-        version='1.1.2',
+        version='1.1.3',
         description='single-cell graph cuts optimization',
-        url='https://github.com/WangPeng-Lab/scGCO',
+        url='https://github.com/fengwanwan/scGCO',
         packages=find_packages(),
         include_package_data=True,
-        install_requires=['pandas','numpy','matplotlib','scipy','sklearn','seaborn','parmap','Cython','pygco',
+        install_requires=['pandas','numpy','matplotlib','scipy','scikit-learn','seaborn','parmap','Cython','pygco',
                         'tqdm','networkx','shapely','statsmodels','hdbscan','pillow','scikit-image','umap-learn','pysal==2.0.0'],
-        author='Peng Wang',
-        author_email='wangpeng@pb.ac.cn',
+        author='Wanwan Feng',
+        author_email='fengwanwan2023@gmail.com',
         license='MIT'
 
 )
 
 ## pip install numpy
 ## pip install pygco
 ## conda install -c conda-forge cython
```

