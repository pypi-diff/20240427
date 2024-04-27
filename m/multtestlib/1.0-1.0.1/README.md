# Comparing `tmp/multtestlib-1.0.tar.gz` & `tmp/multtestlib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multtestlib-1.0.tar", last modified: Sat Mar  9 04:04:48 2024, max compression
+gzip compressed data, was "multtestlib-1.0.1.tar", last modified: Sat Apr 27 13:18:25 2024, max compression
```

## Comparing `multtestlib-1.0.tar` & `multtestlib-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-09 04:04:48.310932 multtestlib-1.0/
--rw-rw-rw-   0        0        0     1109 2024-03-09 02:18:20.000000 multtestlib-1.0/LICENSE
--rw-rw-rw-   0        0        0     4997 2024-03-09 04:04:48.307936 multtestlib-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3193 2024-03-09 02:36:45.000000 multtestlib-1.0/README.md
--rw-rw-rw-   0        0        0      569 2024-03-09 02:19:50.000000 multtestlib-1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-09 04:04:48.311932 multtestlib-1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-09 04:04:48.281314 multtestlib-1.0/src/
--rw-rw-rw-   0        0        0        2 2022-08-19 02:10:43.000000 multtestlib-1.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-09 04:04:48.304946 multtestlib-1.0/src/multtestlib.egg-info/
--rw-rw-rw-   0        0        0     4997 2024-03-09 04:04:48.000000 multtestlib-1.0/src/multtestlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2024-03-09 04:04:48.000000 multtestlib-1.0/src/multtestlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-09 04:04:48.000000 multtestlib-1.0/src/multtestlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-03-09 04:04:48.000000 multtestlib-1.0/src/multtestlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10480 2024-03-08 01:34:46.000000 multtestlib-1.0/src/multtestlib.py
+drwxrwxrwx   0        0        0        0 2024-04-27 13:18:25.278162 multtestlib-1.0.1/
+-rw-rw-rw-   0        0        0     1109 2024-03-09 02:18:20.000000 multtestlib-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     5353 2024-04-27 13:18:25.275142 multtestlib-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3557 2024-04-27 03:55:43.000000 multtestlib-1.0.1/README.md
+-rw-rw-rw-   0        0        0      564 2024-04-27 13:18:00.000000 multtestlib-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-27 13:18:25.278162 multtestlib-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-27 13:18:25.165164 multtestlib-1.0.1/src/
+-rw-rw-rw-   0        0        0        2 2022-08-19 02:10:43.000000 multtestlib-1.0.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 13:18:25.273139 multtestlib-1.0.1/src/multtestlib.egg-info/
+-rw-rw-rw-   0        0        0     5353 2024-04-27 13:18:25.000000 multtestlib-1.0.1/src/multtestlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2024-04-27 13:18:25.000000 multtestlib-1.0.1/src/multtestlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 13:18:25.000000 multtestlib-1.0.1/src/multtestlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-04-27 13:18:25.000000 multtestlib-1.0.1/src/multtestlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10482 2024-04-27 02:52:09.000000 multtestlib-1.0.1/src/multtestlib.py
```

### Comparing `multtestlib-1.0/LICENSE` & `multtestlib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `multtestlib-1.0/PKG-INFO` & `multtestlib-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: multtestlib
-Version: 1.0
-Summary: Multtestlib, a package developed for performing unit tests in Python using parallel processing.
-Author-email: Ricardo Alvarenga <alvarenga.r.ricardo@gmail.com>
+Version: 1.0.1
+Summary: Multtestlib, a package developed for performing unit tests in Python using multiprocessing.
+Author-email: Ricardo Alvarenga <ricardoalvarenga@ita.br>
 License: Copyright (c) 2022-2024 Ricardo Ribeiro de Alvarenga
         
          Permission is hereby granted, free of charge, to any person obtaining a copy
          of this software and associated documentation files (the "Software"), to deal
          in the Software without restriction, including without limitation the rights
          to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
          copies of the Software, and to permit persons to whom the Software is
@@ -18,27 +18,29 @@
          THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
          IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
          FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
          AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
          LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
          OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
          THE SOFTWARE.
-Project-URL: Homepage, https://github.com/alvarengaricardo/multtestlib
-Classifier: Programming Language :: Python :: 3
+Project-URL: homepage, https://github.com/alvarengaricardo/multtestlib
+Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# multtestlib: A package developed for performing unit tests in Python using parallel processing.
+# multtestlib: A package developed for performing unit tests in Python using multiprocessing.
 
-Multtestlib has been devised to aid Python testers in expediting their testing processes through non-distributed parallel processing. This approach allows customizable utilization of the computer's available processor cores, facilitating workload distribution and consequent reduction in the overall execution time of the test suite.
+Multtestlib has been devised to aid Python testers in expediting their testing processes through multiprocessing. This approach allows customizable utilization of the computer's available processor cores, facilitating workload distribution and consequent reduction in the overall execution time of the test suite.
 
 ---
+![GitHub release](https://img.shields.io/github/release/alvarengaricardo/multtestlib.svg) [![Python](https://img.shields.io/badge/Python-%3E%3D%203.7-blue.svg)](https://www.python.org/downloads/) [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) [![Downloads](https://pepy.tech/badge/multtestlib)](https://pepy.tech/project/multtestlib)
+---
 
 ## Installation
 
 Multtestlib is available on PyPi and can be installed using the pip command:
     
     pip install multtestlib
 
@@ -48,17 +50,17 @@
 
 Multtestlib requires Python 3.7 or later to run.
 
 ---
 
 ## Usage
 
-For parallel processing usage, the input parameters of the test functions and their respective expected values must be stored in lists. During the test processing, multtestlib will take care of distributing and managing the data contained in the lists - and functions - among the processor cores indicated in the test program.
+For multiprocessing usage, the input parameters of the test functions and their respective expected values must be stored in lists. During the test processing, multtestlib will take care of distributing and managing the data contained in the lists - and functions - among the processor cores indicated in the test program.
 
-Next, we will see an example of a unit test for the **myfunction(a, b)** being submitted for execution using parallel processing:
+Next, we will see an example of a unit test for the **myfunction(a, b)** being submitted for execution using multiprocessing:
 
     import multtestlib as mtl
     import functions
 
     def main():
         cpus = 8 # Specify the number of CPUs to be used.
         input_values1 = []
```

### Comparing `multtestlib-1.0/README.md` & `multtestlib-1.0.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-# multtestlib: A package developed for performing unit tests in Python using parallel processing.
+# multtestlib: A package developed for performing unit tests in Python using multiprocessing.
 
-Multtestlib has been devised to aid Python testers in expediting their testing processes through non-distributed parallel processing. This approach allows customizable utilization of the computer's available processor cores, facilitating workload distribution and consequent reduction in the overall execution time of the test suite.
+Multtestlib has been devised to aid Python testers in expediting their testing processes through multiprocessing. This approach allows customizable utilization of the computer's available processor cores, facilitating workload distribution and consequent reduction in the overall execution time of the test suite.
 
 ---
+![GitHub release](https://img.shields.io/github/release/alvarengaricardo/multtestlib.svg) [![Python](https://img.shields.io/badge/Python-%3E%3D%203.7-blue.svg)](https://www.python.org/downloads/) [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) [![Downloads](https://pepy.tech/badge/multtestlib)](https://pepy.tech/project/multtestlib)
+---
 
 ## Installation
 
 Multtestlib is available on PyPi and can be installed using the pip command:
     
     pip install multtestlib
 
@@ -16,17 +18,17 @@
 
 Multtestlib requires Python 3.7 or later to run.
 
 ---
 
 ## Usage
 
-For parallel processing usage, the input parameters of the test functions and their respective expected values must be stored in lists. During the test processing, multtestlib will take care of distributing and managing the data contained in the lists - and functions - among the processor cores indicated in the test program.
+For multiprocessing usage, the input parameters of the test functions and their respective expected values must be stored in lists. During the test processing, multtestlib will take care of distributing and managing the data contained in the lists - and functions - among the processor cores indicated in the test program.
 
-Next, we will see an example of a unit test for the **myfunction(a, b)** being submitted for execution using parallel processing:
+Next, we will see an example of a unit test for the **myfunction(a, b)** being submitted for execution using multiprocessing:
 
     import multtestlib as mtl
     import functions
 
     def main():
         cpus = 8 # Specify the number of CPUs to be used.
         input_values1 = []
@@ -76,8 +78,8 @@
 
  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
- THE SOFTWARE.
+ THE SOFTWARE.
```

### Comparing `multtestlib-1.0/pyproject.toml` & `multtestlib-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "multtestlib"
-version = "1.00"
+version = "1.0.1"
 authors = [
-  { name="Ricardo Alvarenga", email="alvarenga.r.ricardo@gmail.com" },
+  { name = "Ricardo Alvarenga", email = "ricardoalvarenga@ita.br" }
 ]
-description = "Multtestlib, a package developed for performing unit tests in Python using parallel processing."
+description = "Multtestlib, a package developed for performing unit tests in Python using multiprocessing."
 readme = "README.md"
-license = { file="LICENSE" }
+license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
     "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+    "Operating System :: OS Independent"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/alvarengaricardo/multtestlib"
+homepage = "https://github.com/alvarengaricardo/multtestlib"
```

### Comparing `multtestlib-1.0/src/multtestlib.egg-info/PKG-INFO` & `multtestlib-1.0.1/src/multtestlib.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: multtestlib
-Version: 1.0
-Summary: Multtestlib, a package developed for performing unit tests in Python using parallel processing.
-Author-email: Ricardo Alvarenga <alvarenga.r.ricardo@gmail.com>
+Version: 1.0.1
+Summary: Multtestlib, a package developed for performing unit tests in Python using multiprocessing.
+Author-email: Ricardo Alvarenga <ricardoalvarenga@ita.br>
 License: Copyright (c) 2022-2024 Ricardo Ribeiro de Alvarenga
         
          Permission is hereby granted, free of charge, to any person obtaining a copy
          of this software and associated documentation files (the "Software"), to deal
          in the Software without restriction, including without limitation the rights
          to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
          copies of the Software, and to permit persons to whom the Software is
@@ -18,27 +18,29 @@
          THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
          IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
          FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
          AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
          LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
          OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
          THE SOFTWARE.
-Project-URL: Homepage, https://github.com/alvarengaricardo/multtestlib
-Classifier: Programming Language :: Python :: 3
+Project-URL: homepage, https://github.com/alvarengaricardo/multtestlib
+Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# multtestlib: A package developed for performing unit tests in Python using parallel processing.
+# multtestlib: A package developed for performing unit tests in Python using multiprocessing.
 
-Multtestlib has been devised to aid Python testers in expediting their testing processes through non-distributed parallel processing. This approach allows customizable utilization of the computer's available processor cores, facilitating workload distribution and consequent reduction in the overall execution time of the test suite.
+Multtestlib has been devised to aid Python testers in expediting their testing processes through multiprocessing. This approach allows customizable utilization of the computer's available processor cores, facilitating workload distribution and consequent reduction in the overall execution time of the test suite.
 
 ---
+![GitHub release](https://img.shields.io/github/release/alvarengaricardo/multtestlib.svg) [![Python](https://img.shields.io/badge/Python-%3E%3D%203.7-blue.svg)](https://www.python.org/downloads/) [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) [![Downloads](https://pepy.tech/badge/multtestlib)](https://pepy.tech/project/multtestlib)
+---
 
 ## Installation
 
 Multtestlib is available on PyPi and can be installed using the pip command:
     
     pip install multtestlib
 
@@ -48,17 +50,17 @@
 
 Multtestlib requires Python 3.7 or later to run.
 
 ---
 
 ## Usage
 
-For parallel processing usage, the input parameters of the test functions and their respective expected values must be stored in lists. During the test processing, multtestlib will take care of distributing and managing the data contained in the lists - and functions - among the processor cores indicated in the test program.
+For multiprocessing usage, the input parameters of the test functions and their respective expected values must be stored in lists. During the test processing, multtestlib will take care of distributing and managing the data contained in the lists - and functions - among the processor cores indicated in the test program.
 
-Next, we will see an example of a unit test for the **myfunction(a, b)** being submitted for execution using parallel processing:
+Next, we will see an example of a unit test for the **myfunction(a, b)** being submitted for execution using multiprocessing:
 
     import multtestlib as mtl
     import functions
 
     def main():
         cpus = 8 # Specify the number of CPUs to be used.
         input_values1 = []
```

### Comparing `multtestlib-1.0/src/multtestlib.py` & `multtestlib-1.0.1/src/multtestlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 '''
-    multtestlib 1.0
+    multtestlib 1.01
     Python package for running unit tests in parallel processing.
     By Ricardo Ribeiro de Alvarenga
        alvarenga.r.ricardo@gmail.com
 
     ITA - Instituto Tecnológico de Aeronáutica - Brasil
           Aeronautics Institute of Thecnology  - Brazil
     
 
-    March 2024
+    April 2024
 
 '''
 
 from datetime import datetime
 import os
 from concurrent.futures import ThreadPoolExecutor
 
@@ -246,15 +246,15 @@
     print("")
     print("*** multtestLib *** ")
     print("")
     print(" Python package for running unit tests in parallel processing.")
     print(" Author: Ricardo Ribeiro de Alvarenga")
     print("         ITA - Instituto Tecnologico de Aeronáutica")
     print("         Brazil")
-    print(" Version: 1.0")
+    print(" Version: 1.01")
     print("")
 
 
 def help():
     print("")
     print("")
     print("-----------------------------------------------")
```

