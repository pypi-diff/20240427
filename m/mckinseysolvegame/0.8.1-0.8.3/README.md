# Comparing `tmp/mckinseysolvegame-0.8.1.tar.gz` & `tmp/mckinseysolvegame-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mckinseysolvegame-0.8.1.tar", last modified: Sat Mar 23 11:01:26 2024, max compression
+gzip compressed data, was "mckinseysolvegame-0.8.3.tar", last modified: Sat Apr 27 14:44:26 2024, max compression
```

## Comparing `mckinseysolvegame-0.8.1.tar` & `mckinseysolvegame-0.8.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:01:26.064031 mckinseysolvegame-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)    15027 2024-03-23 11:01:26.064031 mckinseysolvegame-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14143 2024-03-23 11:01:21.000000 mckinseysolvegame-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:01:26.064031 mckinseysolvegame-0.8.1/mckinseysolvegame/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-23 11:01:21.000000 mckinseysolvegame-0.8.1/mckinseysolvegame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-23 11:01:21.000000 mckinseysolvegame-0.8.1/mckinseysolvegame/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:01:26.064031 mckinseysolvegame-0.8.1/mckinseysolvegame/domain/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-23 11:01:21.000000 mckinseysolvegame-0.8.1/mckinseysolvegame/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-03-23 11:01:21.000000 mckinseysolvegame-0.8.1/mckinseysolvegame/domain/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:01:26.064031 mckinseysolvegame-0.8.1/mckinseysolvegame/domain/services/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-23 11:01:21.000000 mckinseysolvegame-0.8.1/mckinseysolvegame/domain/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-03-23 11:01:21.000000 mckinseysolvegame-0.8.1/mckinseysolvegame/domain/services/optimization_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:01:26.064031 mckinseysolvegame-0.8.1/mckinseysolvegame/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 11:01:21.000000 mckinseysolvegame-0.8.1/mckinseysolvegame/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-03-23 11:01:21.000000 mckinseysolvegame-0.8.1/mckinseysolvegame/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    30676 2024-03-23 11:01:21.000000 mckinseysolvegame-0.8.1/mckinseysolvegame/tests/test_optimization_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:01:26.064031 mckinseysolvegame-0.8.1/mckinseysolvegame.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15027 2024-03-23 11:01:26.000000 mckinseysolvegame-0.8.1/mckinseysolvegame.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-23 11:01:26.000000 mckinseysolvegame-0.8.1/mckinseysolvegame.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 11:01:26.000000 mckinseysolvegame-0.8.1/mckinseysolvegame.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-23 11:01:26.000000 mckinseysolvegame-0.8.1/mckinseysolvegame.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-23 11:01:26.000000 mckinseysolvegame-0.8.1/mckinseysolvegame.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-23 11:01:21.000000 mckinseysolvegame-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-23 11:01:26.068031 mckinseysolvegame-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-23 11:01:21.000000 mckinseysolvegame-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:44:26.248210 mckinseysolvegame-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    15027 2024-04-27 14:44:26.248210 mckinseysolvegame-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14143 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:44:26.244210 mckinseysolvegame-0.8.3/mckinseysolvegame/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/mckinseysolvegame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/mckinseysolvegame/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:44:26.244210 mckinseysolvegame-0.8.3/mckinseysolvegame/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/mckinseysolvegame/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/mckinseysolvegame/domain/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:44:26.244210 mckinseysolvegame-0.8.3/mckinseysolvegame/domain/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/mckinseysolvegame/domain/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/mckinseysolvegame/domain/services/optimization_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:44:26.248210 mckinseysolvegame-0.8.3/mckinseysolvegame/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/mckinseysolvegame/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/mckinseysolvegame/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30532 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/mckinseysolvegame/tests/test_optimization_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:44:26.248210 mckinseysolvegame-0.8.3/mckinseysolvegame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15027 2024-04-27 14:44:26.000000 mckinseysolvegame-0.8.3/mckinseysolvegame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-27 14:44:26.000000 mckinseysolvegame-0.8.3/mckinseysolvegame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 14:44:26.000000 mckinseysolvegame-0.8.3/mckinseysolvegame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-27 14:44:26.000000 mckinseysolvegame-0.8.3/mckinseysolvegame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 14:44:26.000000 mckinseysolvegame-0.8.3/mckinseysolvegame.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-27 14:44:26.248210 mckinseysolvegame-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-27 14:44:22.000000 mckinseysolvegame-0.8.3/setup.py
```

### Comparing `mckinseysolvegame-0.8.1/PKG-INFO` & `mckinseysolvegame-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mckinseysolvegame
-Version: 0.8.1
+Version: 0.8.3
 Summary: Python library for solving the McKinsey Solve Game
 Home-page: https://github.com/SebastienEveno/mckinseysolvegame
 Author: Sebastien Eveno
 Author-email: sebastien.louis.eveno@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mckinseysolvegame Version: 0.8.1 Summary: Python
+Metadata-Version: 2.1 Name: mckinseysolvegame Version: 0.8.3 Summary: Python
 library for solving the McKinsey Solve Game Home-page: https://github.com/
 SebastienEveno/mckinseysolvegame Author: Sebastien Eveno Author-email:
 sebastien.louis.eveno@gmail.com License: MIT Classifier: Development Status ::
 4 - Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Science/Research Classifier: Topic :: Software Development Classifier: Topic ::
```

### Comparing `mckinseysolvegame-0.8.1/README.md` & `mckinseysolvegame-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `mckinseysolvegame-0.8.1/mckinseysolvegame/domain/models.py` & `mckinseysolvegame-0.8.3/mckinseysolvegame/domain/models.py`

 * *Files identical despite different names*

### Comparing `mckinseysolvegame-0.8.1/mckinseysolvegame/tests/test_models.py` & `mckinseysolvegame-0.8.3/mckinseysolvegame/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `mckinseysolvegame-0.8.1/mckinseysolvegame/tests/test_optimization_service.py` & `mckinseysolvegame-0.8.3/mckinseysolvegame/tests/test_optimization_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-import glob
-import json
-import os
-import time
-
 import pytest
 
 from mckinseysolvegame.domain.models import Species
 from mckinseysolvegame.domain.services.optimization_service import Solver
 
 
 @pytest.mark.parametrize(
@@ -424,77 +419,77 @@
                             "Northern Red Snapper",
                             "Coral Trout",
                             "Swordfish",
                             "Sailfin Tang",
                             "Powder Blue Tang",
                             "Flame Angelfish",
                             "Eyestripe Surgeonfish"
-                            ]
+                        ]
                         ),
                 Species(name="Bicolour Angelfish",
                         calories_provided=1900,
                         calories_needed=440,
                         depth_range="61-90m",
                         temperature_range="25-26.6",
                         food_sources=[
                             "Powder Blue Tang",
                             "Flame Angelfish",
                             "Eyestripe Surgeonfish",
                             "Stalked Kelp",
                             "Purple Hydrocoral"
-                            ]
+                        ]
                         ),
                 Species(name="Bicolour Parrotfish",
                         calories_provided=3400,
                         calories_needed=8800,
                         depth_range="0-30m",
                         temperature_range="28.3-30",
                         food_sources=[
                             "Widgeon Grass",
                             "Common Eel Grass",
                             "Fire Coral"
-                            ]
+                        ]
                         ),
                 Species(name="Wahoo",
                         calories_provided=1700,
                         calories_needed=2500,
                         depth_range="0-30m",
                         temperature_range="28.3-30",
                         food_sources=[
                             "Short-tail Stingray",
                             "Blue Striped Angelfish"
-                            ]
+                        ]
                         ),
                 Species(name="Swordfish",
                         calories_provided=2000,
                         calories_needed=500,
                         depth_range="61-90m",
                         temperature_range="25-26.6",
                         food_sources=[
                             "Bicolour Angelfish"
-                            ]
+                        ]
                         ),
                 Species(name="Short-tail Stingray",
                         calories_provided=1450,
                         calories_needed=2050,
                         depth_range="0-30m",
                         temperature_range="28.3-30",
                         food_sources=[
                             "Common Dolphinfish",
                             "Foxface Rabbitfish"
-                            ]
+                        ]
                         ),
                 Species(name="Sailfin Tang",
                         calories_provided=2500,
                         calories_needed=4800,
                         depth_range="61-90m",
                         temperature_range="25-26.6",
                         food_sources=[
                             "Rock Weed"
-                            ]
+                        ]
                         ),
                 Species(name="Queen Parrotfish",
                         calories_provided=3800,
                         calories_needed=4700,
                         depth_range="0-30m",
                         temperature_range="28.3-30",
                         food_sources=["Fire Coral"]),
@@ -503,120 +498,120 @@
                         calories_needed=3100,
                         depth_range="0-30m",
                         temperature_range="28.3-30",
                         food_sources=[
                             "Blue Striped Angelfish",
                             "Queen Parrotfish",
                             "Common Eel Grass"
-                            ]
+                        ]
                         ),
                 Species(name="Powder Blue Tang",
                         calories_provided=3600,
                         calories_needed=4350,
                         depth_range="61-90m",
                         temperature_range="25-26.6",
                         food_sources=[
                             "Stalked Kelp",
                             "Purple Hydrocoral"
-                            ]
+                        ]
                         ),
                 Species(name="Porcupine Pufferfish",
                         calories_provided=2600,
                         calories_needed=3800,
                         depth_range="31-60m",
                         temperature_range="26.7-28.2",
                         food_sources=[
                             "Peacock's Tail Algae",
                             "Passer Angelfish"
-                            ]
+                        ]
                         ),
                 Species(name="Passer Angelfish",
                         calories_provided=2250,
                         calories_needed=4600,
                         depth_range="31-60m",
                         temperature_range="26.7-28.2",
                         food_sources=[
                             "Peacock's Tail Algae"
-                            ]
+                        ]
                         ),
                 Species(name="Pacific Tripletail",
                         calories_provided=2150,
                         calories_needed=2900,
                         depth_range="31-60m",
                         temperature_range="26.7-28.2",
                         food_sources=[
                             "Coral Beauty"
-                            ]
+                        ]
                         ),
                 Species(name="Olive Ridley Turtle",
                         calories_provided=3550,
                         calories_needed=4400,
                         depth_range="31-60m",
                         temperature_range="26.7-28.2",
                         food_sources=[
                             "Green Zoanthid",
                             "Pacific Tripletail"
-                            ]
+                        ]
                         ),
                 Species(name="Northern Red Snapper",
                         calories_provided=1200,
                         calories_needed=2150,
                         depth_range="61-90m",
                         temperature_range="25-26.6",
                         food_sources=[
                             "Majestic Angelfish",
                             "Sailfin Tang",
                             "Flame Angelfish",
                             "Eyestripe Surgeonfish"
-                            ]
+                        ]
                         ),
                 Species(name="Majestic Angelfish",
                         calories_provided=1150,
                         calories_needed=3200,
                         depth_range="61-90m",
                         temperature_range="25-26.6",
                         food_sources=[
                             "Sailfin Tang",
                             "Powder Blue Tang",
                             "Eyestripe Surgeonfish",
                             "Stalked Kelp"
-                            ]
+                        ]
                         ),
                 Species(name="Long Finned Pilot Whale",
                         calories_provided=3100,
                         calories_needed=950,
                         depth_range="31-60m",
                         temperature_range="26.7-28.2",
                         food_sources=[
                             "Pacific Tripletail"
-                            ]
+                        ]
                         ),
                 Species(name="Indo-Pacific Sailfish",
                         calories_provided=1600,
                         calories_needed=5600,
                         depth_range="31-60m",
                         temperature_range="26.7-28.2",
                         food_sources=[
                             "Pacific Tripletail",
                             "Coral Beauty",
-                            "Flameback  Angelfish"
-                            ]
+                            "Flameback Angelfish"
+                        ]
                         ),
                 Species(name="Hawksbill Sea Turtle",
                         calories_provided=2800,
                         calories_needed=4950,
                         depth_range="0-30m",
                         temperature_range="28.3-30",
                         food_sources=[
                             "Blue Striped Angelfish",
                             "Queen Parrotfish",
                             "Foxface Rabbitfish",
                             "Common Eel Grass",
                             "Fire Coral"
-                            ]
+                        ]
                         ),
                 Species(name="Gem Tang",
                         calories_provided=1250,
                         calories_needed=4900,
                         depth_range="0-30m",
                         temperature_range="28.3-30",
                         food_sources=["Widgeon Grass"]),
@@ -624,91 +619,90 @@
                         calories_provided=800,
                         calories_needed=4050,
                         depth_range="0-30m",
                         temperature_range="28.3-30",
                         food_sources=[
                             "Widgeon Grass",
                             "Fire Coral"
-                            ]
+                        ]
                         ),
                 Species(name="Flameback Angelfish",
                         calories_provided=2900,
                         calories_needed=4750,
                         depth_range="31-60m",
                         temperature_range="26.7-28.2",
                         food_sources=[
                             "Green Zoanthid"
-                            ]
+                        ]
                         ),
                 Species(name="Flame Angelfish",
                         calories_provided=2200,
                         calories_needed=4000,
                         depth_range="61-90m",
                         temperature_range="25-26.6",
                         food_sources=[
                             "Stalked Kelp",
                             "Rock Weed"
-                            ]
+                        ]
                         ),
                 Species(name="Eyestripe Surgeonfish",
                         calories_provided=1050,
                         calories_needed=3900,
                         depth_range="61-90m",
                         temperature_range="25-26.6",
                         food_sources=[
                             "Stalked Kelp",
                             "Rock Weed"
-                            ]
+                        ]
                         ),
                 Species(name="Cuvier Beaked Whale",
                         calories_provided=1400,
                         calories_needed=2250,
                         depth_range="31-60m",
                         temperature_range="26.7-28.2",
                         food_sources=[
                             "Coral Beauty",
                             "Flameback Angelfish"
-                            ]
+                        ]
                         ),
                 Species(name="Coral Trout",
                         calories_provided=1850,
                         calories_needed=3000,
                         depth_range="61-90m",
                         temperature_range="25-26.6",
                         food_sources=[
                             "Bicolour Angelfish",
                             "Powder Blue Tang",
                             "Flame Angelfish"
-                            ]
+                        ]
                         ),
                 Species(name="Coral Beauty",
                         calories_provided=2650,
                         calories_needed=4900,
                         depth_range="31-60m",
                         temperature_range="26.7-28.2",
                         food_sources=[
                             "Yellow Tube Sponge",
                             "Peacock's Tail Algae"
-                            ]
+                        ]
                         ),
                 Species(name="Common Dolphinfish",
                         calories_provided=2150,
                         calories_needed=2100,
                         depth_range="0-30m",
                         temperature_range="28.3-30",
                         food_sources=[
                             "Queen Parrotfish"
-                            ]
+                        ]
                         )
             ],
             [
-                'Fire Coral', 'Widgeon Grass', 'Common Eel Grass',
-                'Queen Parrotfish', 'Blue Striped Angelfish',
-                'Common Dolphinfish', 'Wahoo', 'Short-tail Stingray',
-                'Gem Tang'
+                'Purple Hydrocoral', 'Stalked Kelp', 'Blue Shark', 'Rock Weed',
+                'Powder Blue Tang', 'Flame Angelfish', 'Swordfish', 'Bicolour Angelfish',
+                'Northern Red Snapper', 'Eyestripe Surgeonfish'
             ]
         )
     ]
 )
 def test_find_sustainable_food_chain(species, expected_output):
     result = Solver.find_sustainable_food_chain(species)
     assert result.species == expected_output
```

### Comparing `mckinseysolvegame-0.8.1/mckinseysolvegame.egg-info/PKG-INFO` & `mckinseysolvegame-0.8.3/mckinseysolvegame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mckinseysolvegame
-Version: 0.8.1
+Version: 0.8.3
 Summary: Python library for solving the McKinsey Solve Game
 Home-page: https://github.com/SebastienEveno/mckinseysolvegame
 Author: Sebastien Eveno
 Author-email: sebastien.louis.eveno@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mckinseysolvegame Version: 0.8.1 Summary: Python
+Metadata-Version: 2.1 Name: mckinseysolvegame Version: 0.8.3 Summary: Python
 library for solving the McKinsey Solve Game Home-page: https://github.com/
 SebastienEveno/mckinseysolvegame Author: Sebastien Eveno Author-email:
 sebastien.louis.eveno@gmail.com License: MIT Classifier: Development Status ::
 4 - Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Science/Research Classifier: Topic :: Software Development Classifier: Topic ::
```

### Comparing `mckinseysolvegame-0.8.1/mckinseysolvegame.egg-info/SOURCES.txt` & `mckinseysolvegame-0.8.3/mckinseysolvegame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mckinseysolvegame-0.8.1/setup.py` & `mckinseysolvegame-0.8.3/setup.py`

 * *Files identical despite different names*

