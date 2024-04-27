# Comparing `tmp/whatshow_toolbox-1.0.2.tar.gz` & `tmp/whatshow_toolbox-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatshow_toolbox-1.0.2.tar", last modified: Fri Apr 26 03:23:59 2024, max compression
+gzip compressed data, was "whatshow_toolbox-1.0.3.tar", last modified: Sat Apr 27 04:48:59 2024, max compression
```

## Comparing `whatshow_toolbox-1.0.2.tar` & `whatshow_toolbox-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 03:23:59.102356 whatshow_toolbox-1.0.2/
--rw-rw-rw-   0        0        0     2112 2024-04-26 03:23:59.099135 whatshow_toolbox-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2004 2024-04-26 03:23:58.000000 whatshow_toolbox-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-26 03:23:59.102356 whatshow_toolbox-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      403 2024-04-26 03:23:58.000000 whatshow_toolbox-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:23:59.084538 whatshow_toolbox-1.0.2/whatshow_toolbox/
--rw-rw-rw-   0        0        0    13054 2024-04-26 03:23:58.000000 whatshow_toolbox-1.0.2/whatshow_toolbox/MatlabFuncHelper.py
--rw-rw-rw-   0        0        0       46 2024-04-26 03:23:58.000000 whatshow_toolbox-1.0.2/whatshow_toolbox/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:23:59.098136 whatshow_toolbox-1.0.2/whatshow_toolbox.egg-info/
--rw-rw-rw-   0        0        0     2112 2024-04-26 03:23:58.000000 whatshow_toolbox-1.0.2/whatshow_toolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-04-26 03:23:59.000000 whatshow_toolbox-1.0.2/whatshow_toolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 03:23:58.000000 whatshow_toolbox-1.0.2/whatshow_toolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-26 03:23:58.000000 whatshow_toolbox-1.0.2/whatshow_toolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-26 03:23:58.000000 whatshow_toolbox-1.0.2/whatshow_toolbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 04:48:59.096970 whatshow_toolbox-1.0.3/
+-rw-rw-rw-   0        0        0     2112 2024-04-27 04:48:59.094970 whatshow_toolbox-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2004 2024-04-27 04:48:58.000000 whatshow_toolbox-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 04:48:59.096970 whatshow_toolbox-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      403 2024-04-27 04:48:58.000000 whatshow_toolbox-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 04:48:59.081436 whatshow_toolbox-1.0.3/whatshow_toolbox/
+-rw-rw-rw-   0        0        0    13043 2024-04-27 04:48:58.000000 whatshow_toolbox-1.0.3/whatshow_toolbox/MatlabFuncHelper.py
+-rw-rw-rw-   0        0        0       46 2024-04-27 04:48:58.000000 whatshow_toolbox-1.0.3/whatshow_toolbox/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 04:48:59.093992 whatshow_toolbox-1.0.3/whatshow_toolbox.egg-info/
+-rw-rw-rw-   0        0        0     2112 2024-04-27 04:48:58.000000 whatshow_toolbox-1.0.3/whatshow_toolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-04-27 04:48:59.000000 whatshow_toolbox-1.0.3/whatshow_toolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 04:48:58.000000 whatshow_toolbox-1.0.3/whatshow_toolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-27 04:48:58.000000 whatshow_toolbox-1.0.3/whatshow_toolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-27 04:48:58.000000 whatshow_toolbox-1.0.3/whatshow_toolbox.egg-info/top_level.txt
```

### Comparing `whatshow_toolbox-1.0.2/PKG-INFO` & `whatshow_toolbox-1.0.3/whatshow_toolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: whatshow_toolbox
-Version: 1.0.2
+Name: whatshow-toolbox
+Version: 1.0.3
 Description-Content-Type: text/markdown
 
 # Toolbox
-[![PyPi](https://img.shields.io/badge/PyPi-1.0.2-blue)](https://pypi.org/project/whatshow-toolbox/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.0.3-blue)](https://pypi.org/project/whatshow-toolbox/)
 
 
 This repositories offers a toolbox across platforms.
 ## How to use
 * MatlabFuncHelper: this class simulate all Matlab functions in python (batch is supported).
     * batch
         * setBatchSize(batch_size)
```

### Comparing `whatshow_toolbox-1.0.2/README.md` & `whatshow_toolbox-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Toolbox
-[![PyPi](https://img.shields.io/badge/PyPi-1.0.2-blue)](https://pypi.org/project/whatshow-toolbox/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.0.3-blue)](https://pypi.org/project/whatshow-toolbox/)
 
 
 This repositories offers a toolbox across platforms.
 ## How to use
 * MatlabFuncHelper: this class simulate all Matlab functions in python (batch is supported).
     * batch
         * setBatchSize(batch_size)
```

### Comparing `whatshow_toolbox-1.0.2/whatshow_toolbox/MatlabFuncHelper.py` & `whatshow_toolbox-1.0.3/whatshow_toolbox/MatlabFuncHelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,15 @@
     ###########################################################################
     # Batch
     def setBatchSize(self, batch_size):
         self.batch_size = batch_size;
     def getBatchSize(self):
         return self.batch_size;
     
-    ###########################################################################
-    # checkers
+    ###########################################################################   
     '''
     check input is a vector like [(batch_size), n],  [(batch_size), ..., n, 1] or [(batch_size), ..., 1, n] 
     '''
     def isvector(self, mat):
         mat = np.asarray(mat);
         if self.batch_size == self.BATCH_SIZE_NO:
             return mat.ndim == 1 or mat.ndim >= 2 and (mat.shape[-2] == 1 or mat.shape[-1] == 1);
@@ -140,15 +139,15 @@
     
     ###########################################################################
     # transformers
     '''
     remove redundant dimension except for the batch_size
     '''
     def squeeze(self, mat):
-        out = mat.squeeze();
+        out = np.squeeze(mat);
         if self.batch_size == 1 and mat.ndim > 0:
             out = np.expand_dims(out, 0);
         return out;
     
     '''
     reshape
     @in1:   1st dimension
```

### Comparing `whatshow_toolbox-1.0.2/whatshow_toolbox.egg-info/PKG-INFO` & `whatshow_toolbox-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: whatshow-toolbox
-Version: 1.0.2
+Name: whatshow_toolbox
+Version: 1.0.3
 Description-Content-Type: text/markdown
 
 # Toolbox
-[![PyPi](https://img.shields.io/badge/PyPi-1.0.2-blue)](https://pypi.org/project/whatshow-toolbox/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.0.3-blue)](https://pypi.org/project/whatshow-toolbox/)
 
 
 This repositories offers a toolbox across platforms.
 ## How to use
 * MatlabFuncHelper: this class simulate all Matlab functions in python (batch is supported).
     * batch
         * setBatchSize(batch_size)
```

