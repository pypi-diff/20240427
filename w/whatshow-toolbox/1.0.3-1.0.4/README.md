# Comparing `tmp/whatshow_toolbox-1.0.3.tar.gz` & `tmp/whatshow_toolbox-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatshow_toolbox-1.0.3.tar", last modified: Sat Apr 27 04:48:59 2024, max compression
+gzip compressed data, was "whatshow_toolbox-1.0.4.tar", last modified: Sat Apr 27 05:22:00 2024, max compression
```

## Comparing `whatshow_toolbox-1.0.3.tar` & `whatshow_toolbox-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 04:48:59.096970 whatshow_toolbox-1.0.3/
--rw-rw-rw-   0        0        0     2112 2024-04-27 04:48:59.094970 whatshow_toolbox-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2004 2024-04-27 04:48:58.000000 whatshow_toolbox-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 04:48:59.096970 whatshow_toolbox-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      403 2024-04-27 04:48:58.000000 whatshow_toolbox-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 04:48:59.081436 whatshow_toolbox-1.0.3/whatshow_toolbox/
--rw-rw-rw-   0        0        0    13043 2024-04-27 04:48:58.000000 whatshow_toolbox-1.0.3/whatshow_toolbox/MatlabFuncHelper.py
--rw-rw-rw-   0        0        0       46 2024-04-27 04:48:58.000000 whatshow_toolbox-1.0.3/whatshow_toolbox/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 04:48:59.093992 whatshow_toolbox-1.0.3/whatshow_toolbox.egg-info/
--rw-rw-rw-   0        0        0     2112 2024-04-27 04:48:58.000000 whatshow_toolbox-1.0.3/whatshow_toolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-04-27 04:48:59.000000 whatshow_toolbox-1.0.3/whatshow_toolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 04:48:58.000000 whatshow_toolbox-1.0.3/whatshow_toolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-27 04:48:58.000000 whatshow_toolbox-1.0.3/whatshow_toolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-27 04:48:58.000000 whatshow_toolbox-1.0.3/whatshow_toolbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 05:22:00.073376 whatshow_toolbox-1.0.4/
+-rw-rw-rw-   0        0        0     2112 2024-04-27 05:22:00.070325 whatshow_toolbox-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2004 2024-04-27 05:21:58.000000 whatshow_toolbox-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 05:22:00.073376 whatshow_toolbox-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      403 2024-04-27 05:21:58.000000 whatshow_toolbox-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 05:22:00.057347 whatshow_toolbox-1.0.4/whatshow_toolbox/
+-rw-rw-rw-   0        0        0    13043 2024-04-27 05:21:58.000000 whatshow_toolbox-1.0.4/whatshow_toolbox/MatlabFuncHelper.py
+-rw-rw-rw-   0        0        0       46 2024-04-27 05:21:58.000000 whatshow_toolbox-1.0.4/whatshow_toolbox/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 05:22:00.070325 whatshow_toolbox-1.0.4/whatshow_toolbox.egg-info/
+-rw-rw-rw-   0        0        0     2112 2024-04-27 05:21:59.000000 whatshow_toolbox-1.0.4/whatshow_toolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-04-27 05:21:59.000000 whatshow_toolbox-1.0.4/whatshow_toolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 05:21:59.000000 whatshow_toolbox-1.0.4/whatshow_toolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-27 05:21:59.000000 whatshow_toolbox-1.0.4/whatshow_toolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-27 05:21:59.000000 whatshow_toolbox-1.0.4/whatshow_toolbox.egg-info/top_level.txt
```

### Comparing `whatshow_toolbox-1.0.3/PKG-INFO` & `whatshow_toolbox-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: whatshow_toolbox
-Version: 1.0.3
+Version: 1.0.4
 Description-Content-Type: text/markdown
 
 # Toolbox
-[![PyPi](https://img.shields.io/badge/PyPi-1.0.3-blue)](https://pypi.org/project/whatshow-toolbox/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.0.4-blue)](https://pypi.org/project/whatshow-toolbox/)
 
 
 This repositories offers a toolbox across platforms.
 ## How to use
 * MatlabFuncHelper: this class simulate all Matlab functions in python (batch is supported).
     * batch
         * setBatchSize(batch_size)
```

### Comparing `whatshow_toolbox-1.0.3/README.md` & `whatshow_toolbox-1.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Toolbox
-[![PyPi](https://img.shields.io/badge/PyPi-1.0.3-blue)](https://pypi.org/project/whatshow-toolbox/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.0.4-blue)](https://pypi.org/project/whatshow-toolbox/)
 
 
 This repositories offers a toolbox across platforms.
 ## How to use
 * MatlabFuncHelper: this class simulate all Matlab functions in python (batch is supported).
     * batch
         * setBatchSize(batch_size)
```

### Comparing `whatshow_toolbox-1.0.3/whatshow_toolbox/MatlabFuncHelper.py` & `whatshow_toolbox-1.0.4/whatshow_toolbox/MatlabFuncHelper.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
                 end = end + 1;
         elif len(args) == 2:
             beg = in1;
             step = args[0];
             end = args[1];
             if order == 'F':
                 end = end + 1;
-        out = np.arange(beg, step, end);
+        out = np.arange(beg, end, step);
         if self.batch_size != self.BATCH_SIZE_NO:
             out = np.tile(out,(self.batch_size, 1));
         return out;
     
     '''
     generate random values from [0, 1) following a uniform distribution
     @in1:   1st dimension
```

### Comparing `whatshow_toolbox-1.0.3/whatshow_toolbox.egg-info/PKG-INFO` & `whatshow_toolbox-1.0.4/whatshow_toolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: whatshow-toolbox
-Version: 1.0.3
+Version: 1.0.4
 Description-Content-Type: text/markdown
 
 # Toolbox
-[![PyPi](https://img.shields.io/badge/PyPi-1.0.3-blue)](https://pypi.org/project/whatshow-toolbox/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.0.4-blue)](https://pypi.org/project/whatshow-toolbox/)
 
 
 This repositories offers a toolbox across platforms.
 ## How to use
 * MatlabFuncHelper: this class simulate all Matlab functions in python (batch is supported).
     * batch
         * setBatchSize(batch_size)
```

