# Comparing `tmp/openai-cost-logger-0.2.1.tar.gz` & `tmp/openai-cost-logger-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-cost-logger-0.2.1.tar", last modified: Mon Apr 15 20:37:29 2024, max compression
+gzip compressed data, was "openai-cost-logger-0.3.0.tar", last modified: Sat Apr 27 10:17:24 2024, max compression
```

## Comparing `openai-cost-logger-0.2.1.tar` & `openai-cost-logger-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:37:29.964683 openai-cost-logger-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-15 20:37:27.000000 openai-cost-logger-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-15 20:37:29.964683 openai-cost-logger-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-15 20:37:27.000000 openai-cost-logger-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:37:29.964683 openai-cost-logger-0.2.1/openai_cost_logger/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-15 20:37:27.000000 openai-cost-logger-0.2.1/openai_cost_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-15 20:37:27.000000 openai-cost-logger-0.2.1/openai_cost_logger/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-15 20:37:27.000000 openai-cost-logger-0.2.1/openai_cost_logger/openai_cost_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-15 20:37:27.000000 openai-cost-logger-0.2.1/openai_cost_logger/openai_cost_logger_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-04-15 20:37:27.000000 openai-cost-logger-0.2.1/openai_cost_logger/openai_cost_logger_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:37:29.964683 openai-cost-logger-0.2.1/openai_cost_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-15 20:37:29.000000 openai-cost-logger-0.2.1/openai_cost_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-15 20:37:29.000000 openai-cost-logger-0.2.1/openai_cost_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:37:29.000000 openai-cost-logger-0.2.1/openai_cost_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 20:37:29.000000 openai-cost-logger-0.2.1/openai_cost_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 20:37:29.000000 openai-cost-logger-0.2.1/openai_cost_logger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:37:29.964683 openai-cost-logger-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-15 20:37:27.000000 openai-cost-logger-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:17:24.107349 openai-cost-logger-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-27 10:17:19.000000 openai-cost-logger-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-27 10:17:24.103349 openai-cost-logger-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-27 10:17:19.000000 openai-cost-logger-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:17:24.103349 openai-cost-logger-0.3.0/openai_cost_logger/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-27 10:17:19.000000 openai-cost-logger-0.3.0/openai_cost_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-27 10:17:19.000000 openai-cost-logger-0.3.0/openai_cost_logger/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-04-27 10:17:19.000000 openai-cost-logger-0.3.0/openai_cost_logger/openai_cost_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-27 10:17:19.000000 openai-cost-logger-0.3.0/openai_cost_logger/openai_cost_logger_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-27 10:17:19.000000 openai-cost-logger-0.3.0/openai_cost_logger/openai_cost_logger_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:17:24.103349 openai-cost-logger-0.3.0/openai_cost_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-27 10:17:24.000000 openai-cost-logger-0.3.0/openai_cost_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-27 10:17:24.000000 openai-cost-logger-0.3.0/openai_cost_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 10:17:24.000000 openai-cost-logger-0.3.0/openai_cost_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-27 10:17:24.000000 openai-cost-logger-0.3.0/openai_cost_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-27 10:17:24.000000 openai-cost-logger-0.3.0/openai_cost_logger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 10:17:24.107349 openai-cost-logger-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-27 10:17:19.000000 openai-cost-logger-0.3.0/setup.py
```

### Comparing `openai-cost-logger-0.2.1/LICENSE` & `openai-cost-logger-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai-cost-logger-0.2.1/PKG-INFO` & `openai-cost-logger-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,63 @@
 Metadata-Version: 2.1
 Name: openai-cost-logger
-Version: 0.2.1
+Version: 0.3.0
 Summary: OpenAI Cost Logger
 Home-page: https://github.com/drudilorenzo/openai-cost-tracker
 Author: Lorenzo Drudi | Mikolaj Boronski | Ivan Zakazov
 Author-email: lorenzodrudi11@gmail.com
 License: MIT
-Keywords: openai,cost,logger,tracker
+Keywords: openai,cost,logger,tracker,viz,llms
 Platform: UNKNOWN
 Requires: openai
 Requires: pandas
 Requires: matplotlib
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://img.shields.io/badge/chatGPT-74aa9c.svg?logo=openai
 .. image:: https://img.shields.io/pypi/pyversions/setuptools.svg
 
 ==================
 OpenAI Cost Logger
 ==================
 
-Simple cost logger for OpenAI requests.
-Track the cost of every request you make to OpenAI and visualize them in a user-friendly way.
+* Simple **cost logger** for **OpenAI requests**.
+* Track the cost of every request you make to OpenAI and visualize them in a user-friendly way.
+* Homepage on `PyPI <https://pypi.org/project/openai-cost-logger/>`_.
+* `Demo file <https://github.com/drudilorenzo/track-openai-cost/blob/master/demo.ipynb>`_ with a usage example.
 
 How to install:
 ---------------
 * .. code-block:: python
 
       pip install openai-cost-logger
 
 * .. code-block:: python
 
-      from openai_cost_logger.constants import DEFAULT_LOG_PATH, Models, MODELS_COST
-      from openai_cost_logger.openai_cost_logger_viz import OpenAICostLoggerViz
-      from openai_cost_logger.openai_cost_logger_utils import OpenAICostLoggerUtils
-      from openai_cost_logger.openai_cost_logger import OpenAICostLogger
-
-* See also the homepage on `PyPI <https://pypi.org/project/openai-cost-logger/>`_.
-* See the `demo file <https://github.com/drudilorenzo/track-openai-cost/blob/master/demo.ipynb>`_ for a usage example.
+      from openai_cost_logger import OpenAICostLogger
+      from openai_cost_logger import OpenAICostLoggerViz
+      from openai_cost_logger import OpenAICostLoggerUtils
+      from openai_cost_logger import DEFAULT_LOG_PATH, MODELS_COST
 
 Key Features:
 -------------
 * Track the cost of every request you make and save them in a JSON file.
 * Choose the feature you want to track (prompt_tokens, completion_tokens, completion, prompt, etc.).
 * Check the cost of your requests filtering by model or strftime aggregation (see the docs).
 
-Endpoint supported:
+Models supported:
 -------------------
-* Chat completion.
-* Every response passed to *OpenAICostLogger* should contain the fields "*usage.prompt_tokens*" and "*usage.completion_tokens*".
-  This is the only strict requirement of the library, the way you call the OpenAI API is totally up to you. If needed, you can
-  find an easy example in the demo file.
+* The response generation is totally up to the user. The library support every model which response contains the fields **usage.prompt_tokens** and **usage.total_tokens** (e.g. chat completions, embeddings, etc.).
 
-Viz examples:
--------------
-.. image::images/viz_prints.png
-   :alt: Viz prints examples.
-   :align: center
-   :width: 500px
+Note:
+-----
+* Every cost is specified per **million tokens**.
+* If you don't specify the cost, the library will look to the **MODELS_COST** dictionary and get the cost of the model you are using. Be aware that if the model is not in the dictionary, an exception will be raised.
 
-.. image::images/strftime_agg.png
-   :alt: Strftime aggregation example.
+Viz example:
+-------------
+.. image:: images/example.png
+   :alt: Viz example (prints + plot)
    :align: center
-   :width: 500px   
-
```

### Comparing `openai-cost-logger-0.2.1/README.rst` & `openai-cost-logger-0.3.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,45 @@
 .. image:: https://img.shields.io/badge/chatGPT-74aa9c.svg?logo=openai
 .. image:: https://img.shields.io/pypi/pyversions/setuptools.svg
 
 ==================
 OpenAI Cost Logger
 ==================
 
-Simple cost logger for OpenAI requests.
-Track the cost of every request you make to OpenAI and visualize them in a user-friendly way.
+* Simple **cost logger** for **OpenAI requests**.
+* Track the cost of every request you make to OpenAI and visualize them in a user-friendly way.
+* Homepage on `PyPI <https://pypi.org/project/openai-cost-logger/>`_.
+* `Demo file <https://github.com/drudilorenzo/track-openai-cost/blob/master/demo.ipynb>`_ with a usage example.
 
 How to install:
 ---------------
 * .. code-block:: python
 
       pip install openai-cost-logger
 
 * .. code-block:: python
 
-      from openai_cost_logger.constants import DEFAULT_LOG_PATH, Models, MODELS_COST
-      from openai_cost_logger.openai_cost_logger_viz import OpenAICostLoggerViz
-      from openai_cost_logger.openai_cost_logger_utils import OpenAICostLoggerUtils
-      from openai_cost_logger.openai_cost_logger import OpenAICostLogger
-
-* See also the homepage on `PyPI <https://pypi.org/project/openai-cost-logger/>`_.
-* See the `demo file <https://github.com/drudilorenzo/track-openai-cost/blob/master/demo.ipynb>`_ for a usage example.
+      from openai_cost_logger import OpenAICostLogger
+      from openai_cost_logger import OpenAICostLoggerViz
+      from openai_cost_logger import OpenAICostLoggerUtils
+      from openai_cost_logger import DEFAULT_LOG_PATH, MODELS_COST
 
 Key Features:
 -------------
 * Track the cost of every request you make and save them in a JSON file.
 * Choose the feature you want to track (prompt_tokens, completion_tokens, completion, prompt, etc.).
 * Check the cost of your requests filtering by model or strftime aggregation (see the docs).
 
-Endpoint supported:
+Models supported:
 -------------------
-* Chat completion.
-* Every response passed to *OpenAICostLogger* should contain the fields "*usage.prompt_tokens*" and "*usage.completion_tokens*".
-  This is the only strict requirement of the library, the way you call the OpenAI API is totally up to you. If needed, you can
-  find an easy example in the demo file.
+* The response generation is totally up to the user. The library support every model which response contains the fields **usage.prompt_tokens** and **usage.total_tokens** (e.g. chat completions, embeddings, etc.).
 
-Viz examples:
--------------
-.. image::images/viz_prints.png
-   :alt: Viz prints examples.
-   :align: center
-   :width: 500px
+Note:
+-----
+* Every cost is specified per **million tokens**.
+* If you don't specify the cost, the library will look to the **MODELS_COST** dictionary and get the cost of the model you are using. Be aware that if the model is not in the dictionary, an exception will be raised.
 
-.. image::images/strftime_agg.png
-   :alt: Strftime aggregation example.
+Viz example:
+-------------
+.. image:: images/example.png
+   :alt: Viz example (prints + plot)
    :align: center
-   :width: 500px   
-
```

### Comparing `openai-cost-logger-0.2.1/openai_cost_logger/constants.py` & `openai-cost-logger-0.3.0/openai_cost_logger/constants.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,12 @@
-from enum import Enum
-
 """Default value for the cost-logs directory."""
 DEFAULT_LOG_PATH = "cost-logs"
+    
 
-"""Enum containing the tested models."""
-class Models(Enum):
-    TURBO_3_5 = "gpt-3.5-turbo"
-    TURBO_3_5_INSTRUCT = "gpt-3.5-turbo-instruct"
-    AZURE_3_5_TURBO = "gpt-35-turbo-0125"
-    AZURE_4_TURBO = "gpt-4-0125-Preview"
-    AZURE_4 = "gpt-4-0613"
-
-"""The costs of the models above (per million tokens)."""
+"""The costs of the models above (per million tokens). Dictionary used in case the user does not provide the costs."""
 MODELS_COST = {
     "gpt-3.5-turbo": {
         "input": 0.5,
         "output": 1.5
     },
     "gpt-35-turbo-0125": {
         "input": 0.5,
@@ -29,8 +20,12 @@
         "input": 10,
         "output": 30
     },
     "gpt-4-0613": {
         "input": 30,
         "output": 60
     },
+    "text-embedding-ada-002": {
+        "input": 0.1,
+        "output": 0.0
+    }
 }
```

### Comparing `openai-cost-logger-0.2.1/openai_cost_logger/openai_cost_logger_viz.py` & `openai-cost-logger-0.3.0/openai_cost_logger/openai_cost_logger_viz.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
 import json
-from datetime import datetime
 from typing import Dict
 from pathlib import Path
+from datetime import datetime
 import matplotlib.pyplot as plt
 from collections import defaultdict
 
 from openai_cost_logger.constants import DEFAULT_LOG_PATH
 
+
 """Cost logger visualizer."""
 class OpenAICostLoggerViz:
     
     @staticmethod
     def get_total_cost(path: str = DEFAULT_LOG_PATH) -> float:
         """Return the total cost of all the logs in the directory.
 
@@ -53,28 +54,27 @@
             Dict[str, float]: the total cost by model.
         """
         cost_by_model = defaultdict(float)
         for filename in os.listdir(path):
             if filename.endswith(".json"):
                 with open(Path(path, filename), mode='r') as file:
                     data = json.load(file)
-                    if data["model"] not in cost_by_model:
-                        cost_by_model[data["model"]] = 0
-                    cost_by_model[data["model"]] += data["total_cost"]
+                    for entry in data["breakdown"]:
+                        cost_by_model[entry["model"]] += entry["cost"]
         return cost_by_model
 
 
     def print_total_cost_by_model(path: str = DEFAULT_LOG_PATH) -> None:
         """Print the total cost by model of all the logs in the directory.
 
         Args:
             log_folder (str, optional): Cost logs directory. Defaults to DEFAULT_LOG_PATH.
                                         This method reads all the files in the specified directory.
         """
-        cost_by_model = OpenAICostLoggerViz.get_total_cost_by_model(path)
+        cost_by_model = OpenAICostLoggerViz.get_total_cost_by_model(path=path)
         for model, cost in cost_by_model.items():
             print(f"{model}: {round(cost, 6)} (USD)")
 
 
     @staticmethod
     def plot_cost_by_strftime(path: str = DEFAULT_LOG_PATH, strftime_aggregator: str = "%Y-%m-%d", last_n_days: int = None) -> None:
         """Plot the cost by day of all the logs in the directory aggregated using strftime_aggregator.
```

### Comparing `openai-cost-logger-0.2.1/openai_cost_logger.egg-info/PKG-INFO` & `openai-cost-logger-0.3.0/openai_cost_logger.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,63 @@
 Metadata-Version: 2.1
 Name: openai-cost-logger
-Version: 0.2.1
+Version: 0.3.0
 Summary: OpenAI Cost Logger
 Home-page: https://github.com/drudilorenzo/openai-cost-tracker
 Author: Lorenzo Drudi | Mikolaj Boronski | Ivan Zakazov
 Author-email: lorenzodrudi11@gmail.com
 License: MIT
-Keywords: openai,cost,logger,tracker
+Keywords: openai,cost,logger,tracker,viz,llms
 Platform: UNKNOWN
 Requires: openai
 Requires: pandas
 Requires: matplotlib
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://img.shields.io/badge/chatGPT-74aa9c.svg?logo=openai
 .. image:: https://img.shields.io/pypi/pyversions/setuptools.svg
 
 ==================
 OpenAI Cost Logger
 ==================
 
-Simple cost logger for OpenAI requests.
-Track the cost of every request you make to OpenAI and visualize them in a user-friendly way.
+* Simple **cost logger** for **OpenAI requests**.
+* Track the cost of every request you make to OpenAI and visualize them in a user-friendly way.
+* Homepage on `PyPI <https://pypi.org/project/openai-cost-logger/>`_.
+* `Demo file <https://github.com/drudilorenzo/track-openai-cost/blob/master/demo.ipynb>`_ with a usage example.
 
 How to install:
 ---------------
 * .. code-block:: python
 
       pip install openai-cost-logger
 
 * .. code-block:: python
 
-      from openai_cost_logger.constants import DEFAULT_LOG_PATH, Models, MODELS_COST
-      from openai_cost_logger.openai_cost_logger_viz import OpenAICostLoggerViz
-      from openai_cost_logger.openai_cost_logger_utils import OpenAICostLoggerUtils
-      from openai_cost_logger.openai_cost_logger import OpenAICostLogger
-
-* See also the homepage on `PyPI <https://pypi.org/project/openai-cost-logger/>`_.
-* See the `demo file <https://github.com/drudilorenzo/track-openai-cost/blob/master/demo.ipynb>`_ for a usage example.
+      from openai_cost_logger import OpenAICostLogger
+      from openai_cost_logger import OpenAICostLoggerViz
+      from openai_cost_logger import OpenAICostLoggerUtils
+      from openai_cost_logger import DEFAULT_LOG_PATH, MODELS_COST
 
 Key Features:
 -------------
 * Track the cost of every request you make and save them in a JSON file.
 * Choose the feature you want to track (prompt_tokens, completion_tokens, completion, prompt, etc.).
 * Check the cost of your requests filtering by model or strftime aggregation (see the docs).
 
-Endpoint supported:
+Models supported:
 -------------------
-* Chat completion.
-* Every response passed to *OpenAICostLogger* should contain the fields "*usage.prompt_tokens*" and "*usage.completion_tokens*".
-  This is the only strict requirement of the library, the way you call the OpenAI API is totally up to you. If needed, you can
-  find an easy example in the demo file.
+* The response generation is totally up to the user. The library support every model which response contains the fields **usage.prompt_tokens** and **usage.total_tokens** (e.g. chat completions, embeddings, etc.).
 
-Viz examples:
--------------
-.. image::images/viz_prints.png
-   :alt: Viz prints examples.
-   :align: center
-   :width: 500px
+Note:
+-----
+* Every cost is specified per **million tokens**.
+* If you don't specify the cost, the library will look to the **MODELS_COST** dictionary and get the cost of the model you are using. Be aware that if the model is not in the dictionary, an exception will be raised.
 
-.. image::images/strftime_agg.png
-   :alt: Strftime aggregation example.
+Viz example:
+-------------
+.. image:: images/example.png
+   :alt: Viz example (prints + plot)
    :align: center
-   :width: 500px   
-
```

### Comparing `openai-cost-logger-0.2.1/setup.py` & `openai-cost-logger-0.3.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 from setuptools import setup, find_packages
-import os
 
 # Read the README file (reStructuredText format)
 with open('README.rst') as f:
     long_description = f.read()
 
-# Get the version number from the environment
-# version_number = os.getenv('VERSION_NUMBER')
-# version_number = version_number.strip("v")
-
-version_number = '0.2.1'
+version_number = '0.3.0'
 
 setup(
     name='openai-cost-logger',
     version=version_number,
     author='Lorenzo Drudi | Mikolaj Boronski | Ivan Zakazov',
     description='OpenAI Cost Logger',
     author_email='lorenzodrudi11@gmail.com',
     url='https://github.com/drudilorenzo/openai-cost-tracker',
     long_description=long_description,
     long_description_content_type='text/x-rst',
-    keywords=['openai', 'cost', 'logger', 'tracker'],
+    keywords=['openai', 'cost', 'logger', 'tracker', 'viz', 'llms'],
     license='MIT',
     packages=find_packages(include=['openai_cost_logger', 'openai_cost_logger.*']),
     requires=['openai', 'pandas', 'matplotlib'],
     install_requires=['openai', 'pandas', 'matplotlib']
 )
```

