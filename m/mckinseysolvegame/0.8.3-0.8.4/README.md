# Comparing `tmp/mckinseysolvegame-0.8.3.tar.gz` & `tmp/mckinseysolvegame-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mckinseysolvegame-0.8.3.tar", last modified: Sat Apr 27 14:44:26 2024, max compression
+gzip compressed data, was "mckinseysolvegame-0.8.4.tar", last modified: Sat Apr 27 14:50:02 2024, max compression
```

## Comparing `mckinseysolvegame-0.8.3.tar` & `mckinseysolvegame-0.8.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:44:26.248210 mckinseysolvegame-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)    15027 2024-04-27 14:44:26.248210 mckinseysolvegame-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14143 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:44:26.244210 mckinseysolvegame-0.8.3/mckinseysolvegame/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/mckinseysolvegame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/mckinseysolvegame/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:44:26.244210 mckinseysolvegame-0.8.3/mckinseysolvegame/domain/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/mckinseysolvegame/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/mckinseysolvegame/domain/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:44:26.244210 mckinseysolvegame-0.8.3/mckinseysolvegame/domain/services/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/mckinseysolvegame/domain/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/mckinseysolvegame/domain/services/optimization_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:44:26.248210 mckinseysolvegame-0.8.3/mckinseysolvegame/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/mckinseysolvegame/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/mckinseysolvegame/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    30532 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/mckinseysolvegame/tests/test_optimization_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:44:26.248210 mckinseysolvegame-0.8.3/mckinseysolvegame.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15027 2024-04-27 14:44:26.000000 mckinseysolvegame-0.8.3/mckinseysolvegame.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-27 14:44:26.000000 mckinseysolvegame-0.8.3/mckinseysolvegame.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 14:44:26.000000 mckinseysolvegame-0.8.3/mckinseysolvegame.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-27 14:44:26.000000 mckinseysolvegame-0.8.3/mckinseysolvegame.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 14:44:26.000000 mckinseysolvegame-0.8.3/mckinseysolvegame.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-27 14:44:26.248210 mckinseysolvegame-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:50:02.244541 mckinseysolvegame-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-04-27 14:50:02.244541 mckinseysolvegame-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14176 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:50:02.244541 mckinseysolvegame-0.8.4/mckinseysolvegame/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/mckinseysolvegame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/mckinseysolvegame/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:50:02.244541 mckinseysolvegame-0.8.4/mckinseysolvegame/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/mckinseysolvegame/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/mckinseysolvegame/domain/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:50:02.244541 mckinseysolvegame-0.8.4/mckinseysolvegame/domain/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/mckinseysolvegame/domain/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/mckinseysolvegame/domain/services/optimization_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:50:02.244541 mckinseysolvegame-0.8.4/mckinseysolvegame/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/mckinseysolvegame/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/mckinseysolvegame/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30532 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/mckinseysolvegame/tests/test_optimization_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:50:02.244541 mckinseysolvegame-0.8.4/mckinseysolvegame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-04-27 14:50:02.000000 mckinseysolvegame-0.8.4/mckinseysolvegame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-27 14:50:02.000000 mckinseysolvegame-0.8.4/mckinseysolvegame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 14:50:02.000000 mckinseysolvegame-0.8.4/mckinseysolvegame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-27 14:50:02.000000 mckinseysolvegame-0.8.4/mckinseysolvegame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 14:50:02.000000 mckinseysolvegame-0.8.4/mckinseysolvegame.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-27 14:50:02.244541 mckinseysolvegame-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-27 14:49:58.000000 mckinseysolvegame-0.8.4/setup.py
```

### Comparing `mckinseysolvegame-0.8.3/PKG-INFO` & `mckinseysolvegame-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mckinseysolvegame
-Version: 0.8.3
+Version: 0.8.4
 Summary: Python library for solving the McKinsey Solve Game
 Home-page: https://github.com/SebastienEveno/mckinseysolvegame
 Author: Sebastien Eveno
 Author-email: sebastien.louis.eveno@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -291,15 +291,15 @@
             calories_provided=1600,
             calories_needed=5600,
             depth_range="31-60m",
             temperature_range="26.7-28.2",
             food_sources=[
                 "Pacific Tripletail",
                 "Coral Beauty",
-                "Flameback  Angelfish"
+                "Flameback Angelfish"
                 ]),
     Species(name="Hawksbill Sea Turtle",
             calories_provided=2800,
             calories_needed=4950,
             depth_range="0-30m",
             temperature_range="28.3-30",
             food_sources=[
@@ -396,23 +396,24 @@
 result.to_json()
 ```
 
 The API will return a JSON object with the following format:
 ```json
 {
     "species": [
-        "Fire Coral", 
-        "Common Eel Grass", 
-        "Widgeon Grass",
-        "Queen Parrotfish", 
-        "Blue Striped Angelfish",
-        "Common Dolphinfish", 
-        "Wahoo", 
-        "Short-tail Stingray",
-        "Gem Tang"
+        "Purple Hydrocoral", 
+        "Stalked Kelp", 
+        "Blue Shark", 
+        "Rock Weed",
+        "Powder Blue Tang", 
+        "Flame Angelfish", 
+        "Swordfish", 
+        "Bicolour Angelfish",
+        "Northern Red Snapper", 
+        "Eyestripe Surgeonfish"
     ]
 }
 ```
 This object contains the maximum number of species that can sustain, as well as the list of species names.
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mckinseysolvegame Version: 0.8.3 Summary: Python
+Metadata-Version: 2.1 Name: mckinseysolvegame Version: 0.8.4 Summary: Python
 library for solving the McKinsey Solve Game Home-page: https://github.com/
 SebastienEveno/mckinseysolvegame Author: Sebastien Eveno Author-email:
 sebastien.louis.eveno@gmail.com License: MIT Classifier: Development Status ::
 4 - Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Science/Research Classifier: Topic :: Software Development Classifier: Topic ::
@@ -129,17 +129,18 @@
 temperature_range="26.7-28.2", food_sources=[ "Yellow Tube Sponge", "Peacock's
 Tail Algae" ]), Species(name="Common Dolphinfish", calories_provided=2150,
 calories_needed=2100, depth_range="0-30m", temperature_range="28.3-30",
 food_sources=["Queen Parrotfish"]) ] ``` ### Find the species that form a
 sustainable food chain ```python from mckinseysolvegame import Solver result =
 Solver.find_sustainable_food_chain(my_species) result.to_json() ``` The API
 will return a JSON object with the following format: ```json { "species":
-[ "Fire Coral", "Common Eel Grass", "Widgeon Grass", "Queen Parrotfish", "Blue
-Striped Angelfish", "Common Dolphinfish", "Wahoo", "Short-tail Stingray", "Gem
-Tang" ] } ``` This object contains the maximum number of species that can
-sustain, as well as the list of species names. ## Contributing We welcome
-contributions to mckinseysolvegame! If you find a bug or would like to request
-a new feature, please open an issue on the [Github repository](https://
-github.com/sebastieneveno/mckinseysolvegame). If you would like to contribute
-code, please submit a pull request. ## License mckinseysolvegame is released
-under the [MIT License](https://opensource.org/licenses/MIT). ## To Do List -
-Consider the case eating half of calories provided in case of a tie
+[ "Purple Hydrocoral", "Stalked Kelp", "Blue Shark", "Rock Weed", "Powder Blue
+Tang", "Flame Angelfish", "Swordfish", "Bicolour Angelfish", "Northern Red
+Snapper", "Eyestripe Surgeonfish" ] } ``` This object contains the maximum
+number of species that can sustain, as well as the list of species names. ##
+Contributing We welcome contributions to mckinseysolvegame! If you find a bug
+or would like to request a new feature, please open an issue on the [Github
+repository](https://github.com/sebastieneveno/mckinseysolvegame). If you would
+like to contribute code, please submit a pull request. ## License
+mckinseysolvegame is released under the [MIT License](https://opensource.org/
+licenses/MIT). ## To Do List - Consider the case eating half of calories
+provided in case of a tie
```

### Comparing `mckinseysolvegame-0.8.3/README.md` & `mckinseysolvegame-0.8.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,15 @@
             calories_provided=1600,
             calories_needed=5600,
             depth_range="31-60m",
             temperature_range="26.7-28.2",
             food_sources=[
                 "Pacific Tripletail",
                 "Coral Beauty",
-                "Flameback  Angelfish"
+                "Flameback Angelfish"
                 ]),
     Species(name="Hawksbill Sea Turtle",
             calories_provided=2800,
             calories_needed=4950,
             depth_range="0-30m",
             temperature_range="28.3-30",
             food_sources=[
@@ -372,23 +372,24 @@
 result.to_json()
 ```
 
 The API will return a JSON object with the following format:
 ```json
 {
     "species": [
-        "Fire Coral", 
-        "Common Eel Grass", 
-        "Widgeon Grass",
-        "Queen Parrotfish", 
-        "Blue Striped Angelfish",
-        "Common Dolphinfish", 
-        "Wahoo", 
-        "Short-tail Stingray",
-        "Gem Tang"
+        "Purple Hydrocoral", 
+        "Stalked Kelp", 
+        "Blue Shark", 
+        "Rock Weed",
+        "Powder Blue Tang", 
+        "Flame Angelfish", 
+        "Swordfish", 
+        "Bicolour Angelfish",
+        "Northern Red Snapper", 
+        "Eyestripe Surgeonfish"
     ]
 }
 ```
 This object contains the maximum number of species that can sustain, as well as the list of species names.
 
 ## Contributing
```

#### html2text {}

```diff
@@ -118,17 +118,18 @@
 temperature_range="26.7-28.2", food_sources=[ "Yellow Tube Sponge", "Peacock's
 Tail Algae" ]), Species(name="Common Dolphinfish", calories_provided=2150,
 calories_needed=2100, depth_range="0-30m", temperature_range="28.3-30",
 food_sources=["Queen Parrotfish"]) ] ``` ### Find the species that form a
 sustainable food chain ```python from mckinseysolvegame import Solver result =
 Solver.find_sustainable_food_chain(my_species) result.to_json() ``` The API
 will return a JSON object with the following format: ```json { "species":
-[ "Fire Coral", "Common Eel Grass", "Widgeon Grass", "Queen Parrotfish", "Blue
-Striped Angelfish", "Common Dolphinfish", "Wahoo", "Short-tail Stingray", "Gem
-Tang" ] } ``` This object contains the maximum number of species that can
-sustain, as well as the list of species names. ## Contributing We welcome
-contributions to mckinseysolvegame! If you find a bug or would like to request
-a new feature, please open an issue on the [Github repository](https://
-github.com/sebastieneveno/mckinseysolvegame). If you would like to contribute
-code, please submit a pull request. ## License mckinseysolvegame is released
-under the [MIT License](https://opensource.org/licenses/MIT). ## To Do List -
-Consider the case eating half of calories provided in case of a tie
+[ "Purple Hydrocoral", "Stalked Kelp", "Blue Shark", "Rock Weed", "Powder Blue
+Tang", "Flame Angelfish", "Swordfish", "Bicolour Angelfish", "Northern Red
+Snapper", "Eyestripe Surgeonfish" ] } ``` This object contains the maximum
+number of species that can sustain, as well as the list of species names. ##
+Contributing We welcome contributions to mckinseysolvegame! If you find a bug
+or would like to request a new feature, please open an issue on the [Github
+repository](https://github.com/sebastieneveno/mckinseysolvegame). If you would
+like to contribute code, please submit a pull request. ## License
+mckinseysolvegame is released under the [MIT License](https://opensource.org/
+licenses/MIT). ## To Do List - Consider the case eating half of calories
+provided in case of a tie
```

### Comparing `mckinseysolvegame-0.8.3/mckinseysolvegame/domain/models.py` & `mckinseysolvegame-0.8.4/mckinseysolvegame/domain/models.py`

 * *Files identical despite different names*

### Comparing `mckinseysolvegame-0.8.3/mckinseysolvegame/domain/services/optimization_service.py` & `mckinseysolvegame-0.8.4/mckinseysolvegame/domain/services/optimization_service.py`

 * *Files identical despite different names*

### Comparing `mckinseysolvegame-0.8.3/mckinseysolvegame/tests/test_models.py` & `mckinseysolvegame-0.8.4/mckinseysolvegame/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `mckinseysolvegame-0.8.3/mckinseysolvegame/tests/test_optimization_service.py` & `mckinseysolvegame-0.8.4/mckinseysolvegame/tests/test_optimization_service.py`

 * *Files identical despite different names*

### Comparing `mckinseysolvegame-0.8.3/mckinseysolvegame.egg-info/PKG-INFO` & `mckinseysolvegame-0.8.4/mckinseysolvegame.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mckinseysolvegame
-Version: 0.8.3
+Version: 0.8.4
 Summary: Python library for solving the McKinsey Solve Game
 Home-page: https://github.com/SebastienEveno/mckinseysolvegame
 Author: Sebastien Eveno
 Author-email: sebastien.louis.eveno@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -291,15 +291,15 @@
             calories_provided=1600,
             calories_needed=5600,
             depth_range="31-60m",
             temperature_range="26.7-28.2",
             food_sources=[
                 "Pacific Tripletail",
                 "Coral Beauty",
-                "Flameback  Angelfish"
+                "Flameback Angelfish"
                 ]),
     Species(name="Hawksbill Sea Turtle",
             calories_provided=2800,
             calories_needed=4950,
             depth_range="0-30m",
             temperature_range="28.3-30",
             food_sources=[
@@ -396,23 +396,24 @@
 result.to_json()
 ```
 
 The API will return a JSON object with the following format:
 ```json
 {
     "species": [
-        "Fire Coral", 
-        "Common Eel Grass", 
-        "Widgeon Grass",
-        "Queen Parrotfish", 
-        "Blue Striped Angelfish",
-        "Common Dolphinfish", 
-        "Wahoo", 
-        "Short-tail Stingray",
-        "Gem Tang"
+        "Purple Hydrocoral", 
+        "Stalked Kelp", 
+        "Blue Shark", 
+        "Rock Weed",
+        "Powder Blue Tang", 
+        "Flame Angelfish", 
+        "Swordfish", 
+        "Bicolour Angelfish",
+        "Northern Red Snapper", 
+        "Eyestripe Surgeonfish"
     ]
 }
 ```
 This object contains the maximum number of species that can sustain, as well as the list of species names.
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mckinseysolvegame Version: 0.8.3 Summary: Python
+Metadata-Version: 2.1 Name: mckinseysolvegame Version: 0.8.4 Summary: Python
 library for solving the McKinsey Solve Game Home-page: https://github.com/
 SebastienEveno/mckinseysolvegame Author: Sebastien Eveno Author-email:
 sebastien.louis.eveno@gmail.com License: MIT Classifier: Development Status ::
 4 - Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Science/Research Classifier: Topic :: Software Development Classifier: Topic ::
@@ -129,17 +129,18 @@
 temperature_range="26.7-28.2", food_sources=[ "Yellow Tube Sponge", "Peacock's
 Tail Algae" ]), Species(name="Common Dolphinfish", calories_provided=2150,
 calories_needed=2100, depth_range="0-30m", temperature_range="28.3-30",
 food_sources=["Queen Parrotfish"]) ] ``` ### Find the species that form a
 sustainable food chain ```python from mckinseysolvegame import Solver result =
 Solver.find_sustainable_food_chain(my_species) result.to_json() ``` The API
 will return a JSON object with the following format: ```json { "species":
-[ "Fire Coral", "Common Eel Grass", "Widgeon Grass", "Queen Parrotfish", "Blue
-Striped Angelfish", "Common Dolphinfish", "Wahoo", "Short-tail Stingray", "Gem
-Tang" ] } ``` This object contains the maximum number of species that can
-sustain, as well as the list of species names. ## Contributing We welcome
-contributions to mckinseysolvegame! If you find a bug or would like to request
-a new feature, please open an issue on the [Github repository](https://
-github.com/sebastieneveno/mckinseysolvegame). If you would like to contribute
-code, please submit a pull request. ## License mckinseysolvegame is released
-under the [MIT License](https://opensource.org/licenses/MIT). ## To Do List -
-Consider the case eating half of calories provided in case of a tie
+[ "Purple Hydrocoral", "Stalked Kelp", "Blue Shark", "Rock Weed", "Powder Blue
+Tang", "Flame Angelfish", "Swordfish", "Bicolour Angelfish", "Northern Red
+Snapper", "Eyestripe Surgeonfish" ] } ``` This object contains the maximum
+number of species that can sustain, as well as the list of species names. ##
+Contributing We welcome contributions to mckinseysolvegame! If you find a bug
+or would like to request a new feature, please open an issue on the [Github
+repository](https://github.com/sebastieneveno/mckinseysolvegame). If you would
+like to contribute code, please submit a pull request. ## License
+mckinseysolvegame is released under the [MIT License](https://opensource.org/
+licenses/MIT). ## To Do List - Consider the case eating half of calories
+provided in case of a tie
```

### Comparing `mckinseysolvegame-0.8.3/mckinseysolvegame.egg-info/SOURCES.txt` & `mckinseysolvegame-0.8.4/mckinseysolvegame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mckinseysolvegame-0.8.3/setup.py` & `mckinseysolvegame-0.8.4/setup.py`

 * *Files identical despite different names*

