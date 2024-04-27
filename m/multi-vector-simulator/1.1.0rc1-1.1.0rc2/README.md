# Comparing `tmp/multi-vector-simulator-1.1.0rc1.tar.gz` & `tmp/multi-vector-simulator-1.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi-vector-simulator-1.1.0rc1.tar", last modified: Sat Apr 27 21:13:29 2024, max compression
+gzip compressed data, was "multi-vector-simulator-1.1.0rc2.tar", last modified: Sat Apr 27 21:21:57 2024, max compression
```

## Comparing `multi-vector-simulator-1.1.0rc1.tar` & `multi-vector-simulator-1.1.0rc2.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.878079 multi-vector-simulator-1.1.0rc1/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    18092 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/LICENSE.md
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       45 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/MANIFEST.in
--rw-r--r--   0 pierre-francois  (1000) pierre-francois  (1000)    13731 2024-04-27 21:13:29.878079 multi-vector-simulator-1.1.0rc1/PKG-INFO
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11547 2023-02-03 15:33:58.000000 multi-vector-simulator-1.1.0rc1/README.rst
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       38 2024-04-27 21:13:29.878079 multi-vector-simulator-1.1.0rc1/setup.cfg
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9653 2023-06-14 09:01:56.000000 multi-vector-simulator-1.1.0rc1/setup.py
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.854080 multi-vector-simulator-1.1.0rc1/src/
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.862080 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    16859 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/A0_initialization.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    27452 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/A1_csv_to_json.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11661 2023-09-15 14:50:37.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/B0_data_input_json.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    72874 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/C0_data_processing.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    40172 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/C1_verification.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    18277 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/C2_economic_functions.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    14693 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/D0_modelling_and_optimization.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    54729 2024-04-27 21:06:46.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/D1_model_components.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    28866 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/D2_model_constraints.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12129 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/E0_evaluation.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    44646 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/E1_process_results.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    18293 2023-11-01 09:47:08.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/E2_economics.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    44571 2024-03-27 00:09:52.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/E3_indicator_calculation.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9281 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/E4_verification.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9543 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/F0_output.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    37196 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/F1_plotting.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    38813 2023-09-14 20:45:28.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/F2_autoreport.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11757 2023-11-01 08:24:33.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/F3_debug.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/__init__.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    10258 2023-09-12 21:19:20.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/cli.py
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.862080 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    14353 2024-04-27 21:13:29.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/MVS_parameters_list.csv
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.862080 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/assets/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)   168697 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/assets/logo-eland-original.jpg
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     6128 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/assets/styles.css
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.854080 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.866079 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      132 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/constraints.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       92 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/economic_data.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       22 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/energyBusses.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       81 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/energyConsumption.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      332 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/energyConversion.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      355 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/energyProduction.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      312 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/energyProviders.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      150 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/energyStorage.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      121 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/fixcost.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      156 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/project_data.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      105 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/simulation_settings.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      404 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/storage_01.csv
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.866079 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/time_series/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       16 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/time_series/blank
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.866079 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.866079 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      156 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/constraints.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      105 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/economic_data.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      154 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyBusses.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      179 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConsumption.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1068 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConversion.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      562 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProduction.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      410 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProviders.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      221 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyStorage.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      200 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/fixcost.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      249 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/project_data.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      130 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/simulation_settings.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      491 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/storage_01.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    23516 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/mvs_config.json
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.866079 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/time_series/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    78842 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/time_series/demand.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    34217 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/time_series/pv_gen_merra2_2014_eff1_tilt40_az180.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    13451 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/server.py
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.870079 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    25650 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/__init__.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     3404 2022-03-30 10:59:56.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/analysis.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12078 2023-02-03 12:59:38.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/constants.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     8633 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/constants_json_strings.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1495 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/constants_output.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    28826 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/data_parser.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1725 2023-02-03 13:29:18.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/exceptions.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     5563 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/helpers.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      144 2024-04-27 21:13:20.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/version.py
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.874079 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator.egg-info/
--rw-r--r--   0 pierre-francois  (1000) pierre-francois  (1000)    13731 2024-04-27 21:13:29.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator.egg-info/PKG-INFO
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     5026 2024-04-27 21:13:29.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator.egg-info/SOURCES.txt
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)        1 2024-04-27 21:13:29.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator.egg-info/dependency_links.txt
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      192 2024-04-27 21:13:29.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator.egg-info/entry_points.txt
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      403 2024-04-27 21:13:29.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator.egg-info/requires.txt
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       23 2024-04-27 21:13:29.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator.egg-info/top_level.txt
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.874079 multi-vector-simulator-1.1.0rc1/tests/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12150 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/tests/test_A0_initialization.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12999 2022-10-16 15:02:06.000000 multi-vector-simulator-1.1.0rc1/tests/test_A1_csv_to_json.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     6610 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc1/tests/test_B0_data_input_json.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    51979 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc1/tests/test_C0_data_processing.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    32932 2023-02-03 12:59:38.000000 multi-vector-simulator-1.1.0rc1/tests/test_C1_verification.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    10403 2024-04-27 21:08:22.000000 multi-vector-simulator-1.1.0rc1/tests/test_C2_economic_functions.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     8840 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/tests/test_D0_modelling_and_optimization.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    47067 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/tests/test_D1_model_components.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    19212 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/tests/test_D2_model_constraints.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     7318 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc1/tests/test_E0_evaluation.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    21776 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/tests/test_E1_process_results.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11264 2022-09-23 09:34:10.000000 multi-vector-simulator-1.1.0rc1/tests/test_E2_economics.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    31598 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc1/tests/test_E3_indicator_calculation.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12189 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc1/tests/test_E4_verification.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    14321 2022-11-02 09:00:04.000000 multi-vector-simulator-1.1.0rc1/tests/test_F0_output.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     6212 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc1/tests/test_F1_plotting.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    17082 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/tests/test_benchmark_KPI.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    25033 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc1/tests/test_benchmark_constraints.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    15959 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc1/tests/test_benchmark_feedin.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    22774 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/tests/test_benchmark_scenarios.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9113 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/tests/test_benchmark_special_features.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    38791 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/tests/test_benchmark_stratified_thermal_storage.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     3658 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/tests/test_input_folder_parameters.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      641 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/tests/test_sensitivity.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     5255 2022-09-23 09:43:57.000000 multi-vector-simulator-1.1.0rc1/tests/test_utils.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.241921 multi-vector-simulator-1.1.0rc2/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    18092 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/LICENSE.md
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       45 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/MANIFEST.in
+-rw-r--r--   0 pierre-francois  (1000) pierre-francois  (1000)    13769 2024-04-27 21:21:57.241921 multi-vector-simulator-1.1.0rc2/PKG-INFO
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11547 2023-02-03 15:33:58.000000 multi-vector-simulator-1.1.0rc2/README.rst
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       38 2024-04-27 21:21:57.241921 multi-vector-simulator-1.1.0rc2/setup.cfg
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9653 2023-06-14 09:01:56.000000 multi-vector-simulator-1.1.0rc2/setup.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.221921 multi-vector-simulator-1.1.0rc2/src/
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.229921 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    16859 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/A0_initialization.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    27452 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/A1_csv_to_json.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11661 2023-09-15 14:50:37.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/B0_data_input_json.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    72874 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/C0_data_processing.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    40172 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/C1_verification.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    18277 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/C2_economic_functions.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    14693 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/D0_modelling_and_optimization.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    54729 2024-04-27 21:06:46.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/D1_model_components.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    28866 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/D2_model_constraints.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12129 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/E0_evaluation.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    44646 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/E1_process_results.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    18293 2023-11-01 09:47:08.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/E2_economics.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    44571 2024-03-27 00:09:52.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/E3_indicator_calculation.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9281 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/E4_verification.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9543 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/F0_output.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    37196 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/F1_plotting.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    38813 2023-09-14 20:45:28.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/F2_autoreport.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11757 2023-11-01 08:24:33.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/F3_debug.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/__init__.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    10258 2023-09-12 21:19:20.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/cli.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.229921 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    14353 2024-04-27 21:21:56.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/MVS_parameters_list.csv
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.229921 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/assets/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)   168697 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/assets/logo-eland-original.jpg
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     6128 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/assets/styles.css
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.221921 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.233921 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      132 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/constraints.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       92 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/economic_data.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       22 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/energyBusses.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       81 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/energyConsumption.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      332 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/energyConversion.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      355 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/energyProduction.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      312 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/energyProviders.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      150 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/energyStorage.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      121 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/fixcost.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      156 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/project_data.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      105 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/simulation_settings.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      404 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/storage_01.csv
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.233921 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/time_series/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       16 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/time_series/blank
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.233921 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.233921 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      156 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/constraints.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      105 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/economic_data.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      154 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/energyBusses.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      179 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConsumption.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1068 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConversion.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      562 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProduction.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      410 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProviders.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      221 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/energyStorage.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      200 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/fixcost.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      249 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/project_data.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      130 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/simulation_settings.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      491 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/storage_01.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    23516 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/mvs_config.json
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.233921 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/time_series/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    78842 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/time_series/demand.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    34217 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/time_series/pv_gen_merra2_2014_eff1_tilt40_az180.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    13451 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/server.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.233921 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    25650 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/__init__.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     3404 2022-03-30 10:59:56.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/analysis.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12078 2023-02-03 12:59:38.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/constants.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     8633 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/constants_json_strings.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1495 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/constants_output.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    28826 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/data_parser.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1725 2023-02-03 13:29:18.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/exceptions.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     5563 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/helpers.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      144 2024-04-27 21:21:50.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/version.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.237921 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator.egg-info/
+-rw-r--r--   0 pierre-francois  (1000) pierre-francois  (1000)    13769 2024-04-27 21:21:57.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator.egg-info/PKG-INFO
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     5026 2024-04-27 21:21:57.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator.egg-info/SOURCES.txt
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)        1 2024-04-27 21:21:57.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator.egg-info/dependency_links.txt
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      192 2024-04-27 21:21:57.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator.egg-info/entry_points.txt
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      426 2024-04-27 21:21:57.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator.egg-info/requires.txt
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       23 2024-04-27 21:21:57.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator.egg-info/top_level.txt
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.237921 multi-vector-simulator-1.1.0rc2/tests/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12150 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/tests/test_A0_initialization.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12999 2022-10-16 15:02:06.000000 multi-vector-simulator-1.1.0rc2/tests/test_A1_csv_to_json.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     6610 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc2/tests/test_B0_data_input_json.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    51979 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc2/tests/test_C0_data_processing.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    32932 2023-02-03 12:59:38.000000 multi-vector-simulator-1.1.0rc2/tests/test_C1_verification.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    10403 2024-04-27 21:08:22.000000 multi-vector-simulator-1.1.0rc2/tests/test_C2_economic_functions.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     8840 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/tests/test_D0_modelling_and_optimization.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    47067 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/tests/test_D1_model_components.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    19212 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/tests/test_D2_model_constraints.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     7318 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc2/tests/test_E0_evaluation.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    21776 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/tests/test_E1_process_results.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11264 2022-09-23 09:34:10.000000 multi-vector-simulator-1.1.0rc2/tests/test_E2_economics.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    31598 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc2/tests/test_E3_indicator_calculation.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12189 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc2/tests/test_E4_verification.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    14321 2022-11-02 09:00:04.000000 multi-vector-simulator-1.1.0rc2/tests/test_F0_output.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     6212 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc2/tests/test_F1_plotting.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    17082 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/tests/test_benchmark_KPI.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    25033 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc2/tests/test_benchmark_constraints.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    15959 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc2/tests/test_benchmark_feedin.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    22774 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/tests/test_benchmark_scenarios.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9113 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/tests/test_benchmark_special_features.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    38791 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/tests/test_benchmark_stratified_thermal_storage.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     3658 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/tests/test_input_folder_parameters.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      641 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/tests/test_sensitivity.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     5255 2022-09-23 09:43:57.000000 multi-vector-simulator-1.1.0rc2/tests/test_utils.py
```

### Comparing `multi-vector-simulator-1.1.0rc1/LICENSE.md` & `multi-vector-simulator-1.1.0rc2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/PKG-INFO` & `multi-vector-simulator-1.1.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi-vector-simulator
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: Multi-vector Simulation Tool assessing and optimizing Local Energy Systems (LES) for the E-LAND project
 Home-page: https://github.com/rl-institut/multi-vector-simulator
 Author: Reiner Lemoine Institut
 Author-email: pypi@rl-institut.de
 Project-URL: Bug Reports, https://github.com/rl-institut/multi-vector-simulator/issues
 Project-URL: Source, https://github.com/rl-institut/multi-vector-simulator
 Keywords: multi-vector local-energy-systems
@@ -23,14 +23,15 @@
 Requires-Dist: graphviz>=0.14.1
 Requires-Dist: plotly
 Requires-Dist: psutil
 Requires-Dist: kaleido>=0.0.2
 Requires-Dist: openpyxl>=3.0.5
 Requires-Dist: xlrd==1.2.0
 Requires-Dist: oemof.solph==0.5.1
+Requires-Dist: oemof.network==0.5.0a5
 Provides-Extra: docs
 Requires-Dist: sphinx>=2.3.1; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=0.4.3; extra == "docs"
 Requires-Dist: numpydoc>=1.1.0; extra == "docs"
 Requires-Dist: sphinxcontrib-svg2pdfconverter; extra == "docs"
 Provides-Extra: report
 Requires-Dist: dash>=2.3.1; extra == "report"
```

### Comparing `multi-vector-simulator-1.1.0rc1/README.rst` & `multi-vector-simulator-1.1.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/setup.py` & `multi-vector-simulator-1.1.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/A0_initialization.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/A0_initialization.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/A1_csv_to_json.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/A1_csv_to_json.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/B0_data_input_json.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/B0_data_input_json.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/C0_data_processing.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/C0_data_processing.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/C1_verification.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/C1_verification.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/C2_economic_functions.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/C2_economic_functions.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/D0_modelling_and_optimization.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/D0_modelling_and_optimization.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/D1_model_components.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/D1_model_components.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/D2_model_constraints.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/D2_model_constraints.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/E0_evaluation.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/E0_evaluation.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/E1_process_results.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/E1_process_results.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/E2_economics.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/E2_economics.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/E3_indicator_calculation.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/E3_indicator_calculation.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/E4_verification.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/E4_verification.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/F0_output.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/F0_output.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/F1_plotting.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/F1_plotting.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/F2_autoreport.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/F2_autoreport.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/F3_debug.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/F3_debug.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/cli.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/cli.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/MVS_parameters_list.csv` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/MVS_parameters_list.csv`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/assets/logo-eland-original.jpg` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/assets/logo-eland-original.jpg`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/assets/styles.css` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/assets/styles.css`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConversion.csv` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConversion.csv`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProduction.csv` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProduction.csv`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/mvs_config.json` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/mvs_config.json`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/time_series/demand.csv` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/time_series/demand.csv`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/time_series/pv_gen_merra2_2014_eff1_tilt40_az180.csv` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/time_series/pv_gen_merra2_2014_eff1_tilt40_az180.csv`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/server.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/server.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/__init__.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/analysis.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/constants.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/constants.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/constants_json_strings.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/constants_json_strings.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/constants_output.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/constants_output.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/data_parser.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/data_parser.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/exceptions.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/helpers.py` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator.egg-info/PKG-INFO` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi-vector-simulator
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: Multi-vector Simulation Tool assessing and optimizing Local Energy Systems (LES) for the E-LAND project
 Home-page: https://github.com/rl-institut/multi-vector-simulator
 Author: Reiner Lemoine Institut
 Author-email: pypi@rl-institut.de
 Project-URL: Bug Reports, https://github.com/rl-institut/multi-vector-simulator/issues
 Project-URL: Source, https://github.com/rl-institut/multi-vector-simulator
 Keywords: multi-vector local-energy-systems
@@ -23,14 +23,15 @@
 Requires-Dist: graphviz>=0.14.1
 Requires-Dist: plotly
 Requires-Dist: psutil
 Requires-Dist: kaleido>=0.0.2
 Requires-Dist: openpyxl>=3.0.5
 Requires-Dist: xlrd==1.2.0
 Requires-Dist: oemof.solph==0.5.1
+Requires-Dist: oemof.network==0.5.0a5
 Provides-Extra: docs
 Requires-Dist: sphinx>=2.3.1; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=0.4.3; extra == "docs"
 Requires-Dist: numpydoc>=1.1.0; extra == "docs"
 Requires-Dist: sphinxcontrib-svg2pdfconverter; extra == "docs"
 Provides-Extra: report
 Requires-Dist: dash>=2.3.1; extra == "report"
```

### Comparing `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator.egg-info/SOURCES.txt` & `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_A0_initialization.py` & `multi-vector-simulator-1.1.0rc2/tests/test_A0_initialization.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_A1_csv_to_json.py` & `multi-vector-simulator-1.1.0rc2/tests/test_A1_csv_to_json.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_B0_data_input_json.py` & `multi-vector-simulator-1.1.0rc2/tests/test_B0_data_input_json.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_C0_data_processing.py` & `multi-vector-simulator-1.1.0rc2/tests/test_C0_data_processing.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_C1_verification.py` & `multi-vector-simulator-1.1.0rc2/tests/test_C1_verification.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_C2_economic_functions.py` & `multi-vector-simulator-1.1.0rc2/tests/test_C2_economic_functions.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_D0_modelling_and_optimization.py` & `multi-vector-simulator-1.1.0rc2/tests/test_D0_modelling_and_optimization.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_D1_model_components.py` & `multi-vector-simulator-1.1.0rc2/tests/test_D1_model_components.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_D2_model_constraints.py` & `multi-vector-simulator-1.1.0rc2/tests/test_D2_model_constraints.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_E0_evaluation.py` & `multi-vector-simulator-1.1.0rc2/tests/test_E0_evaluation.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_E1_process_results.py` & `multi-vector-simulator-1.1.0rc2/tests/test_E1_process_results.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_E2_economics.py` & `multi-vector-simulator-1.1.0rc2/tests/test_E2_economics.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_E3_indicator_calculation.py` & `multi-vector-simulator-1.1.0rc2/tests/test_E3_indicator_calculation.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_E4_verification.py` & `multi-vector-simulator-1.1.0rc2/tests/test_E4_verification.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_F0_output.py` & `multi-vector-simulator-1.1.0rc2/tests/test_F0_output.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_F1_plotting.py` & `multi-vector-simulator-1.1.0rc2/tests/test_F1_plotting.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_benchmark_KPI.py` & `multi-vector-simulator-1.1.0rc2/tests/test_benchmark_KPI.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_benchmark_constraints.py` & `multi-vector-simulator-1.1.0rc2/tests/test_benchmark_constraints.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_benchmark_feedin.py` & `multi-vector-simulator-1.1.0rc2/tests/test_benchmark_feedin.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_benchmark_scenarios.py` & `multi-vector-simulator-1.1.0rc2/tests/test_benchmark_scenarios.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_benchmark_special_features.py` & `multi-vector-simulator-1.1.0rc2/tests/test_benchmark_special_features.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_benchmark_stratified_thermal_storage.py` & `multi-vector-simulator-1.1.0rc2/tests/test_benchmark_stratified_thermal_storage.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_input_folder_parameters.py` & `multi-vector-simulator-1.1.0rc2/tests/test_input_folder_parameters.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_sensitivity.py` & `multi-vector-simulator-1.1.0rc2/tests/test_sensitivity.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc1/tests/test_utils.py` & `multi-vector-simulator-1.1.0rc2/tests/test_utils.py`

 * *Files identical despite different names*

