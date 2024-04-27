# Comparing `tmp/psyaitools-0.1.5.tar.gz` & `tmp/psyaitools-0.1.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyaitools-0.1.5.tar", max compression
+gzip compressed data, was "psyaitools-0.1.6.dev1.tar", max compression
```

## Comparing `psyaitools-0.1.5.tar` & `psyaitools-0.1.6.dev1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0    35149 2024-04-19 18:30:19.184238 psyaitools-0.1.5/LICENSE
--rw-r--r--   0        0        0      928 2024-04-26 16:26:27.686146 psyaitools-0.1.5/README.md
--rw-r--r--   0        0        0     6148 2024-04-26 16:27:46.412536 psyaitools-0.1.5/psyaitools/.DS_Store
--rw-r--r--   0        0        0        0 2024-04-26 17:38:19.164142 psyaitools-0.1.5/psyaitools/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 09:29:19.590033 psyaitools-0.1.5/psyaitools/functional/IOs/__init__.py
--rw-r--r--   0        0        0     1775 2024-04-26 19:25:04.361766 psyaitools-0.1.5/psyaitools/functional/IOs/base64_wav.py
--rw-r--r--   0        0        0      685 2024-04-26 19:30:17.067431 psyaitools-0.1.5/psyaitools/functional/IOs/base64_xfccs.py
--rw-r--r--   0        0        0      218 2024-04-26 19:09:46.876182 psyaitools-0.1.5/psyaitools/functional/IOs/readFiles.py
--rw-r--r--   0        0        0        0 2024-04-26 17:36:54.161932 psyaitools-0.1.5/psyaitools/functional/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 17:37:47.798436 psyaitools-0.1.5/psyaitools/functional/ext/__init__.py
--rw-r--r--   0        0        0      997 2024-04-26 15:06:50.275222 psyaitools-0.1.5/psyaitools/functional/ext/shInst.py
--rw-r--r--   0        0        0        0 2024-04-26 17:37:24.367135 psyaitools-0.1.5/psyaitools/functional/representation/__init__.py
--rw-r--r--   0        0        0     1527 2024-04-26 16:28:20.020756 psyaitools-0.1.5/psyaitools/functional/representation/factDecomMachine.py
--rw-r--r--   0        0        0     1075 2024-04-26 17:47:56.028505 psyaitools-0.1.5/psyaitools/functional/representation/xfccs.py
--rw-r--r--   0        0        0       23 2024-04-19 18:36:31.305642 psyaitools-0.1.5/psyaitools/res/res.py
--rw-r--r--   0        0        0      432 2024-04-26 19:35:19.792319 psyaitools-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1573 1970-01-01 00:00:00.000000 psyaitools-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-19 18:30:19.184238 psyaitools-0.1.6.dev1/LICENSE
+-rw-r--r--   0        0        0      989 2024-04-27 10:16:07.785454 psyaitools-0.1.6.dev1/README.md
+-rw-r--r--   0        0        0     6148 2024-04-26 16:27:46.412536 psyaitools-0.1.6.dev1/psyaitools/.DS_Store
+-rw-r--r--   0        0        0        0 2024-04-26 17:38:19.164142 psyaitools-0.1.6.dev1/psyaitools/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:29:19.590033 psyaitools-0.1.6.dev1/psyaitools/func/IOs/__init__.py
+-rw-r--r--   0        0        0     1775 2024-04-26 19:25:04.361766 psyaitools-0.1.6.dev1/psyaitools/func/IOs/base64_wav.py
+-rw-r--r--   0        0        0      800 2024-04-27 11:41:26.804950 psyaitools-0.1.6.dev1/psyaitools/func/IOs/base64_xfccs.py
+-rw-r--r--   0        0        0      218 2024-04-26 19:09:46.876182 psyaitools-0.1.6.dev1/psyaitools/func/IOs/readFiles.py
+-rw-r--r--   0        0        0        0 2024-04-26 17:36:54.161932 psyaitools-0.1.6.dev1/psyaitools/func/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 17:37:47.798436 psyaitools-0.1.6.dev1/psyaitools/func/ext/__init__.py
+-rw-r--r--   0        0        0      997 2024-04-26 15:06:50.275222 psyaitools-0.1.6.dev1/psyaitools/func/ext/shInst.py
+-rw-r--r--   0        0        0        0 2024-04-26 17:37:24.367135 psyaitools-0.1.6.dev1/psyaitools/func/representation/__init__.py
+-rw-r--r--   0        0        0     1527 2024-04-26 16:28:20.020756 psyaitools-0.1.6.dev1/psyaitools/func/representation/factDecomMachine.py
+-rw-r--r--   0        0        0      166 2024-04-27 11:40:12.032134 psyaitools-0.1.6.dev1/psyaitools/func/representation/loud.py
+-rw-r--r--   0        0        0     1908 2024-04-27 11:00:06.971921 psyaitools-0.1.6.dev1/psyaitools/func/representation/xfccs.py
+-rw-r--r--   0        0        0     1518 2024-04-27 10:13:40.867570 psyaitools-0.1.6.dev1/psyaitools/res/BSD_3_LICENSE_spafe
+-rw-r--r--   0        0        0       23 2024-04-19 18:36:31.305642 psyaitools-0.1.6.dev1/psyaitools/res/res.py
+-rw-r--r--   0        0        0      454 2024-04-27 11:43:53.909526 psyaitools-0.1.6.dev1/pyproject.toml
+-rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 psyaitools-0.1.6.dev1/PKG-INFO
```

### Comparing `psyaitools-0.1.5/LICENSE` & `psyaitools-0.1.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.5/README.md` & `psyaitools-0.1.6.dev1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-This package tries to build AI methods from the machine learning based brain function models (Domigos, 2012; Doya, 2000) and manifold distribution law (Tenenbaum et al., 2000; Lei et al., 2020). It plans to contain both object-oriented APIs and functional APIs. But this package is still under development. 
+This package tries to build AI methods from the machine learning based brain function models (Domigos, 2012; Doya, 2000) and manifold distribution law (Tenenbaum et al., 2000; Lei et al., 2020). It plans to contain both object-oriented APIs and functional APIs. This package is still under development. Original authors may contact the developer due to license issues.
 
 <b>References</b>
 - Domingos, P. (2012). A few useful things to know about machine learning. Communications of the ACM, 55(10), 78-87.
 - Doya, K. (2000). Complementary roles of basal ganglia and cerebellum in learning and motor control. Current opinion in neurobiology, 10(6), 732-739.
 - Lei, N., An, D., Guo, Y., Su, K., Liu, S., Luo, Z., ... & Gu, X. (2020). A geometric understanding of deep learning. Engineering, 6(3), 361-374.
 - Tenenbaum, J. B., Silva, V. D., & Langford, J. C. (2000). A global geometric framework for nonlinear dimensionality reduction. science, 290(5500), 2319-2323.
```

### Comparing `psyaitools-0.1.5/psyaitools/.DS_Store` & `psyaitools-0.1.6.dev1/psyaitools/.DS_Store`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.5/psyaitools/functional/IOs/base64_wav.py` & `psyaitools-0.1.6.dev1/psyaitools/func/IOs/base64_wav.py`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.5/psyaitools/functional/IOs/base64_xfccs.py` & `psyaitools-0.1.6.dev1/psyaitools/func/IOs/base64_xfccs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 # -*- coding: utf-8 -*-
 import numpy as np
 from .readFiles import *
 from .base64_wav import *
 from ..representation.xfccs import *
+from ..representation.loud import *
 
 def base64_xfccs(path, audioRow, fileName,feature_set="mfcc"):
     dat1 = getRecDat(path)
     base64ToWebm(dat1.loc[audioRow, "response"], fileName, method=2)
     webm2Wav(fileName)
     # Split the filename into name and extension
     nam1, _ = fileName.rsplit('.', 1)
     fs, sig = getWavDat(nam1 + ".wav")
     out1, _ = xfccs(fs, sig, feature_set=feature_set)
     return np.mean(out1, axis=1)
 
 def wav_xfccs(path, feature_set="mfcc"):
     fs, sig = getWavDat(path)
     out1, _ = xfccs(fs, sig, feature_set=feature_set)
-    return np.mean(out1, axis=1)
+    return np.mean(out1, axis=1)
+
+def getLoud(path):
+    fs, sig = getWavDat(path)
+    return loudness(sig, fs)
```

### Comparing `psyaitools-0.1.5/psyaitools/functional/ext/shInst.py` & `psyaitools-0.1.6.dev1/psyaitools/func/ext/shInst.py`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.5/psyaitools/functional/representation/factDecomMachine.py` & `psyaitools-0.1.6.dev1/psyaitools/func/representation/factDecomMachine.py`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.5/PKG-INFO` & `psyaitools-0.1.6.dev1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: psyaitools
-Version: 0.1.5
-Summary: Minor issues fixed
+Version: 0.1.6.dev1
+Summary: Loudness added.
 Author: moomoofarm1
 Author-email: 46774289+moomoofarm1@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: audioread (>=3.0,<4.0)
 Requires-Dist: numpy (>=1.24,<2.0)
 Requires-Dist: pandas (>=2.2,<3.0)
+Requires-Dist: pyloudnorm (>=0.1,<0.2)
 Requires-Dist: pyspark (>=3.5,<4.0)
 Requires-Dist: scipy (>=1.13,<2.0)
 Requires-Dist: spafe (>=0.3,<0.4)
 Description-Content-Type: text/markdown
 
-This package tries to build AI methods from the machine learning based brain function models (Domigos, 2012; Doya, 2000) and manifold distribution law (Tenenbaum et al., 2000; Lei et al., 2020). It plans to contain both object-oriented APIs and functional APIs. But this package is still under development. 
+This package tries to build AI methods from the machine learning based brain function models (Domigos, 2012; Doya, 2000) and manifold distribution law (Tenenbaum et al., 2000; Lei et al., 2020). It plans to contain both object-oriented APIs and functional APIs. This package is still under development. Original authors may contact the developer due to license issues.
 
 <b>References</b>
 - Domingos, P. (2012). A few useful things to know about machine learning. Communications of the ACM, 55(10), 78-87.
 - Doya, K. (2000). Complementary roles of basal ganglia and cerebellum in learning and motor control. Current opinion in neurobiology, 10(6), 732-739.
 - Lei, N., An, D., Guo, Y., Su, K., Liu, S., Luo, Z., ... & Gu, X. (2020). A geometric understanding of deep learning. Engineering, 6(3), 361-374.
 - Tenenbaum, J. B., Silva, V. D., & Langford, J. C. (2000). A global geometric framework for nonlinear dimensionality reduction. science, 290(5500), 2319-2323.
```

