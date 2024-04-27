# Comparing `tmp/mckinseysolvegame-0.8.4.tar.gz` & `tmp/mckinseysolvegame-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mckinseysolvegame-0.8.4.tar", last modified: Sat Apr 27 14:50:02 2024, max compression
+gzip compressed data, was "mckinseysolvegame-1.0.0.tar", last modified: Sat Apr 27 15:16:47 2024, max compression
```

## Comparing `mckinseysolvegame-0.8.4.tar` & `mckinseysolvegame-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:50:02.244541 mckinseysolvegame-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-04-27 14:50:02.244541 mckinseysolvegame-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14176 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:50:02.244541 mckinseysolvegame-0.8.4/mckinseysolvegame/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/mckinseysolvegame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/mckinseysolvegame/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:50:02.244541 mckinseysolvegame-0.8.4/mckinseysolvegame/domain/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/mckinseysolvegame/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/mckinseysolvegame/domain/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:50:02.244541 mckinseysolvegame-0.8.4/mckinseysolvegame/domain/services/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/mckinseysolvegame/domain/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/mckinseysolvegame/domain/services/optimization_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:50:02.244541 mckinseysolvegame-0.8.4/mckinseysolvegame/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/mckinseysolvegame/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/mckinseysolvegame/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    30532 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/mckinseysolvegame/tests/test_optimization_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:50:02.244541 mckinseysolvegame-0.8.4/mckinseysolvegame.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-04-27 14:50:02.000000 mckinseysolvegame-0.8.4/mckinseysolvegame.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-27 14:50:02.000000 mckinseysolvegame-0.8.4/mckinseysolvegame.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 14:50:02.000000 mckinseysolvegame-0.8.4/mckinseysolvegame.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-27 14:50:02.000000 mckinseysolvegame-0.8.4/mckinseysolvegame.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 14:50:02.000000 mckinseysolvegame-0.8.4/mckinseysolvegame.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-27 14:50:02.244541 mckinseysolvegame-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:16:47.345486 mckinseysolvegame-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    14975 2024-04-27 15:16:47.345486 mckinseysolvegame-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14091 2024-04-27 15:16:38.000000 mckinseysolvegame-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:16:47.341486 mckinseysolvegame-1.0.0/mckinseysolvegame/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-27 15:16:38.000000 mckinseysolvegame-1.0.0/mckinseysolvegame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 15:16:38.000000 mckinseysolvegame-1.0.0/mckinseysolvegame/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:16:47.341486 mckinseysolvegame-1.0.0/mckinseysolvegame/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-27 15:16:38.000000 mckinseysolvegame-1.0.0/mckinseysolvegame/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-27 15:16:38.000000 mckinseysolvegame-1.0.0/mckinseysolvegame/domain/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:16:47.341486 mckinseysolvegame-1.0.0/mckinseysolvegame/domain/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-27 15:16:38.000000 mckinseysolvegame-1.0.0/mckinseysolvegame/domain/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-27 15:16:38.000000 mckinseysolvegame-1.0.0/mckinseysolvegame/domain/services/optimization_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:16:47.345486 mckinseysolvegame-1.0.0/mckinseysolvegame/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 15:16:38.000000 mckinseysolvegame-1.0.0/mckinseysolvegame/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-04-27 15:16:38.000000 mckinseysolvegame-1.0.0/mckinseysolvegame/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30532 2024-04-27 15:16:38.000000 mckinseysolvegame-1.0.0/mckinseysolvegame/tests/test_optimization_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:16:47.345486 mckinseysolvegame-1.0.0/mckinseysolvegame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14975 2024-04-27 15:16:47.000000 mckinseysolvegame-1.0.0/mckinseysolvegame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-27 15:16:47.000000 mckinseysolvegame-1.0.0/mckinseysolvegame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 15:16:47.000000 mckinseysolvegame-1.0.0/mckinseysolvegame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-27 15:16:47.000000 mckinseysolvegame-1.0.0/mckinseysolvegame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 15:16:47.000000 mckinseysolvegame-1.0.0/mckinseysolvegame.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-27 15:16:38.000000 mckinseysolvegame-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-27 15:16:47.345486 mckinseysolvegame-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-27 15:16:38.000000 mckinseysolvegame-1.0.0/setup.py
```

### Comparing `mckinseysolvegame-0.8.4/PKG-INFO` & `mckinseysolvegame-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mckinseysolvegame
-Version: 0.8.4
+Version: 1.0.0
 Summary: Python library for solving the McKinsey Solve Game
 Home-page: https://github.com/SebastienEveno/mckinseysolvegame
 Author: Sebastien Eveno
 Author-email: sebastien.louis.eveno@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -420,10 +420,7 @@
 We welcome contributions to mckinseysolvegame! If you find a bug or would like to request a new feature, please open an issue on
 the [Github repository](https://github.com/sebastieneveno/mckinseysolvegame).
 If you would like to contribute code, please submit a pull request.
 
 ## License
 
 mckinseysolvegame is released under the [MIT License](https://opensource.org/licenses/MIT).
-
-## To Do List
-- Consider the case eating half of calories provided in case of a tie
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mckinseysolvegame Version: 0.8.4 Summary: Python
+Metadata-Version: 2.1 Name: mckinseysolvegame Version: 1.0.0 Summary: Python
 library for solving the McKinsey Solve Game Home-page: https://github.com/
 SebastienEveno/mckinseysolvegame Author: Sebastien Eveno Author-email:
 sebastien.louis.eveno@gmail.com License: MIT Classifier: Development Status ::
 4 - Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Science/Research Classifier: Topic :: Software Development Classifier: Topic ::
@@ -138,9 +138,8 @@
 Snapper", "Eyestripe Surgeonfish" ] } ``` This object contains the maximum
 number of species that can sustain, as well as the list of species names. ##
 Contributing We welcome contributions to mckinseysolvegame! If you find a bug
 or would like to request a new feature, please open an issue on the [Github
 repository](https://github.com/sebastieneveno/mckinseysolvegame). If you would
 like to contribute code, please submit a pull request. ## License
 mckinseysolvegame is released under the [MIT License](https://opensource.org/
-licenses/MIT). ## To Do List - Consider the case eating half of calories
-provided in case of a tie
+licenses/MIT).
```

### Comparing `mckinseysolvegame-0.8.4/README.md` & `mckinseysolvegame-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -396,10 +396,7 @@
 We welcome contributions to mckinseysolvegame! If you find a bug or would like to request a new feature, please open an issue on
 the [Github repository](https://github.com/sebastieneveno/mckinseysolvegame).
 If you would like to contribute code, please submit a pull request.
 
 ## License
 
 mckinseysolvegame is released under the [MIT License](https://opensource.org/licenses/MIT).
-
-## To Do List
-- Consider the case eating half of calories provided in case of a tie
```

#### html2text {}

```diff
@@ -127,9 +127,8 @@
 Snapper", "Eyestripe Surgeonfish" ] } ``` This object contains the maximum
 number of species that can sustain, as well as the list of species names. ##
 Contributing We welcome contributions to mckinseysolvegame! If you find a bug
 or would like to request a new feature, please open an issue on the [Github
 repository](https://github.com/sebastieneveno/mckinseysolvegame). If you would
 like to contribute code, please submit a pull request. ## License
 mckinseysolvegame is released under the [MIT License](https://opensource.org/
-licenses/MIT). ## To Do List - Consider the case eating half of calories
-provided in case of a tie
+licenses/MIT).
```

### Comparing `mckinseysolvegame-0.8.4/mckinseysolvegame/domain/models.py` & `mckinseysolvegame-1.0.0/mckinseysolvegame/domain/models.py`

 * *Files identical despite different names*

### Comparing `mckinseysolvegame-0.8.4/mckinseysolvegame/domain/services/optimization_service.py` & `mckinseysolvegame-1.0.0/mckinseysolvegame/domain/services/optimization_service.py`

 * *Files identical despite different names*

### Comparing `mckinseysolvegame-0.8.4/mckinseysolvegame/tests/test_models.py` & `mckinseysolvegame-1.0.0/mckinseysolvegame/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `mckinseysolvegame-0.8.4/mckinseysolvegame/tests/test_optimization_service.py` & `mckinseysolvegame-1.0.0/mckinseysolvegame/tests/test_optimization_service.py`

 * *Files identical despite different names*

### Comparing `mckinseysolvegame-0.8.4/mckinseysolvegame.egg-info/PKG-INFO` & `mckinseysolvegame-1.0.0/mckinseysolvegame.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mckinseysolvegame
-Version: 0.8.4
+Version: 1.0.0
 Summary: Python library for solving the McKinsey Solve Game
 Home-page: https://github.com/SebastienEveno/mckinseysolvegame
 Author: Sebastien Eveno
 Author-email: sebastien.louis.eveno@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -420,10 +420,7 @@
 We welcome contributions to mckinseysolvegame! If you find a bug or would like to request a new feature, please open an issue on
 the [Github repository](https://github.com/sebastieneveno/mckinseysolvegame).
 If you would like to contribute code, please submit a pull request.
 
 ## License
 
 mckinseysolvegame is released under the [MIT License](https://opensource.org/licenses/MIT).
-
-## To Do List
-- Consider the case eating half of calories provided in case of a tie
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mckinseysolvegame Version: 0.8.4 Summary: Python
+Metadata-Version: 2.1 Name: mckinseysolvegame Version: 1.0.0 Summary: Python
 library for solving the McKinsey Solve Game Home-page: https://github.com/
 SebastienEveno/mckinseysolvegame Author: Sebastien Eveno Author-email:
 sebastien.louis.eveno@gmail.com License: MIT Classifier: Development Status ::
 4 - Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Science/Research Classifier: Topic :: Software Development Classifier: Topic ::
@@ -138,9 +138,8 @@
 Snapper", "Eyestripe Surgeonfish" ] } ``` This object contains the maximum
 number of species that can sustain, as well as the list of species names. ##
 Contributing We welcome contributions to mckinseysolvegame! If you find a bug
 or would like to request a new feature, please open an issue on the [Github
 repository](https://github.com/sebastieneveno/mckinseysolvegame). If you would
 like to contribute code, please submit a pull request. ## License
 mckinseysolvegame is released under the [MIT License](https://opensource.org/
-licenses/MIT). ## To Do List - Consider the case eating half of calories
-provided in case of a tie
+licenses/MIT).
```

### Comparing `mckinseysolvegame-0.8.4/mckinseysolvegame.egg-info/SOURCES.txt` & `mckinseysolvegame-1.0.0/mckinseysolvegame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mckinseysolvegame-0.8.4/setup.py` & `mckinseysolvegame-1.0.0/setup.py`

 * *Files identical despite different names*

