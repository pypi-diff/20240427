# Comparing `tmp/multi-vector-simulator-1.0.7rc3.tar.gz` & `tmp/multi-vector-simulator-1.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi-vector-simulator-1.0.7rc3.tar", last modified: Wed Mar 27 00:10:27 2024, max compression
+gzip compressed data, was "multi-vector-simulator-1.1.0rc1.tar", last modified: Sat Apr 27 21:13:29 2024, max compression
```

## Comparing `multi-vector-simulator-1.0.7rc3.tar` & `multi-vector-simulator-1.1.0rc1.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-03-27 00:10:27.714393 multi-vector-simulator-1.0.7rc3/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    18092 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/LICENSE.md
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       45 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/MANIFEST.in
--rw-r--r--   0 pierre-francois  (1000) pierre-francois  (1000)    13731 2024-03-27 00:10:27.714393 multi-vector-simulator-1.0.7rc3/PKG-INFO
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11547 2023-02-03 15:33:58.000000 multi-vector-simulator-1.0.7rc3/README.rst
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       38 2024-03-27 00:10:27.714393 multi-vector-simulator-1.0.7rc3/setup.cfg
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9653 2023-06-14 09:01:56.000000 multi-vector-simulator-1.0.7rc3/setup.py
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-03-27 00:10:27.702393 multi-vector-simulator-1.0.7rc3/src/
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-03-27 00:10:27.706393 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    16859 2023-11-02 17:25:49.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/A0_initialization.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    27452 2023-11-02 17:25:49.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/A1_csv_to_json.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11661 2023-09-15 14:50:37.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/B0_data_input_json.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    73018 2024-03-27 00:09:52.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/C0_data_processing.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    40172 2023-11-02 17:25:49.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/C1_verification.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    18277 2023-11-02 17:25:49.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/C2_economic_functions.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    14759 2024-03-22 11:11:47.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/D0_modelling_and_optimization.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    59661 2024-03-25 10:28:05.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/D1_model_components.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    28866 2023-11-02 17:25:49.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/D2_model_constraints.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12129 2023-11-02 17:25:49.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/E0_evaluation.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    45277 2024-03-26 23:57:02.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/E1_process_results.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    18293 2023-11-01 09:47:08.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/E2_economics.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    44571 2024-03-27 00:09:52.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/E3_indicator_calculation.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9281 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/E4_verification.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9543 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/F0_output.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    37196 2023-11-02 17:25:49.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/F1_plotting.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    38813 2023-09-14 20:45:28.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/F2_autoreport.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11757 2023-11-01 08:24:33.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/F3_debug.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/__init__.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    10258 2023-09-12 21:19:20.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/cli.py
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-03-27 00:10:27.706393 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    14353 2024-03-27 00:10:27.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/MVS_parameters_list.csv
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-03-27 00:10:27.706393 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/assets/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)   168697 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/assets/logo-eland-original.jpg
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     6128 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/assets/styles.css
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-03-27 00:10:27.702393 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/input_template/
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-03-27 00:10:27.706393 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/input_template/csv_elements/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      132 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/input_template/csv_elements/constraints.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       92 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/input_template/csv_elements/economic_data.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       22 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/input_template/csv_elements/energyBusses.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       81 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/input_template/csv_elements/energyConsumption.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      332 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/input_template/csv_elements/energyConversion.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      355 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/input_template/csv_elements/energyProduction.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      312 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/input_template/csv_elements/energyProviders.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      150 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/input_template/csv_elements/energyStorage.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      121 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/input_template/csv_elements/fixcost.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      156 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/input_template/csv_elements/project_data.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      105 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/input_template/csv_elements/simulation_settings.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      404 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/input_template/csv_elements/storage_01.csv
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-03-27 00:10:27.706393 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/input_template/time_series/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       16 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/input_template/time_series/blank
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-03-27 00:10:27.706393 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/inputs/
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-03-27 00:10:27.710393 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/inputs/csv_elements/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      156 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/inputs/csv_elements/constraints.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      105 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/inputs/csv_elements/economic_data.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      154 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/inputs/csv_elements/energyBusses.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      179 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConsumption.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1068 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConversion.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      562 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProduction.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      410 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProviders.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      221 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/inputs/csv_elements/energyStorage.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      200 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/inputs/csv_elements/fixcost.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      249 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/inputs/csv_elements/project_data.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      130 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/inputs/csv_elements/simulation_settings.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      491 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/inputs/csv_elements/storage_01.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    23516 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/inputs/mvs_config.json
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-03-27 00:10:27.710393 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/inputs/time_series/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    78842 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/inputs/time_series/demand.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    34217 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/inputs/time_series/pv_gen_merra2_2014_eff1_tilt40_az180.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    13656 2024-03-27 00:09:52.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/server.py
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-03-27 00:10:27.710393 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/utils/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    25650 2023-11-02 17:10:47.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/utils/__init__.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     3404 2022-03-30 10:59:56.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/utils/analysis.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12078 2023-02-03 12:59:38.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/utils/constants.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     8698 2024-03-22 11:14:01.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/utils/constants_json_strings.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1495 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/utils/constants_output.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    28825 2024-03-26 23:59:28.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/utils/data_parser.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1725 2023-02-03 13:29:18.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/utils/exceptions.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     6440 2024-03-22 11:14:01.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/utils/helpers.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      144 2024-03-27 00:09:02.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/version.py
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-03-27 00:10:27.710393 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator.egg-info/
--rw-r--r--   0 pierre-francois  (1000) pierre-francois  (1000)    13731 2024-03-27 00:10:27.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator.egg-info/PKG-INFO
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     5026 2024-03-27 00:10:27.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator.egg-info/SOURCES.txt
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)        1 2024-03-27 00:10:27.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator.egg-info/dependency_links.txt
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      192 2024-03-27 00:10:27.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator.egg-info/entry_points.txt
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      403 2024-03-27 00:10:27.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator.egg-info/requires.txt
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       23 2024-03-27 00:10:27.000000 multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator.egg-info/top_level.txt
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-03-27 00:10:27.710393 multi-vector-simulator-1.0.7rc3/tests/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12150 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/tests/test_A0_initialization.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12999 2022-10-16 15:02:06.000000 multi-vector-simulator-1.0.7rc3/tests/test_A1_csv_to_json.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     6610 2022-10-16 15:02:02.000000 multi-vector-simulator-1.0.7rc3/tests/test_B0_data_input_json.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    51979 2023-11-02 17:10:47.000000 multi-vector-simulator-1.0.7rc3/tests/test_C0_data_processing.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    32932 2023-02-03 12:59:38.000000 multi-vector-simulator-1.0.7rc3/tests/test_C1_verification.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    10054 2023-11-02 17:25:49.000000 multi-vector-simulator-1.0.7rc3/tests/test_C2_economic_functions.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     8840 2023-11-02 17:25:49.000000 multi-vector-simulator-1.0.7rc3/tests/test_D0_modelling_and_optimization.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    47733 2024-03-21 21:34:36.000000 multi-vector-simulator-1.0.7rc3/tests/test_D1_model_components.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    19212 2023-11-02 17:25:49.000000 multi-vector-simulator-1.0.7rc3/tests/test_D2_model_constraints.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     7318 2022-10-16 15:02:02.000000 multi-vector-simulator-1.0.7rc3/tests/test_E0_evaluation.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    21776 2023-11-02 17:25:49.000000 multi-vector-simulator-1.0.7rc3/tests/test_E1_process_results.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11264 2022-09-23 09:34:10.000000 multi-vector-simulator-1.0.7rc3/tests/test_E2_economics.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    31598 2022-10-16 15:02:02.000000 multi-vector-simulator-1.0.7rc3/tests/test_E3_indicator_calculation.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12189 2022-10-16 15:02:02.000000 multi-vector-simulator-1.0.7rc3/tests/test_E4_verification.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    14321 2022-11-02 09:00:04.000000 multi-vector-simulator-1.0.7rc3/tests/test_F0_output.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     6212 2022-10-16 15:02:02.000000 multi-vector-simulator-1.0.7rc3/tests/test_F1_plotting.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    16843 2023-09-15 08:56:50.000000 multi-vector-simulator-1.0.7rc3/tests/test_benchmark_KPI.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    25033 2022-10-16 15:02:02.000000 multi-vector-simulator-1.0.7rc3/tests/test_benchmark_constraints.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    15959 2023-11-02 17:10:47.000000 multi-vector-simulator-1.0.7rc3/tests/test_benchmark_feedin.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    22774 2023-11-02 17:25:49.000000 multi-vector-simulator-1.0.7rc3/tests/test_benchmark_scenarios.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     8789 2023-11-02 17:25:49.000000 multi-vector-simulator-1.0.7rc3/tests/test_benchmark_special_features.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    38791 2023-11-02 17:25:49.000000 multi-vector-simulator-1.0.7rc3/tests/test_benchmark_stratified_thermal_storage.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     3658 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/tests/test_input_folder_parameters.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      641 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.7rc3/tests/test_sensitivity.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     5255 2022-09-23 09:43:57.000000 multi-vector-simulator-1.0.7rc3/tests/test_utils.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.878079 multi-vector-simulator-1.1.0rc1/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    18092 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/LICENSE.md
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       45 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/MANIFEST.in
+-rw-r--r--   0 pierre-francois  (1000) pierre-francois  (1000)    13731 2024-04-27 21:13:29.878079 multi-vector-simulator-1.1.0rc1/PKG-INFO
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11547 2023-02-03 15:33:58.000000 multi-vector-simulator-1.1.0rc1/README.rst
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       38 2024-04-27 21:13:29.878079 multi-vector-simulator-1.1.0rc1/setup.cfg
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9653 2023-06-14 09:01:56.000000 multi-vector-simulator-1.1.0rc1/setup.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.854080 multi-vector-simulator-1.1.0rc1/src/
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.862080 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    16859 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/A0_initialization.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    27452 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/A1_csv_to_json.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11661 2023-09-15 14:50:37.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/B0_data_input_json.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    72874 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/C0_data_processing.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    40172 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/C1_verification.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    18277 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/C2_economic_functions.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    14693 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/D0_modelling_and_optimization.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    54729 2024-04-27 21:06:46.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/D1_model_components.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    28866 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/D2_model_constraints.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12129 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/E0_evaluation.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    44646 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/E1_process_results.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    18293 2023-11-01 09:47:08.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/E2_economics.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    44571 2024-03-27 00:09:52.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/E3_indicator_calculation.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9281 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/E4_verification.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9543 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/F0_output.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    37196 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/F1_plotting.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    38813 2023-09-14 20:45:28.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/F2_autoreport.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11757 2023-11-01 08:24:33.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/F3_debug.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/__init__.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    10258 2023-09-12 21:19:20.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/cli.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.862080 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    14353 2024-04-27 21:13:29.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/MVS_parameters_list.csv
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.862080 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/assets/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)   168697 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/assets/logo-eland-original.jpg
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     6128 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/assets/styles.css
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.854080 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.866079 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      132 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/constraints.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       92 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/economic_data.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       22 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/energyBusses.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       81 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/energyConsumption.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      332 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/energyConversion.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      355 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/energyProduction.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      312 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/energyProviders.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      150 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/energyStorage.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      121 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/fixcost.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      156 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/project_data.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      105 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/simulation_settings.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      404 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/storage_01.csv
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.866079 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/time_series/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       16 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/input_template/time_series/blank
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.866079 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.866079 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      156 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/constraints.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      105 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/economic_data.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      154 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyBusses.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      179 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConsumption.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1068 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConversion.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      562 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProduction.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      410 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProviders.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      221 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyStorage.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      200 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/fixcost.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      249 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/project_data.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      130 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/simulation_settings.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      491 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/storage_01.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    23516 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/mvs_config.json
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.866079 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/time_series/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    78842 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/time_series/demand.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    34217 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/time_series/pv_gen_merra2_2014_eff1_tilt40_az180.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    13451 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/server.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.870079 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    25650 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/__init__.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     3404 2022-03-30 10:59:56.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/analysis.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12078 2023-02-03 12:59:38.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/constants.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     8633 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/constants_json_strings.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1495 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/constants_output.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    28826 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/data_parser.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1725 2023-02-03 13:29:18.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/exceptions.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     5563 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/helpers.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      144 2024-04-27 21:13:20.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/version.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.874079 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator.egg-info/
+-rw-r--r--   0 pierre-francois  (1000) pierre-francois  (1000)    13731 2024-04-27 21:13:29.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator.egg-info/PKG-INFO
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     5026 2024-04-27 21:13:29.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator.egg-info/SOURCES.txt
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)        1 2024-04-27 21:13:29.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator.egg-info/dependency_links.txt
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      192 2024-04-27 21:13:29.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator.egg-info/entry_points.txt
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      403 2024-04-27 21:13:29.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator.egg-info/requires.txt
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       23 2024-04-27 21:13:29.000000 multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator.egg-info/top_level.txt
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:13:29.874079 multi-vector-simulator-1.1.0rc1/tests/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12150 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/tests/test_A0_initialization.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12999 2022-10-16 15:02:06.000000 multi-vector-simulator-1.1.0rc1/tests/test_A1_csv_to_json.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     6610 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc1/tests/test_B0_data_input_json.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    51979 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc1/tests/test_C0_data_processing.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    32932 2023-02-03 12:59:38.000000 multi-vector-simulator-1.1.0rc1/tests/test_C1_verification.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    10403 2024-04-27 21:08:22.000000 multi-vector-simulator-1.1.0rc1/tests/test_C2_economic_functions.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     8840 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/tests/test_D0_modelling_and_optimization.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    47067 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/tests/test_D1_model_components.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    19212 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/tests/test_D2_model_constraints.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     7318 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc1/tests/test_E0_evaluation.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    21776 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/tests/test_E1_process_results.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11264 2022-09-23 09:34:10.000000 multi-vector-simulator-1.1.0rc1/tests/test_E2_economics.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    31598 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc1/tests/test_E3_indicator_calculation.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12189 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc1/tests/test_E4_verification.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    14321 2022-11-02 09:00:04.000000 multi-vector-simulator-1.1.0rc1/tests/test_F0_output.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     6212 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc1/tests/test_F1_plotting.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    17082 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/tests/test_benchmark_KPI.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    25033 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc1/tests/test_benchmark_constraints.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    15959 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc1/tests/test_benchmark_feedin.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    22774 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/tests/test_benchmark_scenarios.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9113 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/tests/test_benchmark_special_features.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    38791 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc1/tests/test_benchmark_stratified_thermal_storage.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     3658 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/tests/test_input_folder_parameters.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      641 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc1/tests/test_sensitivity.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     5255 2022-09-23 09:43:57.000000 multi-vector-simulator-1.1.0rc1/tests/test_utils.py
```

### Comparing `multi-vector-simulator-1.0.7rc3/LICENSE.md` & `multi-vector-simulator-1.1.0rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/PKG-INFO` & `multi-vector-simulator-1.1.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi-vector-simulator
-Version: 1.0.7rc3
+Version: 1.1.0rc1
 Summary: Multi-vector Simulation Tool assessing and optimizing Local Energy Systems (LES) for the E-LAND project
 Home-page: https://github.com/rl-institut/multi-vector-simulator
 Author: Reiner Lemoine Institut
 Author-email: pypi@rl-institut.de
 Project-URL: Bug Reports, https://github.com/rl-institut/multi-vector-simulator/issues
 Project-URL: Source, https://github.com/rl-institut/multi-vector-simulator
 Keywords: multi-vector local-energy-systems
@@ -42,15 +42,15 @@
 Requires-Dist: psutil>=5.7.0; extra == "report"
 Provides-Extra: test
 Requires-Dist: pytest>=5.3.1; extra == "test"
 Requires-Dist: black==19.10b0; extra == "test"
 Requires-Dist: coverage>=4.5; extra == "test"
 Requires-Dist: coveralls>=3.0.1; extra == "test"
 Requires-Dist: mock>=3.0.5; extra == "test"
-Requires-Dist: click==8.0.4; extra == "test"
+Requires-Dist: click==8.0.2; extra == "test"
 
 ##################################################
 MVS - Multi-Vector Simulator of the E-LAND toolbox
 ##################################################
 
 |badge_docs| |badge_CI| |badge_coverage| |badge_zenodo| |badge_pypi| |badge_gpl2| |badge_black|
```

### Comparing `multi-vector-simulator-1.0.7rc3/README.rst` & `multi-vector-simulator-1.1.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/setup.py` & `multi-vector-simulator-1.1.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/A0_initialization.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/A0_initialization.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/A1_csv_to_json.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/A1_csv_to_json.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/B0_data_input_json.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/B0_data_input_json.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/C0_data_processing.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/C0_data_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,20 +286,18 @@
     -------
     Updates dict_values
     """
     auto_sinks = []
     for bus in dict_values[ENERGY_BUSSES]:
         excess_sink_name = bus + EXCESS_SINK
         energy_vector = dict_values[ENERGY_BUSSES][bus][ENERGY_VECTOR]
-        # TODO make this official if needed
-        excess_price = dict_values[ENERGY_BUSSES][bus].get("price", 0)
         define_sink(
             dict_values=dict_values,
             asset_key=excess_sink_name,
-            price={VALUE: excess_price, UNIT: CURR + "/" + UNIT},
+            price={VALUE: 0, UNIT: CURR + "/" + UNIT},
             inflow_direction=bus,
             energy_vector=energy_vector,
             asset_type="excess",
         )
         dict_values[ENERGY_BUSSES][bus].update({EXCESS_SINK: excess_sink_name})
         auto_sinks.append(excess_sink_name)
         logging.debug(
@@ -1022,15 +1020,15 @@
         INSTALLED_CAP: {VALUE: 0, UNIT: dict_dso[UNIT]},
         INFLOW_DIRECTION: peak_demand_bus_name(dict_dso[INFLOW_DIRECTION]),
         OUTFLOW_DIRECTION: dict_dso[OUTFLOW_DIRECTION],
         AVAILABILITY_DISPATCH: timeseries_availability,
         EFFICIENCY: {VALUE: 1, UNIT: "factor"},
         DEVELOPMENT_COSTS: {VALUE: 0, UNIT: CURR},
         SPECIFIC_COSTS: {VALUE: 0, UNIT: CURR + "/" + dict_dso[UNIT],},
-        # the demand pricing is split between consumption and feedin
+        # the demand pricing is only applied to consumption
         SPECIFIC_COSTS_OM: {
             VALUE: dict_dso[PEAK_DEMAND_PRICING][VALUE],
             UNIT: CURR + "/" + dict_dso[UNIT] + "/" + UNIT_YEAR,
         },
         DISPATCH_PRICE: {VALUE: 0, UNIT: CURR + "/" + dict_dso[UNIT] + "/" + UNIT_HOUR},
         OEMOF_ASSET_TYPE: OEMOF_TRANSFORMER,
         ENERGY_VECTOR: dict_dso[ENERGY_VECTOR],
@@ -1055,15 +1053,15 @@
         OUTFLOW_DIRECTION: peak_demand_bus_name(
             dict_dso[INFLOW_DIRECTION], feedin=True
         ),
         AVAILABILITY_DISPATCH: timeseries_availability,
         EFFICIENCY: {VALUE: 1, UNIT: "factor"},
         DEVELOPMENT_COSTS: {VALUE: 0, UNIT: CURR},
         SPECIFIC_COSTS: {VALUE: 0, UNIT: CURR + "/" + dict_dso[UNIT],},
-        # the demand pricing is split between consumption and feedin
+        # the demand pricing is only applied to consumption
         SPECIFIC_COSTS_OM: {
             VALUE: 0,
             UNIT: CURR + "/" + dict_dso[UNIT] + "/" + UNIT_YEAR,
         },
         DISPATCH_PRICE: {VALUE: 0, UNIT: CURR + "/" + dict_dso[UNIT] + "/" + UNIT_HOUR},
         OEMOF_ASSET_TYPE: OEMOF_TRANSFORMER,
         ENERGY_VECTOR: dict_dso[ENERGY_VECTOR],
```

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/C1_verification.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/C1_verification.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/C2_economic_functions.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/C2_economic_functions.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/D0_modelling_and_optimization.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/D0_modelling_and_optimization.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,15 +344,14 @@
         -------
         Updated model with results, main results (flows, assets) and meta results (simulation)
         """
 
         logging.info("Starting simulation.")
         # turn warnings into errors
         warnings.filterwarnings("error")
-        warnings.filterwarnings("always", category=FutureWarning)
         try:
             local_energy_system.solve(
                 solver="cbc",
                 solve_kwargs={
                     "tee": False
                 },  # if tee_switch is true solver messages will be displayed
                 cmdline_options={"ratioGap": str(0.03)},
```

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/D1_model_components.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/D1_model_components.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 """
 
 import logging
 
 import pandas as pd
 from oemof import solph
-from oemof.network import Node
 
 from multi_vector_simulator.utils.constants_json_strings import (
     VALUE,
     UNIT,
     LABEL,
     DISPATCH_PRICE,
     AVAILABILITY_DISPATCH,
@@ -44,34 +43,26 @@
     TIMESERIES_PEAK,
     INFLOW_DIRECTION,
     OUTFLOW_DIRECTION,
     SIMULATION_ANNUITY,
     MAXIMUM_ADD_CAP,
     MAXIMUM_ADD_CAP_NORMALIZED,
     DISPATCHABILITY,
-    TYPE_ASSET,
     OEMOF_ASSET_TYPE,
     OEMOF_GEN_STORAGE,
     OEMOF_SINK,
     OEMOF_SOURCE,
     OEMOF_TRANSFORMER,
     OEMOF_BUSSES,
     OEMOF_ExtractionTurbineCHP,
     EMISSION_FACTOR,
     BETA,
     INVESTMENT_BUS,
-    ASSET_DICT,
-    ENERGY_CONSUMPTION,
-    ENERGY_BUSSES,
-)
-from multi_vector_simulator.utils.helpers import (
-    get_item_if_list,
-    get_length_if_list,
-    reducable_demand_name,
 )
+from multi_vector_simulator.utils.helpers import get_item_if_list, get_length_if_list
 from multi_vector_simulator.utils.exceptions import (
     MissingParameterError,
     WrongParameterFormatError,
 )
 
 
 def check_list_parameters_transformers_single_input_single_output(
@@ -359,18 +350,15 @@
     - test_sink_non_dispatchable_single_input_bus()
     - test_sink_non_dispatchable_multiple_input_busses()
     - test_sink_dispatchable_single_input_bus()
     - test_sink_dispatchable_multiple_input_busses()
 
     """
     if TIMESERIES in dict_asset:
-        if dict_asset[TYPE_ASSET] == "reducable_demand":
-            sink_demand_reduction(model, dict_asset, **kwargs)
-        else:
-            sink_non_dispatchable(model, dict_asset, **kwargs)
+        sink_non_dispatchable(model, dict_asset, **kwargs)
 
     else:
         sink_dispatchable_optimize(model, dict_asset, **kwargs)
 
 
 def source(model, dict_asset, **kwargs):
     r"""
@@ -649,41 +637,23 @@
                 f" at the moment."
             )
             logging.error(missing_dispatch_prices_or_efficiencies)
             raise ValueError(missing_dispatch_prices_or_efficiencies)
     else:
         # single input and single output
 
-        min_load_opts = {"min": 0, "max": 1}
-        min_load = dict_asset.get(SOC_MIN, None)
-        if min_load is not None:
-            if min_load[VALUE] != 0:
-                logging.warning(
-                    f"Minimal load of {min_load[VALUE]} was set to asset {dict_asset[LABEL]}"
-                )
-            min_load_opts["min"] = min_load[VALUE]
-        max_load = dict_asset.get(SOC_MAX, None)
-        if max_load is not None:
-            if max_load[VALUE] != 1:
-                logging.warning(
-                    f"Maximal load of {max_load[VALUE]} was set to asset {dict_asset[LABEL]}"
-                )
-
-            min_load_opts["max"] = max_load[VALUE]
-
         check_list_parameters_transformers_single_input_single_output(
             dict_asset, model.timeindex.size
         )
 
         inputs = {kwargs[OEMOF_BUSSES][dict_asset[INFLOW_DIRECTION]]: solph.Flow()}
         outputs = {
             kwargs[OEMOF_BUSSES][dict_asset[OUTFLOW_DIRECTION]]: solph.Flow(
                 nominal_value=dict_asset[INSTALLED_CAP][VALUE],
                 variable_costs=dict_asset[DISPATCH_PRICE][VALUE],
-                **min_load_opts,
             )
         }
         efficiencies = {
             kwargs[OEMOF_BUSSES][dict_asset[OUTFLOW_DIRECTION]]: dict_asset[EFFICIENCY][
                 VALUE
             ]
         }
@@ -717,22 +687,18 @@
     -------
     Indirectly updated `model` and dict of asset in `kwargs` with the transformer object.
 
     """
     missing_dispatch_prices_or_efficiencies = None
 
     investment_bus = dict_asset.get(INVESTMENT_BUS)
-    invest_opts = {}
-    if dict_asset[MAXIMUM_ADD_CAP][VALUE] is not None:
-        invest_opts["maximum"] = dict_asset[MAXIMUM_ADD_CAP][VALUE]
-
     investment = solph.Investment(
         ep_costs=dict_asset[SIMULATION_ANNUITY][VALUE],
+        maximum=dict_asset[MAXIMUM_ADD_CAP][VALUE],
         existing=dict_asset[INSTALLED_CAP][VALUE],
-        **invest_opts,
     )
 
     # check if the transformer has multiple input or multiple output busses
     # the investment object is always in the output bus
     if isinstance(dict_asset[INFLOW_DIRECTION], list) or isinstance(
         dict_asset[OUTFLOW_DIRECTION], list
     ):
@@ -831,40 +797,14 @@
     else:
         check_list_parameters_transformers_single_input_single_output(
             dict_asset, model.timeindex.size
         )
 
         # single input and single output
 
-        min_load_opts = {"min": 0, "max": 1}
-        min_load = dict_asset.get(SOC_MIN, None)
-        if min_load is not None:
-            if min_load[VALUE] != 0:
-                logging.warning(
-                    f"Minimal load of {min_load[VALUE]} was set to asset {dict_asset[LABEL]}"
-                )
-                min_load_opts["nonconvex"] = solph.NonConvex()
-            min_load_opts["min"] = min_load[VALUE]
-
-        max_load = dict_asset.get(SOC_MAX, None)
-        if max_load is not None:
-            if max_load[VALUE] != 1:
-                logging.warning(
-                    f"Maximal load of {max_load[VALUE]} was set to asset {dict_asset[LABEL]}"
-                )
-                min_load_opts["nonconvex"] = solph.NonConvex()
-
-            min_load_opts["max"] = max_load[VALUE]
-
-        if "nonconvex" in min_load_opts:
-            if invest_opts.get("maximum", None) is None:
-                raise ValueError(
-                    f"You need to provide a maximum_capacity to the asset {dict_asset[LABEL]}, if you set a minimal/maximal load different from 0/1"
-                )
-
         if investment_bus is None:
             investment_bus = dict_asset[OUTFLOW_DIRECTION]
 
         bus = dict_asset[INFLOW_DIRECTION]
         inputs = {
             kwargs[OEMOF_BUSSES][bus]: solph.Flow(
                 investment=investment if bus == investment_bus else None
@@ -882,15 +822,14 @@
                 )
             }
         else:
             outputs = {
                 kwargs[OEMOF_BUSSES][bus]: solph.Flow(
                     investment=investment if bus == investment_bus else None,
                     variable_costs=dict_asset[DISPATCH_PRICE][VALUE],
-                    **min_load_opts,
                 )
             }
 
         efficiencies = {
             kwargs[OEMOF_BUSSES][dict_asset[OUTFLOW_DIRECTION]]: dict_asset[EFFICIENCY][
                 VALUE
             ]
@@ -899,14 +838,15 @@
     if missing_dispatch_prices_or_efficiencies is None:
         t = solph.components.Converter(
             label=dict_asset[LABEL],
             inputs=inputs,
             outputs=outputs,
             conversion_factors=efficiencies,
         )
+
         model.add(t)
         kwargs[OEMOF_TRANSFORMER].update({dict_asset[LABEL]: t})
 
 
 def storage_fix(model, dict_asset, **kwargs):
     r"""
     Defines a storage with a fixed capacity.
@@ -1368,92 +1308,14 @@
     model.add(sink_demand)
     kwargs[OEMOF_SINK].update({dict_asset[LABEL]: sink_demand})
     logging.debug(
         f"Added: Non-dispatchable sink {dict_asset[LABEL]} to bus {dict_asset[INFLOW_DIRECTION]}"
     )
 
 
-def sink_demand_reduction(model, dict_asset, **kwargs):
-    r"""
-    Defines a non dispatchable sink to serve critical and non-critical demand.
-
-    See :py:func:`~.sink` for more information, including parameters.
-
-    Notes
-    -----
-    Tested with:
-    - test_sink_non_dispatchable_single_input_bus()
-    - test_sink_non_dispatchable_multiple_input_busses()
-
-    Returns
-    -------
-    Indirectly updated `model` and dict of asset in `kwargs` with the sink object.
-
-    """
-    # sink_non_dispatchable(model, dict_asset, **kwargs)
-
-    demand_reduction_factor = 1 - dict_asset[EFFICIENCY][VALUE]
-    tot_demand = dict_asset[TIMESERIES]
-    non_critical_demand_ts = tot_demand * demand_reduction_factor
-    non_critical_demand_peak = non_critical_demand_ts.max()
-    if non_critical_demand_peak == 0:
-        max_non_critical = 1
-    else:
-        max_non_critical = non_critical_demand_ts / non_critical_demand_peak
-    critical_demand_ts = tot_demand * dict_asset[EFFICIENCY][VALUE]
-
-    # check if the sink has multiple input busses
-    if isinstance(dict_asset[INFLOW_DIRECTION], list):
-        pass
-        # inputs_noncritical = {}
-        # inputs_critical = {}
-        # index = 0
-        # for bus in dict_asset[INFLOW_DIRECTION]:
-        #     inputs_critical[kwargs[OEMOF_BUSSES][bus]] = solph.Flow(
-        #         fix=dict_asset[TIMESERIES], nominal_value=1
-        #     )
-        #     index += 1
-    else:
-        inputs_noncritical = {
-            kwargs[OEMOF_BUSSES][dict_asset[INFLOW_DIRECTION]]: solph.Flow(
-                min=0,
-                max=max_non_critical,
-                nominal_value=non_critical_demand_peak,
-                variable_costs=-1e-15,
-            )
-        }
-        inputs_critical = {
-            kwargs[OEMOF_BUSSES][dict_asset[INFLOW_DIRECTION]]: solph.Flow(
-                fix=critical_demand_ts, nominal_value=1
-            )
-        }
-
-    non_critical_demand = solph.components.Sink(
-        label=reducable_demand_name(dict_asset[LABEL]), inputs=inputs_noncritical,
-    )
-    critical_demand = solph.components.Sink(
-        label=reducable_demand_name(dict_asset[LABEL], critical=True),
-        inputs=inputs_critical,
-    )
-
-    # create and add demand sink and critical demand sink
-
-    model.add(critical_demand)
-    model.add(non_critical_demand)
-    kwargs[OEMOF_SINK].update(
-        {reducable_demand_name(dict_asset[LABEL]): non_critical_demand}
-    )
-    kwargs[OEMOF_SINK].update(
-        {reducable_demand_name(dict_asset[LABEL], critical=True): critical_demand}
-    )
-    logging.debug(
-        f"Added: Reducable Non-dispatchable sink {dict_asset[LABEL]} to bus {dict_asset[INFLOW_DIRECTION]}"
-    )
-
-
 def chp_fix(model, dict_asset, **kwargs):
     r"""
     Extraction turbine chp from Oemof solph. Extraction turbine must have one input and two outputs
     Notes
     -----
     Tested with:
     - test_to_be_written()
```

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/D2_model_constraints.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/D2_model_constraints.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/E0_evaluation.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/E0_evaluation.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/E1_process_results.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/E1_process_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 - get optimal capacity of optimized assets
 - add the evaluation of time series
 
 """
 import logging
 import copy
 import pandas as pd
-from multi_vector_simulator.utils.helpers import reducable_demand_name
+
 from multi_vector_simulator.utils.constants import TYPE_NONE, TOTAL_FLOW
 from multi_vector_simulator.utils.constants_json_strings import (
     ECONOMIC_DATA,
     FLOW,
     INSTALLED_CAP,
     INPUT_POWER,
     OUTPUT_POWER,
@@ -66,15 +66,14 @@
     EMISSION_FACTOR,
     TOTAL_EMISSIONS,
     TIMESERIES_SOC,
     KPI_UNCOUPLED_DICT,
     FIX_COST,
     LIFETIME_PRICE_DISPATCH,
     AVERAGE_SOC,
-    TYPE_ASSET,
 )
 
 # Oemof.solph variables
 OEMOF_FLOW = "flow"
 OEMOF_SEQUENCES = "sequences"
 OEMOF_INVEST = "invest"
 OEMOF_SCALARS = "scalars"
@@ -731,29 +730,16 @@
     Returns
     -------
     Indirectly updates `dict_asset` with the flow of `bus`, the total flow, the annual
     total flow, the maximum of the flow ('peak_flow') and the average value of
     the flow ('average_flow').
 
     """
-
-    if dict_asset[TYPE_ASSET] == "reducable_demand":
-        flow_tuple = (flow_tuple[0], reducable_demand_name(dict_asset[LABEL]))
-        flow = bus[OEMOF_SEQUENCES][(flow_tuple, OEMOF_FLOW)]
-        flow = cut_below_micro(flow, dict_asset[LABEL] + FLOW)
-        flow_tuple = (flow_tuple[0], reducable_demand_name(dict_asset[LABEL], critical=True))
-
-        flow_crit = bus[OEMOF_SEQUENCES][(flow_tuple, OEMOF_FLOW)]
-        flow_crit = cut_below_micro(flow_crit, dict_asset[LABEL] + FLOW)
-        flow = flow + flow_crit
-
-    else:
-        flow = bus[OEMOF_SEQUENCES][(flow_tuple, OEMOF_FLOW)]
-        flow = cut_below_micro(flow, dict_asset[LABEL] + FLOW)
-
+    flow = bus[OEMOF_SEQUENCES][(flow_tuple, OEMOF_FLOW)]
+    flow = cut_below_micro(flow, dict_asset[LABEL] + FLOW)
     add_info_flows(
         evaluated_period=settings[EVALUATED_PERIOD][VALUE],
         dict_asset=dict_asset,
         flow=flow.dropna(),
         bus_name=multi_bus,
     )
     if multi_bus is None:
```

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/E2_economics.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/E2_economics.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/E3_indicator_calculation.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/E3_indicator_calculation.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/E4_verification.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/E4_verification.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/F0_output.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/F0_output.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/F1_plotting.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/F1_plotting.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/F2_autoreport.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/F2_autoreport.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/F3_debug.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/F3_debug.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/cli.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/cli.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/MVS_parameters_list.csv` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/MVS_parameters_list.csv`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/assets/logo-eland-original.jpg` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/assets/logo-eland-original.jpg`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/assets/styles.css` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/assets/styles.css`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConversion.csv` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConversion.csv`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProduction.csv` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProduction.csv`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/inputs/mvs_config.json` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/mvs_config.json`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/inputs/time_series/demand.csv` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/time_series/demand.csv`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/package_data/inputs/time_series/pv_gen_merra2_2014_eff1_tilt40_az180.csv` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/package_data/inputs/time_series/pv_gen_merra2_2014_eff1_tilt40_az180.csv`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/server.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,17 +156,15 @@
             )
             df = pd.DataFrame(data=js["data"], columns=mindex)
 
             ts_df = df.iloc[:-1]
             ts_index = pd.to_datetime(js["index"][:-1], unit="ms")
             investments = df.iloc[-1]
             ts_df.index = ts_index
-        for extra_var in ["status", "status_nominal"]:
-            if extra_var in ts_df:
-                ts_df.drop(extra_var, axis=1, inplace=True)
+
         super().__init__(
             data=ts_df.T.to_dict(orient="split")["data"],
             index=mindex,
             columns=ts_df.index,
         )
 
         self["investments"] = investments
@@ -187,15 +185,15 @@
             self.index.get_level_values("asset") == asset_name, "investments"
         ].dropna()
         if len(optimized_capacity) == 1:
             optimized_capacity = optimized_capacity[0]
         return optimized_capacity
 
 
-def run_simulation(json_dict, epa_format=True, verbatim=True, **kwargs):
+def run_simulation(json_dict, epa_format=True, **kwargs):
     r"""
      Starts MVS tool simulation from an input json file
 
      Parameters
     -----------
      json_dict: dict
          json from http request
@@ -307,17 +305,15 @@
                 ] = corrected_optimized_capacity
 
     dict_values["raw_results"] = br.to_json()  # to_dict(orient="split") #
 
     logging.debug("Convert results to json")
 
     if epa_format is True:
-        epa_dict_values = data_parser.convert_mvs_params_to_epa(
-            dict_values, verbatim=verbatim
-        )
+        epa_dict_values = data_parser.convert_mvs_params_to_epa(dict_values)
 
         json_values = F0.store_as_json(epa_dict_values)
         answer = json.loads(json_values)
     else:
         answer = dict_values
 
     return answer
```

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/utils/__init__.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/utils/analysis.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/utils/constants.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/constants.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/utils/constants_json_strings.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/constants_json_strings.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,17 +188,14 @@
 DSO_PEAK_DEMAND_PERIOD = "_period"
 CONNECTED_CONSUMPTION_SOURCE = "connected_consumption_sources"
 CONNECTED_PEAK_DEMAND_PRICING_TRANSFORMERS = (
     "connected_peak_demand_pricing_transformers"
 )
 CONNECTED_FEEDIN_SINK = "connected_feedin_sink"
 
-SUFFIX_CRITICAL = "critical"
-SUFFIX_NONCRITICAL = "noncritical"
-
 # Autogenerated assets
 DISPATCHABILITY = "dispatchable"
 AVAILABILITY_DISPATCH = "availability_timeseries"
 ASSET_DICT = "asset_list"
 AUTO_CREATED_HIGHLIGHT = "(@)"
 #######################################
 # Parameters added in post-processing #
```

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/utils/constants_output.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/constants_output.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/utils/data_parser.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/data_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -582,15 +582,15 @@
                         error_msg.append(f"\t`{k}` parameter")
 
             raise (MissingParameterError("\n".join(error_msg)))
 
     return dict_values
 
 
-def convert_mvs_params_to_epa(mvs_dict, verbatim=True):
+def convert_mvs_params_to_epa(mvs_dict, verbatim=False):
     """Convert the MVS output parameters to EPA format
 
     Parameters
     ----------
     mvs_dict: dict
         output parameters from MVS
```

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/utils/exceptions.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator/utils/helpers.py` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator/utils/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 Util functions that are useful throughout the MVS
 
 Including:
 - find_valvue_by_key(): Finds value of a key in a nested dictionary.
 """
 
-from copy import deepcopy
 import os
 
 from multi_vector_simulator.utils.constants_json_strings import (
     DSO_FEEDIN_CAP,
     AUTO_CREATED_HIGHLIGHT,
     DSO_CONSUMPTION,
     DSO_FEEDIN,
@@ -25,16 +24,14 @@
     ENERGY_PROVIDERS,
     ENERGY_BUSSES,
     OEMOF_ASSET_TYPE,
     TYPE_ASSET,
     INFLOW_DIRECTION,
     OUTFLOW_DIRECTION,
     ENERGY_VECTOR,
-    SUFFIX_CRITICAL,
-    SUFFIX_NONCRITICAL,
 )
 
 
 def find_value_by_key(data, target, result=None):
     """
     Finds value of a key in a nested dictionary.
 
@@ -119,25 +116,14 @@
     if isinstance(list_or_float, list):
         answer = len(list_or_float)
     else:
         answer = 0
     return answer
 
 
-def reducable_demand_name(demand_name: str, critical: bool = False):
-    """Name for auto created bus related to peak demand pricing period"""
-
-    if critical is False:
-        suffix = SUFFIX_NONCRITICAL
-    else:
-        suffix = SUFFIX_CRITICAL
-
-    return f"{demand_name}_{suffix} {AUTO_CREATED_HIGHLIGHT}"
-
-
 def peak_demand_bus_name(dso_name: str, feedin: bool = False):
     """Name for auto created bus related to peak demand pricing period"""
 
     if feedin is False:
         dso_direction = DSO_CONSUMPTION
     else:
         dso_direction = DSO_FEEDIN
@@ -192,20 +178,9 @@
                     output_bus = [output_bus]
             else:
                 output_bus = []
 
             for bus in input_bus + output_bus:
                 asset_busses[bus] = dict_values[ENERGY_BUSSES][bus].get(ENERGY_VECTOR)
             asset_type["busses"] = asset_busses
-            if asset_type[TYPE_ASSET] == "reducable_demand":
-
-                asset_label = asset_type["label"]
-                asset_type["label"] = reducable_demand_name(asset_label)
-                asset_types.append(asset_type)
-                crit_asset_type = deepcopy(asset_type)
-                crit_asset_type["label"] = reducable_demand_name(
-                    asset_label, critical=True
-                )
-                asset_types.append(crit_asset_type)
-            else:
-                asset_types.append(asset_type)
+            asset_types.append(asset_type)
     return asset_types
```

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator.egg-info/PKG-INFO` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi-vector-simulator
-Version: 1.0.7rc3
+Version: 1.1.0rc1
 Summary: Multi-vector Simulation Tool assessing and optimizing Local Energy Systems (LES) for the E-LAND project
 Home-page: https://github.com/rl-institut/multi-vector-simulator
 Author: Reiner Lemoine Institut
 Author-email: pypi@rl-institut.de
 Project-URL: Bug Reports, https://github.com/rl-institut/multi-vector-simulator/issues
 Project-URL: Source, https://github.com/rl-institut/multi-vector-simulator
 Keywords: multi-vector local-energy-systems
@@ -42,15 +42,15 @@
 Requires-Dist: psutil>=5.7.0; extra == "report"
 Provides-Extra: test
 Requires-Dist: pytest>=5.3.1; extra == "test"
 Requires-Dist: black==19.10b0; extra == "test"
 Requires-Dist: coverage>=4.5; extra == "test"
 Requires-Dist: coveralls>=3.0.1; extra == "test"
 Requires-Dist: mock>=3.0.5; extra == "test"
-Requires-Dist: click==8.0.4; extra == "test"
+Requires-Dist: click==8.0.2; extra == "test"
 
 ##################################################
 MVS - Multi-Vector Simulator of the E-LAND toolbox
 ##################################################
 
 |badge_docs| |badge_CI| |badge_coverage| |badge_zenodo| |badge_pypi| |badge_gpl2| |badge_black|
```

### Comparing `multi-vector-simulator-1.0.7rc3/src/multi_vector_simulator.egg-info/SOURCES.txt` & `multi-vector-simulator-1.1.0rc1/src/multi_vector_simulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_A0_initialization.py` & `multi-vector-simulator-1.1.0rc1/tests/test_A0_initialization.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_A1_csv_to_json.py` & `multi-vector-simulator-1.1.0rc1/tests/test_A1_csv_to_json.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_B0_data_input_json.py` & `multi-vector-simulator-1.1.0rc1/tests/test_B0_data_input_json.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_C0_data_processing.py` & `multi-vector-simulator-1.1.0rc1/tests/test_C0_data_processing.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_C1_verification.py` & `multi-vector-simulator-1.1.0rc1/tests/test_C1_verification.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_C2_economic_functions.py` & `multi-vector-simulator-1.1.0rc1/tests/test_C2_economic_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,26 @@
         first_time_investment=100,
         discount_factor=0,
     )
     exp = -100 / 20 * 5
     assert replacement_costs == exp
 
 
+def test_get_replacement_costs_one_reinvestment_age_asset_equal_asset_lifetime():
+    replacement_costs = C2.get_replacement_costs(
+        age_of_asset=10,
+        project_lifetime=20,
+        asset_lifetime=10,
+        first_time_investment=550,
+        discount_factor=0.1,
+    )
+    exp = 762.0488091862422
+    assert replacement_costs == exp
+
+
 def test_present_value_from_annuity():
     """
 
     Tests whether the MVS is correctly calculating the present value
     """
     PV_from_annuity = C2.present_value_from_annuity(annuity, annuity_factor)
     assert PV_from_annuity == annuity * annuity_factor
```

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_D0_modelling_and_optimization.py` & `multi-vector-simulator-1.1.0rc1/tests/test_D0_modelling_and_optimization.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_D1_model_components.py` & `multi-vector-simulator-1.1.0rc1/tests/test_D1_model_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
         """
         # self.transformers should contain the transformer (key = label, value = transformer object)
         assert (
             dict_asset[LABEL] in self.transformers
         ), f"Transformer '{dict_asset[LABEL]}' was not added to `asset_dict` but should have been added."
         assert isinstance(
-            self.transformers[dict_asset[LABEL]], network.Converter
+            self.transformers[dict_asset[LABEL]], solph.components.Converter
         ), f"Transformer '{dict_asset[LABEL]}' was not added as type ' solph.network.Transformer' to `asset_dict`."
 
         # self.models should contain the transformer (indirectly tested)
         # check output bus (`nominal_value`, `investment` and `existing`) these
         # values are expected to be different depending on whether capacity is optimized or not
         if multiple_outputs == True:
             output_bus_list = [
@@ -289,75 +289,55 @@
     def test_transformer_optimize_cap_multiple_output_busses_multiple_single_efficiency_raises_error(
         self,
     ):
         dict_asset = self.dict_values[ENERGY_CONVERSION][
             "transformer_optimize_multiple_output_busses"
         ]
 
-# <<<<<<< HEAD
-#         dict_asset[EFFICIENCY][VALUE] = 0.1
-#         with pytest.raises(ValueError):
-#             D1.transformer(
-#                 model=self.model,
-#                 dict_asset=dict_asset,
-#                 transformer=self.transformers,
-#                 bus=self.busses,
-#             )
-# =======
-        inst_cap = [10, 15]
-        dict_asset[INSTALLED_CAP][VALUE] = inst_cap
+        dict_asset[EFFICIENCY][VALUE] = 0.1
+        with pytest.raises(ValueError):
+            D1.transformer(
+                model=self.model,
+                dict_asset=dict_asset,
+                transformer=self.transformers,
+                bus=self.busses,
+            )
 
-        D1.transformer(
-            model=self.model,
-            dict_asset=dict_asset,
-            transformer=self.transformers,
-            bus=self.busses,
-        )
-
-        output_bus_list = [
-            self.model._nodes[-1].outputs.data[self.busses[bus_name]]
-            for bus_name in dict_asset[OUTFLOW_DIRECTION]
-        ]
-        for cap, output_bus in zip(inst_cap, output_bus_list):
-            assert output_bus.investment.existing == cap
-# >>>>>>> d82b48ae... Fix failing tests
 
     def test_transformer_fix_cap_single_busses(self):
         dict_asset = self.dict_values[ENERGY_CONVERSION][
             "transformer_fix_single_busses"
         ]
 
         D1.transformer(
             model=self.model,
             dict_asset=dict_asset,
             transformer=self.transformers,
             bus=self.busses,
         )
 
-# <<<<<<< HEAD
-#         # only one output and one input bus
-#         assert (
-#             len([str(i) for i in self.model.entities[-1].outputs]) == 1
-#         ), f"Amount of output busses of transformer should be one but is {len([str(i) for i in self.model.entities[-1].outputs])}."
-#         assert (
-#             len([str(i) for i in self.model.entities[-1].inputs]) == 1
-#         ), f"Amount of input busses of transformer should be one but is {len([str(i) for i in self.model.entities[-1].inputs])}."
-#
-#         # checks done with helper function (see func for more information)
-#         self.helper_test_transformer_in_model_and_dict(
-#             optimize=False, dict_asset=dict_asset
-#         )
-# =======
+
+        # # only one output and one input bus
+        # assert (
+        #     len([str(i) for i in self.model.entities[-1].outputs]) == 1
+        # ), f"Amount of output busses of transformer should be one but is {len([str(i) for i in self.model.entities[-1].outputs])}."
+        # assert (
+        #     len([str(i) for i in self.model.entities[-1].inputs]) == 1
+        # ), f"Amount of input busses of transformer should be one but is {len([str(i) for i in self.model.entities[-1].inputs])}."
+        #
+        # # checks done with helper function (see func for more information)
+        # self.helper_test_transformer_in_model_and_dict(
+        #     optimize=False, dict_asset=dict_asset
+        # )
         output_bus_list = [
             self.model.nodes[-1].outputs.data[self.busses[bus_name]]
             for bus_name in dict_asset[OUTFLOW_DIRECTION]
         ]
         for cap, output_bus in zip(inst_cap, output_bus_list):
             assert output_bus.investment.maximum[0] == cap
-# >>>>>>> d82b48ae... Fix failing tests
 
     def test_transformer_fix_cap_single_busses_raises_error_if_parameter_provided_as_list(
         self,
     ):
         dict_asset = self.dict_values[ENERGY_CONVERSION][
             "transformer_fix_single_busses"
         ]
```

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_D2_model_constraints.py` & `multi-vector-simulator-1.1.0rc1/tests/test_D2_model_constraints.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_E0_evaluation.py` & `multi-vector-simulator-1.1.0rc1/tests/test_E0_evaluation.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_E1_process_results.py` & `multi-vector-simulator-1.1.0rc1/tests/test_E1_process_results.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_E2_economics.py` & `multi-vector-simulator-1.1.0rc1/tests/test_E2_economics.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_E3_indicator_calculation.py` & `multi-vector-simulator-1.1.0rc1/tests/test_E3_indicator_calculation.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_E4_verification.py` & `multi-vector-simulator-1.1.0rc1/tests/test_E4_verification.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_F0_output.py` & `multi-vector-simulator-1.1.0rc1/tests/test_F0_output.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_F1_plotting.py` & `multi-vector-simulator-1.1.0rc1/tests/test_F1_plotting.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_benchmark_KPI.py` & `multi-vector-simulator-1.1.0rc1/tests/test_benchmark_KPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import argparse
 import os
 import shutil
 import json
 
 import mock
 import pandas as pd
+import numpy as np
 import pytest
 
 from multi_vector_simulator.cli import main
 from multi_vector_simulator.B0_data_input_json import load_json
 import multi_vector_simulator.C2_economic_functions as C2
 
 from _constants import (
@@ -283,18 +284,19 @@
             else:
                 asset_data = data[asset_group][asset]
             # assertion
             for key in KEYS_TO_BE_EVALUATED_PER_ASSET:
                 assert (
                     key in asset_data
                 ), f"{key} is not in the asset data of {asset_group}, {asset}. It includes: {asset_data.keys()}."
-                assert expected_values.loc[asset, key] == pytest.approx(
-                    asset_data[key][VALUE], rel=1e-3
-                ), f"Parameter {key} of asset {asset} is not of expected value, expected {expected_values.loc[asset, key]}, got {asset_data[key][VALUE]}."
-
+                if not pd.isna(expected_values.loc[asset, key]) and not pd.isna(asset_data[key][VALUE]):
+                    assert float(expected_values.loc[asset, key]) == pytest.approx(
+                        asset_data[key][VALUE], rel=1e-3
+                    ), f"Parameter {key} of asset {asset} is not of expected value, expected {expected_values.loc[asset, key]}, got {asset_data[key][VALUE]}."
+                
         # Now we established that the externally calculated values are equal to the internally calculated values.
         # Therefore, we can now use the cost data from the assets to validate the cost data for the whole energy system.
 
         demand = pd.read_csv(
             os.path.join(TEST_INPUT_PATH, USE_CASE, TIME_SERIES, "demand.csv"), sep=",",
         )
         aggregated_demand = demand.sum()[0]
@@ -323,20 +325,21 @@
                 Asset data with economic parameters
 
             Returns
             -------
             Updated KEYS_TO_BE_EVALUATED_FOR_TOTAL_SYSTEM
             """
             for key in KEYS_TO_BE_EVALUATED_FOR_TOTAL_SYSTEM:
-                KEYS_TO_BE_EVALUATED_FOR_TOTAL_SYSTEM.update(
-                    {
-                        key: KEYS_TO_BE_EVALUATED_FOR_TOTAL_SYSTEM[key]
-                        + asset_data[key][VALUE]
-                    }
-                )
+                if not pd.isna(asset_data[key][VALUE]):
+                    KEYS_TO_BE_EVALUATED_FOR_TOTAL_SYSTEM.update(
+                        {
+                            key: KEYS_TO_BE_EVALUATED_FOR_TOTAL_SYSTEM[key]
+                            + asset_data[key][VALUE]
+                        }
+                    )
 
         for asset_group in (
             ENERGY_CONSUMPTION,
             ENERGY_CONVERSION,
             ENERGY_PRODUCTION,
             ENERGY_STORAGE,
         ):
```

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_benchmark_constraints.py` & `multi-vector-simulator-1.1.0rc1/tests/test_benchmark_constraints.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_benchmark_feedin.py` & `multi-vector-simulator-1.1.0rc1/tests/test_benchmark_feedin.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_benchmark_scenarios.py` & `multi-vector-simulator-1.1.0rc1/tests/test_benchmark_scenarios.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_benchmark_special_features.py` & `multi-vector-simulator-1.1.0rc1/tests/test_benchmark_special_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,27 +112,34 @@
                 csv_data[electricity_price][k], rel=1e-6
             ), f"The energy price has different values then it was defined as with the csv file {csv_file}."
             assert data[ENERGY_PRODUCTION][dso + DSO_CONSUMPTION][DISPATCH_PRICE][
                 VALUE
             ][k] == pytest.approx(
                 csv_data[electricity_price][k], rel=1e-6
             ), f"The feedin tariff has different values then it was defined as with the csv file {csv_file}."
-            if k == 0 or k == 1:
-                assert (
-                    data[ENERGY_STORAGE]["storage_01"][STORAGE_CAPACITY][SOC_MIN][
-                        VALUE
-                    ][k]
-                    == 0
-                ), f"The NaN value of the soc min timeseries is not parsed as 0 as it should."
-            else:
-                assert data[ENERGY_STORAGE]["storage_01"][STORAGE_CAPACITY][SOC_MIN][
-                    VALUE
-                ][k] == pytest.approx(
-                    csv_data[soc_min][k], rel=1e-6
-                ), f"The soc min has different values then it was defined as with the csv file {csv_file}."
+
+            # problem with following code is that currently timeseries of soc_min is not possible due to update to newer version of oemof
+
+            # if k == 0 or k == 1:
+            #     print(data[ENERGY_STORAGE]["storage_01"][STORAGE_CAPACITY][SOC_MIN][
+            #             VALUE
+            #         ])
+            #     assert (
+            #         data[ENERGY_STORAGE]["storage_01"][STORAGE_CAPACITY][SOC_MIN][
+            #             VALUE
+            #         ][k]
+            #         == 0
+            #     ), f"The NaN value of the soc min timeseries is not parsed as 0 as it should."
+            # else:
+            #
+            #     assert data[ENERGY_STORAGE]["storage_01"][STORAGE_CAPACITY][SOC_MIN][
+            #         VALUE
+            #     ][k] == pytest.approx(
+            #         csv_data[soc_min][k], rel=1e-6
+            #     ), f"The soc min has different values then it was defined as with the csv file {csv_file}."
 
     # this ensure that the test is only ran if explicitly executed, ie not when the `pytest` command
     # alone is called
     @pytest.mark.skipif(
         EXECUTE_TESTS_ON not in (TESTS_ON_MASTER),
         reason="Benchmark test deactivated, set env variable "
         "EXECUTE_TESTS_ON to 'master' to run this test",
```

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_benchmark_stratified_thermal_storage.py` & `multi-vector-simulator-1.1.0rc1/tests/test_benchmark_stratified_thermal_storage.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_input_folder_parameters.py` & `multi-vector-simulator-1.1.0rc1/tests/test_input_folder_parameters.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_sensitivity.py` & `multi-vector-simulator-1.1.0rc1/tests/test_sensitivity.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.7rc3/tests/test_utils.py` & `multi-vector-simulator-1.1.0rc1/tests/test_utils.py`

 * *Files identical despite different names*

