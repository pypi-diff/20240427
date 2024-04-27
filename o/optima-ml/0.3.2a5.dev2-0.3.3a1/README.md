# Comparing `tmp/optima_ml-0.3.2a5.dev2.tar.gz` & `tmp/optima_ml-0.3.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optima_ml-0.3.2a5.dev2.tar", last modified: Fri Apr 19 01:05:05 2024, max compression
+gzip compressed data, was "optima_ml-0.3.3a1.tar", last modified: Sat Apr 27 00:10:37 2024, max compression
```

## Comparing `optima_ml-0.3.2a5.dev2.tar` & `optima_ml-0.3.3a1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/
--rw-rw-r--   0 erik     (30000) erik     (30003)    35150 2023-08-12 13:57:40.000000 optima_ml-0.3.2a5.dev2/LICENSE
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/OPTIMA/
--rw-rw-r--   0 erik     (30000) erik     (30003)      382 2024-01-30 16:21:26.000000 optima_ml-0.3.2a5.dev2/OPTIMA/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      132 2023-08-12 13:57:39.000000 optima_ml-0.3.2a5.dev2/OPTIMA/__main__.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/OPTIMA/builtin/
--rw-rw-r--   0 erik     (30000) erik     (30003)      137 2024-02-07 21:12:40.000000 optima_ml-0.3.2a5.dev2/OPTIMA/builtin/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    35402 2024-04-19 01:04:19.000000 optima_ml-0.3.2a5.dev2/OPTIMA/builtin/evaluation.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    32098 2024-02-07 21:12:40.000000 optima_ml-0.3.2a5.dev2/OPTIMA/builtin/figures_of_merit.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    66743 2024-03-23 18:21:18.000000 optima_ml-0.3.2a5.dev2/OPTIMA/builtin/inputs.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      423 2024-04-17 06:54:34.000000 optima_ml-0.3.2a5.dev2/OPTIMA/builtin/model.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     2858 2024-04-19 01:04:19.000000 optima_ml-0.3.2a5.dev2/OPTIMA/builtin/search_space.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/OPTIMA/core/
--rw-rw-r--   0 erik     (30000) erik     (30003)      114 2024-01-30 16:21:26.000000 optima_ml-0.3.2a5.dev2/OPTIMA/core/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    85793 2024-04-19 01:04:19.000000 optima_ml-0.3.2a5.dev2/OPTIMA/core/evaluation.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    19104 2024-03-23 18:05:57.000000 optima_ml-0.3.2a5.dev2/OPTIMA/core/inputs.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    10090 2024-04-17 06:54:34.000000 optima_ml-0.3.2a5.dev2/OPTIMA/core/model.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    25159 2024-04-19 01:04:19.000000 optima_ml-0.3.2a5.dev2/OPTIMA/core/search_space.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     3469 2024-03-23 18:53:01.000000 optima_ml-0.3.2a5.dev2/OPTIMA/core/tools.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    79735 2024-04-19 01:04:19.000000 optima_ml-0.3.2a5.dev2/OPTIMA/core/training.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    80215 2024-04-17 06:54:34.000000 optima_ml-0.3.2a5.dev2/OPTIMA/core/variable_optimization.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    16272 2024-04-17 06:54:34.000000 optima_ml-0.3.2a5.dev2/OPTIMA/defaults.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/OPTIMA/hardware_configs/
--rw-rw-r--   0 erik     (30000) erik     (30003)     2827 2024-04-17 12:02:38.000000 optima_ml-0.3.2a5.dev2/OPTIMA/hardware_configs/Dresden_Taurus.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      111 2024-01-30 16:21:26.000000 optima_ml-0.3.2a5.dev2/OPTIMA/hardware_configs/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    16772 2024-03-30 12:31:40.000000 optima_ml-0.3.2a5.dev2/OPTIMA/hardware_configs/common.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      505 2024-02-19 18:33:13.000000 optima_ml-0.3.2a5.dev2/OPTIMA/hardware_configs/helpers.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/OPTIMA/helpers/
--rw-rw-r--   0 erik     (30000) erik     (30003)       35 2024-01-30 16:21:26.000000 optima_ml-0.3.2a5.dev2/OPTIMA/helpers/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     4853 2024-01-30 16:21:26.000000 optima_ml-0.3.2a5.dev2/OPTIMA/helpers/extract_data_from_NTuples.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     8670 2024-04-17 06:54:34.000000 optima_ml-0.3.2a5.dev2/OPTIMA/helpers/manage_ray_nodes.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/OPTIMA/keras/
--rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-01-30 16:21:26.000000 optima_ml-0.3.2a5.dev2/OPTIMA/keras/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    28643 2024-04-19 01:04:19.000000 optima_ml-0.3.2a5.dev2/OPTIMA/keras/model.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    53862 2024-04-17 06:54:34.000000 optima_ml-0.3.2a5.dev2/OPTIMA/keras/tools.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     3912 2024-04-17 06:54:34.000000 optima_ml-0.3.2a5.dev2/OPTIMA/keras/training.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/OPTIMA/lightning/
--rw-rw-r--   0 erik     (30000) erik     (30003)      106 2024-01-30 16:23:00.000000 optima_ml-0.3.2a5.dev2/OPTIMA/lightning/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    10100 2024-03-24 16:56:32.000000 optima_ml-0.3.2a5.dev2/OPTIMA/lightning/inputs.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     6301 2024-01-30 16:21:26.000000 optima_ml-0.3.2a5.dev2/OPTIMA/lightning/training.py
--rwxrwxr-x   0 erik     (30000) erik     (30003)    99180 2024-04-19 01:04:38.000000 optima_ml-0.3.2a5.dev2/OPTIMA/optima.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/OPTIMA/resources/
--rw-rw-r--   0 erik     (30000) erik     (30003)        0 2023-08-12 13:57:39.000000 optima_ml-0.3.2a5.dev2/OPTIMA/resources/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     4772 2024-03-20 17:10:29.000000 optima_ml-0.3.2a5.dev2/OPTIMA/resources/config_verification.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    48922 2024-03-23 18:53:01.000000 optima_ml-0.3.2a5.dev2/OPTIMA/resources/pbt_with_seed.py
--rw-r--r--   0 erik     (30000) erik     (30003)    88934 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/PKG-INFO
--rw-rw-r--   0 erik     (30000) erik     (30003)    87528 2024-04-19 01:04:19.000000 optima_ml-0.3.2a5.dev2/README.md
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/optima_ml.egg-info/
--rw-r--r--   0 erik     (30000) erik     (30003)    88934 2024-04-19 01:05:05.000000 optima_ml-0.3.2a5.dev2/optima_ml.egg-info/PKG-INFO
--rw-rw-r--   0 erik     (30000) erik     (30003)     1342 2024-04-19 01:05:05.000000 optima_ml-0.3.2a5.dev2/optima_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)        1 2024-04-19 01:05:05.000000 optima_ml-0.3.2a5.dev2/optima_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-04-19 01:05:05.000000 optima_ml-0.3.2a5.dev2/optima_ml.egg-info/entry_points.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)      178 2024-04-19 01:05:05.000000 optima_ml-0.3.2a5.dev2/optima_ml.egg-info/requires.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)        7 2024-04-19 01:05:05.000000 optima_ml-0.3.2a5.dev2/optima_ml.egg-info/top_level.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)       38 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/setup.cfg
--rw-rw-r--   0 erik     (30000) erik     (30003)     4234 2024-04-19 01:04:19.000000 optima_ml-0.3.2a5.dev2/setup.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-19 01:05:05.478408 optima_ml-0.3.2a5.dev2/tests/
--rw-rw-r--   0 erik     (30000) erik     (30003)    37821 2024-04-17 06:54:34.000000 optima_ml-0.3.2a5.dev2/tests/test_builtin.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     8594 2024-02-07 21:12:40.000000 optima_ml-0.3.2a5.dev2/tests/test_core.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     6398 2024-01-30 16:21:26.000000 optima_ml-0.3.2a5.dev2/tests/test_integration.py
--rw-rw-rw-   0 erik     (30000) erik     (30003)     6399 2023-11-02 02:48:49.000000 optima_ml-0.3.2a5.dev2/tests/test_integration_sameMachine.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    56852 2024-03-24 16:53:28.000000 optima_ml-0.3.2a5.dev2/tests/test_preprocessing.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-27 00:10:37.777361 optima_ml-0.3.3a1/
+-rw-rw-r--   0 erik     (30000) erik     (30003)    35150 2023-08-12 13:57:40.000000 optima_ml-0.3.3a1/LICENSE
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-27 00:10:37.773362 optima_ml-0.3.3a1/OPTIMA/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      382 2024-01-30 16:21:26.000000 optima_ml-0.3.3a1/OPTIMA/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      132 2023-08-12 13:57:39.000000 optima_ml-0.3.3a1/OPTIMA/__main__.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-27 00:10:37.773362 optima_ml-0.3.3a1/OPTIMA/builtin/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      137 2024-02-07 21:12:40.000000 optima_ml-0.3.3a1/OPTIMA/builtin/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    35432 2024-04-27 00:05:49.000000 optima_ml-0.3.3a1/OPTIMA/builtin/evaluation.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    32098 2024-02-07 21:12:40.000000 optima_ml-0.3.3a1/OPTIMA/builtin/figures_of_merit.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    66758 2024-04-23 18:38:54.000000 optima_ml-0.3.3a1/OPTIMA/builtin/inputs.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      423 2024-04-17 06:54:34.000000 optima_ml-0.3.3a1/OPTIMA/builtin/model.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     2858 2024-04-27 00:05:49.000000 optima_ml-0.3.3a1/OPTIMA/builtin/search_space.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-27 00:10:37.773362 optima_ml-0.3.3a1/OPTIMA/core/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      114 2024-01-30 16:21:26.000000 optima_ml-0.3.3a1/OPTIMA/core/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    86145 2024-04-27 00:05:49.000000 optima_ml-0.3.3a1/OPTIMA/core/evaluation.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    19104 2024-04-23 18:38:54.000000 optima_ml-0.3.3a1/OPTIMA/core/inputs.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    10090 2024-04-17 06:54:34.000000 optima_ml-0.3.3a1/OPTIMA/core/model.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    41484 2024-04-27 00:05:49.000000 optima_ml-0.3.3a1/OPTIMA/core/search_space.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     3469 2024-04-23 18:38:54.000000 optima_ml-0.3.3a1/OPTIMA/core/tools.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    79732 2024-04-27 00:05:49.000000 optima_ml-0.3.3a1/OPTIMA/core/training.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    80230 2024-04-23 18:38:54.000000 optima_ml-0.3.3a1/OPTIMA/core/variable_optimization.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    17912 2024-04-27 00:05:49.000000 optima_ml-0.3.3a1/OPTIMA/defaults.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-27 00:10:37.773362 optima_ml-0.3.3a1/OPTIMA/hardware_configs/
+-rw-rw-r--   0 erik     (30000) erik     (30003)     2827 2024-04-27 00:05:47.000000 optima_ml-0.3.3a1/OPTIMA/hardware_configs/Dresden_Taurus.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      111 2024-01-30 16:21:26.000000 optima_ml-0.3.3a1/OPTIMA/hardware_configs/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    16772 2024-04-27 00:05:47.000000 optima_ml-0.3.3a1/OPTIMA/hardware_configs/common.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      505 2024-04-23 18:38:54.000000 optima_ml-0.3.3a1/OPTIMA/hardware_configs/helpers.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-27 00:10:37.773362 optima_ml-0.3.3a1/OPTIMA/helpers/
+-rw-rw-r--   0 erik     (30000) erik     (30003)       35 2024-01-30 16:21:26.000000 optima_ml-0.3.3a1/OPTIMA/helpers/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     4853 2024-01-30 16:21:26.000000 optima_ml-0.3.3a1/OPTIMA/helpers/extract_data_from_NTuples.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     8670 2024-04-23 18:38:54.000000 optima_ml-0.3.3a1/OPTIMA/helpers/manage_ray_nodes.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-27 00:10:37.773362 optima_ml-0.3.3a1/OPTIMA/keras/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-01-30 16:21:26.000000 optima_ml-0.3.3a1/OPTIMA/keras/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    28658 2024-04-27 00:05:49.000000 optima_ml-0.3.3a1/OPTIMA/keras/model.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    53862 2024-04-23 18:38:54.000000 optima_ml-0.3.3a1/OPTIMA/keras/tools.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     3912 2024-04-23 18:38:54.000000 optima_ml-0.3.3a1/OPTIMA/keras/training.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-27 00:10:37.777361 optima_ml-0.3.3a1/OPTIMA/lightning/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      106 2024-01-30 16:23:00.000000 optima_ml-0.3.3a1/OPTIMA/lightning/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    10100 2024-04-23 18:38:54.000000 optima_ml-0.3.3a1/OPTIMA/lightning/inputs.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     6301 2024-01-30 16:21:26.000000 optima_ml-0.3.3a1/OPTIMA/lightning/training.py
+-rwxrwxr-x   0 erik     (30000) erik     (30003)    98138 2024-04-27 00:05:49.000000 optima_ml-0.3.3a1/OPTIMA/optima.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-27 00:10:37.777361 optima_ml-0.3.3a1/OPTIMA/resources/
+-rw-rw-r--   0 erik     (30000) erik     (30003)        0 2023-08-12 13:57:39.000000 optima_ml-0.3.3a1/OPTIMA/resources/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     4772 2024-03-20 17:10:29.000000 optima_ml-0.3.3a1/OPTIMA/resources/config_verification.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    48922 2024-04-23 18:38:54.000000 optima_ml-0.3.3a1/OPTIMA/resources/pbt_with_seed.py
+-rw-r--r--   0 erik     (30000) erik     (30003)   117575 2024-04-27 00:10:37.777361 optima_ml-0.3.3a1/PKG-INFO
+-rw-rw-r--   0 erik     (30000) erik     (30003)   116177 2024-04-27 00:05:49.000000 optima_ml-0.3.3a1/README.md
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-27 00:10:37.777361 optima_ml-0.3.3a1/optima_ml.egg-info/
+-rw-r--r--   0 erik     (30000) erik     (30003)   117575 2024-04-27 00:10:37.000000 optima_ml-0.3.3a1/optima_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 erik     (30000) erik     (30003)     1342 2024-04-27 00:10:37.000000 optima_ml-0.3.3a1/optima_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)        1 2024-04-27 00:10:37.000000 optima_ml-0.3.3a1/optima_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-04-27 00:10:37.000000 optima_ml-0.3.3a1/optima_ml.egg-info/entry_points.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)      175 2024-04-27 00:10:37.000000 optima_ml-0.3.3a1/optima_ml.egg-info/requires.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)        7 2024-04-27 00:10:37.000000 optima_ml-0.3.3a1/optima_ml.egg-info/top_level.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)       38 2024-04-27 00:10:37.777361 optima_ml-0.3.3a1/setup.cfg
+-rw-rw-r--   0 erik     (30000) erik     (30003)     4231 2024-04-27 00:05:49.000000 optima_ml-0.3.3a1/setup.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-27 00:10:37.777361 optima_ml-0.3.3a1/tests/
+-rw-rw-r--   0 erik     (30000) erik     (30003)    34759 2024-04-27 00:05:49.000000 optima_ml-0.3.3a1/tests/test_builtin.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    25341 2024-04-27 00:05:49.000000 optima_ml-0.3.3a1/tests/test_core.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     6471 2024-04-27 00:05:49.000000 optima_ml-0.3.3a1/tests/test_integration.py
+-rw-rw-rw-   0 erik     (30000) erik     (30003)     6399 2023-11-02 02:48:49.000000 optima_ml-0.3.3a1/tests/test_integration_sameMachine.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    56852 2024-04-23 18:38:54.000000 optima_ml-0.3.3a1/tests/test_preprocessing.py
```

### Comparing `optima_ml-0.3.2a5.dev2/LICENSE` & `optima_ml-0.3.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/builtin/evaluation.py` & `optima_ml-0.3.3a1/OPTIMA/builtin/evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,18 +107,18 @@
             "testing model using {} training, {} validation and {} testing events".format(
                 inputs_train.shape[0], inputs_val.shape[0], inputs_test.shape[0]
             )
         )
 
     # create the output folders if they do not exist
     if not os.path.exists(fig_dir):
-        os.makedirs(fig_dir)
+        os.makedirs(fig_dir, exist_ok=True)
     if results_dir is not None:
         if not os.path.exists(results_dir):
-            os.makedirs(results_dir)
+            os.makedirs(results_dir, exist_ok=True)
 
     # load the model and get the model predictions
     model = OPTIMA.core.model.load_model(run_config, model_path, cpus)
     pred_train = model.predict(inputs_train, verbose=0)
     pred_val = model.predict(inputs_val, verbose=0)
     if explicit_testing_dataset:
         pred_test = model.predict(inputs_test, verbose=0)
```

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/builtin/figures_of_merit.py` & `optima_ml-0.3.3a1/OPTIMA/builtin/figures_of_merit.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/builtin/inputs.py` & `optima_ml-0.3.3a1/OPTIMA/builtin/inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -751,15 +751,15 @@
                 histtype="step",
                 density=True,
                 label=run_config.evaluation_class_labels,
             )
         ax.set_xlabel(var)
         ax.legend()
         if not os.path.exists(outdir):
-            os.makedirs(outdir)
+            os.makedirs(outdir, exist_ok=True)
         fig.savefig(os.path.join(outdir, "inputs_{}.pdf".format(var)))
         plt.close()
 
 
 train_val_splitting_type = tuple[Union[np.ndarray, list[np.ndarray]], Union[np.ndarray, list[np.ndarray]]]
 train_val_test_splitting_type = tuple[
     Union[np.ndarray, list[np.ndarray]], Union[np.ndarray, list[np.ndarray]], Union[np.ndarray, list[np.ndarray]]
```

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/builtin/search_space.py` & `optima_ml-0.3.3a1/OPTIMA/builtin/search_space.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/core/evaluation.py` & `optima_ml-0.3.3a1/OPTIMA/core/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,15 @@
     # if we are doing the evaluation for the PBT step, we want to skip the fit evaluation
     skip_fit_evaluation = PBT
 
     # check if evaluation was already done previously
     if not os.path.isfile(os.path.join(results_dir, "evaluation.pickle")):
         # create the results directory if not present
         if not os.path.exists(results_dir):
-            os.makedirs(results_dir)
+            os.makedirs(results_dir, exist_ok=True)
 
         # build a list containing the names of all metrics, grouped together like [[train_loss, val_loss], [train_accuracy, val_accuracy], ...]
         metric_names = []
         optimize_name_included = False
         for metric, _ in native_metrics + weighted_native_metrics + custom_metrics:
             group = ("train_" + metric, "val_" + metric)
             metric_names.append(group)
@@ -360,25 +360,26 @@
                 if trial_id in best_trial:
                     model_config_to_evaluate[
                         "trial_id"
                     ] = trial_id  # best_trail is full path to the optimization folder while trails in trial_list as only the names
                     break
             model_configs_to_evaluate.append(model_config_to_evaluate)
 
-            # round the config where necessary (in the same way as during the optimization), and add the hyperparameters to
-            # the dataframe containing the configs of the best trials
+            # Add the hyperparameters to the dataframe containing the configs of the best trials. For hierarchical
+            # search spaces, not all hyperparameters must have a value, so insert "-" for those
             model_config = model_configs_to_evaluate[-1]
             for hp in model_configs_df.index:
-                model_configs_df.loc[hp, metric] = model_config[hp]
+                hp_value = model_config.get(hp)
+                model_configs_df.loc[hp, metric] = hp_value if hp_value is not None else "-"
 
             # create the target folder for the following crossvalidation
             target_folder = os.path.join(results_dir, metric if len(best_trials.index) > 1 else "", "best_value")
             dirs_to_evaluate.append(target_folder)  # mark target_folder to be evaluated later
             if not os.path.exists(target_folder):
-                os.makedirs(target_folder)
+                os.makedirs(target_folder, exist_ok=True)
 
         # then the results from the fit
         if not skip_fit_evaluation:
             for metric, best_trial, best_epoch in zip(
                 best_trials_fit.index,
                 best_trials_fit["trial"],
                 best_trials_fit["best epoch"],
@@ -390,19 +391,20 @@
                         model_config_to_evaluate[
                             "trial_id"
                         ] = trial_id  # best_trail is full path to the optimization folder while trails in trial_list as only the names
                         break
                 model_configs_to_evaluate.append(model_config_to_evaluate)
                 model_config = model_configs_to_evaluate[-1]
                 for hp in model_configs_df.index:
-                    model_configs_df.loc[hp, f"{metric} fit"] = model_config[hp]
+                    hp_value = model_config.get(hp)
+                    model_configs_df.loc[hp, f"{metric} fit"] = hp_value if hp_value is not None else "-"
                 target_folder = os.path.join(results_dir, metric if len(best_trials_fit.index) > 1 else "", "best_fit")
                 dirs_to_evaluate.append(target_folder)  # mark target_folder to be evaluated later
                 if not os.path.exists(target_folder):
-                    os.makedirs(target_folder)
+                    os.makedirs(target_folder, exist_ok=True)
 
         optimization_results_string += tabulate.tabulate(
             model_configs_df,
             headers=[model_configs_df.index.name] + list(model_configs_df.columns),
             tablefmt="fancy_grid",
         )
         print("\n" + optimization_results_string)
@@ -911,15 +913,15 @@
         plt.xlabel("iterations")
         plt.legend()
         plt.gcf().set_figheight(6)
         plt.gcf().set_figwidth(8)
         plt.tight_layout()
         if figs_dir is not None:
             if not os.path.exists(os.path.join(figs_dir, "overview_plots")):
-                os.makedirs(os.path.join(figs_dir, "overview_plots"))
+                os.makedirs(os.path.join(figs_dir, "overview_plots"), exist_ok=True)
             plt.savefig(os.path.join(figs_dir, "overview_plots", "{}.png".format("+".join(metric_group))), dpi=600)
         else:
             plt.show()
         plt.clf()
 
     # extract only those epochs that improved the optimization metrics
     for target_metric, target_op in zip(optimize_name, optimize_op):
@@ -952,15 +954,15 @@
             plt.xlabel("iterations")
             plt.legend()
             plt.gcf().set_figheight(6)
             plt.gcf().set_figwidth(8)
             plt.tight_layout()
             if figs_dir is not None:
                 if not os.path.exists(os.path.join(figs_dir, "progress_plots")):
-                    os.makedirs(os.path.join(figs_dir, "progress_plots"))
+                    os.makedirs(os.path.join(figs_dir, "progress_plots"), exist_ok=True)
                 plt.savefig(
                     os.path.join(
                         figs_dir,
                         "progress_plots",
                         target_metric if len(optimize_name) > 1 else "",
                         "{}.png".format("+".join(metric_group)),
                     ),
@@ -1084,15 +1086,16 @@
                     os.makedirs(
                         os.path.join(
                             figs_dir,
                             target_metric_name if len(optimize_name) > 1 else "",
                             "best_value",
                             "plots",
                             "optimization",
-                        )
+                        ),
+                        exist_ok=True,
                     )
                 plt.savefig(
                     os.path.join(
                         figs_dir,
                         target_metric_name if len(optimize_name) > 1 else "",
                         "best_value",
                         "plots",
@@ -1659,15 +1662,15 @@
                         label = f"{metric_name} fit" if i == 0 else None
                         plt.plot(iterations, metrics, color=color, alpha=alpha, label=label)
                 else:
                     plt.plot(df_for_plotting["training_iteration"], df_for_plotting[metric_name], color=color)
 
                 if figs_dir is not None:
                     if not os.path.exists(figs_dir):
-                        os.makedirs(figs_dir)
+                        os.makedirs(figs_dir, exist_ok=True)
                     plt.gcf().set_figheight(6)
                     plt.gcf().set_figwidth(8)
                     plt.tight_layout()
                     plt.savefig(figs_dir, dpi=600)
                     plt.clf()
             return best_epoch_fit, best_checkpoint_fit, best_metric_fit
         else:
@@ -1700,15 +1703,15 @@
                         df_for_plotting[metric_name],
                         color=color,
                         label=f"{metric_name} fit",
                     )
 
                 if figs_dir is not None:
                     if not os.path.exists(figs_dir):
-                        os.makedirs(figs_dir)
+                        os.makedirs(figs_dir, exist_ok=True)
                     plt.gcf().set_figheight(6)
                     plt.gcf().set_figwidth(8)
                     plt.tight_layout()
                     plt.savefig(figs_dir, dpi=600)
                     plt.clf()
             return fitted_func(return_at_x)
 
@@ -1805,15 +1808,16 @@
                     os.makedirs(
                         os.path.join(
                             figs_dir,
                             target_metric_name if len(optimize_name) > 1 else "",
                             "best_fit",
                             "plots",
                             "optimization",
-                        )
+                        ),
+                        exist_ok=True,
                     )
                 plt.savefig(
                     os.path.join(
                         figs_dir,
                         target_metric_name if len(optimize_name) > 1 else "",
                         "best_fit",
                         "plots",
```

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/core/inputs.py` & `optima_ml-0.3.3a1/OPTIMA/core/inputs.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/core/model.py` & `optima_ml-0.3.3a1/OPTIMA/core/model.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/core/search_space.py` & `optima_ml-0.3.3a1/OPTIMA/core/search_space.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
 """A module that provides general functionality to handle the hyperparameter search space."""
-from typing import Union, Optional, Callable, Any
+from typing import Union, Optional, Callable, Any, Literal
 
 import numpy as np
+import scipy
 import dill
 
+import optuna
 from ray import tune
 
 import OPTIMA.core.tools
 
 run_config_search_space_entry_type = Union[int, float, str, list, tuple, dict]
 
 tune_search_space_entry_type = Union[
@@ -27,30 +29,53 @@
 ]
 
 PBT_search_space_type = dict[
     str, Union[tune.search.sample.Float, tune.search.sample.Integer, tune.search.sample.Categorical, list, dict]
 ]
 
 
-def _get_range_search_space_properties(hp_name, hp_value, optuna=False):
-    """_summary_.
+def _get_range_search_space_properties(
+    hp_name: str, hp_value: dict, optuna: bool = False
+) -> tuple[
+    list, str, str, Union[int, float, Literal[None]], Union[int, float, Literal[None]], Union[int, float, Literal[None]]
+]:
+    """Helper function to extract relevant information from a ``'range'`` search space entry in the run-config format.
+
+    This function enforces the following conditions:
+
+    - a ``'bounds'`` entry is provided as a list of length two, with ``bounds[0] <= bounds[1]``
+    - a ``'value_type'`` entry can only have values ``'int'`` and ``'float'``
+    - a ``'value_type'`` entry can only have values ``'uniform'``, ``'log'`` and ``'normal'``
+    - for integer search spaces, the ``'step'`` value must be an integer (or an integer represented as a float, e.g. ``2.0``)
+    - for integer search spaces with log sampling, ``'step'`` can only be 1 when using Optuna
+    - ``'mean'`` and ``'std'`` need to be provided for normal-sampled search spaces
+    - normal sampled integer search spaces are not supported
+
+    The following default values are set for vacant search space entries:
+
+    - ``'value_type'``: ``'float'``
+    - ``'sampling'``: ``'uniform'``
+    - ``'step'``: ``None``
 
     Parameters
     ----------
-    hp_name : _type_
-        _description_
-    hp_value : _type_
-        _description_
-    optuna : _type_
-        _description_ (Default value = False)
+    hp_name : str
+        Name of the ``'range'`` hyperparameter in the search space.
+    hp_value : dict
+        Corresponding search space entry.
+    optuna : bool
+        Indicates if Optuna is used for the hyperparameter optimization. (Default value = False)
 
     Returns
     -------
-    _type_
-        _description_
+    tuple[list, str, str, Union[int, float, Literal[None]], Union[int, float, Literal[None]], Union[int, float, Literal[None]]]
+        A list containing the lower and upper bounds of the hyperparameter, either ``'int'`` or ``'float'`` describing
+        the type of hyperparameter value, a string describing the desired sampling of the search space (``'uniform'``,
+        ``'log'`` or ``'normal'``), and optional step size for quantization (``None`` if unquantized), an optional mean
+        and standard deviation values for ``'normal'`` search spaces (both ``None`` for other samplings).
     """
     assert "bounds" in hp_value.keys(), "Bounds need to be provided for search space entry of type 'range'!"
     bounds = hp_value["bounds"]
 
     # gather properties of this search space entry and set defaults for vacant entries
     if hp_value.get("value_type") is not None:
         assert hp_value["value_type"] in [
@@ -70,17 +95,17 @@
     else:
         sampling = "uniform"
     if hp_value.get("step") is not None:
         if value_type == "int" and int(hp_value["step"]) != hp_value["step"]:
             raise ValueError(
                 f"A step value of {hp_value['step']} is not possible for integer search space of {hp_name}!"
             )
-        if value_type == "int" and sampling == "log" and hp_value.get("step") != 1 and optuna:
+        if sampling == "log" and optuna:
             raise ValueError(
-                "Optuna does not support integer log sampling with step != 1. Set step to 1 or sampling to 'uniform'."
+                "Optuna does not support discrete log sampling. Set step to None or sampling to 'uniform'."
             )
         step = hp_value["step"]
     else:
         step = None
     if sampling == "normal":
         if value_type == "int":
             raise ValueError(f"Integer normal search space of {hp_name} is not supported by Tune!")
@@ -91,30 +116,48 @@
         std = hp_value["std"]
     else:
         mean, std = None, None
 
     return bounds, value_type, sampling, step, mean, std
 
 
-def _build_search_space_properties(hp_name, hp_value, optuna=False):
-    """_summary_.
+def _build_search_space_properties(hp_name: str, hp_value: dict, optuna: bool = False) -> tuple[str, tuple]:
+    """Helper function to extract relevant information from a search space entry in the run-config format.
+
+    If the search space value is not a dictionary, the hyperparameter is considered fixed to the provided value and
+    returned, together with the search space type ``'fixed'``. Otherwise, a distinction is made between ``'range'``
+    and ``'choice'`` parameters. For ``'range'`` parameters, the ``_get_range_search_space_properties``-function is
+    called to retrieve relevant information. The obtained properties are returned together with the search space type
+    ``'range'``. For ``'choice'``-parameters, a ``'values'``-entry is asserted to be present in the search space entry,
+    which is returned together with the search space type ``'choice'``.
+
+    Since the ``'bounds'`` entry is only used for ``'range'``-parameters and the ``'values'``-entry is only used for
+    choice parameters, the presence of these entries is also used to infer if the search space type is ``'range'`` or
+    ``'choice'``, thus making the ``'type'`` entry optional.
 
     Parameters
     ----------
-    hp_name : _type_
-        _description_
-    hp_value : _type_
-        _description_
-    optuna : _type_
-        _description_ (Default value = False)
+    hp_name : str
+        Name of the ``'range'`` hyperparameter in the search space.
+    hp_value : dict
+        Corresponding search space entry.
+    optuna : bool
+        Indicates if Optuna is used for the hyperparameter optimization. (Default value = False)
 
     Returns
     -------
-    _type_
-        _description_
+    tuple[str, tuple]
+        The first return value describes the type of search space, either ``'fixed'``, ``'range'`` or ``'choice'``. The
+        second return value is a tuple of all relevant information. For a fixed hyperparameter, this is the value set
+        in the run-config. For a choice parameter, this is the value provided as ``'values'``. For a range parameter,
+        this is a tuple containing a list with the lower and upper bounds of the hyperparameter, either ``'int'`` or
+        ``'float'`` describing the type of hyperparameter value, a string describing the desired sampling of the search
+        space (``'uniform'``, ``'log'`` or ``'normal'``), an optional step size for quantization (``None`` if
+        unquantized), and optional mean and standard deviation values for ``'normal'`` search spaces (both ``None``
+        for other samplings).
     """
     # first check if hyperparameter is fixed
     if not isinstance(hp_value, dict):
         search_space_type = "fixed"
         search_space_entry = hp_value
     else:
         # check if it is a range or choice parameter; this can be given via the "type" option or inferred from the
@@ -132,26 +175,40 @@
             search_space_entry = hp_value["values"]
         else:
             raise ValueError(f"Unsupported search space type for hyperparameter {hp_name}: {hp_value}")
 
     return search_space_type, search_space_entry
 
 
-def serialize_conditions(search_space: dict[str, run_config_search_space_entry_type]):
-    """_summary_.
+def serialize_conditions(
+    search_space: dict[str, run_config_search_space_entry_type]
+) -> dict[str, run_config_search_space_entry_type]:
+    """A helper function that serializes all callables in the search space to a string representation.
+
+    Since the search space needs to be serializable with ``pickle``, it must not contain any callables. However, since
+    conditions are described via callables in the run-config, these need to be explicitly serialized beforehand.
+
+    Callables, i.e. conditions, are only expected as the second arguments of the ``'bounds'``, ``'values'`` and ``'only'``
+    entries for each search space entry. If a callable is detected, it is translated into a bytestring using
+    ``dill.dumps()``, and added to the search space in place of the callable. When suggesting hyperparameters, this
+    representation can be translated back into the original callable to evaluate the condition.
+
+    This function does not alter the original provided search space. Instead, it returns a copy with the callables
+    replaced by their bytestring representations.
 
     Parameters
     ----------
     search_space : dict[str, run_config_search_space_entry_type]
-        _description_
+        The search space in the run-config format.
 
     Returns
     -------
-    _type_
-        _description_
+    dict[str, run_config_search_space_entry_type]
+        A copy of the provided search space, with the callables replaced by their bytestring representations obtained
+        using ``dill.dumps()``.
     """
     serialized_search_space = search_space.copy()
     for hp_name, hp_value in search_space.items():
         if isinstance(hp_value, dict):
             serialized_hp_value = hp_value.copy()
             if "bounds" in hp_value.keys() and callable(hp_value["bounds"][1]):
                 bounds_hps, bounds_callable = hp_value["bounds"]
@@ -162,34 +219,48 @@
             if "only" in hp_value.keys():
                 only_hps, only_callable = hp_value["only"]
                 serialized_hp_value["only"] = (only_hps, dill.dumps(only_callable))
             serialized_search_space[hp_name] = serialized_hp_value
     return serialized_search_space
 
 
-def build_tune_search_space(search_space: dict[str, run_config_search_space_entry_type]) -> tune_search_space_type:
+def build_tune_search_space(
+    search_space: dict[str, run_config_search_space_entry_type],
+    PBT: Optional[bool] = False,
+) -> tune_search_space_type:
     """Translates the search space format from the run-config to a Tune search space.
 
     Since Tune does not support conditional search spaces, a ``ValueError`` will be raised if a conditional search space
     is provided.
 
     Parameters
     ----------
     search_space : dict[str, run_config_search_space_entry_type]
         The search space in the format used in the run-config.
+    PBT : bool
+        Since Population Based Training expects lists instead of a tune.search.sample.Categorical-instance, will not
+        convert search space entries of type ``'choice'``. Instead, the ``'values'``-entry is returned directly.
 
     Returns
     -------
     tune_search_space_type
         The search space to be provided to Tune.
     """
     # verify the search space is not conditional
     for _, hp_value in search_space.items():
-        if isinstance(hp_value, dict) and "only" in hp_value.keys():
-            raise ValueError("Tune does not support conditional search spaces!")
+        if isinstance(hp_value, dict):
+            is_conditional = False
+            if "only" in hp_value.keys():
+                is_conditional = True
+            elif "bounds" in hp_value.keys() and callable(hp_value["bounds"][1]):
+                is_conditional = True
+            elif "values" in hp_value.keys() and callable(hp_value["values"][1]):
+                is_conditional = True
+            if is_conditional:
+                raise ValueError("Tune does not support conditional search spaces!")
 
     # build the tune search space
     tune_search_space = {}
     for hp_name, hp_value in search_space.items():
         # get the search space properties, i.e. a set of options that are needed to specify the search space entry.
         # Vacant options are populated with default values
         search_space_type, search_space_properties = _build_search_space_properties(hp_name, hp_value)
@@ -226,52 +297,195 @@
                 if step != 1:
                     tune_search_space[hp_name] = tune.qlograndint(
                         bounds[0], bounds[1], step
                     )  # upper bound is inclusive if step != 1
                 else:
                     tune_search_space[hp_name] = tune.lograndint(bounds[0], bounds[1] + 1)
         elif search_space_type == "choice":
-            tune_search_space[hp_name] = tune.choice(search_space_properties)
+            if PBT:
+                tune_search_space[hp_name] = list(search_space_properties)
+            else:
+                tune_search_space[hp_name] = tune.choice(search_space_properties)
         else:
             raise RuntimeError(f"Unknown search space type {search_space_type}.")
 
     return tune_search_space
 
 
-def optuna_search_space(search_space: dict[str, run_config_search_space_entry_type], trial):
-    """_summary_.
+def _transform_uniform_to_normal(
+    x: Union[int, float], mean: Union[int, float], std: Union[int, float], step: Optional[Union[int, float]] = None
+) -> float:
+    """Helper function to transform a uniformly distributed to a normally distributed random variable with provided mean and width.
+
+    The relationship between the two distributions is given by the Gaussian probability point function. The calculation
+    is done using Scipy's ``scipy.stats.norm.ppf``.
+
+    The result is optionally quantized to the nearest multiple of ``step``.
+
+    Parameters
+    ----------
+    x : Union[int, float]
+        The uniformly distributed random variable to transform to a normal.
+    mean : Union[int, float]
+        The mean of the normal distribution.
+    std : Union[int, float]
+        The standard deviation of the normal distribution.
+    step : Optional[Union[int, float]]
+        An optional step size to use for quantization. (Default value = None)
+
+    Returns
+    -------
+    float
+        The corresponding value of the normally distributed random variable.
+    """
+    y = scipy.stats.norm.ppf(x, loc=mean, scale=std)
+    if step is not None:
+        y = np.round(y / step) * step  # round to nearest multiple of step
+    return y
+
+
+def _optuna_suggest_normal(
+    trial: optuna.trial.Trial,
+    hp_name: str,
+    mean: Union[int, float],
+    std: Union[int, float],
+    step: Optional[Union[int, float]] = None,
+) -> float:
+    """Helper function to suggest a normally distributed variable with Optuna.
+
+    Since Optuna does not natively support normal distributions, we instead need to sample from a uniform distribution
+    and transform the value using the inverse CDF, i.e. the probability point function, to get from a quantile to the
+    corresponding value.
+
+    If a step size is provided resulting value is quantized by rounding to the nearest multiple of ``step``.
+
+    As a side-effect of the uniform suggestion, a new hyperparameter will be added to the trial. As the name, the
+    provided hyperparameter name with an ``'internal_'`` prefix is used to distinguish this hyperparameter from the
+    others.
+
+    Parameters
+    ----------
+    trial : optuna.trial.Trial
+        The Optuna trial for which a normally distributed hyperparameter value should be suggested.
+    hp_name : str
+        The name of the hyperparameter.
+    mean : Union[int, float]
+        The mean of the normal distribution.
+    std : Union[int, float]
+        The standard deviation of the normal distribution.
+    step : Optional[Union[int, float]]
+        An optional step size to use for quantization. (Default value = None)
+
+    Returns
+    -------
+    float
+        The value of the normally distributed hyperparameter.
+    """
+    temp_uniform = None
+    while temp_uniform is None or temp_uniform == 0 or temp_uniform == 1:  # make sure 0 and 1 are excluded!
+        temp_uniform = trial.suggest_float(f"internal_{hp_name}", 0, 1)
+    y_normal = _transform_uniform_to_normal(temp_uniform, mean, std, step)
+
+    return y_normal
+
+
+def optuna_search_space(search_space: dict[str, run_config_search_space_entry_type], trial: optuna.trial.Trial) -> dict:
+    """Suggests new hyperparameters using Optuna's define-by-run API for serialized conditional search spaces in the run-config format.
+
+    This function supports conditional hyperparameter bounds for range parameters and conditional values for choice
+    parameters, allowing to constrain the possible values of a hyperparameter based on other hyperparameter values.
+    Additionally, hierarchical search spaces can be build using the ``'only'`` value, allowing a hyperparameter to only
+    be suggested if a condition is fulfilled.
+
+    Since this function needs to be serializable, the conditions in the provided search space are expected to be converted
+    to their bytestring representations using ``dill``. As such, a value of type ``bytes`` as the second entry of a
+    ``'bounds'`` or ``'values'`` entry is interpreted as an encoded callable.
+
+    Since hyperparameters are not independent anymore for conditional and hierarchical search spaces, the order of the
+    hyperparameter suggestions matters. In particular, while the final set of suggested hyperparameters does not depend
+    on the order they were suggested, the conditions prevent certain orders from being evaluable. As an example, if
+    values for three hyperparameters `a`, `b` and `c` are to be suggested, where `a` and `b` depend on the value of `c`,
+    allowed orders of evaluation are `c`, `a`, `b` and `c`, `b`, `a`. Since `a` and `b` are independent with respect to
+    each other, their respective order does not influence the suggested values. Any other order, however, is obviously
+    forbidden.
+
+    To solve the conditional, hierarchical hyperparameter space, the following order is used:
+
+    1. Suggest values for all non-conditional hyperparameters. These are hyperparameters whose search space does not
+       contain an ``'only'``-entry and whose ``'bounds'`` or ``'values'`` entry (if present) is not conditional.
+    2. In an arbitrary order, iterate over the remaining hyperparameters and check if the hyperparameter's
+       ``'only'``-condition is evaluable (i.e. values have been suggested for all hyperparameters that the
+       ``'only'``-condition depends on). If this is not the case, continue to the next remaining hyperparameter. If the
+       ``'only'``-condition is evaluable, evaluate it. If it returns as ``False``, i.e. this hyperparameter is not needed,
+       remove it from the list of remaining hyperparameters and continue to the next remaining hyperparameter. If a
+       hyperparameter does not have an ``'only'``-condition, it is considered to be ``True``. If the ``'only'``-condition
+       is ``True``, check if this hyperparameter's conditional ``'bounds'`` or ``'values'`` can be evaluated.  If this is
+       not the case, continue to the next remaining hyperparameter. If a hyperparameter does not have conditional
+       ``'bounds'`` or ``'values'``, they are (of cause) considered evaluable. Finally, suggest a value for this
+       hyperparameter and continue to the next remaining hyperparameter.
+    3. Iteratively repeat step 2 until a value has been suggested for all hyperparameters. If no new hyperparameter value
+       is suggested during an iteration, this indicates a circular condition which is not resolvable, and a ``ValueError``
+       is raised.
+
+    An additional layer of complexity arises if hyperparameters depend on hyperparameters with an ``'only'``-condition.
+    As an example, assume hyperparameter B depends on hyperparameter A with the ``'only'``-condition ``A > 0.5``, and
+    hyperparameter C depends on B with the ``'only'``-condition ``B > 0.5``. For the suggestion ``A = 0``, the value of
+    B is undefined, thus C's ``'only'``-condition cannot be evaluated. The same situation arises if the value of C depends
+    on the value of B. To let the user decide on how to deal with such a scenario, the value of a hyperparameter
+    whose ``'only'``-condition was evaluated as ``False`` is set to ``None``, so that it can be provided to the other
+    hyperparameter's conditions. In the example, the ``'only'``-condition of C could for example be adjusted to
+    ``B is not None and B > 0.5`` or ``B is None or B > 0.5``, depending on the intentions. Similarly, if the value of
+    C depends on the value of B, one could either define a default range like ``[B, 3] if B is not None else [0, 3]`` or
+    add an ``'only'``-condition ``B is not None``.
 
     Parameters
     ----------
     search_space : dict[str, run_config_search_space_entry_type]
-        _description_
-    trial : _type_
-        _description_
+        The search space in the run-config format, with callables represented as bytestrings.
+    trial : optuna.trial.Trial
+        The Optuna trial for which hyperparameters should be suggested.
 
     Returns
     -------
-    _type_
-        _description_
+    dict
+        A dictionary of fixed hyperparameters. This is expected by Optuna's define-by-run API.
     """
     # split search space entries into conditional and non-conditional entries and extract the search space properties
     conditional_search_space = {}
     non_conditional_search_space = {}
     for hp_name, serialized_hp_value in search_space.items():
         # assign to conditional and non-conditional sub-search space dicts; serialized callables are bytes instances
         # collect a list of hyperparameters that is needed to check if hp is necessary, and a second list of hps that is
         # needed to decide on a value
         only_depends_hps = []
         value_depends_hps = []
         if isinstance(serialized_hp_value, dict):
+            # when gathering the depends_hps, also allow the first entry to be a string instead of a tuple or list,
+            # and assume that is the name of a single hyperparameter
             if "bounds" in serialized_hp_value.keys() and isinstance(serialized_hp_value["bounds"][1], bytes):
-                value_depends_hps += list(serialized_hp_value["bounds"][0])
+                this_depends_hps = serialized_hp_value["bounds"][0]
+                if isinstance(this_depends_hps, str):
+                    this_depends_hps = [
+                        this_depends_hps,
+                    ]
+                value_depends_hps += list(this_depends_hps)
             if "values" in serialized_hp_value.keys() and isinstance(serialized_hp_value["values"][1], bytes):
-                value_depends_hps += list(serialized_hp_value["values"][0])
+                this_depends_hps = serialized_hp_value["values"][0]
+                if isinstance(this_depends_hps, str):
+                    this_depends_hps = [
+                        this_depends_hps,
+                    ]
+                value_depends_hps += list(this_depends_hps)
             if "only" in serialized_hp_value.keys():
-                only_depends_hps += list(serialized_hp_value["only"][0])
+                this_depends_hps = serialized_hp_value["only"][0]
+                if isinstance(this_depends_hps, str):
+                    this_depends_hps = [
+                        this_depends_hps,
+                    ]
+                only_depends_hps += list(this_depends_hps)
 
         # check if there are any dependencies
         if len(only_depends_hps) + len(value_depends_hps) == 0:
             # get the search space properties, i.e. a set of options that are needed to specify the search space entry.
             # Vacant options are populated with default values
             search_space_type, search_space_properties = _build_search_space_properties(
                 hp_name, serialized_hp_value, optuna=True
@@ -295,62 +509,87 @@
         elif hp_type == "range":
             bounds, value_type, sampling, step, mean, std = hp_properties
             if value_type == "int":
                 suggested_hps[hp_name] = trial.suggest_int(
                     hp_name, bounds[0], bounds[1], step=1 if step is None else step, log=sampling == "log"
                 )
             elif value_type == "float":
-                suggested_hps[hp_name] = trial.suggest_float(
-                    hp_name, bounds[0], bounds[1], step=step, log=sampling == "log"
-                )
+                if sampling != "normal":
+                    suggested_hps[hp_name] = trial.suggest_float(
+                        hp_name, bounds[0], bounds[1], step=step, log=sampling == "log"
+                    )
+                else:
+                    # Optuna does not natively support normal sampling, so calculate a normally distributed variable from
+                    # a transformed, uniformly distributed variable. Since this is not added to the trial suggestions,
+                    # add it to the fixed hps instead, as these are also provided to Tune.
+                    fixed_hps[hp_name] = _optuna_suggest_normal(trial, hp_name, mean, std, step)
         elif hp_type == "choice":
             suggested_hps[hp_name] = trial.suggest_categorical(hp_name, hp_properties)
         else:
             raise RuntimeError(f"Unknown search space type {hp_type}.")
 
     # try to iteratively build conditional hyperparameters (as some conditional hyperparameters can depend on
-    # other conditional hyperparameters
+    # other conditional hyperparameters.
     cond_hps_to_solve = list(conditional_search_space.keys())
     while len(cond_hps_to_solve) > 0:
         # to check at the end of the iteration if we could solve anything, otherwise break and raise an error
         num_left = len(cond_hps_to_solve)
 
         # Iterate over remaining conditional hyperparameters
         for hp_name in cond_hps_to_solve:
             only_depends_hps, value_depends_hps, serialized_hp_value = conditional_search_space[hp_name]
 
+            # check if all depends_hps are actually in the search space
+            for hp_depends in only_depends_hps + value_depends_hps:
+                if hp_depends not in search_space.keys():
+                    raise ValueError(
+                        f"Hyperparameter '{hp_name}' depends on the value of '{hp_depends}', which is not "
+                        f"part of the search space."
+                    )
+
             # See if we can evaluate if hyperparameter is needed
             if len(only_depends_hps) > 0:
                 only_depends_values = {
                     only_depends_hp: suggested_hps[only_depends_hp]
                     if only_depends_hp in suggested_hps.keys()
                     else fixed_hps[only_depends_hp]
                     if only_depends_hp in fixed_hps.keys()
-                    else None
+                    else np.nan
                     for only_depends_hp in only_depends_hps
                 }
-                if not any(only_depends_value is None for only_depends_value in only_depends_values.values()):
+
+                # None cannot be checked with np.isnan, so explicitly exclude it first
+                if not any(
+                    only_depends_value is not None and np.isnan(only_depends_value)
+                    for only_depends_value in only_depends_values.values()
+                ):
                     # evaluate the only condition
                     only_hps, serialized_only_callable = serialized_hp_value["only"]
                     need_hp = dill.loads(serialized_only_callable)(*[only_depends_values[h] for h in only_hps])
+                else:
+                    # we can't evaluate this only condition yet. Check the next remaining hyperparameter.
+                    continue
             else:
                 # no only condition, so we always need this hyperparameter
                 need_hp = True
 
             if need_hp:
                 # if this hyperparameter is needed, check if we can decide on its value
                 value_depends_values = {
                     value_depends_hp: suggested_hps[value_depends_hp]
                     if value_depends_hp in suggested_hps.keys()
                     else fixed_hps[value_depends_hp]
                     if value_depends_hp in fixed_hps.keys()
-                    else None
+                    else np.nan
                     for value_depends_hp in value_depends_hps
                 }
-                if not any(value_depends_value is None for value_depends_value in value_depends_values.values()):
+                if not any(
+                    value_depends_value is not None and np.isnan(value_depends_value)
+                    for value_depends_value in value_depends_values.values()
+                ):
                     # we can decide on this hyperparameter's value, so remove it from the list of remaining hyperparameters
                     cond_hps_to_solve.remove(hp_name)
 
                     # deserialize the hyperparameter search space entry
                     hp_value = serialized_hp_value.copy()
                     if "bounds" in serialized_hp_value.keys() and isinstance(serialized_hp_value["bounds"][1], bytes):
                         bounds_hps, serialized_bounds_callable = serialized_hp_value["bounds"]
@@ -374,47 +613,58 @@
                     elif search_space_type == "range":
                         bounds, value_type, sampling, step, mean, std = search_space_properties
                         if value_type == "int":
                             suggested_hps[hp_name] = trial.suggest_int(
                                 hp_name, bounds[0], bounds[1], step=1 if step is None else step, log=sampling == "log"
                             )
                         elif value_type == "float":
-                            suggested_hps[hp_name] = trial.suggest_float(
-                                hp_name, bounds[0], bounds[1], step=step, log=sampling == "log"
-                            )
+                            if sampling != "normal":
+                                suggested_hps[hp_name] = trial.suggest_float(
+                                    hp_name, bounds[0], bounds[1], step=step, log=sampling == "log"
+                                )
+                            else:
+                                # Optuna does not natively support normal sampling, so calculate a normally distributed variable from
+                                # a transformed, uniformly distributed variable. Since this is not added to the trial suggestions,
+                                # add it to the fixed hps instead, as these are also provided to Tune.
+                                fixed_hps[hp_name] = _optuna_suggest_normal(trial, hp_name, mean, std, step)
                     elif search_space_type == "choice":
                         suggested_hps[hp_name] = trial.suggest_categorical(hp_name, search_space_properties)
                     else:
                         raise RuntimeError(f"Unknown search space type {hp_type}.")
                 else:
-                    # condition is False, thus just skip the suggestion
+                    # we can't evaluate the value condition yet, so continue to the next remaining hyperparameter
                     continue
             else:
-                # we don't need this hyperparameter, so drop it from the list of remaining hyperparameters
+                # we don't need this hyperparameter, so suggest a value of None, add it to the list of suggested
+                # hyperparameters and drop it from the list of remaining hyperparameters. This way, stacked conditions
+                # can be resolved properly as the user gets to decide what to do with hyperparameters that depend on a
+                # hyperparameter that was rejected.
                 cond_hps_to_solve.remove(hp_name)
+                suggested_hps[hp_name] = None
 
-            # check if we actually resolved any new hyperparameter
-            if len(cond_hps_to_solve) == num_left:
-                raise ValueError("Conditional search space contains circular conditions that cannot be resolved.")
+        # check if we actually resolved any new hyperparameter
+        if len(cond_hps_to_solve) == num_left:
+            raise ValueError("Conditional search space contains circular conditions that cannot be resolved.")
 
     return fixed_hps
 
 
 def prepare_search_space_for_PBT(
     search_space: dict[str, run_config_search_space_entry_type], best_hp_values_optuna: Optional[dict] = None
 ) -> tuple[tune_search_space_type, tune_search_space_type]:
     """Builds the search space for the optimization with Population Based Training.
 
     All hyperparameters that are not marked with 'supports_mutation' are fixed to the best values found during the
     previous optimization step. If no previous optimization was performed, all hyperparameters in the search space need
-    to be mutatable, otherwise an error is raised. The resulting search space is then translated to a Tune search space
-    by calling ``build_tune_search_space``.
+    to be mutatable or fixed, otherwise an error is raised. The resulting search space is then translated to a Tune
+    search space by calling ``build_tune_search_space``.
 
-    Since the ``PopulationBasedTraining``-scheduler needs a search space that does not contain fixed values, a second
-    dictionary with the fixed hyperparameter values removed is returned.
+    Since the ``PopulationBasedTraining``-scheduler needs a search space that does not contain fixed values and expects
+    lists instead of tune.search.sample.Categorical-instances, a second dictionary with the fixed hyperparameter values
+    removed and unconverted ``'choice'`` search space entries is returned.
 
     Parameters
     ----------
     search_space : dict[str, run_config_search_space_entry_type]
         The search space as defined in the run-config.
     best_hp_values_optuna : Optional[dict]
         A dictionary containing the best hyperparameter values found during a previous optimization step. (Default value = None)
@@ -425,57 +675,49 @@
         The Tune search space with non-mutatable hyperparameters fixed to their best value and the pruned Tune search
         space, containing only mutatable hyperparameters, which is to be provided to the
         ``PopulationBasedTraining``-scheduler.
     """
     # extract the hyperparameters that are marked with "supports_mutation"
     mutatable_hps = []
     non_mutatable_hps = []
+    fixed_hps = []
     for hp_name, hp_value in search_space.items():
         if isinstance(hp_value, dict) and "supports_mutation" in hp_value.keys() and hp_value["supports_mutation"]:
             mutatable_hps.append(hp_name)
-        else:
+        elif isinstance(hp_value, dict):
             non_mutatable_hps.append(hp_name)
+        else:
+            fixed_hps.append(hp_name)
 
+    # create two variants of the search space, once with only the mutatable hyperparameters and once also with
+    # the fixed best values; for now, only fill the fixed hyperparameters that were fixed from the start
+    search_space_mutatable = {hp_name: search_space[hp_name] for hp_name in mutatable_hps}
+    search_space_with_fixed = {hp_name: search_space[hp_name] for hp_name in mutatable_hps}
+    search_space_with_fixed.update({hp_name: search_space[hp_name] for hp_name in fixed_hps})
+
+    # decide on what to do with non-mutatable, non-fixed hyperparameters
     if best_hp_values_optuna is not None:
-        # create the two variants of the search space, only with only the mutatable hyperparameters and once also with
-        # the fixed best values
-        search_space_with_fixed = {}
-        search_space_mutatable = {}
-        for hp_name, hp_value in search_space.items():
-            if hp_name in mutatable_hps:
-                # add the mutatable hyperparameter to both search spaces
-                search_space_mutatable[hp_name] = hp_value
-                search_space_with_fixed[hp_name] = hp_value
-            elif isinstance(hp_value, dict):
-                # the hyperparameter is not mutatable, thus select the best fixed value and only add it to the
-                # search_space_with_fixed dictionary
-                print(
-                    f"Hyperparameter '{hp_name}' is not marked as mutatable. Fixing it to the best value found during "
-                    f"the previous optimization step: {best_hp_values_optuna[hp_name]}."
-                )
-                search_space_with_fixed[hp_name] = best_hp_values_optuna[hp_name]
-            else:
-                # if the hyperparameter was fixed from the beginning, we can just silently add it again to the search
-                # space
-                search_space_with_fixed[hp_name] = hp_value
-
-            # convert the search spaces to Tune search spaces
-            tune_search_space_with_fixed = build_tune_search_space(search_space_with_fixed)
-            tune_search_space_mutatable = build_tune_search_space(search_space_mutatable)
+        # if we have best values from a previous optimization step, fix these hyperparameters to their best value
+        for hp_name in non_mutatable_hps:
+            print(
+                f"Hyperparameter '{hp_name}' is not marked as mutatable. Fixing it to the best value found during "
+                f"the previous optimization step: {best_hp_values_optuna[hp_name]}."
+            )
+            search_space_with_fixed[hp_name] = best_hp_values_optuna[hp_name]
     else:
         # if we don't have best values to fix non-mutatable hyperparameters, all hyperparameters to optimize need to be
-        # mutatable
+        # mutatable or already fixed
         assert len(non_mutatable_hps) == 0, (
             f"Hyperparameters {non_mutatable_hps} are not marked with 'support_mutation', and no prior optimization has "
             "been performed to choose fixed values from."
         )
 
-        # convert search space to tune search space
-        tune_search_space_mutatable = build_tune_search_space(search_space)
-        tune_search_space_with_fixed = tune_search_space_mutatable
+    # convert the search spaces to Tune search spaces
+    tune_search_space_with_fixed = build_tune_search_space(search_space_with_fixed)
+    tune_search_space_mutatable = build_tune_search_space(search_space_mutatable, PBT=True)
 
     return tune_search_space_with_fixed, tune_search_space_mutatable
 
 
 def add_random_seed_suggestions(seed: Optional[int] = None) -> Callable:
     """Decorator function to add a random seed to the dictionary of suggestions produced by a search algorithm.
```

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/core/tools.py` & `optima_ml-0.3.3a1/OPTIMA/core/tools.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/core/training.py` & `optima_ml-0.3.3a1/OPTIMA/core/training.py`

 * *Files 0% similar despite different names*

```diff
@@ -782,15 +782,15 @@
         """
         (
             self.wait,
             self.wait_overfitting,
             self.best,
             self.best_metrics,
             self.best_weighted_metrics,
-            self.best_composite_metrics,
+            self.best_custom_metrics,
             self.best_composite_metrics,
             self.best_weights,
             self.best_epoch,
             self.stopped_epoch,
             self.early_stopped,
             self.last_valid,
         ) = state
```

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/core/variable_optimization.py` & `optima_ml-0.3.3a1/OPTIMA/core/variable_optimization.py`

 * *Files 0% similar despite different names*

```diff
@@ -875,15 +875,15 @@
     # hybrid mode has two phases, change mode to keep track
     if mode == "hybrid":
         mode = "hybrid_shuffle"
 
     # create output folder if necessary
     if plots_folder is not None:
         if not os.path.exists(plots_folder):
-            os.makedirs(plots_folder)
+            os.makedirs(plots_folder, exist_ok=True)
 
     # define helper functions to interact with the actor_pool. They are passed to the evaluation function.
     def _get_actor_pool(reuse: Optional[bool] = True) -> ray.util.ActorPool:
         """Small helper function to fetch the ``ShufflerAndPredictor`` actor pool.
 
         Parameters
         ----------
```

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/defaults.py` & `optima_ml-0.3.3a1/OPTIMA/defaults.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,49 +13,102 @@
 ]
 
 # the following arguments are required by at least one built-in function, i.e. they need to be provided in the run-config if the corresponding built-in functionality is used
 __requires_builtin__ = [
     (("get_inputs",), "inputs_file"),  # str; path to file containing the input data; needed for built-in get_inputs() function
 ]
 
-# hyperparameter search space. The range of hyperparameters can be specified by:
-#   - giving a fixed value --> no optimization
-#   - giving a list --> only specified values will be tried
-#   - giving a tuple (keyword, a, b, step), where keyword can be 'uniform' or 'log' (in which case the values will be
-#     drawn from a uniform/logarithmic distribution between a and b) or 'normal' (in which case the values will be drawn
-#     from a gaussian distribution with mean a and standard deviation b). step is optional and if given, the distribution
-#     will be discretized with step size step. For 'uniform' and 'log', the datatype of a will decide the datatype of the
-#     drawn value
+# hyperparameter search space. Allowed values can be specified by:
+#   - giving a fixed value (anything other than a dict) --> no optimization
+#   - giving a dict with the following allowed keys:
+#       - "type": either "range" or "choice"
+#       - "value_type": either "int" or "float" (only for type range) (default = float)
+#       - "bounds": lower and upper bounds for type range as list or tuple or conditional as tuple of type ((hp_name_1, ...), callable)
+#       - "sampling": "uniform", "log" or "normal" (only for type range) (default = "uniform")
+#       - "mean": mean of normal sampling (only for type range and sampling set to "normal")
+#       - "std": standard deviation of normal sampling (only for type range and sampling set to "normal")
+#       - "step": quantization step size for range search spaces; data type needs to fit "value_type"; for sampling = "log" and value_type = "int", this needs to be 1; (only for type range) (default = None for value_type = "float" and 1 for value_type = "int")
+#       - "values": allowed values for type "choice"; this can be a list or tuple of values or conditional as tuple of type ((hp_name_1, ...), callable)
+#       - "supports_mutation": bool; specifies if this hyperparameter is mutatable
+#       - "only": condition as a tuple of type ((hp_name_1, ...), callable) to specify if a value should be suggested for this hyperparameter (to build hierarchical search spaces)
+# Conditions are only possible for the pre- and main optimization with Optuna. For PBT, all conditional parameters must
+# be fixed (i.e. non-mutatable).
 # For the built-in MLP: tunable hyperparameters are: "num_layers", "units", "units_i" where i is the ith layer (WARNING:
-# when specifying units for each layer, make sure to give at least as many entries as the maximum possible number of layers
-# and set "optimize_units_per_layer" to True!), "activation", "kernel_initializer", "bias_initializer",
-# "dropout", "batch_size", "learning_rate", "Adam_beta_1", "one_minus_Adam_beta_2", "Adam_epsilon" and "loss_weight_class_i"
-# (with i between 0 and the number of classes - 1; WARNING: you need to specify either no or as many loss_weight_class
-# entries as there are classes). For all hyperparameters (besides loss_weight_class_i) that are not specified here,
-# default values given in OPTIMA.builtin.search_space.get_hp_defaults() will be used.
+# when specifying units for each layer, make sure to give at least as many entries as the maximum possible number of
+# layers), "activation", "kernel_initializer", "bias_initializer", "dropout", "batch_size", "learning_rate",
+# "Adam_beta_1", "one_minus_Adam_beta_2", "Adam_epsilon" and "loss_weight_class_i" (with i between 0 and the number of
+# classes - 1; WARNING: you need to specify either no or as many loss_weight_class entries as there are classes). For
+# all hyperparameters (besides loss_weight_class_i) that are not specified here, default values given in
+# OPTIMA.builtin.search_space.get_hp_defaults() will be used.
 search_space = {
-    "num_layers": ('uniform', 3, 6, 1),
-    "units": ('log', 16, 128, 1),
+    "num_layers": {
+        "type": "range",
+        "value_type": "int",
+        "bounds": [3, 6],
+    },
+    "units": {
+        "type": "range",
+        "value_type": "int",
+        "bounds": [16, 128],
+        "sampling": "log",
+    },
     "activation": 'swish',
     "kernel_initializer": 'auto',
     "bias_initializer": 'auto',
-    "l1_lambda": 0.,  # ('log', 1e-18, 1e-1),
-    "l2_lambda": 0.,  # ('log', 1e-18, 1e-1),
-    "dropout": ('uniform', 0.0, 0.2),
-    "batch_size": ('uniform', 64., 512.),
-    "learning_rate": ('log', 1e-5, 1e-2),
-    "Adam_beta_1": ('uniform', 1e-4, 0.99),
-    "one_minus_Adam_beta_2": ('log', 1e-5, 0.9999),
-    "Adam_epsilon": ('log', 1e-10, 1.0),
+    "l1_lambda": {
+        "type": "range",
+        "bounds": [1e-18, 0.1],
+        "sampling": "log",
+        "supports_mutation": True,
+    },
+    "l2_lambda": {
+        "type": "range",
+        "bounds": [1e-18, 0.1],
+        "sampling": "log",
+        "supports_mutation": True,
+    },
+    "dropout": {
+        "type": "range",
+        "bounds": [0, 0.2],
+        "supports_mutation": True,
+    },
+    "batch_size": {
+        "type": "range",
+        "value_type": "int",
+        "bounds": [64, 256],
+        "supports_mutation": True,
+    },
+    "learning_rate": {
+        "type": "range",
+        "bounds": [1e-5, 1e-2],
+        "sampling": "log",
+        "supports_mutation": True,
+    },
+    "Adam_beta_1": {
+        "type": "range",
+        "bounds": [1e-4, 0.99],
+        "supports_mutation": True,
+    },
+    "one_minus_Adam_beta_2": {
+        "type": "range",
+        "bounds": [1e-5, 0.9999],
+        "sampling": "log",
+        "supports_mutation": True,
+    },
+    "Adam_epsilon": {
+        "type": "range",
+        "bounds": [1e-10, 1.],
+        "sampling": "log",
+        "supports_mutation": True,
+    },
     "loss_function": 'BinaryCrossentropy',
     # "loss_weight_class_0": 1.0,
     # "loss_weight_class_1": 1.0,
     # "loss_weight_class_2": 1.0,
 }
-optimize_units_per_layer = False  # for built-in MLP; should each layer be of the same size or should the size of each layer be optimized individually?
 
 # output folder
 output_name = "OPTIMA_defaults"  # suffix appended to output folder name (which by default also contains the algorithm used and the validation offset as C# when using event numbers for splitting)
 output_path = "DNN_storage"  # this is where the output folder for the optimization will be created
 use_exact_name = False  # omit the automatically created part of the output folder name?
 produce_inputs_plots = True  # produce plots of the input variable before and after scaling
```

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/hardware_configs/Dresden_Taurus.py` & `optima_ml-0.3.3a1/OPTIMA/hardware_configs/Dresden_Taurus.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/hardware_configs/common.py` & `optima_ml-0.3.3a1/OPTIMA/hardware_configs/common.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/helpers/extract_data_from_NTuples.py` & `optima_ml-0.3.3a1/OPTIMA/helpers/extract_data_from_NTuples.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/helpers/manage_ray_nodes.py` & `optima_ml-0.3.3a1/OPTIMA/helpers/manage_ray_nodes.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/keras/model.py` & `optima_ml-0.3.3a1/OPTIMA/keras/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -532,15 +532,15 @@
 
     if scale is None or offset is None:
         logging.error("Could not find the Normalization layer in the provided model, skipping the export to LWTNN...")
         return
     else:
         # we found the normalization layer, so we can do the export
         if not os.path.exists(output_dir):
-            os.makedirs(output_dir)
+            os.makedirs(output_dir, exist_ok=True)
 
     # built the basic structure of the variables part of the lwtnn model
     vars_dict = {
         "input_sequences": [],
         "inputs": [{"name": "node_0", "variables": []}],
         "outputs": [{"labels": [f"out_{i}" for i in range(output_shape[0])], "name": "MyLWTNNOutput"}],
     }
```

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/keras/tools.py` & `optima_ml-0.3.3a1/OPTIMA/keras/tools.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/keras/training.py` & `optima_ml-0.3.3a1/OPTIMA/keras/training.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/lightning/inputs.py` & `optima_ml-0.3.3a1/OPTIMA/lightning/inputs.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/lightning/training.py` & `optima_ml-0.3.3a1/OPTIMA/lightning/training.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/optima.py` & `optima_ml-0.3.3a1/OPTIMA/optima.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Main steering script of OPTIMA."""
 
 __author__ = "E. Bachmann"
 __licence__ = "GPL3"
-__version__ = "0.3.2alpha5_dev2"
+__version__ = "0.3.3alpha1"
 __maintainer__ = "E. Bachmann"
 
 import os
 import sys
 import shutil
 import logging
 import argparse
@@ -14,25 +14,24 @@
 import functools
 
 if sys.platform == "darwin":
     import multiprocess as mp
 else:
     import multiprocessing as mp
 import pickle
-import dill
 import time
 import random as python_random
 
 import numpy as np
 import pyarrow
 import optuna
 
-os.environ["TUNE_RESULT_BUFFER_LENGTH"] = "1000"  # buffer Tune results; allows for speculative execution of trials to reduce overhead during peak reporting
+# os.environ["TUNE_RESULT_BUFFER_LENGTH"] = "1000"  # buffer Tune results; allows for speculative execution of trials to reduce overhead during peak reporting
 os.environ["RAY_DEDUP_LOGS"] = "0"  # disable log deduplication
-os.environ["TUNE_WARN_EXCESSIVE_EXPERIMENT_CHECKPOINT_SYNC_THRESHOLD_S"] = "0"  # temporary solution to disable annoying warnings until a better syncing is implemented
+# os.environ["TUNE_WARN_EXCESSIVE_EXPERIMENT_CHECKPOINT_SYNC_THRESHOLD_S"] = "0"  # temporary solution to disable annoying warnings until a better syncing is implemented
 import ray
 from ray import train, tune
 from ray.tune.schedulers import ASHAScheduler, PopulationBasedTrainingReplay
 # from ray.tune.search.hebo import HEBOSearch
 from ray.tune.search.optuna import OptunaSearch
 from ray.tune.logger import JsonLoggerCallback, CSVLoggerCallback
 from optuna.samplers import TPESampler
@@ -364,15 +363,15 @@
                 enable_checkpointing=False,  # checkpointing is done in the early stopper
             )
             trainer.fit(model, pl_data_module)
 
         # if requested, save the final model
         if "final_model_path" in model_config.keys():
             if not os.path.exists(os.path.dirname(model_config["final_model_path"])):
-                os.makedirs(os.path.dirname(model_config["final_model_path"]))
+                os.makedirs(os.path.dirname(model_config["final_model_path"]), exist_ok=True)
             if run_config.model_type == "Keras":
                 out_path = model_config["final_model_path"] + ".keras"
                 model.save(out_path, save_format="keras")
             elif run_config.model_type == "Lightning":
                 out_path = model_config["final_model_path"] + ".ckpt"
                 trainer.save_checkpoint(out_path)
 
@@ -520,15 +519,15 @@
     target_metric_for_PBT_init = run_config.monitor_name  # when using multiple metrics for the optimization (not yet implemented, TODO!), need to specify one to select the fixed hyperparameters for PBT from the optuna results
     output_dir = OPTIMA.core.tools.get_output_dir(run_config)
     optimization_dir = os.path.join(output_dir, 'optimization')  # this is where all the optimization files are saved
     results_dir = os.path.join(output_dir, 'results')  # when the optimization is done, the best model for each method is copied here and evaluated
 
     # for later reproduction, copy the config to the output folder
     if not os.path.exists(output_dir):
-        os.makedirs(output_dir)
+        os.makedirs(output_dir, exist_ok=True)
     print("copying run-config from {} to {}".format(args.config, os.path.join(output_dir, "config.py")))
     try:
         shutil.copy2(args.config, os.path.join(output_dir, "config.py"))
     except shutil.SameFileError:
         print("Provided run-config is already in the output directory, skipping...")
 
     # also write the defaults config to the output folder
@@ -585,19 +584,14 @@
 
     # build the search space for optuna
     search_space_optuna = functools.partial(
         OPTIMA.core.search_space.optuna_search_space,
         OPTIMA.core.search_space.serialize_conditions(run_config.search_space)
     )
 
-    # clear the local Ray (temp) directory
-    ray_local_dir = os.path.join(get_cluster(args.cluster).ray_temp_path, "ray_results") if args.cluster != 'local' else os.path.join("/tmp", "ray_results")
-    if os.path.exists(ray_local_dir):
-        shutil.rmtree(ray_local_dir)
-
     # setup ray
     if args.is_worker:
         ray.init(address=args.address, _temp_dir=get_cluster(args.cluster).ray_temp_path)
     else:
         ray.init(
             include_dashboard=False,
             num_cpus=args.cpus,
@@ -671,17 +665,17 @@
         if run_config.perform_main_hyperopt or run_config.perform_PBT_hyperopt:
             optimization_dir_varOpt = os.path.join(optimization_dir, "variable_optimization")
             results_dir_variableOpt = os.path.join(results_dir, "variable_optimization")
         else:
             optimization_dir_varOpt = optimization_dir
             results_dir_variableOpt = results_dir
         if not os.path.exists(optimization_dir_varOpt):
-            os.makedirs(optimization_dir_varOpt)
+            os.makedirs(optimization_dir_varOpt, exist_ok=True)
         if not os.path.exists(results_dir_variableOpt):
-            os.makedirs(results_dir_variableOpt)
+            os.makedirs(results_dir_variableOpt, exist_ok=True)
 
         if not os.path.isfile(os.path.join(results_dir_variableOpt, "analysis.pickle")):
             # the only way to add a unique random seed for each trial is to include it as part of the hyperparameter
             # suggestions. Since we don't want the search algorithm to try to optimize the seed, we cannot include it in
             # the search space (i.e. via a uniform distribution). Instead, create a subclass of the searcher that adds a
             # randomly generated seed to the suggestions, thus the searcher does not know about the seed at all.
             OptunaWithSeed = OPTIMA.core.search_space.add_random_seed_suggestions(rng_varOpt.randint(*max_seeds))(OptunaSearch)
@@ -698,33 +692,28 @@
             asha_scheduler = ASHAScheduler(
                 grace_period=run_config.ASHA_grace_period,
                 max_t=run_config.ASHA_max_t,
                 reduction_factor=run_config.ASHA_reduction_factor,
                 stop_last_trials=False
             ) if run_config.use_ASHAScheduler else None
 
-            # set Tune results dir before initializeing the Tuner, otherwise Tuner is not saved correctly; TODO: check if this is still the case!
-            os.environ["RAY_AIR_LOCAL_CACHE_DIR"] = ray_local_dir
-
             resume_failed = False
             if resume_experiment and tune.Tuner.can_restore(os.path.abspath(optimization_dir_varOpt)):
                 # currently, restore does not handle relative paths; TODO: still True?
                 tuner = tune.Tuner.restore(os.path.abspath(optimization_dir_varOpt), trainable=trainable, resume_errored=True)
             else:
                 tuner = tune.Tuner(
                     tune.with_resources(
                         trainable,
                         resources=tune.PlacementGroupFactory([{"CPU": args.cpus_per_trial, "GPU": args.gpus_per_trial, "memory": memory_per_trial}]),
                     ),
                     # param_space=search_space,
                     run_config=train.RunConfig(
                         name=os.path.basename(optimization_dir_varOpt),
                         storage_path=os.path.dirname(os.path.abspath(optimization_dir_varOpt)),  # with Ray 2.7 this needs to be absolute, otherwise Ray complains about write permissions?
-                        local_dir=ray_local_dir,
-                        storage_filesystem=pyarrow.fs.LocalFileSystem(),
                         stop=stopper,
                         checkpoint_config=train.CheckpointConfig(
                             num_to_keep=1,
                             # checkpoint_score_attribute=optimize_name,
                             # checkpoint_score_order=optimize_op
                         ),
                         failure_config=train.FailureConfig(
@@ -905,17 +894,17 @@
         if run_config.perform_variable_opt or run_config.perform_PBT_hyperopt:
             optimization_dir_optuna = os.path.join(optimization_dir, "optuna+ASHA")
             results_dir_optuna = os.path.join(results_dir, "optuna+ASHA")
         else:
             optimization_dir_optuna = optimization_dir
             results_dir_optuna = results_dir
         if not os.path.exists(optimization_dir_optuna):
-            os.makedirs(optimization_dir_optuna)
+            os.makedirs(optimization_dir_optuna, exist_ok=True)
         if not os.path.exists(results_dir_optuna):
-            os.makedirs(results_dir_optuna)
+            os.makedirs(results_dir_optuna, exist_ok=True)
 
         if not os.path.isfile(os.path.join(results_dir_optuna, "analysis.pickle")):
             # the only way to add a unique random seed for each trial is to include it as part of the hyperparameter
             # suggestions. Since we don't want the search algorithm to try to optimize the seed, we cannot include it in
             # the search space (i.e. via a uniform distribution). Instead, create a subclass of the searcher that adds a
             # randomly generated seed to the suggestions, thus the searcher does not know about the seed at all.
             OptunaWithSeed = OPTIMA.core.search_space.add_random_seed_suggestions(rng_optuna.randint(*max_seeds))(OptunaSearch)
@@ -932,33 +921,28 @@
             asha_scheduler = ASHAScheduler(
                 grace_period=run_config.ASHA_grace_period,
                 max_t=run_config.ASHA_max_t,
                 reduction_factor=run_config.ASHA_reduction_factor,
                 stop_last_trials=False
             ) if run_config.use_ASHAScheduler else None
 
-            # set Tune results dir before initializeing the Tuner, otherwise Tuner is not saved correctly; TODO: check if this is still the case!
-            os.environ["RAY_AIR_LOCAL_CACHE_DIR"] = ray_local_dir
-
             if resume_experiment and tune.Tuner.can_restore(os.path.abspath(optimization_dir_optuna)):
                 # currently, restore does not handle relative paths; TODO: still True?
                 tuner = tune.Tuner.restore(os.path.abspath(optimization_dir_optuna), trainable=trainable, resume_errored=True)
             else:
                 tuner = tune.Tuner(
                     tune.with_resources(
                         trainable,
                         resources=tune.PlacementGroupFactory(
                             [{"CPU": args.cpus_per_trial, "GPU": args.gpus_per_trial, "memory": memory_per_trial}]),
                     ),
                     # param_space=search_space,
                     run_config=train.RunConfig(
                         name=os.path.basename(optimization_dir_optuna),
                         storage_path=os.path.dirname(os.path.abspath(optimization_dir_optuna)),  # with Ray 2.7 this needs to be absolute, otherwise Ray complains about write permissions?
-                        local_dir=ray_local_dir,
-                        storage_filesystem=pyarrow.fs.LocalFileSystem(),  # all trials will be on the same filesystem, so we don't need syncing
                         stop=stopper,
                         checkpoint_config=train.CheckpointConfig(
                             num_to_keep=1,
                             # checkpoint_score_attribute=optimize_name,
                             # checkpoint_score_order=optimize_op
                         ),
                         failure_config=train.FailureConfig(
@@ -1074,35 +1058,33 @@
         if run_config.perform_variable_opt or run_config.perform_main_hyperopt:
             optimization_dir_PBT = os.path.join(optimization_dir, "PBT")
             results_dir_PBT = os.path.join(results_dir, "PBT")
         else:
             optimization_dir_PBT = optimization_dir
             results_dir_PBT = results_dir
         if not os.path.exists(optimization_dir_PBT):
-            os.makedirs(optimization_dir_PBT)
+            os.makedirs(optimization_dir_PBT, exist_ok=True)
         if not os.path.exists(results_dir_PBT):
-            os.makedirs(results_dir_PBT)
+            os.makedirs(results_dir_PBT, exist_ok=True)
 
-        def _get_PBT_tuner(trainable, scheduler, stopper, name, storage_path, verbose=1, replay=False):
-            # set Tune results dir before initializeing the Tuner, otherwise Tuner is not saved correctly; TODO: check if this is still the case!
-            os.environ["RAY_AIR_LOCAL_CACHE_DIR"] = ray_local_dir
+        # since PBT only uses the RandomSampler, we can safely increase the number of pending trails
+        os.environ['TUNE_MAX_PENDING_TRIALS_PG'] = str(run_config.num_samples_PBT)
 
+        def _get_PBT_tuner(trainable, scheduler, stopper, name, storage_path, verbose=1, replay=False):
             tuner = tune.Tuner(
                 tune.with_resources(
                     trainable,
                     resources=tune.PlacementGroupFactory(
                         [{"CPU": args.cpus_per_trial, "GPU": args.gpus_per_trial, "memory": memory_per_trial}]),
                     # resources={"cpu": cpus_per_trial, "gpu": args.gpus_per_trial, "memory": memory_per_trial},
                 ),
                 param_space=search_space_PBT if not replay else None,
                 run_config=train.RunConfig(
                     name=name,
                     storage_path=os.path.abspath(storage_path),  # with Ray 2.7 this needs to be absolute, otherwise Ray complains about write permissions?
-                    local_dir=ray_local_dir,
-                    storage_filesystem=pyarrow.fs.LocalFileSystem(),  # all trials will be on the same filesystem, so we don't need syncing
                     stop=stopper,
                     checkpoint_config=train.CheckpointConfig(
                         num_to_keep=2*max(run_config.perturbation_interval, run_config.burn_in_period)+2,
                         # checkpoint_score_attribute=optimize_name,
                         # checkpoint_score_order=optimize_op
                     ),
                     failure_config=train.FailureConfig(
@@ -1411,15 +1393,15 @@
 {ray_setup_2}
 
 {command}""".format(environment=environment_str, ulimit=ulimit_str, ray_setup_1=ray_setup_str_1, ray_setup_2=ray_setup_str_2,
                command=command_str)
 
     # create logs folder
     if not os.path.exists("logs"):
-        os.makedirs("logs")
+        os.makedirs("logs", exist_ok=True)
 
     # write copy of batch job file to output path for reproducibility
     job.payload = job_str
     output_dir = OPTIMA.core.tools.get_output_dir(run_config)
     cluster.submit_job(job, job_file_path=os.path.join(output_dir, "submit_DNNOptimization_ray.sh"), dry_run=True)
 
     # execute the job; do not overwrite existing batch scripts, instead append next free number
@@ -1461,15 +1443,15 @@
     parser.add_argument('--cpus_per_trial', type=int, default=1, help="Number of CPUs that are used for each trial.")
     parser.add_argument('--gpus_per_trial', type=float, default=0.0, help="Number of GPUs that are used for each trial. This can be a fractional number to run multiple trials on each GPU.")
     parser.add_argument('--max_pending_trials', type=int, default=None, help="Set how many trials are allowed to be 'pending'. If not set, will set to cpus / cpus_per_trail.")
 
     parser.add_argument('--is_worker', default=False, action="store_true", help="Is used to differentiate between the initialization step (create and execute batch script) and the working step (where the optimization is done).")
     parser.add_argument('--address', default=None, help="IP-address and port of the head node. This is set automatically for the working step.")
     parser.add_argument('--local_source', default=False, action="store_true", help="If set, will use the local source code even if OPTIMA is installed in the python environment.")
-    parser.add_argument('--temp_dir', type=str, default=None, help="Overwrite Ray's default root temporary directory. This must be an absolute path.")
+    parser.add_argument('--temp_dir', type=str, default=None, help="Overwrite Ray's default root temporary directory when running locally (i.e. --cluster 'local'). This must be an absolute path.")
 
     args = parser.parse_args(sys.argv[1:])
 
     # logging config
     DFormat = '%(asctime)s - %(levelname)s - %(message)s'
     logging.basicConfig(format=DFormat, level=logging.INFO)
 
@@ -1653,21 +1635,21 @@
                 if args.gpus_per_worker > cluster.gpus_per_node:
                     logging.critical(f"The provided number of GPUs of {args.gpus} and number of nodes of {args.workers} "
                                      f"results in a number of GPUs per node of {args.gpus_per_worker}, which exceeds the "
                                      f"cluster limit of {cluster.gpus_per_node}.")
                     sys.exit(1)
 
             # consistency: CPU
-            if args.cpus % args.cpus_per_worker != args.workers:
+            if args.cpus // args.cpus_per_worker != args.workers:
                 logging.critical(f"Number of CPUs of {args.cpus}, number of CPUs per node of {args.cpus_per_worker} "
                                  f"and number of nodes of {args.workers} are not consistent, i.e. num_nodes * num_cpus_per_node != num_cpus!")
                 sys.exit(1)
 
             # consistency: GPU
-            if args.gpus % args.gpus_per_worker != args.workers:
+            if args.gpus > 0 and args.gpus // args.gpus_per_worker != args.workers:
                 logging.critical(f"Number of GPUs of {args.gpus}, number of GPUs per node of {args.gpus_per_worker} "
                                  f"and number of nodes of {args.workers} are not consistent, i.e. num_nodes * num_gpus_per_node != num_gpus!")
                 sys.exit(1)
         else:
             # number of cpus needs to be specified for variable node size to work!
             if args.cpus is None:
                 logging.critical(f"The number of CPU cores need to be specified for the variable Ray node size to work!")
```

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/resources/config_verification.py` & `optima_ml-0.3.3a1/OPTIMA/resources/config_verification.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.2a5.dev2/OPTIMA/resources/pbt_with_seed.py` & `optima_ml-0.3.3a1/OPTIMA/resources/pbt_with_seed.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.2a5.dev2/PKG-INFO` & `optima_ml-0.3.3a1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optima-ml
-Version: 0.3.2a5.dev2
+Version: 0.3.3a1
 Summary: Distributed hyperparameter optimization and input variable selection for artificial neural networks.
 Home-page: https://gitlab.cern.ch/atlas-germany-dresden-vbs-group/optima
 Author: E. Bachmann
 Author-email: erik.bachmann@tu-dresden.de
 License: GPL
 Platform: linux
 Platform: darwin
@@ -16,16 +16,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: optuna==3.5.0
-Requires-Dist: ray[data,train,tune]==2.9.2
+Requires-Dist: optuna==3.6
+Requires-Dist: ray[data,train,tune]==2.11
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: seaborn
 Requires-Dist: tabulate
 Requires-Dist: scikit-learn
@@ -70,15 +70,14 @@
     - [Custom Keras objects](#custom-keras-objects)
     - [Cluster setup](#cluster-setup)
   + [Built-in functionality](#built-in-functionality)
     - [Keras](#keras-1)
     - [Inputs](#inputs-1)
     - [Trial selection](#trial-selection-1)
     - [Evaluation](#evaluation-1)
-    - [Hyperparameter optimization](#hyperparameter-optimization-1)
     - [Input variable selection](#input-variable-selection-1)
 
 ## Documentation
 
 A quick overview and instructions on how to configure OPTIMA to perform an optimization is given in [usage](#usage).
 A more detailed introduction including a description of the inner workings of OPTIMA can be found in chapter 4.2 of
 https://inspirehep.net/literature/2707309. Automatically generated API documentation is published at
@@ -283,14 +282,15 @@
 - `defaults`: Path to an alternative defaults-config. This overwrites the built-in default parameter values. (Default: `None`)
 - `cpus`: Total number of CPUs to use. (Default: `1`)
 - `gpus`: Total number of GPUs to use. (Default: `0`)
 - `mem_per_cpu`: Amount of memory to allocate per CPU (in MB). (Default: `1000`)
 - `cpus_per_trial`: Number of CPUs to use per trial. (Default: `1`)
 - `gpus_per_trial`: Number of GPUs to use per trial. This can be a fractional number if multiple trials should share a GPU. (Default: `0`)
 - `max_pending_trials`: The maximum number of trials that are allowed to be `'pending'`. (Default: `cpus / cpus_per_trial`)
+- `temp_dir`: Overwrite Ray's default root temporary directory (`/tmp/ray`). This must be an absolute path.
 
 #### Cluster
 
 If the `cluster` command line argument is set to the name of a built-in cluster or to `'custom'`, the optimization will be
 launched as a cluster job. This is done by manually launching a Ray node on each node in the job in order to build a Ray
 cluster, to which OPTIMA in then connected. Ray then takes care of distributing all tasks across the cluster. It is
 possible to run multiple optimizations in parallel on the same cluster; each job will consequently build its own Ray cluster.
@@ -389,37 +389,37 @@
 |------------------------------------|---------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `monitor_name` *(str)*             | `'val_loss'`  | Controls which metric is used as the target of the optimization and for early stopping during training. Allowed are native, weighted native, custom and composite metrics as well as all metrics reported by the ML backend during training (e.g. `"val_loss"`). Make sure to add the `"val_"`-prefix when using native, weighted native or custom metrics.                                                                                                                                                                                                                                                                                                                                                                |
 | `monitor_op` *(str)*               | `'min'`       | Is the target metric to be minimized (`'min'`) or maximized (`'max'`)?                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
 | `native_metrics` *(list)*          | `[]`          | A list of references to a metric class native to the used ML backend. Each entry must be a tuple of the form `("name", (ClassReference, {"kwarg1": kwarg1, ...}))`. Their values are calculated separately on the training and validation datasets and reported as `"train_name" and "val_name". Event weights are not applied.                                                                                                                                                                                                                                                                                                                                                                                            |
 | `weighted_native_metrics` *(list)* | `[]`          | A list of references to a metric class native to the used ML backend. Each entry must be a tuple of the form `("name", (ClassReference, {"kwarg1": kwarg1, ...}))`. Their values are calculated separately on the training and validation datasets and reported as `"train_name" and "val_name". Event weights are applied. Currently, weighted metrics are not supported for Lightning (see https://github.com/Lightning-AI/torchmetrics/issues/784).                                                                                                                                                                                                                                                                     |
 | `custom_metrics` *(list)*          | `[]`          | A list of custom metrics. Each entry must be a tuple of the form `("name", callable)`. `callable` needs to accept target values, model prediction and sample weights and return a number or a boolean. Their values are calculated at the end of each epoch separately on the training and validation datasets and reported as `"train_name" and "val_name".                                                                                                                                                                                                                                                                                                                                                               |
 | `composite_metrics` *(list)*       | `[]`          | A list of composite metrics. These are metrics that combine the values of already existing metrics. Each entry must be a tuple of the form `("name", (metric_name1, metric_name2, ...), callable)` where `callable` accepts the same number of positional arguments as the number of provided metric names and returns a number or a boolean. They are calculated at the end of each epoch and allow all native, weighted native and custom metrics as well as metrics directly reported by the ML backend (e.g. validation loss) as inputs. It is possible to mix training and validation metrics, allowing e.g. to assess the generalization gap. The value of composite metrics is reported as "name" without a prefix. |
-| `overtraining_conditions` *(list)* | `[]`          | A list of overtraining conditions. Thse are special composite metrics that should return `True` when overtraining is detected and `False` otherwise. Each entry must be a tuple of the form `("name", (metric_name1, metric_name2, ...), callable)` where `callable` accepts the same number of positional arguments as the number of provided metric names and returns a boolean. They are calculated at the end of each epoch and allow all native, weighted native, custom and composite metrics as well as metrics directly reported by the ML backend (e.g. validation loss) as inputs. Naturally, it is possible to mix training and validation metrics. The value of overtraining conditions is not reported.       |
+| `overtraining_conditions` *(list)* | `[]`          | A list of overtraining conditions. These are special composite metrics that should return `True` when overtraining is detected and `False` otherwise. Each entry must be a tuple of the form `("name", (metric_name1, metric_name2, ...), callable)` where `callable` accepts the same number of positional arguments as the number of provided metric names and returns a boolean. They are calculated at the end of each epoch and allow all native, weighted native, custom and composite metrics as well as metrics directly reported by the ML backend (e.g. validation loss) as inputs. Naturally, it is possible to mix training and validation metrics. The value of overtraining conditions is not reported.      |
 
 #### Training
 
 | Parameter                         | Default value | Explanation                                                                                                                                                                                                                                                                                                                   |
 |-----------------------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `max_epochs` *(int)*              | `200`         | The maximal number of epochs until the training is terminated. Early stopping may terminate the training earlier.                                                                                                                                                                                                             |
 | `early_stopping_patience` *(int)* | `6`           | The maximal number of consecutive epochs without an improvement of the target metric before early-stopping the training.                                                                                                                                                                                                      |
 | `overtraining_patience` *(int)*   | `6`           | The maximal number of consecutive epochs with overtraining detected (i.e. at least one overtraining condition detected overtraining) before early-stopping the training. This is ignored if no overtraining conditions are defined.                                                                                           |
 | `callbacks` *(list)*              | `[]`          | A list of references to a callback class native to the used ML backend (i.e. a subclass of `keras.callbacks.Callback` for Keras or `lightning.pytorch.callbacks.Callback` for Lightning. Each entry must be a tuple of the form `(ClassReference, {"kwarg1": kwarg1, ...})`. The callbacks are only used during the training. |
 
 #### Hyperparameter optimization
 
 ##### General
 
-| Parameter                             | Default value                                                                                                                 | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
-|---------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `optimize_on_best_value` *(bool)*     | `False`                                                                                                                       | Controls how each trial is evaluated during the hyperparameter optimization. While the target metric is calculated every epoch, *Tune* only allows accepts a single value to evaluate a trial. If `True`, the best epoch that passes all overtraining conditions (which is usually representative of the best performance possible with these hyperparameters, but may also be an outlier) is used. If `False`, the last epoch that passed all overtraining conditions (which is less likely an outlier but may be degraded due to overtraining) is used.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
-| `restore_on_best_checkpoint` *(bool)* | `True`                                                                                                                        | When resuming a trial (e.g. during Population Based Training), resume from the best epoch (`True`) or last epoch (`False`)?                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
-| `num_samples_variableOpt` *(int)*     | `1`                                                                                                                           | The number of trials (hyperparameter combinations) to try during the initial hyperparameter optimization step.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
-| `num_samples_main` *(int)*            | `1`                                                                                                                           | The number of trials (hyperparameter combinations) to try during the main hyperparameter optimization step.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
-| `num_samples_PBT` *(int)*             | `4`                                                                                                                           | The number of trials in the population for the hyperparameter fine-tuning step with Population Based Training.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
-| `search_space` *(dict)*               | see [here](https://gitlab.cern.ch/atlas-germany-dresden-vbs-group/optima/-/blob/master/OPTIMA/defaults.py?ref_type=heads#L35) | Defines the hyperparameter search space. Each dictionary entry corresponds to a hyperparameter. The corresponding range can be specified by giving a fixed value (no optimization), a list (only provided values are tried) or a tuple `(keyword, a, b, step)` where keyword can be `'uniform'` or `'log'` (in which case the values will be drawn from a uniform/logarithmic distribution between `a` and `b`) or `'normal'` (in which case the values will be drawn from a gaussian distribution with mean `a` and standard deviation `b`). `step` is optional and if provided, the distribution will be discretized with step size step. For `'uniform'` and `'log'`, the datatype of `a` decides the datatype of the drawn value. Being independent of the particular task, the batch size (with key `'batch_size'`) must always be provided as a hyperparameter, either as a fixed integer, an integer search space or a continuous search space and quantizing in the `limit_and_round_hyperparameters` function. The last option is necessary to allow Population Based Training to optimize the batch size. |
+| Parameter                             | Default value                                                                                                                 | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+|---------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `optimize_on_best_value` *(bool)*     | `False`                                                                                                                       | Controls how each trial is evaluated during the hyperparameter optimization. While the target metric is calculated every epoch, *Tune* only allows accepts a single value to evaluate a trial. If `True`, the best epoch that passes all overtraining conditions (which is usually representative of the best performance possible with these hyperparameters, but may also be an outlier) is used. If `False`, the last epoch that passed all overtraining conditions (which is less likely an outlier but may be degraded due to overtraining) is used.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| `restore_on_best_checkpoint` *(bool)* | `True`                                                                                                                        | When resuming a trial (e.g. during Population Based Training), resume from the best epoch (`True`) or last epoch (`False`)?                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+| `num_samples_variableOpt` *(int)*     | `1`                                                                                                                           | The number of trials (hyperparameter combinations) to try during the initial hyperparameter optimization step.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+| `num_samples_main` *(int)*            | `1`                                                                                                                           | The number of trials (hyperparameter combinations) to try during the main hyperparameter optimization step.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+| `num_samples_PBT` *(int)*             | `4`                                                                                                                           | The number of trials in the population for the hyperparameter fine-tuning step with Population Based Training.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+| `search_space` *(dict)*               | see [here](https://gitlab.cern.ch/atlas-germany-dresden-vbs-group/optima/-/blob/master/OPTIMA/defaults.py?ref_type=heads#L42) | Defines the hyperparameter search space. Each dictionary entry corresponds to a hyperparameter, and the corresponding search space is defined using a dictionary with the following allowed key-value pairs:<br><ul><li>`'type'`: Specifies if a range of values (`'range'`) or a list of allowed values (`'choice'`) defines the search space.</li><li>`'bounds'`: Specifies the lower and upper bounds for range search spaces. This can be given as a list or tuple of type `(lower_bound, upper_bound)`. Alternatively, conditional bounds that depend on the values of other hyperparameters can be specified as a tuple of type `(hp_depends_tuple, callable)`. Here, `hp_depends_tuple` is a tuple of hyperparameters the bounds depend on (i.e. each entry must correspond to another key in the search space). The `callable` will be provided with the values of the hyperparameters specified in `hp_depends_tuple` as positional arguments and needs to return a list or tuple of type `(lower_bound, upper_bound)`. Conditional bounds are not supported for Population Based Training. This is only used for range search spaces.</li><li>`'value_type'`: Specifies if an integer (`'int'`) or float (`'float'`) value should be suggested. Defaults to `'float'`. This is only used for range search spaces.</li><li>`'sampling'`: Specifies if the search space should be sampled uniformly (`'uniform'`), logarithmically (`'log'`) or gaussian distributed (`'normal'`). Gaussian sampled integer search spaces are not supported. Defaults to `'uniform'`. This is only used for range search spaces.</li><li>`'mean'`: Specifies the mean of the gaussian sampling. This can be given as a float or integer. Only used for range search spaces and `'sampling'` set to `'normal'`.</li><li>`'std'`: Specifies the standard deviation of the gaussian sampling. This can be given as a float or integer. Only used for range search spaces and `'sampling'` set to `'normal'`.</li><li>`'step'`: Used to quantize range search spaces. For integer search spaces, this must be an integer. For float search spaces, this can be an integer or a float. For log-sampled search spaces, setting a step size is not supported. Defaults to `None` (i.e. unquantized) for float and `1` for integer parameters. This is only used for range search spaces.</li><li>`'values'`: Specifies the allowed values for choice search spaces. This can be a list or a tuple. Alternatively, conditional values that depend on the values of other hyperparameters can be specified as a tuple of type `(hp_depends_tuple, callable)`. Here, `hp_depends_tuple` is a tuple of hyperparameters the values depend on (i.e. each entry must correspond to another key in the search space). The `callable` will be provided with the values of the hyperparameters specified in `hp_depends_tuple` as positional arguments and needs to return a list or tuple of allowed values. Conditional values are not supported for Population Based Training. This is only used for choice search spaces.</li><li>`'supports_mutation'`: A `bool` that specifies if this hyperparameter can be altered during the training without loosing the training state. Only these hyperparameters can be optimized with Population Based Training. The remaining hyperparameters will be fixed to the best value found during the previous hyperparameter optimization step. If only the Population Based Training step is performed, all hyperparameters need to be fixed or mutatable.</li><li>`'only'`: Used to build hierarchical search spaces where not all hyperparameters are always needed (e.g. the number of neurons in the fourth layer are only needed if the number of layers is at least four). If provided, this needs to be a tuple of type `(hp_depends_tuple, callable)`. Here, `hp_depends_tuple` is a tuple of hyperparameters that are necessary to decide if this hyperparameter is needed (i.e. each entry must correspond to another key in the search space). The `callable` will be provided with the values of the hyperparameters specified in `hp_depends_tuple` as positional arguments and needs to return a `bool` that signifies if a value should be suggested for this hyperparameter. If the condition is evaluated as `False`, the value if the hyperparameter is explicitly set to `None` and provided as such to all conditions that depend on this hyperparameter. This allows defining multiple dependency layers where, e.g., `B` is only needed if `A > 0` and `C` is only needed if `B` exists and `B > 0`. Rejected hyperparameters will, however, not be added to the `model_config`. Hierarchical search spaces are not supported for Population Based Training.</li></ul>Any search space entry that is not a dictionary is considered fixed and the corresponding hyperparameter will not be optimized but still added to the `model_config`. Being independent of the particular task, the batch size (with key `'batch_size'`) must always be provided as a hyperparameter, either as a fixed integer or as an integer range search space. |
 
 
 ##### Bayesian optimization (Optuna)
 
 | Parameter                       | Default value | Explanation                                                                                                                                |
 |---------------------------------|---------------|--------------------------------------------------------------------------------------------------------------------------------------------|
 | `use_TPESampler` *(bool)*       | `True`        | Use Optuna's Tree-structured Parzen Estimator algorithm or random sampling?                                                                |
@@ -427,19 +427,19 @@
 | `use_ASHAScheduler` *(bool)*    | `True`        | Use the Asynchronous HyperBand scheduler (ASHA) to prune trials or not?                                                                    |
 | `ASHA_grace_period` *(int)*     | `15`          | The minimum number of epochs to wait before the ASHA scheduler is allowed to prune a trial. Only used if `use_ASHAScheduler` is `True`.    |
 | `ASHA_max_t` *(int)*            | `max_epochs`  | The end point of the reduction with ASHA. Only used if `use_ASHAScheduler` is `True`.                                                      |
 | `ASHA_reduction_factor` *(int)* | `2`           | Controls which fraction of trials is terminated at each point by ASHA. A value of `2` corresponds to the termination of 50% of all trials. |
 
 ##### Population Based Training
 
-| Parameter                          | Default value | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
-|------------------------------------|---------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `use_fit_results_for_PBT` *(bool)* | `True`        | PBT cannot optimize all hyperparameters. If the inital or main hyperparameter optimization step was run before, all unsupported hyperparameters are fixed to their optimized values from the previous optimization step. If `use_fit_results_for_PBT` is `True`, the best-fit results are used, otherwise the best-value results are used. If only the PBT step is performed, unsupported parameters are set to the default values defined by `get_hp_defaults()`. |
-| `perturbation_interval` *(int)*    | `6`           | The number of epochs to train between each perturbation of a trial.                                                                                                                                                                                                                                                                                                                                                                                                |
-| `burn_in_period` *(int)*           | `6`           | The number of epochs to wait before the first perturbation of a trial.                                                                                                                                                                                                                                                                                                                                                                                             |
+| Parameter                          | Default value | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
+|------------------------------------|---------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `use_fit_results_for_PBT` *(bool)* | `True`        | PBT is only applied to hyperparameters that are marked with `'supports_mutation'` set to `True`. If the initial and/or main hyperparameter optimization step was run before, all unsupported hyperparameters are fixed to their optimized values from the previous optimization step. If `use_fit_results_for_PBT` is `True`, the best-fit results are used, otherwise the best-value results are used. If only the PBT step is performed, all provided hyperparameters need to be fixed or support mutation. |
+| `perturbation_interval` *(int)*    | `6`           | The number of epochs to train between each perturbation of a trial.                                                                                                                                                                                                                                                                                                                                                                                                                                           |
+| `burn_in_period` *(int)*           | `6`           | The number of epochs to wait before the first perturbation of a trial.                                                                                                                                                                                                                                                                                                                                                                                                                                        |
 
 #### Trial selection
 
 To select the best set of hyperparameters and the number of epochs to train from the pool of tested trials, two
 independent algorithms are used:
 
 - **best-value**: the best trial is given by the best reported value of the target metric (i.e. best single epoch) while
@@ -545,26 +545,33 @@
 as the built-in counterpart, unless otherwise specified.
 
 All overwritable components are collected in the following sections. If a built-in components uses parameters in the
 run-config, they are collected in a table in the corresponding section.
 
 #### Keras
 
+Both the built-in `build_model` and `compile_model` functions provide default values for their required hyperparameters.
+If a hyperparameter is omitted from the search space, it will be fixed to its default value. Additionally, for
+hyperparameters that support mutation (all hyperparameters of the `compile_model` function and those updated by the
+`update_model` function), search space entries that do not explicitly set the `supports_mutation` flag will be updated
+with this flag set to `True`. If either of the two functions is overwritten, this behavior is of cause disabled for the
+corresponding hyperparameters.
+
 ##### build_model
 
 A function that builds a Functional Keras multilayer perceptron for provided hyperparameter values. Supported
-hyperparameters are:
+hyperparameters and corresponding default values are:
 
-- `'num_layers'`: the number of hidden layers
-- `'units'`: the number of neurons per hidden layer (constant for all layers)
-- `'units_i'`: the number of neurons in hidden layer `i`, counting from 1 (has higher priority than `'units'`)
-- `'activation'`: the activation function
-- `'kernel_initializer'` and `'bias_initializer'`: initializers of the weights and biases of the hidden layers
-- `'l1_lambda'` and `'l2_lambda'`: the strength of the L1 and L2 regularizations
-- `'dropout'`: the dropout rate
+- `'num_layers'`: the number of hidden layers. Default: `3`
+- `'units'`: the number of neurons per hidden layer (constant for all layers). Default: `32`
+- `'units_i'`: the number of neurons in hidden layer `i`, counting from 1 (has higher priority than `'units'`). Default: `None`
+- `'activation'`: the activation function. Default: `'swish'`
+- `'kernel_initializer'` and `'bias_initializer'`: initializers of the weights and biases of the hidden layers. Defaults: `'auto'`
+- `'l1_lambda'` and `'l2_lambda'`: the strength of the L1 and L2 regularizations. Defaults: `0.0`
+- `'dropout'`: the dropout rate. Default: `0.1`
 
 The input variables are normalized using a custom non-linear normalization layer, whose documentation can be found
 [here](https://optima-docs.docs.cern.ch/keras/tools.html#OPTIMA.keras.tools.NonLinearNormalization). This layer first
 applies the non-linear transformations returned by the `get_nonlinear_scaling`-function of the [InputHandler](#inputhandler);
 supported are $\sqrt{\bullet}$, $\log_{10}(\bullet)$ or the identity. After that, a linear transformation to achieve
 zero mean and unit variance for all input features on the training dataset is applied. A batch normalization layer is
 added between each hidden layer unless the SELU activation function is used. The number of nodes in the output layer is
@@ -576,23 +583,24 @@
 ##### compile_model
 
 A function that compiles the provided Keras model. It is called after creating a new model by executing the
 `build_model`-function (with parameter `first_compile` set to `True`) and after reloading a model from a checkpoint
 (with parameter `first_compile` set to `False`). It uses the Adam optimizer with the following tunable hyperparameters
 (see https://arxiv.org/abs/1412.6980v9 for the Adam update rule):
 
-- `'learning_rate'`: $\alpha$
-- `'Adam_beta_1'`: $\beta_1$
-- `'one_minus_Adam_beta_2''`: $1 - \beta_2$
-- `'Adam_epsilon'`: $\varepsilon$
+- `'learning_rate'`: $\alpha$. Default: `0.001`
+- `'Adam_beta_1'`: $\beta_1$. Default: `0.9`
+- `'one_minus_Adam_beta_2''`: $1 - \beta_2$. Default: `0.001`
+- `'Adam_epsilon'`: $\varepsilon$. Default: `1e-7`
 
 Supported loss functions, set using the hyperparameter `'loss_function'`, are binary crossentropy loss
 (`'BinaryCrossentropy'`), categorical crossentropy loss (`'CategoricalCrossentropy'`), and Kullback–Leibler divergence
-loss (`'KLDivergence'`). For all available loss functions, the loss values can be weighted using class weights,
-controlled via hyperparameters of type `'loss_weight_class_N'` with `N` corresponding to the `N`-th class.
+loss (`'KLDivergence'`). By default, binary crossentropy loss is used. For all available loss functions, the loss values
+can be weighted using class weights, controlled via hyperparameters of type `'loss_weight_class_N'` with `N`
+corresponding to the `N`-th class.
 
 If an already compiled model is provided, the loss function and the parameters of the Adam optimizer are updated without
 losing the training state of the model. This functionality is needed to allow mutations during the Population Based
 Training step.
 
 For more details, see the documentation [here](https://optima-docs.docs.cern.ch/keras/model.html#OPTIMA.keras.model.compile_model)
 
@@ -757,64 +765,14 @@
 - `model_info`: A dictionary containing information of the current model:
   * `'name'`: The file name of the current model. This must be appended with `'.keras'` for Keras models and `'.ckpt'`
     for lightning models.
   * `'split`: An index denoting which of the `k` crossvalidation model this is. This ranges from `0` to `k-1`.
   * `'config'`: A dictionary containing the hyperparameter values of the current model.
 - `input_handler`: A reference to the InputHandler instance.
 
-#### Hyperparameter optimization
-
-##### get_hp_defaults
-
-A function that provides a default value for each hyperparameter. It is specific to the built-in `build_model`
-and `compile_model` functions. The concrete hyperparameter defaults can be found in the
-[documentation](https://optima-docs.docs.cern.ch/builtin/search_space.html#OPTIMA.builtin.search_space.get_hp_defaults).
-
-This function is only needed if the built-in `build_model` function is used, if a `build_search_space` function is
-defined in the run-config or if *only* the fine-tuning step with Population Based Training is performed and not all
-hyperparameters in the search space support mutation.
-
-##### build_search_space
-
-A function that builds the search space that is required by `Tune` from the `seach_space` defined in the run-config and
-the hyperparameter default values. It is a wrapper around the direct conversion implemented in
-`OPTIMA.core.search_space.run_config_to_tune_converter` to handle special cases specific to the built-in `build_model`
-and `compile_model` functions. Amongst others, it makes building the search space easier when optimizing the number of
-neurons in each hidden layer independently. All hyperparameters that are not present in the `search_space` but have a
-default value provided will be fixed to their default value. More details can be found in the
-[documentation](https://optima-docs.docs.cern.ch/builtin/search_space.html#OPTIMA.builtin.search_space.build_search_space).
-
-This function is only used if the built-in `build_model` function is used or if it is re-defined in the run-config.
-
-| Parameter                           | Default value | Explanation                                                                                                                 |
-|-------------------------------------|---------------|-----------------------------------------------------------------------------------------------------------------------------|
-| `optimize_units_per_layer` *(bool)* | `False`       | Should each hidden layer have the same number of neurons (`False`) or should each layer be optimized individually (`True`)? |
-
-##### limit_and_round_hyperparameters
-
-A limit that enforces limits and rounds the values of specific hyperparameters. It is provided with hyperparameter values
-that have been selected by the search algorithm. This can be necessary since Population Based Training does not respect
-the limits of the search space which can result in invalid hyperparameter values (e.g. a dropout rate larger than 1).
-Additionally, hyperparameters can be rounded. This is useful to e.g. allow Population Based Training (which only supports
-continuous search spaces) to mutate discrete hyperparameters like the batch size.
-
-This function is specific to the build-in `build_model` and `compile_model` functions. Details on the enforced limits
-can be found in the
-[documentation](https://optima-docs.docs.cern.ch/builtin/search_space.html#OPTIMA.builtin.search_space.limit_and_round_hyperparameters).
-
-##### prepare_search_space_for_PBT
-
-A function that replaces hyperparameter search space entries that do not support PBT mutation. If a prior pre- or main
-hyperparameter optimization is performed, unsupported hyperparameters are fixed to their optimized values. If only
-the fine-tuning step is performed, unsupported hyperparameters are fixed to their default values.
-
-This function is specific to the built-in `build_model` and `compile_model` functions and therefore replaces corresponding
-unsupported hyperparameters. Details can be found in the
-[documentation](https://optima-docs.docs.cern.ch/builtin/search_space.html#OPTIMA.builtin.search_space.prepare_search_space_for_PBT).
-
 #### Input variable selection
 
 ##### create_variable_sets_to_try
 
 A function that generates the sets of input variables to evaluate for each iteration of the input variable selection.
 By default, each leave-one-out subset of the remaining set of input variables is tested. To overwrite this behavior, a
 `create_variable_sets_to_try` function that accepts the following parameters needs to be defined in the run-config:
```

### Comparing `optima_ml-0.3.2a5.dev2/README.md` & `optima_ml-0.3.3a1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     - [Custom Keras objects](#custom-keras-objects)
     - [Cluster setup](#cluster-setup)
   + [Built-in functionality](#built-in-functionality)
     - [Keras](#keras-1)
     - [Inputs](#inputs-1)
     - [Trial selection](#trial-selection-1)
     - [Evaluation](#evaluation-1)
-    - [Hyperparameter optimization](#hyperparameter-optimization-1)
     - [Input variable selection](#input-variable-selection-1)
 
 ## Documentation
 
 A quick overview and instructions on how to configure OPTIMA to perform an optimization is given in [usage](#usage).
 A more detailed introduction including a description of the inner workings of OPTIMA can be found in chapter 4.2 of
 https://inspirehep.net/literature/2707309. Automatically generated API documentation is published at
@@ -244,14 +243,15 @@
 - `defaults`: Path to an alternative defaults-config. This overwrites the built-in default parameter values. (Default: `None`)
 - `cpus`: Total number of CPUs to use. (Default: `1`)
 - `gpus`: Total number of GPUs to use. (Default: `0`)
 - `mem_per_cpu`: Amount of memory to allocate per CPU (in MB). (Default: `1000`)
 - `cpus_per_trial`: Number of CPUs to use per trial. (Default: `1`)
 - `gpus_per_trial`: Number of GPUs to use per trial. This can be a fractional number if multiple trials should share a GPU. (Default: `0`)
 - `max_pending_trials`: The maximum number of trials that are allowed to be `'pending'`. (Default: `cpus / cpus_per_trial`)
+- `temp_dir`: Overwrite Ray's default root temporary directory (`/tmp/ray`). This must be an absolute path.
 
 #### Cluster
 
 If the `cluster` command line argument is set to the name of a built-in cluster or to `'custom'`, the optimization will be
 launched as a cluster job. This is done by manually launching a Ray node on each node in the job in order to build a Ray
 cluster, to which OPTIMA in then connected. Ray then takes care of distributing all tasks across the cluster. It is
 possible to run multiple optimizations in parallel on the same cluster; each job will consequently build its own Ray cluster.
@@ -350,37 +350,37 @@
 |------------------------------------|---------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `monitor_name` *(str)*             | `'val_loss'`  | Controls which metric is used as the target of the optimization and for early stopping during training. Allowed are native, weighted native, custom and composite metrics as well as all metrics reported by the ML backend during training (e.g. `"val_loss"`). Make sure to add the `"val_"`-prefix when using native, weighted native or custom metrics.                                                                                                                                                                                                                                                                                                                                                                |
 | `monitor_op` *(str)*               | `'min'`       | Is the target metric to be minimized (`'min'`) or maximized (`'max'`)?                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
 | `native_metrics` *(list)*          | `[]`          | A list of references to a metric class native to the used ML backend. Each entry must be a tuple of the form `("name", (ClassReference, {"kwarg1": kwarg1, ...}))`. Their values are calculated separately on the training and validation datasets and reported as `"train_name" and "val_name". Event weights are not applied.                                                                                                                                                                                                                                                                                                                                                                                            |
 | `weighted_native_metrics` *(list)* | `[]`          | A list of references to a metric class native to the used ML backend. Each entry must be a tuple of the form `("name", (ClassReference, {"kwarg1": kwarg1, ...}))`. Their values are calculated separately on the training and validation datasets and reported as `"train_name" and "val_name". Event weights are applied. Currently, weighted metrics are not supported for Lightning (see https://github.com/Lightning-AI/torchmetrics/issues/784).                                                                                                                                                                                                                                                                     |
 | `custom_metrics` *(list)*          | `[]`          | A list of custom metrics. Each entry must be a tuple of the form `("name", callable)`. `callable` needs to accept target values, model prediction and sample weights and return a number or a boolean. Their values are calculated at the end of each epoch separately on the training and validation datasets and reported as `"train_name" and "val_name".                                                                                                                                                                                                                                                                                                                                                               |
 | `composite_metrics` *(list)*       | `[]`          | A list of composite metrics. These are metrics that combine the values of already existing metrics. Each entry must be a tuple of the form `("name", (metric_name1, metric_name2, ...), callable)` where `callable` accepts the same number of positional arguments as the number of provided metric names and returns a number or a boolean. They are calculated at the end of each epoch and allow all native, weighted native and custom metrics as well as metrics directly reported by the ML backend (e.g. validation loss) as inputs. It is possible to mix training and validation metrics, allowing e.g. to assess the generalization gap. The value of composite metrics is reported as "name" without a prefix. |
-| `overtraining_conditions` *(list)* | `[]`          | A list of overtraining conditions. Thse are special composite metrics that should return `True` when overtraining is detected and `False` otherwise. Each entry must be a tuple of the form `("name", (metric_name1, metric_name2, ...), callable)` where `callable` accepts the same number of positional arguments as the number of provided metric names and returns a boolean. They are calculated at the end of each epoch and allow all native, weighted native, custom and composite metrics as well as metrics directly reported by the ML backend (e.g. validation loss) as inputs. Naturally, it is possible to mix training and validation metrics. The value of overtraining conditions is not reported.       |
+| `overtraining_conditions` *(list)* | `[]`          | A list of overtraining conditions. These are special composite metrics that should return `True` when overtraining is detected and `False` otherwise. Each entry must be a tuple of the form `("name", (metric_name1, metric_name2, ...), callable)` where `callable` accepts the same number of positional arguments as the number of provided metric names and returns a boolean. They are calculated at the end of each epoch and allow all native, weighted native, custom and composite metrics as well as metrics directly reported by the ML backend (e.g. validation loss) as inputs. Naturally, it is possible to mix training and validation metrics. The value of overtraining conditions is not reported.      |
 
 #### Training
 
 | Parameter                         | Default value | Explanation                                                                                                                                                                                                                                                                                                                   |
 |-----------------------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `max_epochs` *(int)*              | `200`         | The maximal number of epochs until the training is terminated. Early stopping may terminate the training earlier.                                                                                                                                                                                                             |
 | `early_stopping_patience` *(int)* | `6`           | The maximal number of consecutive epochs without an improvement of the target metric before early-stopping the training.                                                                                                                                                                                                      |
 | `overtraining_patience` *(int)*   | `6`           | The maximal number of consecutive epochs with overtraining detected (i.e. at least one overtraining condition detected overtraining) before early-stopping the training. This is ignored if no overtraining conditions are defined.                                                                                           |
 | `callbacks` *(list)*              | `[]`          | A list of references to a callback class native to the used ML backend (i.e. a subclass of `keras.callbacks.Callback` for Keras or `lightning.pytorch.callbacks.Callback` for Lightning. Each entry must be a tuple of the form `(ClassReference, {"kwarg1": kwarg1, ...})`. The callbacks are only used during the training. |
 
 #### Hyperparameter optimization
 
 ##### General
 
-| Parameter                             | Default value                                                                                                                 | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
-|---------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `optimize_on_best_value` *(bool)*     | `False`                                                                                                                       | Controls how each trial is evaluated during the hyperparameter optimization. While the target metric is calculated every epoch, *Tune* only allows accepts a single value to evaluate a trial. If `True`, the best epoch that passes all overtraining conditions (which is usually representative of the best performance possible with these hyperparameters, but may also be an outlier) is used. If `False`, the last epoch that passed all overtraining conditions (which is less likely an outlier but may be degraded due to overtraining) is used.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
-| `restore_on_best_checkpoint` *(bool)* | `True`                                                                                                                        | When resuming a trial (e.g. during Population Based Training), resume from the best epoch (`True`) or last epoch (`False`)?                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
-| `num_samples_variableOpt` *(int)*     | `1`                                                                                                                           | The number of trials (hyperparameter combinations) to try during the initial hyperparameter optimization step.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
-| `num_samples_main` *(int)*            | `1`                                                                                                                           | The number of trials (hyperparameter combinations) to try during the main hyperparameter optimization step.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
-| `num_samples_PBT` *(int)*             | `4`                                                                                                                           | The number of trials in the population for the hyperparameter fine-tuning step with Population Based Training.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
-| `search_space` *(dict)*               | see [here](https://gitlab.cern.ch/atlas-germany-dresden-vbs-group/optima/-/blob/master/OPTIMA/defaults.py?ref_type=heads#L35) | Defines the hyperparameter search space. Each dictionary entry corresponds to a hyperparameter. The corresponding range can be specified by giving a fixed value (no optimization), a list (only provided values are tried) or a tuple `(keyword, a, b, step)` where keyword can be `'uniform'` or `'log'` (in which case the values will be drawn from a uniform/logarithmic distribution between `a` and `b`) or `'normal'` (in which case the values will be drawn from a gaussian distribution with mean `a` and standard deviation `b`). `step` is optional and if provided, the distribution will be discretized with step size step. For `'uniform'` and `'log'`, the datatype of `a` decides the datatype of the drawn value. Being independent of the particular task, the batch size (with key `'batch_size'`) must always be provided as a hyperparameter, either as a fixed integer, an integer search space or a continuous search space and quantizing in the `limit_and_round_hyperparameters` function. The last option is necessary to allow Population Based Training to optimize the batch size. |
+| Parameter                             | Default value                                                                                                                 | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+|---------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `optimize_on_best_value` *(bool)*     | `False`                                                                                                                       | Controls how each trial is evaluated during the hyperparameter optimization. While the target metric is calculated every epoch, *Tune* only allows accepts a single value to evaluate a trial. If `True`, the best epoch that passes all overtraining conditions (which is usually representative of the best performance possible with these hyperparameters, but may also be an outlier) is used. If `False`, the last epoch that passed all overtraining conditions (which is less likely an outlier but may be degraded due to overtraining) is used.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| `restore_on_best_checkpoint` *(bool)* | `True`                                                                                                                        | When resuming a trial (e.g. during Population Based Training), resume from the best epoch (`True`) or last epoch (`False`)?                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+| `num_samples_variableOpt` *(int)*     | `1`                                                                                                                           | The number of trials (hyperparameter combinations) to try during the initial hyperparameter optimization step.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+| `num_samples_main` *(int)*            | `1`                                                                                                                           | The number of trials (hyperparameter combinations) to try during the main hyperparameter optimization step.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+| `num_samples_PBT` *(int)*             | `4`                                                                                                                           | The number of trials in the population for the hyperparameter fine-tuning step with Population Based Training.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+| `search_space` *(dict)*               | see [here](https://gitlab.cern.ch/atlas-germany-dresden-vbs-group/optima/-/blob/master/OPTIMA/defaults.py?ref_type=heads#L42) | Defines the hyperparameter search space. Each dictionary entry corresponds to a hyperparameter, and the corresponding search space is defined using a dictionary with the following allowed key-value pairs:<br><ul><li>`'type'`: Specifies if a range of values (`'range'`) or a list of allowed values (`'choice'`) defines the search space.</li><li>`'bounds'`: Specifies the lower and upper bounds for range search spaces. This can be given as a list or tuple of type `(lower_bound, upper_bound)`. Alternatively, conditional bounds that depend on the values of other hyperparameters can be specified as a tuple of type `(hp_depends_tuple, callable)`. Here, `hp_depends_tuple` is a tuple of hyperparameters the bounds depend on (i.e. each entry must correspond to another key in the search space). The `callable` will be provided with the values of the hyperparameters specified in `hp_depends_tuple` as positional arguments and needs to return a list or tuple of type `(lower_bound, upper_bound)`. Conditional bounds are not supported for Population Based Training. This is only used for range search spaces.</li><li>`'value_type'`: Specifies if an integer (`'int'`) or float (`'float'`) value should be suggested. Defaults to `'float'`. This is only used for range search spaces.</li><li>`'sampling'`: Specifies if the search space should be sampled uniformly (`'uniform'`), logarithmically (`'log'`) or gaussian distributed (`'normal'`). Gaussian sampled integer search spaces are not supported. Defaults to `'uniform'`. This is only used for range search spaces.</li><li>`'mean'`: Specifies the mean of the gaussian sampling. This can be given as a float or integer. Only used for range search spaces and `'sampling'` set to `'normal'`.</li><li>`'std'`: Specifies the standard deviation of the gaussian sampling. This can be given as a float or integer. Only used for range search spaces and `'sampling'` set to `'normal'`.</li><li>`'step'`: Used to quantize range search spaces. For integer search spaces, this must be an integer. For float search spaces, this can be an integer or a float. For log-sampled search spaces, setting a step size is not supported. Defaults to `None` (i.e. unquantized) for float and `1` for integer parameters. This is only used for range search spaces.</li><li>`'values'`: Specifies the allowed values for choice search spaces. This can be a list or a tuple. Alternatively, conditional values that depend on the values of other hyperparameters can be specified as a tuple of type `(hp_depends_tuple, callable)`. Here, `hp_depends_tuple` is a tuple of hyperparameters the values depend on (i.e. each entry must correspond to another key in the search space). The `callable` will be provided with the values of the hyperparameters specified in `hp_depends_tuple` as positional arguments and needs to return a list or tuple of allowed values. Conditional values are not supported for Population Based Training. This is only used for choice search spaces.</li><li>`'supports_mutation'`: A `bool` that specifies if this hyperparameter can be altered during the training without loosing the training state. Only these hyperparameters can be optimized with Population Based Training. The remaining hyperparameters will be fixed to the best value found during the previous hyperparameter optimization step. If only the Population Based Training step is performed, all hyperparameters need to be fixed or mutatable.</li><li>`'only'`: Used to build hierarchical search spaces where not all hyperparameters are always needed (e.g. the number of neurons in the fourth layer are only needed if the number of layers is at least four). If provided, this needs to be a tuple of type `(hp_depends_tuple, callable)`. Here, `hp_depends_tuple` is a tuple of hyperparameters that are necessary to decide if this hyperparameter is needed (i.e. each entry must correspond to another key in the search space). The `callable` will be provided with the values of the hyperparameters specified in `hp_depends_tuple` as positional arguments and needs to return a `bool` that signifies if a value should be suggested for this hyperparameter. If the condition is evaluated as `False`, the value if the hyperparameter is explicitly set to `None` and provided as such to all conditions that depend on this hyperparameter. This allows defining multiple dependency layers where, e.g., `B` is only needed if `A > 0` and `C` is only needed if `B` exists and `B > 0`. Rejected hyperparameters will, however, not be added to the `model_config`. Hierarchical search spaces are not supported for Population Based Training.</li></ul>Any search space entry that is not a dictionary is considered fixed and the corresponding hyperparameter will not be optimized but still added to the `model_config`. Being independent of the particular task, the batch size (with key `'batch_size'`) must always be provided as a hyperparameter, either as a fixed integer or as an integer range search space. |
 
 
 ##### Bayesian optimization (Optuna)
 
 | Parameter                       | Default value | Explanation                                                                                                                                |
 |---------------------------------|---------------|--------------------------------------------------------------------------------------------------------------------------------------------|
 | `use_TPESampler` *(bool)*       | `True`        | Use Optuna's Tree-structured Parzen Estimator algorithm or random sampling?                                                                |
@@ -388,19 +388,19 @@
 | `use_ASHAScheduler` *(bool)*    | `True`        | Use the Asynchronous HyperBand scheduler (ASHA) to prune trials or not?                                                                    |
 | `ASHA_grace_period` *(int)*     | `15`          | The minimum number of epochs to wait before the ASHA scheduler is allowed to prune a trial. Only used if `use_ASHAScheduler` is `True`.    |
 | `ASHA_max_t` *(int)*            | `max_epochs`  | The end point of the reduction with ASHA. Only used if `use_ASHAScheduler` is `True`.                                                      |
 | `ASHA_reduction_factor` *(int)* | `2`           | Controls which fraction of trials is terminated at each point by ASHA. A value of `2` corresponds to the termination of 50% of all trials. |
 
 ##### Population Based Training
 
-| Parameter                          | Default value | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
-|------------------------------------|---------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `use_fit_results_for_PBT` *(bool)* | `True`        | PBT cannot optimize all hyperparameters. If the inital or main hyperparameter optimization step was run before, all unsupported hyperparameters are fixed to their optimized values from the previous optimization step. If `use_fit_results_for_PBT` is `True`, the best-fit results are used, otherwise the best-value results are used. If only the PBT step is performed, unsupported parameters are set to the default values defined by `get_hp_defaults()`. |
-| `perturbation_interval` *(int)*    | `6`           | The number of epochs to train between each perturbation of a trial.                                                                                                                                                                                                                                                                                                                                                                                                |
-| `burn_in_period` *(int)*           | `6`           | The number of epochs to wait before the first perturbation of a trial.                                                                                                                                                                                                                                                                                                                                                                                             |
+| Parameter                          | Default value | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
+|------------------------------------|---------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `use_fit_results_for_PBT` *(bool)* | `True`        | PBT is only applied to hyperparameters that are marked with `'supports_mutation'` set to `True`. If the initial and/or main hyperparameter optimization step was run before, all unsupported hyperparameters are fixed to their optimized values from the previous optimization step. If `use_fit_results_for_PBT` is `True`, the best-fit results are used, otherwise the best-value results are used. If only the PBT step is performed, all provided hyperparameters need to be fixed or support mutation. |
+| `perturbation_interval` *(int)*    | `6`           | The number of epochs to train between each perturbation of a trial.                                                                                                                                                                                                                                                                                                                                                                                                                                           |
+| `burn_in_period` *(int)*           | `6`           | The number of epochs to wait before the first perturbation of a trial.                                                                                                                                                                                                                                                                                                                                                                                                                                        |
 
 #### Trial selection
 
 To select the best set of hyperparameters and the number of epochs to train from the pool of tested trials, two
 independent algorithms are used:
 
 - **best-value**: the best trial is given by the best reported value of the target metric (i.e. best single epoch) while
@@ -506,26 +506,33 @@
 as the built-in counterpart, unless otherwise specified.
 
 All overwritable components are collected in the following sections. If a built-in components uses parameters in the
 run-config, they are collected in a table in the corresponding section.
 
 #### Keras
 
+Both the built-in `build_model` and `compile_model` functions provide default values for their required hyperparameters.
+If a hyperparameter is omitted from the search space, it will be fixed to its default value. Additionally, for
+hyperparameters that support mutation (all hyperparameters of the `compile_model` function and those updated by the
+`update_model` function), search space entries that do not explicitly set the `supports_mutation` flag will be updated
+with this flag set to `True`. If either of the two functions is overwritten, this behavior is of cause disabled for the
+corresponding hyperparameters.
+
 ##### build_model
 
 A function that builds a Functional Keras multilayer perceptron for provided hyperparameter values. Supported
-hyperparameters are:
+hyperparameters and corresponding default values are:
 
-- `'num_layers'`: the number of hidden layers
-- `'units'`: the number of neurons per hidden layer (constant for all layers)
-- `'units_i'`: the number of neurons in hidden layer `i`, counting from 1 (has higher priority than `'units'`)
-- `'activation'`: the activation function
-- `'kernel_initializer'` and `'bias_initializer'`: initializers of the weights and biases of the hidden layers
-- `'l1_lambda'` and `'l2_lambda'`: the strength of the L1 and L2 regularizations
-- `'dropout'`: the dropout rate
+- `'num_layers'`: the number of hidden layers. Default: `3`
+- `'units'`: the number of neurons per hidden layer (constant for all layers). Default: `32`
+- `'units_i'`: the number of neurons in hidden layer `i`, counting from 1 (has higher priority than `'units'`). Default: `None`
+- `'activation'`: the activation function. Default: `'swish'`
+- `'kernel_initializer'` and `'bias_initializer'`: initializers of the weights and biases of the hidden layers. Defaults: `'auto'`
+- `'l1_lambda'` and `'l2_lambda'`: the strength of the L1 and L2 regularizations. Defaults: `0.0`
+- `'dropout'`: the dropout rate. Default: `0.1`
 
 The input variables are normalized using a custom non-linear normalization layer, whose documentation can be found
 [here](https://optima-docs.docs.cern.ch/keras/tools.html#OPTIMA.keras.tools.NonLinearNormalization). This layer first
 applies the non-linear transformations returned by the `get_nonlinear_scaling`-function of the [InputHandler](#inputhandler);
 supported are $\sqrt{\bullet}$, $\log_{10}(\bullet)$ or the identity. After that, a linear transformation to achieve
 zero mean and unit variance for all input features on the training dataset is applied. A batch normalization layer is
 added between each hidden layer unless the SELU activation function is used. The number of nodes in the output layer is
@@ -537,23 +544,24 @@
 ##### compile_model
 
 A function that compiles the provided Keras model. It is called after creating a new model by executing the
 `build_model`-function (with parameter `first_compile` set to `True`) and after reloading a model from a checkpoint
 (with parameter `first_compile` set to `False`). It uses the Adam optimizer with the following tunable hyperparameters
 (see https://arxiv.org/abs/1412.6980v9 for the Adam update rule):
 
-- `'learning_rate'`: $\alpha$
-- `'Adam_beta_1'`: $\beta_1$
-- `'one_minus_Adam_beta_2''`: $1 - \beta_2$
-- `'Adam_epsilon'`: $\varepsilon$
+- `'learning_rate'`: $\alpha$. Default: `0.001`
+- `'Adam_beta_1'`: $\beta_1$. Default: `0.9`
+- `'one_minus_Adam_beta_2''`: $1 - \beta_2$. Default: `0.001`
+- `'Adam_epsilon'`: $\varepsilon$. Default: `1e-7`
 
 Supported loss functions, set using the hyperparameter `'loss_function'`, are binary crossentropy loss
 (`'BinaryCrossentropy'`), categorical crossentropy loss (`'CategoricalCrossentropy'`), and Kullback–Leibler divergence
-loss (`'KLDivergence'`). For all available loss functions, the loss values can be weighted using class weights,
-controlled via hyperparameters of type `'loss_weight_class_N'` with `N` corresponding to the `N`-th class.
+loss (`'KLDivergence'`). By default, binary crossentropy loss is used. For all available loss functions, the loss values
+can be weighted using class weights, controlled via hyperparameters of type `'loss_weight_class_N'` with `N`
+corresponding to the `N`-th class.
 
 If an already compiled model is provided, the loss function and the parameters of the Adam optimizer are updated without
 losing the training state of the model. This functionality is needed to allow mutations during the Population Based
 Training step.
 
 For more details, see the documentation [here](https://optima-docs.docs.cern.ch/keras/model.html#OPTIMA.keras.model.compile_model)
 
@@ -718,64 +726,14 @@
 - `model_info`: A dictionary containing information of the current model:
   * `'name'`: The file name of the current model. This must be appended with `'.keras'` for Keras models and `'.ckpt'`
     for lightning models.
   * `'split`: An index denoting which of the `k` crossvalidation model this is. This ranges from `0` to `k-1`.
   * `'config'`: A dictionary containing the hyperparameter values of the current model.
 - `input_handler`: A reference to the InputHandler instance.
 
-#### Hyperparameter optimization
-
-##### get_hp_defaults
-
-A function that provides a default value for each hyperparameter. It is specific to the built-in `build_model`
-and `compile_model` functions. The concrete hyperparameter defaults can be found in the
-[documentation](https://optima-docs.docs.cern.ch/builtin/search_space.html#OPTIMA.builtin.search_space.get_hp_defaults).
-
-This function is only needed if the built-in `build_model` function is used, if a `build_search_space` function is
-defined in the run-config or if *only* the fine-tuning step with Population Based Training is performed and not all
-hyperparameters in the search space support mutation.
-
-##### build_search_space
-
-A function that builds the search space that is required by `Tune` from the `seach_space` defined in the run-config and
-the hyperparameter default values. It is a wrapper around the direct conversion implemented in
-`OPTIMA.core.search_space.run_config_to_tune_converter` to handle special cases specific to the built-in `build_model`
-and `compile_model` functions. Amongst others, it makes building the search space easier when optimizing the number of
-neurons in each hidden layer independently. All hyperparameters that are not present in the `search_space` but have a
-default value provided will be fixed to their default value. More details can be found in the
-[documentation](https://optima-docs.docs.cern.ch/builtin/search_space.html#OPTIMA.builtin.search_space.build_search_space).
-
-This function is only used if the built-in `build_model` function is used or if it is re-defined in the run-config.
-
-| Parameter                           | Default value | Explanation                                                                                                                 |
-|-------------------------------------|---------------|-----------------------------------------------------------------------------------------------------------------------------|
-| `optimize_units_per_layer` *(bool)* | `False`       | Should each hidden layer have the same number of neurons (`False`) or should each layer be optimized individually (`True`)? |
-
-##### limit_and_round_hyperparameters
-
-A limit that enforces limits and rounds the values of specific hyperparameters. It is provided with hyperparameter values
-that have been selected by the search algorithm. This can be necessary since Population Based Training does not respect
-the limits of the search space which can result in invalid hyperparameter values (e.g. a dropout rate larger than 1).
-Additionally, hyperparameters can be rounded. This is useful to e.g. allow Population Based Training (which only supports
-continuous search spaces) to mutate discrete hyperparameters like the batch size.
-
-This function is specific to the build-in `build_model` and `compile_model` functions. Details on the enforced limits
-can be found in the
-[documentation](https://optima-docs.docs.cern.ch/builtin/search_space.html#OPTIMA.builtin.search_space.limit_and_round_hyperparameters).
-
-##### prepare_search_space_for_PBT
-
-A function that replaces hyperparameter search space entries that do not support PBT mutation. If a prior pre- or main
-hyperparameter optimization is performed, unsupported hyperparameters are fixed to their optimized values. If only
-the fine-tuning step is performed, unsupported hyperparameters are fixed to their default values.
-
-This function is specific to the built-in `build_model` and `compile_model` functions and therefore replaces corresponding
-unsupported hyperparameters. Details can be found in the
-[documentation](https://optima-docs.docs.cern.ch/builtin/search_space.html#OPTIMA.builtin.search_space.prepare_search_space_for_PBT).
-
 #### Input variable selection
 
 ##### create_variable_sets_to_try
 
 A function that generates the sets of input variables to evaluate for each iteration of the input variable selection.
 By default, each leave-one-out subset of the remaining set of input variables is tested. To overwrite this behavior, a
 `create_variable_sets_to_try` function that accepts the following parameters needs to be defined in the run-config:
```

### Comparing `optima_ml-0.3.2a5.dev2/optima_ml.egg-info/PKG-INFO` & `optima_ml-0.3.3a1/optima_ml.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optima-ml
-Version: 0.3.2a5.dev2
+Version: 0.3.3a1
 Summary: Distributed hyperparameter optimization and input variable selection for artificial neural networks.
 Home-page: https://gitlab.cern.ch/atlas-germany-dresden-vbs-group/optima
 Author: E. Bachmann
 Author-email: erik.bachmann@tu-dresden.de
 License: GPL
 Platform: linux
 Platform: darwin
@@ -16,16 +16,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: optuna==3.5.0
-Requires-Dist: ray[data,train,tune]==2.9.2
+Requires-Dist: optuna==3.6
+Requires-Dist: ray[data,train,tune]==2.11
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: seaborn
 Requires-Dist: tabulate
 Requires-Dist: scikit-learn
@@ -70,15 +70,14 @@
     - [Custom Keras objects](#custom-keras-objects)
     - [Cluster setup](#cluster-setup)
   + [Built-in functionality](#built-in-functionality)
     - [Keras](#keras-1)
     - [Inputs](#inputs-1)
     - [Trial selection](#trial-selection-1)
     - [Evaluation](#evaluation-1)
-    - [Hyperparameter optimization](#hyperparameter-optimization-1)
     - [Input variable selection](#input-variable-selection-1)
 
 ## Documentation
 
 A quick overview and instructions on how to configure OPTIMA to perform an optimization is given in [usage](#usage).
 A more detailed introduction including a description of the inner workings of OPTIMA can be found in chapter 4.2 of
 https://inspirehep.net/literature/2707309. Automatically generated API documentation is published at
@@ -283,14 +282,15 @@
 - `defaults`: Path to an alternative defaults-config. This overwrites the built-in default parameter values. (Default: `None`)
 - `cpus`: Total number of CPUs to use. (Default: `1`)
 - `gpus`: Total number of GPUs to use. (Default: `0`)
 - `mem_per_cpu`: Amount of memory to allocate per CPU (in MB). (Default: `1000`)
 - `cpus_per_trial`: Number of CPUs to use per trial. (Default: `1`)
 - `gpus_per_trial`: Number of GPUs to use per trial. This can be a fractional number if multiple trials should share a GPU. (Default: `0`)
 - `max_pending_trials`: The maximum number of trials that are allowed to be `'pending'`. (Default: `cpus / cpus_per_trial`)
+- `temp_dir`: Overwrite Ray's default root temporary directory (`/tmp/ray`). This must be an absolute path.
 
 #### Cluster
 
 If the `cluster` command line argument is set to the name of a built-in cluster or to `'custom'`, the optimization will be
 launched as a cluster job. This is done by manually launching a Ray node on each node in the job in order to build a Ray
 cluster, to which OPTIMA in then connected. Ray then takes care of distributing all tasks across the cluster. It is
 possible to run multiple optimizations in parallel on the same cluster; each job will consequently build its own Ray cluster.
@@ -389,37 +389,37 @@
 |------------------------------------|---------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `monitor_name` *(str)*             | `'val_loss'`  | Controls which metric is used as the target of the optimization and for early stopping during training. Allowed are native, weighted native, custom and composite metrics as well as all metrics reported by the ML backend during training (e.g. `"val_loss"`). Make sure to add the `"val_"`-prefix when using native, weighted native or custom metrics.                                                                                                                                                                                                                                                                                                                                                                |
 | `monitor_op` *(str)*               | `'min'`       | Is the target metric to be minimized (`'min'`) or maximized (`'max'`)?                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
 | `native_metrics` *(list)*          | `[]`          | A list of references to a metric class native to the used ML backend. Each entry must be a tuple of the form `("name", (ClassReference, {"kwarg1": kwarg1, ...}))`. Their values are calculated separately on the training and validation datasets and reported as `"train_name" and "val_name". Event weights are not applied.                                                                                                                                                                                                                                                                                                                                                                                            |
 | `weighted_native_metrics` *(list)* | `[]`          | A list of references to a metric class native to the used ML backend. Each entry must be a tuple of the form `("name", (ClassReference, {"kwarg1": kwarg1, ...}))`. Their values are calculated separately on the training and validation datasets and reported as `"train_name" and "val_name". Event weights are applied. Currently, weighted metrics are not supported for Lightning (see https://github.com/Lightning-AI/torchmetrics/issues/784).                                                                                                                                                                                                                                                                     |
 | `custom_metrics` *(list)*          | `[]`          | A list of custom metrics. Each entry must be a tuple of the form `("name", callable)`. `callable` needs to accept target values, model prediction and sample weights and return a number or a boolean. Their values are calculated at the end of each epoch separately on the training and validation datasets and reported as `"train_name" and "val_name".                                                                                                                                                                                                                                                                                                                                                               |
 | `composite_metrics` *(list)*       | `[]`          | A list of composite metrics. These are metrics that combine the values of already existing metrics. Each entry must be a tuple of the form `("name", (metric_name1, metric_name2, ...), callable)` where `callable` accepts the same number of positional arguments as the number of provided metric names and returns a number or a boolean. They are calculated at the end of each epoch and allow all native, weighted native and custom metrics as well as metrics directly reported by the ML backend (e.g. validation loss) as inputs. It is possible to mix training and validation metrics, allowing e.g. to assess the generalization gap. The value of composite metrics is reported as "name" without a prefix. |
-| `overtraining_conditions` *(list)* | `[]`          | A list of overtraining conditions. Thse are special composite metrics that should return `True` when overtraining is detected and `False` otherwise. Each entry must be a tuple of the form `("name", (metric_name1, metric_name2, ...), callable)` where `callable` accepts the same number of positional arguments as the number of provided metric names and returns a boolean. They are calculated at the end of each epoch and allow all native, weighted native, custom and composite metrics as well as metrics directly reported by the ML backend (e.g. validation loss) as inputs. Naturally, it is possible to mix training and validation metrics. The value of overtraining conditions is not reported.       |
+| `overtraining_conditions` *(list)* | `[]`          | A list of overtraining conditions. These are special composite metrics that should return `True` when overtraining is detected and `False` otherwise. Each entry must be a tuple of the form `("name", (metric_name1, metric_name2, ...), callable)` where `callable` accepts the same number of positional arguments as the number of provided metric names and returns a boolean. They are calculated at the end of each epoch and allow all native, weighted native, custom and composite metrics as well as metrics directly reported by the ML backend (e.g. validation loss) as inputs. Naturally, it is possible to mix training and validation metrics. The value of overtraining conditions is not reported.      |
 
 #### Training
 
 | Parameter                         | Default value | Explanation                                                                                                                                                                                                                                                                                                                   |
 |-----------------------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `max_epochs` *(int)*              | `200`         | The maximal number of epochs until the training is terminated. Early stopping may terminate the training earlier.                                                                                                                                                                                                             |
 | `early_stopping_patience` *(int)* | `6`           | The maximal number of consecutive epochs without an improvement of the target metric before early-stopping the training.                                                                                                                                                                                                      |
 | `overtraining_patience` *(int)*   | `6`           | The maximal number of consecutive epochs with overtraining detected (i.e. at least one overtraining condition detected overtraining) before early-stopping the training. This is ignored if no overtraining conditions are defined.                                                                                           |
 | `callbacks` *(list)*              | `[]`          | A list of references to a callback class native to the used ML backend (i.e. a subclass of `keras.callbacks.Callback` for Keras or `lightning.pytorch.callbacks.Callback` for Lightning. Each entry must be a tuple of the form `(ClassReference, {"kwarg1": kwarg1, ...})`. The callbacks are only used during the training. |
 
 #### Hyperparameter optimization
 
 ##### General
 
-| Parameter                             | Default value                                                                                                                 | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
-|---------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `optimize_on_best_value` *(bool)*     | `False`                                                                                                                       | Controls how each trial is evaluated during the hyperparameter optimization. While the target metric is calculated every epoch, *Tune* only allows accepts a single value to evaluate a trial. If `True`, the best epoch that passes all overtraining conditions (which is usually representative of the best performance possible with these hyperparameters, but may also be an outlier) is used. If `False`, the last epoch that passed all overtraining conditions (which is less likely an outlier but may be degraded due to overtraining) is used.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
-| `restore_on_best_checkpoint` *(bool)* | `True`                                                                                                                        | When resuming a trial (e.g. during Population Based Training), resume from the best epoch (`True`) or last epoch (`False`)?                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
-| `num_samples_variableOpt` *(int)*     | `1`                                                                                                                           | The number of trials (hyperparameter combinations) to try during the initial hyperparameter optimization step.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
-| `num_samples_main` *(int)*            | `1`                                                                                                                           | The number of trials (hyperparameter combinations) to try during the main hyperparameter optimization step.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
-| `num_samples_PBT` *(int)*             | `4`                                                                                                                           | The number of trials in the population for the hyperparameter fine-tuning step with Population Based Training.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
-| `search_space` *(dict)*               | see [here](https://gitlab.cern.ch/atlas-germany-dresden-vbs-group/optima/-/blob/master/OPTIMA/defaults.py?ref_type=heads#L35) | Defines the hyperparameter search space. Each dictionary entry corresponds to a hyperparameter. The corresponding range can be specified by giving a fixed value (no optimization), a list (only provided values are tried) or a tuple `(keyword, a, b, step)` where keyword can be `'uniform'` or `'log'` (in which case the values will be drawn from a uniform/logarithmic distribution between `a` and `b`) or `'normal'` (in which case the values will be drawn from a gaussian distribution with mean `a` and standard deviation `b`). `step` is optional and if provided, the distribution will be discretized with step size step. For `'uniform'` and `'log'`, the datatype of `a` decides the datatype of the drawn value. Being independent of the particular task, the batch size (with key `'batch_size'`) must always be provided as a hyperparameter, either as a fixed integer, an integer search space or a continuous search space and quantizing in the `limit_and_round_hyperparameters` function. The last option is necessary to allow Population Based Training to optimize the batch size. |
+| Parameter                             | Default value                                                                                                                 | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+|---------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `optimize_on_best_value` *(bool)*     | `False`                                                                                                                       | Controls how each trial is evaluated during the hyperparameter optimization. While the target metric is calculated every epoch, *Tune* only allows accepts a single value to evaluate a trial. If `True`, the best epoch that passes all overtraining conditions (which is usually representative of the best performance possible with these hyperparameters, but may also be an outlier) is used. If `False`, the last epoch that passed all overtraining conditions (which is less likely an outlier but may be degraded due to overtraining) is used.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| `restore_on_best_checkpoint` *(bool)* | `True`                                                                                                                        | When resuming a trial (e.g. during Population Based Training), resume from the best epoch (`True`) or last epoch (`False`)?                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+| `num_samples_variableOpt` *(int)*     | `1`                                                                                                                           | The number of trials (hyperparameter combinations) to try during the initial hyperparameter optimization step.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+| `num_samples_main` *(int)*            | `1`                                                                                                                           | The number of trials (hyperparameter combinations) to try during the main hyperparameter optimization step.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+| `num_samples_PBT` *(int)*             | `4`                                                                                                                           | The number of trials in the population for the hyperparameter fine-tuning step with Population Based Training.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+| `search_space` *(dict)*               | see [here](https://gitlab.cern.ch/atlas-germany-dresden-vbs-group/optima/-/blob/master/OPTIMA/defaults.py?ref_type=heads#L42) | Defines the hyperparameter search space. Each dictionary entry corresponds to a hyperparameter, and the corresponding search space is defined using a dictionary with the following allowed key-value pairs:<br><ul><li>`'type'`: Specifies if a range of values (`'range'`) or a list of allowed values (`'choice'`) defines the search space.</li><li>`'bounds'`: Specifies the lower and upper bounds for range search spaces. This can be given as a list or tuple of type `(lower_bound, upper_bound)`. Alternatively, conditional bounds that depend on the values of other hyperparameters can be specified as a tuple of type `(hp_depends_tuple, callable)`. Here, `hp_depends_tuple` is a tuple of hyperparameters the bounds depend on (i.e. each entry must correspond to another key in the search space). The `callable` will be provided with the values of the hyperparameters specified in `hp_depends_tuple` as positional arguments and needs to return a list or tuple of type `(lower_bound, upper_bound)`. Conditional bounds are not supported for Population Based Training. This is only used for range search spaces.</li><li>`'value_type'`: Specifies if an integer (`'int'`) or float (`'float'`) value should be suggested. Defaults to `'float'`. This is only used for range search spaces.</li><li>`'sampling'`: Specifies if the search space should be sampled uniformly (`'uniform'`), logarithmically (`'log'`) or gaussian distributed (`'normal'`). Gaussian sampled integer search spaces are not supported. Defaults to `'uniform'`. This is only used for range search spaces.</li><li>`'mean'`: Specifies the mean of the gaussian sampling. This can be given as a float or integer. Only used for range search spaces and `'sampling'` set to `'normal'`.</li><li>`'std'`: Specifies the standard deviation of the gaussian sampling. This can be given as a float or integer. Only used for range search spaces and `'sampling'` set to `'normal'`.</li><li>`'step'`: Used to quantize range search spaces. For integer search spaces, this must be an integer. For float search spaces, this can be an integer or a float. For log-sampled search spaces, setting a step size is not supported. Defaults to `None` (i.e. unquantized) for float and `1` for integer parameters. This is only used for range search spaces.</li><li>`'values'`: Specifies the allowed values for choice search spaces. This can be a list or a tuple. Alternatively, conditional values that depend on the values of other hyperparameters can be specified as a tuple of type `(hp_depends_tuple, callable)`. Here, `hp_depends_tuple` is a tuple of hyperparameters the values depend on (i.e. each entry must correspond to another key in the search space). The `callable` will be provided with the values of the hyperparameters specified in `hp_depends_tuple` as positional arguments and needs to return a list or tuple of allowed values. Conditional values are not supported for Population Based Training. This is only used for choice search spaces.</li><li>`'supports_mutation'`: A `bool` that specifies if this hyperparameter can be altered during the training without loosing the training state. Only these hyperparameters can be optimized with Population Based Training. The remaining hyperparameters will be fixed to the best value found during the previous hyperparameter optimization step. If only the Population Based Training step is performed, all hyperparameters need to be fixed or mutatable.</li><li>`'only'`: Used to build hierarchical search spaces where not all hyperparameters are always needed (e.g. the number of neurons in the fourth layer are only needed if the number of layers is at least four). If provided, this needs to be a tuple of type `(hp_depends_tuple, callable)`. Here, `hp_depends_tuple` is a tuple of hyperparameters that are necessary to decide if this hyperparameter is needed (i.e. each entry must correspond to another key in the search space). The `callable` will be provided with the values of the hyperparameters specified in `hp_depends_tuple` as positional arguments and needs to return a `bool` that signifies if a value should be suggested for this hyperparameter. If the condition is evaluated as `False`, the value if the hyperparameter is explicitly set to `None` and provided as such to all conditions that depend on this hyperparameter. This allows defining multiple dependency layers where, e.g., `B` is only needed if `A > 0` and `C` is only needed if `B` exists and `B > 0`. Rejected hyperparameters will, however, not be added to the `model_config`. Hierarchical search spaces are not supported for Population Based Training.</li></ul>Any search space entry that is not a dictionary is considered fixed and the corresponding hyperparameter will not be optimized but still added to the `model_config`. Being independent of the particular task, the batch size (with key `'batch_size'`) must always be provided as a hyperparameter, either as a fixed integer or as an integer range search space. |
 
 
 ##### Bayesian optimization (Optuna)
 
 | Parameter                       | Default value | Explanation                                                                                                                                |
 |---------------------------------|---------------|--------------------------------------------------------------------------------------------------------------------------------------------|
 | `use_TPESampler` *(bool)*       | `True`        | Use Optuna's Tree-structured Parzen Estimator algorithm or random sampling?                                                                |
@@ -427,19 +427,19 @@
 | `use_ASHAScheduler` *(bool)*    | `True`        | Use the Asynchronous HyperBand scheduler (ASHA) to prune trials or not?                                                                    |
 | `ASHA_grace_period` *(int)*     | `15`          | The minimum number of epochs to wait before the ASHA scheduler is allowed to prune a trial. Only used if `use_ASHAScheduler` is `True`.    |
 | `ASHA_max_t` *(int)*            | `max_epochs`  | The end point of the reduction with ASHA. Only used if `use_ASHAScheduler` is `True`.                                                      |
 | `ASHA_reduction_factor` *(int)* | `2`           | Controls which fraction of trials is terminated at each point by ASHA. A value of `2` corresponds to the termination of 50% of all trials. |
 
 ##### Population Based Training
 
-| Parameter                          | Default value | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
-|------------------------------------|---------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `use_fit_results_for_PBT` *(bool)* | `True`        | PBT cannot optimize all hyperparameters. If the inital or main hyperparameter optimization step was run before, all unsupported hyperparameters are fixed to their optimized values from the previous optimization step. If `use_fit_results_for_PBT` is `True`, the best-fit results are used, otherwise the best-value results are used. If only the PBT step is performed, unsupported parameters are set to the default values defined by `get_hp_defaults()`. |
-| `perturbation_interval` *(int)*    | `6`           | The number of epochs to train between each perturbation of a trial.                                                                                                                                                                                                                                                                                                                                                                                                |
-| `burn_in_period` *(int)*           | `6`           | The number of epochs to wait before the first perturbation of a trial.                                                                                                                                                                                                                                                                                                                                                                                             |
+| Parameter                          | Default value | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
+|------------------------------------|---------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `use_fit_results_for_PBT` *(bool)* | `True`        | PBT is only applied to hyperparameters that are marked with `'supports_mutation'` set to `True`. If the initial and/or main hyperparameter optimization step was run before, all unsupported hyperparameters are fixed to their optimized values from the previous optimization step. If `use_fit_results_for_PBT` is `True`, the best-fit results are used, otherwise the best-value results are used. If only the PBT step is performed, all provided hyperparameters need to be fixed or support mutation. |
+| `perturbation_interval` *(int)*    | `6`           | The number of epochs to train between each perturbation of a trial.                                                                                                                                                                                                                                                                                                                                                                                                                                           |
+| `burn_in_period` *(int)*           | `6`           | The number of epochs to wait before the first perturbation of a trial.                                                                                                                                                                                                                                                                                                                                                                                                                                        |
 
 #### Trial selection
 
 To select the best set of hyperparameters and the number of epochs to train from the pool of tested trials, two
 independent algorithms are used:
 
 - **best-value**: the best trial is given by the best reported value of the target metric (i.e. best single epoch) while
@@ -545,26 +545,33 @@
 as the built-in counterpart, unless otherwise specified.
 
 All overwritable components are collected in the following sections. If a built-in components uses parameters in the
 run-config, they are collected in a table in the corresponding section.
 
 #### Keras
 
+Both the built-in `build_model` and `compile_model` functions provide default values for their required hyperparameters.
+If a hyperparameter is omitted from the search space, it will be fixed to its default value. Additionally, for
+hyperparameters that support mutation (all hyperparameters of the `compile_model` function and those updated by the
+`update_model` function), search space entries that do not explicitly set the `supports_mutation` flag will be updated
+with this flag set to `True`. If either of the two functions is overwritten, this behavior is of cause disabled for the
+corresponding hyperparameters.
+
 ##### build_model
 
 A function that builds a Functional Keras multilayer perceptron for provided hyperparameter values. Supported
-hyperparameters are:
+hyperparameters and corresponding default values are:
 
-- `'num_layers'`: the number of hidden layers
-- `'units'`: the number of neurons per hidden layer (constant for all layers)
-- `'units_i'`: the number of neurons in hidden layer `i`, counting from 1 (has higher priority than `'units'`)
-- `'activation'`: the activation function
-- `'kernel_initializer'` and `'bias_initializer'`: initializers of the weights and biases of the hidden layers
-- `'l1_lambda'` and `'l2_lambda'`: the strength of the L1 and L2 regularizations
-- `'dropout'`: the dropout rate
+- `'num_layers'`: the number of hidden layers. Default: `3`
+- `'units'`: the number of neurons per hidden layer (constant for all layers). Default: `32`
+- `'units_i'`: the number of neurons in hidden layer `i`, counting from 1 (has higher priority than `'units'`). Default: `None`
+- `'activation'`: the activation function. Default: `'swish'`
+- `'kernel_initializer'` and `'bias_initializer'`: initializers of the weights and biases of the hidden layers. Defaults: `'auto'`
+- `'l1_lambda'` and `'l2_lambda'`: the strength of the L1 and L2 regularizations. Defaults: `0.0`
+- `'dropout'`: the dropout rate. Default: `0.1`
 
 The input variables are normalized using a custom non-linear normalization layer, whose documentation can be found
 [here](https://optima-docs.docs.cern.ch/keras/tools.html#OPTIMA.keras.tools.NonLinearNormalization). This layer first
 applies the non-linear transformations returned by the `get_nonlinear_scaling`-function of the [InputHandler](#inputhandler);
 supported are $\sqrt{\bullet}$, $\log_{10}(\bullet)$ or the identity. After that, a linear transformation to achieve
 zero mean and unit variance for all input features on the training dataset is applied. A batch normalization layer is
 added between each hidden layer unless the SELU activation function is used. The number of nodes in the output layer is
@@ -576,23 +583,24 @@
 ##### compile_model
 
 A function that compiles the provided Keras model. It is called after creating a new model by executing the
 `build_model`-function (with parameter `first_compile` set to `True`) and after reloading a model from a checkpoint
 (with parameter `first_compile` set to `False`). It uses the Adam optimizer with the following tunable hyperparameters
 (see https://arxiv.org/abs/1412.6980v9 for the Adam update rule):
 
-- `'learning_rate'`: $\alpha$
-- `'Adam_beta_1'`: $\beta_1$
-- `'one_minus_Adam_beta_2''`: $1 - \beta_2$
-- `'Adam_epsilon'`: $\varepsilon$
+- `'learning_rate'`: $\alpha$. Default: `0.001`
+- `'Adam_beta_1'`: $\beta_1$. Default: `0.9`
+- `'one_minus_Adam_beta_2''`: $1 - \beta_2$. Default: `0.001`
+- `'Adam_epsilon'`: $\varepsilon$. Default: `1e-7`
 
 Supported loss functions, set using the hyperparameter `'loss_function'`, are binary crossentropy loss
 (`'BinaryCrossentropy'`), categorical crossentropy loss (`'CategoricalCrossentropy'`), and Kullback–Leibler divergence
-loss (`'KLDivergence'`). For all available loss functions, the loss values can be weighted using class weights,
-controlled via hyperparameters of type `'loss_weight_class_N'` with `N` corresponding to the `N`-th class.
+loss (`'KLDivergence'`). By default, binary crossentropy loss is used. For all available loss functions, the loss values
+can be weighted using class weights, controlled via hyperparameters of type `'loss_weight_class_N'` with `N`
+corresponding to the `N`-th class.
 
 If an already compiled model is provided, the loss function and the parameters of the Adam optimizer are updated without
 losing the training state of the model. This functionality is needed to allow mutations during the Population Based
 Training step.
 
 For more details, see the documentation [here](https://optima-docs.docs.cern.ch/keras/model.html#OPTIMA.keras.model.compile_model)
 
@@ -757,64 +765,14 @@
 - `model_info`: A dictionary containing information of the current model:
   * `'name'`: The file name of the current model. This must be appended with `'.keras'` for Keras models and `'.ckpt'`
     for lightning models.
   * `'split`: An index denoting which of the `k` crossvalidation model this is. This ranges from `0` to `k-1`.
   * `'config'`: A dictionary containing the hyperparameter values of the current model.
 - `input_handler`: A reference to the InputHandler instance.
 
-#### Hyperparameter optimization
-
-##### get_hp_defaults
-
-A function that provides a default value for each hyperparameter. It is specific to the built-in `build_model`
-and `compile_model` functions. The concrete hyperparameter defaults can be found in the
-[documentation](https://optima-docs.docs.cern.ch/builtin/search_space.html#OPTIMA.builtin.search_space.get_hp_defaults).
-
-This function is only needed if the built-in `build_model` function is used, if a `build_search_space` function is
-defined in the run-config or if *only* the fine-tuning step with Population Based Training is performed and not all
-hyperparameters in the search space support mutation.
-
-##### build_search_space
-
-A function that builds the search space that is required by `Tune` from the `seach_space` defined in the run-config and
-the hyperparameter default values. It is a wrapper around the direct conversion implemented in
-`OPTIMA.core.search_space.run_config_to_tune_converter` to handle special cases specific to the built-in `build_model`
-and `compile_model` functions. Amongst others, it makes building the search space easier when optimizing the number of
-neurons in each hidden layer independently. All hyperparameters that are not present in the `search_space` but have a
-default value provided will be fixed to their default value. More details can be found in the
-[documentation](https://optima-docs.docs.cern.ch/builtin/search_space.html#OPTIMA.builtin.search_space.build_search_space).
-
-This function is only used if the built-in `build_model` function is used or if it is re-defined in the run-config.
-
-| Parameter                           | Default value | Explanation                                                                                                                 |
-|-------------------------------------|---------------|-----------------------------------------------------------------------------------------------------------------------------|
-| `optimize_units_per_layer` *(bool)* | `False`       | Should each hidden layer have the same number of neurons (`False`) or should each layer be optimized individually (`True`)? |
-
-##### limit_and_round_hyperparameters
-
-A limit that enforces limits and rounds the values of specific hyperparameters. It is provided with hyperparameter values
-that have been selected by the search algorithm. This can be necessary since Population Based Training does not respect
-the limits of the search space which can result in invalid hyperparameter values (e.g. a dropout rate larger than 1).
-Additionally, hyperparameters can be rounded. This is useful to e.g. allow Population Based Training (which only supports
-continuous search spaces) to mutate discrete hyperparameters like the batch size.
-
-This function is specific to the build-in `build_model` and `compile_model` functions. Details on the enforced limits
-can be found in the
-[documentation](https://optima-docs.docs.cern.ch/builtin/search_space.html#OPTIMA.builtin.search_space.limit_and_round_hyperparameters).
-
-##### prepare_search_space_for_PBT
-
-A function that replaces hyperparameter search space entries that do not support PBT mutation. If a prior pre- or main
-hyperparameter optimization is performed, unsupported hyperparameters are fixed to their optimized values. If only
-the fine-tuning step is performed, unsupported hyperparameters are fixed to their default values.
-
-This function is specific to the built-in `build_model` and `compile_model` functions and therefore replaces corresponding
-unsupported hyperparameters. Details can be found in the
-[documentation](https://optima-docs.docs.cern.ch/builtin/search_space.html#OPTIMA.builtin.search_space.prepare_search_space_for_PBT).
-
 #### Input variable selection
 
 ##### create_variable_sets_to_try
 
 A function that generates the sets of input variables to evaluate for each iteration of the input variable selection.
 By default, each leave-one-out subset of the remaining set of input variables is tested. To overwrite this behavior, a
 `create_variable_sets_to_try` function that accepts the following parameters needs to be defined in the run-config:
```

### Comparing `optima_ml-0.3.2a5.dev2/optima_ml.egg-info/SOURCES.txt` & `optima_ml-0.3.3a1/optima_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.2a5.dev2/setup.py` & `optima_ml-0.3.3a1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 REQUIRES_PYTHON = '>=3.9.0'  # TODO: find minimum!
 VERSION = re.search('^__version__\s*=\s*"(.*)"', open('OPTIMA/optima.py').read(), re.M).group(1)
 
 # Which platforms are supported?
 PLATFORMS = ['linux', 'darwin']
 
 REQUIRED = [
-    'optuna==3.5.0',
-    'ray[data,train,tune]==2.9.2',
+    'optuna==3.6',
+    'ray[data,train,tune]==2.11',
     'numpy',
     'scipy',
     'pandas',
     'matplotlib',
     'seaborn',
     'tabulate',
     'scikit-learn',
```

### Comparing `optima_ml-0.3.2a5.dev2/tests/test_builtin.py` & `optima_ml-0.3.3a1/tests/test_builtin.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,124 +26,67 @@
     # get dummy input handler with linear input scaling
     input_handler = builtin_inputs.InputHandler(run_config)
     input_handler.set_vars([f"input_{i}" for i in range(13)])
     input_handler.scaling_dict = {f"input_{i}": ("linear", (1.0, 0.0)) for i in range(13)}
     dummy_inputs = np.concatenate([np.ones((1000, 13)), -1 * np.ones((1000, 13))])  # mean zero, variance one
     dummy_targets = np.ones((2000, 1))
     model = builtin_model.build_model(
-        model_config=builtin_search_space.get_hp_defaults(),
+        model_config=builtin_search_space.get_hp_defaults()[0],
         input_handler=input_handler,
         inputs_train=dummy_inputs,
         targets_train=dummy_targets,
         seed=42
     )
     return model
 
 
 def get_default_custom_objects():
     return {
-            "swish": tf.keras.activations.swish,
-            "WeightedBinaryCrossentropy": keras_tools.WeightedBinaryCrossentropy,
-            }
+        "swish": tf.keras.activations.swish,
+        "WeightedBinaryCrossentropy": keras_tools.WeightedBinaryCrossentropy,
+    }
 
 
 def get_default_training_data():
     input_handler = builtin_inputs.InputHandler(run_config)
 
     # load test dataset of 10000 events, 5000 signal and 5000 background. 13 input variables are set in test config.
     (inputs,
      targets,
      weights,
      normalized_weights,
-     event_nums) = builtin_inputs.get_inputs(run_config,
-                                                    nevts=run_config.max_num_events,
-                                                    input_vars_list=input_handler.get_vars())
+     event_nums) = builtin_inputs.get_inputs(
+        run_config,
+        nevts=run_config.max_num_events,
+        input_vars_list=input_handler.get_vars()
+    )
 
     # use custom manual plus standard scaler
     scaler_class = [builtin_inputs.CustomManualPlusStandardScaler, (input_handler,)]
 
     # randomly split into training and validation data
-    return builtin_inputs.get_training_data(inputs,
-                                                   targets,
-                                                   weights,
-                                                   normalized_weights,
-                                                   splitting_cond=0.2,
-                                                   preprocessor=scaler_class)
+    return builtin_inputs.get_training_data(
+        inputs,
+        targets,
+        weights,
+        normalized_weights,
+        splitting_cond=0.2,
+        preprocessor=scaler_class
+    )
 
 
 def test_get_hp_defaults():
     hp_defaults = builtin_search_space.get_hp_defaults()
-    assert isinstance(hp_defaults, dict)
+    assert isinstance(hp_defaults, tuple) and len(hp_defaults) == 2
+    assert isinstance(hp_defaults[0], dict) and isinstance(hp_defaults[1], dict)
 
-    for hp_value in hp_defaults.values():
+    for hp_value in hp_defaults[0].values():
+        assert isinstance(hp_value, str) or isinstance(hp_value, int) or isinstance(hp_value, float)
+    for hp_value in hp_defaults[1].values():
         assert isinstance(hp_value, str) or isinstance(hp_value, int) or isinstance(hp_value, float)
-
-
-def test_build_search_space():
-    default_hps = builtin_search_space.get_hp_defaults()
-
-    # fixed layer sizes
-    search_space = builtin_search_space.build_search_space(default_hps, run_config)
-    assert isinstance(search_space, dict)
-    for hp, hp_value in search_space.items():
-        assert (
-            isinstance(hp_value, tune.search.sample.Float)
-            or isinstance(hp_value, tune.search.sample.Integer)
-            or isinstance(hp_value, tune.search.sample.Categorical)
-            or isinstance(hp_value, list)
-            or isinstance(hp_value, dict)
-            or isinstance(hp_value, type(default_hps[hp]))
-        )
-    assert "units" in search_space.keys() and not all([f"units_{i}" in search_space.keys() for i in range(1, 5)])
-
-    # variable layer sizes with same search space; can have up to 6 layers, thus need units_1, ..., units_6
-    optimize_units_before = run_config.optimize_units_per_layer
-    run_config.optimize_units_per_layer = True
-    search_space = builtin_search_space.build_search_space(default_hps, run_config)
-    assert "units" not in search_space.keys() and all([f"units_{i}" in search_space.keys() for i in range(1, 5)])
-
-    search_space_before = run_config.search_space.copy()
-    del run_config.search_space["units"]
-    run_config.search_space.update({f"units_{i+1}": ('log', 8, int(32-2*i), 1) for i in range(0, 6)})
-    search_space = builtin_search_space.build_search_space(default_hps, run_config)
-    assert "units" not in search_space.keys() and all([f"units_{i}" in search_space.keys() for i in range(1, 5)])
-
-    run_config.optimize_units_per_layer = optimize_units_before
-    run_config.search_space = search_space_before
-
-
-def test_prepare_search_space_for_PBT():
-    default_hps = builtin_search_space.get_hp_defaults()
-
-    # PBT can only mutate l1, l2, dropout, batch_size, Adam-parameters, loss_function and signal_weight. Thus, num_layers,
-    # units, activation and initializers should be replaced with defaults
-    search_space = {
-        "num_layers": ('uniform', 3, 6, 1),
-        "units": ('log', 8, 32, 1),
-        "activation": ['swish', 'relu'],
-        "kernel_initializer": ['glorot_uniform', tf.keras.initializers.HeNormal(seed=42)],
-        "bias_initializer": ['zeros'],
-        "l1_lambda": ('log', 1e-18, 1e-1),
-        "l2_lambda": ('log', 1e-18, 1e-1),
-        "dropout": ('uniform', 0.0, 0.5),
-        "batch_size": ('uniform', 64., 256.),
-        "learning_rate": ('log', 1e-5, 1e-2),
-        "Adam_beta_1": ('uniform', 1e-4, 0.99),
-        "one_minus_Adam_beta_2": ('log', 1e-5, 0.9999),
-        "Adam_epsilon": ('log', 1e-10, 1.0),
-        "loss_function": ['BinaryCrossentropy', 'KLDivergence'],
-        "loss_signal_weight": ('uniform', 0.5, 1.5),
-    }
-    to_replace = ["num_layers", "units", "activation", "kernel_initializer", "bias_initializer", "loss_function"]
-    search_space_replaced = search_space.copy()
-    for hp in search_space_replaced.keys():
-        if hp in to_replace:
-            search_space_replaced[hp] = default_hps[hp]
-    PBT_search_space = builtin_search_space.prepare_search_space_for_PBT(search_space, default_hps)
-    assert PBT_search_space == search_space_replaced
 
 
 @pytest.mark.skipif(os.environ.get('TEST_QUICK') == '1', reason='Test takes more than 5 seconds to run.')
 def test_build_model():
     hp_allowed_values = {
         "num_layers": [3],
         "units": [8],
@@ -469,15 +412,16 @@
      targets_split,
      _,
      normalized_weights_split) = get_default_training_data()
     trained_val_loss = model.evaluate(x=inputs_split[1], y=targets_split[1])
     assert abs(trained_val_loss - 0.53826028) < 1e-7
 
     # check updatable hyperparameters
-    default_hps = builtin_search_space.get_hp_defaults()
+    default_hps_build, default_hps_compile = builtin_search_space.get_hp_defaults()
+    default_hps = default_hps_build | default_hps_compile
     for layer in model.layers:
         if isinstance(layer, tf.keras.layers.Dense) and layer.name != "output":
             assert layer.kernel_regularizer.l1 == default_hps["l1_lambda"]
             assert layer.kernel_regularizer.l2 == default_hps["l2_lambda"]
 
     # continue training for 1 epoch, loss should be low and evaluation similar
     history = model.fit(
@@ -512,15 +456,16 @@
     trained_val_loss = model.evaluate(x=inputs_split[1], y=targets_split[1])
     assert abs(trained_val_loss - 0.54785) < 1e-4
 
 
 @pytest.mark.skipif(os.environ.get('TEST_QUICK') == '1', reason='Test takes more than 5 seconds to run.')
 def test_compile_model():
     # get the default model
-    default_hps = builtin_search_space.get_hp_defaults()
+    default_hps_build, default_hps_compile = builtin_search_space.get_hp_defaults()
+    default_hps = default_hps_build | default_hps_compile
     model = get_default_model()
 
     # some example metrics
     metrics = [tf.keras.metrics.AUC(name="AUC")]
     weighted_metrics = [tf.keras.metrics.BinaryAccuracy(name="weighted_BA"),
                         tf.keras.metrics.AUC(name="weighted_AUC"),
                         tf.keras.metrics.BinaryCrossentropy(name="weighted_BCE")]
```

### Comparing `optima_ml-0.3.2a5.dev2/tests/test_integration.py` & `optima_ml-0.3.3a1/tests/test_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     # not be identical due to numerical differences on different systems arising during the crossvalidation). The path
     # to the trial of cause is expected to be different.
     assert (2 * (best_trials.drop(columns="trial") - best_trials_reference.drop(columns="trial")) / (best_trials.drop(columns="trial") + best_trials_reference.drop(columns="trial"))).abs().max().max() < 1e-2
     assert (2 * (best_trials_fit.drop(columns="trial") - best_trials_fit_reference.drop(columns="trial")) / (best_trials_fit.drop(columns="trial") + best_trials_fit_reference.drop(columns="trial"))).abs().max().max() < 1e-2
     assert configs_df.equals(configs_df_reference)
     for raw, raw_test in zip(raw_metric_values, raw_metric_values_reference):
         if raw != 0 or raw_test != 0:
-            assert abs(2 * (raw - raw_test) / (raw + raw_test)) < 2e-2
+            assert abs(2 * (raw - raw_test) / (raw + raw_test)) < 0.1
 
     # check the variable optimization
     with open("tests/test_optimization/results/variable_optimization/optimized_vars.pickle", "rb") as f:
         optimized_vars = pickle.load(f)
     with open("tests/test_optimization/results/variable_optimization/variable_optimization.pickle", "rb") as f:
         var_opt_baseline, var_opt_results = pickle.load(f)
     with open("tests/temp_integration_test/test_optimization/results/variable_optimization/optimized_vars.pickle", "rb") as f:
@@ -66,15 +66,15 @@
     with open("tests/temp_integration_test/test_optimization/results/variable_optimization/variable_optimization.pickle", "rb") as f:
         var_opt_baseline_reference, var_opt_results_reference = pickle.load(f)
 
     assert optimized_vars == optimized_vars_reference
     assert np.max(np.abs(var_opt_baseline - var_opt_baseline_reference)) < 1e-4
     for it in range(len(var_opt_results_reference)):
         for var_set in var_opt_results_reference[it].keys():
-            assert np.max(np.abs(np.array(var_opt_results[it][var_set]) - np.array(var_opt_results_reference[it][var_set]))) < 1e-4
+            assert np.max(np.abs(np.array(var_opt_results[it][var_set]) - np.array(var_opt_results_reference[it][var_set]))) < 1e-3
 
     # check the main optimization step
     with open("tests/test_optimization/results/optuna+ASHA/evaluation.pickle", "rb") as evaluation_file:
         (
             best_trials,
             best_trials_fit,
             configs_df,
@@ -98,15 +98,15 @@
             raw_metric_values_reference
         ) = pickle.load(evaluation_file)
     assert (2 * (best_trials.drop(columns="trial") - best_trials_reference.drop(columns="trial")) / (best_trials.drop(columns="trial") + best_trials_reference.drop(columns="trial"))).abs().max().max() < 1e-2
     assert (2 * (best_trials_fit.drop(columns="trial") - best_trials_fit_reference.drop(columns="trial")) / (best_trials_fit.drop(columns="trial") + best_trials_fit_reference.drop(columns="trial"))).abs().max().max() < 1e-2
     assert configs_df.equals(configs_df_reference)
     for raw, raw_test in zip(raw_metric_values, raw_metric_values_reference):
         if raw != 0 or raw_test != 0:
-            assert abs(2 * (raw - raw_test) / (raw + raw_test)) < 2e-2
+            assert abs(2 * (raw - raw_test) / (raw + raw_test)) < 0.1
 
     # check the PBT step
     with open("tests/test_optimization/results/PBT/evaluation.pickle", "rb") as evaluation_file:
         (
             best_trials,
             _,
             configs_df,
@@ -125,16 +125,17 @@
             _,
             _,
             _,
             _,
             evaluation_string_reference,
             raw_metric_values_reference
         ) = pickle.load(evaluation_file)
-    assert (2 * (best_trials.drop(columns="trial") - best_trials_reference.drop(columns="trial")) / (best_trials.drop(columns="trial") + best_trials_reference.drop(columns="trial"))).abs().max().max() < 1e-2
+    assert (2 * (best_trials.drop(columns=["trial", "best index"]) - best_trials_reference.drop(columns=["trial", "best index"]))
+            / (best_trials.drop(columns=["trial", "best index"]) + best_trials_reference.drop(columns=["trial", "best index"]))).abs().max().max() < 1e-2
     assert configs_df.equals(configs_df_reference)
     for raw, raw_test in zip(raw_metric_values, raw_metric_values_reference):
         if raw != 0 or raw_test != 0:
-            assert abs(2 * (raw - raw_test) / (raw + raw_test)) < 2e-2
+            assert abs(2 * (raw - raw_test) / (raw + raw_test)) < 0.1
 
     # cleanup
     shutil.rmtree("tests/test_optimization")
     shutil.rmtree("tests/temp_integration_test")
```

### Comparing `optima_ml-0.3.2a5.dev2/tests/test_integration_sameMachine.py` & `optima_ml-0.3.3a1/tests/test_integration_sameMachine.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.2a5.dev2/tests/test_preprocessing.py` & `optima_ml-0.3.3a1/tests/test_preprocessing.py`

 * *Files identical despite different names*

