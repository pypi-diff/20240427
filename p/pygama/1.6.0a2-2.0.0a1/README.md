# Comparing `tmp/pygama-1.6.0a2.tar.gz` & `tmp/pygama-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygama-1.6.0a2.tar", last modified: Mon Feb 19 14:35:21 2024, max compression
+gzip compressed data, was "pygama-2.0.0a1.tar", last modified: Sat Apr 27 18:10:36 2024, max compression
```

## Comparing `pygama-1.6.0a2.tar` & `pygama-2.0.0a1.tar`

### file list

```diff
@@ -1,118 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.771134 pygama-1.6.0a2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-19 14:35:15.000000 pygama-1.6.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-02-19 14:35:21.771134 pygama-1.6.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-02-19 14:35:15.000000 pygama-1.6.0a2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-02-19 14:35:15.000000 pygama-1.6.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-02-19 14:35:21.771134 pygama-1.6.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-19 14:35:15.000000 pygama-1.6.0a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.747134 pygama-1.6.0a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.755134 pygama-1.6.0a2/src/pygama/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-02-19 14:35:21.000000 pygama-1.6.0a2/src/pygama/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12125 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.755134 pygama-1.6.0a2/src/pygama/dsp/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/dsp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.755134 pygama-1.6.0a2/src/pygama/dsp/processors/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/dsp/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.755134 pygama-1.6.0a2/src/pygama/evt/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/evt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19450 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/evt/aggregators.py
--rw-r--r--   0 runner    (1001) docker     (127)    20525 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/evt/build_evt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/evt/build_tcm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.759134 pygama-1.6.0a2/src/pygama/evt/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/evt/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/evt/modules/legend.py
--rw-r--r--   0 runner    (1001) docker     (127)    14011 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/evt/modules/spm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/evt/tcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8030 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/evt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.759134 pygama-1.6.0a2/src/pygama/flow/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62489 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/flow/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    27425 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/flow/file_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/flow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.759134 pygama-1.6.0a2/src/pygama/hit/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/hit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9009 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/hit/build_hit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.759134 pygama-1.6.0a2/src/pygama/lgdo/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/lgdo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.759134 pygama-1.6.0a2/src/pygama/math/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17489 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/math/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    39910 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/math/peak_fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/math/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/math/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.763134 pygama-1.6.0a2/src/pygama/pargen/
--rw-r--r--   0 runner    (1001) docker     (127)    91370 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/pargen/AoE_cal.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/pargen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14040 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/pargen/cuts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/pargen/data_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)    18784 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/pargen/dplms_ge_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    13153 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/pargen/dsp_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)    51533 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/pargen/ecal_th.py
--rw-r--r--   0 runner    (1001) docker     (127)    60876 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/pargen/energy_cal.py
--rw-r--r--   0 runner    (1001) docker     (127)    72845 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/pargen/energy_optimisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9016 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/pargen/extract_tau.py
--rw-r--r--   0 runner    (1001) docker     (127)    32202 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/pargen/lq_cal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11037 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/pargen/mse_psd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13096 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/pargen/noise_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/pargen/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.763134 pygama-1.6.0a2/src/pygama/raw/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/raw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.763134 pygama-1.6.0a2/src/pygama/skm/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/skm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/skm/build_skm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.763134 pygama-1.6.0a2/src/pygama/vis/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-19 14:35:15.000000 pygama-1.6.0a2/src/pygama/vis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.767134 pygama-1.6.0a2/src/pygama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-02-19 14:35:21.000000 pygama-1.6.0a2/src/pygama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-02-19 14:35:21.000000 pygama-1.6.0a2/src/pygama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 14:35:21.000000 pygama-1.6.0a2/src/pygama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-19 14:35:21.000000 pygama-1.6.0a2/src/pygama.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 14:35:21.000000 pygama-1.6.0a2/src/pygama.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-02-19 14:35:21.000000 pygama-1.6.0a2/src/pygama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-19 14:35:21.000000 pygama-1.6.0a2/src/pygama.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.763134 pygama-1.6.0a2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.763134 pygama-1.6.0a2/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/configs/icpc-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/configs/sipm-dplms-config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/configs/sipm-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.763134 pygama-1.6.0a2/tests/evt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.763134 pygama-1.6.0a2/tests/evt/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/evt/configs/basic-evt-config.json
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/evt/configs/module-test-evt-config.json
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/evt/configs/module-test-t0-vov-evt-config.json
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/evt/configs/query-test-evt-config.json
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/evt/configs/vov-test-evt-config.json
--rw-r--r--   0 runner    (1001) docker     (127)    12355 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/evt/test_build_evt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/evt/test_build_tcm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.767134 pygama-1.6.0a2/tests/flow/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.767134 pygama-1.6.0a2/tests/flow/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/flow/configs/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/flow/configs/data-loader-config.json
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/flow/configs/filedb-config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.767134 pygama-1.6.0a2/tests/flow/configs/nested/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/flow/configs/nested/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/flow/configs/nested/data-loader-config-nested.json
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/flow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/flow/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10122 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/flow/test_filedb.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/flow/test_flow_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.767134 pygama-1.6.0a2/tests/hit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.767134 pygama-1.6.0a2/tests/hit/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/hit/configs/aggregations-hit-config.json
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/hit/configs/basic-hit-config.json
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/hit/configs/spms-hit-a-config.json
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/hit/configs/spms-hit-config.json
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/hit/configs/spms-hit-multi-config.json
--rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/hit/test_build_hit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.767134 pygama-1.6.0a2/tests/math/
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/math/test_fwhm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.767134 pygama-1.6.0a2/tests/pargen/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/pargen/test_ecal.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/pargen/test_energy_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.767134 pygama-1.6.0a2/tests/skm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:35:21.767134 pygama-1.6.0a2/tests/skm/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/skm/configs/basic-skm-config.json
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-02-19 14:35:15.000000 pygama-1.6.0a2/tests/skm/test_build_skm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.795232 pygama-2.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 18:10:33.000000 pygama-2.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-27 18:10:36.795232 pygama-2.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-27 18:10:33.000000 pygama-2.0.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-27 18:10:33.000000 pygama-2.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 18:10:36.795232 pygama-2.0.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.767232 pygama-2.0.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.771232 pygama-2.0.0a1/src/pygama/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-27 18:10:36.000000 pygama-2.0.0a1/src/pygama/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.771232 pygama-2.0.0a1/src/pygama/dsp/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/dsp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.771232 pygama-2.0.0a1/src/pygama/dsp/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/dsp/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.775231 pygama-2.0.0a1/src/pygama/evt/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/evt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15979 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/evt/aggregators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20976 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/evt/build_evt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/evt/build_tcm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.775231 pygama-2.0.0a1/src/pygama/evt/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/evt/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/evt/modules/geds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/evt/modules/larveto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/evt/modules/legend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/evt/modules/spms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/evt/tcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7577 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/evt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.775231 pygama-2.0.0a1/src/pygama/flow/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62482 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/flow/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27426 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/flow/file_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/flow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.775231 pygama-2.0.0a1/src/pygama/hit/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/hit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/hit/build_hit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.775231 pygama-2.0.0a1/src/pygama/lgdo/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/lgdo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.775231 pygama-2.0.0a1/src/pygama/math/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13992 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/binned_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/distributions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.779232 pygama-2.0.0a1/src/pygama/math/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/crystal_ball.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/error_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/exgauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/exponential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/gauss_on_exgauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/gauss_on_exponential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/gauss_on_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/gauss_on_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/gauss_on_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/hpge_peak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/moyal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/poisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/pygama_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10727 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30820 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/sum_dists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/triple_gauss_on_double_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26563 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/hpge_peak_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/least_squares.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/unbinned_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.783232 pygama-2.0.0a1/src/pygama/pargen/
+-rw-r--r--   0 runner    (1001) docker     (127)    84627 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/pargen/AoE_cal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/pargen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35158 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/pargen/data_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18349 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/pargen/dplms_ge_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29751 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/pargen/dsp_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95343 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/pargen/energy_cal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17554 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/pargen/energy_optimisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/pargen/extract_tau.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32272 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/pargen/lq_cal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11949 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/pargen/noise_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/pargen/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.783232 pygama-2.0.0a1/src/pygama/raw/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.783232 pygama-2.0.0a1/src/pygama/vis/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/vis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.791232 pygama-2.0.0a1/src/pygama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-27 18:10:36.000000 pygama-2.0.0a1/src/pygama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-27 18:10:36.000000 pygama-2.0.0a1/src/pygama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 18:10:36.000000 pygama-2.0.0a1/src/pygama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-27 18:10:36.000000 pygama-2.0.0a1/src/pygama.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 18:10:36.000000 pygama-2.0.0a1/src/pygama.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-27 18:10:36.000000 pygama-2.0.0a1/src/pygama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-27 18:10:36.000000 pygama-2.0.0a1/src/pygama.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.783232 pygama-2.0.0a1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.783232 pygama-2.0.0a1/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/configs/icpc-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/configs/sipm-dplms-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/configs/sipm-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.783232 pygama-2.0.0a1/tests/evt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.783232 pygama-2.0.0a1/tests/evt/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/evt/configs/basic-evt-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/evt/configs/query-test-evt-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/evt/configs/spms-module-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/evt/configs/vov-test-evt-config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.783232 pygama-2.0.0a1/tests/evt/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/evt/modules/larveto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/evt/test_build_evt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/evt/test_build_tcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/evt/test_evt_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.787232 pygama-2.0.0a1/tests/flow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.787232 pygama-2.0.0a1/tests/flow/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/flow/configs/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/flow/configs/data-loader-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/flow/configs/filedb-config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.787232 pygama-2.0.0a1/tests/flow/configs/nested/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/flow/configs/nested/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/flow/configs/nested/data-loader-config-nested.json
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/flow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/flow/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/flow/test_filedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/flow/test_flow_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.787232 pygama-2.0.0a1/tests/hit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.787232 pygama-2.0.0a1/tests/hit/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/hit/configs/aggregations-hit-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/hit/configs/basic-hit-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/hit/configs/spms-hit-a-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/hit/configs/spms-hit-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/hit/configs/spms-hit-multi-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/hit/test_build_hit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.787232 pygama-2.0.0a1/tests/math/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.791232 pygama-2.0.0a1/tests/math/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_crystal_ball.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_error_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_exgauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_exponential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_gauss_on_exgauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_gauss_on_exponential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_gauss_on_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_gauss_on_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_gauss_on_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_hpge_peak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_moyal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_numba_frozen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_poisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_sum_dists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_triple_gauss_on_double_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/test_binned_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/test_distribution_selector_in_sum_dists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/test_hpge_peak_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/test_iminuit_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/test_least_squares.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/test_math_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/test_math_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/test_unbinned_fitting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.791232 pygama-2.0.0a1/tests/pargen/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/pargen/test_aoecal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/pargen/test_datacleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/pargen/test_ecal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/pargen/test_energy_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/pargen/test_lqcal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/test_utils.py
```

### Comparing `pygama-1.6.0a2/LICENSE` & `pygama-2.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygama-1.6.0a2/PKG-INFO` & `pygama-2.0.0a1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 Metadata-Version: 2.1
 Name: pygama
-Version: 1.6.0a2
-Summary: Python package for decoding and processing digitizer data
-Home-page: https://github.com/legend-exp/pygama
+Version: 2.0.0a1
+Summary: Python package for data processing and analysis
 Author: The LEGEND collaboration
 Maintainer: The LEGEND collaboration
-License: GPL-3.0
-Project-URL: Documentation, https://pygama.readthedocs.io
+Project-URL: Homepage, https://github.com/legend-exp/pygama
+Project-URL: Bug Tracker, https://github.com/legend-exp/pygama/issues
+Project-URL: Discussions, https://github.com/legend-exp/pygama/discussions
+Project-URL: Changelog, https://github.com/legend-exp/pygama/releases
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Software Development
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: hist
 Requires-Dist: colorlog
-Requires-Dist: dspeed>=1.3.0a4
+Requires-Dist: dspeed>=1.3
 Requires-Dist: h5py>=3.2
 Requires-Dist: iminuit
-Requires-Dist: legend-daq2lh5>=1.2.0a1
-Requires-Dist: legend-pydataobj>=1.5.0a5
+Requires-Dist: legend-daq2lh5>=1.2.1
+Requires-Dist: legend-pydataobj>=1.6
 Requires-Dist: matplotlib
 Requires-Dist: numba!=0.53.*,!=0.54.*,!=0.57
 Requires-Dist: numpy>=1.21
 Requires-Dist: pandas>=1.4.4
 Requires-Dist: pint
+Requires-Dist: pyyaml
 Requires-Dist: scikit-learn
 Requires-Dist: scipy>=1.0.1
 Requires-Dist: tables
-Requires-Dist: tqdm>=4.27
+Requires-Dist: tqdm>=4.66
 Provides-Extra: all
 Requires-Dist: pygama[docs,test]; extra == "all"
 Provides-Extra: docs
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: jupyter; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: nbsphinx; extra == "docs"
@@ -67,14 +65,15 @@
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Codecov](https://img.shields.io/codecov/c/github/legend-exp/pygama?logo=codecov)](https://app.codecov.io/gh/legend-exp/pygama)
 [![GitHub issues](https://img.shields.io/github/issues/legend-exp/pygama?logo=github)](https://github.com/legend-exp/pygama/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/legend-exp/pygama?logo=github)](https://github.com/legend-exp/pygama/pulls)
 [![License](https://img.shields.io/github/license/legend-exp/pygama)](https://github.com/legend-exp/pygama/blob/main/LICENSE)
 [![Read the Docs](https://img.shields.io/readthedocs/pygama?logo=readthedocs)](https://pygama.readthedocs.io)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10614246.svg)](https://zenodo.org/doi/10.5281/zenodo.10614246)
 
 *pygama* is a Python package for:
 
 - converting physics data acquisition system output to
   [LH5-format](https://legend-exp.github.io/legend-data-format-specs) HDF5
   files (functionality provided by the
   [legend-pydataobj](https://legend-pydataobj.readthedocs.io) and
@@ -83,11 +82,18 @@
   (functionality provided by the [dspeed](https://dspeed.readthedocs.io)
   package)
 - optimizing DSP routines and tuning associated analysis parameters
 - generating and selecting high-level event data for further analysis
 
 Check out the [online documentation](https://pygama.readthedocs.io).
 
+If you are using this software, consider
+[citing](https://zenodo.org/doi/10.5281/zenodo.10614246)!
+
 ## Related repositories
-- [legend-exp/legend-pydataobj](https://github.com/legend-exp/legend-pydataobj) → LEGEND Python Data Objects
-- [legend-exp/legend-daq2lh5](https://github.com/legend-exp/legend-daq2lh5) → Convert digitizer data to LEGEND HDF5
-- [legend-exp/dspeed](https://github.com/legend-exp/dspeed) → Fast Digital Signal Processing for particle detector signals in Python
+
+- [legend-exp/legend-pydataobj](https://github.com/legend-exp/legend-pydataobj)
+  → LEGEND Python Data Objects
+- [legend-exp/legend-daq2lh5](https://github.com/legend-exp/legend-daq2lh5)
+  → Convert digitizer data to LEGEND HDF5
+- [legend-exp/dspeed](https://github.com/legend-exp/dspeed)
+  → Fast Digital Signal Processing for particle detector signals in Python
```

### Comparing `pygama-1.6.0a2/src/pygama/cli.py` & `pygama-2.0.0a1/src/pygama/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 pygama's command line interface utilities.
 """
+
 import argparse
 import logging
 import os
 import sys
 
 import numpy as np
 from daq2lh5 import build_raw
```

### Comparing `pygama-1.6.0a2/src/pygama/evt/build_evt.py` & `pygama-2.0.0a1/src/pygama/evt/build_evt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,86 @@
 """
 This module implements routines to build the `evt` tier.
 """
 
 from __future__ import annotations
 
+import importlib
 import itertools
-import json
 import logging
 import re
-from importlib import import_module
+from collections.abc import Mapping, Sequence
+from typing import Any
 
 import awkward as ak
 import numpy as np
 from lgdo import Array, ArrayOfEqualSizedArrays, Table, VectorOfVectors, lh5
-from lgdo.lh5 import LH5Store
 
+from ..utils import load_dict
 from . import aggregators, utils
 
 log = logging.getLogger(__name__)
 
 
 def build_evt(
-    f_tcm: str,
-    f_dsp: str,
-    f_hit: str,
-    evt_config: str | dict,
-    f_evt: str | None = None,
+    datainfo: utils.DataInfo | Mapping[str, Sequence[str, ...]],
+    config: str | Mapping[str, ...],
     wo_mode: str = "write_safe",
-    evt_group: str = "evt",
-    tcm_group: str = "hardware_tcm_1",
-    dsp_group: str = "dsp",
-    hit_group: str = "hit",
-    tcm_id_table_pattern: str = "ch{}",
 ) -> None | Table:
-    """Transform data from the `hit` and `dsp` levels which a channel sorted to a
-    event sorted data format.
+    r"""Transform data from hit-structured tiers to event-structured data.
 
     Parameters
     ----------
-    f_tcm
-        input LH5 file of the `tcm` level.
-    f_dsp
-        input LH5 file of the `dsp` level.
-    f_hit
-        input LH5 file of the `hit` level.
-    evt_config
+    datainfo
+        input and output LH5 datainfo with HDF5 groups where tables are found,
+        (see :obj:`.utils.DataInfo`). Example: ::
+
+            # syntax: {"tier-name": ("file-name", "hdf5-group"[, "table-format"])}
+            {
+              "tcm": ("data-tier_tcm.lh5", "hardware_tcm_1"),
+              "dsp": ("data-tier_dsp.lh5", "dsp", "ch{}"),
+              "hit": ("data-tier_hit.lh5", "hit", "ch{}"),
+              "evt": ("data-tier_evt.lh5", "evt")
+            }
+
+    config
         name of configuration file or dictionary defining event fields. Channel
         lists can be defined by importing a metadata module.
 
-        - ``operations`` defines the fields ``name=key``, where ``channels``
-          specifies the channels used to for this field (either a string or a
-          list of strings),
+        - ``channels`` specifies the channels used to for this field (either a
+          string or a list of strings).
+        - ``operations`` defines the event fields (``name=key``). If the key
+          contains slahes it will be interpreted as the path to the output
+          field inside nested sub-tables.
+        - ``outputs`` defines the fields that are actually included in the
+          output table.
+
+        Inside the ``operations`` block:
+
         - ``aggregation_mode`` defines how the channels should be combined (see
           :func:`evaluate_expression`).
-        - ``expression`` defnies the mathematical/special function to apply
+        - ``expression`` defines the expression or function call to apply
           (see :func:`evaluate_expression`),
         - ``query`` defines an expression to mask the aggregation.
         - ``parameters`` defines any other parameter used in expression.
+        - ``dtype`` defines the NumPy data type of the resulting data.
+        - ``initial`` defines the initial/default value. Useful with some types
+          of aggregators.
 
         For example:
 
         .. code-block:: json
 
             {
               "channels": {
                 "geds_on": ["ch1084803", "ch1084804", "ch1121600"],
                 "spms_on": ["ch1057600", "ch1059201", "ch1062405"],
                 "muon": "ch1027202",
               },
+              "outputs": ["energy_id", "multiplicity"],
               "operations": {
                 "energy_id":{
                   "channels": "geds_on",
                   "aggregation_mode": "gather",
                   "query": "hit.cuspEmax_ctc_cal > 25",
                   "expression": "tcm.array_id",
                   "sort": "ascend_by:dsp.tp_0_est"
@@ -79,511 +88,489 @@
                 "energy":{
                   "aggregation_mode": "keep_at_ch:evt.energy_id",
                   "expression": "hit.cuspEmax_ctc_cal > 25"
                 }
                 "is_muon_rejected":{
                   "channels": "muon",
                   "aggregation_mode": "any",
-                  "expression": "dsp.wf_max>a",
-                  "parameters": {"a":15100},
+                  "expression": "dsp.wf_max > a",
+                  "parameters": {"a": 15100},
                   "initial": false
                 },
                 "multiplicity":{
                   "channels":  ["geds_on", "geds_no_psd", "geds_ac"],
                   "aggregation_mode": "sum",
                   "expression": "hit.cuspEmax_ctc_cal > a",
-                  "parameters": {"a":25},
+                  "parameters": {"a": 25},
                   "initial": 0
                 },
                 "t0":{
                   "aggregation_mode": "keep_at_ch:evt.energy_id",
-                  "expression": "dsp.tp_0_est"
+                  "expression": "dsp.tp_0_est",
+                  "initial": "np.nan"
                 },
                 "lar_energy":{
                   "channels": "spms_on",
                   "aggregation_mode": "function",
-                  "expression": ".modules.spm.get_energy(0.5, evt.t0, 48000, 1000, 5000)"
+                  "expression": "pygama.evt.modules.spms.gather_pulse_data(<...>, observable='hit.energy_in_pe')"
                 },
               }
             }
 
-    f_evt
-        name of the output file. If ``None``, return the output :class:`.Table`
-        instead of writing to disk.
     wo_mode
-        writing mode.
-    evt group
-        LH5 root group name of `evt` tier.
-    tcm_group
-        LH5 root group in `tcm` file.
-    dsp_group
-        LH5 root group in `dsp` file.
-    hit_group
-        LH5 root group in `hit` file.
-    tcm_id_table_pattern
-        pattern to format `tcm` id values to table name in higher tiers. Must
-        have one placeholder which is the `tcm` id.
+        writing mode, see :func:`lgdo.lh5.core.write`.
     """
+    if not isinstance(config, dict):
+        config = load_dict(config)
 
-    store = LH5Store()
-    tbl_cfg = evt_config
-    if not isinstance(tbl_cfg, (str, dict)):
-        raise TypeError()
-    if isinstance(tbl_cfg, str):
-        with open(tbl_cfg) as f:
-            tbl_cfg = json.load(f)
-
-    if "channels" not in tbl_cfg.keys():
+    if "channels" not in config.keys():
         raise ValueError("channel field needs to be specified in the config")
-    if "operations" not in tbl_cfg.keys():
+    if "operations" not in config.keys():
         raise ValueError("operations field needs to be specified in the config")
 
-    # check tcm_id_table_pattern validity
-    pattern_check = re.findall(r"{([^}]*?)}", tcm_id_table_pattern)
+    # convert into a nice named tuple
+    f = utils.make_files_config(datainfo)
+
+    # check chname_fmt validity
+    chname_fmt = f.hit.table_fmt
+    pattern_check = re.findall(r"{([^}]*?)}", chname_fmt)
     if len(pattern_check) != 1:
-        raise ValueError(
-            f"tcm_id_table_pattern must have exactly one placeholder. {tcm_id_table_pattern} is invalid."
-        )
+        raise ValueError("chname_fmt must have exactly one placeholder {}")
     elif "{" in pattern_check[0] or "}" in pattern_check[0]:
-        raise ValueError(
-            f"tcm_id_table_pattern {tcm_id_table_pattern} has an invalid placeholder."
-        )
+        raise ValueError(f"{chname_fmt=} has an invalid placeholder.")
 
     if (
         utils.get_table_name_by_pattern(
-            tcm_id_table_pattern,
-            utils.get_tcm_id_by_pattern(tcm_id_table_pattern, lh5.ls(f_hit)[0]),
+            chname_fmt,
+            utils.get_tcm_id_by_pattern(chname_fmt, lh5.ls(f.hit.file)[0]),
         )
-        != lh5.ls(f_hit)[0]
+        != lh5.ls(f.hit.file)[0]
     ):
-        raise ValueError(
-            f"tcm_id_table_pattern {tcm_id_table_pattern} does not match keys in data!"
-        )
+        raise ValueError(f"chname_fmt {chname_fmt} does not match keys in data!")
 
     # create channel list according to config
     # This can be either read from the meta data
     # or a list of channel names
-    log.debug("Creating channel dictionary")
+    log.debug("creating channel dictionary")
 
-    chns = {}
+    channels = {}
 
-    for k, v in tbl_cfg["channels"].items():
+    for key, v in config["channels"].items():
         if isinstance(v, dict):
             # it is a meta module. module_name must exist
             if "module" not in v.keys():
                 raise ValueError(
                     "Need module_name to load channel via a meta data module"
                 )
 
             attr = {}
-            # the time_key argument is set to the time key of the DSP file
-            # in case it is not provided by the config
+            # the time_key argument is mandatory
             if "time_key" not in v.keys():
-                attr["time_key"] = re.search(r"\d{8}T\d{6}Z", f_dsp).group(0)
+                raise RuntimeError("the 'time_key' configuration field is mandatory")
 
             # if "None" do None
             elif "None" == v["time_key"]:
                 attr["time_key"] = None
 
             # load module
             p, m = v["module"].rsplit(".", 1)
-            met = getattr(import_module(p, package=__package__), m)
-            chns[k] = met(v | attr)
+            met = getattr(importlib.import_module(p, package=__package__), m)
+            channels[key] = met(v | attr)
 
         elif isinstance(v, str):
-            chns[k] = [v]
+            channels[key] = [v]
 
         elif isinstance(v, list):
-            chns[k] = [e for e in v]
-
-    nrows = store.read_n_rows(f"/{tcm_group}/cumulative_length", f_tcm)
+            channels[key] = [e for e in v]
 
-    table = Table(size=nrows)
+    # load tcm data from disk
+    tcm = utils.TCMData(
+        id=lh5.read_as(f"/{f.tcm.group}/array_id", f.tcm.file, library="np"),
+        idx=lh5.read_as(f"/{f.tcm.group}/array_idx", f.tcm.file, library="np"),
+        cumulative_length=lh5.read_as(
+            f"/{f.tcm.group}/cumulative_length", f.tcm.file, library="np"
+        ),
+    )
 
-    for k, v in tbl_cfg["operations"].items():
-        log.debug("Processing field " + k)
+    # get number of events in file (ask the TCM)
+    n_rows = len(tcm.cumulative_length)
+    table = Table(size=n_rows)
+
+    # now loop over operations (columns in evt table)
+    for field, v in config["operations"].items():
+        log.debug(f"processing field: '{field}'")
 
-        # if mode not defined in operation, it can only be an operation on the evt level.
+        # if mode not defined in operation, it can only be an operation on the
+        # evt level
         if "aggregation_mode" not in v.keys():
-            var = {}
-            if "parameters" in v.keys():
-                var = var | v["parameters"]
-            res = table.eval(v["expression"].replace(f"{evt_group}.", ""), var)
+            # compute and eventually get rid of evt. suffix
+            obj = table.eval(
+                v["expression"].replace("evt.", ""), v.get("parameters", {})
+            )
 
-            # add attribute if present
+            # add attributes if present
             if "lgdo_attrs" in v.keys():
-                res.attrs |= v["lgdo_attrs"]
-
-            table.add_field(k, res)
+                obj.attrs |= v["lgdo_attrs"]
 
-        # Else we build the event entry
+        # else we build the event entry
         else:
             if "channels" not in v.keys():
-                chns_e = []
+                channels_e = []
             elif isinstance(v["channels"], str):
-                chns_e = chns[v["channels"]]
+                channels_e = channels[v["channels"]]
             elif isinstance(v["channels"], list):
-                chns_e = list(
-                    itertools.chain.from_iterable([chns[e] for e in v["channels"]])
+                channels_e = list(
+                    itertools.chain.from_iterable([channels[e] for e in v["channels"]])
                 )
-            chns_rm = []
+            channels_skip = []
             if "exclude_channels" in v.keys():
                 if isinstance(v["exclude_channels"], str):
-                    chns_rm = chns[v["exclude_channels"]]
+                    channels_skip = channels[v["exclude_channels"]]
                 elif isinstance(v["exclude_channels"], list):
-                    chns_rm = list(
+                    channels_skip = list(
                         itertools.chain.from_iterable(
-                            [chns[e] for e in v["exclude_channels"]]
+                            [channels[e] for e in v["exclude_channels"]]
                         )
                     )
 
-            pars, qry, defaultv, srter = None, None, np.nan, None
-            if "parameters" in v.keys():
-                pars = v["parameters"]
-            if "query" in v.keys():
-                qry = v["query"]
-            if "initial" in v.keys():
-                defaultv = v["initial"]
-                if isinstance(defaultv, str) and (
-                    defaultv in ["np.nan", "np.inf", "-np.inf"]
-                ):
-                    defaultv = eval(defaultv)
-            if "sort" in v.keys():
-                srter = v["sort"]
+            defaultv = v.get("initial", np.nan)
+            if isinstance(defaultv, str) and (
+                defaultv in ["np.nan", "np.inf", "-np.inf"]
+            ):
+                defaultv = eval(defaultv)
 
             obj = evaluate_expression(
-                f_tcm=f_tcm,
-                f_hit=f_hit,
-                f_dsp=f_dsp,
-                chns=chns_e,
-                chns_rm=chns_rm,
+                datainfo,
+                tcm,
+                channels=channels_e,
+                channels_skip=channels_skip,
                 mode=v["aggregation_mode"],
                 expr=v["expression"],
-                nrows=nrows,
+                n_rows=n_rows,
                 table=table,
-                para=pars,
-                qry=qry,
-                defv=defaultv,
-                sorter=srter,
-                tcm_id_table_pattern=tcm_id_table_pattern,
-                evt_group=evt_group,
-                hit_group=hit_group,
-                dsp_group=dsp_group,
-                tcm_group=tcm_group,
+                parameters=v.get("parameters", None),
+                query=v.get("query", None),
+                default_value=defaultv,
+                sorter=v.get("sort", None),
             )
 
             # add attribute if present
             if "lgdo_attrs" in v.keys():
                 obj.attrs |= v["lgdo_attrs"]
 
-            table.add_field(k, obj)
-
-    # write output fields into f_evt
-    if "outputs" in tbl_cfg.keys():
-        if len(tbl_cfg["outputs"]) < 1:
-            log.warning("No output fields specified, no file will be written.")
-            return table
-        else:
-            clms_to_remove = [e for e in table.keys() if e not in tbl_cfg["outputs"]]
-            for fld in clms_to_remove:
-                table.remove_field(fld, True)
-
-            if f_evt:
-                store.write(
-                    obj=table, name=f"/{evt_group}/", lh5_file=f_evt, wo_mode=wo_mode
-                )
-            else:
-                return table
+        # cast to type, if required
+        # hijack the poor LGDO
+        if "dtype" in v:
+            type_ = v["dtype"]
+
+            if isinstance(obj, Array):
+                obj.nda = obj.nda.astype(type_)
+            if isinstance(obj, VectorOfVectors):
+                fldata_ptr = obj.flattened_data
+                while isinstance(fldata_ptr, VectorOfVectors):
+                    fldata_ptr = fldata_ptr.flattened_data
+
+                fldata_ptr.nda = fldata_ptr.nda.astype(type_)
+
+        log.debug(f"new column {field!s} = {obj!r}")
+        table.add_field(field, obj)
+
+    # might need to re-organize fields in subtables, create a new object for that
+    nested_tbl = Table(size=n_rows)
+    output_fields = config.get("outputs", table.keys())
+
+    for field, obj in table.items():
+        # also only add fields requested by the user
+        if field not in output_fields:
+            continue
+
+        # if names contain slahes, put in sub-tables
+        lvl_ptr = nested_tbl
+        subfields = field.strip("/").split("___")
+        for level in subfields:
+            # if we are at the end, just add the field
+            if level == subfields[-1]:
+                lvl_ptr.add_field(level, obj)
+                break
+
+            if not level:
+                msg = f"invalid field name '{field}'"
+                raise RuntimeError(msg)
+
+            # otherwise, increase nesting
+            if level not in lvl_ptr:
+                lvl_ptr.add_field(level, Table(size=n_rows))
+            lvl_ptr = lvl_ptr[level]
+
+    # write output fields into outfile
+    if output_fields:
+        if f.evt.file is None:
+            return nested_tbl
+
+        lh5.write(
+            obj=nested_tbl,
+            name=f.evt.group,
+            lh5_file=f.evt.file,
+            wo_mode=wo_mode,
+        )
     else:
-        log.warning("No output fields specified, no file will be written.")
-
-    key = re.search(r"\d{8}T\d{6}Z", f_hit).group(0)
-    log.info(
-        f"Applied {len(tbl_cfg['operations'])} operations to key {key} and saved "
-        f"{len(tbl_cfg['outputs'])} evt fields across {len(chns)} channel groups"
-    )
+        log.warning("no output fields specified, no file will be written.")
+        return nested_tbl
 
 
 def evaluate_expression(
-    f_tcm: str,
-    f_hit: str,
-    f_dsp: str,
-    chns: list,
-    chns_rm: list,
+    datainfo: utils.DataInfo | Mapping[str, Sequence[str, ...]],
+    tcm: utils.TCMData,
+    channels: Sequence[str],
+    channels_skip: Sequence[list],
     mode: str,
     expr: str,
-    nrows: int,
+    n_rows: int,
     table: Table = None,
-    para: dict = None,
-    qry: str = None,
-    defv: bool | int | float = np.nan,
+    parameters: Mapping[str, Any] = None,
+    query: str = None,
+    default_value: bool | int | float = np.nan,
     sorter: str = None,
-    tcm_id_table_pattern: str = "ch{}",
-    evt_group: str = "evt",
-    hit_group: str = "hit",
-    dsp_group: str = "dsp",
-    tcm_group: str = "tcm",
 ) -> Array | ArrayOfEqualSizedArrays | VectorOfVectors:
     """Evaluates the expression defined by the user across all channels
     according to the mode.
 
     Parameters
     ----------
-    f_tcm
-       path to `tcm` tier file.
-    f_hit
-       path to `hit` tier file.
-    f_dsp
-       path to `dsp` tier file.
-    chns
-       list of channel names across which expression gets evaluated (form:
-       ``ch<rawid>``).
-    chns_rm
+    datainfo
+        input and output LH5 files with HDF5 groups where tables are found.
+        (see :obj:`.utils.DataInfo`)
+    tcm
+        tcm data structure (see :obj:`.utils.TCMData`)
+    channels
+       list of channel names across which expression gets evaluated
+    channels_skip
        list of channels which get set to default value during evaluation. In
-       function mode they are removed entirely (form: ``ch<rawid>``)
+       function mode they are removed entirely
     mode
        The mode determines how the event entry is calculated across channels.
        Options are:
 
        - ``first_at:sorter``: aggregates across channels by returning the
          expression of the channel with smallest value of sorter.
        - ``last_at``: aggregates across channels by returning the expression of
          the channel with largest value of sorter.
        - ``sum``: aggregates by summation.
        - ``any``: aggregates by logical or.
        - ``all``: aggregates by logical and.
        - ``keep_at_ch:ch_field``: aggregates according to passed ch_field.
        - ``keep_at_idx:tcm_idx_field``: aggregates according to passed tcm
          index field.
-       - ``gather``: Channels are not combined, but result saved as
+       - ``gather``: channels are not combined, but result saved as
          :class:`.VectorOfVectors`.
+       - ``function``: the function call specified in `expr` is evaluated, and
+         the resulting column is inserted into the output table.
 
-    qry
+    query
        a query that can mask the aggregation.
     expr
        the expression. That can be any mathematical equation/comparison. If
        `mode` is ``function``, the expression needs to be a special processing
-       function defined in modules (e.g. :func:`.modules.spm.get_energy`). In
-       the expression parameters from either hit, dsp, evt tier (from
-       operations performed before this one! Dictionary operations order
-       matters), or from the ``parameters`` field can be used.
-    nrows
+       function defined in :mod:`.modules`. In the expression, parameters from
+       either `evt` or lower tiers (from operations performed before this one!
+       Dictionary operations order matters), or from the ``parameters`` field
+       can be used. Fields can be prefixed with the tier id (e.g.
+       ``evt.energy`` or `hit.quality_flag``).
+    n_rows
        number of rows to be processed.
     table
        table of `evt` tier data.
-    para
+    parameters
        dictionary of parameters defined in the ``parameters`` field in the
        configuration dictionary.
-    defv
+    default_value
        default value of evaluation.
     sorter
        can be used to sort vector outputs according to sorter expression (see
-       :func:`evaluate_to_vector`).
-    tcm_id_table_pattern
-        pattern to format tcm id values to table name in higher tiers. Must have one
-        placeholder which is the `tcm` id.
-    evt group
-        LH5 root group name of `evt` tier.
-    tcm_group
-        LH5 root group in `tcm` file.
-    dsp_group
-        LH5 root group in `dsp` file.
-    hit_group
-        LH5 root group in `hit` file.
-    """
+       :func:`.evaluate_to_vector`).
 
-    store = LH5Store()
+    Note
+    ----
+    The specification of custom functions that can be used as expression is
+    documented in :mod:`.modules`.
+    """
+    f = utils.make_files_config(datainfo)
 
-    # find parameters in evt file or in parameters
-    exprl = re.findall(
-        rf"({evt_group}|{hit_group}|{dsp_group}).([a-zA-Z_$][\w$]*)", expr
-    )
-    var_ph = {}
-    if table:
-        var_ph = var_ph | {
-            e: table[e].view_as("ak")
-            for e in table.keys()
-            if isinstance(table[e], (Array, ArrayOfEqualSizedArrays, VectorOfVectors))
+    # build dictionary of parameter names and their values
+    # a parameter can be a column in the existing table...
+    pars_dict = {}
+
+    if table is not None:
+        pars_dict = {
+            k: v for k, v in table.items() if isinstance(v, (Array, VectorOfVectors))
         }
-    if para:
-        var_ph = var_ph | para
+
+    # ...or defined through the configuration
+    if parameters:
+        pars_dict = pars_dict | parameters
 
     if mode == "function":
-        # evaluate expression
-        func, params = expr.split("(")
-        params = (
-            params.replace(f"{dsp_group}.", f"{dsp_group}_")
-            .replace(f"{hit_group}.", f"{hit_group}_")
-            .replace(f"{evt_group}.", "")
+        # syntax:
+        #
+        #     pygama.evt.modules.spms.my_func([...], arg1=val, arg2=val)
+
+        # get arguments list passed to the function (outermost parentheses)
+        args_str = re.search(r"\((.*)\)$", expr.strip()).group(1)
+
+        # handle tier scoping: evt.<>
+        args_str = args_str.replace("evt.", "")
+
+        good_chns = [x for x in channels if x not in channels_skip]
+
+        # replace stuff before first comma with list of mandatory args
+        full_args_str = "datainfo, tcm, table_names," + ",".join(
+            args_str.split(",")[1:]
         )
-        params = [
-            f_hit,
-            f_dsp,
-            f_tcm,
-            hit_group,
-            dsp_group,
-            tcm_group,
-            tcm_id_table_pattern,
-            [x for x in chns if x not in chns_rm],
-        ] + [utils.num_and_pars(e, var_ph) for e in params[:-1].split(",")]
-
-        # load function dynamically
-        p, m = func.rsplit(".", 1)
-        met = getattr(import_module(p, package=__package__), m)
-        return met(*params)
+
+        # get module and function names
+        func_call = expr.strip().split("(")[0]
+        subpackage, func = func_call.rsplit(".", 1)
+        package = subpackage.split(".")[0]
+
+        # import function into current namespace
+        log.debug(f"importing module {subpackage}")
+        importlib.import_module(subpackage, package=__package__)
+
+        # declare imported package as globals (see eval() call later)
+        globs = {
+            package: importlib.import_module(package),
+        }
+
+        # lookup dictionary for variables used in function arguments (see eval() call later)
+        locs = {"datainfo": f, "tcm": tcm, "table_names": good_chns} | pars_dict
+
+        # evil eval() to avoid annoying args casting logic
+        call_str = f"{func_call}({full_args_str})"
+        log.debug(f"evaluating {call_str}")
+        log.debug(f"...globals={globs} and locals={locs}")
+        log.debug(f"...locals={locs}")
+
+        return eval(call_str, globs, locs)
 
     else:
+        # find parameters in evt file or in parameters
+        field_list = re.findall(
+            rf"({'|'.join(f._asdict().keys())}).([a-zA-Z_$][\w$]*)", expr
+        )
+
         # check if query is either on channel basis or evt basis (and not a mix)
-        qry_mask = qry
-        if qry is not None:
-            if f"{evt_group}." in qry and (
-                f"{hit_group}." in qry or f"{dsp_group}." in qry
-            ):
+        query_mask = query
+        if query is not None:
+            hit_tiers = [k for k in f._asdict() if k != "evt"]
+            if "evt." in query and (any([t in query for t in hit_tiers])):
                 raise ValueError(
-                    f"Query can't be a mix of {evt_group} tier and lower tiers."
+                    f"Query can't be a mix of {f.evt.group} tier and lower tiers."
                 )
 
             # if it is an evt query we can evaluate it directly here
-            if table and f"{evt_group}." in qry:
-                qry_mask = eval(qry.replace(f"{evt_group}.", ""), table)
-
-        # load TCM data to define an event
-        ids = store.read(f"/{tcm_group}/array_id", f_tcm)[0].view_as("np")
-        idx = store.read(f"/{tcm_group}/array_idx", f_tcm)[0].view_as("np")
-        cumulength = store.read(f"/{tcm_group}/cumulative_length", f_tcm)[0].view_as(
-            "np"
-        )
+            if table and "evt." in query:
+                query_mask = eval(query.replace("evt.", ""), table)
 
         # switch through modes
-        if table and (("keep_at_ch:" == mode[:11]) or ("keep_at_idx:" == mode[:12])):
-            if "keep_at_ch:" == mode[:11]:
-                ch_comp = table[mode[11:].replace(f"{evt_group}.", "")]
+        if table and (
+            mode.startswith("keep_at_ch:") or mode.startswith("keep_at_idx:")
+        ):
+            if mode.startswith("keep_at_ch:"):
+                ch_comp = table[mode[11:].replace("evt.", "")]
             else:
-                ch_comp = table[mode[12:].replace(f"{evt_group}.", "")]
+                ch_comp = table[mode[12:].replace("evt.", "")]
                 if isinstance(ch_comp, Array):
-                    ch_comp = Array(nda=ids[ch_comp.view_as("np")])
+                    ch_comp = Array(tcm.id[ch_comp.view_as("np")])
                 elif isinstance(ch_comp, VectorOfVectors):
                     ch_comp = ch_comp.view_as("ak")
                     ch_comp = VectorOfVectors(
-                        array=ak.unflatten(
-                            ids[ak.flatten(ch_comp)], ak.count(ch_comp, axis=-1)
+                        ak.unflatten(
+                            tcm.id[ak.flatten(ch_comp)], ak.count(ch_comp, axis=-1)
                         )
                     )
                 else:
                     raise NotImplementedError(
                         type(ch_comp)
                         + " not supported (only Array and VectorOfVectors are supported)"
                     )
 
             if isinstance(ch_comp, Array):
                 return aggregators.evaluate_at_channel(
-                    cumulength=cumulength,
-                    idx=idx,
-                    ids=ids,
-                    f_hit=f_hit,
-                    f_dsp=f_dsp,
-                    chns_rm=chns_rm,
+                    datainfo=datainfo,
+                    tcm=tcm,
+                    channels_skip=channels_skip,
                     expr=expr,
-                    exprl=exprl,
+                    field_list=field_list,
                     ch_comp=ch_comp,
-                    var_ph=var_ph,
-                    defv=defv,
-                    tcm_id_table_pattern=tcm_id_table_pattern,
-                    evt_group=evt_group,
-                    hit_group=hit_group,
-                    dsp_group=dsp_group,
+                    pars_dict=pars_dict,
+                    default_value=default_value,
                 )
-            elif isinstance(ch_comp, VectorOfVectors):
+
+            if isinstance(ch_comp, VectorOfVectors):
                 return aggregators.evaluate_at_channel_vov(
-                    cumulength=cumulength,
-                    idx=idx,
-                    ids=ids,
-                    f_hit=f_hit,
-                    f_dsp=f_dsp,
+                    datainfo=datainfo,
+                    tcm=tcm,
                     expr=expr,
-                    exprl=exprl,
+                    field_list=field_list,
                     ch_comp=ch_comp,
-                    chns_rm=chns_rm,
-                    var_ph=var_ph,
-                    defv=defv,
-                    tcm_id_table_pattern=tcm_id_table_pattern,
-                    evt_group=evt_group,
-                    hit_group=hit_group,
-                    dsp_group=dsp_group,
-                )
-            else:
-                raise NotImplementedError(
-                    type(ch_comp)
-                    + " not supported (only Array and VectorOfVectors are supported)"
+                    channels_skip=channels_skip,
+                    pars_dict=pars_dict,
+                    default_value=default_value,
                 )
-        elif "first_at:" in mode or "last_at:" in mode:
+
+            raise NotImplementedError(
+                "{type(ch_comp).__name__} not supported "
+                "(only Array and VectorOfVectors are supported)"
+            )
+
+        if "first_at:" in mode or "last_at:" in mode:
             sorter = tuple(
                 re.findall(
-                    rf"({evt_group}|{hit_group}|{dsp_group}).([a-zA-Z_$][\w$]*)",
+                    rf"({'|'.join(f._asdict().keys())}).([a-zA-Z_$][\w$]*)",
                     mode.split("first_at:")[-1],
                 )[0]
             )
             return aggregators.evaluate_to_first_or_last(
-                cumulength=cumulength,
-                idx=idx,
-                ids=ids,
-                f_hit=f_hit,
-                f_dsp=f_dsp,
-                chns=chns,
-                chns_rm=chns_rm,
+                datainfo=datainfo,
+                tcm=tcm,
+                channels=channels,
+                channels_skip=channels_skip,
                 expr=expr,
-                exprl=exprl,
-                qry=qry_mask,
-                nrows=nrows,
+                field_list=field_list,
+                query=query_mask,
+                n_rows=n_rows,
                 sorter=sorter,
-                var_ph=var_ph,
-                defv=defv,
+                pars_dict=pars_dict,
+                default_value=default_value,
                 is_first=True if "first_at:" in mode else False,
-                tcm_id_table_pattern=tcm_id_table_pattern,
-                evt_group=evt_group,
-                hit_group=hit_group,
-                dsp_group=dsp_group,
             )
-        elif mode in ["sum", "any", "all"]:
+
+        if mode in ["sum", "any", "all"]:
             return aggregators.evaluate_to_scalar(
+                datainfo=datainfo,
+                tcm=tcm,
                 mode=mode,
-                cumulength=cumulength,
-                idx=idx,
-                ids=ids,
-                f_hit=f_hit,
-                f_dsp=f_dsp,
-                chns=chns,
-                chns_rm=chns_rm,
+                channels=channels,
+                channels_skip=channels_skip,
                 expr=expr,
-                exprl=exprl,
-                qry=qry_mask,
-                nrows=nrows,
-                var_ph=var_ph,
-                defv=defv,
-                tcm_id_table_pattern=tcm_id_table_pattern,
-                evt_group=evt_group,
-                hit_group=hit_group,
-                dsp_group=dsp_group,
+                field_list=field_list,
+                query=query_mask,
+                n_rows=n_rows,
+                pars_dict=pars_dict,
+                default_value=default_value,
             )
-        elif "gather" == mode:
+        if mode == "gather":
             return aggregators.evaluate_to_vector(
-                cumulength=cumulength,
-                idx=idx,
-                ids=ids,
-                f_hit=f_hit,
-                f_dsp=f_dsp,
-                chns=chns,
-                chns_rm=chns_rm,
+                datainfo=datainfo,
+                tcm=tcm,
+                channels=channels,
+                channels_skip=channels_skip,
                 expr=expr,
-                exprl=exprl,
-                qry=qry_mask,
-                nrows=nrows,
-                var_ph=var_ph,
-                defv=defv,
+                field_list=field_list,
+                query=query_mask,
+                n_rows=n_rows,
+                pars_dict=pars_dict,
+                default_value=default_value,
                 sorter=sorter,
-                tcm_id_table_pattern=tcm_id_table_pattern,
-                evt_group=evt_group,
-                hit_group=hit_group,
-                dsp_group=dsp_group,
             )
-        else:
-            raise ValueError(mode + " not a valid mode")
+
+        raise ValueError(f"'{mode}' is not a valid mode")
```

### Comparing `pygama-1.6.0a2/src/pygama/evt/build_tcm.py` & `pygama-2.0.0a1/src/pygama/evt/build_tcm.py`

 * *Files identical despite different names*

### Comparing `pygama-1.6.0a2/src/pygama/evt/modules/legend.py` & `pygama-2.0.0a1/src/pygama/evt/modules/legend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Module provides LEGEND internal functions
 """
+
 from importlib import import_module
 
 from lgdo.lh5 import utils
 
 
 def metadata(params: dict) -> list:
     # only import legend meta data when needed.
```

### Comparing `pygama-1.6.0a2/src/pygama/evt/tcm.py` & `pygama-2.0.0a1/src/pygama/evt/tcm.py`

 * *Files identical despite different names*

### Comparing `pygama-1.6.0a2/src/pygama/flow/data_loader.py` & `pygama-2.0.0a1/src/pygama/flow/data_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import numpy as np
 import pandas as pd
 from dspeed.vis import WaveformBrowser
 from lgdo.lh5 import LH5Iterator, LH5Store
 from lgdo.lh5.utils import expand_vars
 from lgdo.types import Array, Struct, Table
-from lgdo.types.vectorofvectors import build_cl, explode_arrays, explode_cl
+from lgdo.types.vovutils import build_cl, explode_arrays, explode_cl
 from tqdm.auto import tqdm
 
 from . import utils
 from .file_db import FileDB
 
 log = logging.getLogger(__name__)
```

### Comparing `pygama-1.6.0a2/src/pygama/flow/file_db.py` & `pygama-2.0.0a1/src/pygama/flow/file_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for LH5 file inventory."""
+
 from __future__ import annotations
 
 import json
 import logging
 import os
 import re
 import string
```

### Comparing `pygama-1.6.0a2/src/pygama/flow/utils.py` & `pygama-2.0.0a1/src/pygama/flow/utils.py`

 * *Files identical despite different names*

### Comparing `pygama-1.6.0a2/src/pygama/hit/build_hit.py` & `pygama-2.0.0a1/src/pygama/hit/build_hit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
 This module implements routines to evaluate expressions to columnar data.
 """
+
 from __future__ import annotations
 
-import json
 import logging
 import os
 from collections import OrderedDict
 from typing import Iterable, Mapping
 
 import lgdo
 import numpy as np
 from lgdo.lh5 import LH5Iterator, LH5Store, ls
 
+from .. import utils
+
 log = logging.getLogger(__name__)
 
 
 def build_hit(
     infile: str,
     outfile: str = None,
     hit_config: str | Mapping = None,
@@ -91,28 +93,25 @@
             "lh5_tables_config and hit_config/lh5_tables options are mutually exclusive"
         )
 
     if lh5_tables_config is not None:
         tbl_cfg = lh5_tables_config
         # sanitize config
         if isinstance(tbl_cfg, str):
-            with open(tbl_cfg) as f:
-                tbl_cfg = json.load(f)
+            tbl_cfg = utils.load_dict(tbl_cfg)
 
         for k, v in tbl_cfg.items():
             if isinstance(v, str):
-                with open(v) as f:
-                    tbl_cfg[k] = json.load(f)
+                tbl_cfg[k] = utils.load_dict(v)
         lh5_tables_config = tbl_cfg
 
     else:
         if isinstance(hit_config, str):
             # sanitize config
-            with open(hit_config) as f:
-                hit_config = json.load(f)
+            hit_config = utils.load_dict(hit_config)
 
         if lh5_tables is None:
             lh5_tables_config = {}
             if "dsp" in ls(infile):
                 log.debug("found candidate table /dsp")
                 lh5_tables_config["dsp"] = hit_config
             for el in ls(infile):
@@ -150,14 +149,15 @@
             for outname, info in cfg["operations"].items():
                 outcol = outtbl_obj.eval(
                     info["expression"], info.get("parameters", None)
                 )
                 if "lgdo_attrs" in info:
                     outcol.attrs |= info["lgdo_attrs"]
 
+                log.debug(f"made new column {outname!r}={outcol!r}")
                 outtbl_obj.add_column(outname, outcol)
 
             # make high level flags
             if "aggregations" in cfg:
                 for high_lvl_flag, flags in cfg["aggregations"].items():
                     flags_list = list(flags.values())
                     n_flags = len(flags_list)
```

### Comparing `pygama-1.6.0a2/src/pygama/logging.py` & `pygama-2.0.0a1/src/pygama/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module implements some helpers for setting up logging."""
+
 import logging
 
 import colorlog
 
 DEBUG = logging.DEBUG
 INFO = logging.INFO
 WARNING = logging.WARNING
```

### Comparing `pygama-1.6.0a2/src/pygama/math/histogram.py` & `pygama-2.0.0a1/src/pygama/math/histogram.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,268 +10,423 @@
 variance = counts (Poisson stats)
 
 These are just convenience functions, provided for your convenience. Hopefully
 they will help you if you need to do something trickier than is provided (e.g.
 2D hists).
 """
 
+import logging
+from typing import Callable, Optional, Union
+
+import hist as bh
 import matplotlib.pyplot as plt
+import numba as nb
 import numpy as np
 from matplotlib import rcParams
-import logging
 
 import pygama.math.utils as pgu
 
 log = logging.getLogger(__name__)
 
 
-def get_hist(data, bins=None, range=None, dx=None, wts=None):
+def get_hist(
+    data: np.ndarray,
+    bins: Optional[Union[int, np.ndarray, str]] = None,
+    range: Optional[tuple[float, float]] = None,
+    dx: Optional[float] = None,
+    wts: Optional[Union[float, np.ndarray]] = None,
+) -> tuple[np.ndarray, ...]:
     """return hist, bins, var after binning data
 
-    This is just a wrapper for numpy.histogram, with optional weights for each
+    This is just a wrapper for humba.histogram, with optional weights for each
     element and proper computing of variances.
 
     Note: there are no overflow / underflow bins.
 
     Available binning methods:
 
       - Default (no binning arguments) : 100 bins over an auto-detected range
-      - bins=N, range=(x_lo, x_hi) : N bins over the specified range (or leave
+      - bins=n, range=(x_lo, x_hi) : n bins over the specified range (or leave
         range=None for auto-detected range)
       - bins=[str] : use one of np.histogram's automatic binning algorithms
       - bins=bin_edges_array : array lower bin edges, supports non-uniform binning
       - dx=dx, range=(x_lo, x_hi): bins of width dx over the specified range.
         Note: dx overrides the bins argument!
 
     Parameters
     ----------
-    data : array like
+    data
         The array of data to be histogrammed
-    bins : int, array, or str (optional)
+    bins
         int: the number of bins to be used in the histogram
         array: an array of bin edges to use
         str: the name of the np.histogram automatic binning algorithm to use
-        If not provided, np.histogram's default auto-binning routine is used
-    range : tuple (float, float) (optional)
+        If not provided, humba.histogram's default auto-binning routine is used
+    range
         (x_lo, x_high) is the tuple of low and high x values to uses for the
         very ends of the bin range. If not provided, np.histogram chooses the
         ends based on the data in data
-    dx : float (optional)
+    dx
         Specifies the bin width. Overrides "bins" if both arguments are present
-    wts : float or array like (optional)
+    wts
         Array of weights for each bin. For example, if you want to divide all
         bins by a time T to get the bin contents in count rate, set wts = 1/T.
         Variances will be computed for each bin that appropriately account for
         each data point's weighting.
 
     Returns
     -------
-    hist : array
+    hist
         the values in each bin of the histogram
-    bins : array
+    bins
         an array of bin edges: bins[i] is the lower edge of the ith bin.
         Note: it includes the upper edge of the last bin and does not
         include underflow or overflow bins. So len(bins) = len(hist) + 1
-    var : array
+    var
         array of variances in each bin of the histogram
     """
     if bins is None:
-        bins = 100 # override np.histogram default of just 10
+        bins = 100  # override boost_histogram.Histogram default of just 10
 
     if dx is not None:
         bins = int((range[1] - range[0]) / dx)
 
+    if range is None:
+        range = [np.amin(data), np.amax(data)]
+
     # bins includes left edge of first bin and right edge of all other bins
     # allow scalar weights
-    if wts is not None and np.shape(wts) == (): wts = np.full_like(data, wts)
-    hist, bins = np.histogram(data, bins=bins, range=range, weights=wts)
+    if wts is not None and np.shape(wts) == ():
+        wts = np.full_like(data, wts)
 
-    if wts is None:
-        # no weights: var = hist, but return a copy so that mods to var don't
-        # modify hist.
-        # Note: If you don't want a var copy, just call np.histogram()
-        return hist, bins, hist.copy()
+    # initialize the boost_histogram object
+    if isinstance(bins, int):
+        boost_histogram = bh.Hist(
+            bh.axis.Regular(bins=bins, start=range[0], stop=range[1]),
+            storage=bh.storage.Weight(),
+        )
     else:
-        # get the variances by binning with double the weight
-        var, bins = np.histogram(data, bins=bins, weights=wts*wts)
-        return hist, bins, var
+        # if bins are specified need to use variable
+        boost_histogram = bh.Hist(bh.axis.Variable(bins), storage=bh.storage.Weight())
+    # create the histogram
+    boost_histogram.fill(data, weight=wts)
+    # read out the histogram, bins, and variances
+    hist, bins = boost_histogram.to_numpy()
+    var = boost_histogram.variances()
+
+    return hist, bins, var
 
 
-def better_int_binning(x_lo=0, x_hi=None, dx=None, n_bins=None):
-    """ Get a good binning for integer data.
+def better_int_binning(
+    x_lo: float = 0, x_hi: float = None, dx: float = None, n_bins: float = None
+) -> tuple[int, int, int, int]:
+    """Get a good binning for integer data.
 
     Guarantees an integer bin width.
 
     At least two of x_hi, dx, or n_bins must be provided.
 
     Parameters
     ----------
-    x_lo : float
+    x_lo
         Desired low x value for the binning
-    x_hi : float
+    x_hi
         Desired high x value for the binning
-    dx : float
+    dx
         Desired bin width
-    n_bins : float
+    n_bins
         Desired number of bins
 
     Returns
     -------
-    x_lo: int
+    x_lo
         int values for best x_lo
-    x_hi: int
+    x_hi
         int values for best x_hi, returned if x_hi is not None
-    dx : int
+    dx
         best int bin width, returned if arg dx is not None
-    n_bins : int
+    n_bins
         best int n_bins, returned if arg n_bins is not None
     """
     # process inputs
-    n_Nones = int(x_hi is None) + int(dx is None) + int(n_bins is None)
-    if n_Nones > 1:
-        print('better_int_binning: must provide two of x_hi, dx or n_bins')
-        return
-    if n_Nones == 0:
-        print('better_int_binning: overconstrained. Ignoring x_hi.')
+    n_nones = int(x_hi is None) + int(dx is None) + int(n_bins is None)
+    if n_nones > 1:
+        raise ValueError("must provide two of x_hi, dx or n_bins")
+    if n_nones == 0:
+        log.warning("Overconstrained. Ignoring x_hi.")
         x_hi = None
 
     # get valid dx or n_bins
     if dx is not None:
         if dx <= 0:
-            print(f'better_int_binning: invalid dx={dx}')
-            return
+            raise ValueError(f"invalid dx={dx}")
         dx = np.round(dx)
-        if dx == 0: dx = 1
+        if dx == 0:
+            dx = 1
     if n_bins is not None:
         if n_bins <= 0:
-            print(f'better_int_binning: invalid n_bins={n_bins}')
-            return
+            raise ValueError(f"invalid n_bins={n_bins}")
         n_bins = np.round(n_bins)
 
     # can already return if no x_hi
-    if x_hi is None: # must have both dx and n_bins
+    if x_hi is None:  # must have both dx and n_bins
         return int(x_lo), int(dx), int(n_bins)
 
     # x_hi is valid. Get a valid dx if we don't have one
-    if dx is None: # must have n_bins
-        dx = np.round((x_hi-x_lo)/n_bins)
-    if dx == 0: dx = 1
+    if dx is None:  # must have n_bins
+        dx = np.round((x_hi - x_lo) / n_bins)
+    if dx == 0:
+        dx = 1
 
     # Finally, build a good binning from dx
-    n_bins = np.ceil((x_hi-x_lo)/dx)
+    n_bins = np.ceil((x_hi - x_lo) / dx)
     x_lo = np.floor(x_lo)
-    x_hi = x_lo + n_bins*dx
-    if n_bins is None: return int(x_lo), int(x_hi), int(dx)
-    else: return int(x_lo), int(x_hi), int(n_bins)
+    x_hi = x_lo + n_bins * dx
+    if n_bins is None:
+        return int(x_lo), int(x_hi), int(dx)
+    else:
+        return int(x_lo), int(x_hi), int(n_bins)
 
 
-def get_bin_centers(bins):
+@nb.njit(parallel=False, fastmath=True)
+def get_bin_centers(bins: np.ndarray) -> np.ndarray:
     """
     Returns an array of bin centers from an input array of bin edges.
     Works for non-uniform binning. Note: a new array is allocated
 
-    Parameters:
+    Parameters
+    ----------
+    bins
+        The input array of bin-edges
+
+    Returns
+    ----------
+    bin_centers
+        The array of bin centers
     """
-    return (bins[:-1] + bins[1:]) / 2.
+    return (bins[:-1] + bins[1:]) / 2.0
 
 
-def get_bin_widths(bins):
+@nb.njit(parallel=False, fastmath=True)
+def get_bin_widths(bins: np.ndarray) -> np.ndarray:
     """
     Returns an array of bin widths from an input array of bin edges.
     Works for non-uniform binning.
+
+    Parameters
+    ----------
+    bins
+        The input array of bin-edges
+
+    Returns
+    ----------
+    bin_widths
+        An array of bin widths
     """
-    return (bins[1:] - bins[:-1])
+    return bins[1:] - bins[:-1]
 
 
-def find_bin(x, bins):
+@nb.njit(parallel=False, fastmath=True)
+def find_bin(x: float, bins: np.ndarray) -> int:
     """
     Returns the index of the bin containing x
     Returns -1 for underflow, and len(bins) for overflow
     For uniform bins, jumps directly to the appropriate index.
     For non-uniform bins, binary search is used.
+
+    Parameters
+    ----------
+    x
+        The value to search for amongst the bins
+    bins
+        The input array of bin-edges
+
+    Returns
+    -------
+    bin_idx
+        Index of the bin containing x
+
+    TODO: replace np.searchsorted with for loops, numba will speed this function up then
     """
     # first handle overflow / underflow
-    if len(bins) == 0: return 0 # i.e. overflow
-    if x < bins[0]: return -1
-    if x > bins[-1]: return len(bins)
+    if len(bins) == 0:
+        return 0  # i.e. overflow
+    if x < bins[0]:
+        return -1
+    if x > bins[-1]:
+        return len(bins)
 
     # we are definitely in range, and there are at least 2 bin edges, one below
     # and one above x. try assuming uniform bins
-    dx = bins[1]-bins[0]
-    index = int(np.floor((x-bins[0])/dx))
-    if bins[index] <= x and bins[index+1] > x: return index
+    dx = bins[1] - bins[0]
+    index = int(np.floor((x - bins[0]) / dx))
+    if bins[index] <= x and bins[index + 1] > x:
+        return index
 
     # bins are non-uniform: find by binary search
-    return np.searchsorted(bins, x, side='right')
+    return np.searchsorted(bins, x, side="right")
+
+
+def range_slice(
+    x_min: float,
+    x_max: float,
+    hist: np.ndarray,
+    bins: np.ndarray,
+    var: Optional[np.ndarray] = None,
+) -> tuple[np.ndarray, ...]:
+    """
+    Get the histogram bins and values for a given slice of the range
 
+    Parameters
+    ----------
+    x_min
+        Lower endpoint of the range
+    x_min
+        Upper endpoint of the range
+    hist, bins, var
+        The histogrammed data to search through
 
-def range_slice(x_min, x_max, hist, bins, var=None):
+    See Also
+    --------
+    find_bin
+        for parameters and return values
+    """
     i_min = find_bin(x_min, bins)
     i_max = find_bin(x_max, bins)
-    if var is not None: var = var[i_min:i_max]
-    return hist[i_min:i_max], bins[i_min:i_max+1], var
+    if var is not None:
+        var = var[i_min:i_max]
+    return hist[i_min:i_max], bins[i_min : i_max + 1], var
+
+
+def get_fwhm(
+    hist: np.ndarray,
+    bins: np.ndarray,
+    var: Optional[np.ndarray] = None,
+    mx: Optional[Union[float, tuple[float, float]]] = None,
+    dmx: Optional[float] = 0,
+    bl: Optional[Union[float, tuple[float, float]]] = 0,
+    dbl: Optional[float] = 0,
+    method: str = "bins_over_f",
+    n_slope: int = 3,
+) -> tuple[float, float]:
+    """Convenience function for the FWHM of data in a histogram
 
+    Typically used by sending slices around a peak. Searches about argmax(hist)
+    for the peak to fall by [fraction] from mx to bl
+
+    Parameters
+    ----------
+    fraction
+        The fractional amplitude at which to evaluate the full width
+    hist
+        The histogram data array containing the peak
+    bins
+        An array of bin edges for the histogram
+    var
+        An array of histogram variances. Used with the 'fit_slopes' method
+    mx
+        The value to use for the max of the peak. If None, np.amax(hist) is
+        used.
+    dmx
+        The uncertainty in mx
+    bl
+        Used to specify an offset from which to estimate the FWFM.
+    dbl
+        The uncertainty in the bl
+    method
+        'bins_over_f' : the simplest method: just take the difference in the bin
+            centers that are over [fraction] of max. Only works for high stats and
+            FWFM/bin_width >> 1
+        'interpolate' : interpolate between the bins that cross the [fraction]
+            line.  Works well for high stats and a reasonable number of bins.
+            Uncertainty incorporates var, if provided.
+        'fit_slopes' : fit over n_slope bins in the vicinity of the FWFM and
+            interpolate to get the fractional crossing point. Works okay even
+            when stats are moderate but requires enough bins that dx traversed
+            by n_slope bins is approximately linear. Incorporates bin variances
+            in fit and final uncertainties if provided.
+    n_slope
+        Number of bins in the vicinity of the FWFM used to interpolate the fractional
+        crossing point with the 'fit_slopes' method
+
+    Returns
+    -------
+    fwhm, dfwhm
+        fwfm: the full width at half of the maximum above bl
+        dfwfm: the uncertainty in fwhm
 
-def get_fwhm(hist, bins, var=None, mx=None, dmx=0, bl=0, dbl=0, method='bins_over_f', n_slope=3):
-    """Estimate the FWHM of data in a histogram
 
     See Also
     --------
-    get_fwfm : for parameters and return values
+    get_fwfm
+        Function that computes the FWFM
     """
     if len(bins) == len(hist):
-        print("note: this function has been updated to require bins rather",
-              "than bin_centers. Don't trust this result")
+        log.warning(
+            "note: this function has been updated to require bins rather than bin_centers. Don't trust this result"
+        )
     return get_fwfm(0.5, hist, bins, var, mx, dmx, bl, dbl, method, n_slope)
 
 
-def get_fwfm(fraction, hist, bins, var=None, mx=None, dmx=0, bl=0, dbl=0, method='bins_over_f', n_slope=3):
+def get_fwfm(
+    fraction: float,
+    hist: np.ndarray,
+    bins: np.ndarray,
+    var: Optional[np.ndarray] = None,
+    mx: Optional[Union[float, tuple[float, float]]] = None,
+    dmx: Optional[float] = 0,
+    bl: Optional[Union[float, tuple[float, float]]] = 0,
+    dbl: Optional[float] = 0,
+    method: str = "bins_over_f",
+    n_slope: int = 3,
+) -> tuple[float, float]:
     """
     Estimate the full width at some fraction of the max of data in a histogram
 
     Typically used by sending slices around a peak. Searches about argmax(hist)
     for the peak to fall by [fraction] from mx to bl
 
     Parameters
     ----------
-    fraction : float
+    fraction
         The fractional amplitude at which to evaluate the full width
-    hist : array-like
+    hist
         The histogram data array containing the peak
-    bins : array-like
+    bins
         An array of bin edges for the histogram
-    var : array-like (optional)
+    var
         An array of histogram variances. Used with the 'fit_slopes' method
-    mx : float or tuple(float, float) (optional)
+    mx
         The value to use for the max of the peak. If None, np.amax(hist) is
         used.
-    dmx : float (optional)
+    dmx
         The uncertainty in mx
-    bl : float or tuple (float, float) (optional)
+    bl
         Used to specify an offset from which to estimate the FWFM.
-    dbl : float (optional)
+    dbl
         The uncertainty in the bl
-    method : string
+    method
         'bins_over_f' : the simplest method: just take the difference in the bin
             centers that are over [fraction] of max. Only works for high stats and
             FWFM/bin_width >> 1
-        'interpolate' : interpolate between the bins that cross the [fration]
+        'interpolate' : interpolate between the bins that cross the [fraction]
             line.  Works well for high stats and a reasonable number of bins.
             Uncertainty incorporates var, if provided.
         'fit_slopes' : fit over n_slope bins in the vicinity of the FWFM and
             interpolate to get the fractional crossing point. Works okay even
             when stats are moderate but requires enough bins that dx traversed
             by n_slope bins is approximately linear. Incorporates bin variances
             in fit and final uncertainties if provided.
-    n_slope : int
-        DOCME
+    n_slope
+        Number of bins in the vicinity of the FWFM used to interpolate the fractional
+        crossing point with the 'fit_slopes' method
 
     Returns
     -------
-    fwfm, dfwfm : float, float
+    fwfm, dfwfm
         fwfm: the full width at [fraction] of the maximum above bl
         dfwfm: the uncertainty in fwfm
 
     Examples
     --------
     >>> import pygama.analysis.histograms as pgh
     >>> from numpy.random import normal
@@ -281,186 +436,387 @@
 
     >>> pgh.get_fwfm(0.5, hist, bins, var, method='interpolate')
     (2.2041666666666666, 0.09790931254396479) # may vary
 
     >>> pgh.get_fwfm(0.5, hist, bins, var, method='fit_slopes')
     (2.3083363869003466, 0.10939486522749278) # may vary
     """
-
     # find bins over [fraction]
     if mx is None:
         mx = np.amax(hist)
         if var is not None and dmx == 0:
             dmx = np.sqrt(var[np.argmax(hist)])
-    idxs_over_f = hist > (bl + fraction * (mx-bl))
+    idxs_over_f = hist > (bl + fraction * (mx - bl))
 
     # argmax will return the index of the first occurrence of a maximum
     # so we can use it to find the first and last time idxs_over_f is "True"
     bin_lo = np.argmax(idxs_over_f)
     bin_hi = len(idxs_over_f) - np.argmax(idxs_over_f[::-1])
     bin_centers = get_bin_centers(bins)
 
     # precalc dheight: uncertainty in height used as the threshold
-    dheight2 = (fraction*dmx)**2 + ((1-fraction)*dbl)**2
+    dheight2 = (fraction * dmx) ** 2 + ((1 - fraction) * dbl) ** 2
 
-    if method == 'bins_over_f':
+    if method == "bins_over_f":
         # the simplest method: just take the difference in the bin centers
         fwfm = bin_centers[bin_hi] - bin_centers[bin_lo]
 
         # compute rough uncertainty as [bin width] (+) [dheight / slope]
-        dx = bin_centers[bin_lo] - bin_centers[bin_lo-1]
-        dy = hist[bin_lo] - hist[bin_lo-1]
-        if dy == 0: dy = (hist[bin_lo+1] - hist[bin_lo-2])/3
-        dfwfm2 = dx**2 + dheight2 * (dx/dy)**2
-        dx = bin_centers[bin_hi+1] - bin_centers[bin_hi]
-        dy = hist[bin_hi] - hist[bin_hi+1]
-        if dy == 0: dy = (hist[bin_hi-1] - hist[bin_hi+2])/3
-        dfwfm2 += dx**2 + dheight2 * (dx/dy)**2
+        dx = bin_centers[bin_lo] - bin_centers[bin_lo - 1]
+        dy = hist[bin_lo] - hist[bin_lo - 1]
+        if dy == 0:
+            dy = (hist[bin_lo + 1] - hist[bin_lo - 2]) / 3
+        dfwfm2 = dx**2 + dheight2 * (dx / dy) ** 2
+        dx = bin_centers[bin_hi + 1] - bin_centers[bin_hi]
+        dy = hist[bin_hi] - hist[bin_hi + 1]
+        if dy == 0:
+            dy = (hist[bin_hi - 1] - hist[bin_hi + 2]) / 3
+        dfwfm2 += dx**2 + dheight2 * (dx / dy) ** 2
         return fwfm, np.sqrt(dfwfm2)
 
-    elif method == 'interpolate':
+    elif method == "interpolate":
         # interpolate between the two bins that cross the [fraction] line
         # works well for high stats
-        if bin_lo < 1 or bin_hi >= len(hist)-1:
-            log.debug(f"get_fwhm: can't interpolate ({bin_lo}, {bin_hi})")
-            return 0, 0
+        if bin_lo < 1 or bin_hi >= len(hist) - 1:
+            raise ValueError(f"Can't interpolate ({bin_lo}, {bin_hi})")
 
-        val_f = bl + fraction*(mx-bl)
+        val_f = bl + fraction * (mx - bl)
 
         # x_lo
-        dx = bin_centers[bin_lo] - bin_centers[bin_lo-1]
-        dhf = val_f - hist[bin_lo-1]
-        dh = hist[bin_lo] - hist[bin_lo-1]
-        x_lo = bin_centers[bin_lo-1] + dx * dhf/dh
+        dx = bin_centers[bin_lo] - bin_centers[bin_lo - 1]
+        dhf = val_f - hist[bin_lo - 1]
+        dh = hist[bin_lo] - hist[bin_lo - 1]
+        x_lo = bin_centers[bin_lo - 1] + dx * dhf / dh
         # uncertainty
         dx2_lo = 0
         if var is not None:
-            dx2_lo = (dhf/dh)**2 * var[bin_lo] + ((dh-dhf)/dh)**2 * var[bin_lo-1]
-            dx2_lo *= (dx/dh)**2
-        dDdh = -dx/dh
+            dx2_lo = (dhf / dh) ** 2 * var[bin_lo] + ((dh - dhf) / dh) ** 2 * var[
+                bin_lo - 1
+            ]
+            dx2_lo *= (dx / dh) ** 2
+        dd_dh = -dx / dh
 
         # x_hi
-        dx = bin_centers[bin_hi+1] - bin_centers[bin_hi]
+        dx = bin_centers[bin_hi + 1] - bin_centers[bin_hi]
         dhf = hist[bin_hi] - val_f
-        dh = hist[bin_hi] - hist[bin_hi+1]
+        dh = hist[bin_hi] - hist[bin_hi + 1]
         if dh == 0:
-            raise ValueError(f"get_fwhm: interpolation failed, dh == 0")
-        x_hi = bin_centers[bin_hi] + dx * dhf/dh
+            raise ValueError("Interpolation failed, dh == 0")
+        x_hi = bin_centers[bin_hi] + dx * dhf / dh
         if x_hi < x_lo:
-            raise ValueError(f"get_fwfm: interpolation produced negative fwfm")
+            raise ValueError("Interpolation produced negative fwfm")
         # uncertainty
         dx2_hi = 0
         if var is not None:
-            dx2_hi = (dhf/dh)**2 * var[bin_hi+1] + ((dh-dhf)/dh)**2 * var[bin_hi]
-            dx2_hi *= (dx/dh)**2
-        dDdh += dx/dh
+            dx2_hi = (dhf / dh) ** 2 * var[bin_hi + 1] + ((dh - dhf) / dh) ** 2 * var[
+                bin_hi
+            ]
+            dx2_hi *= (dx / dh) ** 2
+        dd_dh += dx / dh
 
-        return x_hi - x_lo, np.sqrt(dx2_lo + dx2_hi + dDdh**2 * dheight2)
+        return x_hi - x_lo, np.sqrt(dx2_lo + dx2_hi + dd_dh**2 * dheight2)
 
-    elif method == 'fit_slopes':
+    elif method == "fit_slopes":
         # evaluate the [fraction] point on a line fit to n_slope bins near the crossing.
         # works okay even when stats are moderate
-        val_f = bl + fraction*(mx-bl)
+        val_f = bl + fraction * (mx - bl)
 
         # x_lo
-        i_0 = bin_lo - int(np.floor(n_slope/2))
+        i_0 = bin_lo - int(np.floor(n_slope / 2))
         if i_0 < 0:
-            log.debug(f"get_fwfm: fit slopes failed")
-            return 0, 0
+            raise RuntimeError("Fit slopes failed")
         i_n = i_0 + n_slope
-        wts = None if var is None else 1/np.sqrt(var[i_0:i_n]) #fails for any var = 0
+        wts = (
+            None if var is None else 1 / np.sqrt(var[i_0:i_n])
+        )  # fails for any var = 0
         wts = [w if w != np.inf else 0 for w in wts]
 
         try:
-            (m, b), cov = np.polyfit(bin_centers[i_0:i_n], hist[i_0:i_n], 1, w=wts, cov='unscaled')
+            (m, b), cov = np.polyfit(
+                bin_centers[i_0:i_n], hist[i_0:i_n], 1, w=wts, cov="unscaled"
+            )
         except np.linalg.LinAlgError:
-            log.debug(f"get_fwfm: LinAlgError")
-            return 0, 0
-        x_lo = (val_f-b)/m
-        #uncertainty
-        dxl2 = cov[0,0]/m**2 + (cov[1,1] + dheight2)/(val_f-b)**2 + 2*cov[0,1]/(val_f-b)/m
+            raise RuntimeError("LinAlgError in x_lo")
+        x_lo = (val_f - b) / m
+        # uncertainty
+        dxl2 = (
+            cov[0, 0] / m**2
+            + (cov[1, 1] + dheight2) / (val_f - b) ** 2
+            + 2 * cov[0, 1] / (val_f - b) / m
+        )
         dxl2 *= x_lo**2
 
         # x_hi
-        i_0 = bin_hi - int(np.floor(n_slope/2)) + 1
+        i_0 = bin_hi - int(np.floor(n_slope / 2)) + 1
         if i_0 == len(hist):
-            log.debug(f"get_fwfm: fit slopes failed")
-            return 0, 0
+            raise RuntimeError("Fit slopes failed")
 
         i_n = i_0 + n_slope
-        wts = None if var is None else 1/np.sqrt(var[i_0:i_n])
+        wts = None if var is None else 1 / np.sqrt(var[i_0:i_n])
         wts = [w if w != np.inf else 0 for w in wts]
         try:
-            (m, b), cov = np.polyfit(bin_centers[i_0:i_n], hist[i_0:i_n], 1, w=wts, cov='unscaled')
+            (m, b), cov = np.polyfit(
+                bin_centers[i_0:i_n], hist[i_0:i_n], 1, w=wts, cov="unscaled"
+            )
         except np.linalg.LinAlgError:
-            log.debug(f"get_fwfm: LinAlgError")
-            return 0, 0
-        x_hi = (val_f-b)/m
+            raise RuntimeError("LinAlgError in x_hi")
+        x_hi = (val_f - b) / m
         if x_hi < x_lo:
-            log.debug(f"get_fwfm: fit slopes produced negative fwfm")
-            return 0, 0
+            raise RuntimeError("Fit slopes produced negative fwfm")
 
-        #uncertainty
-        dxh2 = cov[0,0]/m**2 + (cov[1,1] + dheight2)/(val_f-b)**2 + 2*cov[0,1]/(val_f-b)/m
+        # uncertainty
+        dxh2 = (
+            cov[0, 0] / m**2
+            + (cov[1, 1] + dheight2) / (val_f - b) ** 2
+            + 2 * cov[0, 1] / (val_f - b) / m
+        )
         dxh2 *= x_hi**2
 
         return x_hi - x_lo, np.sqrt(dxl2 + dxh2)
 
     else:
-        log.debug(f"get_fwhm: unrecognized method {method}")
-        return 0, 0
+        raise NameError(f"Unrecognized method {method}")
 
 
-def plot_hist(hist, bins, var=None, show_stats=False, stats_hloc=0.75, stats_vloc=0.85, fill=False, fillcolor='r', fillalpha=0.2, **kwargs):
+def plot_hist(
+    hist: np.ndarray,
+    bins: np.ndarray,
+    var: Optional[np.ndarray] = None,
+    show_stats: bool = False,
+    stats_hloc: float = 0.75,
+    stats_vloc: float = 0.85,
+    fill: bool = False,
+    fillcolor: str = "r",
+    fillalpha: float = 0.2,
+    **kwargs,
+) -> None:
     """
-    plot a step histogram, with optional error bars
+    Plot a step histogram, with optional error bars
+
+    Parameters
+    ----------
+    hist
+        The histogram data array containing the peak
+    bins
+        An array of bin edges for the histogram
+    var
+        An array of histogram variances. Used with the 'fit_slopes' method
+    show_stats
+        If True, shows the mean, mean error, and standard deviation of the histogram on the plot
+    stats_hloc
+        matplotlib.pyplot horizontal location to place the stats
+    stats_vloc
+        matplotlib.pyplot vertical location to place the stats
+    fill
+        If True, fills in a step histogram when plotting
+    fill_color
+        Color to fill the step histogram if fill is True
+    fill_alpha
+        Alpha amount if fill is True
     """
     if fill:
         # the concat calls get the steps to draw correctly at the range boundaries
         # where="post" tells plt to draw the step y[i] between x[i] and x[i+1]
         save_color = None
-        if 'color' in kwargs: save_color = kwargs.pop('color')
-        elif 'c' in kwargs: save_color = kwargs.pop('c')
-        plt.fill_between(np.concatenate(([bins[0]], bins)), np.concatenate(([0], hist, [0])), step="post", color=fillcolor, alpha=fillalpha, **kwargs)
-        if save_color is not None: kwargs['color'] = save_color
+        if "color" in kwargs:
+            save_color = kwargs.pop("color")
+        elif "c" in kwargs:
+            save_color = kwargs.pop("c")
+        plt.fill_between(
+            np.concatenate(([bins[0]], bins)),
+            np.concatenate(([0], hist, [0])),
+            step="post",
+            color=fillcolor,
+            alpha=fillalpha,
+            **kwargs,
+        )
+        if save_color is not None:
+            kwargs["color"] = save_color
     if var is None:
         # the concat calls get the steps to draw correctly at the range boundaries
         # where="post" tells plt to draw the step y[i] between x[i] and x[i+1]
-        plt.step(np.concatenate(([bins[0]], bins)), np.concatenate(([0], hist, [0])), where="post", **kwargs)
+        plt.step(
+            np.concatenate(([bins[0]], bins)),
+            np.concatenate(([0], hist, [0])),
+            where="post",
+            **kwargs,
+        )
     else:
-        plt.errorbar(get_bin_centers(bins), hist,
-                     xerr=get_bin_widths(bins) / 2, yerr=np.sqrt(var),
-                     fmt='none', **kwargs)
+        plt.errorbar(
+            get_bin_centers(bins),
+            hist,
+            xerr=get_bin_widths(bins) / 2,
+            yerr=np.sqrt(var),
+            fmt="none",
+            **kwargs,
+        )
     if show_stats is True:
         bin_centers = get_bin_centers(bins)
-        N = np.sum(hist)
-        if N <= 1:
-            print("can't compute sigma for N =", N)
-            return
-        mean = np.sum(hist*bin_centers)/N
-        x2ave = np.sum(hist*bin_centers*bin_centers)/N
-        stddev = np.sqrt(N/(N-1) * (x2ave - mean*mean))
-        dmean = stddev/np.sqrt(N)
+        n = np.sum(hist)
+        if n <= 1:
+            raise RuntimeError(f"can't compute sigma for n = {n}")
+        mean = np.sum(hist * bin_centers) / n
+        x2ave = np.sum(hist * bin_centers * bin_centers) / n
+        stddev = np.sqrt(n / (n - 1) * (x2ave - mean * mean))
+        dmean = stddev / np.sqrt(n)
 
         mean, dmean = pgu.get_formatted_stats(mean, dmean, 2)
-        stats = f'$\\mu={mean} \\pm {dmean}$\n$\\sigma={stddev:#.3g}$'
-        stats_fontsize = rcParams['legend.fontsize']
-        plt.text(stats_hloc, stats_vloc, stats, transform=plt.gca().transAxes, fontsize = stats_fontsize)
+        stats = f"$\\mu={mean} \\pm {dmean}$\n$\\sigma={stddev:#.3g}$"
+        stats_fontsize = rcParams["legend.fontsize"]
+        plt.text(
+            stats_hloc,
+            stats_vloc,
+            stats,
+            transform=plt.gca().transAxes,
+            fontsize=stats_fontsize,
+        )
 
 
-def get_gaussian_guess(hist, bins):
+def get_gaussian_guess(
+    hist: np.ndarray, bins: np.ndarray
+) -> tuple[float, float, float]:
     """
     given a hist, gives guesses for mu, sigma, and amplitude
+
+    Parameters
+    ----------
+    hist
+        Array of histogrammed data
+    bins
+        Array of histogram bins
+
+    Returns
+    -------
+    guess_mu
+        guess for the mu parameter of a Gaussian
+    guess_sigma
+        guess for the sigma parameter of a Gaussian
+    guess_area
+        guess for the A parameter of a Gaussian
     """
     if len(bins) == len(hist):
-        print("note: this function has been updated to require bins rather",
-              "than bin_centers. Don't trust this result")
+        log.warning(
+            "note: this function has been updated to require bins rather than bin_centers. Don't trust this result"
+        )
 
     max_idx = np.argmax(hist)
-    guess_e = (bins[max_idx] + bins[max_idx])/2 # bin center
+    guess_mu = (bins[max_idx] + bins[max_idx]) / 2  # bin center
     guess_amp = hist[max_idx]
 
     # find 50% amp bounds on both sides for a FWHM guess
     guess_sigma = get_fwhm(hist, bins)[0] / 2.355  # FWHM to sigma
     guess_area = guess_amp * guess_sigma * np.sqrt(2 * np.pi)
 
-    return (guess_e, guess_sigma, guess_area)
+    return (guess_mu, guess_sigma, guess_area)
+
+
+def get_bin_estimates(
+    pars: np.ndarray,
+    func: Callable,
+    bins: np.ndarray,
+    is_integral: bool = False,
+    **kwargs,
+) -> np.ndarray:
+    """
+    Bin expected means are estimated by f(bin_center)*bin_width. Supply an
+    integrating function to compute the integral over the bin instead.
+    TODO: make default integrating function a numerical method that is off by
+    default.
+
+    Parameters
+    ----------
+    pars
+        The parameters of the function, func
+    func
+        The function at which to evaluate the bin centers
+    bins
+        Array of histogram bins
+    is_integral
+        if True, then func is an integral function
+
+    Returns
+    -------
+    f(bin_center)*bin_width
+        The expected mean of a bin
+
+    See Also
+    --------
+    get_bin_widths
+        Returns the width of the bins
+    get_bin_centers
+        Finds the bin centers of the supplied bins
+    """
+    if is_integral is False:
+        return func(get_bin_centers(bins), *pars, **kwargs) * get_bin_widths(bins)
+    else:
+        # func can be an integral functions
+        return func(bins[1:], *pars, **kwargs) - func(bins[:-1], *pars, **kwargs)
+
+
+def get_i_local_extrema(data, delta):
+    """Get lists of indices of the local maxima and minima of data
+
+    The "local" extrema are those maxima / minima that have heights / depths of
+    at least delta.
+    Converted from MATLAB script at: http://billauer.co.il/peakdet.html
+
+    Parameters
+    ----------
+    data : array-like
+        the array of data within which extrema will be found
+    delta : scalar
+        the absolute level by which data must vary (in one direction) about an
+        extremum in order for it to be tagged
+
+    Returns
+    -------
+    imaxes, imins : 2-tuple ( array, array )
+        A 2-tuple containing arrays of variable length that hold the indices of
+        the identified local maxima (first tuple element) and minima (second
+        tuple element)
+    """
+
+    # prepare output
+    imaxes, imins = [], []
+
+    # sanity checks
+    data = np.asarray(data)
+    if not np.isscalar(delta):
+        log.error("get_i_local_extrema: Input argument delta must be a scalar")
+        return np.array(imaxes), np.array(imins)
+    if delta <= 0:
+        log.error(f"get_i_local_extrema: delta ({delta}) must be positive")
+        return np.array(imaxes), np.array(imins)
+
+    # now loop over data
+    imax, imin = 0, 0
+    find_max = True
+    for i in range(len(data)):
+        if data[i] > data[imax]:
+            imax = i
+        if data[i] < data[imin]:
+            imin = i
+
+        if find_max:
+            # if the sample is less than the current max by more than delta,
+            # declare the previous one a maximum, then set this as the new "min"
+            if data[i] < data[imax] - delta:
+                imaxes.append(imax)
+                imin = i
+                find_max = False
+        else:
+            # if the sample is more than the current min by more than delta,
+            # declare the previous one a minimum, then set this as the new "max"
+            if data[i] > data[imin] + delta:
+                imins.append(imin)
+                imax = i
+                find_max = True
+
+    return np.array(imaxes), np.array(imins)
+
+
+def get_i_local_maxima(data, delta):
+    return get_i_local_extrema(data, delta)[0]
+
+
+def get_i_local_minima(data, delta):
+    return get_i_local_extrema(data, delta)[1]
```

### Comparing `pygama-1.6.0a2/src/pygama/pargen/AoE_cal.py` & `pygama-2.0.0a1/src/pygama/pargen/AoE_cal.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,844 +1,392 @@
 """
 This module provides functions for correcting the a/e energy dependence, determining the cut level and calculating survival fractions.
 """
 
 from __future__ import annotations
 
-import json
 import logging
-import os
-import pathlib
 import re
 from datetime import datetime
 from typing import Callable
 
-import matplotlib as mpl
-
-mpl.use("agg")
-import lgdo.lh5 as lh5
-import matplotlib.cm as cmx
-import matplotlib.colors as mcolors
 import matplotlib.dates as mdates
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-from iminuit import Minuit, cost, util
-from matplotlib.backends.backend_pdf import PdfPages
+from iminuit import Minuit, cost
 from matplotlib.colors import LogNorm
 from scipy.stats import chi2
 
+import pygama.math.binned_fitting as pgf
 import pygama.math.histogram as pgh
-import pygama.math.peak_fitting as pgf
-from pygama.math.peak_fitting import nb_erfc
-from pygama.pargen.energy_cal import get_i_local_maxima
-from pygama.pargen.utils import *
+import pygama.pargen.energy_cal as pgc
+from pygama.math.distributions import (
+    exgauss,
+    gauss_on_exgauss,
+    gauss_on_step,
+    gaussian,
+    hpge_peak,
+    nb_erfc,
+)
+from pygama.math.functions.hpge_peak import hpge_get_fwfm, hpge_get_fwhm, hpge_get_mode
+from pygama.math.functions.sum_dists import SumDists
+from pygama.pargen.utils import convert_to_minuit, return_nans
 
 log = logging.getLogger(__name__)
 
+(x_lo, x_hi, n_sig, mu, sigma, n_bkg, tau) = range(7)
+par_array = [(gaussian, [mu, sigma]), (exgauss, [mu, sigma, tau])]
+aoe_peak = SumDists(
+    par_array,
+    [n_sig, n_bkg],
+    "areas",
+    parameter_names=["x_lo", "x_hi", "n_sig", "mu", "sigma", "n_bkg", "tau"],
+    name="aoe_peak",
+)
+
+
+(x_lo, x_hi, n_sig, mu, sigma, frac1, tau, n_bkg, tau_bkg) = range(9)
+par_array = [
+    (gauss_on_exgauss, [mu, sigma, frac1, tau]),
+    (exgauss, [mu, sigma, tau_bkg]),
+]
+aoe_peak_with_high_tail = SumDists(
+    par_array,
+    [n_sig, n_bkg],
+    "areas",
+    parameter_names=[
+        "x_lo",
+        "x_hi",
+        "n_sig",
+        "mu",
+        "sigma",
+        "htail",
+        "tau_sig",
+        "n_bkg",
+        "tau",
+    ],
+    name="aoe_peak_with_high_tail",
+)
+aoe_peak_with_high_tail.get_fwfm = hpge_get_fwfm.__get__(aoe_peak_with_high_tail)
+aoe_peak_with_high_tail.get_mode = hpge_get_mode.__get__(aoe_peak_with_high_tail)
+aoe_peak_with_high_tail.get_fwhm = hpge_get_fwhm.__get__(aoe_peak_with_high_tail)
 
-class PDF:
-
-    """
-    Base class for A/E pdfs.
-    """
 
-    def pdf(x):
-        return
+def aoe_peak_guess(func, hist, bins, var, **kwargs):
+    bin_centers = (bins[:-1] + bins[1:]) / 2
 
-    def _replace_values(dic, **kwargs):
-        for item, value in kwargs.items():
-            dic[item] = value
-        return dic
-
-
-class standard_aoe(PDF):
-    def pdf(
-        x: np.array,
-        n_sig: float,
-        mu: float,
-        sigma: float,
-        n_bkg: float,
-        tau_bkg: float,
-        lower_range: float = np.inf,
-        upper_range: float = np.inf,
-        components: bool = False,
-    ) -> np.array:
-        """
-        PDF for A/E consists of a gaussian signal with gaussian tail background
-        """
-        try:
-            sig = n_sig * pgf.gauss_norm(x, mu, sigma)
-            bkg = n_bkg * pgf.gauss_tail_norm(
-                x, mu, sigma, tau_bkg, lower_range, upper_range
-            )
-        except:
-            sig = np.full_like(x, np.nan)
-            bkg = np.full_like(x, np.nan)
-
-        if components == False:
-            return sig + bkg
-        else:
-            return sig, bkg
-
-    def extended_pdf(
-        x: np.array,
-        n_sig: float,
-        mu: float,
-        sigma: float,
-        n_bkg: float,
-        tau_bkg: float,
-        lower_range: float = np.inf,
-        upper_range: float = np.inf,
-        components: bool = False,
-    ) -> tuple(float, np.array):
-        """
-        Extended PDF for A/E consists of a gaussian signal with gaussian tail background
-        """
-        if components == True:
-            sig, bkg = standard_aoe.pdf(
-                x,
-                n_sig,
-                mu,
-                sigma,
-                n_bkg,
-                tau_bkg,
-                lower_range,
-                upper_range,
-                components,
-            )
-            return n_sig + n_bkg, sig, bkg
-        else:
-            return n_sig + n_bkg, standard_aoe.pdf(
-                x,
-                n_sig,
-                mu,
-                sigma,
-                n_bkg,
-                tau_bkg,
-                lower_range,
-                upper_range,
-                components,
-            )
-
-    def guess(hist, bins, var, **kwargs):
-        bin_centers = (bins[:-1] + bins[1:]) / 2
-
-        mu = bin_centers[np.argmax(hist)]
-        try:
-            _, sigma, _ = pgh.get_gaussian_guess(hist, bins)
-        except:
-            pars, cov = pgf.gauss_mode_width_max(
-                hist, bins, var, mode_guess=mu, n_bins=20
-            )
-            _, sigma, _ = pars
-        ls_guess = 2 * np.sum(
-            hist[(bin_centers > mu) & (bin_centers < (mu + 2.5 * sigma))]
-        )
+    mu = bin_centers[np.argmax(hist)]
+    try:
+        _, sigma, _ = pgh.get_gaussian_guess(hist, bins)
+    except Exception:
+        pars, cov = pgf.gauss_mode_width_max(hist, bins, var, mode_guess=mu, n_bins=20)
+        _, sigma, _ = pars
+    ls_guess = 2 * np.sum(hist[(bin_centers > mu) & (bin_centers < (mu + 2.5 * sigma))])
 
+    if func == aoe_peak:
         guess_dict = {
+            "x_lo": bins[0],
+            "x_hi": bins[-1],
             "n_sig": ls_guess,
             "mu": mu,
             "sigma": sigma,
             "n_bkg": np.sum(hist) - ls_guess,
-            "tau_bkg": 0.1,
-            "lower_range": np.nanmin(bins),
-            "upper_range": np.nanmax(bins),
-            "components": 0,
+            "tau": 0.1,
         }
         for key, guess in guess_dict.items():
             if np.isnan(guess):
                 guess_dict[key] = 0
 
-        return standard_aoe._replace_values(guess_dict, **kwargs)
-
-    def bounds(guess, **kwargs):
-        bounds_dict = {
-            "n_sig": (0, None),
-            "mu": (None, None),
-            "sigma": (0, None),
-            "n_bkg": (0, None),
-            "tau_bkg": (0, None),
-            "lower_range": (None, None),
-            "upper_range": (None, None),
-            "components": (None, None),
-        }
-
-        return [
-            bound
-            for field, bound in standard_aoe._replace_values(
-                bounds_dict, **kwargs
-            ).items()
-        ]
-
-    def fixed(**kwargs):
-        fixed_dict = {
-            "n_sig": False,
-            "mu": False,
-            "sigma": False,
-            "n_bkg": False,
-            "tau_bkg": False,
-            "lower_range": True,
-            "upper_range": True,
-            "components": True,
-        }
-
-        return [
-            fixed
-            for field, fixed in standard_aoe._replace_values(
-                fixed_dict, **kwargs
-            ).items()
-        ]
-
-    def width(pars, errs, cov):
-        return pars["sigma"], errs["sigma"]
-
-    def centroid(pars, errs, cov):
-        return pars["mu"], errs["mu"]
-
-
-class standard_aoe_with_high_tail(PDF):
-    def pdf(
-        x: np.array,
-        n_sig: float,
-        mu: float,
-        sigma: float,
-        htail: float,
-        tau_sig: float,
-        n_bkg: float,
-        tau_bkg: float,
-        lower_range: float = np.inf,
-        upper_range: float = np.inf,
-        components: bool = False,
-    ) -> np.array:
-        """
-        PDF for A/E consists of a gaussian signal with tail with gaussian tail background
-        """
-        try:
-            sig = n_sig * (
-                (1 - htail) * pgf.gauss_norm(x, mu, sigma)
-                + htail
-                * pgf.gauss_tail_norm(x, mu, sigma, tau_sig, lower_range, upper_range)
-            )
-            bkg = n_bkg * pgf.gauss_tail_norm(
-                x, mu, sigma, tau_bkg, lower_range, upper_range
-            )
-        except:
-            sig = np.full_like(x, np.nan)
-            bkg = np.full_like(x, np.nan)
-
-        if components == False:
-            return sig + bkg
-        else:
-            return sig, bkg
-
-    def extended_pdf(
-        x: np.array,
-        n_sig: float,
-        mu: float,
-        sigma: float,
-        htail: float,
-        tau_sig: float,
-        n_bkg: float,
-        tau_bkg: float,
-        lower_range: float = np.inf,
-        upper_range: float = np.inf,
-        components: bool = False,
-    ) -> tuple(float, np.array):
-        """
-        Extended PDF for A/E consists of a gaussian signal with gaussian tail background
-        """
-        if components == True:
-            sig, bkg = standard_aoe_with_high_tail.pdf(
-                x,
-                n_sig,
-                mu,
-                sigma,
-                htail,
-                tau_sig,
-                n_bkg,
-                tau_bkg,
-                lower_range,
-                upper_range,
-                components,
-            )
-            return n_sig + n_bkg, sig, bkg
-        else:
-            return n_sig + n_bkg, standard_aoe_with_high_tail.pdf(
-                x,
-                n_sig,
-                mu,
-                sigma,
-                htail,
-                tau_sig,
-                n_bkg,
-                tau_bkg,
-                lower_range,
-                upper_range,
-                components,
-            )
-
-    def guess(hist, bins, var, **kwargs):
-        bin_centers = (bins[:-1] + bins[1:]) / 2
-        mu = bin_centers[np.argmax(hist)]
-        try:
-            _, sigma, _ = pgh.get_gaussian_guess(hist, bins)
-        except:
-            pars, cov = pgf.gauss_mode_width_max(
-                hist, bins, var, mode_guess=mu, n_bins=20
-            )
-            _, sigma, _ = pars
-        ls_guess = 2 * np.sum(
-            hist[(bin_centers > mu) & (bin_centers < (mu + 2.5 * sigma))]
-        )
-
+    elif func == aoe_peak_with_high_tail:
         guess_dict = {
+            "x_lo": bins[0],
+            "x_hi": bins[-1],
             "n_sig": ls_guess,
             "mu": mu,
             "sigma": sigma,
             "htail": 0.1,
             "tau_sig": -0.1,
             "n_bkg": np.sum(hist) - ls_guess,
-            "tau_bkg": 0.1,
-            "lower_range": np.nanmin(bins),
-            "upper_range": np.nanmax(bins),
-            "components": 0,
+            "tau": 0.1,
         }
         for key, guess in guess_dict.items():
             if np.isnan(guess):
                 guess_dict[key] = 0
 
-        return standard_aoe_with_high_tail._replace_values(guess_dict, **kwargs)
-
-    def bounds(guess, **kwargs):
-        bounds_dict = {
-            "n_sig": (0, None),
-            "mu": (None, None),
-            "sigma": (0, None),
-            "htail": (0, 1),
-            "tau_sig": (None, 0),
-            "n_bkg": (0, None),
-            "tau_bkg": (0, None),
-            "lower_range": (None, None),
-            "upper_range": (None, None),
-            "components": (None, None),
-        }
-
-        return [
-            bound
-            for field, bound in standard_aoe_with_high_tail._replace_values(
-                bounds_dict, **kwargs
-            ).items()
-        ]
-
-    def fixed(**kwargs):
-        fixed_dict = {
-            "n_sig": False,
-            "mu": False,
-            "sigma": False,
-            "htail": False,
-            "tau_sig": False,
-            "n_bkg": False,
-            "tau_bkg": False,
-            "lower_range": True,
-            "upper_range": True,
-            "components": True,
-        }
-
-        return [
-            fixed
-            for field, fixed in standard_aoe_with_high_tail._replace_values(
-                fixed_dict, **kwargs
-            ).items()
-        ]
-
-    def width(pars, errs, cov):
-        fwhm, fwhm_err = pgf.radford_fwhm(
-            pars[2], pars[3], np.abs(pars[4]), cov=cov[:7, :7]
-        )
-        return fwhm / 2.355, fwhm_err / 2.355
-
-    def centroid(pars, errs, cov):
-        return pars["mu"], errs["mu"]
-
-
-class standard_aoe_bkg(PDF):
-    def pdf(
-        x: np.array,
-        n_events: float,
-        mu: float,
-        sigma: float,
-        tau_bkg: float,
-        lower_range: float = np.inf,
-        upper_range: float = np.inf,
-    ) -> np.array:
-        """
-        PDF for A/E consists of a gaussian signal with tail with gaussian tail background
-        """
-        try:
-            sig = n_events * pgf.gauss_tail_norm(
-                x, mu, sigma, tau_bkg, lower_range, upper_range
-            )
-        except:
-            sig = np.full_like(x, np.nan)
-
-        return sig
-
-    def extended_pdf(
-        x: np.array,
-        n_events: float,
-        mu: float,
-        sigma: float,
-        tau_bkg: float,
-        lower_range: float = np.inf,
-        upper_range: float = np.inf,
-    ) -> tuple(float, np.array):
-        """
-        Extended PDF for A/E consists of a gaussian signal with gaussian tail background
-        """
-        return n_events, standard_aoe_bkg.pdf(
-            x, n_events, mu, sigma, tau_bkg, lower_range, upper_range
-        )
-
-    def guess(hist, bins, var, **kwargs):
-        bin_centers = (bins[:-1] + bins[1:]) / 2
-
-        mu = bin_centers[np.argmax(hist)]
-        try:
-            _, sigma, _ = pgh.get_gaussian_guess(hist, bins)
-        except:
-            pars, cov = pgf.gauss_mode_width_max(
-                hist, bins, var, mode_guess=mu, n_bins=20
-            )
-            _, sigma, _ = pars
-        ls_guess = 2 * np.sum(
-            hist[(bin_centers > mu) & (bin_centers < (mu + 2.5 * sigma))]
-        )
-
+    elif func == exgauss:
         guess_dict = {
-            "n_events": np.sum(hist) - ls_guess,
+            "x_lo": bins[0],
+            "x_hi": bins[-1],
+            "area": np.sum(hist) - ls_guess,
             "mu": mu,
             "sigma": sigma,
-            "tau_bkg": 0.1,
-            "lower_range": np.nanmin(bins),
-            "upper_range": np.nanmax(bins),
+            "tau": 0.1,
         }
         for key, guess in guess_dict.items():
             if np.isnan(guess):
                 guess_dict[key] = 0
 
-        return standard_aoe_bkg._replace_values(guess_dict, **kwargs)
-
-    def bounds(guess, **kwargs):
-        bounds_dict = {
-            "n_events": (0, None),
-            "mu": (None, None),
-            "sigma": (0, None),
-            "tau_bkg": (0, None),
-            "lower_range": (None, None),
-            "upper_range": (None, None),
-        }
-
-        return [
-            bound
-            for field, bound in standard_aoe_bkg._replace_values(
-                bounds_dict, **kwargs
-            ).items()
-        ]
-
-    def fixed(**kwargs):
-        fixed_dict = {
-            "n_bkg": False,
-            "mu": False,
-            "sigma": False,
-            "tau_bkg": False,
-            "lower_range": True,
-            "upper_range": True,
+    elif func == gaussian:
+        guess_dict = {
+            "x_lo": bins[0],
+            "x_hi": bins[-1],
+            "area": ls_guess,
+            "mu": mu,
+            "sigma": sigma,
         }
-
-        return [
-            fixed
-            for field, fixed in standard_aoe_bkg._replace_values(
-                fixed_dict, **kwargs
-            ).items()
-        ]
-
-
-class gaussian(PDF):
-    def pdf(x: np.array, n_events: float, mu: float, sigma: float) -> np.array:
-        """
-        PDF for A/E consists of a gaussian signal with tail with gaussian tail background
-        """
-        try:
-            sig = n_events * pgf.gauss_norm(x, mu, sigma)
-        except:
-            sig = np.full_like(x, np.nan)
-
-        return sig
-
-    def extended_pdf(
-        x: np.array, n_events: float, mu: float, sigma: float
-    ) -> tuple(float, np.array):
-        """
-        Extended PDF for A/E consists of a gaussian signal with gaussian tail background
-        """
-        return n_events, gaussian.pdf(x, n_events, mu, sigma)
-
-    def guess(hist, bins, var, **kwargs):
-        bin_centers = (bins[:-1] + bins[1:]) / 2
-        mu = bin_centers[np.argmax(hist)]
-        try:
-            _, sigma, _ = pgh.get_gaussian_guess(hist, bins)
-        except:
-            pars, cov = pgf.gauss_mode_width_max(
-                hist, bins, var, mode_guess=mu, n_bins=20
-            )
-            _, sigma, _ = pars
-        ls_guess = 2 * np.sum(
-            hist[(bin_centers > mu) & (bin_centers < (mu + 2.5 * sigma))]
-        )
-
-        guess_dict = {"n_events": ls_guess, "mu": mu, "sigma": sigma}
         for key, guess in guess_dict.items():
             if np.isnan(guess):
                 guess_dict[key] = 0
 
-        return gaussian._replace_values(guess_dict, **kwargs)
+    for item, value in kwargs.items():
+        guess_dict[item] = value
 
-    def bounds(gpars, **kwargs):
-        bounds_dict = {"n_events": (0, None), "mu": (None, None), "sigma": (0, None)}
+    return convert_to_minuit(guess_dict, func).values
 
-        return [
-            bound
-            for field, bound in gaussian._replace_values(bounds_dict, **kwargs).items()
-        ]
 
-    def fixed(**kwargs):
-        fixed_dict = {
-            "n_events": False,
-            "mu": False,
-            "sigma": False,
+def aoe_peak_bounds(func, guess, **kwargs):
+    if func == aoe_peak:
+        bounds_dict = {
+            "x_lo": (None, None),
+            "x_hi": (None, None),
+            "n_sig": (0, None),
+            "mu": (guess["x_lo"], guess["x_hi"]),
+            "sigma": (0, None),
+            "n_bkg": (0, None),
+            "tau": (0, None),
         }
-
-        return [
-            fixed
-            for field, fixed in gaussian._replace_values(fixed_dict, **kwargs).items()
-        ]
-
-
-class drift_time_distribution(PDF):
-    def pdf(
-        x,
-        n_sig1,
-        mu1,
-        sigma1,
-        htail1,
-        tau1,
-        n_sig2,
-        mu2,
-        sigma2,
-        htail2,
-        tau2,
-        components,
-    ):
-        gauss1 = n_sig1 * pgf.gauss_with_tail_pdf(x, mu1, sigma1, htail1, tau1)
-        gauss2 = n_sig2 * pgf.gauss_with_tail_pdf(x, mu2, sigma2, tau2, htail2)
-        if components is True:
-            return gauss1, gauss2
-        else:
-            return gauss1 + gauss2
-
-    def extended_pdf(
-        x,
-        n_sig1,
-        mu1,
-        sigma1,
-        htail1,
-        tau1,
-        n_sig2,
-        mu2,
-        sigma2,
-        htail2,
-        tau2,
-        components,
-    ):
-        if components is True:
-            gauss1, gauss2 = drift_time_distribution.pdf(
-                x,
-                n_sig1,
-                mu1,
-                sigma1,
-                htail1,
-                tau1,
-                n_sig2,
-                mu2,
-                sigma2,
-                htail2,
-                tau2,
-                components,
-            )
-            return n_sig1 + n_sig2, gauss1, gauss2
-
-        else:
-            return n_sig1 + n_sig2, drift_time_distribution.pdf(
-                x,
-                n_sig1,
-                mu1,
-                sigma1,
-                htail1,
-                tau1,
-                n_sig2,
-                mu2,
-                sigma2,
-                htail2,
-                tau2,
-                components,
-            )
-
-    def guess(hist: np.array, bins: np.array, var: np.array, **kwargs) -> list:
-        """
-        Guess for fitting dt spectrum
-        """
-        bcs = pgh.get_bin_centers(bins)
-        mus = get_i_local_maxima(hist / (np.sqrt(var) + 10**-99), 5)
-        if len(mus) > 2:
-            mus = get_i_local_maxima(hist / (np.sqrt(var) + 10**-99), 8)
-        elif len(mus) < 2:
-            mus = get_i_local_maxima(hist / (np.sqrt(var) + 10**-99), 3)
-        mu1 = bcs[mus[0]]
-        mu2 = bcs[mus[-1]]
-
-        pars, cov = pgf.gauss_mode_width_max(
-            hist,
-            bins,
-            var=None,
-            mode_guess=mu1,
-            n_bins=10,
-            cost_func="Least Squares",
-            inflate_errors=False,
-            gof_method="var",
-        )
-        mu1, sigma1, amp = pars
-        ix = np.where(bcs < mu1 + 3 * sigma1)[0][-1]
-        n_sig1 = np.sum(hist[:ix])
-        pars2, cov2 = pgf.gauss_mode_width_max(
-            hist,
-            bins,
-            var=None,
-            mode_guess=mu2,
-            n_bins=10,
-            cost_func="Least Squares",
-            inflate_errors=False,
-            gof_method="var",
-        )
-        mu2, sigma2, amp2 = pars2
-
-        guess_dict = {
-            "n_sig1": n_sig1,
-            "mu1": mu1,
-            "sigma1": sigma1,
-            "htail1": 0.5,
-            "tau1": 0.1,
-            "n_sig2": np.sum(hist) - n_sig1,
-            "mu2": mu2,
-            "sigma2": sigma2,
-            "htail2": 0.5,
-            "tau2": 0.1,
-            "components": 0,
+    elif func == aoe_peak_with_high_tail:
+        bounds_dict = {
+            "x_lo": (None, None),
+            "x_hi": (None, None),
+            "n_sig": (0, None),
+            "mu": (guess["x_lo"], guess["x_hi"]),
+            "sigma": (0, None),
+            "htail": (0, 1),
+            "tau_sig": (None, 0),
+            "n_bkg": (0, None),
+            "tau": (0, None),
         }
-        for key, guess in guess_dict.items():
-            if np.isnan(guess):
-                guess_dict[key] = 0
-
-        return drift_time_distribution._replace_values(guess_dict, **kwargs)
-
-    def bounds(guess, **kwargs):
+    elif func == exgauss:
         bounds_dict = {
-            "n_sig1": (0, None),
-            "mu1": (None, None),
-            "sigma1": (0, None),
-            "htail1": (0, 1),
-            "tau1": (None, None),
-            "n_sig2": (0, None),
-            "mu2": (None, None),
-            "sigma2": (0, None),
-            "htail2": (0, 1),
-            "tau2": (None, None),
-            "components": (None, None),
+            "x_lo": (None, None),
+            "x_hi": (None, None),
+            "area": (0, None),
+            "mu": (guess["x_lo"], guess["x_hi"]),
+            "sigma": (0, None),
+            "tau": (0, None),
         }
-
-        return [
-            bound
-            for field, bound in drift_time_distribution._replace_values(
-                bounds_dict, **kwargs
-            ).items()
-        ]
-
-    def fixed(**kwargs):
-        fixed_dict = {
-            "n_sig1": False,
-            "mu1": False,
-            "sigma1": False,
-            "htail1": False,
-            "tau1": False,
-            "n_sig2": False,
-            "mu2": False,
-            "sigma2": False,
-            "htail2": False,
-            "tau2": False,
-            "components": True,
+    elif func == gaussian:
+        bounds_dict = {
+            "x_lo": (None, None),
+            "x_hi": (None, None),
+            "area": (0, None),
+            "mu": (guess["x_lo"], guess["x_hi"]),
+            "sigma": (0, None),
         }
 
-        return [
-            fixed
-            for field, fixed in drift_time_distribution._replace_values(
-                fixed_dict, **kwargs
-            ).items()
-        ]
+    for item, value in kwargs.items():
+        bounds_dict[item] = value
+    return bounds_dict
+
+
+def aoe_peak_fixed(func, **kwargs):
+    if func == aoe_peak:
+        fixed = ["x_lo", "x_hi"]
+    elif func == aoe_peak_with_high_tail:
+        fixed = ["x_lo", "x_hi"]
+    elif func == exgauss:
+        fixed = ["x_lo", "x_hi"]
+    elif func == gaussian:
+        fixed = ["x_lo", "x_hi"]
+    mask = ~np.in1d(func.required_args(), fixed)
+    return fixed, mask
 
 
-class pol1:
+class Pol1:
+    @staticmethod
     def func(x, a, b):
         return x * a + b
 
+    @staticmethod
     def string_func(input_param):
         return f"{input_param}*a+b"
 
+    @staticmethod
     def guess(bands, means, mean_errs):
         return [-1e-06, 5e-01]
 
 
-class sigma_fit:
+class SigmaFit:
+    @staticmethod
     def func(x, a, b, c):
         return np.sqrt(a + (b / (x + 10**-99)) ** c)
 
+    @staticmethod
     def string_func(input_param):
         return f"(a+(b/({input_param}+10**-99))**c)**(0.5)"
 
+    @staticmethod
     def guess(bands, sigmas, sigma_errs):
         return [np.nanpercentile(sigmas, 50) ** 2, 2, 2]
 
 
-class sigmoid_fit:
+class SigmoidFit:
+    @staticmethod
     def func(x, a, b, c, d):
         return (a + b * x) * nb_erfc(c * x + d)
 
+    @staticmethod
     def guess(xs, ys, y_errs):
         return [np.nanmax(ys) / 2, 0, 1, 1.5]
 
 
 def unbinned_aoe_fit(
-    aoe: np.array, pdf=standard_aoe, display: int = 0, verbose: bool = False
+    aoe: np.array,
+    pdf=aoe_peak,
+    display: int = 0,
 ) -> tuple(np.array, np.array):
     """
-    Fitting function for A/E, first fits just a gaussian before using the full pdf to fit
+    Fitting function for A/E, first fits just a Gaussian before using the full pdf to fit
     if fails will return NaN values
+
+    Parameters
+    ----------
+    aoe: np.array
+        A/E values
+    pdf: PDF
+        PDF to fit to
+    display: int
+        Level of display
+
+    Returns
+    -------
+    tuple(np.array, np.array)
+        Tuple of fit values and errors
     """
+    if not isinstance(aoe, np.ndarray):
+        aoe = np.array(aoe)
+
+    bin_width = (
+        2
+        * (np.nanpercentile(aoe, 75) - np.nanpercentile(aoe, 25))
+        * len(aoe) ** (-1 / 3)
+    )
+    nbins = int(np.ceil((np.nanmax(aoe) - np.nanmin(aoe)) / bin_width))
     hist, bins, var = pgh.get_hist(aoe, bins=500)
 
-    gpars = gaussian.guess(hist, bins, var)
+    gpars = aoe_peak_guess(gaussian, hist, bins, var)
     c1_min = gpars["mu"] - 2 * gpars["sigma"]
     c1_max = gpars["mu"] + 3 * gpars["sigma"]
 
     # Initial fit just using Gaussian
-    c1 = cost.UnbinnedNLL(aoe[(aoe < c1_max) & (aoe > c1_min)], gaussian.pdf)
+    c1 = cost.ExtendedUnbinnedNLL(
+        aoe[(aoe < c1_max) & (aoe > c1_min)], gaussian.pdf_ext
+    )
 
-    m1 = Minuit(c1, **gpars)
-    m1.limits = [
-        (0, len(aoe[(aoe < c1_max) & (aoe > c1_min)])),
-        (gpars["mu"] * 0.8, gpars["mu"] * 1.2),
-        (0.8 * gpars["sigma"], gpars["sigma"] * 1.2),
-    ]
-    m1.fixed = gaussian.fixed()
-    m1.migrad()
+    m1 = Minuit(c1, *gpars)
 
-    if verbose:
-        print(m1)
+    bounds = aoe_peak_bounds(gaussian, gpars)
+    for arg, val in bounds.items():
+        m1.limits[arg] = val
+    for fix in aoe_peak_fixed(gaussian)[0]:
+        m1.fixed[fix] = True
+    m1.migrad()
 
     # Range to fit over, below this tail behaviour more exponential, few events above
     fmin = m1.values["mu"] - 15 * m1.values["sigma"]
     if fmin < np.nanmin(aoe):
         fmin = np.nanmin(aoe)
     fmax_bkg = m1.values["mu"] - 5 * m1.values["sigma"]
     fmax = m1.values["mu"] + 5 * m1.values["sigma"]
 
-    n_bkg_guess = len(aoe[(aoe < fmax) & (aoe > fmin)]) - m1.values["n_events"]
+    n_bkg_guess = len(aoe[(aoe < fmax) & (aoe > fmin)]) - m1.values["area"]
 
-    bkg_guess = standard_aoe_bkg.guess(
+    bkg_guess = aoe_peak_guess(
+        exgauss,
         hist,
         bins,
         var,
-        n_events=n_bkg_guess,
+        area=n_bkg_guess,
         mu=m1.values["mu"],
         sigma=m1.values["sigma"],
-        lower_range=fmin,
-        upper_range=fmax_bkg,
+        x_lo=fmin,
+        x_hi=fmax_bkg,
     )
 
-    c2 = cost.ExtendedUnbinnedNLL(
-        aoe[(aoe < fmax_bkg) & (aoe > fmin)], standard_aoe_bkg.extended_pdf
-    )
-    m2 = Minuit(c2, **bkg_guess)
-    m2.fixed = standard_aoe_bkg.fixed(mu=True)
-    m2.limits = standard_aoe_bkg.bounds(
-        bkg_guess, n_events=(0, 2 * len(aoe[(aoe < fmax_bkg) & (aoe > fmin)]))
-    )
+    c2 = cost.ExtendedUnbinnedNLL(aoe[(aoe < fmax_bkg) & (aoe > fmin)], exgauss.pdf_ext)
+    m2 = Minuit(c2, *bkg_guess)
+
+    bounds = aoe_peak_bounds(exgauss, bkg_guess)
+
+    for arg, val in bounds.items():
+        m2.limits[arg] = val
+    for fix in aoe_peak_fixed(exgauss)[0]:
+        m2.fixed[fix] = True
     m2.simplex().migrad()
     m2.hesse()
 
-    x0 = pdf.guess(
+    x0 = aoe_peak_guess(
+        pdf,
         hist,
         bins,
         var,
-        n_sig=m1.values["n_events"],
+        n_sig=m1.values["area"],
         mu=m1.values["mu"],
         sigma=m1.values["sigma"],
-        n_bkg=m2.values["n_events"],
-        tau_bkg=m2.values["tau_bkg"],
-        lower_range=fmin,
-        upper_range=fmax,
+        n_bkg=m2.values["area"],
+        tau=m2.values["tau"],
+        x_lo=fmin,
+        x_hi=fmax,
     )
-    if verbose:
-        print(x0)
 
-    # Full fit using gaussian signal with gaussian tail background
-    c = cost.ExtendedUnbinnedNLL(aoe[(aoe < fmax) & (aoe > fmin)], pdf.extended_pdf)
-    m = Minuit(c, **x0)
-    m.limits = pdf.bounds(
-        x0,
-        n_sig=(0, 2 * len(aoe[(aoe < fmax) & (aoe > fmin)])),
-        n_bkg=(0, 2 * len(aoe[(aoe < fmax) & (aoe > fmin)])),
-    )
-    m.fixed = pdf.fixed()
+    bounds = aoe_peak_bounds(pdf, x0)
+
+    # Full fit using Gaussian signal with Gaussian tail background
+    c = cost.ExtendedUnbinnedNLL(aoe[(aoe < fmax) & (aoe > fmin)], pdf.pdf_ext)
+    m = Minuit(c, *x0)
+    for arg, val in bounds.items():
+        m.limits[arg] = val
+    fixed, mask = aoe_peak_fixed(pdf)
+    for fix in fixed:
+        m.fixed[fix] = True
     m.migrad()
     m.hesse()
 
-    if verbose:
-        print(m)
-
     if np.isnan(m.errors).all():
         try:
             m.simplex.migrad()
             m.hesse()
-        except:
+        except Exception:
             return return_nans(pdf)
 
     if display > 1:
+        aoe = aoe[(aoe < fmax) & (aoe > fmin)]
+        bin_width = (
+            2
+            * (np.nanpercentile(aoe, 75) - np.nanpercentile(aoe, 25))
+            * len(aoe) ** (-1 / 3)
+        )
+        nbins = int(np.ceil((np.nanmax(aoe) - np.nanmin(aoe)) / bin_width))  # *5
+
         plt.figure()
         xs = np.linspace(fmin, fmax, 1000)
-        counts, bins, bars = plt.hist(
-            aoe[(aoe < fmax) & (aoe > fmin)], bins=200, histtype="step", label="Data"
-        )
+        counts, bins, bars = plt.hist(aoe, bins=nbins, histtype="step", label="Data")
         dx = np.diff(bins)
-        plt.plot(xs, pdf.pdf(xs, *m.values) * dx[0], label="Full fit")
-        sig, bkg = pdf.pdf(xs, *m.values[:-1], True)
+        plt.plot(xs, pdf.get_pdf(xs, *m.values) * dx[0], label="Full fit")
+        pdf.components = True
+        sig, bkg = pdf.get_pdf(xs, *m.values)
+        pdf.components = False
         plt.plot(xs, sig * dx[0], label="Signal")
         plt.plot(xs, bkg * dx[0], label="Background")
-        plt.plot(xs, gaussian.pdf(xs, *m1.values) * dx[0], label="Initial Gaussian")
-        plt.plot(xs, standard_aoe_bkg.pdf(xs, *m2.values) * dx[0], label="Bkg guess")
+        plt.plot(
+            xs, gaussian.pdf_ext(xs, *m1.values)[1] * dx[0], label="Initial Gaussian"
+        )
+        plt.plot(xs, exgauss.pdf_ext(xs, *m2.values)[1] * dx[0], label="Bkg guess")
         plt.xlabel("A/E")
         plt.ylabel("Counts")
         plt.legend(loc="upper left")
         plt.show()
 
         plt.figure()
         bin_centers = (bins[1:] + bins[:-1]) / 2
@@ -852,265 +400,137 @@
         plt.show()
         return m.values, m.errors, m.covariance
 
     else:
         return m.values, m.errors, m.covariance
 
 
-def fit_time_means(tstamps, means, reses):
+def fit_time_means(tstamps, means, sigmas):
+    """
+    Fit the time dependence of the means of the A/E distribution
+
+    Args:
+
+    tstamps: np.array
+        Timestamps of the data
+    means: np.array
+        Means of the A/E distribution
+    sigmas: np.array
+        Sigmas of the A/E distribution
+
+    Returns: dict
+        Dictionary of the time dependence of the means
+    """
     out_dict = {}
     current_tstamps = []
     current_means = []
-    current_reses = []
+    current_sigmas = []
     rolling_mean = means[
         np.where(
-            (np.abs(np.diff(means)) < (0.4 * np.array(reses)[1:]))
-            & (~np.isnan(np.abs(np.diff(means)) < (0.4 * np.array(reses)[1:])))
+            (np.abs(np.diff(means)) < (0.4 * np.array(sigmas)[1:]))
+            & (~np.isnan(np.abs(np.diff(means)) < (0.4 * np.array(sigmas)[1:])))
         )[0][0]
     ]
     for i, tstamp in enumerate(tstamps):
         if (
             (
-                np.abs(means[i] - rolling_mean) > 0.4 * reses[i]
+                np.abs(means[i] - rolling_mean) > 0.4 * sigmas[i]
                 and np.abs(means[i] - rolling_mean) > rolling_mean * 0.01
             )
             or np.isnan(means[i])
-            or np.isnan(reses[i])
+            or np.isnan(sigmas[i])
         ):
             if i + 1 == len(means):
                 out_dict[tstamp] = np.nan
             else:
-                if (np.abs(means[i + 1] - means[i]) < 0.4 * reses[i + 1]) and not (
+                if (np.abs(means[i + 1] - means[i]) < 0.4 * sigmas[i + 1]) and not (
                     np.isnan(means[i])
                     or np.isnan(means[i + 1])
-                    or np.isnan(reses[i])
-                    or np.isnan(reses[i + 1])
+                    or np.isnan(sigmas[i])
+                    or np.isnan(sigmas[i + 1])
                 ):
                     for ts in current_tstamps:
                         out_dict[ts] = rolling_mean
                     rolling_mean = means[i]
                     current_means = [means[i]]
                     current_tstamps = [tstamp]
-                    current_reses = [reses[i]]
+                    current_sigmas = [sigmas[i]]
                 else:
                     out_dict[tstamp] = np.nan
         else:
             current_tstamps.append(tstamp)
             current_means.append(means[i])
-            current_reses.append(reses[i])
+            current_sigmas.append(sigmas[i])
             rolling_mean = np.average(
-                current_means, weights=1 / np.array(current_reses)
+                current_means, weights=1 / np.array(current_sigmas)
             )
     for tstamp in current_tstamps:
         out_dict[tstamp] = rolling_mean
     return out_dict
 
 
-def energy_guess(hist, bins, var, func_i, peak, eres, fit_range):
+def energy_guess(energy, func_i, fit_range=None, bin_width=1, peak=None, eres=None):
     """
     Simple guess for peak fitting
     """
-    if func_i == pgf.extended_radford_pdf:
-        bin_cs = (bins[1:] + bins[:-1]) / 2
-        sigma = eres / 2.355
-        i_0 = np.nanargmax(hist)
-        mu = peak
-        height = hist[i_0]
-        bg0 = np.mean(hist[-10:])
-        step = np.mean(hist[:10]) - bg0
-        htail = 1.0 / 5
-        tau = 0.5 * sigma
-
-        hstep = step / (bg0 + np.mean(hist[:10]))
-        dx = np.diff(bins)[0]
-        n_bins_range = int((3 * sigma) // dx)
-        nsig_guess = np.sum(hist[i_0 - n_bins_range : i_0 + n_bins_range]) - (
-            (n_bins_range * 2) * (bg0 - step / 2)
-        )
-        nbkg_guess = np.sum(hist) - nsig_guess
-        if nbkg_guess < 0:
-            nbkg_guess = 0
-        if nsig_guess < 0:
-            nsig_guess = 0
-        parguess = [
-            nsig_guess,
-            mu,
-            sigma,
-            htail,
-            tau,
-            nbkg_guess,
-            hstep,
-            fit_range[0],
-            fit_range[1],
-            0,
-        ]
-        for i, guess in enumerate(parguess):
-            if np.isnan(guess):
-                parguess[i] = 0
-        return parguess
+    if fit_range is None:
+        fit_range = (np.nanmin(energy), np.nanmax(energy))
+    if func_i == hpge_peak or func_i == gauss_on_step:
+        parguess = pgc.get_hpge_energy_peak_par_guess(
+            energy, func_i, fit_range=fit_range
+        )
+
+        if peak is not None:
+            parguess["mu"] = peak
+
+        if eres is not None:
+            parguess["sigma"] = eres / 2.355
 
-    elif func_i == pgf.extended_gauss_step_pdf:
-        mu = peak
-        sigma = eres / 2.355
-        i_0 = np.argmax(hist)
-        bg = np.mean(hist[-10:])
-        step = bg - np.mean(hist[:10])
-        hstep = step / (bg + np.mean(hist[:10]))
-        dx = np.diff(bins)[0]
-        n_bins_range = int((3 * sigma) // dx)
-        nsig_guess = np.sum(hist[i_0 - n_bins_range : i_0 + n_bins_range])
-        nbkg_guess = np.sum(hist) - nsig_guess
-        if nbkg_guess < 0:
-            nbkg_guess = 0
-        if nsig_guess < 0:
-            nsig_guess = 0
-
-        parguess = [
-            nsig_guess,
-            mu,
-            sigma,
-            nbkg_guess,
-            hstep,
-            fit_range[0],
-            fit_range[1],
-            0,
-        ]
         for i, guess in enumerate(parguess):
             if np.isnan(guess):
                 parguess[i] = 0
-        return parguess
 
+    else:
+        log.error(f"energy_guess not implemented for {func_i}")
+        return None
+    return parguess
 
-def unbinned_energy_fit(
-    energy: np.array,
-    peak: float,
-    eres: list,
-    simplex=False,
-    guess=None,
-    display=0,
-    verbose: bool = False,
-) -> tuple(np.array, np.array):
+
+def fix_all_but_nevents(func):
     """
-    Fitting function for energy peaks used to calculate survival fractions
+    Returns: Sequence list of fixed indexes for fitting and mask for parameters
     """
-    try:
-        hist, bins, var = pgh.get_hist(
-            energy, dx=0.5, range=(np.nanmin(energy), np.nanmax(energy))
-        )
-    except ValueError:
-        pars, errs, cov = return_nans(pgf.radford_pdf)
-        return pars, errs
-    sigma = eres / 2.355
-    if guess is None:
-        x0 = energy_guess(
-            hist,
-            bins,
-            var,
-            pgf.extended_gauss_step_pdf,
-            peak,
-            eres,
-            (np.nanmin(energy), np.nanmax(energy)),
-        )
-        c = cost.ExtendedUnbinnedNLL(energy, pgf.extended_gauss_step_pdf)
-        m = Minuit(c, *x0)
-        m.limits = [
-            (0, 2 * np.sum(hist)),
-            (peak - 1, peak + 1),
-            (0, None),
-            (0, 2 * np.sum(hist)),
-            (-1, 1),
-            (None, None),
-            (None, None),
-            (None, None),
-        ]
-        m.fixed[-3:] = True
-        m.simplex().migrad()
-        m.hesse()
-        x0 = m.values[:3]
-        x0 += [0.2, 0.2 * m.values[2]]
-        x0 += m.values[3:]
-        if verbose:
-            print(m)
-        bounds = [
-            (0, 2 * np.sum(hist)),
-            (peak - 1, peak + 1),
-            (0, None),
-            (0, 1),
-            (0, None),
-            (0, 2 * np.sum(hist)),
-            (-1, 1),
-            (None, None),
-            (None, None),
-            (None, None),
-        ]
-        fixed = [7, 8, 9]
-    else:
-        x0 = guess
-        x1 = energy_guess(
-            hist,
-            bins,
-            var,
-            pgf.extended_radford_pdf,
-            peak,
-            eres,
-            (np.nanmin(energy), np.nanmax(energy)),
-        )
-        x0[0] = x1[0]
-        x0[5] = x1[5]
-        bounds = [
-            (0, 2 * np.sum(hist)),
-            (guess[1] - 0.5, guess[1] + 0.5),
-            sorted((0.8 * guess[2], 1.2 * guess[2])),
-            sorted((0.8 * guess[3], 1.2 * guess[3])),
-            sorted((0.8 * guess[4], 1.2 * guess[4])),
-            (0, 2 * np.sum(hist)),
-            sorted((0.8 * guess[6], 1.2 * guess[6])),
-            (None, None),
-            (None, None),
-            (None, None),
-        ]
-        fixed = [1, 2, 3, 4, 6, 7, 8, 9]
-    if len(x0) == 0:
-        pars, errs, cov = return_nans(pgf.extended_radford_pdf)
-        return pars, errs
-
-    if verbose:
-        print(x0)
-    c = cost.ExtendedUnbinnedNLL(energy, pgf.extended_radford_pdf)
-    m = Minuit(c, *x0)
-    m.limits = bounds
-    for fix in fixed:
-        m.fixed[fix] = True
-    if simplex == True:
-        m.simplex().migrad()
+
+    if func == gauss_on_step:
+        # pars are: n_sig, mu, sigma, n_bkg, hstep, lower, upper, components
+        fixed = ["x_lo", "x_hi", "mu", "sigma", "hstep"]
+
+    elif func == hpge_peak:
+        # pars are: , components
+        fixed = ["x_lo", "x_hi", "mu", "sigma", "htail", "tau", "hstep"]
+
     else:
-        m.migrad()
+        log.error(f"get_hpge_E_fixed not implemented for {func}")
+        return None, None
+    mask = ~np.in1d(func.required_args(), fixed)
+    return fixed, mask
 
-    m.hesse()
-    if verbose:
-        print(m)
-    if display > 1:
-        plt.figure()
-        bcs = (bins[1:] + bins[:-1]) / 2
-        plt.step(bcs, hist, where="mid")
-        plt.plot(bcs, pgf.radford_pdf(bcs, *x0) * np.diff(bcs)[0])
-        plt.plot(bcs, pgf.radford_pdf(bcs, *m.values) * np.diff(bcs)[0])
-        plt.show()
 
-    if not np.isnan(m.errors[:-3]).all():
-        return m.values, m.errors
+def get_bounds(func, parguess):
+    if func == hpge_peak or func == gauss_on_step:
+        bounds = pgc.get_hpge_energy_bounds(func, parguess)
+
+        bounds["mu"] = (parguess["mu"] - 1, parguess["mu"] + 1)
+        bounds["n_sig"] = (0, 2 * (parguess["n_sig"] + parguess["n_bkg"]))
+        bounds["n_bkg"] = (0, 2 * (parguess["n_sig"] + parguess["n_bkg"]))
+
     else:
-        try:
-            m.simplex().migrad()
-            m.minos()
-            if not np.isnan(m.errors[:-3]).all():
-                return m.values, m.errors
-        except:
-            pars, errs, cov = return_nans(pgf.extended_radford_pdf)
-            return pars, errs
+        log.error(f"get_bounds not implemented for {func}")
+        return None
+    return bounds
 
 
 def get_peak_label(peak: float) -> str:
     if peak == 2039:
         return "CC @"
     elif peak == 1592.5:
         return "Tl DEP @"
@@ -1118,162 +538,276 @@
         return "Bi FEP @"
     elif peak == 2103.53:
         return "Tl SEP @"
     elif peak == 2614.5:
         return "Tl FEP @"
 
 
+def update_guess(func, parguess, energies):
+    if func == gauss_on_step:
+        total_events = len(energies)
+        parguess["n_sig"] = len(
+            energies[
+                (energies > parguess["mu"] - 2 * parguess["sigma"])
+                & (energies < parguess["mu"] + 2 * parguess["sigma"])
+            ]
+        )
+        parguess["n_bkg"] = total_events - parguess["n_sig"]
+        return parguess
+
+    if func == hpge_peak:
+        total_events = len(energies)
+        parguess["n_sig"] = len(
+            energies[
+                (energies > parguess["mu"] - 2 * parguess["sigma"])
+                & (energies < parguess["mu"] + 2 * parguess["sigma"])
+            ]
+        )
+        parguess["n_bkg"] = total_events - parguess["n_sig"]
+        return parguess
+
+    else:
+        log.error(f"update_guess not implemented for {func}")
+        return parguess
+
+
 def get_survival_fraction(
     energy,
     cut_param,
     cut_val,
     peak,
     eres_pars,
+    fit_range=None,
     high_cut=None,
     guess_pars_cut=None,
     guess_pars_surv=None,
     dt_mask=None,
     mode="greater",
+    func=hpge_peak,
     display=0,
 ):
     if dt_mask is None:
         dt_mask = np.full(len(cut_param), True, dtype=bool)
 
+    if not isinstance(energy, np.ndarray):
+        energy = np.array(energy)
+    if not isinstance(cut_param, np.ndarray):
+        cut_param = np.array(cut_param)
+
+    if fit_range is None:
+        fit_range = (np.nanmin(energy), np.nanmax(energy))
+
     nan_idxs = np.isnan(cut_param)
     if high_cut is not None:
         idxs = (cut_param > cut_val) & (cut_param < high_cut) & dt_mask
     else:
         if mode == "greater":
             idxs = (cut_param > cut_val) & dt_mask
         elif mode == "less":
             idxs = (cut_param < cut_val) & dt_mask
         else:
             raise ValueError("mode not recognised")
 
     if guess_pars_cut is None or guess_pars_surv is None:
-        pars, errs = unbinned_energy_fit(energy, peak, eres_pars, simplex=True)
+        (pars, errs, cov, _, func, _, _, _) = pgc.unbinned_staged_energy_fit(
+            energy,
+            func,
+            guess_func=energy_guess,
+            bounds_func=get_bounds,
+            guess_kwargs={"peak": peak, "eres": eres_pars},
+            fit_range=fit_range,
+        )
+
         guess_pars_cut = pars
         guess_pars_surv = pars
-
-    cut_pars, ct_errs = unbinned_energy_fit(
+    # add update guess here for n_sig and n_bkg
+    guess_pars_cut = update_guess(func, guess_pars_cut, energy[(~nan_idxs) & (~idxs)])
+    (cut_pars, cut_errs, cut_cov, _, _, _, _, _) = pgc.unbinned_staged_energy_fit(
         energy[(~nan_idxs) & (~idxs)],
-        peak,
-        eres_pars,
+        func,
         guess=guess_pars_cut,
-        simplex=False,
-        display=display,
-        verbose=False,
+        guess_func=energy_guess,
+        bounds_func=get_bounds,
+        fixed_func=fix_all_but_nevents,
+        guess_kwargs={"peak": peak, "eres": eres_pars},
+        lock_guess=True,
+        allow_tail_drop=False,
+        fit_range=fit_range,
     )
-
-    surv_pars, surv_errs = unbinned_energy_fit(
+    guess_pars_surv = update_guess(func, guess_pars_cut, energy[(~nan_idxs) & (idxs)])
+    (surv_pars, surv_errs, surv_cov, _, _, _, _, _) = pgc.unbinned_staged_energy_fit(
         energy[(~nan_idxs) & (idxs)],
-        peak,
-        eres_pars,
+        func,
         guess=guess_pars_surv,
-        simplex=False,
-        display=display,
+        guess_func=energy_guess,
+        bounds_func=get_bounds,
+        fixed_func=fix_all_but_nevents,
+        guess_kwargs={"peak": peak, "eres": eres_pars},
+        lock_guess=True,
+        allow_tail_drop=False,
+        fit_range=fit_range,
     )
 
     ct_n = cut_pars["n_sig"]
-    ct_err = ct_errs["n_sig"]
+    ct_err = cut_errs["n_sig"]
     surv_n = surv_pars["n_sig"]
     surv_err = surv_errs["n_sig"]
 
     pc_n = ct_n + surv_n
     pc_err = np.sqrt(surv_err**2 + ct_err**2)
 
     sf = (surv_n / pc_n) * 100
     err = sf * np.sqrt((pc_err / pc_n) ** 2 + (surv_err / surv_n) ** 2)
     return sf, err, cut_pars, surv_pars
 
 
 def get_sf_sweep(
     energy: np.array,
     cut_param: np.array,
-    final_cut_value: float,
-    peak: float,
-    eres_pars: list,
+    final_cut_value: float = None,
+    peak: float = 1592.5,
+    eres_pars: list = None,
     dt_mask=None,
     cut_range=(-5, 5),
-    n_samples=51,
+    n_samples=26,
     mode="greater",
+    fit_range=None,
+    debug_mode=False,
 ) -> tuple(pd.DataFrame, float, float):
     """
     Calculates survival fraction for gamma lines using fitting method as in cut determination
     """
 
     if dt_mask is None:
         dt_mask = np.full(len(cut_param), True, dtype=bool)
 
+    if not isinstance(energy, np.ndarray):
+        energy = np.array(energy)
+    if not isinstance(cut_param, np.ndarray):
+        cut_param = np.array(cut_param)
+
     cut_vals = np.linspace(cut_range[0], cut_range[1], n_samples)
-    out_df = pd.DataFrame(columns=["cut_val", "sf", "sf_err"])
+    out_df = pd.DataFrame()
+
+    (pars, _, _, _, func, _, _, _) = pgc.unbinned_staged_energy_fit(
+        energy,
+        hpge_peak,
+        guess_func=energy_guess,
+        bounds_func=get_bounds,
+        guess_kwargs={"peak": peak, "eres": eres_pars},
+        fit_range=fit_range,
+    )
+    guess_pars_cut = pars
+    guess_pars_surv = pars
+
     for cut_val in cut_vals:
         try:
-            sf, err, cut_pars, surv_pars = get_survival_fraction(
-                energy, cut_param, cut_val, peak, eres_pars, dt_mask=dt_mask, mode=mode
+            sf, err, _, _ = get_survival_fraction(
+                energy,
+                cut_param,
+                cut_val,
+                peak,
+                eres_pars,
+                fit_range=fit_range,
+                dt_mask=dt_mask,
+                mode=mode,
+                guess_pars_cut=guess_pars_cut,
+                guess_pars_surv=guess_pars_surv,
+                func=func,
             )
             out_df = pd.concat(
                 [out_df, pd.DataFrame([{"cut_val": cut_val, "sf": sf, "sf_err": err}])]
             )
-        except:
-            pass
+        except BaseException as e:
+            if e == KeyboardInterrupt:
+                raise (e)
+            elif debug_mode:
+                raise (e)
     out_df.set_index("cut_val", inplace=True)
-    sf, sf_err, cut_pars, surv_pars = get_survival_fraction(
-        energy, cut_param, final_cut_value, peak, eres_pars, dt_mask=dt_mask, mode=mode
-    )
+    if final_cut_value is not None:
+        sf, sf_err, cut_pars, surv_pars = get_survival_fraction(
+            energy,
+            cut_param,
+            final_cut_value,
+            peak,
+            eres_pars,
+            fit_range=fit_range,
+            dt_mask=dt_mask,
+            mode=mode,
+            guess_pars_cut=guess_pars_cut,
+            guess_pars_surv=guess_pars_surv,
+            func=func,
+        )
+    else:
+        sf = None
+        sf_err = None
     return (
-        out_df.query(
-            f'sf_err<5*{np.nanpercentile(out_df["sf_err"], 50)}& sf_err==sf_err & sf<=100'
-        ),
+        out_df,
         sf,
         sf_err,
     )
 
 
 def compton_sf(cut_param, low_cut_val, high_cut_val=None, mode="greater", dt_mask=None):
     if dt_mask is None:
         dt_mask = np.full(len(cut_param), True, dtype=bool)
 
+    if not isinstance(cut_param, np.ndarray):
+        cut_param = np.array(cut_param)
+
     if high_cut_val is not None:
         mask = (cut_param > low_cut_val) & (cut_param < high_cut_val) & dt_mask
     else:
         if mode == "greater":
             mask = (cut_param > low_cut_val) & dt_mask
         elif mode == "less":
             mask = (cut_param < low_cut_val) & dt_mask
         else:
             raise ValueError("mode not recognised")
 
-    sf = 100 * len(cut_param[mask]) / len(cut_param)
-    sf_err = sf * np.sqrt((1 / len(cut_param)) + 1 / (len(cut_param[mask]) + 10**-99))
+    ct_n = len(cut_param[~mask])
+    ct_err = np.sqrt(len(cut_param[~mask]))
+    surv_n = len(cut_param[mask])
+    surv_err = np.sqrt(len(cut_param[mask]))
+
+    pc_n = ct_n + surv_n
+    pc_err = np.sqrt(surv_err**2 + ct_err**2)
+
+    sf = (surv_n / pc_n) * 100
+    err = sf * np.sqrt((pc_err / pc_n) ** 2 + (surv_err / surv_n) ** 2)
+
     return {
         "low_cut": low_cut_val,
         "sf": sf,
-        "sf_err": sf_err,
+        "sf_err": err,
         "high_cut": high_cut_val,
     }
 
 
 def compton_sf_sweep(
     energy: np.array,
     cut_param: np.array,
     final_cut_value: float,
     peak: float,
-    eres: list[float, float],
+    eres: list[float, float] = None,
     dt_mask: np.array = None,
     cut_range=(-5, 5),
     n_samples=51,
     mode="greater",
 ) -> tuple(float, np.array, list):
     """
     Determines survival fraction for compton continuum by basic counting
     """
+    if not isinstance(energy, np.ndarray):
+        energy = np.array(energy)
+    if not isinstance(cut_param, np.ndarray):
+        cut_param = np.array(cut_param)
 
     cut_vals = np.linspace(cut_range[0], cut_range[1], n_samples)
-    out_df = pd.DataFrame(columns=["cut_val", "sf", "sf_err"])
+    out_df = pd.DataFrame()
 
     for cut_val in cut_vals:
         ct_dict = compton_sf(cut_param, cut_val, mode=mode, dt_mask=dt_mask)
         df = pd.DataFrame(
             [
                 {
                     "cut_val": ct_dict["low_cut"],
@@ -1286,80 +820,72 @@
     out_df.set_index("cut_val", inplace=True)
 
     sf_dict = compton_sf(cut_param, final_cut_value, mode=mode, dt_mask=dt_mask)
 
     return out_df, sf_dict["sf"], sf_dict["sf_err"]
 
 
-class cal_aoe:
+class CalAoE:
     def __init__(
         self,
-        cal_dicts: dict = {},
+        cal_dicts: dict = None,
         cal_energy_param: str = "cuspEmax_ctc_cal",
         eres_func: callable = lambda x: 1,
-        pdf=standard_aoe,
-        selection_string: str = "",
+        pdf=aoe_peak,
+        selection_string: str = "index==index",
         dt_corr: bool = False,
-        dep_acc: float = 0.9,
         dep_correct: bool = False,
         dt_cut: dict = None,
         dt_param: str = "dt_eff",
         high_cut_val: int = 3,
-        mean_func: Callable = pol1,
-        sigma_func: Callable = sigma_fit,
-        comptBands_width: int = 20,
-        plot_options: dict = {},
+        mean_func: Callable = Pol1,
+        sigma_func: Callable = SigmaFit,
+        compt_bands_width: int = 20,
+        debug_mode: bool = False,
     ):
-        self.cal_dicts = cal_dicts
+        self.cal_dicts = cal_dicts if cal_dicts is not None else {}
         self.cal_energy_param = cal_energy_param
         self.eres_func = eres_func
         self.pdf = pdf
         self.selection_string = selection_string
         self.dt_corr = dt_corr
         self.dt_param = "dt_eff"
         self.dep_correct = dep_correct
         self.dt_cut = dt_cut
-        self.dep_acc = dep_acc
         if self.dt_cut is not None:
             self.dt_cut_param = dt_cut["out_param"]
             self.fit_selection = f"{self.selection_string} & {self.dt_cut_param}"
             self.dt_cut_hard = dt_cut["hard"]
         else:
             self.dt_cut_param = None
             self.dt_cut_hard = False
             self.fit_selection = self.selection_string
         self.high_cut_val = high_cut_val
         self.mean_func = mean_func
         self.sigma_func = sigma_func
-        self.comptBands_width = comptBands_width
-        self.plot_options = plot_options
+        self.compt_bands_width = compt_bands_width
+        self.debug_mode = debug_mode
 
     def update_cal_dicts(self, update_dict):
-        if re.match(r"(\d{8})T(\d{6})Z", list(self.cal_dicts)[0]):
+        if len(self.cal_dicts) > 0 and re.match(
+            r"(\d{8})T(\d{6})Z", list(self.cal_dicts)[0]
+        ):
             for tstamp in self.cal_dicts:
                 if tstamp in update_dict:
                     self.cal_dicts[tstamp].update(update_dict[tstamp])
                 else:
                     self.cal_dicts[tstamp].update(update_dict)
         else:
             self.cal_dicts.update(update_dict)
 
-    def aoe_timecorr(self, df, aoe_param, output_name="AoE_Timecorr", display=0):
+    def time_correction(self, df, aoe_param, output_name="AoE_Timecorr", display=0):
         log.info("Starting A/E time correction")
-        self.timecorr_df = pd.DataFrame(
-            columns=["run_timestamp", "mean", "mean_err", "res", "res_err"]
-        )
+        self.timecorr_df = pd.DataFrame()
         try:
             if "run_timestamp" in df:
-                tstamps = sorted(np.unique(df["run_timestamp"]))
-                means = []
-                errors = []
-                reses = []
-                res_errs = []
-                final_tstamps = []
                 for tstamp, time_df in df.groupby("run_timestamp", sort=True):
                     try:
                         pars, errs, cov = unbinned_aoe_fit(
                             time_df.query(
                                 f"{self.fit_selection} & ({self.cal_energy_param}>1000) & ({self.cal_energy_param}<1300)"
                             )[aoe_param],
                             pdf=self.pdf,
@@ -1370,63 +896,86 @@
                                 self.timecorr_df,
                                 pd.DataFrame(
                                     [
                                         {
                                             "run_timestamp": tstamp,
                                             "mean": pars["mu"],
                                             "mean_err": errs["mu"],
+                                            "sigma": pars["sigma"],
+                                            "sigma_err": errs["sigma"],
                                             "res": pars["sigma"] / pars["mu"],
                                             "res_err": (pars["sigma"] / pars["mu"])
                                             * np.sqrt(
                                                 errs["sigma"] / pars["sigma"]
                                                 + errs["mu"] / pars["mu"]
                                             ),
                                         }
                                     ]
                                 ),
                             ]
                         )
-                    except:
+                    except BaseException as e:
+                        if e == KeyboardInterrupt:
+                            raise (e)
+                        elif self.debug_mode:
+                            raise (e)
                         self.timecorr_df = pd.concat(
                             [
                                 self.timecorr_df,
                                 pd.DataFrame(
                                     [
                                         {
                                             "run_timestamp": tstamp,
                                             "mean": np.nan,
                                             "mean_err": np.nan,
+                                            "sigma": np.nan,
+                                            "sigma_err": np.nan,
                                             "res": np.nan,
                                             "res_err": np.nan,
                                         }
                                     ]
                                 ),
                             ]
                         )
                 self.timecorr_df.set_index("run_timestamp", inplace=True)
-                time_dict = fit_time_means(
-                    np.array(self.timecorr_df.index),
-                    np.array(self.timecorr_df["mean"]),
-                    np.array(self.timecorr_df["res"]),
-                )
+                if len(self.timecorr_df) > 1:
+                    time_dict = fit_time_means(
+                        np.array(self.timecorr_df.index),
+                        np.array(self.timecorr_df["mean"]),
+                        np.array(self.timecorr_df["sigma"]),
+                    )
 
-                df[output_name] = df[aoe_param] / np.array(
-                    [time_dict[tstamp] for tstamp in df["run_timestamp"]]
-                )
-                self.update_cal_dicts(
-                    {
-                        tstamp: {
+                    df[output_name] = df[aoe_param] / np.array(
+                        [time_dict[tstamp] for tstamp in df["run_timestamp"]]
+                    )
+                    self.update_cal_dicts(
+                        {
+                            tstamp: {
+                                output_name: {
+                                    "expression": f"{aoe_param}/a",
+                                    "parameters": {"a": t_dict},
+                                }
+                            }
+                            for tstamp, t_dict in time_dict.items()
+                        }
+                    )
+                else:
+                    df[output_name] = (
+                        df[aoe_param] / np.array(self.timecorr_df["mean"])[0]
+                    )
+                    self.update_cal_dicts(
+                        {
                             output_name: {
                                 "expression": f"{aoe_param}/a",
-                                "parameters": {"a": t_dict},
+                                "parameters": {
+                                    "a": np.array(self.timecorr_df["mean"])[0]
+                                },
                             }
                         }
-                        for tstamp, t_dict in time_dict.items()
-                    }
-                )
+                    )
                 log.info("A/E time correction finished")
             else:
                 try:
                     pars, errs, cov = unbinned_aoe_fit(
                         df.query(
                             f"{self.fit_selection} & {self.cal_energy_param}>1000 & {self.cal_energy_param}<1300"
                         )[aoe_param],
@@ -1435,36 +984,47 @@
                     )
                     self.timecorr_df = pd.concat(
                         [
                             self.timecorr_df,
                             pd.DataFrame(
                                 [
                                     {
+                                        "run_timestamp": np.nan,
                                         "mean": pars["mu"],
                                         "mean_err": errs["mu"],
+                                        "sigma": pars["sigma"],
+                                        "sigma_err": errs["sigma"],
                                         "res": pars["sigma"] / pars["mu"],
                                         "res_err": (pars["sigma"] / pars["mu"])
                                         * np.sqrt(
                                             errs["sigma"] / pars["sigma"]
                                             + errs["mu"] / pars["mu"]
                                         ),
                                     }
                                 ]
                             ),
                         ]
                     )
-                except:
+                except BaseException as e:
+                    if e == KeyboardInterrupt:
+                        raise (e)
+                    elif self.debug_mode:
+                        raise (e)
+
                     self.timecorr_df = pd.concat(
                         [
                             self.timecorr_df,
                             pd.DataFrame(
                                 [
                                     {
+                                        "run_timestamp": np.nan,
                                         "mean": np.nan,
                                         "mean_err": np.nan,
+                                        "sigma": np.nan,
+                                        "sigma_err": np.nan,
                                         "res": np.nan,
                                         "res_err": np.nan,
                                     }
                                 ]
                             ),
                         ]
                     )
@@ -1473,30 +1033,36 @@
                     {
                         output_name: {
                             "expression": f"{aoe_param}/a",
                             "parameters": {"a": pars["mu"]},
                         }
                     }
                 )
-                log.info("A/E time correction finished")
-        except:
+                log.info("Finished A/E time correction")
+        except BaseException as e:
+            if e == KeyboardInterrupt:
+                raise (e)
+            elif self.debug_mode:
+                raise (e)
             log.error("A/E time correction failed")
+            df[output_name] = df[aoe_param] / np.nan
             self.update_cal_dicts(
                 {
                     output_name: {
                         "expression": f"{aoe_param}/a",
                         "parameters": {"a": np.nan},
                     }
                 }
             )
 
     def drift_time_correction(
         self,
         data: pd.DataFrame,
         aoe_param,
+        out_param="AoE_DTcorr",
         display: int = 0,
     ):
         """
         Calculates the correction needed to align the two drift time regions for ICPC detectors
         """
         log.info("Starting A/E drift time correction")
         self.dt_res_dict = {}
@@ -1514,113 +1080,142 @@
             aoe_range = [mu * 0.9, mu * 1.1]
 
             dt_range = [
                 np.nanpercentile(dep_events[self.dt_param], 1),
                 np.nanpercentile(dep_events[self.dt_param], 99),
             ]
 
-            self.dt_res_dict[
-                "final_selection"
-            ] = f"{aoe_param}>{aoe_range[0]}&{aoe_param}<{aoe_range[1]}&{self.dt_param}>{dt_range[0]}&{self.dt_param}<{dt_range[1]}&{self.dt_param}=={self.dt_param}"
+            self.dt_res_dict["final_selection"] = (
+                f"{aoe_param}>{aoe_range[0]}&{aoe_param}<{aoe_range[1]}&{self.dt_param}>{dt_range[0]}&{self.dt_param}<{dt_range[1]}&{self.dt_param}=={self.dt_param}"
+            )
 
             final_df = dep_events.query(self.dt_res_dict["final_selection"])
 
             hist, bins, var = pgh.get_hist(
                 final_df[self.dt_param],
                 dx=10,
                 range=(
                     np.nanmin(final_df[self.dt_param]),
                     np.nanmax(final_df[self.dt_param]),
                 ),
             )
 
-            gpars = self.dt_res_dict["dt_guess"] = drift_time_distribution.guess(
-                hist, bins, var
-            )
-            cost_func = cost.ExtendedUnbinnedNLL(
-                final_df[self.dt_param], drift_time_distribution.extended_pdf
-            )
-            m = Minuit(cost_func, **gpars)
-            m.limits = drift_time_distribution.bounds(gpars)
-            m.fixed = drift_time_distribution.fixed()
-            m.simplex().migrad()
-            m.hesse()
+            bcs = pgh.get_bin_centers(bins)
+            mus = pgc.get_i_local_maxima(hist / (np.sqrt(var) + 10**-99), 2)
+            pk_pars, pk_covs = pgc.hpge_fit_energy_peak_tops(
+                hist,
+                bins,
+                var=var,
+                peak_locs=mus,
+                n_to_fit=5,
+            )
+
+            mus = pk_pars[:, 0]
+            sigmas = pk_pars[:, 1]
+            amps = pk_pars[:, 2]
+
+            if len(mus) > 2:
+                ids = np.array(
+                    sorted([np.argmax(amps), np.argmax(amps[amps != np.argmax(amps)])])
+                )
+            else:
+                ids = np.full(len(mus), True, dtype=bool)
+            mus = [bcs[int(mu)] for mu in mus[ids]]
+            sigmas = sigmas[ids]
+            amps = amps[ids]
 
-            self.dt_res_dict["dt_fit"] = {
-                "pars": m.values,
-                "errs": m.errors,
-                "object": m,
-            }
-            aoe_grp1 = self.dt_res_dict[
-                "aoe_grp1"
-            ] = f'{self.dt_param}>{m.values["mu1"] - 2 * m.values["sigma1"]} & {self.dt_param}<{m.values["mu1"] + 2 * m.values["sigma1"]}'
-            aoe_grp2 = self.dt_res_dict[
-                "aoe_grp2"
-            ] = f'{self.dt_param}>{m.values["mu2"] - 2 * m.values["sigma2"]} & {self.dt_param}<{m.values["mu2"] + 2 * m.values["sigma2"]}'
+            self.dt_res_dict["dt_fit"] = {"mus": mus, "sigmas": sigmas, "amps": amps}
 
-            aoe_pars, aoe_errs, _ = unbinned_aoe_fit(
-                final_df.query(aoe_grp1)[aoe_param], pdf=self.pdf, display=display
-            )
+            if len(mus) < 2:
+                log.info("Only 1 drift time peak found, no correction needed")
+                self.alpha = 0
 
-            self.dt_res_dict["aoe_fit1"] = {"pars": aoe_pars, "errs": aoe_errs}
+            else:
+                aoe_grp1 = self.dt_res_dict["aoe_grp1"] = (
+                    f"{self.dt_param}>{mus[0] - 2 * sigmas[0]} & {self.dt_param}<{mus[0] + 2 * sigmas[0]}"
+                )
+                aoe_grp2 = self.dt_res_dict["aoe_grp2"] = (
+                    f"{self.dt_param}>{mus[1] - 2 * sigmas[1]} & {self.dt_param}<{mus[1] + 2 * sigmas[1]}"
+                )
 
-            aoe_pars2, aoe_errs2, _ = unbinned_aoe_fit(
-                final_df.query(aoe_grp2)[aoe_param], pdf=self.pdf, display=display
-            )
+                aoe_pars, aoe_errs, _ = unbinned_aoe_fit(
+                    final_df.query(aoe_grp1)[aoe_param], pdf=self.pdf, display=display
+                )
 
-            self.dt_res_dict["aoe_fit2"] = {"pars": aoe_pars2, "errs": aoe_errs2}
+                self.dt_res_dict["aoe_fit1"] = {
+                    "pars": aoe_pars.to_dict(),
+                    "errs": aoe_errs.to_dict(),
+                }
 
-            try:
-                self.alpha = (aoe_pars["mu"] - aoe_pars2["mu"]) / (
-                    (m.values["mu2"] * aoe_pars2["mu"])
-                    - (m.values["mu1"] * aoe_pars["mu"])
+                aoe_pars2, aoe_errs2, _ = unbinned_aoe_fit(
+                    final_df.query(aoe_grp2)[aoe_param], pdf=self.pdf, display=display
                 )
-            except ZeroDivisionError:
-                self.alpha = 0
-            self.dt_res_dict["alpha"] = self.alpha
-            log.info(f"dtcorr successful alpha:{self.alpha}")
-            data["AoE_DTcorr"] = data[aoe_param] * (
-                1 + self.alpha * data[self.dt_param]
-            )
-        except:
+
+                self.dt_res_dict["aoe_fit2"] = {
+                    "pars": aoe_pars2.to_dict(),
+                    "errs": aoe_errs2.to_dict(),
+                }
+
+                try:
+                    self.alpha = (aoe_pars["mu"] - aoe_pars2["mu"]) / (
+                        (mus[0] * aoe_pars2["mu"]) - (mus[1] * aoe_pars["mu"])
+                    )
+                except ZeroDivisionError:
+                    self.alpha = 0
+                self.dt_res_dict["alpha"] = self.alpha
+                log.info(f"dtcorr successful alpha:{self.alpha}")
+
+        except BaseException as e:
+            if e == KeyboardInterrupt:
+                raise (e)
+            elif self.debug_mode:
+                raise (e)
             log.error("Drift time correction failed")
-            self.alpha = np.nan
+            self.alpha = 0
 
+        data[out_param] = data[aoe_param] * (1 + self.alpha * data[self.dt_param])
         self.update_cal_dicts(
             {
-                "AoE_DTcorr": {
+                out_param: {
                     "expression": f"{aoe_param}*(1+a*{self.dt_param})",
                     "parameters": {"a": self.alpha},
                 }
             }
         )
 
-    def AoEcorrection(self, data: pd.DataFrame, aoe_param: str, display: int = 0):
+    def energy_correction(
+        self,
+        data: pd.DataFrame,
+        aoe_param: str,
+        corrected_param="AoE_Corrected",
+        classifier_param="AoE_Classifier",
+        display: int = 0,
+    ):
         """
         Calculates the corrections needed for the energy dependence of the A/E.
         Does this by fitting the compton continuum in slices and then applies fits to the centroid and variance.
         """
 
         log.info("Starting A/E energy correction")
         self.energy_corr_res_dict = {}
 
-        comptBands = np.arange(900, 2350, self.comptBands_width)
+        compt_bands = np.arange(900, 2350, self.compt_bands_width)
         peaks = np.array(
             [1080, 1094, 1459, 1512, 1552, 1592, 1620, 1650, 1670, 1830, 2105]
         )
         allowed = np.array([], dtype=bool)
-        for i, band in enumerate(comptBands):
+        for band in compt_bands:
             allow = True
             for peak in peaks:
-                if (peak - 5) > band and (peak - 5) < (band + self.comptBands_width):
+                if (peak - 5) > band and (peak - 5) < (band + self.compt_bands_width):
                     allow = False
-                elif (peak + 5 > band) and (peak + 5) < (band + self.comptBands_width):
+                elif (peak + 5 > band) and (peak + 5) < (band + self.compt_bands_width):
                     allow = False
             allowed = np.append(allowed, allow)
-        comptBands = comptBands[allowed]
+        compt_bands = compt_bands[allowed]
 
         self.energy_corr_fits = pd.DataFrame(
             columns=[
                 "compt_bands",
                 "mean",
                 "mean_err",
                 "sigma",
@@ -1630,34 +1225,37 @@
             ],
             dtype=float,
         )
         try:
             select_df = data.query(f"{self.fit_selection} & {aoe_param}>0")
 
             # Fit each compton band
-            for band in comptBands:
+            for band in compt_bands:
                 try:
                     pars, errs, cov = unbinned_aoe_fit(
                         select_df.query(
-                            f"{self.cal_energy_param}>{band}&{self.cal_energy_param}< {self.comptBands_width+band}"
+                            f"{self.cal_energy_param}>{band}&{self.cal_energy_param}< {self.compt_bands_width+band}"
                         )[aoe_param],
                         pdf=self.pdf,
                         display=display,
                     )
 
-                    mean, mean_err = self.pdf.centroid(pars, errs, cov)
-                    sigma, sigma_err = self.pdf.width(pars, errs, cov)
+                    mean, mean_err = self.pdf.get_mu(pars, cov)
+                    sigma, sigma_err = self.pdf.get_fwhm(pars, cov)
+                    sigma = sigma / 2.355
+                    sigma_err = sigma_err / 2.355
 
                     self.energy_corr_fits = pd.concat(
                         [
                             self.energy_corr_fits,
                             pd.DataFrame(
                                 [
                                     {
-                                        "compt_bands": band + self.comptBands_width / 2,
+                                        "compt_bands": band
+                                        + self.compt_bands_width / 2,
                                         "mean": mean,
                                         "mean_err": mean_err,
                                         "sigma": sigma,
                                         "sigma_err": sigma_err,
                                         "ratio": pars["n_sig"] / pars["n_bkg"],
                                         "ratio_err": (pars["n_sig"] / pars["n_bkg"])
                                         * np.sqrt(
@@ -1666,15 +1264,19 @@
                                         ),
                                     }
                                 ]
                             ),
                         ]
                     )
 
-                except:
+                except BaseException as e:
+                    if e == KeyboardInterrupt:
+                        raise (e)
+                    elif self.debug_mode:
+                        raise (e)
                     self.energy_corr_fits = pd.concat(
                         [
                             self.energy_corr_fits,
                             pd.DataFrame(
                                 [
                                     {
                                         "compt_bands": band,
@@ -1720,15 +1322,15 @@
                         valid_fits["mean"]
                         - self.mean_func.func(valid_fits.index, *mu_pars)
                     )
                     ** 2
                 )
                 / valid_fits["mean_err"]
             )
-            dof_mu = len(valid_fits["mean"]) - len(pars)
+            dof_mu = len(valid_fits["mean"]) - len(mu_pars)
             p_val_mu = chi2.sf(csqr_mu, dof_mu)
             self.mean_fit_obj = m_mu
 
             # Fit sigma against energy
             p0_sig = self.sigma_func.guess(
                 valid_fits.index, valid_fits["sigma"], valid_fits["sigma_err"]
             )
@@ -1756,15 +1358,15 @@
                     ** 2
                 )
                 / valid_fits["sigma_err"]
             )
             dof_sig = len(valid_fits["sigma"]) - len(sig_pars)
             p_val_sig = chi2.sf(csqr_sig, dof_sig)
 
-            self.sigma_fit_obj = m_sig
+            self.SigmaFit_obj = m_sig
 
             # Get DEP fit
             n_sigma = 4
             peak = 1592
             sigma = self.eres_func(peak) / 2.355
             emin = peak - n_sigma * sigma
             emax = peak + n_sigma * sigma
@@ -1772,243 +1374,207 @@
                 dep_pars, dep_err, _ = unbinned_aoe_fit(
                     select_df.query(
                         f"{self.cal_energy_param}>{emin}&{self.cal_energy_param}<{emax}"
                     )[aoe_param],
                     pdf=self.pdf,
                     display=display,
                 )
-            except:
+            except BaseException as e:
+                if e == KeyboardInterrupt:
+                    raise (e)
+                elif self.debug_mode:
+                    raise (e)
+
                 dep_pars, dep_err, _ = return_nans(self.pdf)
 
-            data["AoE_Corrected"] = data[aoe_param] / self.mean_func.func(
+            data[corrected_param] = data[aoe_param] / self.mean_func.func(
                 data[self.cal_energy_param], *mu_pars
             )
-            data["AoE_Classifier"] = (data["AoE_Corrected"] - 1) / self.sigma_func.func(
+            data[classifier_param] = (data[corrected_param] - 1) / self.sigma_func.func(
                 data[self.cal_energy_param], *sig_pars
             )
             log.info("Finished A/E energy successful")
             log.info(f"mean pars are {mu_pars.to_dict()}")
             log.info(f"sigma pars are {sig_pars.to_dict()}")
-        except:
+
+        except BaseException as e:
+            if e == KeyboardInterrupt:
+                raise (e)
+            elif self.debug_mode:
+                raise (e)
             log.error("A/E energy correction failed")
             mu_pars, mu_errs, mu_cov = return_nans(self.mean_func.func)
             csqr_mu, dof_mu, p_val_mu = (np.nan, np.nan, np.nan)
             csqr_sig, dof_sig, p_val_sig = (np.nan, np.nan, np.nan)
             sig_pars, sig_errs, sig_cov = return_nans(self.sigma_func.func)
             dep_pars, dep_err, dep_cov = return_nans(self.pdf)
+            data[corrected_param] = data[aoe_param] * np.nan
+            data[classifier_param] = data[aoe_param] * np.nan
 
         self.energy_corr_res_dict["mean_fits"] = {
             "func": self.mean_func.__name__,
             "module": self.mean_func.__module__,
             "expression": self.mean_func.string_func("x"),
             "pars": mu_pars.to_dict(),
             "errs": mu_errs.to_dict(),
             "p_val_mu": p_val_mu,
             "csqr_mu": (csqr_mu, dof_mu),
         }
 
-        self.energy_corr_res_dict["sigma_fits"] = {
+        self.energy_corr_res_dict["SigmaFits"] = {
             "func": self.sigma_func.__name__,
             "module": self.sigma_func.__module__,
             "expression": self.sigma_func.string_func("x"),
             "pars": sig_pars.to_dict(),
             "errs": sig_errs.to_dict(),
             "p_val_mu": p_val_sig,
             "csqr_mu": (csqr_sig, dof_sig),
         }
 
         self.energy_corr_res_dict["dep_fit"] = {
-            "func": self.pdf.__name__,
-            "module": self.pdf.__module__,
+            "func": self.pdf.name,
             "pars": dep_pars.to_dict(),
             "errs": dep_err.to_dict(),
         }
 
         self.update_cal_dicts(
             {
-                "AoE_Corrected": {
+                corrected_param: {
                     "expression": f"{aoe_param}/({self.mean_func.string_func(self.cal_energy_param)})",
                     "parameters": mu_pars.to_dict(),
                 },
-                "AoE_Classifier": {
-                    "expression": f"(AoE_Corrected-1)/({self.sigma_func.string_func(self.cal_energy_param)})",
+                classifier_param: {
+                    "expression": f"({corrected_param}-1)/({self.sigma_func.string_func(self.cal_energy_param)})",
                     "parameters": sig_pars.to_dict(),
                 },
             }
         )
 
     def get_aoe_cut_fit(
         self,
         data: pd.DataFrame,
         aoe_param: str,
         peak: float,
         ranges: tuple,
         dep_acc: float,
+        output_cut_param: str = "AoE_Low_Cut",
         display: int = 1,
     ):
         """
         Determines A/E cut by sweeping through values and for each one fitting the DEP to determine how many events survive.
         Then interpolates to get cut value at desired DEP survival fraction (typically 90%)
         """
 
         log.info("Starting A/E low cut determination")
         self.low_cut_res_dict = {}
-        self.cut_fits = pd.DataFrame(columns=["cut_val", "sf", "sf_err"])
+        self.cut_fits = pd.DataFrame()
 
         min_range, max_range = ranges
-
+        erange = (peak - min_range, peak + max_range)
         try:
             select_df = data.query(
-                f"{self.fit_selection}&({self.cal_energy_param} > {peak - min_range}) & ({self.cal_energy_param} < {peak + max_range})"
+                f"{self.fit_selection}&({self.cal_energy_param} > {erange[0]}) & ({self.cal_energy_param} < {erange[1]})"
             )
 
             # if dep_correct is True:
             #     peak_aoe = (select_df[aoe_param] / dep_mu(select_df[self.cal_energy_param])) - 1
             #     peak_aoe = select_df[aoe_param] / sig_func(select_df[self.cal_energy_param])
 
-            cut_vals = np.arange(-8, 0, 0.2)
-            sfs = []
-            sf_errs = []
-            for cut_val in cut_vals:
-                sf, err, cut_pars, surv_pars = get_survival_fraction(
-                    select_df[self.cal_energy_param].to_numpy(),
-                    select_df[aoe_param].to_numpy(),
-                    cut_val,
-                    peak,
-                    self.eres_func(peak),
-                    guess_pars_cut=None,
-                    guess_pars_surv=None,
-                )
-                self.cut_fits = pd.concat(
-                    [
-                        self.cut_fits,
-                        pd.DataFrame(
-                            [
-                                {
-                                    "cut_val": cut_val,
-                                    "sf": sf,
-                                    "sf_err": err,
-                                }
-                            ]
-                        ),
-                    ]
-                )
-            self.cut_fits.set_index("cut_val", inplace=True)
+            self.cut_fits, _, _ = get_sf_sweep(
+                select_df[self.cal_energy_param],
+                select_df[aoe_param],
+                None,
+                peak,
+                self.eres_func(peak),
+                fit_range=erange,
+                dt_mask=None,
+                cut_range=(-8, 0),
+                n_samples=40,
+                mode="greater",
+                debug_mode=self.debug_mode,
+            )
+
             valid_fits = self.cut_fits.query(
-                f'sf_err<{(1.5 * np.nanpercentile(self.cut_fits["sf_err"],85))}&sf_err==sf_err'
+                f'sf_err<{(1.5 * np.nanpercentile(self.cut_fits["sf_err"], 85))}&sf_err==sf_err'
             )
 
             c = cost.LeastSquares(
                 valid_fits.index,
                 valid_fits["sf"],
                 valid_fits["sf_err"],
-                sigmoid_fit.func,
+                SigmoidFit.func,
             )
             c.loss = "soft_l1"
             m1 = Minuit(
                 c,
-                *sigmoid_fit.guess(
+                *SigmoidFit.guess(
                     valid_fits.index, valid_fits["sf"], valid_fits["sf_err"]
                 ),
             )
             m1.simplex().migrad()
             xs = np.arange(
                 np.nanmin(valid_fits.index), np.nanmax(valid_fits.index), 0.01
             )
-            p = sigmoid_fit.func(xs, *m1.values)
+            p = SigmoidFit.func(xs, *m1.values)
             self.cut_fit = {
-                "function": sigmoid_fit.__name__,
+                "function": SigmoidFit.__name__,
                 "pars": m1.values.to_dict(),
                 "errs": m1.errors.to_dict(),
             }
-            self.low_cut_val = round(xs[np.argmin(np.abs(p - (100 * self.dep_acc)))], 3)
+            self.low_cut_val = round(xs[np.argmin(np.abs(p - (100 * dep_acc)))], 3)
             log.info(f"Cut found at {self.low_cut_val}")
 
-            data["AoE_Low_Cut"] = data[aoe_param] > self.low_cut_val
+            data[output_cut_param] = data[aoe_param] > self.low_cut_val
             if self.dt_cut_param is not None:
-                data["AoE_Low_Cut"] = data["AoE_Low_Cut"] & (data[self.dt_cut_param])
-            data["AoE_Double_Sided_Cut"] = data["AoE_Low_Cut"] & (
-                data[aoe_param] < self.high_cut_val
-            )
-        except:
+                data[output_cut_param] = data[output_cut_param] & (
+                    data[self.dt_cut_param]
+                )
+        except BaseException as e:
+            if e == KeyboardInterrupt:
+                raise (e)
+            elif self.debug_mode:
+                raise (e)
             log.error("A/E cut determination failed")
             self.low_cut_val = np.nan
-        if self.dt_cut_param is not None and self.dt_cut_hard == True:
+            data[output_cut_param] = False
+        if self.dt_cut_param is not None and self.dt_cut_hard is True:
             self.update_cal_dicts(
                 {
-                    "AoE_Low_Cut": {
+                    output_cut_param: {
                         "expression": f"({aoe_param}>a) & ({self.dt_cut_param})",
                         "parameters": {"a": self.low_cut_val},
                     }
                 }
             )
         else:
             self.update_cal_dicts(
                 {
-                    "AoE_Low_Cut": {
+                    output_cut_param: {
                         "expression": f"({aoe_param}>a)",
                         "parameters": {"a": self.low_cut_val},
                     }
                 }
             )
-        self.update_cal_dicts(
-            {
-                "AoE_Double_Sided_Cut": {
-                    "expression": f"(a>{aoe_param}) & (AoE_Low_Cut)",
-                    "parameters": {"a": self.high_cut_val},
-                }
-            }
-        )
 
-    def get_results_dict(self):
-        return {
-            "cal_energy_param": self.cal_energy_param,
-            "dt_param": self.dt_param,
-            "rt_correction": self.dt_corr,
-            "pdf": self.pdf.__name__,
-            "1000-1300keV": self.timecorr_df.to_dict("index"),
-            "correction_fit_results": self.energy_corr_res_dict,
-            "low_cut": self.low_cut_val,
-            "high_cut": self.high_cut_val,
-            "low_side_sfs": self.low_side_sf.to_dict("index"),
-            "2_side_sfs": self.two_side_sf.to_dict("index"),
-        }
-
-    def fill_plot_dict(self, data, plot_dict={}):
-        for key, item in self.plot_options.items():
-            if item["options"] is not None:
-                plot_dict[key] = item["function"](self, data, **item["options"])
-            else:
-                plot_dict[key] = item["function"](self, data)
-        return plot_dict
-
-    def calibrate(self, df, initial_aoe_param):
-        self.aoe_timecorr(df, initial_aoe_param)
-        log.info("Finished A/E time correction")
-
-        if self.dt_corr == True:
-            aoe_param = "AoE_DTcorr"
-            self.drift_time_correction(df, "AoE_Timecorr")
-        else:
-            aoe_param = "AoE_Timecorr"
-
-        self.AoEcorrection(df, aoe_param)
-
-        self.get_aoe_cut_fit(df, "AoE_Classifier", 1592, (40, 20), 0.9)
-
-        aoe_param = "AoE_Classifier"
-        log.info("  Compute low side survival fractions: ")
-        self.low_side_sf = pd.DataFrame(columns=["peak", "sf", "sf_err"])
-        peaks_of_interest = [1592.5, 1620.5, 2039, 2103.53, 2614.50]
-        fit_widths = [(40, 25), (25, 40), (0, 0), (25, 40), (50, 50)]
-        self.low_side_peak_dfs = {}
+    def calculate_survival_fractions_sweep(
+        self,
+        data,
+        aoe_param,
+        peaks,
+        fit_widths,
+        n_samples=26,
+        cut_range=(-5, 5),
+        mode="greater",
+    ):
+        sfs = pd.DataFrame()
+        peak_dfs = {}
 
-        for i, peak in enumerate(peaks_of_interest):
+        for i, peak in enumerate(peaks):
             try:
-                select_df = df.query(
+                select_df = data.query(
                     f"{self.selection_string}&{aoe_param}=={aoe_param}"
                 )
                 fwhm = self.eres_func(peak)
                 if peak == 2039:
                     emin = 2 * fwhm
                     emax = 2 * fwhm
                     peak_df = select_df.query(
@@ -2017,127 +1583,278 @@
 
                     cut_df, sf, sf_err = compton_sf_sweep(
                         peak_df[self.cal_energy_param].to_numpy(),
                         peak_df[aoe_param].to_numpy(),
                         self.low_cut_val,
                         peak,
                         fwhm,
-                        dt_mask=peak_df[self.dt_cut_param].to_numpy()
-                        if self.dt_cut_param is not None
-                        else None,
+                        cut_range=cut_range,
+                        n_samples=n_samples,
+                        mode=mode,
+                        dt_mask=(
+                            peak_df[self.dt_cut_param].to_numpy()
+                            if self.dt_cut_param is not None
+                            else None
+                        ),
                     )
-                    self.low_side_sf = pd.concat(
+                    sfs = pd.concat(
                         [
-                            self.low_side_sf,
+                            sfs,
                             pd.DataFrame([{"peak": peak, "sf": sf, "sf_err": sf_err}]),
                         ]
                     )
-                    self.low_side_peak_dfs[peak] = cut_df
+                    peak_dfs[peak] = cut_df
                 else:
                     emin, emax = fit_widths[i]
+                    fit_range = (peak - emin, peak + emax)
                     peak_df = select_df.query(
                         f"({self.cal_energy_param}>{peak-emin})&({self.cal_energy_param}<{peak+emax})"
                     )
                     cut_df, sf, sf_err = get_sf_sweep(
                         peak_df[self.cal_energy_param].to_numpy(),
                         peak_df[aoe_param].to_numpy(),
                         self.low_cut_val,
                         peak,
                         fwhm,
-                        dt_mask=peak_df[self.dt_cut_param].to_numpy()
-                        if self.dt_cut_param is not None
-                        else None,
+                        fit_range=fit_range,
+                        cut_range=cut_range,
+                        n_samples=n_samples,
+                        mode=mode,
+                        dt_mask=(
+                            peak_df[self.dt_cut_param].to_numpy()
+                            if self.dt_cut_param is not None
+                            else None
+                        ),
+                        debug_mode=self.debug_mode,
                     )
-                    self.low_side_sf = pd.concat(
+
+                    cut_df = cut_df.query(
+                        f'sf_err<5*{np.nanpercentile(cut_df["sf_err"], 50)}& sf_err==sf_err & sf<=100'
+                    )
+
+                    sfs = pd.concat(
                         [
-                            self.low_side_sf,
+                            sfs,
                             pd.DataFrame([{"peak": peak, "sf": sf, "sf_err": sf_err}]),
                         ]
                     )
-                    self.low_side_peak_dfs[peak] = cut_df
+                    peak_dfs[peak] = cut_df
                 log.info(f"{peak}keV: {sf:2.1f} +/- {sf_err:2.1f} %")
-            except:
-                self.low_side_sf = pd.concat(
+            except BaseException as e:
+                if e == KeyboardInterrupt:
+                    raise (e)
+                elif self.debug_mode:
+                    raise (e)
+                sfs = pd.concat(
                     [
-                        self.low_side_sf,
+                        sfs,
                         pd.DataFrame([{"peak": peak, "sf": np.nan, "sf_err": np.nan}]),
                     ]
                 )
                 log.error(
-                    f"A/E Low side Survival fraction determination failed for {peak} peak"
+                    f"A/E Survival fraction sweep determination failed for {peak} peak"
                 )
-        self.low_side_sf.set_index("peak", inplace=True)
+        sfs.set_index("peak", inplace=True)
+        return sfs, peak_dfs
 
-        self.two_side_sf = pd.DataFrame(columns=["peak", "sf", "sf_err"])
-        log.info("Calculating 2 sided cut sfs")
-        for i, peak in enumerate(peaks_of_interest):
+    def calculate_survival_fractions(
+        self, data, aoe_param, peaks, fit_widths, mode="greater"
+    ):
+        sfs = pd.DataFrame()
+        for i, peak in enumerate(peaks):
             fwhm = self.eres_func(peak)
             try:
                 if peak == 2039:
                     emin = 2 * fwhm
                     emax = 2 * fwhm
-                    peak_df = select_df.query(
+                    peak_df = data.query(
                         f"({self.cal_energy_param}>{peak-emin})&({self.cal_energy_param}<{peak+emax})"
                     )
 
                     sf_dict = compton_sf(
                         peak_df[aoe_param].to_numpy(),
                         self.low_cut_val,
                         self.high_cut_val,
-                        dt_mask=peak_df[self.dt_cut_param].to_numpy()
-                        if self.dt_cut_param is not None
-                        else None,
+                        mode=mode,
+                        dt_mask=(
+                            peak_df[self.dt_cut_param].to_numpy()
+                            if self.dt_cut_param is not None
+                            else None
+                        ),
                     )
                     sf = sf_dict["sf"]
                     sf_err = sf_dict["sf_err"]
-                    self.two_side_sf = pd.concat(
+                    sfs = pd.concat(
                         [
-                            self.two_side_sf,
+                            sfs,
                             pd.DataFrame([{"peak": peak, "sf": sf, "sf_err": sf_err}]),
                         ]
                     )
                 else:
                     emin, emax = fit_widths[i]
-                    peak_df = select_df.query(
+                    fit_range = (peak - emin, peak + emax)
+                    peak_df = data.query(
                         f"({self.cal_energy_param}>{peak-emin})&({self.cal_energy_param}<{peak+emax})"
                     )
                     sf, sf_err, _, _ = get_survival_fraction(
                         peak_df[self.cal_energy_param].to_numpy(),
                         peak_df[aoe_param].to_numpy(),
                         self.low_cut_val,
                         peak,
                         fwhm,
+                        fit_range=fit_range,
+                        mode=mode,
                         high_cut=self.high_cut_val,
-                        dt_mask=peak_df[self.dt_cut_param].to_numpy()
-                        if self.dt_cut_param is not None
-                        else None,
+                        dt_mask=(
+                            peak_df[self.dt_cut_param].to_numpy()
+                            if self.dt_cut_param is not None
+                            else None
+                        ),
                     )
-                    self.two_side_sf = pd.concat(
+                    sfs = pd.concat(
                         [
-                            self.two_side_sf,
+                            sfs,
                             pd.DataFrame([{"peak": peak, "sf": sf, "sf_err": sf_err}]),
                         ]
                     )
                 log.info(f"{peak}keV: {sf:2.1f} +/- {sf_err:2.1f} %")
 
-            except:
-                self.two_side_sf = pd.concat(
+            except BaseException as e:
+                if e == KeyboardInterrupt:
+                    raise (e)
+                elif self.debug_mode:
+                    raise (e)
+                sfs = pd.concat(
                     [
-                        self.two_side_sf,
+                        sfs,
                         pd.DataFrame([{"peak": peak, "sf": np.nan, "sf_err": np.nan}]),
                     ]
                 )
-                log.error(
-                    f"A/E two side Survival fraction determination failed for {peak} peak"
+                log.error(f"A/E survival fraction determination failed for {peak} peak")
+        sfs.set_index("peak", inplace=True)
+        return sfs
+
+    def calibrate(
+        self,
+        df,
+        initial_aoe_param,
+        peaks_of_interest=None,
+        fit_widths=None,
+        cut_peak_idx=0,
+        dep_acc=0.9,
+        sf_nsamples=11,
+        sf_cut_range=(-5, 5),
+    ):
+        if peaks_of_interest is None:
+            peaks_of_interest = [1592.5, 1620.5, 2039, 2103.53, 2614.50]
+        if fit_widths is None:
+            fit_widths = [(40, 25), (25, 40), (0, 0), (25, 40), (50, 50)]
+
+        self.time_correction(df, initial_aoe_param, output_name="AoE_Timecorr")
+
+        if self.dt_corr is True:
+            aoe_param = "AoE_DTcorr"
+            self.drift_time_correction(df, "AoE_Timecorr", out_param=aoe_param)
+        else:
+            aoe_param = "AoE_Timecorr"
+
+        self.energy_correction(
+            df,
+            aoe_param,
+            corrected_param="AoE_Corrected",
+            classifier_param="AoE_Classifier",
+        )
+
+        self.get_aoe_cut_fit(
+            df,
+            "AoE_Classifier",
+            peaks_of_interest[cut_peak_idx],
+            fit_widths[cut_peak_idx],
+            dep_acc,
+            output_cut_param="AoE_Low_Cut",
+        )
+
+        df["AoE_Double_Sided_Cut"] = df["AoE_Low_Cut"] & (
+            df["AoE_Classifier"] < self.high_cut_val
+        )
+
+        if self.dt_cut_param is not None and self.dt_cut_hard is True:
+            self.update_cal_dicts(
+                {
+                    "AoE_High_Side_Cut": {
+                        "expression": f"(a>AoE_Classifier)& ({self.dt_cut_param})",
+                        "parameters": {"a": self.high_cut_val},
+                    }
+                }
+            )
+        else:
+            self.update_cal_dicts(
+                {
+                    "AoE_High_Side_Cut": {
+                        "expression": "(a>AoE_Classifier)",
+                        "parameters": {"a": self.high_cut_val},
+                    }
+                }
+            )
+
+        self.update_cal_dicts(
+            {
+                "AoE_Double_Sided_Cut": {
+                    "expression": "(AoE_High_Side_Cut) & (AoE_Low_Cut)",
+                    "parameters": {},
+                }
+            }
+        )
+
+        log.info("Compute low side survival fractions: ")
+        (
+            self.low_side_sfs,
+            self.low_side_peak_dfs,
+        ) = self.calculate_survival_fractions_sweep(
+            df,
+            "AoE_Classifier",
+            peaks_of_interest,
+            fit_widths,
+            n_samples=sf_nsamples,
+            cut_range=sf_cut_range,
+            mode="greater",
+        )
+
+        log.info("Compute 2 side survival fractions: ")
+        self.two_side_sfs = self.calculate_survival_fractions(
+            df, "AoE_Classifier", peaks_of_interest, fit_widths, mode="greater"
+        )
+
+        if re.match(r"(\d{8})T(\d{6})Z", list(self.cal_dicts)[0]):
+            self.low_side_sfs_by_run = {}
+            self.two_side_sfs_by_run = {}
+            for tstamp in self.cal_dicts:
+                log.info(f"Compute survival fractions for {tstamp}: ")
+                self.low_side_sfs_by_run[tstamp] = self.calculate_survival_fractions(
+                    df.query(f"run_timestamp == '{tstamp}'"),
+                    "AoE_Classifier",
+                    peaks_of_interest,
+                    fit_widths,
+                    mode="greater",
+                )
+
+                self.two_side_sfs_by_run[tstamp] = self.calculate_survival_fractions(
+                    df.query(f"run_timestamp == '{tstamp}'"),
+                    "AoE_Classifier",
+                    peaks_of_interest,
+                    fit_widths,
+                    mode="greater",
                 )
-        self.two_side_sf.set_index("peak", inplace=True)
+        else:
+            self.low_side_sfs_by_run = None
+            self.two_side_sfs_by_run = None
 
 
 def plot_aoe_mean_time(
-    aoe_class, data, time_param="AoE_Timecorr", figsize=[12, 8], fontsize=12
+    aoe_class, data, time_param="AoE_Timecorr", figsize=(12, 8), fontsize=12
 ):
     plt.rcParams["figure.figsize"] = figsize
     plt.rcParams["font.size"] = fontsize
     fig, ax = plt.subplots(1, 1)
     try:
         ax.errorbar(
             [
@@ -2177,56 +1894,56 @@
                 for tstamp in aoe_class.cal_dicts
             ],
             y1=np.array(grouped_means) - 0.4 * np.array(aoe_class.timecorr_df["res"]),
             y2=np.array(grouped_means) + 0.4 * np.array(aoe_class.timecorr_df["res"]),
             color="yellow",
             alpha=0.2,
         )
-    except:
+    except Exception:
         pass
     ax.set_xlabel("time")
     ax.set_ylabel("A/E mean")
-    myFmt = mdates.DateFormatter("%b %d")
-    ax.xaxis.set_major_formatter(myFmt)
+    myfmt = mdates.DateFormatter("%b %d")
+    ax.xaxis.set_major_formatter(myfmt)
     plt.close()
     return fig
 
 
 def plot_aoe_res_time(
-    aoe_class, data, time_param="AoE_Timecorr", figsize=[12, 8], fontsize=12
+    aoe_class, data, time_param="AoE_Timecorr", figsize=(12, 8), fontsize=12
 ):
     plt.rcParams["figure.figsize"] = figsize
     plt.rcParams["font.size"] = fontsize
     fig, ax = plt.subplots(1, 1)
     try:
         ax.errorbar(
             [
                 datetime.strptime(tstamp, "%Y%m%dT%H%M%SZ")
                 for tstamp in aoe_class.timecorr_df.index
             ],
             aoe_class.timecorr_df["res"],
             yerr=aoe_class.timecorr_df["res_err"],
             linestyle=" ",
         )
-    except:
+    except Exception:
         pass
     ax.set_xlabel("time")
     ax.set_ylabel("A/E res")
-    myFmt = mdates.DateFormatter("%b %d")
-    ax.xaxis.set_major_formatter(myFmt)
+    myfmt = mdates.DateFormatter("%b %d")
+    ax.xaxis.set_major_formatter(myfmt)
     plt.close()
     return fig
 
 
 def drifttime_corr_plot(
     aoe_class,
     data,
     aoe_param="AoE_Timecorr",
     aoe_param_corr="AoE_DTcorr",
-    figsize=[12, 8],
+    figsize=(12, 8),
     fontsize=12,
 ):
     plt.rcParams["figure.figsize"] = figsize
     plt.rcParams["font.size"] = fontsize
 
     fig = plt.figure()
 
@@ -2235,46 +1952,50 @@
             f"{aoe_class.fit_selection}&{aoe_class.cal_energy_param}>1582&{aoe_class.cal_energy_param}<1602&{aoe_class.cal_energy_param}=={aoe_class.cal_energy_param}&{aoe_param}=={aoe_param}"
         )
         final_df = dep_events.query(aoe_class.dt_res_dict["final_selection"])
 
         plt.subplot(2, 2, 1)
         aoe_pars = aoe_class.dt_res_dict["aoe_fit1"]["pars"]
 
-        xs = np.linspace(aoe_pars["lower_range"], aoe_pars["upper_range"], 100)
+        xs = np.linspace(aoe_pars["x_lo"], aoe_pars["x_hi"], 100)
         counts, aoe_bins, bars = plt.hist(
             final_df.query(
-                f'{aoe_class.dt_res_dict["aoe_grp1"]}&({aoe_param}<{aoe_pars["upper_range"]})&({aoe_param}>{aoe_pars["lower_range"]})'
+                f'{aoe_class.dt_res_dict["aoe_grp1"]}&({aoe_param}<{aoe_pars["x_hi"]})&({aoe_param}>{aoe_pars["x_lo"]})'
             )[aoe_param],
             bins=400,
             histtype="step",
             label="data",
         )
         dx = np.diff(aoe_bins)
-        plt.plot(xs, aoe_class.pdf.pdf(xs, *aoe_pars) * dx[0], label="full fit")
-        sig, bkg = aoe_class.pdf.pdf(xs, *aoe_pars[:-1], True)
+        plt.plot(xs, aoe_class.pdf.get_pdf(xs, *aoe_pars) * dx[0], label="full fit")
+        aoe_class.pdf.components = True
+        sig, bkg = aoe_class.pdf.get_pdf(xs, *aoe_pars)
+        aoe_class.pdf.components = False
         plt.plot(xs, sig * dx[0], label="peak fit")
         plt.plot(xs, bkg * dx[0], label="bkg fit")
         plt.legend(loc="upper left")
         plt.xlabel("A/E")
         plt.ylabel("counts")
 
         aoe_pars2 = aoe_class.dt_res_dict["aoe_fit2"]["pars"]
         plt.subplot(2, 2, 2)
-        xs = np.linspace(aoe_pars2["lower_range"], aoe_pars2["upper_range"], 100)
+        xs = np.linspace(aoe_pars2["x_lo"], aoe_pars2["x_hi"], 100)
         counts, aoe_bins2, bars = plt.hist(
             final_df.query(
-                f'{aoe_class.dt_res_dict["aoe_grp2"]}&({aoe_param}<{aoe_pars2["upper_range"]})&({aoe_param}>{aoe_pars2["lower_range"]})'
+                f'{aoe_class.dt_res_dict["aoe_grp2"]}&({aoe_param}<{aoe_pars2["x_hi"]})&({aoe_param}>{aoe_pars2["x_lo"]})'
             )[aoe_param],
             bins=400,
             histtype="step",
             label="Data",
         )
         dx = np.diff(aoe_bins2)
-        plt.plot(xs, aoe_class.pdf.pdf(xs, *aoe_pars2) * dx[0], label="full fit")
-        sig, bkg = aoe_class.pdf.pdf(xs, *aoe_pars2[:-1], True)
+        plt.plot(xs, aoe_class.pdf.get_pdf(xs, *aoe_pars2) * dx[0], label="full fit")
+        aoe_class.pdf.components = True
+        sig, bkg = aoe_class.pdf.get_pdf(xs, *aoe_pars2)
+        aoe_class.pdf.components = False
         plt.plot(xs, sig * dx[0], label="peak fit")
         plt.plot(xs, bkg * dx[0], label="bkg fit")
         plt.legend(loc="upper left")
         plt.xlabel("A/E")
         plt.ylabel("counts")
 
         hist, bins, var = pgh.get_hist(
@@ -2284,33 +2005,26 @@
                 np.nanmin(final_df[aoe_class.dt_param]),
                 np.nanmax(final_df[aoe_class.dt_param]),
             ),
         )
 
         plt.subplot(2, 2, 3)
         plt.step(pgh.get_bin_centers(bins), hist, label="data")
-        plt.plot(
-            pgh.get_bin_centers(bins),
-            drift_time_distribution.pdf(
-                pgh.get_bin_centers(bins), **aoe_class.dt_res_dict["dt_guess"]
-            )
-            * np.diff(bins)[0],
-            label="Guess",
-        )
-        plt.plot(
-            pgh.get_bin_centers(bins),
-            drift_time_distribution.pdf(
-                pgh.get_bin_centers(bins), *aoe_class.dt_res_dict["dt_fit"]["pars"]
+
+        mus = aoe_class.dt_res_dict["dt_fit"]["mus"]
+        sigmas = aoe_class.dt_res_dict["dt_fit"]["sigmas"]
+        amps = aoe_class.dt_res_dict["dt_fit"]["amps"]
+
+        for mu, sigma, amp in zip(mus, sigmas, amps):
+            plt.plot(
+                pgh.get_bin_centers(bins),
+                gaussian.get_pdf(pgh.get_bin_centers(bins), mu, sigma) * amp,
             )
-            * np.diff(bins)[0],
-            label="fit",
-        )
         plt.xlabel("drift time (ns)")
         plt.ylabel("Counts")
-        plt.legend(loc="upper left")
 
         plt.subplot(2, 2, 4)
         bins = np.linspace(
             np.nanpercentile(final_df[aoe_param], 1),
             np.nanpercentile(final_df[aoe_param_corr], 99),
             200,
         )
@@ -2319,30 +2033,30 @@
             final_df[aoe_param_corr], bins=bins, histtype="step", label="corrected"
         )
         plt.xlabel("A/E")
         plt.ylabel("counts")
         plt.legend(loc="upper left")
         plt.tight_layout()
         plt.xlim(bins[0], bins[-1])
-    except:
+    except Exception:
         pass
     plt.close()
     return fig
 
 
 def plot_compt_bands_overlayed(
     aoe_class,
     data,
     eranges: list[tuple],
     aoe_param="AoE_Timecorr",
     aoe_range: list[float] = None,
     title="Compton Bands",
     density=True,
     n_bins=50,
-    figsize=[12, 8],
+    figsize=(12, 8),
     fontsize=12,
 ) -> None:
     """
     Function to plot various compton bands to check energy dependence and corrections
     """
     plt.rcParams["figure.figsize"] = figsize
     plt.rcParams["font.size"] = fontsize
@@ -2364,15 +2078,15 @@
             plt.hist(
                 select_df[aoe_param],
                 bins=bins,
                 histtype="step",
                 label=f"{erange[0]}-{erange[1]}",
                 density=density,
             )
-        except:
+        except Exception:
             pass
     plt.ylabel("counts")
     plt.xlabel(aoe_param)
     plt.title(title)
     plt.legend(loc="upper left")
     plt.close()
     return fig
@@ -2380,17 +2094,17 @@
 
 def plot_dt_dep(
     aoe_class,
     data,
     eranges: list[tuple],
     titles: list = None,
     aoe_param="AoE_Timecorr",
-    bins=[200, 100],
+    bins=(200, 100),
     dt_max=2000,
-    figsize=[12, 8],
+    figsize=(12, 8),
     fontsize=12,
 ) -> None:
     """
     Function to produce 2d histograms of A/E against drift time to check dependencies
     """
     plt.rcParams["figure.figsize"] = figsize
     plt.rcParams["font.size"] = fontsize
@@ -2419,31 +2133,31 @@
             )
             plt.ylabel("drift time (ns)")
             plt.xlabel("A/E")
             if titles is None:
                 plt.title(f"{erange[0]}-{erange[1]}")
             else:
                 plt.title(titles[i])
-        except:
+        except Exception:
             pass
     plt.tight_layout()
     plt.close()
     return fig
 
 
-def plot_mean_fit(aoe_class, data, figsize=[12, 8], fontsize=12) -> plt.figure:
+def plot_mean_fit(aoe_class, data, figsize=(12, 8), fontsize=12) -> plt.figure:
     plt.rcParams["figure.figsize"] = figsize
     plt.rcParams["font.size"] = fontsize
     fig, (ax1, ax2) = plt.subplots(2, 1, sharex=True)
     try:
         ax1.errorbar(
             aoe_class.energy_corr_fits.index,
             aoe_class.energy_corr_fits["mean"],
             yerr=aoe_class.energy_corr_fits["mean_err"],
-            xerr=aoe_class.comptBands_width / 2,
+            xerr=aoe_class.compt_bands_width / 2,
             label="data",
             linestyle=" ",
         )
 
         ax1.plot(
             aoe_class.energy_corr_fits.index.to_numpy(),
             aoe_class.mean_func.func(
@@ -2492,42 +2206,40 @@
             )
             / aoe_class.mean_func.func(
                 1592, **aoe_class.energy_corr_res_dict["mean_fits"]["pars"]
             ),
             lw=1,
             c="g",
         )
-    except:
+    except Exception:
         pass
     ax2.set_ylabel("residuals %", ha="right", y=1)
     ax2.set_xlabel("energy (keV)", ha="right", x=1)
     plt.tight_layout()
     plt.close()
     return fig
 
 
-def plot_sigma_fit(aoe_class, data, figsize=[12, 8], fontsize=12) -> plt.figure:
+def plot_sigma_fit(aoe_class, data, figsize=(12, 8), fontsize=12) -> plt.figure:
     plt.rcParams["figure.figsize"] = figsize
     plt.rcParams["font.size"] = fontsize
 
     fig, (ax1, ax2) = plt.subplots(2, 1, sharex=True)
     try:
         ax1.errorbar(
             aoe_class.energy_corr_fits.index,
             aoe_class.energy_corr_fits["sigma"],
             yerr=aoe_class.energy_corr_fits["sigma_err"],
-            xerr=aoe_class.comptBands_width / 2,
+            xerr=aoe_class.compt_bands_width / 2,
             label="data",
             linestyle=" ",
         )
-        sig_pars = aoe_class.energy_corr_res_dict["sigma_fits"]["pars"]
-        if aoe_class.sigma_func == sigma_fit:
+        sig_pars = aoe_class.energy_corr_res_dict["SigmaFits"]["pars"]
+        if aoe_class.sigma_func == SigmaFit:
             label = f'sqrt model: \nsqrt({sig_pars["a"]:1.4f}+({sig_pars["b"]:1.1f}/E)^{sig_pars["c"]:1.1f})'
-        elif aoe_class.sigma_func == sigma_fit_quadratic:
-            label = f'quad model: \n({sig_pars["a"]:1.4f}+({sig_pars["b"]:1.6f}*E)+\n({sig_pars["c"]:1.6f}*E)^2)'
         else:
             raise ValueError("unknown sigma function")
         ax1.plot(
             aoe_class.energy_corr_fits.index.to_numpy(),
             aoe_class.sigma_func.func(
                 aoe_class.energy_corr_fits.index.to_numpy(), **sig_pars
             ),
@@ -2563,69 +2275,71 @@
                 aoe_class.energy_corr_res_dict["dep_fit"]["pars"]["sigma"]
                 - aoe_class.sigma_func.func(1592, **sig_pars)
             )
             / aoe_class.sigma_func.func(1592, **sig_pars),
             lw=1,
             c="g",
         )
-    except:
+    except Exception:
         pass
     ax2.set_ylabel("residuals", ha="right", y=1)
     ax2.set_xlabel("energy (keV)", ha="right", x=1)
     plt.tight_layout()
     plt.close()
     return fig
 
 
-def plot_cut_fit(aoe_class, data, figsize=[12, 8], fontsize=12) -> plt.figure:
+def plot_cut_fit(
+    aoe_class, data, dep_acc=0.9, figsize=(12, 8), fontsize=12
+) -> plt.figure:
     plt.rcParams["figure.figsize"] = figsize
     plt.rcParams["font.size"] = fontsize
     fig = plt.figure()
     try:
         plt.errorbar(
             aoe_class.cut_fits.index,
             aoe_class.cut_fits["sf"],
             yerr=aoe_class.cut_fits["sf_err"],
             linestyle=" ",
         )
 
         plt.plot(
             aoe_class.cut_fits.index.to_numpy(),
-            sigmoid_fit.func(
+            SigmoidFit.func(
                 aoe_class.cut_fits.index.to_numpy(), **aoe_class.cut_fit["pars"]
             ),
         )
         plt.hlines(
-            (100 * aoe_class.dep_acc),
+            (100 * dep_acc),
             -8.1,
             aoe_class.low_cut_val,
             color="red",
             linestyle="--",
         )
         plt.vlines(
             aoe_class.low_cut_val,
             np.nanmin(aoe_class.cut_fits["sf"]) * 0.9,
-            (100 * aoe_class.dep_acc),
+            (100 * dep_acc),
             color="red",
             linestyle="--",
         )
         plt.xlim([-8.1, 0.1])
         vals, labels = plt.yticks()
         plt.yticks(vals, [f"{x:,.0f} %" for x in vals])
         plt.ylim([np.nanmin(aoe_class.cut_fits["sf"]) * 0.9, 102])
-    except:
+    except Exception:
         pass
     plt.xlabel("cut value")
     plt.ylabel("survival percentage")
     plt.close()
     return fig
 
 
 def plot_survival_fraction_curves(
-    aoe_class, data, figsize=[12, 8], fontsize=12
+    aoe_class, data, figsize=(12, 8), fontsize=12
 ) -> plt.figure:
     plt.rcParams["figure.figsize"] = figsize
     plt.rcParams["font.size"] = fontsize
 
     fig = plt.figure()
     try:
         plt.vlines(
@@ -2638,19 +2352,19 @@
 
         for peak, survival_df in aoe_class.low_side_peak_dfs.items():
             try:
                 plt.errorbar(
                     survival_df.index,
                     survival_df["sf"],
                     yerr=survival_df["sf_err"],
-                    label=f'{get_peak_label(peak)} {peak} keV: {aoe_class.low_side_sf.loc[peak]["sf"]:2.1f} +/- {aoe_class.low_side_sf.loc[peak]["sf_err"]:2.1f} %',
+                    label=f'{get_peak_label(peak)} {peak} keV: {aoe_class.low_side_sfs.loc[peak]["sf"]:2.1f} +/- {aoe_class.low_side_sfs.loc[peak]["sf_err"]:2.1f} %',
                 )
-            except:
+            except Exception:
                 pass
-    except:
+    except Exception:
         pass
     vals, labels = plt.yticks()
     plt.yticks(vals, [f"{x:,.0f} %" for x in vals])
     plt.legend(loc="upper right")
     plt.xlabel("cut value")
     plt.ylabel("survival percentage")
     plt.ylim([0, 105])
@@ -2661,15 +2375,15 @@
 def plot_spectra(
     aoe_class,
     data,
     xrange=(900, 3000),
     n_bins=2101,
     xrange_inset=(1580, 1640),
     n_bins_inset=200,
-    figsize=[12, 8],
+    figsize=(12, 8),
     fontsize=12,
 ) -> plt.figure:
     plt.rcParams["figure.figsize"] = figsize
     plt.rcParams["font.size"] = fontsize
 
     fig, ax = plt.subplots()
     try:
@@ -2732,27 +2446,27 @@
         axins.hist(
             select_df.query(f"{aoe_class.selection_string} & (~AoE_Double_Sided_Cut)")[
                 aoe_class.cal_energy_param
             ],
             bins=bins,
             histtype="step",
         )
-    except:
+    except Exception:
         pass
     ax.set_xlim(xrange)
     ax.set_yscale("log")
     plt.xlabel("energy (keV)")
     plt.ylabel("counts")
     plt.legend(loc="upper left")
     plt.close()
     return fig
 
 
 def plot_sf_vs_energy(
-    aoe_class, data, xrange=(900, 3000), n_bins=701, figsize=[12, 8], fontsize=12
+    aoe_class, data, xrange=(900, 3000), n_bins=701, figsize=(12, 8), fontsize=12
 ) -> plt.figure:
     plt.rcParams["figure.figsize"] = figsize
     plt.rcParams["font.size"] = fontsize
 
     fig = plt.figure()
     try:
         bins = np.linspace(xrange[0], xrange[1], n_bins)
@@ -2765,15 +2479,15 @@
         counts, bins, _ = pgh.get_hist(
             data.query(aoe_class.selection_string)[aoe_class.cal_energy_param],
             bins=bins,
         )
         survival_fracs = counts_pass / (counts + 10**-99)
 
         plt.step(pgh.get_bin_centers(bins_pass), 100 * survival_fracs)
-    except:
+    except Exception:
         pass
     plt.ylim([0, 100])
     vals, labels = plt.yticks()
     plt.yticks(vals, [f"{x:,.0f} %" for x in vals])
     plt.xlabel("energy (keV)")
     plt.ylabel("survival percentage")
     plt.close()
@@ -2784,15 +2498,15 @@
     aoe_class,
     data,
     aoe_param="AoE_Classifier",
     xrange=(900, 3000),
     yrange=(-50, 10),
     xn_bins=700,
     yn_bins=500,
-    figsize=[12, 8],
+    figsize=(12, 8),
     fontsize=12,
 ) -> plt.figure:
     plt.rcParams["figure.figsize"] = figsize
     plt.rcParams["font.size"] = fontsize
 
     fig = plt.figure()
     try:
@@ -2801,15 +2515,15 @@
             data.query(aoe_class.selection_string)[aoe_param],
             bins=[
                 np.linspace(xrange[0], xrange[1], xn_bins),
                 np.linspace(yrange[0], yrange[1], yn_bins),
             ],
             norm=LogNorm(),
         )
-    except:
+    except Exception:
         pass
     plt.xlabel("energy (keV)")
     plt.ylabel(aoe_param)
     plt.xlim(xrange)
     plt.ylim(yrange)
     plt.close()
     return fig
```

### Comparing `pygama-1.6.0a2/src/pygama/pargen/dplms_ge_dict.py` & `pygama-2.0.0a1/src/pygama/pargen/dplms_ge_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,127 +1,118 @@
 """
 This module is for creating dplms dictionary for ge processing
 """
 
 from __future__ import annotations
 
 import itertools
-import json
 import logging
-import os
 import time
 
 import matplotlib.pyplot as plt
 import numpy as np
-from lgdo import Array, Table, lh5
+from lgdo import Table, lh5
 from scipy.signal import convolve, convolve2d
+from scipy.stats import chi2
 
-from pygama.math.histogram import get_hist
-from pygama.math.peak_fitting import (
-    extended_gauss_step_pdf,
-    extended_radford_pdf,
-    gauss_step_pdf,
-    radford_pdf,
-)
-from pygama.pargen.cuts import generate_cuts, get_cut_indexes
+from pygama.math.distributions import gauss_on_step
+from pygama.pargen.data_cleaning import generate_cuts
 from pygama.pargen.dsp_optimize import run_one_dsp
-from pygama.pargen.energy_optimisation import fom_FWHM_with_dt_corr_fit
+from pygama.pargen.energy_optimisation import fom_fwhm_with_alpha_fit
 
 log = logging.getLogger(__name__)
 sto = lh5.LH5Store()
 
 
 def dplms_ge_dict(
-    lh5_path: str,
     raw_fft: Table,
     raw_cal: Table,
     dsp_config: dict,
     par_dsp: dict,
-    par_dsp_lh5: str,
     dplms_dict: dict,
     decay_const: float = 0,
     ene_par: str = "dplmsEmax",
+    p_val_lim: float = 10**-20,
     display: int = 0,
 ) -> dict:
     """
     This function calculates the dplms dictionary for HPGe detectors.
 
     Parameters
     ----------
-    lh5_path
-        Name of channel to process, should be name of lh5 group in raw files
     fft_files
         table with fft data
     raw_cal
         table with cal data
     dsp_config
         dsp config file
     par_dsp
         Dictionary with db parameters for dsp processing
-    par_dsp_lh5
-        Path for saving dplms coefficients
     dplms_dict
         Dictionary with various parameters
 
     Returns
     -------
     out_dict
     """
 
     t0 = time.time()
-    log.info(f"\nSelecting baselines")
+    log.info("Selecting baselines")
+
+    dsp_fft = run_one_dsp(raw_fft, dsp_config, db_dict=par_dsp)
+
+    cut_dict = generate_cuts(dsp_fft, cut_dict=dplms_dict["bls_cut_pars"])
+    log.debug(f"Cuts are {cut_dict}")
+    idxs = np.full(len(dsp_fft), True, dtype=bool)
+    for outname, info in cut_dict.items():
+        outcol = dsp_fft.eval(info["expression"], info.get("parameters", None))
+        dsp_fft.add_column(outname, outcol)
+    for cut in cut_dict:
+        idxs = dsp_fft[cut].nda & idxs
+    log.debug("Applied Cuts")
 
-    dsp_fft = run_one_dsp(raw_fft, dsp_config, db_dict=par_dsp[lh5_path])
-    cut_dict = generate_cuts(dsp_fft, parameters=dplms_dict["bls_cut_pars"])
-    idxs = get_cut_indexes(dsp_fft, cut_dict)
     bl_field = dplms_dict["bl_field"]
-    log.info(f"... {len(dsp_fft[bl_field].values.nda[idxs,:])} baselines after cuts")
+    log.info(f"... {len(dsp_fft[bl_field].values.nda[idxs, :])} baselines after cuts")
 
     bls = dsp_fft[bl_field].values.nda[idxs, : dplms_dict["bsize"]]
     bls_par = {}
     bls_cut_pars = [par for par in dplms_dict["bls_cut_pars"].keys()]
     for par in bls_cut_pars:
         bls_par[par] = dsp_fft[par].nda
     t1 = time.time()
     log.info(
         f"total events {len(raw_fft)}, {len(bls)} baseline selected in {(t1-t0):.2f} s"
     )
 
     log.info(
-        "\nCalculating noise matrix of length",
-        dplms_dict["length"],
-        "n. events",
-        bls.shape[0],
-        "size",
-        bls.shape[1],
+        f'Calculating noise matrix of length {dplms_dict["length"]} n. events: {bls.shape[0]}, size: {bls.shape[1]}'
     )
     nmat = noise_matrix(bls, dplms_dict["length"])
     t2 = time.time()
     log.info(f"Time to calculate noise matrix {(t2-t1):.2f} s")
 
-    log.info("\nSelecting signals")
+    log.info("Selecting signals")
     wsize = dplms_dict["wsize"]
     wf_field = dplms_dict["wf_field"]
-    peaks_keV = np.array(dplms_dict["peaks_keV"])
+    peaks_kev = np.array(dplms_dict["peaks_kev"])
     kev_widths = [tuple(kev_width) for kev_width in dplms_dict["kev_widths"]]
 
     log.info(f"Produce dsp data for {len(raw_cal)} events")
-    dsp_cal = run_one_dsp(raw_cal, dsp_config, db_dict=par_dsp[lh5_path])
+    dsp_cal = run_one_dsp(raw_cal, dsp_config, db_dict=par_dsp)
     t3 = time.time()
     log.info(f"Time to run dsp production {(t3-t2):.2f} s")
 
     dsp_config["outputs"] = [ene_par, "dt_eff"]
 
     # dictionary for peak fitting
     peak_dict = {
-        "peak": peaks_keV[-1],
+        "peak": peaks_kev[-1],
         "kev_width": kev_widths[-1],
         "parameter": ene_par,
-        "func": extended_gauss_step_pdf,
-        "gof_func": gauss_step_pdf,
+        "func": gauss_on_step,
     }
 
     if display > 0:
         plot_dict = {}
         plot_dict["dplms"] = {}
 
     # penalized coefficients
@@ -134,21 +125,18 @@
     prod = list(itertools.product(*lists))
     grid_dict = {}
     min_fom = float("inf")
     min_idx = None
 
     for i, values in enumerate(prod):
         coeff_values = dict(zip(coeff_keys, values))
+        log_msg = f"Case {i} ->"
+        for key, value in coeff_values.items():
+            log_msg += f" {key} = {value}"
 
-        log.info(
-            "\nCase",
-            i,
-            "->",
-            ", ".join(f"{key} = {value}" for key, value in coeff_values.items()),
-        )
         grid_dict[i] = coeff_values
 
         sel_dict = signal_selection(dsp_cal, dplms_dict, coeff_values)
         wfs = dsp_cal[wf_field].nda[sel_dict["idxs"], :]
         log.info(f"... {len(wfs)} signals after signal selection")
 
         ref, rmat, pmat, fmat = signal_matrices(wfs, dplms_dict["length"], decay_const)
@@ -162,30 +150,30 @@
             rmat,
             za_coeff,
             pmat,
             ft_coeff * fmat,
             dplms_dict["length"],
             wsize,
         )
-        par_dsp[lh5_path]["dplms"] = {"length": dplms_dict["length"], "coefficients": x}
+        par_dsp["dplms"] = {"length": dplms_dict["length"], "coefficients": x}
         log.info(
-            f"Filter synthesis in {time.time()-t_tmp:.1f} s, filter area", np.sum(x)
+            f"Filter synthesis in {time.time()-t_tmp:.1f} s, filter area {np.sum(x)}"
         )
 
         t_tmp = time.time()
-        dsp_opt = run_one_dsp(raw_cal, dsp_config, db_dict=par_dsp[lh5_path])
+        dsp_opt = run_one_dsp(raw_cal, dsp_config, db_dict=par_dsp)
 
         try:
-            res = fom_FWHM_with_dt_corr_fit(
+            res = fom_fwhm_with_alpha_fit(
                 dsp_opt,
                 peak_dict,
-                "QDrift",
+                "dt_eff",
                 idxs=np.where(~np.isnan(dsp_opt["dt_eff"].nda))[0],
             )
-        except:
+        except Exception:
             log.debug("FWHM not calculated")
             continue
 
         fwhm, fwhm_err, alpha, chisquare = (
             res["fwhm"],
             res["fwhm_err"],
             res["alpha"],
@@ -194,19 +182,20 @@
         log.info(
             f"FWHM = {fwhm:.2f} ± {fwhm_err:.2f} keV, evaluated in {time.time()-t_tmp:.1f} s"
         )
 
         grid_dict[i]["fwhm"] = fwhm
         grid_dict[i]["fwhm_err"] = fwhm_err
         grid_dict[i]["alpha"] = alpha
-
+        p_val = chi2.sf(chisquare[0], chisquare[1])
         if (
             fwhm < dplms_dict["fwhm_limit"]
             and fwhm_err < dplms_dict["err_limit"]
-            and chisquare < dplms_dict["chi_limit"]
+            and p_val > p_val_lim
+            and ~np.isnan(fwhm)
         ):
             if fwhm < min_fom:
                 min_idx, min_fom = i, fwhm
 
     if min_idx is not None:
         min_result = grid_dict[min_idx]
         best_case_values = {key: min_result[key] for key in min_result.keys()}
@@ -238,14 +227,16 @@
             log.error("Some values are missing in the best case results")
     else:
         log.error("Filter synthesis failed")
         nm_coeff = dplms_dict["dp_def"]["nm"]
         ft_coeff = dplms_dict["dp_def"]["ft"]
         rt_coeff = dplms_dict["dp_def"]["rt"]
         pt_coeff = dplms_dict["dp_def"]["pt"]
+        best_case_values = {}
+        alpha = 0
 
     # filter synthesis
     sel_dict = signal_selection(dsp_cal, dplms_dict, best_case_values)
     idxs = sel_dict["idxs"]
     wfs = dsp_cal[wf_field].nda[idxs, :]
     ref, rmat, pmat, fmat = signal_matrices(wfs, dplms_dict["length"], decay_const)
 
@@ -256,26 +247,18 @@
         za_coeff,
         pmat,
         ft_coeff * fmat,
         dplms_dict["length"],
         wsize,
     )
 
-    sto.write(
-        Array(x),
-        name="dplms",
-        lh5_file=par_dsp_lh5,
-        wo_mode="overwrite",
-        group=lh5_path,
-    )
-
     out_dict = {
         "dplms": {
             "length": dplms_dict["length"],
-            "coefficients": f"loadlh5('{par_dsp_lh5}', '{lh5_path}/dplms')",
+            "coefficients": x,
             "dp_coeffs": {
                 "nm": nm_coeff,
                 "za": za_coeff,
                 "ft": ft_coeff,
                 "rt": rt_coeff,
                 "pt": pt_coeff,
             },
@@ -288,71 +271,76 @@
         }
     }
     out_dict.update({"ctc_params": out_alpha_dict})
 
     log.info(f"Time to complete DPLMS filter synthesis {time.time()-t0:.1f}")
 
     if display > 0:
-        plot_dict["dplms"]["ref"] = ref
-        plot_dict["dplms"]["coefficients"] = x
+        plot_dict = {"ref": ref, "coefficients": x}
 
         bl_idxs = np.random.choice(len(bls), dplms_dict["n_plot"])
         bls = bls[bl_idxs]
         fig, ax = plt.subplots(figsize=(12, 6.75), facecolor="white")
         for ii, wf in enumerate(bls):
             if ii < 10:
                 ax.plot(wf, label=f"mean = {wf.mean():.1f}")
             else:
                 ax.plot(wf)
-        ax.legend(title=f"{lh5_path}", loc="upper right")
-        plot_dict["dplms"]["bls"] = fig
+        ax.legend(loc="upper right")
+        plot_dict["bls"] = fig
         fig, ax = plt.subplots(nrows=2, ncols=3, figsize=(16, 9), facecolor="white")
         for ii, par in enumerate(bls_cut_pars):
-            mean = cut_dict[par]["Mean Value"]
-            llo, lup = cut_dict[par]["Lower Boundary"], cut_dict[par]["Upper Boundary"]
+            if "parameters" in cut_dict[par]:
+                if "a" in cut_dict[par]["parameters"]:
+                    llo = cut_dict[par]["parameters"]["a"]
+                else:
+                    llo = np.nan
+                if "b" in cut_dict[par]["parameters"]:
+                    lup = cut_dict[par]["parameters"]["b"]
+                else:
+                    lup = np.nan
+            mean = (lup + llo) / 2
             plo, pup = mean - 2 * (mean - llo), mean + 2 * (lup - mean)
             hh, bb = np.histogram(bls_par[par], bins=np.linspace(plo, pup, 200))
             ax.flat[ii].plot(bb[1:], hh, ds="steps", label=f"cut on {par}")
             ax.flat[ii].axvline(lup, color="k", linestyle=":", label="selection")
             ax.flat[ii].axvline(llo, color="k", linestyle=":")
             ax.flat[ii].set_xlabel(par)
             ax.flat[ii].set_yscale("log")
-            ax.flat[ii].legend(title=f"{lh5_path}", loc="upper right")
-        plot_dict["dplms"]["bl_sel"] = fig
+            ax.flat[ii].legend(loc="upper right")
+        plot_dict["bl_sel"] = fig
 
         wf_idxs = np.random.choice(len(wfs), dplms_dict["n_plot"])
         wfs = wfs[wf_idxs]
-        peak_pos = dsp_cal["peak_pos"].nda
-        peak_pos_neg = dsp_cal["peak_pos_neg"].nda
         centroid = dsp_cal["centroid"].nda
-        risetime = dsp_cal["tp_90"].nda - dsp_cal["tp_10"].nda
-        rt_low = dplms_dict["rt_low"]
-        rt_high = dplms_dict["rt_high"]
-        peak_lim = dplms_dict["peak_lim"]
-        cal_par = {}
-        wfs_cut_pars = [par for par in dplms_dict["wfs_cut_pars"].keys()]
-        for par in wfs_cut_pars:
-            cal_par[par] = dsp_cal[par].nda
+
         fig, ax = plt.subplots(figsize=(12, 6.75), facecolor="white")
         for ii, wf in enumerate(wfs):
             if ii < 10:
                 ax.plot(wf, label=f"centr = {centroid[ii]}")
             else:
                 ax.plot(wf)
-        ax.legend(title=f"{lh5_path}", loc="upper right")
+        ax.legend(loc="upper right")
         axin = ax.inset_axes([0.1, 0.15, 0.35, 0.5])
         for wf in wfs:
             axin.plot(wf)
         axin.set_xlim(wsize / 2 - dplms_dict["zoom"], wsize / 2 + dplms_dict["zoom"])
         axin.set_yticklabels("")
-        plot_dict["dplms"]["wfs"] = fig
+        plot_dict["wfs"] = fig
+
+        peak_pos = dsp_cal["peak_pos"].nda
+        risetime = dsp_cal["tp_90"].nda - dsp_cal["tp_10"].nda
+        rt_low = dplms_dict["rt_low"]
+        rt_high = dplms_dict["rt_high"]
+        peak_lim = dplms_dict["peak_lim"]
+        cal_par = {}
+        wfs_cut_pars = ["centroid", "peak_pos", "risetime"]
+
         fig, ax = plt.subplots(nrows=2, ncols=3, figsize=(16, 9), facecolor="white")
-        wfs_cut_pars.append("centroid")
-        wfs_cut_pars.append("peak_pos")
-        wfs_cut_pars.append("risetime")
+
         for ii, par in enumerate(wfs_cut_pars):
             pspace = np.linspace(
                 wsize / 2 - peak_lim, wsize / 2 + peak_lim, 2 * peak_lim
             )
             if par == "centroid":
                 llo, lup = sel_dict["ct_ll"], sel_dict["ct_hh"]
                 hh, bb = np.histogram(centroid, bins=pspace)
@@ -371,31 +359,31 @@
             ax.flat[ii + 1].axvline(
                 llo, color="k", linestyle=":", label=f"sel. {llo:.1f} {lup:.1f}"
             )
             if par != "centroid":
                 ax.flat[ii + 1].axvline(lup, color="k", linestyle=":")
             ax.flat[ii + 1].set_xlabel(par)
             ax.flat[ii + 1].set_yscale("log")
-            ax.flat[ii + 1].legend(title=f"{lh5_path}", loc="upper right")
+            ax.flat[ii + 1].legend(loc="upper right")
         roughenergy = dsp_cal["trapTmax"].nda
         roughenergy_sel = roughenergy[idxs]
         ell, ehh = roughenergy.min(), roughenergy.max()
         he, be = np.histogram(roughenergy, bins=np.linspace(ell, ehh, 1000))
         hs, be = np.histogram(roughenergy_sel, bins=np.linspace(ell, ehh, 1000))
         ax.flat[0].plot(be[1:], he, c="b", ds="steps", label="initial")
         ax.flat[0].plot(be[1:], hs, c="r", ds="steps", label="selected")
         ax.flat[0].set_xlabel("rough energy (ADC)")
         ax.flat[0].set_yscale("log")
-        ax.flat[0].legend(loc="upper right", title=f"{lh5_path}")
-        plot_dict["dplms"]["wf_sel"] = fig
+        ax.flat[0].legend(loc="upper right")
+        plot_dict["wf_sel"] = fig
 
         fig, ax = plt.subplots(figsize=(12, 6.75), facecolor="white")
-        ax.plot(x, "r-", label=f"filter")
+        ax.plot(x, "r-", label="filter")
         ax.axhline(0, color="black", linestyle=":")
-        ax.legend(loc="upper right", title=f"{lh5_path}")
+        ax.legend(loc="upper right")
         axin = ax.inset_axes([0.6, 0.1, 0.35, 0.33])
         axin.plot(x, "r-")
         axin.set_xlim(
             dplms_dict["length"] / 2 - dplms_dict["zoom"],
             dplms_dict["length"] / 2 + dplms_dict["zoom"],
         )
         axin.set_yticklabels("")
@@ -452,15 +440,14 @@
 def signal_selection(dsp_cal, dplms_dict, coeff_values):
     peak_pos = dsp_cal["peak_pos"].nda
     peak_pos_neg = dsp_cal["peak_pos_neg"].nda
     centroid = dsp_cal["centroid"].nda
     risetime = dsp_cal["tp_90"].nda - dsp_cal["tp_10"].nda
 
     rt_low = dplms_dict["rt_low"]
-    rt_high = dplms_dict["rt_high"]
     peak_lim = dplms_dict["peak_lim"]
     wsize = dplms_dict["wsize"]
     bsize = dplms_dict["bsize"]
 
     centroid_lim = dplms_dict["centroid_lim"]
     if "rt" in coeff_values:
         perc = coeff_values["rt"]
@@ -468,21 +455,21 @@
         perc = dplms_dict["dp_def"]["rt"]
     if "pt" in coeff_values:
         thr = coeff_values["pt"]
     else:
         thr = dplms_dict["dp_def"]["rt"]
 
     idxs_ct, ct_ll, ct_hh = is_valid_centroid(centroid, centroid_lim, wsize, bsize)
-    log.info(f"... {len(peak_pos[idxs_ct,:])} signals after alignment")
+    log.info(f"... {len(peak_pos[idxs_ct, :])} signals after alignment")
 
     idxs_pp, pp_ll, pp_hh = is_not_pile_up(peak_pos, peak_pos_neg, thr, peak_lim, wsize)
-    log.info(f"... {len(peak_pos[idxs_pp,:])} signals after pile-up cut")
+    log.info(f"... {len(peak_pos[idxs_pp, :])} signals after pile-up cut")
 
     idxs_rt, rt_ll, rt_hh = is_valid_risetime(risetime, rt_low, perc)
-    log.info(f"... {len(peak_pos[idxs_rt,:])} signals after risetime cut")
+    log.info(f"... {len(peak_pos[idxs_rt, :])} signals after risetime cut")
 
     idxs = idxs_ct & idxs_pp & idxs_rt
     sel_dict = {
         "idxs": idxs,
         "ct_ll": ct_ll,
         "ct_hh": ct_hh,
         "pp_ll": pp_ll,
```

### Comparing `pygama-1.6.0a2/src/pygama/pargen/energy_optimisation.py` & `pygama-2.0.0a1/src/pygama/pargen/energy_cal.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,2123 +1,2666 @@
+"""routines for automatic calibration.
+
+- hpge_find_energy_peaks (Find uncalibrated E peaks whose E spacing matches the pattern in peaks_kev)
+- hpge_get_energy_peaks (Get uncalibrated E peaks at the energies of peaks_kev)
+- hpge_fit_energy_peaks (fits the energy peals)
+- hpge_E_calibration (main routine -- finds and fits peaks specified)
 """
-This module contains the functions for performing the energy optimisation.
-This happens in 2 steps, firstly a grid search is performed on each peak
-separately using the optimiser, then the resulting grids are interpolated
-to provide the best energy resolution at Qbb
-"""
 
-import json
+from __future__ import annotations
+
+import inspect
 import logging
-import os
-import pathlib
-import pickle as pkl
-import sys
-from collections import namedtuple
+import string
 
-import lgdo.lh5 as lh5
-import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
-import pandas as pd
-from iminuit import Minuit, cost, util
-from matplotlib.backends.backend_pdf import PdfPages
-from matplotlib.colors import LogNorm
-from scipy.optimize import curve_fit, minimize
-from scipy.stats import chisquare, norm
-from sklearn.exceptions import ConvergenceWarning
-from sklearn.gaussian_process import GaussianProcessRegressor
-from sklearn.gaussian_process.kernels import RBF, ConstantKernel
-from sklearn.utils._testing import ignore_warnings
+import scipy.stats
+from iminuit import Minuit, cost
+from iminuit.util import ValueView
+from numpy.polynomial.polynomial import Polynomial
+from scipy.stats import chi2
 
+import pygama.math.binned_fitting as pgb
+import pygama.math.distributions as pgf
 import pygama.math.histogram as pgh
-import pygama.math.peak_fitting as pgf
-import pygama.pargen.cuts as cts
-import pygama.pargen.dsp_optimize as opt
-import pygama.pargen.energy_cal as pgc
+from pygama.math.histogram import get_i_local_maxima
+from pygama.math.least_squares import fit_simple_scaling
+from pygama.pargen.utils import convert_to_minuit, return_nans
 
 log = logging.getLogger(__name__)
-sto = lh5.LH5Store()
 
 
-def run_optimisation(
-    file,
-    opt_config,
-    dsp_config,
-    cuts,
-    fom,
-    db_dict=None,
-    n_events=8000,
-    wf_field="waveform",
-    **fom_kwargs,
-):
+class HPGeCalibration:
     """
-    Runs optimisation on .lh5 file
+    Calibrate HPGe data to a set of known peaks. Class stores the calibration parameters
+    as well as the peaks locations and energies used. Each function called updates a results
+    dictionary with any additional information which is stored in the class.
 
     Parameters
     ----------
-    file: string
-        path to raw .lh5 file
-    opt_config: str
-        path to JSON dictionary to configure optimisation
-    dsp_config: str
-        path to JSON dictionary specifying dsp configuration
-    fom: function
-        When given the output lh5 table of a DSP iteration, the
-        fom_function must return a scalar figure-of-merit value upon which the
-        optimization will be based. Should accept verbosity as a second argument
-    db_dict: dict
-        Dictionary specifying any values to put in processing chain e.g. pz constant
-    n_events : int
-        Number of events to run over
-    """
-    grid = set_par_space(opt_config)
-    waveforms = sto.read(f"/raw/{wf_field}", file, idx=cuts, n_rows=n_events)[0]
-    baseline = sto.read("/raw/baseline", file, idx=cuts, n_rows=n_events)[0]
-    tb_data = lh5.Table(col_dict={f"{wf_field}": waveforms, "baseline": baseline})
-    return opt.run_grid(tb_data, dsp_config, grid, fom, db_dict, **fom_kwargs)
-
-
-def run_optimisation_multiprocessed(
-    file,
-    opt_config,
-    dsp_config,
-    cuts,
-    lh5_path,
-    fom=None,
-    db_dict=None,
-    processes=5,
-    n_events=8000,
-    **fom_kwargs,
-):
-    """
-    Runs optimisation on .lh5 file, this version multiprocesses the grid points, it also can handle multiple grids being passed
-    as long as they are the same dimensions.
+    e_uncal : array
+        uncalibrated energy data
+    glines : array
+        list of peak energies to be fit to. Each must be in the data
+    guess_kev : float
+        a rough initial guess at the conversion factor from e_uncal to kev. Must
+        be positive
+    deg : non-negative int
+        degree of the polynomial for the E_cal function E_kev = poly(e_uncal).
+        deg = 0 corresponds to a simple scaling E_kev = scale * e_uncal.
+        Otherwise follows the convention in np.polynomial.polynomial of
+        lowest order to highest order
+    uncal_is_int : bool
+        if True, attempts will be made to avoid picket-fencing when binning
+        e_uncal
+    fixed : dict
+        dictionary of fixed parameters for the calibration function
 
-    Parameters
-    ----------
-    file: string
-        path to raw .lh5 file
-    opt_config: str
-        path to JSON dictionary to configure optimisation
-    dsp_config: str
-        path to JSON dictionary specifying dsp configuration
-    fom: function
-        When given the output lh5 table of a DSP iteration, the
-        fom_function must return a scalar figure-of-merit value upon which the
-        optimization will be based. Should accept verbosity as a second argument
-    n_events : int
-        Number of events to run over
-    db_dict: dict
-        Dictionary specifying any values to put in processing chain e.g. pz constant
-    processes : int
-        Number of separate processes to run for the multiprocessing
     """
 
-    def form_dict(in_dict, length):
-        keys = list(in_dict.keys())
-        out_list = []
-        for i in range(length):
-            out_list.append({keys[0]: 0})
-        for key in keys:
-            if isinstance(in_dict[key], list):
-                if len(in_dict[key]) == length:
-                    for i in range(length):
-                        out_list[i][key] = in_dict[key][i]
-                else:
-                    for i in range(length):
-                        out_list[i][key] = in_dict[key]
+    def __init__(
+        self,
+        energy_param,
+        glines,
+        guess_kev: float,
+        deg: int = 1,
+        uncal_is_int: bool = False,
+        fixed=None,
+        debug_mode: bool = False,
+    ):
+        self.energy_param = energy_param
+
+        if deg < -1:
+            log.error(f"hpge_E_cal warning: invalid deg = {deg}")
+            return
+        self.deg = int(deg)
+
+        self.peaks_kev = np.asarray(sorted(glines))
+        self.peak_locs = []
+
+        if guess_kev <= 0:
+            log.error(f"hpge_E_cal warning: invalid guess_kev = {guess_kev}")
+        if deg == -1:
+            self.pars = np.zeros(2, dtype=float)
+            self.pars[0] = guess_kev
+            self.fixed = {1: 1}
+        elif deg == 0:
+            self.pars = np.zeros(2, dtype=float)
+            self.pars[1] = guess_kev
+            self.fixed = {0: 0}
+        else:
+            self.pars = np.zeros(self.deg + 1, dtype=float)
+            self.pars[1] = guess_kev
+            self.fixed = fixed
+        self.results = {}
+
+        self.uncal_is_int = uncal_is_int
+        self.debug_mode = debug_mode
+
+    def gen_pars_dict(self):
+        """
+        Generate a dictionary containing the expression and parameters used for energy calibration.
+
+        Returns:
+            dict: A dictionary with keys 'expression' and 'parameters'.
+                  'expression' is a string representing the energy calibration expression.
+                  'parameters' is a dictionary containing the parameter values used in the expression.
+        """
+        expression = ""
+        parameters = {}
+        for i, coeff in enumerate(self.pars):
+            parameter_name = string.ascii_lowercase[i]
+            if i == 0:
+                expression += f"{parameter_name}"
+            elif i == 1:
+                expression += f" + {parameter_name} * {self.energy_param}"
             else:
-                for i in range(length):
-                    out_list[i][key] = in_dict[key]
-        return out_list
-
-    if not isinstance(opt_config, list):
-        opt_config = [opt_config]
-    grid = []
-    for i, opt_conf in enumerate(opt_config):
-        grid.append(set_par_space(opt_conf))
-    if fom_kwargs:
-        if "fom_kwargs" in fom_kwargs:
-            fom_kwargs = fom_kwargs["fom_kwargs"]
-        fom_kwargs = form_dict(fom_kwargs, len(grid))
-    sto = lh5.LH5Store()
-    waveforms = sto.read(f"{lh5_path}/{wf_field}", file, idx=cuts, n_rows=n_events)[0]
-    baseline = sto.read(f"{lh5_path}/baseline", file, idx=cuts, n_rows=n_events)[0]
-    tb_data = lh5.Table(col_dict={f"{wf_field}": waveforms, "baseline": baseline})
-    return opt.run_grid_multiprocess_parallel(
-        tb_data,
-        dsp_config,
-        grid,
-        fom,
-        db_dict=db_dict,
-        processes=processes,
-        fom_kwargs=fom_kwargs,
-    )
+                expression += f" + {parameter_name} * {self.energy_param}**{i} "
+            parameters[parameter_name] = coeff
+        return {"expression": expression, "parameters": parameters}
+
+    def update_results_dict(self, results_dict):
+        name = inspect.stack()[1][3]
+        if name in self.results:
+            it = 0
+            for n in self.results:
+                if name in n:
+                    if name == n:
+                        pass
+                    else:
+                        new_it = int(n.split("_")[-1])
+                        if new_it > it:
+                            it = new_it
+            it += 1
+            name += f"_{it}"
+        self.results[name] = results_dict
+
+    def hpge_find_energy_peaks(
+        self,
+        e_uncal,
+        peaks_kev=None,
+        n_sigma=5,
+        etol_kev=None,
+        bin_width_kev=1,
+        erange=None,
+        var_zero=1,
+        update_cal_pars=True,
+    ):
+        """
+        Find uncalibrated energy peaks whose energy spacing matches the pattern in peaks_kev.
+
+        Parameters
+        ----------
+        e_uncal (array-like):
+            Uncalibrated energy values.
+        peaks_kev (array-like, optional):
+            Pattern of energy peaks to match. If not provided, the peaks from the object's attribute `peaks_kev` will be used.
+        n_sigma (float, optional):
+             Number of standard deviations above the mean to consider a peak significant. Default is 5.
+        etol_kev (float, optional):
+            Tolerance in energy units for matching peaks. If not provided, it will be estimated based on the peak widths.
+        bin_width_kev (float, optional):
+            Width of the energy bins for initial peak search. Default is 1 keV.
+        erange (tuple, optional):
+            Range of uncalibrated energy values to consider. If not provided, the range will be determined based on the peaks.
+        var_zero (float, optional):
+            Value to replace zero variance with. Default is 1.
+        update_cal_pars (bool, optional):
+            Whether to update the calibration parameters. Default is True.
+
+        Returns:
+            None
+
+        """
+
+        if peaks_kev is None:
+            peaks_kev = self.peaks_kev
+
+        peaks_adc = [(Polynomial(self.pars) - ei).roots() for ei in peaks_kev]
+
+        # bin the histogram in ~1 kev bins for the initial rough peak search
+        if erange is None:
+            euc_min = np.nanmin(peaks_adc) * 0.6
+            euc_max = np.nanmax(peaks_adc) * 1.1
 
+        else:
+            euc_min, euc_max = erange
+        d_euc = bin_width_kev / self.pars[1]
+        if self.uncal_is_int:
+            euc_min, euc_max, d_euc = pgh.better_int_binning(
+                x_lo=euc_min, x_hi=euc_max, dx=d_euc
+            )
+        hist, bins, var = pgh.get_hist(e_uncal, range=(euc_min, euc_max), dx=d_euc)
+
+        # clean up var if necessary
+        if np.any(var == 0):
+            log.debug(f"hpge_find_energy_peaks: replacing var zeros with {var_zero}")
+            var[np.where(var == 0)] = var_zero
+        peaks_kev = np.asarray(peaks_kev)
+
+        # Find all maxes with > n_sigma significance
+        imaxes = get_i_local_maxima(hist / np.sqrt(var), n_sigma)
+
+        # Now pattern match to peaks_kev within etol_kev using poly_match
+        detected_max_locs = pgh.get_bin_centers(bins)[imaxes]
+
+        if etol_kev is None:
+            # estimate etol_kev
+            pt_pars, pt_covs = hpge_fit_energy_peak_tops(
+                hist, bins, var, detected_max_locs, n_to_fit=15
+            )
+            if (
+                sum(np.sum(c.flatten()) if c.ndim != 0 else 0 for c in pt_covs)
+                == np.inf
+                or sum(np.sum(c.flatten()) if c.ndim != 0 else 0 for c in pt_covs) == 0
+            ):
+                log.debug(
+                    "hpge_find_energy_peaks: can safely ignore previous covariance warning, not used"
+                )
+            pt_pars = pt_pars[np.array([x is not None for x in pt_pars])]
+            med_sigma_ratio = np.median(
+                np.stack(pt_pars)[:, 1] / np.stack(pt_pars)[:, 0]
+            )
 
-def set_par_space(opt_config):
-    """
-    Generates grid for optimizer from dictionary of form {param : {start: , end: , spacing: }}
-    """
-    par_space = opt.ParGrid()
-    for name in opt_config.keys():
-        p_values = opt_config[name]
-        for param in p_values.keys():
-            str_vals = set_values(p_values[param])
-            par_space.add_dimension(name, param, str_vals)
-    return par_space
+            etol_kev = 5.0 * (med_sigma_ratio / 0.003)
+        pars, ixtup, iytup = poly_match(
+            detected_max_locs, peaks_kev, deg=self.deg, atol=etol_kev, fixed=self.fixed
+        )
 
+        if len(ixtup) != len(peaks_kev):
+            log.info(
+                f"hpge_find_energy_peaks: only found {len(ixtup)} of {len(peaks_kev)} expected peaks"
+            )
 
-def set_values(par_values):
-    """
-    Finds values for grid
-    """
-    string_values = np.arange(
-        par_values["start"], par_values["end"], par_values["spacing"]
-    )
-    try:
-        string_values = [f'{val:.4f}*{par_values["unit"]}' for val in string_values]
-    except:
-        string_values = [f"{val:.4f}" for val in string_values]
-    return string_values
+        self.update_results_dict(
+            {
+                "input_peaks_kev": peaks_kev,
+                "found_peaks_kev": peaks_kev[iytup],
+                "found_peaks_locs": detected_max_locs[iytup],
+            }
+        )
+        log.info(f"{len(peaks_kev[iytup])} peaks found:")
+        log.info("\t   Energy   | Position  ")
+        for i, (li, ei) in enumerate(zip(detected_max_locs[ixtup], peaks_kev[iytup])):
+            log.info(f"\t{i}".ljust(4) + str(ei).ljust(9) + f"| {li:g}".ljust(5))
+
+        if update_cal_pars is False:
+            return
+
+        self.peak_locs = detected_max_locs[ixtup]
+        self.peaks_kev = peaks_kev[iytup]
+        self.pars = np.array(pars)
+
+    def hpge_get_energy_peaks(
+        self,
+        e_uncal,
+        peaks_kev=None,
+        n_sigma=3,
+        etol_kev=5,
+        var_zero=1,
+        bin_width_kev=0.2,
+        update_cal_pars=True,
+        erange=None,
+    ):
+        """Get uncalibrated E peaks at the energies of peaks_kev
+
+        Parameters
+        ----------
+        e_uncal : array
+            Uncalibrated energy values.
+        peaks_kev : array, optional
+            Energies of peaks to search for (in keV). If not provided, the peaks_kev
+            attribute of the object will be used.
+        n_sigma : float, optional
+            Threshold for detecting a peak in sigma (i.e. sqrt(var)). Default is 3.
+        etol_kev : float, optional
+            Absolute tolerance in energy for matching peaks. Default is 5.
+        var_zero : float, optional
+            Number used to replace zeros of var to avoid divide-by-zero in hist/sqrt(var).
+            Default is 1. Usually when var = 0, it's because hist = 0, and any value here is fine.
+        bin_width_kev : float, optional
+            Width of the energy bins for re-binning the histogram. Default is 0.2 keV.
+        update_cal_pars : bool, optional
+            Flag indicating whether to update the calibration parameters. Default is True.
+        erange : tuple, optional
+            Range of energy values to consider for peak search. If not provided, the range
+            will be determined automatically based on the peaks_kev values.
+
+        Returns
+        -------
+        None
+
+        Notes
+        -----
+        This method performs the following steps:
+        1. Re-bins the histogram in ~0.2 keV bins with updated energy scale parameters for peak-top fits.
+        2. Finds all local maxima in the histogram with significance greater than n_sigma.
+        3. Matches the calculated peak energies with the expected peak energies.
+        4. Removes duplicate peak matches.
+        5. Updates the input peaks, got peaks, and got peak locations in the results dictionary.
+        6. If update_cal_pars is True, calculates the updated calibration curve using the matched peak energies.
+
+        """
+        if peaks_kev is None:
+            peaks_kev = self.peaks_kev
+
+        peaks_kev = np.asarray(peaks_kev)
+
+        # re-bin the histogram in ~0.2 kev bins with updated E scale par for peak-top fits
+        if erange is None:
+            euc_min, euc_max = (
+                (Polynomial(self.pars) - i).roots()
+                for i in (peaks_kev[0] * 0.9, peaks_kev[-1] * 1.1)
+            )
+            euc_min = euc_min[0]
+            euc_max = euc_max[0]
+            if euc_min < 0:
+                euc_min = 0
+            if euc_max > np.nanmax(e_uncal) * 1.1:
+                euc_max = np.nanmax(e_uncal) * 1.1
+        else:
+            euc_min, euc_max = erange
 
+        d_euc = bin_width_kev / self.pars[1]
 
-def simple_guess(hist, bins, var, func_i, fit_range):
-    """
-    Simple guess for peak fitting
-    """
-    if func_i == pgf.extended_radford_pdf:
-        bin_cs = (bins[1:] + bins[:-1]) / 2
-        _, sigma, amp = pgh.get_gaussian_guess(hist, bins)
-        i_0 = np.nanargmax(hist)
-        mu = bin_cs[i_0]
-        height = hist[i_0]
-        bg0 = np.mean(hist[-10:])
-        step = np.mean(hist[:10]) - bg0
-        htail = 1.0 / 5
-        tau = 0.5 * sigma
-
-        hstep = step / (bg0 + np.mean(hist[:10]))
-        dx = np.diff(bins)[0]
-        n_bins_range = int((4 * sigma) // dx)
-        nsig_guess = np.sum(hist[i_0 - n_bins_range : i_0 + n_bins_range])
-        nbkg_guess = np.sum(hist) - nsig_guess
-        parguess = [
-            nsig_guess,
-            mu,
-            sigma,
-            htail,
-            tau,
-            nbkg_guess,
-            hstep,
-            fit_range[0],
-            fit_range[1],
-            0,
-        ]  #
-        return parguess
-
-    elif func_i == pgf.extended_gauss_step_pdf:
-        mu, sigma, amp = pgh.get_gaussian_guess(hist, bins)
-        i_0 = np.argmax(hist)
-        bg = np.mean(hist[-10:])
-        step = bg - np.mean(hist[:10])
-        hstep = step / (bg + np.mean(hist[:10]))
-        dx = np.diff(bins)[0]
-        n_bins_range = int((4 * sigma) // dx)
-        nsig_guess = np.sum(hist[i_0 - n_bins_range : i_0 + n_bins_range])
-        nbkg_guess = np.sum(hist) - nsig_guess
-        return [nsig_guess, mu, sigma, nbkg_guess, hstep, fit_range[0], fit_range[1], 0]
+        if self.uncal_is_int:
+            euc_min, euc_max, d_euc = pgh.better_int_binning(
+                x_lo=euc_min, x_hi=euc_max, dx=d_euc
+            )
+        hist, bins, var = pgh.get_hist(e_uncal, range=(euc_min, euc_max), dx=d_euc)
+
+        # clean up var if necessary
+        if np.any(var == 0):
+            log.debug(f"hpge_find_energy_peaks: replacing var zeros with {var_zero}")
+            var[np.where(var == 0)] = var_zero
+
+        # Find all maxes with > n_sigma significance
+        imaxes = get_i_local_maxima(hist / np.sqrt(var), n_sigma)
+
+        # Keep maxes if they coincide with expected peaks
+        test_peaks_kev = np.asarray([pgf.nb_poly(i, self.pars) for i in bins[imaxes]])
+        imatch = [abs(peaks_kev - i).min() < etol_kev for i in test_peaks_kev]
+
+        got_peak_locations = bins[imaxes[imatch]]
+        got_peak_energies = test_peaks_kev[imatch]
+
+        # Match calculated and true peak energies
+        matched_energies = peaks_kev[
+            [np.argmin(abs(peaks_kev - i)) for i in got_peak_energies]
+        ]
+        while not all([list(matched_energies).count(x) == 1 for x in matched_energies]):
+            for i in range(len(matched_energies)):
+                if matched_energies[i + 1] == matched_energies[i]:
+                    # remove duplicates
+                    if np.argmin(
+                        abs(got_peak_energies[i : i + 2] - matched_energies[i])
+                    ):  # i+1 is best match
+                        got_peak_locations = np.delete(got_peak_locations, i)
+                        got_peak_energies = np.delete(got_peak_energies, i)
+                    else:  # i is best match
+                        got_peak_locations = np.delete(got_peak_locations, i + 1)
+                        got_peak_energies = np.delete(got_peak_energies, i + 1)
+                    matched_energies = np.delete(matched_energies, i)
+                    break
+                i += 1
+
+        input_peaks = peaks_kev.copy()
+
+        self.update_results_dict(
+            {
+                "input_peaks_kev": input_peaks,
+                "got_peaks_kev": matched_energies,
+                "got_peaks_locs": got_peak_locations,
+            }
+        )
 
+        if update_cal_pars is False:
+            return
 
-def unbinned_energy_fit(
-    energy,
-    func,
-    gof_func,
-    gof_range,
-    fit_range=(np.inf, np.inf),
-    guess=None,
-    tol=None,
-    verbose=False,
-    display=0,
-):
-    """
-    Unbinned fit to energy. This is different to the default fitting as
-    it will try different fitting methods and choose the best. This is necessary for the lower statistics.
-    """
+        self.peak_locs = got_peak_locations
+        self.peaks_kev = matched_energies
 
-    bin_width = 1
-    lower_bound = (np.nanmin(energy) // bin_width) * bin_width
-    upper_bound = ((np.nanmax(energy) // bin_width) + 1) * bin_width
-    hist1, bins, var = pgh.get_hist(
-        energy, dx=bin_width, range=(lower_bound, upper_bound)
-    )
-    bin_cs1 = (bins[:-1] + bins[1:]) / 2
-    if guess is not None:
-        x0 = [*guess[:-2], fit_range[0], fit_range[1], False]
-    else:
-        if func == pgf.extended_radford_pdf:
-            x0 = simple_guess(hist1, bins, var, pgf.extended_gauss_step_pdf, fit_range)
-            if verbose:
-                print(x0)
-            c = cost.ExtendedUnbinnedNLL(energy, pgf.extended_gauss_step_pdf)
-            m = Minuit(c, *x0)
-            m.fixed[-3:] = True
-            m.simplex().migrad()
-            m.hesse()
-            if guess is not None:
-                x0_rad = [*guess[:-2], fit_range[0], fit_range[1], False]
-            else:
-                x0_rad = simple_guess(hist1, bins, var, func, fit_range)
-            x0 = m.values[:3]
-            x0 += x0_rad[3:5]
-            x0 += m.values[3:]
+        # Calculate updated calibration curve
+        if self.deg == 0:
+            scale, _ = fit_simple_scaling(got_peak_locations, matched_energies)
+            poly_pars = np.array([0, scale])
         else:
-            x0 = simple_guess(hist1, bins, var, func, fit_range)
-    if verbose:
-        print(x0)
-    c = cost.ExtendedUnbinnedNLL(energy, func)
-    m = Minuit(c, *x0)
-    if tol is not None:
-        m.tol = tol
-    m.fixed[-3:] = True
-    m.migrad()
-    m.hesse()
+            # Calculate updated calibration curve
+            poly_pars = (
+                Polynomial.fit(got_peak_locations, matched_energies, len(self.pars) - 1)
+                .convert()
+                .coef
+            )
+        c = cost.LeastSquares(
+            matched_energies,
+            got_peak_locations,
+            np.full_like(got_peak_locations, 1),
+            poly_wrapper,
+        )
+        if self.fixed is not None:
+            for idx, val in self.fixed.items():
+                if val is True or val is None:
+                    pass
+                else:
+                    poly_pars[idx] = val
+        m = Minuit(c, *poly_pars)
+        if self.fixed is not None:
+            for idx in list(self.fixed):
+                m.fixed[idx] = True
+
+        self.pars = np.array(m.values)
+
+        log.info(f"{len(self.peak_locs)} peaks obtained:")
+        log.info("\t   Energy   | Position  ")
+        for i, (li, ei) in enumerate(zip(self.peak_locs, self.peaks_kev)):
+            log.info(f"\t{i}".ljust(4) + str(ei).ljust(9) + f"| {li:g}".ljust(5))
+
+    def hpge_cal_energy_peak_tops(
+        self,
+        e_uncal,
+        n_sigmas=1.2,
+        peaks_kev=None,
+        default_n_bins=50,
+        n_events=None,
+        allowed_p_val=0.01,
+        update_cal_pars=True,
+    ):
+        """
+        Perform energy calibration for HPGe detector using peak fitting.
+
+        Args:
+            e_uncal (array-like):
+                Uncalibrated energy values.
+            n_sigmas (float, optional):
+                Number of standard deviations to use for peak fitting range. Defaults to 1.2.
+            peaks_kev (array-like, optional):
+                Known peak positions in keV. If not provided, uses self.peaks_kev. Defaults to None.
+            default_n_bins (int, optional):
+                    Number of bins for histogram. Defaults to 50.
+            n_events (int, optional):
+                Number of events to consider for calibration. Defaults to None which uses all events.
+            allowed_p_val (float, optional):
+                Maximum p-value for a fit to be considered valid. Defaults to 0.05.
+            update_cal_pars (bool, optional):
+                Whether to update the calibration parameters. Defaults to True.
+        """
+
+        results_dict = {}
+
+        # check no peaks in self.peaks_kev missing from peak_pars
+        if peaks_kev is None:
+            peaks_kev = self.peaks_kev
+
+        peak_pars = [(peak, None, pgf.gauss_on_uniform) for peak in peaks_kev]
+
+        # convert peak pars to array of tuples
+        tmp = np.empty(len(peak_pars), dtype=object)
+        tmp[:] = peak_pars
+        peak_pars = tmp
+
+        peak_pars_lines = [i[0] for i in peak_pars]
+        peaks_mask = np.array(
+            [True if peak in peaks_kev else False for peak in peak_pars_lines],
+            dtype=bool,
+        )
+        peak_pars = peak_pars[peaks_mask]
 
-    hist, bins, var = pgh.get_hist(energy, dx=1, range=gof_range)
-    bin_cs = (bins[:-1] + bins[1:]) / 2
-    m_fit = func(bin_cs1, *m.values)[1]
+        fit_peaks_mask = np.array(
+            [True for i in peak_pars if i[2] is not None],
+            dtype=bool,
+        )
+        peak_pars = peak_pars[fit_peaks_mask]
 
-    valid1 = (
-        m.valid
-        # & m.accurate
-        & (~np.isnan(m.errors).any())
-        & (~(np.array(m.errors[:-3]) == 0).all())
-    )
+        # First calculate range around peaks to fit
 
-    cs = pgf.goodness_of_fit(
-        hist, bins, None, gof_func, m.values[:-3], method="Pearson"
-    )
-    cs = cs[0] / cs[1]
-    m2 = Minuit(c, *x0)
-    if tol is not None:
-        m2.tol = tol
-    m2.fixed[-3:] = True
-    m2.simplex().migrad()
-    m2.hesse()
-    m2_fit = func(bin_cs1, *m2.values)[1]
-    valid2 = (
-        m2.valid
-        # & m2.accurate
-        & (~np.isnan(m.errors).any())
-        & (~(np.array(m2.errors[:-3]) == 0).all())
-    )
+        euc_min, euc_max = (
+            (Polynomial(self.pars) - i).roots()
+            for i in (peaks_kev[0] * 0.9, peaks_kev[-1] * 1.1)
+        )
+        euc_min = euc_min[0]
+        euc_max = euc_max[0]
 
-    cs2 = pgf.goodness_of_fit(
-        hist, bins, None, gof_func, m2.values[:-3], method="Pearson"
-    )
-    cs2 = cs2[0] / cs2[1]
+        if euc_min < 0:
+            euc_min = 0
+        if euc_max > np.nanmax(e_uncal) * 1.1:
+            euc_max = np.nanmax(e_uncal) * 1.1
 
-    frac_errors1 = np.sum(np.abs(np.array(m.errors)[:-3] / np.array(m.values)[:-3]))
-    frac_errors2 = np.sum(np.abs(np.array(m2.errors)[:-3] / np.array(m2.values)[:-3]))
+        d_euc = 0.5 / self.pars[1]
+        if self.uncal_is_int:
+            euc_min, euc_max, d_euc = pgh.better_int_binning(
+                x_lo=euc_min, x_hi=euc_max, dx=d_euc
+            )
 
-    if verbose:
-        print(m)
-        print(m2)
-        print(frac_errors1, frac_errors2)
+        hist, bins, var = pgh.get_hist(e_uncal, range=(euc_min, euc_max), dx=d_euc)
 
-    if display > 1:
-        m_fit = gof_func(bin_cs1, *m.values)
-        m2_fit = gof_func(bin_cs1, *m2.values)
-        plt.figure()
-        plt.plot(bin_cs1, hist1, label=f"hist")
-        plt.plot(bin_cs1, func(bin_cs1, *x0)[1], label=f"Guess")
-        plt.plot(bin_cs1, m_fit, label=f"Fit 1: {cs}")
-        plt.plot(bin_cs1, m2_fit, label=f"Fit 2: {cs2}")
-        plt.legend()
-        plt.show()
+        uncal_peak_pars = []
+        for pars in peak_pars:
+            peak, fit_range, func = pars
 
-    if valid1 == False and valid2 == False:
-        log.debug("Extra simplex needed")
-        m = Minuit(c, *x0)
-        if tol is not None:
-            m.tol = tol
-        m.fixed[-3:] = True
-        m.limits = pgc.get_hpge_E_bounds(func)
-        m.simplex().simplex().migrad()
-        m.hesse()
-        if verbose:
-            print(m)
-        cs = pgf.goodness_of_fit(
-            hist, bins, None, gof_func, m.values[:-3], method="Pearson"
-        )
-        cs = cs[0] / cs[1]
-        valid3 = (
-            m.valid
-            # & m.accurate
-            & (~np.isnan(m.errors).any())
-            & (~(np.array(m.errors[:-3]) == 0).all())
-        )
-        if valid3 is False:
+            if peak in self.peaks_kev:
+                loc = self.peak_locs[np.where(peak == self.peaks_kev)][0]
+            else:
+                loc = (Polynomial(self.pars) - peak).roots()[0]
+
+            # Need to do initial fit
+            pt_pars, _ = hpge_fit_energy_peak_tops(hist, bins, var, [loc], n_to_fit=7)
+            # Drop failed fits
+            if pt_pars[0] is not None:
+                range_uncal = (float(pt_pars[0][1]) * 20, float(pt_pars[0][1]) * 20)
+                n_bins = default_n_bins
+            else:
+                range_uncal = None
+            if range_uncal is not None:
+                uncal_peak_pars.append((peak, loc, range_uncal, n_bins, func))
+
+        fit_dict = {}
+
+        for i_peak, uncal_peak_par in enumerate(uncal_peak_pars):
             try:
-                m.minos()
-                valid3 = (
-                    m.valid
-                    & (~np.isnan(m.errors).any())
-                    & (~(np.array(m.errors[:-3]) == 0).all())
+                peak_kev, mode_guess, wwidth_i, n_bins_i, func_i = uncal_peak_par
+                wleft_i, wright_i = wwidth_i
+                euc_min = mode_guess - wleft_i
+                euc_max = mode_guess + wright_i
+
+                if self.uncal_is_int is True:
+                    euc_min, euc_max, n_bins_i = pgh.better_int_binning(
+                        x_lo=euc_min, x_hi=euc_max, n_bins=n_bins_i
+                    )
+
+                energies = e_uncal[(e_uncal > euc_min) & (e_uncal < euc_max)][:n_events]
+                binw_1 = (euc_max - euc_min) / n_bins_i
+
+                x0 = get_hpge_energy_peak_par_guess(
+                    energies,
+                    func_i,
+                    (euc_min, euc_max),
+                    bin_width=binw_1,
+                    mode_guess=mode_guess,
                 )
-            except:
-                raise RuntimeError
 
-        pars = np.array(m.values)[:-1]
-        errs = np.array(m.errors)[:-1]
-        cov = np.array(m.covariance)[:-1, :-1]
-        csqr = cs
-
-    elif valid2 == False or cs * 1.05 < cs2:
-        pars = np.array(m.values)[:-1]
-        errs = np.array(m.errors)[:-3]
-        cov = np.array(m.covariance)[:-1, :-1]
-        csqr = cs
-
-    elif valid1 == False or cs2 * 1.05 < cs:
-        pars = np.array(m2.values)[:-1]
-        errs = np.array(m2.errors)[:-3]
-        cov = np.array(m2.covariance)[:-1, :-1]
-        csqr = cs2
+                euc_min = x0["mu"] - n_sigmas * x0["sigma"]
+                euc_max = x0["mu"] + n_sigmas * x0["sigma"]
 
-    elif frac_errors1 < frac_errors2:
-        pars = np.array(m.values)[:-1]
-        errs = np.array(m.errors)[:-3]
-        cov = np.array(m.covariance)[:-1, :-1]
-        csqr = cs
+                bin_width = (x0["sigma"]) * len(energies) ** (-1 / 3)
+                n_bins_i = int((euc_max - euc_min) / bin_width)
 
-    elif frac_errors1 > frac_errors2:
-        pars = np.array(m2.values)[:-1]
-        errs = np.array(m2.errors)[:-3]
-        cov = np.array(m2.covariance)[:-1, :-1]
-        csqr = cs2
+                if self.uncal_is_int is True:
+                    euc_min, euc_max, n_bins_i = pgh.better_int_binning(
+                        x_lo=euc_min, x_hi=euc_max, n_bins=n_bins_i
+                    )
 
-    else:
-        raise RuntimeError
+                hist, bins, var = pgh.get_hist(
+                    energies, bins=n_bins_i, range=(euc_min, euc_max)
+                )
 
-    return pars, errs, cov, csqr
+                x0["x_lo"] = euc_min
+                x0["x_hi"] = euc_max
 
+                fixed, mask = get_hpge_energy_fixed(func_i)
+                fixed.append("n_bkg")
+                mask[np.where(np.array(func_i.required_args()) == "n_bkg")[0]] = True
+                bounds = get_hpge_energy_bounds(func_i, x0)
+
+                pars_i, errs_i, cov_i = pgb.fit_binned(
+                    func_i.cdf_ext,
+                    hist,
+                    bins,
+                    var=var,
+                    guess=x0,
+                    cost_func="LL",
+                    extended=True,
+                    fixed=fixed,
+                    bounds=bounds,
+                )
+                valid_fit = True
 
-def get_peak_fwhm_with_dt_corr(
-    Energies,
-    alpha,
-    dt,
-    func,
-    gof_func,
-    peak,
-    kev_width,
-    guess=None,
-    kev=False,
-    display=0,
-):
-    """
-    Applies the drift time correction and fits the peak returns the fwhm, fwhm/max and associated errors,
-    along with the number of signal events and the reduced chi square of the fit. Can return result in ADC or keV.
-    """
+                csqr = pgb.goodness_of_fit(
+                    hist,
+                    bins,
+                    None,
+                    func_i.get_pdf,
+                    pars_i,
+                    method="Pearson",
+                    scale_bins=True,
+                )
+                csqr = (csqr[0], csqr[1] + len(np.where(mask)[0]))
 
-    correction = np.multiply(
-        np.multiply(alpha, dt, dtype="float64"), Energies, dtype="float64"
-    )
-    ct_energy = np.add(correction, Energies)
+                if np.isnan(pars_i).any():
+                    log.debug(
+                        f"hpge_cal_energy_peak_tops: fit failed for i_peak={i_peak} at loc {mode_guess:g}, par is nan : {pars_i}"
+                    )
+                    raise RuntimeError
 
-    bin_width = 1
-    lower_bound = (np.nanmin(ct_energy) // bin_width) * bin_width
-    upper_bound = ((np.nanmax(ct_energy) // bin_width) + 1) * bin_width
-    hist, bins, var = pgh.get_hist(
-        ct_energy, dx=bin_width, range=(lower_bound, upper_bound)
-    )
-    mu = bins[np.nanargmax(hist)]
-    adc_to_kev = mu / peak
-    # Making the window slightly smaller removes effects where as mu moves edge can be outside bin width
-    lower_bound = mu - ((kev_width[0] - 2) * adc_to_kev)
-    upper_bound = mu + ((kev_width[1] - 2) * adc_to_kev)
-    win_idxs = (ct_energy > lower_bound) & (ct_energy < upper_bound)
-    fit_range = (lower_bound, upper_bound)
-    if peak > 1500:
-        gof_range = (mu - (7 * adc_to_kev), mu + (7 * adc_to_kev))
-    else:
-        gof_range = (mu - (5 * adc_to_kev), mu + (5 * adc_to_kev))
-    # if kev==True:
-    # else:
-    #    tol=0.01
-    tol = None
-    try:
-        if display > 0:
-            energy_pars, energy_err, cov, chisqr = unbinned_energy_fit(
-                ct_energy[win_idxs],
-                func,
-                gof_func,
-                gof_range,
-                fit_range,
-                tol=tol,
-                guess=guess,
-                verbose=True,
-                display=display,
-            )
-            print(energy_pars)
-            print(energy_err)
-            print(cov)
-            plt.figure()
-            xs = np.arange(lower_bound, upper_bound, bin_width)
-            hist, bins, var = pgh.get_hist(
-                ct_energy, dx=bin_width, range=(lower_bound, upper_bound)
-            )
-            plt.plot((bins[1:] + bins[:-1]) / 2, hist)
-            plt.plot(xs, gof_func(xs, *energy_pars))
-            plt.show()
-        else:
-            energy_pars, energy_err, cov, chisqr = unbinned_energy_fit(
-                ct_energy[win_idxs],
-                func,
-                gof_func,
-                gof_range,
-                fit_range,
-                guess=guess,
-                tol=tol,
-            )
-        if func == pgf.extended_radford_pdf:
-            if energy_pars[3] < 1e-6 and energy_err[3] < 1e-6:
-                fwhm = energy_pars[2] * 2 * np.sqrt(2 * np.log(2))
-                fwhm_err = np.sqrt(cov[2][2]) * 2 * np.sqrt(2 * np.log(2))
-            else:
-                fwhm = pgf.radford_fwhm(energy_pars[2], energy_pars[3], energy_pars[4])
+                p_val = scipy.stats.chi2.sf(csqr[0], csqr[1])
 
-        elif func == pgf.extended_gauss_step_pdf:
-            fwhm = energy_pars[2] * 2 * np.sqrt(2 * np.log(2))
-            fwhm_err = np.sqrt(cov[2][2]) * 2 * np.sqrt(2 * np.log(2))
+                if (
+                    cov_i is None
+                    or cov_i.ndim == 0
+                    or sum(sum(c) for c in cov_i[mask, :][:, mask]) == np.inf
+                    or sum(sum(c) for c in cov_i[mask, :][:, mask]) == 0
+                    or np.isnan(sum(sum(c) for c in cov_i[mask, :][:, mask]))
+                ):
+                    log.debug(
+                        f"hpge_cal_energy_peak_tops: cov estimation failed for i_peak={i_peak} at loc {mode_guess:g}"
+                    )
+                    valid_pk = False
 
-        xs = np.arange(lower_bound, upper_bound, 0.1)
-        y = func(xs, *energy_pars)[1]
-        max_val = np.amax(y)
+                elif valid_fit is False:
+                    log.debug(
+                        f"hpge_cal_energy_peak_tops: peak fitting failed for i_peak={i_peak} at loc {mode_guess:g}"
+                    )
+                    valid_pk = False
 
-        fwhm_o_max = fwhm / max_val
+                elif (
+                    errs_i is None
+                    or pars_i is None
+                    or np.abs(np.array(errs_i)[mask] / np.array(pars_i)[mask]) < 1e-7
+                ).any() or np.isnan(np.array(errs_i)[mask]).any():
+                    log.debug(
+                        f"hpge_cal_energy_peak_tops: failed for i_peak={i_peak} at loc {mode_guess:g}, parameter error too low"
+                    )
+                    valid_pk = False
 
-        rng = np.random.default_rng(1)
-        # generate set of bootstrapped parameters
-        par_b = rng.multivariate_normal(energy_pars, cov, size=100)
-        y_max = np.array([func(xs, *p)[1] for p in par_b])
-        maxs = np.nanmax(y_max, axis=1)
+                elif p_val < allowed_p_val or np.isnan(p_val):
+                    log.debug(
+                        f"hpge_cal_energy_peak_tops: fit failed for i_peak={i_peak}, p-value too low: {p_val}"
+                    )
+                    valid_pk = False
+                else:
+                    valid_pk = True
 
-        yerr_boot = np.nanstd(y_max, axis=0)
+                mu, mu_err = func_i.get_mu(pars_i, errors=errs_i)
 
-        if func == pgf.extended_radford_pdf and not (
-            energy_pars[3] < 1e-6 and energy_err[3] < 1e-6
-        ):
-            y_b = np.zeros(len(par_b))
-            for i, p in enumerate(par_b):
-                try:
-                    y_b[i] = pgf.radford_fwhm(p[2], p[3], p[4])  #
-                except:
-                    y_b[i] = np.nan
-            fwhm_err = np.nanstd(y_b, axis=0)
-            if fwhm_err == 0:
-                fwhm, fwhm_err = pgf.radford_fwhm(
-                    energy_pars[2],
-                    energy_pars[3],
-                    energy_pars[4],
-                    cov=cov[:, :-2][:-2, :],
+            except BaseException as e:
+                if e == KeyboardInterrupt:
+                    raise (e)
+                elif self.debug_mode:
+                    raise (e)
+                log.debug(
+                    f"hpge_fit_energy_peaks: fit failed for i_peak={i_peak}, unknown error"
                 )
-            fwhm_o_max_err = np.nanstd(y_b / maxs, axis=0)
-        else:
-            max_err = np.nanstd(maxs)
-            fwhm_o_max_err = fwhm_o_max * np.sqrt(
-                (np.array(fwhm_err) / np.array(fwhm)) ** 2
-                + (np.array(max_err) / np.array(max_val)) ** 2
-            )
-
-        if display > 1:
-            plt.figure()
-            plt.plot((bins[1:] + bins[:-1]) / 2, hist)
-            for i in range(100):
-                plt.plot(xs, y_max[i, :])
-            plt.show()
-
-        if display > 0:
-            plt.figure()
-            hist, bins, var = pgh.get_hist(
-                ct_energy, dx=bin_width, range=(lower_bound, upper_bound)
-            )
-            plt.plot((bins[1:] + bins[:-1]) / 2, hist)
-            plt.plot(xs, gof_func(xs, *energy_pars))
-            plt.fill_between(
-                xs, y - yerr_boot, y + yerr_boot, facecolor="C1", alpha=0.5
-            )
-            plt.show()
-
-    except:
-        return np.nan, np.nan, np.nan, np.nan, np.nan, np.nan, np.nan, None
-
-    if kev == True:
-        fwhm *= peak / energy_pars[1]
-        fwhm_err *= peak / energy_pars[1]
-
-    return (
-        fwhm,
-        fwhm_o_max,
-        fwhm_err,
-        fwhm_o_max_err,
-        chisqr,
-        energy_pars[0],
-        energy_err[0],
-        energy_pars,
-    )
+                valid_pk = False
+                pars_i, errs_i, cov_i = return_nans(func_i)
+                p_val = 0
+                mu = np.nan
+                mu_err = np.nan
+
+            fit_dict[peak_kev] = {
+                "function": func_i,
+                "validity": valid_pk,
+                "parameters": pars_i,
+                "uncertainties": errs_i,
+                "covariance": cov_i,
+                "nbins": binw_1,
+                "range": [euc_min, euc_max],
+                "p_value": p_val,
+                "position": mu,
+                "position_uncertainty": mu_err,
+            }
 
+        results_dict["peak_parameters"] = fit_dict
 
-def fom_FWHM_with_dt_corr_fit(tb_in, kwarg_dict, ctc_parameter, idxs=None, display=0):
-    """
-    FOM for sweeping over ctc values to find the best value, returns the best found fwhm with its error,
-    the corresponding alpha value and the number of events in the fitted peak, also the reduced chisquare of the
-    """
-    parameter = kwarg_dict["parameter"]
-    func = kwarg_dict["func"]
-    gof_func = kwarg_dict["gof_func"]
-    Energies = tb_in[parameter].nda
-    Energies = Energies.astype("float64")
-    peak = kwarg_dict["peak"]
-    kev_width = kwarg_dict["kev_width"]
-    min_alpha = 0
-    max_alpha = 3.50e-06
-    astep = 1.250e-07
-    if ctc_parameter == "QDrift":
-        dt = tb_in["dt_eff"].nda
-    elif ctc_parameter == "dt":
-        dt = np.subtract(tb_in["tp_99"].nda, tb_in["tp_0_est"].nda, dtype="float64")
-    elif ctc_parameter == "rt":
-        dt = np.subtract(tb_in["tp_99"].nda, tb_in["tp_01"].nda, dtype="float64")
-
-    if idxs is not None:
-        Energies = Energies[idxs]
-        dt = dt[idxs]
+        fitted_peaks_kev = np.array(
+            [peak for peak in fit_dict if fit_dict[peak]["validity"]]
+        )
 
-    if np.isnan(Energies).any():
-        return {
-            "fwhm": np.nan,
-            "fwhm_err": np.nan,
-            "alpha": np.nan,
-            "alpha_err": np.nan,
-            "chisquare": np.nan,
-            "n_sig": np.nan,
-            "n_sig_err": np.nan,
-        }
-    if np.isnan(dt).any():
-        return {
-            "fwhm": np.nan,
-            "fwhm_err": np.nan,
-            "alpha": np.nan,
-            "alpha_err": np.nan,
-            "chisquare": np.nan,
-            "n_sig": np.nan,
-            "n_sig_err": np.nan,
-        }
+        log.info(f"{len(fitted_peaks_kev)} peaks fitted:")
+        for peak, peak_dict in fit_dict.items():
+            if peak_dict["validity"] is True:
+                varnames = peak_dict["function"].required_args()
+                pars = np.asarray(peak_dict["parameters"], dtype=float)
+                errors = np.asarray(peak_dict["uncertainties"], dtype=float)
+                log.info(f"\tEnergy: {str(peak)}")
+                log.info("\t\tParameter  |    Value +/- Sigma  ")
+                for vari, pari, errorsi in zip(varnames, pars, errors):
+                    log.info(
+                        f'\t\t{str(vari).ljust(10)} | {("%4.2f" % pari).rjust(8)} +/- {("%4.2f" % errorsi).ljust(8)}'
+                    )
 
-    alphas = np.array(
-        [
-            0.000e00,
-            1.250e-07,
-            2.500e-07,
-            3.750e-07,
-            5.000e-07,
-            6.250e-07,
-            7.500e-07,
-            8.750e-07,
-            1.000e-06,
-            1.125e-06,
-            1.250e-06,
-            1.375e-06,
-            1.500e-06,
-            1.625e-06,
-            1.750e-06,
-            1.875e-06,
-            2.000e-06,
-            2.125e-06,
-            2.250e-06,
-            2.375e-06,
-            2.500e-06,
-            2.625e-06,
-            2.750e-06,
-            2.875e-06,
-            3.000e-06,
-            3.125e-06,
-            3.250e-06,
-            3.375e-06,
-            3.500e-06,
-        ],
-        dtype="float64",
-    )
-    fwhms = np.array([])
-    final_alphas = np.array([])
-    fwhm_errs = np.array([])
-    guess = None
-    best_fwhm = np.inf
-    for alpha in alphas:
-        (
-            _,
-            fwhm_o_max,
-            _,
-            fwhm_o_max_err,
-            _,
-            _,
-            _,
-            fit_pars,
-        ) = get_peak_fwhm_with_dt_corr(
-            Energies, alpha, dt, func, gof_func, peak, kev_width, guess=guess
-        )
-        if not np.isnan(fwhm_o_max):
-            fwhms = np.append(fwhms, fwhm_o_max)
-            final_alphas = np.append(final_alphas, alpha)
-            fwhm_errs = np.append(fwhm_errs, fwhm_o_max_err)
-            guess = fit_pars
-            if fwhms[-1] < best_fwhm:
-                best_fwhm = fwhms[-1]
-                best_fit = fit_pars
-        log.info(f"alpha: {alpha}, fwhm/max:{fwhm_o_max}+-{fwhm_o_max_err}")
-
-    # Make sure fit isn't based on only a few points
-    if len(fwhms) < 10:
-        log.debug("less than 10 fits successful")
-        return {
-            "fwhm": np.nan,
-            "fwhm_err": np.nan,
-            "alpha": np.nan,
-            "alpha_err": np.nan,
-            "chisquare": np.nan,
-            "n_sig": np.nan,
-            "n_sig_err": np.nan,
-        }
+        if len(fitted_peaks_kev) == 0:
+            log.error("hpge_fit_energy_peaks: no peaks fitted")
+            self.update_results_dict(results_dict)
+            return
+
+        mus = [
+            fit_dict[peak]["position"]
+            for peak in fit_dict
+            if fit_dict[peak]["validity"]
+        ]
+        mu_vars = [
+            fit_dict[peak]["position_uncertainty"]
+            for peak in fit_dict
+            if fit_dict[peak]["validity"]
+        ]
+
+        mus = results_dict["pk_pos"] = np.asarray(mus)
+        mu_vars = results_dict["pk_pos_uncertainties"] = np.asarray(mu_vars) ** 2
+
+        if update_cal_pars is False:
+            self.update_results_dict(results_dict)
+            return
 
-    ids = (fwhm_errs < 2 * np.nanpercentile(fwhm_errs, 50)) & (fwhm_errs > 0)
-    # Fit alpha curve to get best alpha
+        self.peaks_kev = np.asarray(fitted_peaks_kev)
+        self.peak_locs = np.asarray(mus)
 
-    try:
-        alphas = np.arange(
-            final_alphas[ids][0], final_alphas[ids][-1], astep / 20, dtype="float64"
-        )
-        alpha_fit, cov = np.polyfit(
-            final_alphas[ids], fwhms[ids], w=1 / fwhm_errs[ids], deg=4, cov=True
-        )
-        fit_vals = np.polynomial.polynomial.polyval(alphas, alpha_fit[::-1])
-        alpha = alphas[np.nanargmin(fit_vals)]
-
-        rng = np.random.default_rng(1)
-        alpha_pars_b = rng.multivariate_normal(alpha_fit, cov, size=1000)
-        fits = np.array(
-            [
-                np.polynomial.polynomial.polyval(alphas, pars[::-1])
-                for pars in alpha_pars_b
-            ]
-        )
-        min_alphas = np.array([alphas[np.nanargmin(fit)] for fit in fits])
-        alpha_err = np.nanstd(min_alphas)
-        if display > 0:
-            plt.figure()
-            yerr_boot = np.std(fits, axis=0)
-            plt.errorbar(final_alphas, fwhms, yerr=fwhm_errs, linestyle=" ")
-            plt.plot(alphas, fit_vals)
-            plt.fill_between(
-                alphas,
-                fit_vals - yerr_boot,
-                fit_vals + yerr_boot,
-                facecolor="C1",
-                alpha=0.5,
+        # Now fit the E scale
+        try:
+            pars, errs, cov = hpge_fit_energy_scale(
+                mus, mu_vars, fitted_peaks_kev, deg=self.deg, fixed=self.fixed
             )
-            plt.show()
 
-    except:
-        log.debug("alpha fit failed")
-        return {
-            "fwhm": np.nan,
-            "fwhm_err": np.nan,
-            "alpha": np.nan,
-            "alpha_err": np.nan,
-            "chisquare": np.nan,
-            "n_sig": np.nan,
-            "n_sig_err": np.nan,
-        }
+            results_dict["pk_cal_pars"] = pars
+            results_dict["pk_cal_errs"] = errs
+            results_dict["pk_cal_cov"] = cov
+
+            # Invert the E scale fit to get a calibration function
+            pars, errs, cov = hpge_fit_energy_cal_func(
+                mus,
+                mu_vars,
+                fitted_peaks_kev,
+                pars,
+                deg=self.deg,
+                fixed=self.fixed,
+            )
+            self.pars = np.array(pars)
+
+        except ValueError:
+            log.error("Failed to fit enough peaks to get accurate calibration")
+
+        self.update_results_dict(results_dict)
+
+    def hpge_fit_energy_peaks(
+        self,
+        e_uncal,
+        peak_pars=None,
+        peaks_kev=None,
+        bin_width_kev=1,
+        peak_param="mode",
+        method="unbinned",
+        n_events=None,
+        allowed_p_val=0.01,
+        tail_weight=0,
+        update_cal_pars=True,
+        use_bin_width_in_fit=True,
+    ):
+        """
+        Fit the energy peaks specified using the given function.
+
+        Parameters
+        ----------
+        e_uncal : array
+            Unbinned energy data to be fit.
+        peaks_kev : array, optional
+            Array of energy values for the peaks to fit. If not provided, it uses the peaks_kev attribute of the class.
+        peak_pars : list of tuples, optional
+            List containing tuples of the form (peak, range, func) where peak is the energy of the peak to fit,
+            range is the range in keV to fit, and func is the function to fit.
+        bin_width_kev : int, optional
+            Default binwidth to use for the fit window histogramming. Default is 1 keV.
+        peak_param : str, optional
+            Parameter to use for peak fitting. Default is "mode".
+        method : str, optional
+            Method to use for fitting. Default is "unbinned". Can specify to use binned fit method instead.
+        n_events : int, optional
+            Number of events to use for unbinned fit.
+        allowed_p_val : float, optional
+            Lower limit on p-value of fit.
+        tail_weight : int, optional
+            Weight to apply to the tail of the fit.
+        update_cal_pars : bool, optional
+            Whether to update the calibration parameters. Default is True.
+
+        Returns
+        -------
+        results_dict : dict
+            Dictionary containing the fit results for each peak.
+
+        Raises
+        ------
+        RuntimeError
+            If the fit fails.
+
+        Notes
+        -----
+        This function fits the energy peaks specified using the given function. It calculates the range around each peak to fit,
+        performs the fitting using either unbinned or binned method, and returns the fit results in a dictionary.
+
+        """
+
+        results_dict = {}
+        # check no peaks in self.peaks_kev missing from peak_pars
+
+        if peaks_kev is None:
+            peaks_kev = self.peaks_kev
+
+        if peak_pars is None:
+            peak_pars = [(peak, None, pgf.gauss_on_step) for peak in peaks_kev]
+
+        # convert peak pars to array of tuples
+        tmp = np.empty(len(peak_pars), dtype=object)
+        tmp[:] = peak_pars
+        peak_pars = tmp
+
+        peak_pars_lines = [i[0] for i in peak_pars]
+        peaks_mask = np.array(
+            [True if peak in peaks_kev else False for peak in peak_pars_lines],
+            dtype=bool,
+        )
+        peak_pars = peak_pars[peaks_mask]
 
-    if np.isnan(fit_vals).all():
-        log.debug("alpha fit all nan")
-        return {
-            "fwhm": np.nan,
-            "fwhm_err": np.nan,
-            "alpha": np.nan,
-            "alpha_err": np.nan,
-            "chisquare": np.nan,
-            "n_sig": np.nan,
-            "n_sig_err": np.nan,
-        }
+        fit_peaks_mask = np.array(
+            [True for i in peak_pars if i[1] is not None and i[2] is not None],
+            dtype=bool,
+        )
+        peak_pars = peak_pars[fit_peaks_mask]
 
-    else:
-        # Return fwhm of optimal alpha in kev with error
-        (
-            final_fwhm,
-            _,
-            final_err,
-            _,
-            csqr,
-            n_sig,
-            n_sig_err,
-            _,
-        ) = get_peak_fwhm_with_dt_corr(
-            Energies,
-            alpha,
-            dt,
-            func,
-            gof_func,
-            peak,
-            kev_width,
-            guess=best_fit,
-            kev=True,
-            display=display,
-        )
-        if np.isnan(final_fwhm) or np.isnan(final_err):
-            (
-                final_fwhm,
-                _,
-                final_err,
-                _,
-                csqr,
-                n_sig,
-                n_sig_err,
-                _,
-            ) = get_peak_fwhm_with_dt_corr(
-                Energies,
-                alpha,
-                dt,
-                func,
-                gof_func,
-                peak,
-                kev_width,
-                kev=True,
-                display=display,
-            )
-        if np.isnan(final_fwhm) or np.isnan(final_err):
-            log.debug(f"final fit failed, alpha was {alpha}")
-        return {
-            "fwhm": final_fwhm,
-            "fwhm_err": final_err,
-            "alpha": alpha,
-            "alpha_err": alpha_err,
-            "chisquare": csqr,
-            "n_sig": n_sig,
-            "n_sig_err": n_sig_err,
-        }
+        # First calculate range around peaks to fit
 
+        uncal_peak_pars = []
+        derco = Polynomial(self.pars).deriv().coef
+        for pars in peak_pars:
+            peak, fit_range, func = pars
 
-def fom_all_fit(tb_in, kwarg_dict):
-    """
-    FOM to run over different ctc parameters
-    """
-    ctc_parameters = ["QDrift"]  #'dt',
-    output_dict = {}
-    for param in ctc_parameters:
-        out = fom_FWHM_with_dt_corr_fit(tb_in, kwarg_dict, param)
-        output_dict[param] = out
-    return output_dict
+            if peak in self.peaks_kev:
+                loc = self.peak_locs[np.where(peak == self.peaks_kev)][0]
+            else:
+                loc = (Polynomial(self.pars) - peak).roots()[0]
 
+            if fit_range is None:
+                euc_min, euc_max = (
+                    (Polynomial(self.pars) - i).roots()
+                    for i in (peaks_kev[0] * 0.9, peaks_kev[-1] * 1.1)
+                )
+                euc_min = euc_min[0]
+                euc_max = euc_max[0]
+                if euc_min < 0:
+                    euc_min = 0
+                if euc_max > np.nanmax(e_uncal) * 1.1:
+                    euc_max = np.nanmax(e_uncal) * 1.1
+                d_euc = 0.5 / self.pars[1]
+                if self.uncal_is_int:
+                    euc_min, euc_max, d_euc = pgh.better_int_binning(
+                        x_lo=euc_min, x_hi=euc_max, dx=d_euc
+                    )
+                hist, bins, var = pgh.get_hist(
+                    e_uncal, range=(euc_min, euc_max), dx=d_euc
+                )
+                # Need to do initial fit
+                pt_pars, _ = hpge_fit_energy_peak_tops(
+                    hist, bins, var, [loc], n_to_fit=7
+                )
+                # Drop failed fits
+                if pt_pars[0] is not None:
+                    range_uncal = (float(pt_pars[0][1]) * 20, float(pt_pars[0][1]) * 20)
+                    n_bins = int(range_uncal / bin_width_kev)
+                else:
+                    range_uncal = None
+            elif isinstance(fit_range, tuple):
+                der = pgf.nb_poly(peak, derco)
+                range_uncal = (fit_range[0] / der, fit_range[1] / der)
+                n_bins = int(sum(fit_range) / (der * bin_width_kev))
+
+            if range_uncal is not None:
+                uncal_peak_pars.append((peak, loc, range_uncal, n_bins, func))
+
+        fit_dict = {}
+
+        for i_peak, uncal_peak_par in enumerate(uncal_peak_pars):
+            peak_kev, mode_guess, wwidth_i, n_bins_i, func_i = uncal_peak_par
+            wleft_i, wright_i = wwidth_i
+            try:
+                euc_min = mode_guess - wleft_i
+                euc_max = mode_guess + wright_i
 
-def fom_FWHM_fit(tb_in, kwarg_dict):
-    """
-    FOM with no ctc sweep, used for optimising ftp.
-    """
-    parameter = kwarg_dict["parameter"]
-    func = kwarg_dict["func"]
-    gof_func = kwarg_dict["gof_func"]
-    Energies = tb_in[parameter].nda
-    Energies = Energies.astype("float64")
-    peak = kwarg_dict["peak"]
-    kev_width = kwarg_dict["kev_width"]
-    try:
-        alpha = kwarg_dict["alpha"]
-        if isinstance(alpha, dict):
-            alpha = alpha[parameter]
-    except KeyError:
-        alpha = 0
-    try:
-        ctc_param = kwarg_dict["ctc_param"]
-        dt = tb_in[ctc_param].nda
-    except KeyError:
-        dt = 0
+                if self.uncal_is_int is True:
+                    euc_min, euc_max, n_bins_i = pgh.better_int_binning(
+                        x_lo=euc_min, x_hi=euc_max, n_bins=n_bins_i
+                    )
+                energies = e_uncal[(e_uncal > euc_min) & (e_uncal < euc_max)][:n_events]
+                binw_1 = (euc_max - euc_min) / n_bins_i
+                if method == "unbinned":
+                    (
+                        pars_i,
+                        errs_i,
+                        cov_i,
+                        csqr_i,
+                        func_i,
+                        mask,
+                        valid_fit,
+                        _,
+                    ) = unbinned_staged_energy_fit(
+                        energies,
+                        func=func_i,
+                        fit_range=(euc_min, euc_max),
+                        guess_func=get_hpge_energy_peak_par_guess,
+                        bounds_func=get_hpge_energy_bounds,
+                        fixed_func=get_hpge_energy_fixed,
+                        allow_tail_drop=True,
+                        tail_weight=tail_weight,
+                        bin_width=binw_1 if use_bin_width_in_fit is True else None,
+                        guess_kwargs={"mode_guess": mode_guess},
+                    )
+                    if pars_i["n_sig"] < 100:
+                        valid_fit = False
+                    csqr = csqr_i
 
-    if np.isnan(Energies).any():
-        return {
-            "fwhm_o_max": np.nan,
-            "max_o_fwhm": np.nan,
-            "chisquare": np.nan,
-            "n_sig": np.nan,
-            "n_sig_err": np.nan,
-        }
+                else:
+                    hist, bins, var = pgh.get_hist(
+                        energies, bins=n_bins_i, range=(euc_min, euc_max)
+                    )
+                    binw_1 = (bins[-1] - bins[0]) / (len(bins) - 1)
+                    par_guesses = get_hpge_energy_peak_par_guess(
+                        hist, bins, var, func_i, mode_guess=mode_guess
+                    )
+                    bounds = get_hpge_energy_bounds(func_i, par_guesses)
+                    fixed, mask = get_hpge_energy_fixed(func_i)
 
-    (
-        _,
-        final_fwhm_o_max,
-        _,
-        final_fwhm_o_max_err,
-        csqr,
-        n_sig,
-        n_sig_err,
-    ) = get_peak_fwhm_with_dt_corr(
-        Energies, alpha, dt, func, gof_func, peak=peak, kev_width=kev_width, kev=True
-    )
-    return {
-        "fwhm_o_max": final_fwhm_o_max,
-        "max_o_fwhm": final_fwhm_o_max_err,
-        "chisquare": csqr,
-        "n_sig": n_sig,
-        "n_sig_err": n_sig_err,
-    }
-
-
-def get_wf_indexes(sorted_indexs, n_events):
-    out_list = []
-    if isinstance(n_events, list):
-        for i in range(len(n_events)):
-            new_list = []
-            for idx, entry in enumerate(sorted_indexs):
-                if (entry >= np.sum(n_events[:i])) and (
-                    entry < np.sum(n_events[: i + 1])
+                    x0 = get_hpge_energy_peak_par_guess(
+                        energies, func_i, (euc_min, euc_max), bin_width=binw_1
+                    )
+                    fixed, mask = get_hpge_energy_fixed(func_i)
+                    bounds = get_hpge_energy_bounds(func_i, x0)
+
+                    pars_i, errs_i, cov_i = pgb.fit_binned(
+                        func_i.get_pdf,
+                        hist,
+                        bins,
+                        var=var,
+                        guess=x0,
+                        cost_func=method,
+                        extended=True,
+                        fixed=fixed,
+                        bounds=bounds,
+                    )
+                    valid_fit = True
+
+                    csqr = pgb.goodness_of_fit(
+                        hist,
+                        bins,
+                        None,
+                        func_i.get_pdf,
+                        pars_i,
+                        method="Pearson",
+                        scale_bins=True,
+                    )
+                    csqr = (csqr[0], csqr[1] + len(np.where(mask)[0]))
+
+                if np.isnan(pars_i).any():
+                    log.debug(
+                        f"hpge_fit_energy_peaks: fit failed for i_peak={i_peak} at loc {mode_guess:g}, par is nan : {pars_i}"
+                    )
+                    raise RuntimeError
+
+                p_val = scipy.stats.chi2.sf(csqr[0], csqr[1])
+
+                total_events = func_i.get_total_events(pars_i, errors=errs_i)
+                if (
+                    cov_i is None
+                    or cov_i.ndim == 0
+                    or sum(sum(c) for c in cov_i[mask, :][:, mask]) == np.inf
+                    or sum(sum(c) for c in cov_i[mask, :][:, mask]) == 0
+                    or np.isnan(sum(sum(c) for c in cov_i[mask, :][:, mask]))
                 ):
-                    new_list.append(idx)
-            out_list.append(new_list)
-    else:
-        for i in range(int(len(sorted_indexs) / n_events)):
-            new_list = []
-            for idx, entry in enumerate(sorted_indexs):
-                if (entry >= i * n_events) and (entry < (i + 1) * n_events):
-                    new_list.append(idx)
-            out_list.append(new_list)
-    return out_list
-
-
-def index_data(data, indexes, wf_field="waveform"):
-    new_baselines = lh5.Array(data["baseline"].nda[indexes])
-    new_waveform_values = data[wf_field]["values"].nda[indexes]
-    new_waveform_dts = data[wf_field]["dt"].nda[indexes]
-    new_waveform_t0 = data[wf_field]["t0"].nda[indexes]
-    new_waveform = lh5.WaveformTable(
-        None, new_waveform_t0, "ns", new_waveform_dts, "ns", new_waveform_values
-    )
-    new_data = lh5.Table(col_dict={wf_field: new_waveform, "baseline": new_baselines})
-    return new_data
+                    log.debug(
+                        f"hpge_fit_energy_peaks: cov estimation failed for i_peak={i_peak} at loc {mode_guess:g}"
+                    )
+                    valid_pk = False
 
+                elif valid_fit is False:
+                    log.debug(
+                        f"hpge_fit_energy_peaks: peak fitting failed for i_peak={i_peak} at loc {mode_guess:g}"
+                    )
+                    valid_pk = False
 
-def event_selection(
-    raw_files,
-    lh5_path,
-    dsp_config,
-    db_dict,
-    peaks_keV,
-    peak_idxs,
-    kev_widths,
-    cut_parameters={"bl_mean": 4, "bl_std": 4, "pz_std": 4},
-    pulser_mask=None,
-    energy_parameter="trapTmax",
-    wf_field: str = "waveform",
-    n_events=10000,
-    threshold=1000,
-):
-    if not isinstance(peak_idxs, list):
-        peak_idxs = [peak_idxs]
-    if not isinstance(kev_widths, list):
-        kev_widths = [kev_widths]
-
-    df = sto.read(lh5_path, raw_files, field_mask=["daqenergy", "timestamp"])[
-        0
-    ].view_as("pd")
-
-    if pulser_mask is None:
-        pulser_props = cts.find_pulser_properties(df, energy="daqenergy")
-        if len(pulser_props) > 0:
-            final_mask = None
-            for entry in pulser_props:
-                e_cut = (df.daqenergy.values < entry[0] + entry[1]) & (
-                    df.daqenergy.values > entry[0] - entry[1]
-                )
-                if final_mask is None:
-                    final_mask = e_cut
+                elif (
+                    errs_i is None
+                    or pars_i is None
+                    or np.abs(np.array(errs_i)[mask] / np.array(pars_i)[mask]) < 1e-7
+                ).any() or np.isnan(np.array(errs_i)[mask]).any():
+                    log.debug(
+                        f"hpge_fit_energy_peaks: failed for i_peak={i_peak} at loc {mode_guess:g}, parameter error too low"
+                    )
+                    valid_pk = False
+
+                elif np.abs(total_events[0] - len(energies)) / len(energies) > 0.1:
+                    log.debug(
+                        f"hpge_fit_energy_peaks: fit failed for i_peak={i_peak} at loc {mode_guess:g}, total_events is outside limit"
+                    )
+                    valid_pk = False
+
+                elif p_val < allowed_p_val or np.isnan(p_val):
+                    log.debug(
+                        f"hpge_fit_energy_peaks: fit failed for i_peak={i_peak}, p-value too low: {p_val}"
+                    )
+                    valid_pk = False
                 else:
-                    final_mask = final_mask | e_cut
-            ids = final_mask
-            log.debug(f"pulser found: {pulser_props}")
-        else:
-            log.debug("no_pulser")
-            ids = np.zeros(len(df.daqenergy.values), dtype=bool)
-        # Get events around peak using raw file values
-    else:
-        ids = pulser_mask
-    initial_mask = (df.daqenergy.values > threshold) & (~ids)
-    rough_energy = df.daqenergy.values[initial_mask]
-    initial_idxs = np.where(initial_mask)[0]
-
-    guess_keV = 2620 / np.nanpercentile(rough_energy, 99)
-    Euc_min = threshold / guess_keV * 0.6
-    Euc_max = 2620 / guess_keV * 1.1
-    dEuc = 1  # / guess_keV
-    hist, bins, var = pgh.get_hist(rough_energy, range=(Euc_min, Euc_max), dx=dEuc)
-    detected_peaks_locs, detected_peaks_keV, roughpars = pgc.hpge_find_E_peaks(
-        hist,
-        bins,
-        var,
-        np.array([238.632, 583.191, 727.330, 860.564, 1620.5, 2103.53, 2614.553]),
-    )
-    log.debug(f"detected {detected_peaks_keV} keV peaks at {detected_peaks_locs}")
+                    valid_pk = True
 
-    masks = []
-    for peak_idx in peak_idxs:
-        peak = peaks_keV[peak_idx]
-        kev_width = kev_widths[peak_idx]
-        try:
-            if peak not in detected_peaks_keV:
-                raise ValueError
-            detected_peak_idx = np.where(detected_peaks_keV == peak)[0]
-            peak_loc = detected_peaks_locs[detected_peak_idx]
-            log.info(f"{peak} peak found at {peak_loc}")
-            rough_adc_to_kev = roughpars[0]
-            e_lower_lim = peak_loc - (1.1 * kev_width[0]) / rough_adc_to_kev
-            e_upper_lim = peak_loc + (1.1 * kev_width[1]) / rough_adc_to_kev
-        except:
-            log.debug(f"{peak} peak not found attempting to use rough parameters")
-            peak_loc = (peak - roughpars[1]) / roughpars[0]
-            rough_adc_to_kev = roughpars[0]
-            e_lower_lim = peak_loc - (1.5 * kev_width[0]) / rough_adc_to_kev
-            e_upper_lim = peak_loc + (1.5 * kev_width[1]) / rough_adc_to_kev
-        log.debug(f"lower_lim:{e_lower_lim}, upper_lim:{e_upper_lim}")
-        e_mask = (rough_energy > e_lower_lim) & (rough_energy < e_upper_lim)
-        e_idxs = initial_idxs[e_mask][: int(2.5 * n_events)]
-        masks.append(e_idxs)
-        log.debug(f"{len(e_idxs)} events found in energy range for {peak}")
-
-    idx_list_lens = [len(masks[peak_idx]) for peak_idx in peak_idxs]
-
-    sort_index = np.argsort(np.concatenate(masks))
-    idx_list = get_wf_indexes(sort_index, idx_list_lens)
-    idxs = np.array(sorted(np.concatenate(masks)))
-
-    input_data = sto.read(f"{lh5_path}", raw_files, idx=idxs, n_rows=len(idxs))[0]
-
-    if isinstance(dsp_config, str):
-        with open(dsp_config) as r:
-            dsp_config = json.load(r)
-
-    dsp_config["outputs"] = cts.get_keys(
-        dsp_config["outputs"], list(cut_parameters)
-    ) + [energy_parameter]
-
-    log.debug("Processing data")
-    tb_data = opt.run_one_dsp(input_data, dsp_config, db_dict=db_dict)
-
-    cut_dict = cts.generate_cuts(tb_data, cut_parameters)
-    log.debug(f"Cuts are: {cut_dict}")
-    log.debug("Loaded Cuts")
-    ct_mask = cts.get_cut_indexes(tb_data, cut_dict)
-
-    final_events = []
-    out_events = []
-    for peak_idx in peak_idxs:
-        peak = peaks_keV[peak_idx]
-        kev_width = kev_widths[peak_idx]
-
-        peak_ids = np.array(idx_list[peak_idx])
-        peak_ct_mask = ct_mask[peak_ids]
-        peak_ids = peak_ids[peak_ct_mask]
-
-        energy = tb_data[energy_parameter].nda[peak_ids]
-
-        hist, bins, var = pgh.get_hist(
-            energy, range=(int(threshold), int(np.nanmax(energy))), dx=1
-        )
-        peak_loc = pgh.get_bin_centers(bins)[np.nanargmax(hist)]
-        rough_adc_to_kev = peak / peak_loc
-
-        e_lower_lim = peak_loc - (1.5 * kev_width[0]) / rough_adc_to_kev
-        e_upper_lim = peak_loc + (1.5 * kev_width[1]) / rough_adc_to_kev
-
-        e_ranges = (int(peak_loc - e_lower_lim), int(e_upper_lim - peak_loc))
-        (
-            params,
-            errors,
-            covs,
-            bins,
-            ranges,
-            p_val,
-            valid_pks,
-            pk_funcs,
-        ) = pgc.hpge_fit_E_peaks(
-            energy,
-            [peak_loc],
-            [e_ranges],
-            n_bins=(np.nanmax(energy) - np.nanmin(energy)) // 1,
-            uncal_is_int=True,
-        )
-        if params[0] is None or np.isnan(params[0]).any():
-            log.debug("Fit failed, using max guess")
-            hist, bins, var = pgh.get_hist(
-                energy, range=(int(e_lower_lim), int(e_upper_lim)), dx=1
-            )
-            params = [[0, pgh.get_bin_centers(bins)[np.nanargmax(hist)], 0, 0, 0, 0]]
-        updated_adc_to_kev = peak / params[0][1]
-        e_lower_lim = params[0][1] - (kev_width[0]) / updated_adc_to_kev
-        e_upper_lim = params[0][1] + (kev_width[1]) / updated_adc_to_kev
-        log.info(f"lower lim is :{e_lower_lim}, upper lim is {e_upper_lim}")
-        final_mask = (energy > e_lower_lim) & (energy < e_upper_lim)
-        final_events.append(peak_ids[final_mask][:n_events])
-        out_events.append(idxs[final_events[-1]])
-        log.info(f"{len(peak_ids[final_mask][:n_events])} passed selections for {peak}")
-        if len(peak_ids[final_mask]) < 0.5 * n_events:
-            log.warning("Less than half number of specified events found")
-        elif len(peak_ids[final_mask]) < 0.1 * n_events:
-            log.error("Less than 10% number of specified events found")
-    out_events = np.unique(np.concatenate(out_events))
-    sort_index = np.argsort(np.concatenate(final_events))
-    idx_list = get_wf_indexes(sort_index, [len(mask) for mask in final_events])
-    return out_events, idx_list
+                if peak_param == "mu":
+                    mu, mu_err = func_i.get_mu(pars_i, errors=errs_i)
 
+                elif peak_param == "mode":
+                    mu, mu_err = func_i.get_mode(pars_i, cov=cov_i)
+                else:
+                    log.error(
+                        f"hpge_fit_energy_peaks: mode {self.peak_param} not recognized"
+                    )
+                    raise RuntimeError
 
-def fwhm_slope(x, m0, m1, m2):
-    """
-    Fit the energy resolution curve
-    """
-    return np.sqrt(m0 + m1 * x + m2 * (x**2))
+            except BaseException as e:
+                if e == KeyboardInterrupt:
+                    raise (e)
+                elif self.debug_mode:
+                    raise (e)
+                log.debug(
+                    f"hpge_fit_energy_peaks: fit failed for i_peak={i_peak}, unknown error"
+                )
+                valid_pk = False
+                pars_i, errs_i, cov_i = return_nans(func_i)
+                p_val = 0
+                mu = np.nan
+                mu_err = np.nan
+
+            fit_dict[peak_kev] = {
+                "function": func_i,
+                "validity": valid_pk,
+                "parameters": pars_i,
+                "uncertainties": errs_i,
+                "covariance": cov_i,
+                "nbins": binw_1,
+                "range": [euc_min, euc_max],
+                "p_value": p_val,
+                "position": mu,
+                "position_uncertainty": mu_err,
+            }
 
+        results_dict["peak_parameters"] = fit_dict
 
-def interpolate_energy(peak_energies, points, err_points, energy):
-    nan_mask = np.isnan(points) | (points < 0)
-    if len(points[~nan_mask]) < 3:
-        return np.nan, np.nan, np.nan
-    else:
-        param_guess = [2, 0.001, 0.000001]  #
-        # param_bounds = (0, [10., 1. ])#
-        try:
-            fit_pars, fit_covs = curve_fit(
-                fwhm_slope,
-                peak_energies[~nan_mask],
-                points[~nan_mask],
-                sigma=err_points[~nan_mask],
-                p0=param_guess,
-                absolute_sigma=True,
-            )  # bounds=param_bounds,
-            fit_qbb = fwhm_slope(energy, *fit_pars)
-
-            xs = np.arange(peak_energies[0], peak_energies[-1], 0.1)
-
-            rng = np.random.default_rng(1)
-
-            # generate set of bootstrapped parameters
-            par_b = rng.multivariate_normal(fit_pars, fit_covs, size=1000)
-            qbb_vals = np.array([fwhm_slope(energy, *p) for p in par_b])
-            qbb_err = np.nanstd(qbb_vals)
-        except:
-            return np.nan, np.nan, np.nan
-
-        if nan_mask[-1] == True or nan_mask[-2] == True:
-            qbb_err = np.nan
-        if qbb_err / fit_qbb > 0.1:
-            qbb_err = np.nan
+        fitted_peaks_kev = np.array(
+            [peak for peak in fit_dict if fit_dict[peak]["validity"]]
+        )
 
-    return fit_qbb, qbb_err, fit_pars
+        log.info(f"{len(fitted_peaks_kev)} peaks fitted:")
+        for peak, peak_dict in fit_dict.items():
+            if peak_dict["validity"] is True:
+                varnames = peak_dict["function"].required_args()
+                pars = np.asarray(peak_dict["parameters"], dtype=float)
+                errors = np.asarray(peak_dict["uncertainties"], dtype=float)
+                log.info(f"\tEnergy: {str(peak)}")
+                log.info("\t\tParameter  |    Value +/- Sigma  ")
+                for vari, pari, errorsi in zip(varnames, pars, errors):
+                    log.info(
+                        f'\t\t{str(vari).ljust(10)} | {("%4.2f" % pari).rjust(8)} +/- {("%4.2f" % errorsi).ljust(8)}'
+                    )
 
+        if len(fitted_peaks_kev) == 0:
+            log.error("hpge_fit_energy_peaks: no peaks fitted")
+            self.update_results_dict(results_dict)
+            return
+
+        mus = [
+            fit_dict[peak]["position"]
+            for peak in fit_dict
+            if fit_dict[peak]["validity"]
+        ]
+        mu_vars = [
+            fit_dict[peak]["position_uncertainty"]
+            for peak in fit_dict
+            if fit_dict[peak]["validity"]
+        ]
+
+        results_dict["peak_param"] = peak_param
+        mus = results_dict["pk_pos"] = np.asarray(mus)
+        mu_vars = results_dict["pk_pos_uncertainties"] = np.asarray(mu_vars) ** 2
+
+        if update_cal_pars is False:
+            self.update_results_dict(results_dict)
+            return
 
-def fom_FWHM(tb_in, kwarg_dict, ctc_parameter, alpha, idxs=None, display=0):
-    """
-    FOM for sweeping over ctc values to find the best value, returns the best found fwhm
-    """
-    parameter = kwarg_dict["parameter"]
-    func = kwarg_dict["func"]
-    cs_func = kwarg_dict["gof_func"]
-    Energies = tb_in[parameter].nda
-    Energies = Energies.astype("float64")
-    peak = kwarg_dict["peak"]
-    kev_width = kwarg_dict["kev_width"]
-
-    if ctc_parameter == "QDrift":
-        dt = tb_in["dt_eff"].nda
-    elif ctc_parameter == "dt":
-        dt = np.subtract(tb_in["tp_99"].nda, tb_in["tp_0_est"].nda, dtype="float64")
-    elif ctc_parameter == "rt":
-        dt = np.subtract(tb_in["tp_99"].nda, tb_in["tp_01"].nda, dtype="float64")
-    if np.isnan(Energies).any() or np.isnan(dt).any():
-        if np.isnan(Energies).any():
-            log.debug(f"nan energy values for peak {peak}")
-        else:
-            log.debug(f"nan dt values for peak {peak}")
-        return {
-            "fwhm": np.nan,
-            "fwhm_err": np.nan,
-            "alpha": np.nan,
-            "chisquare": np.nan,
-            "n_sig": np.nan,
-            "n_sig_err": np.nan,
-        }
+        self.peaks_kev = np.asarray(fitted_peaks_kev)
+        self.peak_locs = np.asarray(mus)
 
-    if idxs is not None:
-        Energies = Energies[idxs]
-        dt = dt[idxs]
-
-    # Return fwhm of optimal alpha in kev with error
-    try:
-        (
-            final_fwhm,
-            _,
-            final_err,
-            _,
-            csqr,
-            n_sig,
-            n_sig_err,
-            _,
-        ) = get_peak_fwhm_with_dt_corr(
-            Energies,
-            alpha,
-            dt,
-            func,
-            cs_func,
-            peak,
-            kev_width,
-            kev=True,
-            display=display,
-        )
-    except:
-        final_fwhm = np.nan
-        final_err = np.nan
-        csqr = np.nan
-        n_sig = np.nan
-        n_sig_err = np.nan
-    return {
-        "fwhm": final_fwhm,
-        "fwhm_err": final_err,
-        "alpha": alpha,
-        "chisquare": csqr,
-        "n_sig": n_sig,
-        "n_sig_err": n_sig_err,
-    }
-
-
-def single_peak_fom(data, kwarg_dict):
-    peaks = kwarg_dict["peaks_keV"]
-    idx_list = kwarg_dict["idx_list"]
-    ctc_param = kwarg_dict["ctc_param"]
-    peak_dicts = kwarg_dict["peak_dicts"]
+        # Now fit the E scale
+        try:
+            pars, errs, cov = hpge_fit_energy_scale(
+                mus, mu_vars, fitted_peaks_kev, deg=self.deg, fixed=self.fixed
+            )
 
-    out_dict = fom_FWHM_with_dt_corr_fit(
-        data, peak_dicts[0], ctc_param, idxs=idx_list[0], display=0
-    )
-    out_dict["y_val"] = out_dict["fwhm"]
-    out_dict["y_err"] = out_dict["fwhm_err"]
-    return out_dict
+            results_dict["pk_cal_pars"] = pars
+            results_dict["pk_cal_errs"] = errs
+            results_dict["pk_cal_cov"] = cov
 
+            # Invert the E scale fit to get a calibration function
+            pars, errs, cov = hpge_fit_energy_cal_func(
+                mus,
+                mu_vars,
+                fitted_peaks_kev,
+                pars,
+                deg=self.deg,
+                fixed=self.fixed,
+            )
+            self.pars = np.array(pars)
 
-def new_fom(data, kwarg_dict):
-    peaks = kwarg_dict["peaks_keV"]
-    idx_list = kwarg_dict["idx_list"]
-    ctc_param = kwarg_dict["ctc_param"]
+        except ValueError:
+            log.error("Failed to fit enough peaks to get accurate calibration")
 
-    peak_dicts = kwarg_dict["peak_dicts"]
+        self.update_results_dict(results_dict)
 
-    out_dict = fom_FWHM_with_dt_corr_fit(
-        data, peak_dicts[-1], ctc_param, idxs=idx_list[-1], display=0
-    )
-    alpha = out_dict["alpha"]
-    log.info(alpha)
-    fwhms = []
-    fwhm_errs = []
-    n_sig = []
-    n_sig_err = []
-    for i, peak in enumerate(peaks[:-1]):
-        out_peak_dict = fom_FWHM(
-            data, peak_dicts[i], ctc_param, alpha, idxs=idx_list[i], display=0
-        )
-        # n_sig_minimum = peak_dicts[i]["n_sig_minimum"]
-        # if peak_dict["n_sig"]<n_sig_minimum:
-        #    out_peak_dict['fwhm'] = np.nan
-        #   out_peak_dict['fwhm_err'] = np.nan
-        fwhms.append(out_peak_dict["fwhm"])
-        fwhm_errs.append(out_peak_dict["fwhm_err"])
-        n_sig.append(out_peak_dict["n_sig"])
-        n_sig_err.append(out_peak_dict["n_sig_err"])
-    fwhms.append(out_dict["fwhm"])
-    fwhm_errs.append(out_dict["fwhm_err"])
-    n_sig.append(out_dict["n_sig"])
-    n_sig_err.append(out_dict["n_sig_err"])
-    log.info(f"fwhms are {fwhms}keV +- {fwhm_errs}")
-    qbb, qbb_err, fit_pars = interpolate_energy(
-        np.array(peaks), np.array(fwhms), np.array(fwhm_errs), 2039
-    )
+    def get_fwhms(self):
+        """
+        Updates last results dictionary with fwhms in kev
+        """
 
-    log.info(f"Qbb fwhm is {qbb} keV +- {qbb_err}")
+        peak_parameters = self.results[list(self.results)[-1]].get(
+            "peak_parameters", None
+        )
 
-    return {
-        "y_val": qbb,
-        "y_err": qbb_err,
-        "qbb_fwhm": qbb,
-        "qbb_fwhm_err": qbb_err,
-        "alpha": alpha,
-        "peaks": peaks.tolist(),
-        "fwhms": fwhms,
-        "fwhm_errs": fwhm_errs,
-        "n_events": n_sig,
-        "n_sig_err": n_sig_err,
-    }
-
-
-OptimiserDimension = namedtuple(
-    "OptimiserDimension", "name parameter min_val max_val rounding unit"
-)
-
-
-class BayesianOptimizer:
-    np.random.seed(55)
-    lambda_param = 0.01
-    eta_param = 0
-    # FIXME: the following throws a TypeError
-    # kernel=ConstantKernel(1.0, constant_value_bounds="fixed") * RBF(1, length_scale_bounds="fixed") #+ WhiteKernel(noise_level=0.0111)
-
-    def __init__(self, acq_func, batch_size, kernel=None):
-        self.dims = []
-        self.current_iter = 0
-
-        self.batch_size = batch_size
-        self.iters = 0
-
-        self.gauss_pr = GaussianProcessRegressor(kernel=kernel)
-        self.best_samples_ = pd.DataFrame(columns=["x", "y", "ei"])
-        self.distances_ = []
-
-        if acq_func == "ei":
-            self.acq_function = self._get_expected_improvement
-        elif acq_func == "ucb":
-            self.acq_function = self._get_ucb
-        elif acq_func == "lcb":
-            self.acq_function = self._get_lcb
-
-    def add_dimension(self, name, parameter, min_val, max_val, rounding=2, unit=None):
-        self.dims.append(
-            OptimiserDimension(name, parameter, min_val, max_val, rounding, unit)
-        )
-
-    def get_n_dimensions(self):
-        return len(self.dims)
-
-    def add_initial_values(self, x_init, y_init, yerr_init):
-        self.x_init = x_init
-        self.y_init = y_init
-        self.yerr_init = yerr_init
-
-    def _get_expected_improvement(self, x_new):
-        mean_y_new, sigma_y_new = self.gauss_pr.predict(
-            np.array([x_new]), return_std=True
-        )
-
-        mean_y = self.gauss_pr.predict(self.x_init)
-        min_mean_y = np.min(mean_y)
-        z = (mean_y_new[0] - min_mean_y - 1) / (sigma_y_new[0] + 1e-9)
-        exp_imp = (mean_y_new[0] - min_mean_y - 1) * norm.cdf(z) + sigma_y_new[
-            0
-        ] * norm.pdf(z)
-        return exp_imp
-
-    def _get_ucb(self, x_new):
-        mean_y_new, sigma_y_new = self.gauss_pr.predict(
-            np.array([x_new]), return_std=True
-        )
-        return mean_y_new[0] + self.lambda_param * sigma_y_new[0]
-
-    def _get_lcb(self, x_new):
-        mean_y_new, sigma_y_new = self.gauss_pr.predict(
-            np.array([x_new]), return_std=True
-        )
-        return mean_y_new[0] - self.lambda_param * sigma_y_new[0]
-
-    def _get_next_probable_point(self):
-        min_ei = float(sys.maxsize)
-        x_optimal = None
-        # Trial with an array of random data points
-        rands = np.random.uniform(
-            np.array([dim.min_val for dim in self.dims]),
-            np.array([dim.max_val for dim in self.dims]),
-            (self.batch_size, self.get_n_dimensions()),
-        )
-        for x_start in rands:
-            response = minimize(
-                fun=self.acq_function,
-                x0=x_start,
-                bounds=[(dim.min_val, dim.max_val) for dim in self.dims],
-                method="L-BFGS-B",
-            )
-            if response.fun < min_ei:
-                min_ei = response.fun
-                x_optimal = [
-                    y.round(dim.rounding) for y, dim in zip(response.x, self.dims)
-                ]
-        if x_optimal in self.x_init and self.iters < 5:
-            if self.iters < 5:
-                self.iters += 1
-                x_optimal, min_ei = self._get_next_probable_point()
-            else:
-                perturb = np.random.uniform(
-                    np.array([(dim.max_val - dim.min_val) / 100 for dim in self.dims]),
-                    np.array([(dim.max_val - dim.min_val) / 10 for dim in self.dims]),
-                    (1, len(self.dims)),
+        if peak_parameters is None:
+            log.error("No peak parameters found")
+            return
+
+        cal_fwhms = []
+        cal_fwhm_errs = []
+        for peak, peak_dict in peak_parameters.items():
+            # Calculate the uncalibrated fwhm
+            if peak_dict["validity"] is True:
+                uncal_fwhm, uncal_fwhm_err = peak_dict["function"].get_fwhm(
+                    peak_dict["parameters"],
+                    cov=peak_dict["covariance"],
                 )
-                x_optimal += perturb
-                x_optimal = [
-                    y.round(dim.rounding) for y, dim in zip(x_optimal[0], self.dims)
-                ]
-                for i, y in enumerate(x_optimal):
-                    if y > self.dims[i].max_val:
-                        x_optimal[i] = self.dims[i].max_val
-                    elif y < self.dims[i].min_val:
-                        x_optimal[i] = self.dims[i].min_val
-
-        return x_optimal, min_ei
-
-    def _extend_prior_with_posterior_data(self, x, y, yerr):
-        self.x_init = np.append(self.x_init, np.array([x]), axis=0)
-        self.y_init = np.append(self.y_init, np.array(y), axis=0)
-        self.yerr_init = np.append(self.yerr_init, np.array(yerr), axis=0)
-
-    def get_first_point(self):
-        y_min_ind = np.nanargmin(self.y_init)
-        self.y_min = self.y_init[y_min_ind]
-        self.optimal_x = self.x_init[y_min_ind]
-        self.optimal_ei = None
-        return self.optimal_x, self.optimal_ei
-
-    @ignore_warnings(category=ConvergenceWarning)
-    def iterate_values(self):
-        nan_idxs = np.isnan(self.y_init)
-        self.gauss_pr.fit(self.x_init[~nan_idxs], np.array(self.y_init)[~nan_idxs])
-        x_next, ei = self._get_next_probable_point()
-        return x_next, ei
-
-    def update_db_dict(self, db_dict):
-        if self.current_iter == 0:
-            x_new, ei = self.get_first_point()
-        x_new, ei = self.iterate_values()
-        self.current_x = x_new
-        self.current_ei = ei
-        for i, val in enumerate(x_new):
-            name, parameter, min_val, max_val, rounding, unit = self.dims[i]
-            if unit is not None:
-                value_str = f"{val}*{unit}"
             else:
-                value_str = f"{val}"
-            if name not in db_dict.keys():
-                db_dict[name] = {parameter: value_str}
-            else:
-                db_dict[name][parameter] = value_str
-        self.current_iter += 1
-        return db_dict
-
-    def update(self, results):
-        y_val = results["y_val"]
-        y_err = results["y_err"]
-        self._extend_prior_with_posterior_data(
-            self.current_x, np.array([y_val]), np.array([y_err])
-        )
+                uncal_fwhm, uncal_fwhm_err = (np.nan, np.nan)
 
-        if np.isnan(y_val) | np.isnan(y_err):
-            pass
-        else:
-            if y_val < self.y_min:
-                self.y_min = y_val
-                self.optimal_x = self.current_x
-                self.optimal_ei = self.current_ei
-                self.optimal_results = results
+            # Apply calibration
 
-        if self.current_iter == 1:
-            self.prev_x = self.current_x
-        else:
-            self.distances_.append(
-                np.linalg.norm(np.array(self.prev_x) - np.array(self.current_x))
-            )
-            self.prev_x = self.current_x
+            derco = Polynomial(self.pars).deriv().coef
+            der = pgf.nb_poly(peak, derco)
+            cal_fwhm = uncal_fwhm * der
+            cal_fwhm_err = uncal_fwhm_err * der
+
+            peak_dict.update({"fwhm_in_kev": cal_fwhm, "fwhm_err_in_kev": cal_fwhm_err})
 
-        self.best_samples_ = pd.concat(
+            if peak_dict["validity"] is True:
+                cal_fwhms.append(cal_fwhm)
+                cal_fwhm_errs.append(cal_fwhm_err)
+
+        cal_fwhms = np.array(cal_fwhms)
+        cal_fwhm_errs = np.array(cal_fwhm_errs)
+        fitted_peaks_kev = np.array(
             [
-                self.best_samples_,
-                pd.DataFrame(
-                    {"x": self.optimal_x, "y": self.y_min, "ei": self.optimal_ei}
-                ),
-            ],
-            ignore_index=True,
+                peak
+                for peak, peak_dict in peak_parameters.items()
+                if peak_dict["validity"]
+            ]
         )
 
-    def get_best_vals(self):
-        out_dict = {}
-        for i, val in enumerate(self.optimal_x):
-            name, parameter, min_val, max_val, rounding, unit = self.dims[i]
-            value_str = f"{val}*{unit}"
-            if name not in out_dict.keys():
-                out_dict[name] = {parameter: value_str}
-            else:
-                out_dict[name][parameter] = value_str
-        return out_dict
+        log.info(f"{len(cal_fwhms)} FWHMs found:")
+        log.info("\t   Energy   | FWHM  ")
+        for i, (ei, fwhm, fwhme) in enumerate(
+            zip(fitted_peaks_kev, cal_fwhms, cal_fwhm_errs)
+        ):
+            log.info(
+                f"\t{i}".ljust(4)
+                + str(ei).ljust(9)
+                + f"| {fwhm:.2f}+-{fwhme:.2f} kev".ljust(5)
+            )
 
-    @ignore_warnings(category=ConvergenceWarning)
-    def plot(self, init_samples=None):
-        nan_idxs = np.isnan(self.y_init)
-        fail_idxs = np.isnan(self.yerr_init)
-        self.gauss_pr.fit(self.x_init[~nan_idxs], np.array(self.y_init)[~nan_idxs])
-        if (len(self.dims) != 2) and (len(self.dims) != 1):
-            raise Exception("Acquisition Function Plotting not implemented for dim!=2")
-        elif len(self.dims) == 1:
-            points = np.arange(self.dims[0].min_val, self.dims[0].max_val, 0.1)
-            ys = np.zeros_like(points)
-            ys_err = np.zeros_like(points)
-            for i, point in enumerate(points):
-                ys[i], ys_err[i] = self.gauss_pr.predict(
-                    np.array([point]).reshape(1, -1), return_std=True
-                )
-            fig = plt.figure()
+    @staticmethod
+    def fit_energy_res_curve(fwhm_func, fwhm_peaks, fwhms, dfwhms):
+        try:
+            if len(fwhm_peaks) == 0:
+                raise RuntimeError
+            c_lin = cost.LeastSquares(fwhm_peaks, fwhms, dfwhms, fwhm_func.func)
+            # c_lin.loss = "soft_l1"
+            m = Minuit(c_lin, *fwhm_func.guess(fwhm_peaks, fwhms, dfwhms))
+            bounds = fwhm_func.bounds(fwhms)
+            for arg, val in enumerate(bounds):
+                m.limits[arg] = val
+            m.simplex()
+            m.migrad()
+            m.hesse()
+
+            p_val = scipy.stats.chi2.sf(m.fval, len(fwhm_peaks) - len(m.values))
 
-            plt.scatter(np.array(self.x_init), np.array(self.y_init), label="Samples")
-            plt.scatter(
-                np.array(self.x_init)[fail_idxs],
-                np.array(self.y_init)[fail_idxs],
-                color="green",
-                label="Failed samples",
-            )
-            plt.fill_between(points, ys - ys_err, ys + ys_err, alpha=0.1)
-            if init_samples is not None:
-                init_ys = np.array(
-                    [
-                        np.where(init_sample == self.x_init)[0][0]
-                        for init_sample in init_samples
-                    ]
+            results = {
+                "function": fwhm_func,
+                "module": fwhm_func.__module__,
+                "expression": fwhm_func.string_func("x"),
+                "parameters": m.values,
+                "uncertainties": m.errors,
+                "cov": m.covariance,
+                "csqr": (m.fval, len(fwhm_peaks) - len(m.values)),
+                "p_val": p_val,
+            }
+
+            log.info(f'FWHM fit: {results["parameters"].to_dict()}')
+            log.info("FWHM fit values:")
+            log.info("\t   Energy   | FWHM (kev)  | Predicted (kev)")
+            for i, (peak, fwhm, fwhme) in enumerate(zip(fwhm_peaks, fwhms, dfwhms)):
+                log.info(
+                    f"\t{i}".ljust(4)
+                    + str(peak).ljust(9)
+                    + f"| {fwhm:.2f}+-{fwhme:.2f}  ".ljust(5)
+                    + f"| {fwhm_func.func(peak, *results['parameters']):.2f}".ljust(5)
                 )
-                plt.scatter(
-                    np.array(init_samples)[:, 0],
-                    np.array(self.y_init)[init_ys],
-                    color="red",
-                    label="Init Samples",
+        except RuntimeError:
+            pars, errs, cov = return_nans(fwhm_func.func)
+            results = {
+                "function": fwhm_func,
+                "module": fwhm_func.__module__,
+                "expression": fwhm_func.string_func("x"),
+                "parameters": pars,
+                "uncertainties": errs,
+                "cov": cov,
+                "csqr": (np.nan, np.nan),
+                "p_val": 0,
+            }
+            log.error("FWHM fit failed to converge")
+        return results
+
+    @staticmethod
+    def interpolate_energy_res(
+        fwhm_func, fwhm_peaks, fwhm_results, interp_energy_kev=None, debug_mode=False
+    ):
+        if interp_energy_kev is not None:
+            for key, energy in interp_energy_kev.items():
+                try:
+                    if energy > np.nanmax(fwhm_peaks) or energy < np.nanmin(fwhm_peaks):
+                        raise RuntimeError(
+                            "Interpolating energy out of range of fitted peaks"
+                        )
+                    rng = np.random.default_rng(1)
+                    pars_b = rng.multivariate_normal(
+                        fwhm_results["parameters"], fwhm_results["cov"], size=1000
+                    )
+                    interp_vals = np.array(
+                        [fwhm_func.func(energy, *par_b) for par_b in pars_b]
+                    )
+                    interp_err = np.nanstd(interp_vals)
+                    interp_fwhm = fwhm_func.func(energy, *fwhm_results["parameters"])
+                except BaseException as e:
+                    if debug_mode:
+                        raise (e)
+                    interp_fwhm = np.nan
+                    interp_err = np.nan
+                fwhm_results.update(
+                    {
+                        "interp_energy_in_kev": energy,
+                        f"{key}_fwhm_in_kev": interp_fwhm,
+                        f"{key}_fwhm_err_in_kev": interp_err,
+                    }
+                )
+                log.info(
+                    f"FWHM {key} energy resolution at {energy} : {interp_fwhm:1.2f} +- {interp_err:1.2f} kev"
                 )
-            plt.scatter(self.optimal_x[0], self.y_min, color="orange", label="Optimal")
+        return fwhm_results
 
-            plt.xlabel(
-                f"{self.dims[0].name}-{self.dims[0].parameter}({self.dims[0].unit})"
-            )
-            plt.ylabel(f"Kernel Value")
-            plt.legend()
-        elif len(self.dims) == 2:
-            x, y = np.mgrid[
-                self.dims[0].min_val : self.dims[0].max_val : 0.1,
-                self.dims[1].min_val : self.dims[1].max_val : 0.1,
+    def get_energy_res_curve(self, fwhm_func, interp_energy_kev=None):
+        peak_parameters = self.results[list(self.results)[-1]].get(
+            "peak_parameters", None
+        )
+        if peak_parameters is None:
+            log.error("No peak parameters found")
+            return
+        fitted_peaks_kev = np.array(
+            [
+                peak
+                for peak, peak_dict in peak_parameters.items()
+                if peak_dict["validity"]
             ]
-            points = np.vstack((x.flatten(), y.flatten())).T
-            out_grid = np.zeros(
-                (
-                    int((self.dims[0].max_val - self.dims[0].min_val) * 10),
-                    int((self.dims[1].max_val - self.dims[1].min_val) * 10),
-                )
-            )
+        )
+        if len(fitted_peaks_kev) == 0:
+            return
+        if "fwhm_in_kev" not in peak_parameters[fitted_peaks_kev[0]]:
+            self.get_fwhms()
+            peak_parameters = self.results[list(self.results)[-1]].get(
+                "peak_parameters", None
+            )
+
+        fwhm_peaks = np.array([], dtype=np.float32)
+        fwhms = np.array([], dtype=np.float32)
+        dfwhms = np.array([], dtype=np.float32)
+        all_peaks = np.array([], dtype=np.float32)
+        #####
+        # Remove the Doppler Broadened peaks from calibration if found
+        for peak, peak_dict in peak_parameters.items():
+            all_peaks = np.append(all_peaks, peak)
+            if np.abs(peak - 2103.5) < 1:
+                log.info("Tl SEP removed from fwhm fitting")
+            elif np.abs(peak - 1592.53) < 1:
+                log.info("Tl DEP removed from fwhm fitting")
+            elif np.abs(peak - 511.0) < 1:
+                log.info("e annihilation removed from fwhm fitting")
+            elif np.isnan(peak_dict["fwhm_in_kev"]) or np.isnan(
+                peak_dict["fwhm_err_in_kev"]
+            ):
+                log.info(f"{peak} failed, removed from fwhm fitting")
+            else:
+                fwhm_peaks = np.append(fwhm_peaks, peak)
+                fwhms = np.append(fwhms, peak_dict["fwhm_in_kev"])
+                dfwhms = np.append(dfwhms, peak_dict["fwhm_err_in_kev"])
+
+        log.info(f"Running FWHM fit for : {fwhm_func.__name__}")
+
+        results = self.fit_energy_res_curve(fwhm_func, fwhm_peaks, fwhms, dfwhms)
+        if interp_energy_kev is not None:
+            results = self.interpolate_energy_res(
+                fwhm_func,
+                fwhm_peaks,
+                results,
+                interp_energy_kev,
+                debug_mode=self.debug_mode,
+            )
+        self.results[list(self.results)[-1]].update({fwhm_func.__name__: results})
+
+    def full_calibration(
+        self,
+        e_uncal,
+        peak_pars,
+        allowed_p_val=10**-20,
+        tail_weight=0,
+        peak_param="mode",
+        n_events=None,
+    ):
+        log.debug(f"Find peaks and compute calibration curve for {self.energy_param}")
+        log.debug(f"Guess is {self.pars[1]:.3f}")
+        self.hpge_find_energy_peaks(e_uncal)
+        self.hpge_get_energy_peaks(e_uncal)
+
+        got_peaks_kev = self.peaks_kev.copy()
+        self.hpge_fit_energy_peaks(
+            e_uncal,
+            peak_pars=peak_pars,
+            allowed_p_val=allowed_p_val,
+            tail_weight=tail_weight,
+            peak_param=peak_param,
+            n_events=n_events,
+        )
+        if len(self.peaks_kev) != len(got_peaks_kev):
+            for i, peak in enumerate(got_peaks_kev):
+                if peak not in self.peaks_kev:
+                    for i, peak_par in enumerate(peak_pars):
+                        if peak_par[0] == peak:
+                            new_kev_ranges = (peak_par[1][0] - 5, peak_par[1][1] - 5)
+                            peak_pars[i] = (peak, new_kev_ranges, peak_par[2])
+            for i, peak in enumerate(self.peaks_kev):
+                try:
+                    if (
+                        self.results["pk_fwhms"][:, 1][i]
+                        / self.results["pk_fwhms"][:, 0][i]
+                        > 0.05
+                    ):
+                        for i, peak_par in enumerate(peak_pars):
+                            if peak_par[0] == peak:
+                                new_kev_ranges = (
+                                    peak_par[1][0] - 5,
+                                    peak_par[1][1] - 5,
+                                )
+                                peak_pars[i] = (peak, new_kev_ranges, peak_par[2])
+                except BaseException as e:
+                    if self.debug_mode:
+                        raise (e)
+
+            self.hpge_fit_energy_peaks(
+                e_uncal,
+                peaks=got_peaks_kev,
+                peak_pars=peak_pars,
+                allowed_p_val=allowed_p_val,
+                tail_weight=tail_weight,
+                peak_param=peak_param,
+                n_events=n_events,
+            )
+
+            if self.pars is None:
+                if self.deg < 1:
+                    self.pars = np.full(2, np.nan)
+                else:
+                    self.pars = np.full(self.deg + 1, np.nan)
 
-            j = 0
-            for i, _ in np.ndenumerate(out_grid):
-                out_grid[i] = self.gauss_pr.predict(
-                    points[j].reshape(1, -1), return_std=False
-                )
-                j += 1
+                log.error(f"Calibration failed completely for {self.energy_param}")
+                return
+
+        log.debug("Calibrated found")
+        log.info(f"Calibration pars are {self.pars}")
+
+        self.get_energy_res_curve(
+            FWHMLinear,
+            interp_energy_kev={"Qbb": 2039.0},
+        )
+        self.get_energy_res_curve(
+            FWHMQuadratic,
+            interp_energy_kev={"Qbb": 2039.0},
+        )
+
+    def fit_calibrated_peaks(self, e_uncal, peak_pars):
+        log.debug(f"Fitting {self.energy_param}")
+        self.hpge_get_energy_peaks(e_uncal, update_cal_pars=False)
+        self.hpge_fit_energy_peaks(e_uncal, peak_pars=peak_pars, update_cal_pars=False)
+        self.get_energy_res_curve(
+            FWHMLinear,
+            interp_energy_kev={"Qbb": 2039.0},
+        )
+        self.get_energy_res_curve(
+            FWHMQuadratic,
+            interp_energy_kev={"Qbb": 2039.0},
+        )
+
+    def calibrate_prominent_peak(
+        self,
+        e_uncal,
+        peak,
+        peak_pars,
+        allowed_p_val=10**-20,
+        tail_weight=0,
+        peak_param="mode",
+        n_events=None,
+    ):
+        log.debug(f"Find peaks and compute calibration curve for {self.energy_param}")
+        log.debug(f"Guess is {self.pars[1]:.3f}")
+        if self.deg != 0:
+            log.error("deg must be 0 for calibrate_prominent_peak")
+            return
+        self.hpge_find_energy_peaks(e_uncal)
+        self.hpge_get_energy_peaks(e_uncal)
+
+        got_peaks_kev = self.peaks_kev.copy()
+        self.hpge_fit_energy_peaks(
+            e_uncal,
+            peaks_kev=[peak],
+            peak_pars=peak_pars,
+            allowed_p_val=allowed_p_val,
+            tail_weight=tail_weight,
+            peak_param=peak_param,
+            n_events=n_events,
+        )
+        self.hpge_fit_energy_peaks(
+            e_uncal,
+            peaks_kev=got_peaks_kev,
+            peak_pars=peak_pars,
+            allowed_p_val=allowed_p_val,
+            tail_weight=tail_weight,
+            peak_param=peak_param,
+            n_events=n_events,
+            update_cal_pars=False,
+        )
+        self.get_energy_res_curve(
+            FWHMLinear,
+            interp_energy_kev={"Qbb": 2039.0},
+        )
+        self.get_energy_res_curve(
+            FWHMQuadratic,
+            interp_energy_kev={"Qbb": 2039.0},
+        )
+
+    def plot_cal_fit(self, data, figsize=(12, 8), fontsize=12, erange=(200, 2700)):
+        fig, (ax1, ax2) = plt.subplots(
+            2, 1, sharex=True, gridspec_kw={"height_ratios": [3, 1]}, figsize=figsize
+        )
+
+        cal_bins = np.linspace(0, np.nanmax(self.peak_locs) * 1.1, 20)
+
+        ax1.scatter(self.peaks_kev, self.peak_locs, marker="x", c="b")
+
+        ax1.plot(pgf.nb_poly(cal_bins, self.pars), cal_bins, lw=1, c="g")
+
+        ax1.grid()
+        ax1.set_xlim([erange[0], erange[1]])
+        ax1.set_ylabel("Energy (ADC)", fontsize=fontsize)
+        ax2.scatter(
+            self.peaks_kev,
+            pgf.nb_poly(np.array(self.peak_locs), self.pars) - self.peaks_kev,
+            marker="x",
+            c="b",
+        )
+        ax2.grid()
+        ax2.set_xlabel("Energy (keV)", fontsize=fontsize)
+        ax2.set_ylabel("Residuals (keV)", fontsize=fontsize)
+        plt.close()
+        return fig
+
+    def plot_fits(
+        self, energies, figsize=(12, 8), fontsize=12, ncols=3, nrows=3, binning_kev=5
+    ):
+        plt.rcParams["font.size"] = fontsize
+
+        pk_parameters = self.results[list(self.results)[-1]].get(
+            "peak_parameters", None
+        )
+
+        fig = plt.figure(figsize=figsize)
+        derco = Polynomial(self.pars).deriv().coef
+        der = [pgf.nb_poly(5, derco) for _ in list(pk_parameters)]
+        for i, peak in enumerate(pk_parameters):
+            range_adu = 5 / der[i]
+            plt.subplot(nrows, ncols, i + 1)
+            pk_dict = pk_parameters[peak]
+            pk_pars = pk_dict["parameters"]
+            pk_ranges = pk_dict["range"]
+            pk_func = pk_dict["function"]
+            mu = pk_func.get_mu(pk_pars) if pk_pars is not None else np.nan
+
+            try:
+                binning = np.arange(pk_ranges[0], pk_ranges[1], 0.1 / der[i])
+                bin_cs = (binning[1:] + binning[:-1]) / 2
+
+                counts, bs, bars = plt.hist(energies, bins=binning, histtype="step")
+                if pk_pars is not None:
+                    fit_vals = pk_func.get_pdf(bin_cs, *pk_pars, 0) * np.diff(bs)[0]
+                    plt.plot(bin_cs, fit_vals)
+                    plt.step(
+                        bin_cs,
+                        [
+                            (fval - count) / count if count != 0 else (fval - count)
+                            for count, fval in zip(counts, fit_vals)
+                        ],
+                        where="mid",
+                    )
+
+                    plt.annotate(
+                        f"{peak:.1f} keV", (0.02, 0.8), xycoords="axes fraction"
+                    )
+                    plt.annotate(
+                        f"p-value : {pk_dict['p_value']:.4f}",
+                        (0.02, 0.7),
+                        xycoords="axes fraction",
+                    )
+                    plt.xlabel("Energy (keV)")
+                    plt.ylabel("Counts")
+                    plt.legend(loc="upper left", frameon=False)
+
+                    plt.xlim([mu - range_adu, mu + range_adu])
+                    locs, labels = plt.xticks()
+
+                    def get_peak_labels(
+                        labels: list[str], pars: list[float]
+                    ) -> tuple(list[float], list[float]):
+                        out = []
+                        out_labels = []
+                        for i, label in enumerate(labels):
+                            if i % 2 == 1:
+                                continue
+                            else:
+                                out.append(f"{pgf.nb_poly(label, pars):.1f}")
+                                out_labels.append(label)
+                        return out_labels, out
+
+                    new_locs, new_labels = get_peak_labels(locs, self.pars)
+                    plt.xticks(ticks=new_locs, labels=new_labels)
+
+            except BaseException as e:
+                if self.debug_mode:
+                    raise (e)
 
-            fig = plt.figure()
-            plt.imshow(
-                out_grid,
-                norm=LogNorm(),
-                origin="lower",
-                aspect="auto",
-                extent=(0, out_grid.shape[1], 0, out_grid.shape[0]),
-            )
-            plt.scatter(
-                np.array(self.x_init - self.dims[1].min_val)[:, 1] * 10,
-                np.array(self.x_init - self.dims[0].min_val)[:, 0] * 10,
-            )
-            if init_samples is not None:
-                plt.scatter(
-                    (init_samples[:, 1] - self.dims[1].min_val) * 10,
-                    (init_samples[:, 0] - self.dims[0].min_val) * 10,
-                    color="red",
-                )
-            plt.scatter(
-                (self.optimal_x[1] - self.dims[1].min_val) * 10,
-                (self.optimal_x[0] - self.dims[0].min_val) * 10,
-                color="orange",
-            )
-            ticks, labels = plt.xticks()
-            labels = np.linspace(self.dims[1].min_val, self.dims[1].max_val, 5)
-            ticks = np.linspace(0, out_grid.shape[1], 5)
-            plt.xticks(ticks=ticks, labels=labels, rotation=45)
-            ticks, labels = plt.yticks()
-            labels = np.linspace(self.dims[0].min_val, self.dims[0].max_val, 5)
-            ticks = np.linspace(0, out_grid.shape[0], 5)
-            plt.yticks(ticks=ticks, labels=labels, rotation=45)
-            plt.xlabel(
-                f"{self.dims[1].name}-{self.dims[1].parameter}({self.dims[1].unit})"
-            )
-            plt.ylabel(
-                f"{self.dims[0].name}-{self.dims[0].parameter}({self.dims[0].unit})"
-            )
-        plt.title(f"{self.dims[0].name} Kernel Prediction")
         plt.tight_layout()
         plt.close()
         return fig
 
-    @ignore_warnings(category=ConvergenceWarning)
-    def plot_acq(self, init_samples=None):
-        nan_idxs = np.isnan(self.y_init)
-        self.gauss_pr.fit(self.x_init[~nan_idxs], np.array(self.y_init)[~nan_idxs])
-        if (len(self.dims) != 2) and (len(self.dims) != 1):
-            raise Exception("Acquisition Function Plotting not implemented for dim!=2")
-        elif len(self.dims) == 1:
-            points = np.arange(self.dims[0].min_val, self.dims[0].max_val, 0.1)
-            ys = np.zeros_like(points)
-            for i, point in enumerate(points):
-                ys[i] = self.acq_function(np.array([point]).reshape(1, -1)[0])
+    def plot_eres_fit(self, data, erange=(200, 2700), figsize=(12, 8), fontsize=12):
+        plt.rcParams["font.size"] = fontsize
+
+        pk_parameters = self.results[list(self.results)[-1]].get(
+            "peak_parameters", None
+        )
+
+        if pk_parameters is None:
             fig = plt.figure()
-            plt.plot(points, ys)
-            plt.scatter(np.array(self.x_init), np.array(self.y_init), label="Samples")
-            if init_samples is not None:
-                init_ys = np.array(
-                    [
-                        np.where(init_sample == self.x_init)[0][0]
-                        for init_sample in init_samples
-                    ]
-                )
-                plt.scatter(
-                    np.array(init_samples)[:, 0],
-                    np.array(self.y_init)[init_ys],
-                    color="red",
-                    label="Init Samples",
-                )
-            plt.scatter(self.optimal_x[0], self.y_min, color="orange", label="Optimal")
+            return fig
 
-            plt.xlabel(
-                f"{self.dims[0].name}-{self.dims[0].parameter}({self.dims[0].unit})"
-            )
-            plt.ylabel(f"Acquisition Function Value")
-            plt.legend()
+        #####
+        # Remove the Tl SEP and DEP from calibration if found
+        fwhm_peaks = np.array([], dtype=np.float32)
+        fwhms = np.array([], dtype=np.float32)
+        dfwhms = np.array([], dtype=np.float32)
+
+        for peak, pk_dict in pk_parameters.items():
+            if peak == 2103.53:
+                pass
+            elif peak == 1592.53:
+                pass
+            elif peak == 511.0:
+                pass
+            elif pk_dict["validity"] is False:
+                pass
+            elif np.isnan(pk_dict["fwhm_err_in_kev"]):
+                pass
+            else:
+                fwhm_peaks = np.append(fwhm_peaks, peak)
+                fwhms = np.append(fwhms, pk_dict["fwhm_in_kev"])
+                dfwhms = np.append(dfwhms, pk_dict["fwhm_err_in_kev"])
+
+        fwhm_dicts = {}
+        interp_energy = None
+        interp_fwhm_name = None
+        for name, item in self.results[list(self.results)[-1]].items():
+            if "FWHM" in name:
+                fwhm_dicts[name] = item
+                if "interp_energy_in_kev" in item:
+                    interp_energy = item["interp_energy_in_kev"]
+                    for field in item:
+                        if "_fwhm_in_kev" in field:
+                            interp_fwhm_name = field.replace("_fwhm_in_kev", "")
 
-        elif len(self.dims) == 2:
-            x, y = np.mgrid[
-                self.dims[0].min_val : self.dims[0].max_val : 0.1,
-                self.dims[1].min_val : self.dims[1].max_val : 0.1,
-            ]
-            points = np.vstack((x.flatten(), y.flatten())).T
-            out_grid = np.zeros(
-                (
-                    int((self.dims[0].max_val - self.dims[0].min_val) * 10),
-                    int((self.dims[1].max_val - self.dims[1].min_val) * 10),
-                )
-            )
+        fig, (ax1, ax2) = plt.subplots(
+            2, 1, sharex=True, gridspec_kw={"height_ratios": [3, 1]}, figsize=figsize
+        )
+        if len(np.where((~np.isnan(fwhms)) & (~np.isnan(dfwhms)))[0]) > 0:
+            ax1.errorbar(fwhm_peaks, fwhms, yerr=dfwhms, marker="x", ls=" ", c="black")
 
-            j = 0
-            for i, _ in np.ndenumerate(out_grid):
-                out_grid[i] = self.acq_function(points[j])
-                j += 1
+            fwhm_slope_bins = np.arange(erange[0], erange[1], 10)
 
-            fig = plt.figure()
-            plt.imshow(
-                out_grid,
-                norm=LogNorm(),
-                origin="lower",
-                aspect="auto",
-                extent=(0, out_grid.shape[1], 0, out_grid.shape[0]),
-            )
-            plt.scatter(
-                np.array(self.x_init - self.dims[1].min_val)[:, 1] * 10,
-                np.array(self.x_init - self.dims[0].min_val)[:, 0] * 10,
-            )
-            if init_samples is not None:
-                plt.scatter(
-                    (init_samples[:, 1] - self.dims[1].min_val) * 10,
-                    (init_samples[:, 0] - self.dims[0].min_val) * 10,
-                    color="red",
+            if interp_energy is not None:
+                qbb_line_vx = [interp_energy, interp_energy]
+                qbb_line_hx = [erange[0], interp_energy]
+                for name, fwhm_dict in fwhm_dicts.items():
+                    qbb_line_vy = [np.inf, -np.inf]
+                    low_lim = 0.9 * np.nanmin(
+                        fwhm_dict["function"].func(
+                            fwhm_slope_bins, *fwhm_dict["parameters"]
+                        )
+                    )
+                    up_lim = fwhm_dict[f"{interp_fwhm_name}_fwhm_in_kev"]
+                    if low_lim < qbb_line_vy[0]:
+                        qbb_line_vy[0] = low_lim
+                    if up_lim > qbb_line_vy[1]:
+                        qbb_line_vy[1] = up_lim
+                    ax1.plot(
+                        qbb_line_hx,
+                        [
+                            fwhm_dict[f"{interp_fwhm_name}_fwhm_in_kev"],
+                            fwhm_dict[f"{interp_fwhm_name}_fwhm_in_kev"],
+                        ],
+                        lw=1,
+                        c="r",
+                        ls="--",
+                    )
+                    ax1.plot(
+                        fwhm_slope_bins,
+                        fwhm_dict["function"].func(
+                            fwhm_slope_bins, *fwhm_dict["parameters"]
+                        ),
+                        lw=1,
+                        label=f'{name}, {interp_fwhm_name} fwhm: {fwhm_dict[f"{interp_fwhm_name}_fwhm_in_kev"]:1.2f} +- {fwhm_dict[f"{interp_fwhm_name}_fwhm_err_in_kev"]:1.2f} keV',
+                    )
+                    ax1.plot(qbb_line_vx, qbb_line_vy, lw=1, c="r", ls="--")
+
+            ax1.set_xlim(erange)
+            ax1.set_ylim([low_lim, None])
+            ax1.set_ylabel("FWHM energy resolution (keV)")
+            for _, fwhm_dict in fwhm_dicts.items():
+                ax2.plot(
+                    fwhm_peaks,
+                    (
+                        fwhms
+                        - fwhm_dict["function"].func(
+                            fwhm_peaks, *fwhm_dict["parameters"]
+                        )
+                    )
+                    / dfwhms,
+                    lw=0,
+                    marker="x",
                 )
-            plt.scatter(
-                (self.optimal_x[1] - self.dims[1].min_val) * 10,
-                (self.optimal_x[0] - self.dims[0].min_val) * 10,
-                color="orange",
-            )
-            ticks, labels = plt.xticks()
-            labels = np.linspace(self.dims[1].min_val, self.dims[1].max_val, 5)
-            ticks = np.linspace(0, out_grid.shape[1], 5)
-            plt.xticks(ticks=ticks, labels=labels, rotation=45)
-            ticks, labels = plt.yticks()
-            labels = np.linspace(self.dims[0].min_val, self.dims[0].max_val, 5)
-            ticks = np.linspace(0, out_grid.shape[0], 5)
-            plt.yticks(ticks=ticks, labels=labels, rotation=45)
-            plt.xlabel(
-                f"{self.dims[1].name}-{self.dims[1].parameter}({self.dims[1].unit})"
-            )
-            plt.ylabel(
-                f"{self.dims[0].name}-{self.dims[0].parameter}({self.dims[0].unit})"
-            )
-        plt.title(f"{self.dims[0].name} Acquisition Space")
+            ax2.plot(erange, [0, 0], color="black", lw=0.5)
+            ax2.set_xlabel("Energy (keV)")
+            ax2.set_ylabel("Normalised Residuals")
         plt.tight_layout()
         plt.close()
         return fig
 
 
-def run_optimisation(
-    tb_data,
-    dsp_config,
-    fom_function,
-    optimisers,
-    fom_kwargs=None,
-    db_dict=None,
-    nan_val=10,
-    n_iter=10,
+class FWHMLinear:
+    @staticmethod
+    def func(x, a, b):
+        return np.sqrt(a + b * x)
+
+    @staticmethod
+    def string_func(input_param):
+        return f"(a+b*{input_param})**(0.5)"
+
+    @staticmethod
+    def guess(xs, ys, y_errs):
+        return [np.nanmin(ys), 10**-3]
+
+    @staticmethod
+    def bounds(ys):
+        return [(0, None), (0, None)]
+
+
+class FWHMQuadratic:
+    @staticmethod
+    def func(x, a, b, c):
+        return np.sqrt(a + b * x + c * x**2)
+
+    @staticmethod
+    def string_func(input_param):
+        return f"(a+b*{input_param}+c*{input_param}**2)**(0.5)"
+
+    @staticmethod
+    def guess(xs, ys, y_errs):
+        return [np.nanmin(ys), 2 * 10**-3, 10**-8]
+
+    @staticmethod
+    def bounds(ys):
+        return [(0, np.nanmin(ys) ** 2), (10**-3, None), (0, None)]
+
+
+def hpge_fit_energy_peak_tops(
+    hist,
+    bins,
+    var,
+    peak_locs,
+    n_to_fit=7,
+    cost_func="Least Squares",
+    inflate_errors=False,
+    gof_method="var",
+    debug_mode=False,
 ):
-    if not isinstance(optimisers, list):
-        optimisers = [optimisers]
-    if not isinstance(fom_kwargs, list):
-        fom_kwargs = [fom_kwargs]
-    if not isinstance(fom_function, list):
-        fom_function = [fom_function]
-
-    for j in range(n_iter):
-        for optimiser in optimisers:
-            db_dict = optimiser.update_db_dict(db_dict)
-
-        log.info(f"Iteration number: {j+1}")
-        log.info(f"Processing with {db_dict}")
-
-        tb_out = opt.run_one_dsp(tb_data, dsp_config, db_dict=db_dict)
-
-        res = np.ndarray(shape=len(optimisers), dtype="O")
-
-        for i in range(len(optimisers)):
-            if fom_kwargs[i] is not None:
-                if len(fom_function) > 1:
-                    res[i] = fom_function[i](tb_out, fom_kwargs[i])
-                else:
-                    res[i] = fom_function[0](tb_out, fom_kwargs[i])
-            else:
-                if len(fom_function) > 1:
-                    res[i] = fom_function[i](tb_out)
-                else:
-                    res[i] = fom_function[0](tb_out)
+    """Fit gaussians to the tops of peaks
 
-        log.info(f"Results of iteration {j+1} are {res}")
+    Parameters
+    ----------
+    hist, bins, var : array, array, array
+        Histogram of uncalibrated energies, see pgh.get_hist()
+    peak_locs : array
+        locations of peaks in hist. Must be accurate two within +/- 2*n_to_fit
+    n_to_fit : int
+        number of hist bins near the peak top to include in the gaussian fit
+    cost_func : bool (optional)
+        Flag passed to gauss_mode_width_max()
+    inflate_errors : bool (optional)
+        Flag passed to gauss_mode_width_max()
+    gof_method : str (optional)
+        method flag passed to gauss_mode_width_max()
+
+    Returns
+    -------
+    pars_list : list of array
+        a list of best-fit parameters (mode, sigma, max) for each peak-top fit
+    cov_list : list of 2D arrays
+        a list of covariance matrices for each pars
+    """
+    pars_list = []
+    cov_list = []
+    for e_peak in peak_locs:
+        try:
+            pars, cov = pgb.gauss_mode_width_max(
+                hist,
+                bins,
+                var,
+                mode_guess=e_peak,
+                n_bins=n_to_fit,
+                cost_func=cost_func,
+                inflate_errors=inflate_errors,
+                gof_method=gof_method,
+            )
+        except BaseException as e:
+            if e == KeyboardInterrupt:
+                raise (e)
+            elif debug_mode:
+                raise (e)
+            pars, cov = None, None
+
+        pars_list.append(pars)
+        cov_list.append(cov)
+    return np.array(pars_list, dtype=object), np.array(cov_list, dtype=object)
 
-        for i, optimiser in enumerate(optimisers):
-            if np.isnan(res[i]["y_val"]):
-                if isinstance(nan_val, list):
-                    res[i]["y_val"] = nan_val[i]
+
+def get_hpge_energy_peak_par_guess(
+    energy, func, fit_range=None, bin_width=None, mode_guess=None
+):
+    """
+    Get parameter guesses for func fit to peak in hist
+
+    Parameters
+    ----------
+    energy : array
+        An array of energy values in the range around the peak for guessing.
+    func : function
+        The function to be fit to the peak in the histogram.
+    fit_range : tuple, optional
+        A tuple specifying the range around the peak to perform the fit. If not provided, the entire range of energy values will be used.
+    bin_width : float, optional
+        The width of the bins in the histogram. Default is 1.
+    mode_guess : float, optional
+        A guess for the mode (mu) parameter of the function. If not provided, it will be estimated from the data.
+
+    Returns
+    -------
+    ValueView
+        A ValueView object from iminuit containing the parameter guesses for the function fit.
+
+    Notes
+    -----
+    This function calculates parameter guesses for fitting a function to a peak in a histogram. It uses various methods to estimate the parameters based on the provided energy values and the selected function.
+
+    If the function is 'gauss_on_step', the following parameters will be estimated:
+    - n_sig: Number of signal events in the peak.
+    - mu: Mean of the peak.
+    - sigma: Standard deviation of the peak.
+    - n_bkg: Number of background events.
+    - hstep: Height of the step between the peak and the background.
+    - x_lo: Lower bound of the fit range.
+    - x_hi: Upper bound of the fit range.
+
+    If the function is 'hpge_peak', the following parameters will be estimated:
+    - n_sig: Number of signal events in the peak.
+    - mu: Mean of the peak.
+    - sigma: Standard deviation of the peak.
+    - htail: Height of the tail component.
+    - tau: Decay constant of the tail component.
+    - n_bkg: Number of background events.
+    - hstep: Height of the step between the peak and the background.
+    - x_lo: Lower bound of the fit range.
+    - x_hi: Upper bound of the fit range.
+
+    If the provided function is not implemented, an error will be raised.
+
+    Examples
+    --------
+    >>> energy = [1, 2, 3, 4, 5]
+    >>> func = pgf.gauss_on_step
+    >>> fit_range = (2, 4)
+    >>> bin_width = 0.5
+    >>> mode_guess = 3.5
+    >>> get_hpge_energy_peak_par_guess(energy, func, fit_range, bin_width, mode_guess)
+    {'n_sig': 3, 'mu': 3.5, 'sigma': 0.5, 'n_bkg': 2, 'hstep': 0.5, 'x_lo': 2, 'x_hi': 4}
+    """
+    if fit_range is None:
+        fit_range = (np.nanmin(energy), np.nanmax(energy))
+
+    energy = energy[(energy >= fit_range[0]) & (energy <= fit_range[1])]
+    if bin_width is None:
+        init_bin_width = (
+            2
+            * (np.nanpercentile(energy, 75) - np.nanpercentile(energy, 25))
+            * len(energy) ** (-1 / 3)
+        )
+        init_hist, init_bins, _ = pgh.get_hist(
+            energy, dx=init_bin_width, range=fit_range
+        )
+        try:
+            _, init_sigma, _ = pgh.get_gaussian_guess(init_hist, init_bins)
+        except IndexError:
+            init_hist, init_bins, _ = pgh.get_hist(
+                energy, dx=init_bin_width / 2, range=fit_range
+            )
+            try:
+                _, init_sigma, _ = pgh.get_gaussian_guess(init_hist, init_bins)
+            except IndexError:
+                init_sigma = np.nanstd(energy)
+        bin_width = 2 * (init_sigma) * len(energy) ** (-1 / 3)
+
+    hist, bins, var = pgh.get_hist(energy, dx=bin_width, range=fit_range)
+
+    if (
+        func == pgf.gauss_on_step
+        or func == pgf.hpge_peak
+        or func == pgf.gauss_on_uniform
+    ):
+        # get mu and height from a gauss fit, also sigma as fallback
+        pars, cov = pgb.gauss_mode_width_max(
+            hist, bins, var, mode_guess=mode_guess, n_bins=5
+        )
+
+        bin_centres = pgh.get_bin_centers(bins)
+        if pars is None:
+            log.info("get_hpge_energy_peak_par_guess: gauss_mode_width_max failed")
+            i_0 = np.argmax(hist)
+            mu = bin_centres[i_0]
+            height = hist[i_0]
+            sigma_guess = None
+        else:
+            mu = mode_guess if mode_guess is not None else pars[0]
+            sigma_guess = pars[1]
+            height = pars[2]
+        # get bg and step from edges of hist
+        bg = np.mean(hist[-10:])
+        step = bg - np.mean(hist[:10])
+        # get sigma from fwfm with f = 1/sqrt(e)
+        try:
+            sigma = pgh.get_fwfm(
+                0.6065,
+                hist,
+                bins,
+                var,
+                mx=height,
+                bl=bg - step / 2,
+                method="interpolate",
+            )[0]
+            if sigma <= 0:
+                raise ValueError
+        except ValueError:
+            try:
+                sigma = pgh.get_fwfm(
+                    0.6065,
+                    hist,
+                    bins,
+                    var,
+                    mx=height,
+                    bl=bg - step / 2,
+                    method="fit_slopes",
+                )[0]
+            except RuntimeError:
+                sigma = -1
+            if sigma <= 0 or sigma > 1000:
+                if sigma_guess is not None and sigma_guess > 0 and sigma_guess < 1000:
+                    sigma = sigma_guess
                 else:
-                    res[i]["y_val"] = nan_val
+                    (_, sigma, _) = pgh.get_gaussian_guess(hist, bins)
+                    if sigma is not None and sigma_guess > 0 and sigma_guess < 1000:
+                        pass
+                    else:
+                        log.info(
+                            "get_hpge_energy_peak_par_guess: sigma estimation failed"
+                        )
+                        return {}
+        # now compute amp and return
+        n_sig = np.sum(
+            hist[(bin_centres > mu - 3 * sigma) & (bin_centres < mu + 3 * sigma)]
+        )
+        n_bkg = np.sum(hist) - n_sig
 
-            optimiser.update(res[i])
+        parguess = {
+            "n_sig": n_sig,
+            "mu": mu,
+            "sigma": sigma,
+            "n_bkg": n_bkg,
+            "x_lo": bins[0],
+            "x_hi": bins[-1],
+        }
 
-    out_param_dict = {}
-    out_results_list = []
-    for optimiser in optimisers:
-        param_dict = optimiser.get_best_vals()
-        out_param_dict.update(param_dict)
-        results_dict = optimiser.optimal_results
-        if np.isnan(results_dict["y_val"]):
-            log.error(f"Energy optimisation failed for {optimiser.dims[0][0]}")
-        out_results_list.append(results_dict)
+        if func == pgf.gauss_on_step or func == pgf.hpge_peak:
+            hstep = step / (bg + np.mean(hist[:10]))
+            parguess["hstep"] = hstep
+
+        if func == pgf.hpge_peak:
+            sigma = sigma * 0.8  # roughly remove some amount due to tail
+            # for now hard-coded
+            htail = 1.0 / 5
+            tau = sigma / 2
+            parguess["sigma"] = sigma
+            parguess["htail"] = htail
+            parguess["tau"] = tau
+
+        for name, guess in parguess.items():
+            if np.isnan(guess):
+                parguess[name] = 0
+
+    else:
+        log.error(f"get_hpge_energy_peak_par_guess not implemented for {func.__name__}")
+        return return_nans(func)
 
-    return out_param_dict, out_results_list
+    return convert_to_minuit(parguess, func).values
 
 
-def get_ctc_grid(grids, ctc_param):
+def get_hpge_energy_fixed(func):
     """
-    Reshapes optimizer grids to be in easier form
+    Get the fixed indexes for fitting and mask for parameters based on the given function.
+
+    Parameters
+    ----------
+    func : function
+        The function for which the fixed indexes and mask are to be determined.
+
+    Returns
+    -------
+    fixed : list
+        A sequence list of fixed indexes for fitting.
+    mask : ndarray
+        A boolean mask indicating which parameters are fixed (False) and which are not fixed (True).
+    """
+
+    if (
+        func == pgf.gauss_on_step
+        or func == pgf.hpge_peak
+        or func == pgf.gauss_on_uniform
+    ):
+        # pars are: n_sig, mu, sigma, n_bkg, hstep, components
+        fixed = ["x_lo", "x_hi"]
+
+    else:
+        log.error(f"get_hpge_energy_fixed not implemented for {func.__name__}")
+        return None
+    mask = ~np.in1d(func.required_args(), fixed)
+    return fixed, mask
+
+
+def get_hpge_energy_bounds(func, parguess):
+    if func == pgf.gauss_on_step:
+        return {
+            "n_sig": (0, None),
+            "mu": (parguess["x_lo"], parguess["x_hi"]),
+            "sigma": (0, None),
+            "n_bkg": (0, None),
+            "hstep": (-1, 1),
+            "x_lo": (None, None),
+            "x_hi": (None, None),
+        }
+
+    elif func == pgf.hpge_peak:
+        return {
+            "n_sig": (0, None),
+            "mu": (parguess["x_lo"], parguess["x_hi"]),
+            "sigma": (0, None),
+            "htail": (0, 0.5),
+            "tau": (0.1 * parguess["sigma"], 10 * parguess["sigma"]),
+            "n_bkg": (0, None),
+            "hstep": (-1, 1),
+            "x_lo": (None, None),
+            "x_hi": (None, None),
+        }
+
+    if func == pgf.gauss_on_uniform:
+        return {
+            "n_sig": (0, None),
+            "mu": (parguess["x_lo"], parguess["x_hi"]),
+            "sigma": (0, None),
+            "n_bkg": (0, None),
+            "x_lo": (None, None),
+            "x_hi": (None, None),
+        }
+
+    else:
+        log.error(f"get_hpge_energy_bounds not implemented for {func.__name__}")
+        return []
+
+
+class TailPrior:
     """
-    error_grids = []
-    dt_grids = []
-    alpha_grids = []
-    alpha_error_grids = []
-    nevents_grids = []
-    for grid in grids:
-        shape = grid.shape
-        dt_grid = np.ndarray(shape=shape)
-        alpha_grid = np.ndarray(shape=shape)
-        error_grid = np.ndarray(shape=shape)
-        alpha_error_grid = np.ndarray(shape=shape)
-        nevents_grid = np.ndarray(shape=shape)
-        for i in range(shape[0]):
-            for j in range(shape[1]):
-                dt_grid[i, j] = grid[i, j][ctc_param]["fwhm"]
-                error_grid[i, j] = grid[i, j][ctc_param]["fwhm_err"]
-                nevents_grid[i, j] = grid[i, j][ctc_param]["n_sig"]
-                try:
-                    alpha_grid[i, j] = grid[i, j][ctc_param]["alpha"]
-                except:
-                    pass
-                try:
-                    alpha_error_grid[i, j] = grid[i, j][ctc_param]["alpha_err"]
-                except:
-                    pass
-        dt_grids.append(dt_grid)
-        alpha_grids.append(alpha_grid)
-        error_grids.append(error_grid)
-        alpha_error_grids.append(alpha_error_grid)
-        nevents_grids.append(nevents_grid)
-    return dt_grids, error_grids, alpha_grids, alpha_error_grids, nevents_grids
+    Generic least-squares cost function with error.
+    """
+
+    verbose = 0
+    errordef = Minuit.LIKELIHOOD  # for Minuit to compute errors correctly
 
+    def __init__(self, data, model, tail_weight=0):
+        self.model = model  # model predicts y for given x
+        self.data = data
+        self.tail_weight = tail_weight
 
-def interpolate_energy_old(peak_energies, grids, error_grids, energy, nevents_grids):
+    def _call(self, *pars):
+        return self.__call__(*pars[0])
+
+    def _value(self, *pars):
+        return self.__call__(*pars[0])
+
+    def __call__(
+        self,
+        x_lo,
+        x_hi,
+        n_sig,
+        mu,
+        sigma,
+        htail,
+        tau,
+        n_bkg,
+        hstep,
+    ):
+        return self.tail_weight * np.log(htail + 0.1)  # len(self.data)/
+
+
+def unbinned_staged_energy_fit(
+    energy,
+    func,
+    gof_range=None,
+    fit_range=None,
+    guess=None,
+    guess_func=get_hpge_energy_peak_par_guess,
+    bounds_func=get_hpge_energy_bounds,
+    fixed_func=get_hpge_energy_fixed,
+    guess_kwargs=None,
+    bounds_kwargs=None,
+    fixed_kwargs=None,
+    tol=None,
+    tail_weight=0,
+    allow_tail_drop=True,
+    bin_width=None,
+    lock_guess=False,
+    display=0,
+):
     """
-    Interpolates fwhm vs energy for every grid point
+    Unbinned fit to energy. This is different to the default fitting as
+    it will try different fitting methods and choose the best. This is necessary for the lower statistics.
     """
 
-    grid_no = len(grids)
-    grid_shape = grids[0].shape
-    out_grid = np.empty(grid_shape)
-    out_grid_err = np.empty(grid_shape)
-    n_event_lim = np.array(
-        [0.98 * np.nanpercentile(nevents_grid, 50) for nevents_grid in nevents_grids]
-    )
-    for index, x in np.ndenumerate(grids[0]):
-        points = np.array([grids[i][index] for i in range(len(grids))])
-        err_points = np.array([error_grids[i][index] for i in range(len(grids))])
-        n_sigs = np.array([nevents_grids[i][index] for i in range(len(grids))])
-        nan_mask = (
-            np.isnan(points)
-            | (points < 0)
-            | (0.1 * points < err_points)
-            | (n_sigs < n_event_lim)
+    if fit_range is None:
+        fit_range = (np.nanmin(energy), np.nanmax(energy))
+
+    if gof_range is None:
+        gof_range = fit_range
+
+    if bin_width is None:
+        init_bin_width = (
+            2
+            * (np.nanpercentile(energy, 75) - np.nanpercentile(energy, 25))
+            * len(energy) ** (-1 / 3)
+        )
+        init_hist, init_bins, _ = pgh.get_hist(
+            energy, dx=init_bin_width, range=fit_range
         )
         try:
-            if len(points[nan_mask]) > 2:
-                raise ValueError
-            elif nan_mask[-1] == True or nan_mask[-2] == True:
-                raise ValueError
-            param_guess = [0.2, 0.001, 0.000001]
-            param_bounds = param_bounds = (0, [1, np.inf, np.inf])  # ,0.1
-            fit_pars, fit_covs = curve_fit(
-                fwhm_slope,
-                peak_energies[~nan_mask],
-                points[~nan_mask],
-                sigma=err_points[~nan_mask],
-                p0=param_guess,
-                bounds=param_bounds,
-                absolute_sigma=True,
-            )  #
-            fit_qbb = fwhm_slope(energy, *fit_pars)
-            sderrs = np.sqrt(np.diag(fit_covs))
-            qbb_err = fwhm_slope(energy, *(fit_pars + sderrs)) - fwhm_slope(
-                energy, *fit_pars
-            )
-            out_grid[index] = fit_qbb
-            out_grid_err[index] = qbb_err
-        except:
-            out_grid[index] = np.nan
-            out_grid_err[index] = np.nan
-    return out_grid, out_grid_err
+            _, init_sigma, _ = pgh.get_gaussian_guess(init_hist, init_bins)
+        except IndexError:
+            init_hist, init_bins, _ = pgh.get_hist(
+                energy, dx=init_bin_width / 2, range=fit_range
+            )
+            try:
+                _, init_sigma, _ = pgh.get_gaussian_guess(init_hist, init_bins)
+            except IndexError:
+                init_sigma = np.nanstd(energy)
+        bin_width = 2 * (init_sigma) * len(energy) ** (-1 / 3)
 
+    gof_hist, gof_bins, gof_var = pgh.get_hist(energy, range=gof_range, dx=bin_width)
 
-def find_lowest_grid_point_save(grid, err_grid, opt_dict):
-    """
-    Finds the lowest grid point, if more than one with same value returns shortest filter.
-    """
-    opt_name = list(opt_dict.keys())[0]
-    print(opt_name)
-    keys = list(opt_dict[opt_name].keys())
-    param_list = []
-    shape = []
-    db_dict = {}
-    for key in keys:
-        param_dict = opt_dict[opt_name][key]
-        grid_axis = np.arange(
-            param_dict["start"], param_dict["end"], param_dict["spacing"]
-        )
-        unit = param_dict.get("unit")
-        param_list.append(grid_axis)
-        shape.append(len(grid_axis))
-
-    total_lengths = np.zeros(shape)
-
-    for index, x in np.ndenumerate(total_lengths):
-        for i, param in enumerate(param_list):
-            total_lengths[index] += param[index[i]]
-    min_val = np.nanmin(grid)
-    lowest_ixs = np.where(grid == min_val)
-    try:
-        fwhm_dict = {"fwhm": min_val, "fwhm_err": err_grid[lowest_ixs][0]}
-    except:
-        print(lowest_ixs)
-    if len(lowest_ixs[0]) == 1:
-        for i, key in enumerate(keys):
-            if i == 0:
-                if unit is not None:
-                    db_dict[opt_name] = {
-                        key: f"{param_list[i][lowest_ixs[i]][0]}*{unit}"
-                    }
-                else:
-                    db_dict[opt_name] = {key: f"{param_list[i][lowest_ixs[i]][0]}"}
+    if guess is not None:
+        if not isinstance(guess, ValueView):
+            x0 = convert_to_minuit(guess, func)
+        if lock_guess is True:
+            x0 = guess
+            x0["x_lo"] = fit_range[0]
+            x0["x_hi"] = fit_range[1]
+        else:
+            x0["x_lo"] = fit_range[0]
+            x0["x_hi"] = fit_range[1]
+            x1 = guess_func(
+                energy,
+                func,
+                fit_range,
+                bin_width=bin_width,
+                **guess_kwargs if guess_kwargs is not None else {},
+            )
+            for arg, val in x1.items():
+                if arg not in x0:
+                    x0[arg] = val
+            if len(x0) == len(x1):
+                cs, _ = pgb.goodness_of_fit(
+                    gof_hist, gof_bins, None, func.pdf_norm, x0, method="Pearson"
+                )
+                cs2, _ = pgb.goodness_of_fit(
+                    gof_hist, gof_bins, None, func.pdf_norm, x1, method="Pearson"
+                )
+                if cs >= cs2:
+                    x0 = x1
             else:
-                if unit is not None:
-                    db_dict[opt_name][key] = f"{param_list[i][lowest_ixs[i]][0]}*{unit}"
-                else:
-                    db_dict[opt_name][key] = f"{param_list[i][lowest_ixs[i]][0]}"
+                x0 = x1
     else:
-        shortest_length = np.argmin(total_lengths[lowest_ixs])
-        final_idxs = [lowest_ix[shortest_length] for lowest_ix in lowest_ixs]
-        for i, key in enumerate(keys):
-            if unit is not None:
-                db_dict[opt_name] = {key: f"{param_list[i][lowest_ixs[i]][0]}*{unit}"}
-            else:
-                db_dict[opt_name] = {key: f"{param_list[i][lowest_ixs[i]][0]}"}
-    return lowest_ixs, fwhm_dict, db_dict
+        if func == pgf.hpge_peak:
+            x0_notail = guess_func(
+                energy,
+                pgf.gauss_on_step,
+                fit_range,
+                bin_width=bin_width,
+                **guess_kwargs if guess_kwargs is not None else {},
+            )
+            c = cost.ExtendedUnbinnedNLL(energy, pgf.gauss_on_step.pdf_ext)
+            m = Minuit(c, *x0_notail)
+            bounds = bounds_func(
+                pgf.gauss_on_step,
+                x0_notail,
+                **bounds_kwargs if bounds_kwargs is not None else {},
+            )
+            for arg, val in bounds.items():
+                m.limits[arg] = val
+            fixed, mask = fixed_func(
+                pgf.gauss_on_step,
+                **fixed_kwargs if fixed_kwargs is not None else {},
+            )
+            m.fixed[fixed] = True
+            m.simplex().migrad()
+            m.hesse()
+            x0 = guess_func(
+                energy,
+                func,
+                fit_range,
+                bin_width=bin_width,
+                **guess_kwargs if guess_kwargs is not None else {},
+            )
+            if m.valid:
+                for arg in x0_notail.to_dict():
+                    x0[arg] = x0_notail[arg]
 
+        else:
+            x0 = guess_func(
+                energy,
+                func,
+                fit_range,
+                bin_width=bin_width,
+                **guess_kwargs if guess_kwargs is not None else {},
+            )
 
-def interpolate_grid(energies, grids, int_energy, deg, nevents_grids):
-    """
-    Interpolates energy vs parameter for every grid point using polynomial.
-    """
-    grid_no = len(grids)
-    grid_shape = grids[0].shape
-    out_grid = np.empty(grid_shape)
-    n_event_lim = np.array(
-        [0.98 * np.nanpercentile(nevents_grid, 50) for nevents_grid in nevents_grids]
-    )
-    for index, x in np.ndenumerate(grids[0]):
-        points = np.array([grids[i][index] for i in range(len(grids))])
-        n_sigs = np.array([nevents_grids[i][index] for i in range(len(grids))])
-        nan_mask = np.isnan(points) | (points < 0) | (n_sigs < n_event_lim)
-        try:
-            if len(points[~nan_mask]) < 3:
-                raise IndexError
-            fit_point = np.polynomial.polynomial.polyfit(
-                energies[~nan_mask], points[~nan_mask], deg=deg
-            )
-            out_grid[index] = np.polynomial.polynomial.polyval(int_energy, fit_point)
-        except:
-            out_grid[index] = np.nan
-    return out_grid
+    if (func == pgf.hpge_peak) and allow_tail_drop is True:
+        fit_no_tail = unbinned_staged_energy_fit(
+            energy,
+            func=pgf.gauss_on_step,
+            gof_range=gof_range,
+            fit_range=fit_range,
+            guess=None,
+            guess_func=guess_func,
+            bounds_func=bounds_func,
+            fixed_func=fixed_func,
+            guess_kwargs=guess_kwargs,
+            bounds_kwargs=bounds_kwargs,
+            fixed_kwargs=fixed_kwargs,
+            tol=tol,
+            tail_weight=None,
+            allow_tail_drop=False,
+            bin_width=bin_width,
+        )
+
+        c = cost.ExtendedUnbinnedNLL(energy, func.pdf_ext) + TailPrior(
+            energy, func, tail_weight=tail_weight
+        )
+    else:
+        c = cost.ExtendedUnbinnedNLL(energy, func.pdf_ext)
 
+    fixed, mask = fixed_func(func, **fixed_kwargs if fixed_kwargs is not None else {})
+    bounds = bounds_func(func, x0, **bounds_kwargs if bounds_kwargs is not None else {})
 
-def get_best_vals(peak_grids, peak_energies, param, opt_dict, save_path=None):
-    """
-    Finds best filter parameters
-    """
-    dt_grids, error_grids, alpha_grids, alpha_error_grids, nevents_grids = get_ctc_grid(
-        peak_grids, param
+    # try without simplex
+    m = Minuit(c, *x0)
+    if tol is not None:
+        m.tol = tol
+    m.fixed[fixed] = True
+    for arg, val in bounds.items():
+        m.limits[arg] = val
+    m.migrad()
+    m.hesse()
+
+    valid1 = (
+        m.valid
+        & (~np.isnan(np.array(m.errors)[mask]).any())
+        & (~(np.array(m.errors)[mask] == 0).all())
     )
-    qbb_grid, qbb_errs = interpolate_energy(
-        peak_energies, dt_grids, error_grids, 2039.061, nevents_grids
+
+    cs = pgb.goodness_of_fit(
+        gof_hist,
+        gof_bins,
+        gof_var,
+        func.get_pdf,
+        m.values,
+        method="Pearson",
+        scale_bins=True,
     )
-    qbb_alphas = interpolate_grid(
-        peak_energies[2:], alpha_grids[2:], 2039.061, 1, nevents_grids[2:]
+    cs = (cs[0], cs[1] + len(np.where(mask)[0]))
+
+    fit1 = (m.values, m.errors, m.covariance, cs, func, mask, valid1, m)
+
+    # Now try with simplex
+    m2 = Minuit(c, *x0)
+    if tol is not None:
+        m2.tol = tol
+    m2.fixed[fixed] = True
+    for arg, val in bounds.items():
+        m2.limits[arg] = val
+    m2.simplex().migrad()
+    m2.hesse()
+
+    valid2 = (
+        m2.valid
+        & (~np.isnan(np.array(m2.errors)[mask]).any())
+        & (~(np.array(m2.errors)[mask] == 0).all())
     )
-    ixs, fwhm_dict, db_dict = find_lowest_grid_point_save(qbb_grid, qbb_errs, opt_dict)
-    out_grid = {"fwhm": qbb_grid, "fwhm_err": qbb_errs, "alphas": qbb_alphas}
 
-    if isinstance(save_path, str):
-        mpl.use("pdf")
-        e_param = list(opt_dict.keys())[0]
-        opt_dict = opt_dict[e_param]
-
-        detector = save_path.split("/")[-1]
-        save_path = os.path.join(save_path, f"{e_param}-{param}.pdf")
-        pathlib.Path(os.path.dirname(save_path)).mkdir(parents=True, exist_ok=True)
-
-        with PdfPages(save_path) as pdf:
-            keys = list(opt_dict.keys())
-            print(keys)
-            x_dict = opt_dict[keys[1]]
-            xvals = np.arange(x_dict["start"], x_dict["end"], x_dict["spacing"])
-            xs = (
-                np.arange(0, len(xvals), 1),
-                np.arange(x_dict["start"], x_dict["end"], x_dict["spacing"]),
-            )
-            y_dict = opt_dict[keys[0]]
-            yvals = np.arange(y_dict["start"], y_dict["end"], y_dict["spacing"])
-            ys = (
-                np.arange(0, len(yvals), 1),
-                np.arange(y_dict["start"], y_dict["end"], y_dict["spacing"]),
-            )
-            for i, x in enumerate(xs[1]):
-                xs[1][i] = round(x, 1)
-            for i, y in enumerate(ys[1]):
-                ys[1][i] = round(y, 1)
-            print(ixs)
-            points = np.array(
-                [dt_grids[i][ixs[0][0], ixs[1][0]] for i in range(len(dt_grids))]
-            )
-            err_points = np.array(
-                [error_grids[i][ixs[0][0], ixs[1][0]] for i in range(len(error_grids))]
-            )
-            alpha_points = np.array(
-                [alpha_grids[i][ixs[0][0], ixs[1][0]] for i in range(len(alpha_grids))]
-            )
-            alpha_error_points = np.array(
-                [
-                    alpha_error_grids[i][ixs[0][0], ixs[1][0]]
-                    for i in range(len(alpha_error_grids))
-                ]
-            )
-            param_guess = [0.2, 0.001, 0.000001]
-            param_bounds = (0, [1, np.inf, np.inf])  # ,0.1
-            nan_mask = np.isnan(points)
-            nan_mask = nan_mask | (points < 0) | (0.1 * points < err_points)
-            fit_pars, fit_covs = curve_fit(
-                fwhm_slope,
-                peak_energies[~nan_mask],
-                points[~nan_mask],
-                sigma=err_points[~nan_mask],
-                p0=param_guess,
-                bounds=param_bounds,
-                absolute_sigma=True,
-            )  #
-            energy_x = np.arange(200, 2600, 10)
-            plt.rcParams["figure.figsize"] = (12, 18)
-            plt.rcParams["font.size"] = 12
-            plt.figure()
-            for i, dt_grid in enumerate(dt_grids):
-                plt.subplot(3, 2, i + 1)
-                v_min = np.nanmin(np.abs(dt_grid))
-                if v_min == 0:
-                    for j in range(10):
-                        v_min = np.nanpercentile(np.abs(dt_grid), j + 1)
-                        if v_min > 0.1:
-                            break
-                plt.imshow(
-                    dt_grid,
-                    norm=LogNorm(vmin=v_min, vmax=np.nanpercentile(dt_grid, 98)),
-                    cmap="viridis",
-                )
+    cs2 = pgb.goodness_of_fit(
+        gof_hist,
+        gof_bins,
+        gof_var,
+        func.get_pdf,
+        m2.values,
+        method="Pearson",
+        scale_bins=True,
+    )
+    cs2 = (cs2[0], cs2[1] + len(np.where(mask)[0]))
 
-                plt.xticks(xs[0], xs[1])
-                plt.yticks(ys[0], ys[1])
+    fit2 = (m2.values, m2.errors, m2.covariance, cs2, func, mask, valid2, m2)
 
-                plt.xlabel(f"{keys[1]} (us)")
-                plt.ylabel(f"{keys[0]} (us)")
-                plt.title(f"{peak_energies[i]:.1f} kev")
-                plt.xticks(rotation=45)
-                cbar = plt.colorbar()
-                cbar.set_label("FWHM (keV)")
-            plt.tight_layout()
-            plt.suptitle(f"{detector}-{e_param}-{param}")
-            pdf.savefig()
-            plt.close()
-
-            plt.figure()
-
-            plt.imshow(
-                qbb_grid,
-                norm=LogNorm(
-                    vmin=np.nanmin(qbb_grid), vmax=np.nanpercentile(dt_grid, 98)
-                ),
-                cmap="viridis",
-            )
-            plt.xlabel(f"{keys[1]} (us)")
-            plt.ylabel(f"{keys[0]} (us)")
-            plt.title(f"Qbb")
-            plt.xticks(rotation=45)
-            cbar = plt.colorbar()
-            cbar.set_label("FWHM (keV)")
-            plt.tight_layout()
-            plt.suptitle(f"{detector}-{e_param}-{param}")
-            pdf.savefig()
-            plt.close()
-
-            fig, (ax1, ax2) = plt.subplots(2, 1, constrained_layout=True, sharex=True)
-            ax1.errorbar(peak_energies, points, yerr=err_points, fmt=" ")
-            ax1.plot(energy_x, fwhm_slope(energy_x, *fit_pars))
-            ax1.errorbar(
-                [2039], qbb_grid[ixs[0], ixs[1]], yerr=qbb_errs[ixs[0], ixs[1]], fmt=" "
-            )
-            ax1.set_ylabel("FWHM energy resolution (keV)", ha="right", y=1)
-            ax2.scatter(
-                peak_energies,
-                (points - fwhm_slope(peak_energies, *fit_pars)) / err_points,
-                lw=1,
-                c="b",
-            )
-            ax2.set_xlabel("Energy (keV)", ha="right", x=1)
-            ax2.set_ylabel("Standardised Residuals", ha="right", y=1)
-            fig.suptitle(f"{detector}-{e_param}-{param}")
-            pdf.savefig()
-            plt.close()
+    frac_errors1 = np.sum(np.abs(np.array(m.errors)[mask] / np.array(m.values)[mask]))
+    frac_errors2 = np.sum(np.abs(np.array(m2.errors)[mask] / np.array(m2.values)[mask]))
+
+    if display > 1:
+        hist, bins, _ = pgh.get_hist(energy, range=fit_range, dx=bin_width)
+        bin_cs = (bins[:-1] + bins[1:]) / 2
+
+        m_fit = func.get_pdf(bin_cs, *m.values) * np.diff(bin_cs)[0]
+        m2_fit = func.get_pdf(bin_cs, *m2.values) * np.diff(bin_cs)[0]
+        guess_fit = func.get_pdf(bin_cs, *x0) * np.diff(bin_cs)[0]
+        plt.figure()
+        plt.step(bin_cs, hist, label="hist")
+        plt.plot(bin_cs, guess_fit, label="Guess")
+        plt.plot(bin_cs, m_fit, label=f"Fit 1: {cs}")
+        plt.plot(bin_cs, m2_fit, label=f"Fit 2: {cs2}")
+        plt.legend()
+        plt.show()
 
+    if valid1 is False and valid2 is False:
+        log.debug("Extra simplex needed")
+        m = Minuit(c, *x0)
+        if tol is not None:
+            m.tol = tol
+        m.fixed[fixed] = True
+        for arg, val in bounds.items():
+            m.limits[arg] = val
+        m.simplex().simplex().migrad()
+        m.hesse()
+        cs = pgb.goodness_of_fit(
+            gof_hist,
+            gof_bins,
+            gof_var,
+            func.get_pdf,
+            m.values,
+            method="Pearson",
+            scale_bins=True,
+        )
+        cs = (cs[0], cs[1] + len(np.where(mask)[0]))
+        valid3 = (
+            m.valid
+            & (~np.isnan(np.array(m.errors)[mask]).any())
+            & (~(np.array(m.errors)[mask] == 0).all())
+        )
+        if valid3 is False:
             try:
-                alphas = qbb_alphas[ixs[0], ixs[1]][0]
-                if isinstance(save_path, str):
-                    alpha_fit = np.polynomial.polynomial.polyfit(
-                        peak_energies[2:], alpha_points[2:], deg=1
-                    )
-                    fig, (ax1, ax2) = plt.subplots(
-                        2, 1, constrained_layout=True, sharex=True
-                    )
-                    ax1.errorbar(
-                        peak_energies[:],
-                        alpha_points[:],
-                        yerr=alpha_error_points[:],
-                        linestyle=" ",
-                    )
-                    ax1.plot(
-                        peak_energies[2:],
-                        np.polynomial.polynomial.polyval(peak_energies[2:], alpha_fit),
-                    )
-                    ax1.scatter([2039], qbb_alphas[ixs[0], ixs[1]])
-                    ax1.set_ylabel("Charge Trapping Value", ha="right", y=1)
-                    ax2.scatter(
-                        peak_energies[2:],
-                        (
-                            alpha_points[2:]
-                            - np.polynomial.polynomial.polyval(
-                                peak_energies[2:], alpha_fit
-                            )
-                        )
-                        / alpha_points[2:],
-                        lw=1,
-                        c="b",
-                    )
-                    ax2.set_xlabel("Energy (keV)", ha="right", x=1)
-                    ax2.set_ylabel("Residuals (%)", ha="right", y=1)
-                    fig.suptitle(f"{detector}-{param}")
-                    pdf.savefig()
-                    plt.close()
-            except:
-                alphas = np.nan
+                m.minos()
+                valid3 = (
+                    m.valid
+                    & (~np.isnan(np.array(m.errors)[mask]).any())
+                    & (~(np.array(m.errors)[mask] == 0).all())
+                )
+            except Exception:
+                raise RuntimeError
+
+        fit = (m.values, m.errors, m.covariance, cs, func, mask, valid3, m)
+
+    elif valid2 is False:
+        fit = fit1
+
+    elif valid1 is False:
+        fit = fit2
+
+    elif cs[0] * 1.05 < cs2[0]:
+        fit = fit1
+
+    elif cs2[0] * 1.05 < cs[0]:
+        fit = fit2
+
+    elif frac_errors1 < frac_errors2:
+        fit = fit1
+
+    elif frac_errors1 > frac_errors2:
+        fit = fit2
+
     else:
-        try:
-            alphas = qbb_alphas[ixs[0], ixs[1]][0]
-        except:
-            alphas = np.nan
-    return alphas, fwhm_dict, db_dict, out_grid
+        raise RuntimeError
+
+    if (func == pgf.hpge_peak) and allow_tail_drop is True:
+        p_val = chi2.sf(fit[3][0], fit[3][1])
+        p_val_no_tail = chi2.sf(fit_no_tail[3][0], fit_no_tail[3][1])
+        if fit[0]["htail"] < fit[1]["htail"] or p_val_no_tail > p_val:
+            debug_string = f'dropping tail tail val : {fit[0]["htail"]} tail err : {fit[1]["htail"]} '
+            debug_string += f"p_val no tail: : {p_val_no_tail} p_val with tail: {p_val}"
+            log.debug(debug_string)
+
+            if display > 0:
+                m_fit = pgf.gauss_on_step.get_pdf(bin_cs, *fit_no_tail[0])
+                m_fit_tail = pgf.hpge_peak.get_pdf(bin_cs, *fit[0])
+                plt.figure()
+                plt.step(bin_cs, hist, where="mid", label="hist")
+                plt.plot(
+                    bin_cs,
+                    m_fit * np.diff(bin_cs)[0],
+                    label=f"Drop tail: {p_val_no_tail}",
+                )
+                plt.plot(
+                    bin_cs,
+                    m_fit_tail * np.diff(bin_cs)[0],
+                    label=f"Drop tail: {p_val}",
+                )
+                plt.legend()
+                plt.show()
+
+            fit = fit_no_tail
+    return fit
+
+
+def poly_wrapper(x, *pars):
+    return pgf.nb_poly(x, np.array(pars))
 
 
-def get_filter_params(
-    grids, matched_configs, peak_energies, parameters, save_path=None
+def hpge_fit_energy_scale(mus, mu_vars, energies_kev, deg=0, fixed=None):
+    """Find best fit of poly(E) = mus +/- sqrt(mu_vars)
+    Compare to hpge_fit_energy_cal_func which fits for E = poly(mu)
+
+    Parameters
+    ----------
+    mus : array
+        uncalibrated energies
+    mu_vars : array
+        variances in the mus
+    energies_kev : array
+        energies to fit to, in kev
+    deg : int
+        degree for energy scale fit. deg=0 corresponds to a simple scaling
+        mu = scale * E. Otherwise deg follows the definition in np.polyfit
+    fixed : dict
+        dict where keys are index of polyfit pars to fix and vals are the value
+        to fix at, can be None to fix at guess value
+    Returns
+    -------
+    pars : array
+        parameters of the best fit. Follows the convention in np.polyfit
+    cov : 2D array
+        covariance matrix for the best fit parameters.
+    """
+    if deg == 0:
+        scale, scale_cov = fit_simple_scaling(energies_kev, mus, var=mu_vars)
+        pars = np.array([0, scale])
+        cov = np.array([[0, 0], [0, scale_cov]])
+        errs = np.diag(np.sqrt(cov))
+    else:
+        poly_pars = (
+            Polynomial.fit(energies_kev, mus, deg=deg, w=1 / np.sqrt(mu_vars))
+            .convert()
+            .coef
+        )
+        c = cost.LeastSquares(energies_kev, mus, np.sqrt(mu_vars), poly_wrapper)
+        if fixed is not None:
+            for idx, val in fixed.items():
+                if val is True or val is None:
+                    pass
+                else:
+                    poly_pars[idx] = val
+        m = Minuit(c, *poly_pars)
+        if fixed is not None:
+            for idx in list(fixed):
+                m.fixed[idx] = True
+        m.simplex()
+        m.migrad()
+        m.hesse()
+        pars = m.values
+        cov = m.covariance
+        errs = m.errors
+    return pars, errs, cov
+
+
+def hpge_fit_energy_cal_func(
+    mus, mu_vars, energies_kev, energy_scale_pars, deg=0, fixed=None
 ):
-    """
-    Finds best parameters for filter
-    """
+    """Find best fit of E = poly(mus +/- sqrt(mu_vars))
+    This is an inversion of hpge_fit_energy_scale.
+    E uncertainties are computed from mu_vars / dmu/dE where mu = poly(E) is the
+    E_scale function
 
-    full_db_dict = {}
-    full_fwhm_dict = {}
-    full_grids = {}
-
-    for param in parameters:
-        opt_dict = matched_configs[param]
-        peak_grids = grids[param]
-        ctc_params = list(peak_grids[0][0, 0].keys())
-        ctc_dict = {}
-
-        for ctc_param in ctc_params:
-            if ctc_param == "QDrift":
-                alpha, fwhm, db_dict, output_grid = get_best_vals(
-                    peak_grids, peak_energies, ctc_param, opt_dict, save_path=save_path
-                )
-                opt_name = list(opt_dict.keys())[0]
-                db_dict[opt_name].update({"alpha": alpha})
+    Parameters
+    ----------
+    mus : array
+        uncalibrated energies
+    mu_vars : array
+        variances in the mus
+    energies_kev : array
+        energies to fit to, in kev
+    energy_scale_pars : array
+        Parameters from the escale fit (kev to ADC) used for calculating
+        uncertainties
+    deg : int
+        degree for energy scale fit. deg=0 corresponds to a simple scaling
+        mu = scale * E. Otherwise deg follows the definition in np.polyfit
+    fixed : dict
+        dict where keys are index of polyfit pars to fix and vals are the value
+        to fix at, can be None to fix at guess value
+
+    Returns
+    -------
+    pars : array
+        parameters of the best fit. Follows the convention in np.polyfit
+    cov : 2D array
+        covariance matrix for the best fit parameters.
+    """
+    if deg == 0:
+        e_vars = mu_vars / energy_scale_pars[1] ** 2
+        scale, scale_cov = fit_simple_scaling(mus, energies_kev, var=e_vars)
+        pars = np.array([0, scale])
+        cov = np.array([[0, 0], [0, scale_cov]])
+        errs = np.diag(np.sqrt(cov))
+    else:
+        d_mu_d_es = np.zeros(len(mus))
+        for n in range(len(energy_scale_pars) - 1):
+            d_mu_d_es += energy_scale_pars[n + 1] * mus ** (n + 1)
+        e_weights = np.sqrt(d_mu_d_es * mu_vars)
+        poly_pars = (
+            Polynomial.fit(mus, energies_kev, deg=deg, w=1 / e_weights).convert().coef
+        )
+        if fixed is not None:
+            for idx, val in fixed.items():
+                if val is True or val is None:
+                    pass
+                else:
+                    poly_pars[idx] = val
+        c = cost.LeastSquares(mus, energies_kev, e_weights, poly_wrapper)
+        m = Minuit(c, *poly_pars)
+        if fixed is not None:
+            for idx in list(fixed):
+                m.fixed[idx] = True
+        m.simplex()
+        m.migrad()
+        m.hesse()
+        pars = m.values
+        errs = m.errors
+        cov = m.covariance
+    return pars, errs, cov
 
-            else:
-                alpha, fwhm, _, output_grid = get_best_vals(
-                    peak_grids, peak_energies, ctc_param, opt_dict, save_path=save_path
-                )
-            try:
-                full_grids[param][ctc_param] = output_grid
-            except:
-                full_grids[param] = {ctc_param: output_grid}
-            fwhm.update({"alpha": alpha})
-            ctc_dict[ctc_param] = fwhm
-        full_fwhm_dict[param] = ctc_dict
-        full_db_dict.update(db_dict)
-    return full_db_dict, full_fwhm_dict, full_grids
+
+def poly_match(xx, yy, deg=-1, rtol=1e-5, atol=1e-8, fixed=None):
+    """Find the polynomial function best matching pol(xx) = yy
+
+    Finds the poly fit of xx to yy that obtains the most matches between pol(xx)
+    and yy in the np.isclose() sense. If multiple fits give the same number of
+    matches, the fit with the best gof is used, where gof is computed only among
+    the matches.
+    Assumes that the relationship between xx and yy is monotonic
+
+    Parameters
+    ----------
+    xx : array-like
+        domain data array. Must be sorted from least to largest. Must satisfy
+        len(xx) >= len(yy)
+    yy : array-like
+        range data array: the values to which pol(xx) will be compared. Must be
+        sorted from least to largest. Must satisfy len(yy) > max(2, deg+2)
+    deg : int
+        degree of the polynomial to be used. If deg = 0, will fit for a simple
+        scaling: scale * xx = yy. If deg = -1, fits to a simple shift in the
+        data: xx + shift = yy. Otherwise, deg is equivalent to the deg argument
+        of np.polyfit()
+    rtol : float
+        the relative tolerance to be sent to np.isclose()
+    atol : float
+        the absolute tolerance to be sent to np.isclose(). Has the same units
+        as yy.
+
+    Returns
+    -------
+    pars: None or array of floats
+        The parameters of the best fit of poly(xx) = yy.  Follows the convention
+        used for the return value "p" of polyfit. Returns None when the inputs
+        are bad.
+    i_matches : list of int
+        list of indices in xx for the matched values in the best match
+    """
+
+    # input handling
+    xx = np.asarray(xx)
+    yy = np.asarray(yy)
+    #    if len(xx) <= len(yy):
+    #        print(f"poly_match error: len(xx)={len(xx)} <= len(yy)={len(yy)}")
+    #        return None, 0
+    deg = int(deg)
+    if deg < -1:
+        log.error(f"poly_match error: got bad deg = {deg}")
+        return None, 0
+    req_ylen = max(2, deg + 2)
+    if len(yy) < req_ylen:
+        log.error(
+            f"poly_match error: len(yy) must be at least {req_ylen} for deg={deg}, got {len(yy)}"
+        )
+        return None, 0
+
+    maxoverlap = min(len(xx), len(yy))
+
+    # build ixtup: the indices in xx to compare with the values in yy
+    ixtup = np.array(list(range(maxoverlap)))
+    iytup = np.array(list(range(maxoverlap)))
+    best_ixtup = None
+    best_iytup = None
+    n_close = 0
+    gof = np.inf  # lower is better gof
+    while True:
+        xx_i = xx[ixtup]
+        yy_i = yy[iytup]
+        gof_i = np.inf
+
+        # simple shift
+        if deg == -1:
+            pars_i = np.array([(np.sum(yy_i) - np.sum(xx_i)) / len(yy_i), 1])
+            polxx = xx_i + pars_i[0]
+
+        # simple scaling
+        elif deg == 0:
+            pars_i = np.array([0, np.sum(yy_i * xx_i) / np.sum(xx_i * xx_i)])
+            polxx = pars_i[1] * xx_i
+
+        # generic poly of degree >= 1
+        else:
+            poly_pars = Polynomial.fit(xx_i, yy_i, deg=deg).convert().coef
+            c = cost.LeastSquares(xx_i, yy_i, np.full_like(yy_i, 1), poly_wrapper)
+            if fixed is not None:
+                for idx, val in fixed.items():
+                    if val is True or val is None:
+                        pass
+                    else:
+                        poly_pars[idx] = val
+            m = Minuit(c, *poly_pars)
+            if fixed is not None:
+                for idx in list(fixed):
+                    m.fixed[idx] = True
+            pars_i = np.array(m.values)
+            polxx = np.zeros(len(yy_i))
+            polxx = pgf.nb_poly(xx_i, pars_i)
+
+        # by here we have the best polxx. Search for matches and store pars_i if
+        # its the best so far
+        matches = np.isclose(polxx, yy_i, rtol=rtol, atol=atol)
+        n_close_i = np.sum(matches)
+        if n_close_i >= n_close:
+            gof_i = np.sum(np.power(polxx[matches] - yy_i[matches], 2))
+            if n_close_i > n_close or (n_close_i == n_close and gof_i < gof):
+                n_close = n_close_i
+                gof = gof_i
+                pars = pars_i
+                best_ixtup = np.copy(ixtup)
+                best_iytup = np.copy(iytup)
+
+        # increment ixtup
+        # first find the index of ixtup that needs to be incremented
+        ii = 0
+        while ii < len(ixtup) - 1:
+            if ixtup[ii] < ixtup[ii + 1] - 1:
+                break
+            ii += 1
+
+        # quit if ii is the last index of ixtup and it's already maxed out
+        if not (ii == len(ixtup) - 1 and ixtup[ii] == len(xx) - 1):
+            # otherwise increment ii and reset indices < ii
+            ixtup[ii] += 1
+            ixtup[0:ii] = list(range(ii))
+            continue
+
+        # increment iytup
+        # first find the index of iytup that needs to be incremented
+        ii = 0
+        while ii < len(iytup) - 1:
+            if iytup[ii] < iytup[ii + 1] - 1:
+                break
+            ii += 1
+
+        # quit if ii is the last index of iytup and it's already maxed out
+        if not (ii == len(iytup) - 1 and iytup[ii] == len(yy) - 1):
+            # otherwise increment ii and reset indices < ii
+            iytup[ii] += 1
+            iytup[0:ii] = list(range(ii))
+            ixtup = np.array(list(range(len(iytup))))  # (reset ix)
+            continue
+
+        if n_close == len(iytup):  # found best
+            break
+
+        # reduce overlap
+        new_len = len(iytup) - 1
+        if new_len < req_ylen:
+            break
+        ixtup = np.array(list(range(new_len)))
+        iytup = np.array(list(range(new_len)))
+
+        best_ixtup = None
+        best_iytup = None
+        n_close = 0
+        gof = np.inf
+
+    return pars, best_ixtup, best_iytup
```

### Comparing `pygama-1.6.0a2/src/pygama/pargen/extract_tau.py` & `pygama-2.0.0a1/src/pygama/pargen/extract_tau.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,163 +1,195 @@
 """
 This module is for extracting a single pole zero constant from the decay tail
 """
 
 from __future__ import annotations
 
-import json
 import logging
-import os
-import pathlib
-import pickle as pkl
-from collections import OrderedDict
 
-import matplotlib as mpl
-
-mpl.use("agg")
 import lgdo
 import lgdo.lh5 as lh5
 import matplotlib.pyplot as plt
 import numpy as np
 
+import pygama.math.binned_fitting as pgf
 import pygama.math.histogram as pgh
-import pygama.math.peak_fitting as pgf
-import pygama.pargen.cuts as cts
 import pygama.pargen.dsp_optimize as opt
 import pygama.pargen.energy_optimisation as om
+from pygama.pargen.data_cleaning import get_mode_stdev
 
 log = logging.getLogger(__name__)
 sto = lh5.LH5Store()
 
 
-def load_data(
-    raw_file: list[str],
-    lh5_path: str,
-    pulser_mask=None,
-    n_events: int = 10000,
-    threshold: int = 5000,
-    wf_field: str = "waveform",
-) -> lgdo.Table:
-    df = sto.read(lh5_path, raw_file, field_mask=["daqenergy", "timestamp"])[0].view_as(
-        "pd"
-    )
-
-    if pulser_mask is None:
-        pulser_props = cts.find_pulser_properties(df, energy="daqenergy")
-        if len(pulser_props) > 0:
-            final_mask = None
-            for entry in pulser_props:
-                e_cut = (df.daqenergy.values < entry[0] + entry[1]) & (
-                    df.daqenergy.values > entry[0] - entry[1]
-                )
-                if final_mask is None:
-                    final_mask = e_cut
-                else:
-                    final_mask = final_mask | e_cut
-            ids = final_mask
-            log.debug(f"pulser found: {pulser_props}")
+class ExtractTau:
+    def __init__(self, dsp_config, wf_field, debug_mode=False):
+        self.dsp_config = dsp_config
+        self.wf_field = wf_field
+        self.output_dict = {}
+        self.results_dict = {}
+        self.debug_mode = debug_mode
+
+    def get_decay_constant(
+        self, slopes: np.array, wfs: lgdo.WaveformTable, display: int = 0
+    ) -> dict:
+        """
+        Finds the decay constant from the modal value of the tail slope after cuts
+        and saves it to the specified json. Updates self.output_dict with tau value
+
+        Parameters
+        ----------
+        - slopes: numpy array of tail slopes
+        - wfs: WaveformTable object containing waveform data
+        - display: integer indicating the level of display (0: no display, 1: plot histogram, 2: show histogram)
+
+        Returns
+        -------
+        - out_plot_dict: dictionary containing the plot figure (only returned if display > 0)
+        """
+
+        mode, stdev = get_mode_stdev(slopes)
+        tau = round(-1 / (mode), 1)
+        err = round((-1 / (mode + (stdev / np.sqrt(len(slopes))))) - tau, 1)
+
+        sampling_rate = wfs["dt"].nda[0]
+        units = wfs["dt"].attrs["units"]
+        tau = f"{tau*sampling_rate}*{units}"
+
+        if "pz" in self.output_dict:
+            self.output_dict["pz"].update({"tau": tau, "tau_err": err})
         else:
-            log.debug("no_pulser")
-            ids = np.zeros(len(df.daqenergy.values), dtype=bool)
-    else:
-        ids = pulser_mask
-
-    cuts = np.where((df.daqenergy.values > threshold) & (~ids))[0]
-
-    waveforms = sto.read(f"{lh5_path}/{wf_field}", raw_file, idx=cuts, n_rows=n_events)[
-        0
-    ]
-    baseline = sto.read(f"{lh5_path}/baseline", raw_file, idx=cuts, n_rows=n_events)[0]
-    tb_data = lh5.Table(col_dict={f"{wf_field}": waveforms, "baseline": baseline})
-    return tb_data
-
-
-def get_decay_constant(
-    slopes: np.array, wfs: lgdo.WaveformTable, display: int = 0
-) -> dict:
-    """
-    Finds the decay constant from the modal value of the tail slope after cuts
-    and saves it to the specified json.
-
-    Parameters
-    ----------
-    slopes : array
-        tail slope array
-
-    dict_file : str
-        path to json file to save decay constant value to.
-        It will be saved as a dictionary of form {'pz': {'tau': decay_constant}}
-
-    Returns
-    -------
-    tau_dict : dict
-    """
-    tau_dict = {}
-
-    pz = tau_dict.get("pz")
-
-    counts, bins, var = pgh.get_hist(slopes, bins=100000, range=(-0.01, 0))
-    bin_centres = pgh.get_bin_centers(bins)
-    high_bin = bin_centres[np.argmax(counts)]
-    try:
-        pars, cov = pgf.gauss_mode_width_max(
-            counts,
-            bins,
-            n_bins=10,
-            cost_func="Least Squares",
-            inflate_errors=False,
-            gof_method="var",
+            self.output_dict["pz"] = {"tau": tau, "tau_err": err}
+
+        self.results_dict.update(
+            {"single_decay_constant": {"slope_pars": {"mode": mode, "stdev": stdev}}}
         )
-        if np.abs(np.abs(pars[0] - high_bin) / high_bin) > 0.05:
-            raise ValueError
-        high_bin = pars[0]
-    except:
-        pass
-    tau = round(-1 / (high_bin), 1)
-
-    sampling_rate = wfs["dt"].nda[0]
-    units = wfs["dt"].attrs["units"]
-    tau = f"{tau*sampling_rate}*{units}"
-
-    tau_dict["pz"] = {"tau": tau}
-    if display > 0:
-        out_plot_dict = {}
+        if display <= 0:
+            return
+        else:
+            out_plot_dict = {}
+
+            return out_plot_dict
+
+    def get_dpz_consts(self, grid_out, opt_dict):
+        std_grid = np.ndarray(shape=grid_out.shape)
+        for i in range(grid_out.shape[0]):
+            for j in range(grid_out.shape[1]):
+                std_grid[i, j] = grid_out[i, j]["y_val"]
+        min_point = np.where(std_grid == np.amin(std_grid))
+
+        opt_name = list(opt_dict.keys())[0]
+        keys = list(opt_dict[opt_name].keys())
+        param_list = []
+        shape = []
+        db_dict = {}
+        for key in keys:
+            param_dict = opt_dict[opt_name][key]
+            grid_axis = np.arange(
+                param_dict["start"], param_dict["end"], param_dict["spacing"]
+            )
+            unit = param_dict.get("unit")
+            param_list.append(grid_axis)
+            shape.append(len(grid_axis))
+        for i, key in enumerate(keys):
+            unit = opt_dict[opt_name][key].get("unit")
+
+            if unit is not None:
+                try:
+                    db_dict[opt_name].update(
+                        {key: f"{param_list[i][min_point[i]][0]}*{unit}"}
+                    )
+                except BaseException as e:
+                    if e == KeyboardInterrupt:
+                        raise (e)
+                    elif self.debug_mode:
+                        raise (e)
+                    db_dict[opt_name] = {
+                        key: f"{param_list[i][min_point[i]][0]}*{unit}"
+                    }
+            else:
+                try:
+                    db_dict[opt_name].update({key: f"{param_list[i][min_point[i]][0]}"})
+                except BaseException as e:
+                    if e == KeyboardInterrupt:
+                        raise (e)
+                    elif self.debug_mode:
+                        raise (e)
+                    db_dict[opt_name] = {key: f"{param_list[i][min_point[i]][0]}"}
+        return db_dict
+
+    def calculate_dpz(self, tb_data, opt_dict):
+        log.debug("Calculating double pz constants")
+        pspace = om.set_par_space(opt_dict)
+        grid_out = opt.run_grid(
+            tb_data, self.dsp_config, pspace, fom_dpz, self.output_dict, fom_kwargs=None
+        )
+        out_dict = self.get_dpz_consts(grid_out, opt_dict)
+        if "pz" in self.output_dict:
+            self.output_dict["pz"].update(out_dict["pz"])
+        else:
+            self.output_dict["pz"] = out_dict["pz"]
+
+    def plot_waveforms_after_correction(
+        self, tb_data, wf_field, norm_param=None, display=0
+    ):
+        tb_out = opt.run_one_dsp(tb_data, self.dsp_config, db_dict=self.output_dict)
+        wfs = tb_out[wf_field]["values"].nda
+        wf_idxs = np.random.choice(len(wfs), 100)
+        if norm_param is not None:
+            means = tb_out[norm_param].nda[wf_idxs]
+            wfs = np.divide(wfs[wf_idxs], np.reshape(means, (len(wf_idxs), 1)))
+        else:
+            wfs = wfs[wf_idxs]
+        fig = plt.figure()
+        for wf in wfs:
+            plt.plot(np.arange(0, len(wf), 1), wf)
+        plt.axhline(1, color="black")
+        plt.axhline(0, color="black")
+        plt.xlabel("Samples")
+        plt.ylabel("ADU")
+        plot_dict = {"waveforms": fig}
+        if display > 1:
+            plt.show()
+        else:
+            plt.close()
+        return plot_dict
+
+    def plot_slopes(self, slopes, display=0):
+        high_bin = self.results_dict["single_decay_constant"]["slope_pars"]["mode"]
+        sigma = self.results_dict["single_decay_constant"]["slope_pars"]["stdev"]
         plt.rcParams["figure.figsize"] = (10, 6)
         plt.rcParams["font.size"] = 8
         fig, ax = plt.subplots()
-        bins = np.linspace(-0.01, 0, 100000)  # change if needed
+        bins = np.arange(
+            np.nanpercentile(slopes, 1),
+            np.nanpercentile(slopes, 99),
+            np.nanpercentile(slopes, 51) - np.nanpercentile(slopes, 50),
+        )
         counts, bins, bars = ax.hist(slopes, bins=bins, histtype="step")
-        plot_max = np.argmax(counts)
-        in_min = plot_max - 20
-        if in_min < 0:
-            in_min = 0
-        in_max = plot_max + 21
-        if in_max >= len(bins):
-            in_min = len(bins) - 1
+        ax.axvline(high_bin, color="red")
+        in_min = high_bin - 4 * sigma
+        in_max = high_bin + 4 * sigma
         plt.xlabel("Slope")
         plt.ylabel("Counts")
-        plt.yscale("log")
-        axins = ax.inset_axes([0.5, 0.45, 0.47, 0.47])
+        axins = ax.inset_axes([0.6, 0.6, 0.4, 0.4])
         axins.hist(
-            slopes[(slopes > bins[in_min]) & (slopes < bins[in_max])],
-            bins=200,
+            slopes[(slopes > in_min) & (slopes < in_max)],
+            bins=50,
             histtype="step",
         )
         axins.axvline(high_bin, color="red")
-        axins.set_xlim(bins[in_min], bins[in_max])
-        ax.set_xticks(ax.get_xticks())
-        ax.set_xticklabels(labels=ax.get_xticklabels(), rotation=45)
-        out_plot_dict["slope"] = fig
+        axins.set_xlim(in_min, in_max)
+        ax.set_xlim(np.nanpercentile(slopes, 1), np.nanpercentile(slopes, 99))
+        out_plot_dict = {"slope": fig}
         if display > 1:
             plt.show()
         else:
             plt.close()
-        return tau_dict, out_plot_dict
-    else:
-        return tau_dict
+        return out_plot_dict
 
 
 def fom_dpz(tb_data, verbosity=0, rand_arg=None):
     std = tb_data["pz_std"].nda
     counts, start_bins, var = pgh.get_hist(std, dx=0.1, range=(0, 400))
     max_idx = np.argmax(counts)
     mu = start_bins[max_idx]
@@ -170,127 +202,11 @@
             cost_func="Least Squares",
             inflate_errors=False,
             gof_method="var",
         )
 
         mu = pars[0]
 
-    except:
+    except Exception:
         mu = start_bins[max_idx]
 
     return {"y_val": np.abs(mu)}
-
-
-def get_dpz_consts(grid_out, opt_dict):
-    std_grid = np.ndarray(shape=grid_out.shape)
-    for i in range(grid_out.shape[0]):
-        for j in range(grid_out.shape[1]):
-            std_grid[i, j] = grid_out[i, j]["y_val"]
-    min_val = np.amin(std_grid)
-    min_point = np.where(std_grid == np.amin(std_grid))
-
-    opt_name = list(opt_dict.keys())[0]
-    keys = list(opt_dict[opt_name].keys())
-    param_list = []
-    shape = []
-    db_dict = {}
-    for key in keys:
-        param_dict = opt_dict[opt_name][key]
-        grid_axis = np.arange(
-            param_dict["start"], param_dict["end"], param_dict["spacing"]
-        )
-        unit = param_dict.get("unit")
-        param_list.append(grid_axis)
-        shape.append(len(grid_axis))
-    for i, key in enumerate(keys):
-        unit = opt_dict[opt_name][key].get("unit")
-
-        if unit is not None:
-            try:
-                db_dict[opt_name].update(
-                    {key: f"{param_list[i][min_point[i]][0]}*{unit}"}
-                )
-            except:
-                db_dict[opt_name] = {key: f"{param_list[i][min_point[i]][0]}*{unit}"}
-        else:
-            try:
-                db_dict[opt_name].update({key: f"{param_list[i][min_point[i]][0]}"})
-            except:
-                db_dict[opt_name] = {key: f"{param_list[i][min_point[i]][0]}"}
-    return db_dict
-
-
-def dsp_preprocess_decay_const(
-    tb_data,
-    dsp_config: dict,
-    double_pz: bool = False,
-    display: int = 0,
-    opt_dict: dict = None,
-    wf_field: str = "waveform",
-    wf_plot: str = "wf_pz",
-    norm_param: str = "pz_mean",
-    cut_parameters: dict = {"bl_mean": 4, "bl_std": 4, "bl_slope": 4},
-) -> dict:
-    """
-    This function calculates the pole zero constant for the input data
-
-    Parameters
-    ----------
-    f_raw : str
-        The raw file to run the macro on
-    dsp_config: str
-        Path to the dsp config file, this is a stripped down version which just includes cuts and slope of decay tail
-    channel:  str
-        Name of channel to process, should be name of lh5 group in raw files
-
-    Returns
-    -------
-    tau_dict : dict
-    """
-
-    tb_out = opt.run_one_dsp(tb_data, dsp_config)
-    log.debug("Processed Data")
-    cut_dict = cts.generate_cuts(tb_out, parameters=cut_parameters)
-    log.debug("Generated Cuts:", cut_dict)
-    idxs = cts.get_cut_indexes(tb_out, cut_dict)
-    log.debug("Applied cuts")
-    log.debug(f"{len(idxs)} events passed cuts")
-    slopes = tb_out["tail_slope"].nda
-    log.debug("Calculating pz constant")
-    if display > 0:
-        tau_dict, plot_dict = get_decay_constant(
-            slopes[idxs], tb_data[wf_field], display=display
-        )
-    else:
-        tau_dict = get_decay_constant(slopes[idxs], tb_data[wf_field])
-    if double_pz == True:
-        log.debug("Calculating double pz constants")
-        pspace = om.set_par_space(opt_dict)
-        grid_out = opt.run_grid(
-            tb_data, dsp_config, pspace, fom_dpz, tau_dict, fom_kwargs=None
-        )
-        out_dict = get_dpz_consts(grid_out, opt_dict)
-        tau_dict["pz"].update(out_dict["pz"])
-    if display > 0:
-        tb_out = opt.run_one_dsp(tb_data, dsp_config, db_dict=tau_dict)
-        wfs = tb_out[wf_plot]["values"].nda[idxs]
-        wf_idxs = np.random.choice(len(wfs), 100)
-        if norm_param is not None:
-            means = tb_out[norm_param].nda[idxs][wf_idxs]
-            wfs = np.divide(wfs[wf_idxs], np.reshape(means, (len(wf_idxs), 1)))
-        else:
-            wfs = wfs[wf_idxs]
-        fig2 = plt.figure()
-        for wf in wfs:
-            plt.plot(np.arange(0, len(wf), 1), wf)
-        plt.axhline(1, color="black")
-        plt.axhline(0, color="black")
-        plt.xlabel("Samples")
-        plt.ylabel("ADU")
-        plot_dict["waveforms"] = fig2
-        if display > 1:
-            plt.show()
-        else:
-            plt.close()
-        return tau_dict, plot_dict
-    else:
-        return tau_dict
```

### Comparing `pygama-1.6.0a2/src/pygama/pargen/lq_cal.py` & `pygama-2.0.0a1/src/pygama/pargen/lq_cal.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,25 @@
 from __future__ import annotations
 
-import json
 import logging
-import os
-import pathlib
 import re
 from datetime import datetime
-from typing import Callable
 
-import matplotlib as mpl
-
-mpl.use("agg")
-
-import lgdo.lh5_store as lh5
-import matplotlib.cm as cmx
 import matplotlib.colors as mcolors
 import matplotlib.dates as mdates
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-from iminuit import Minuit, cost, util
-from matplotlib.backends.backend_pdf import PdfPages
+from iminuit import Minuit, cost
 from matplotlib.colors import LogNorm
 from scipy.stats import linregress
 
 import pygama.math.histogram as pgh
-import pygama.math.peak_fitting as pgf
-import pygama.pargen.AoE_cal as aoe
-from pygama.pargen.utils import *
+import pygama.pargen.AoE_cal as AoE
+from pygama.math.distributions import gaussian
 
 log = logging.getLogger(__name__)
 
 
 def get_fit_range(lq: np.array) -> tuple(float, float):
     """
     Function for determining the fit range for a given distribution of lq values
@@ -107,15 +95,15 @@
 
 
 def binned_lq_fit(
     df: pd.DataFrame,
     lq_param: str,
     cal_energy_param: str,
     peak: float,
-    cdf=pgf.gauss_cdf,
+    cdf=gaussian,
     sidebands: bool = True,
 ):
     """Function for fitting a distribution of LQ values within a specified
         energy peak. Fits a gaussian to the distribution
 
     Parameters
     ----------
@@ -155,16 +143,16 @@
     hist[hist < 0] = 0
 
     bin_centers = (bins[:-1] + bins[1:]) / 2
 
     mu = bin_centers[np.argmax(hist)]
     _, sigma, _ = pgh.get_gaussian_guess(hist, bins)
 
-    c1 = cost.BinnedNLL(hist, bins, pgf.gauss_cdf, verbose=0)
-    m1 = Minuit(c1, mu, sigma)
+    c1 = cost.BinnedNLL(hist, bins, gaussian.get_cdf, verbose=0)
+    m1 = Minuit(c1, mu=mu, sigma=sigma)
     m1.simplex().migrad()
     m1.hesse()
 
     return m1.values, m1.errors, hist, bins
 
 
 def fit_time_means(tstamps, means, reses):
@@ -216,26 +204,25 @@
                 current_means, weights=1 / np.array(current_reses)
             )
     for tstamp in current_tstamps:
         out_dict[tstamp] = rolling_mean
     return out_dict
 
 
-class cal_lq:
-
+class LQCal:
     """A class for calibrating the LQ parameter and determining the LQ cut value"""
 
     def __init__(
         self,
         cal_dicts: dict,
         cal_energy_param: str,
         eres_func: callable,
-        cdf: callable = pgf.gauss_cdf,
+        cdf: callable = gaussian,
         selection_string: str = "is_valid_cal&is_not_pulser",
-        plot_options: dict = {},
+        debug_mode=False,
     ):
         """
         Parameters
         ----------
         cal_dicts: dict
             A dictionary containing the hit-level operations to apply
             to the data.
@@ -253,15 +240,15 @@
         """
 
         self.cal_dicts = cal_dicts
         self.cal_energy_param = cal_energy_param
         self.eres_func = eres_func
         self.cdf = cdf
         self.selection_string = selection_string
-        self.plot_options = plot_options
+        self.debug_mode = debug_mode
 
     def update_cal_dicts(self, update_dict):
         if re.match(r"(\d{8})T(\d{6})Z", list(self.cal_dicts)[0]):
             for tstamp in self.cal_dicts:
                 if tstamp in update_dict:
                     self.cal_dicts[tstamp].update(update_dict[tstamp])
                 else:
@@ -273,25 +260,17 @@
         """
         Calculates the average LQ value for DEP events for each specified run
         run_timestamp. Applies a time normalization based on the average LQ value
         in the DEP across all run_timestamps.
         """
 
         log.info("Starting LQ time correction")
-        self.timecorr_df = pd.DataFrame(
-            columns=["run_timestamp", "mean", "mean_err", "res", "res_err"]
-        )
+        self.timecorr_df = pd.DataFrame()
         try:
             if "run_timestamp" in df:
-                tstamps = sorted(np.unique(df["run_timestamp"]))
-                means = []
-                errors = []
-                reses = []
-                res_errs = []
-                final_tstamps = []
                 for tstamp, time_df in df.groupby("run_timestamp", sort=True):
                     try:
                         pars, errs, _, _ = binned_lq_fit(
                             time_df.query(f"{self.selection_string}"),
                             lq_param,
                             self.cal_energy_param,
                             peak=1592.5,
@@ -314,15 +293,20 @@
                                                 + errs["mu"] / pars["mu"]
                                             ),
                                         }
                                     ]
                                 ),
                             ]
                         )
-                    except:
+                    except BaseException as e:
+                        if e == KeyboardInterrupt:
+                            raise (e)
+                        elif self.debug_mode:
+                            raise (e)
+
                         self.timecorr_df = pd.concat(
                             [
                                 self.timecorr_df,
                                 pd.DataFrame(
                                     [
                                         {
                                             "run_timestamp": tstamp,
@@ -331,14 +315,15 @@
                                             "res": np.nan,
                                             "res_err": np.nan,
                                         }
                                     ]
                                 ),
                             ]
                         )
+
                 self.timecorr_df.set_index("run_timestamp", inplace=True)
                 time_dict = fit_time_means(
                     np.array(self.timecorr_df.index),
                     np.array(self.timecorr_df["mean"]),
                     np.array(self.timecorr_df["res"]),
                 )
 
@@ -369,34 +354,40 @@
                     )
                     self.timecorr_df = pd.concat(
                         [
                             self.timecorr_df,
                             pd.DataFrame(
                                 [
                                     {
+                                        "run_timestamp": np.nan,
                                         "mean": pars["mu"],
                                         "mean_err": errs["mu"],
                                         "res": pars["sigma"] / pars["mu"],
                                         "res_err": (pars["sigma"] / pars["mu"])
                                         * np.sqrt(
                                             errs["sigma"] / pars["sigma"]
                                             + errs["mu"] / pars["mu"]
                                         ),
                                     }
                                 ]
                             ),
                         ]
                     )
-                except:
+                except BaseException as e:
+                    if e == KeyboardInterrupt:
+                        raise (e)
+                    elif self.debug_mode:
+                        raise (e)
                     self.timecorr_df = pd.concat(
                         [
                             self.timecorr_df,
                             pd.DataFrame(
                                 [
                                     {
+                                        "run_timestamp": np.nan,
                                         "mean": np.nan,
                                         "mean_err": np.nan,
                                         "res": np.nan,
                                         "res_err": np.nan,
                                     }
                                 ]
                             ),
@@ -408,15 +399,19 @@
                         output_name: {
                             "expression": f"{lq_param}/a",
                             "parameters": {"a": pars["mu"]},
                         }
                     }
                 )
                 log.info("LQ time correction finished")
-        except:
+        except BaseException as e:
+            if e == KeyboardInterrupt:
+                raise (e)
+            elif self.debug_mode:
+                raise (e)
             log.error("LQ time correction failed")
             self.update_cal_dicts(
                 {
                     output_name: {
                         "expression": f"{lq_param}/a",
                         "parameters": {"a": np.nan},
                     }
@@ -430,15 +425,14 @@
         Deterimines the drift time correction parameters for LQ by fitting a degree 1 polynomial to
         the LQ vs drift time distribution for DEP events. Corrects for any linear dependence and
         centers the final LQ distribution to a mean of 0.
         """
 
         log.info("Starting LQ drift time correction")
         try:
-            dt_dict = {}
             pars = binned_lq_fit(df, lq_param, self.cal_energy_param, peak=1592.5)[0]
             mean = pars[0]
             sigma = pars[1]
 
             lq_mask = (df[lq_param] < (2 * sigma + mean)) & (
                 df[lq_param] > (mean - 2 * sigma)
             )
@@ -452,15 +446,19 @@
             )
             self.dt_fit_pars = result
 
             df["LQ_Classifier"] = (
                 df[lq_param] - df["dt_eff"] * self.dt_fit_pars[0] - self.dt_fit_pars[1]
             )
 
-        except:
+        except BaseException as e:
+            if e == KeyboardInterrupt:
+                raise (e)
+            elif self.debug_mode:
+                raise (e)
             log.error("LQ drift time correction failed")
             self.dt_fit_pars = (np.nan, np.nan)
 
         self.update_cal_dicts(
             {
                 "LQ_Classifier": {
                     "expression": f"{lq_param} - dt_eff*a - b",
@@ -487,45 +485,31 @@
             self.cut_fit_pars = pars
             self.cut_fit_errs = errs
             self.fit_hist = (hist, bins)
             self.cut_val = cut_val
 
             df["LQ_Cut"] = df[lq_param] < self.cut_val
 
-        except:
+        except BaseException as e:
+            if e == KeyboardInterrupt:
+                raise (e)
+            elif self.debug_mode:
+                raise (e)
             log.error("LQ cut determination failed")
             self.cut_val = np.nan
 
         self.update_cal_dicts(
             {
                 "LQ_Cut": {
                     "expression": f"({lq_param} < a)",
                     "parameters": {"a": self.cut_val},
                 }
             }
         )
 
-    def get_results_dict(self):
-        return {
-            "cal_energy_param": self.cal_energy_param,
-            "rt_correction": self.dt_fit_pars,
-            "cdf": self.cdf.__name__,
-            "1590-1596keV": self.timecorr_df.to_dict("index"),
-            "cut_value": self.cut_val,
-            "sfs": self.low_side_sf.to_dict("index"),
-        }
-
-    def fill_plot_dict(self, data, plot_dict={}):
-        for key, item in self.plot_options.items():
-            if item["options"] is not None:
-                plot_dict[key] = item["function"](self, data, **item["options"])
-            else:
-                plot_dict[key] = item["function"](self, data)
-        return plot_dict
-
     def calibrate(self, df, initial_lq_param):
         """Run the LQ calibration and calculate the cut value"""
 
         self.lq_timecorr(df, lq_param="LQ_Ecorr")
         log.info("Finished LQ Time Correction")
 
         self.drift_time_correction(
@@ -536,15 +520,15 @@
         self.get_cut_lq_dep(
             df, lq_param="LQ_Classifier", cal_energy_param=self.cal_energy_param
         )
         log.info("Finished Calculating the LQ Cut Value")
 
         final_lq_param = "LQ_Classifier"
         peaks_of_interest = [1592.5, 1620.5, 2039, 2103.53, 2614.50]
-        self.low_side_sf = pd.DataFrame(columns=["peak", "sf", "sf_err"])
+        self.low_side_sf = pd.DataFrame()
         fit_widths = [(40, 25), (25, 40), (0, 0), (25, 40), (50, 50)]
         self.low_side_peak_dfs = {}
 
         log.info("Calculating peak survival fractions")
         for i, peak in enumerate(peaks_of_interest):
             try:
                 select_df = df.query(f"{self.selection_string}")
@@ -552,65 +536,73 @@
                 if peak == 2039:
                     emin = 2 * fwhm
                     emax = 2 * fwhm
                     peak_df = select_df.query(
                         f"({self.cal_energy_param}>{peak-emin})&({self.cal_energy_param}<{peak+emax})"
                     )
 
-                    cut_df, sf, sf_err = aoe.compton_sf_sweep(
+                    cut_df, sf, sf_err = AoE.compton_sf_sweep(
                         peak_df[self.cal_energy_param].to_numpy(),
                         peak_df[final_lq_param].to_numpy(),
                         self.cut_val,
                         peak,
                         fwhm,
                         cut_range=(0, 0.6),
+                        n_samples=10,
                         mode="less",
                     )
                     self.low_side_sf = pd.concat(
                         [
                             self.low_side_sf,
                             pd.DataFrame([{"peak": peak, "sf": sf, "sf_err": sf_err}]),
                         ]
                     )
                     self.low_side_peak_dfs[peak] = cut_df
                 else:
                     emin, emax = fit_widths[i]
+                    fit_range = (peak - emin, peak + emax)
                     peak_df = select_df.query(
-                        f"({self.cal_energy_param}>{peak-emin})&({self.cal_energy_param}<{peak+emax})"
+                        f"({self.cal_energy_param}>{fit_range[0]})&({self.cal_energy_param}<{fit_range[1]})"
                     )
-                    cut_df, sf, sf_err = aoe.get_sf_sweep(
+                    cut_df, sf, sf_err = AoE.get_sf_sweep(
                         peak_df[self.cal_energy_param].to_numpy(),
                         peak_df[final_lq_param].to_numpy(),
                         self.cut_val,
                         peak,
                         fwhm,
+                        fit_range=fit_range,
                         cut_range=(0, 0.6),
+                        n_samples=10,
                         mode="less",
                     )
                     self.low_side_sf = pd.concat(
                         [
                             self.low_side_sf,
                             pd.DataFrame([{"peak": peak, "sf": sf, "sf_err": sf_err}]),
                         ]
                     )
                     self.low_side_peak_dfs[peak] = cut_df
                 log.info(f"{peak}keV: {sf:2.1f} +/- {sf_err:2.1f} %")
-            except:
+            except BaseException as e:
+                if e == KeyboardInterrupt:
+                    raise (e)
+                elif self.debug_mode:
+                    raise (e)
                 self.low_side_sf = pd.concat(
                     [
                         self.low_side_sf,
                         pd.DataFrame([{"peak": peak, "sf": np.nan, "sf_err": np.nan}]),
                     ]
                 )
                 log.error(f"LQ Survival fraction determination failed for {peak} peak")
         self.low_side_sf.set_index("peak", inplace=True)
 
 
 def plot_lq_mean_time(
-    lq_class, data, lq_param="LQ_Timecorr", figsize=[12, 8], fontsize=12
+    lq_class, data, lq_param="LQ_Timecorr", figsize=(12, 8), fontsize=12
 ) -> plt.figure:
     """Plots the mean LQ value calculated for each given timestamp"""
 
     plt.rcParams["figure.figsize"] = figsize
     plt.rcParams["font.size"] = fontsize
     fig, ax = plt.subplots(1, 1)
     # try:
@@ -643,26 +635,26 @@
     ax.fill_between(
         [datetime.strptime(tstamp, "%Y%m%dT%H%M%SZ") for tstamp in lq_class.cal_dicts],
         y1=np.array(grouped_means) - 0.4 * np.array(lq_class.timecorr_df["res"]),
         y2=np.array(grouped_means) + 0.4 * np.array(lq_class.timecorr_df["res"]),
         color="yellow",
         alpha=0.2,
     )
-    # except:
+    # except Exception:
     #     pass
     ax.set_xlabel("time")
     ax.set_ylabel("LQ mean")
-    myFmt = mdates.DateFormatter("%b %d")
-    ax.xaxis.set_major_formatter(myFmt)
+    myfmt = mdates.DateFormatter("%b %d")
+    ax.xaxis.set_major_formatter(myfmt)
     plt.close()
     return fig
 
 
 def plot_drift_time_correction(
-    lq_class, data, lq_param="LQ_Timecorr", figsize=[12, 8], fontsize=12
+    lq_class, data, lq_param="LQ_Timecorr", figsize=(12, 8), fontsize=12
 ) -> plt.figure:
     """Plots a 2D histogram of LQ versus effective drift time in a 6 keV
     window around the DEP. Additionally plots the fit results for the
     drift time correction."""
 
     plt.rcParams["figure.figsize"] = figsize
     plt.rcParams["font.size"] = fontsize
@@ -692,23 +684,23 @@
         plt.plot(x, model, color="r")
 
         plt.xlabel("Drift Time (ns)")
         plt.ylabel("LQ")
 
         plt.title("LQ versus Drift Time for DEP")
 
-    except:
+    except Exception:
         pass
 
     plt.tight_layout()
     plt.close()
     return fig
 
 
-def plot_lq_cut_fit(lq_class, data, figsize=[12, 8], fontsize=12) -> plt.figure:
+def plot_lq_cut_fit(lq_class, data, figsize=(12, 8), fontsize=12) -> plt.figure:
     """Plots the final histogram of LQ values for events in the
     DEP, and the fit results used for determining the cut
     value"""
 
     plt.rcParams["figure.figsize"] = figsize
     plt.rcParams["font.size"] = fontsize
     fig, (ax1, ax2) = plt.subplots(2, 1)
@@ -719,40 +711,40 @@
 
         ax1.stairs(hist, bins, label="data")
         xs = np.linspace(round(bins[0], 3), round(bins[-1], 3), len(bins) - 1)
         ls = np.sum(hist)
         dx = np.diff(bins)
         ax1.plot(
             xs,
-            pgf.gauss_pdf(xs, fit_pars[0], fit_pars[1], ls) * dx,
+            gaussian.pdf_norm(xs, fit_pars[0], fit_pars[1]) * dx * ls,
             label="Gaussian Fit",
         )
 
         # ax1.set_xlabel('LQ')
         ax1.set_title("Fit of LQ events in DEP")
         ax1.legend()
 
         bin_centers = (bins[:-1] + bins[1:]) / 2
         reses = (
-            hist - (pgf.gauss_pdf(bin_centers, fit_pars[0], fit_pars[1], ls) * dx)
-        ) / (pgf.gauss_pdf(bin_centers, fit_pars[0], fit_pars[1], ls) * dx)
+            hist - (gaussian.pdf_norm(bin_centers, fit_pars[0], fit_pars[1]) * dx * ls)
+        ) / (gaussian.pdf_norm(bin_centers, fit_pars[0], fit_pars[1]) * dx * ls)
         ax2.plot(bin_centers, reses, marker="s", linestyle="")
         ax2.set_xlabel("LQ")
         ax2.set_ylabel("residuals")
 
-    except:
+    except Exception:
         pass
 
     plt.tight_layout()
     plt.close()
     return fig
 
 
 def plot_survival_fraction_curves(
-    lq_class, data, figsize=[12, 8], fontsize=12
+    lq_class, data, figsize=(12, 8), fontsize=12
 ) -> plt.figure:
     """Plots the survival fraction curves as a function of
     LQ cut values for every peak of interest"""
 
     plt.rcParams["figure.figsize"] = figsize
     plt.rcParams["font.size"] = fontsize
 
@@ -768,32 +760,32 @@
 
         for peak, survival_df in lq_class.low_side_peak_dfs.items():
             try:
                 plt.errorbar(
                     survival_df.index,
                     survival_df["sf"],
                     yerr=survival_df["sf_err"],
-                    label=f'{aoe.get_peak_label(peak)} {peak} keV: {lq_class.low_side_sf.loc[peak]["sf"]:2.1f} +/- {lq_class.low_side_sf.loc[peak]["sf_err"]:2.1f} %',
+                    label=f'{AoE.get_peak_label(peak)} {peak} keV: {lq_class.low_side_sf.loc[peak]["sf"]:2.1f} +/- {lq_class.low_side_sf.loc[peak]["sf_err"]:2.1f} %',
                 )
-            except:
+            except Exception:
                 pass
-    except:
+    except Exception:
         pass
     vals, labels = plt.yticks()
     plt.yticks(vals, [f"{x:,.0f} %" for x in vals])
     plt.legend(loc="lower right")
     plt.xlabel("cut value")
     plt.ylabel("survival percentage")
     plt.ylim([0, 105])
     plt.close()
     return fig
 
 
 def plot_sf_vs_energy(
-    lq_class, data, xrange=(900, 3000), n_bins=701, figsize=[12, 8], fontsize=12
+    lq_class, data, xrange=(900, 3000), n_bins=701, figsize=(12, 8), fontsize=12
 ) -> plt.figure:
     """Plots the survival fraction as a function of energy"""
 
     plt.rcParams["figure.figsize"] = figsize
     plt.rcParams["font.size"] = fontsize
 
     fig = plt.figure()
@@ -808,15 +800,15 @@
         counts, bins, _ = pgh.get_hist(
             data.query(lq_class.selection_string)[lq_class.cal_energy_param],
             bins=bins,
         )
         survival_fracs = counts_pass / (counts + 10**-99)
 
         plt.step(pgh.get_bin_centers(bins_pass), 100 * survival_fracs)
-    except:
+    except Exception:
         pass
     plt.ylim([0, 100])
     vals, labels = plt.yticks()
     plt.yticks(vals, [f"{x:,.0f} %" for x in vals])
     plt.xlabel("energy (keV)")
     plt.ylabel("survival percentage")
     plt.close()
@@ -826,15 +818,15 @@
 def plot_spectra(
     lq_class,
     data,
     xrange=(900, 3000),
     n_bins=2101,
     xrange_inset=(1580, 1640),
     n_bins_inset=200,
-    figsize=[12, 8],
+    figsize=(12, 8),
     fontsize=12,
 ) -> plt.figure:
     """Plots a 2D histogram of the LQ classifier vs calibrated energy"""
 
     plt.rcParams["figure.figsize"] = figsize
     plt.rcParams["font.size"] = fontsize
 
@@ -899,15 +891,15 @@
         axins.hist(
             select_df.query(f"{lq_class.selection_string} & (~LQ_Cut)")[
                 lq_class.cal_energy_param
             ],
             bins=bins,
             histtype="step",
         )
-    except:
+    except Exception:
         pass
     ax.set_xlim(xrange)
     ax.set_yscale("log")
     plt.xlabel("energy (keV)")
     plt.ylabel("counts")
     plt.legend(loc="upper left")
     plt.close()
@@ -918,15 +910,15 @@
     lq_class,
     data,
     lq_param="LQ_Classifier",
     xrange=(800, 3000),
     yrange=(-2, 8),
     xn_bins=700,
     yn_bins=500,
-    figsize=[12, 8],
+    figsize=(12, 8),
     fontsize=12,
 ) -> plt.figure:
     plt.rcParams["figure.figsize"] = figsize
     plt.rcParams["font.size"] = fontsize
 
     fig = plt.figure()
     try:
@@ -935,15 +927,15 @@
             data.query(lq_class.selection_string)[lq_param],
             bins=[
                 np.linspace(xrange[0], xrange[1], xn_bins),
                 np.linspace(yrange[0], yrange[1], yn_bins),
             ],
             norm=LogNorm(),
         )
-    except:
+    except Exception:
         pass
     plt.xlabel("energy (keV)")
     plt.ylabel(lq_param)
     plt.xlim(xrange)
     plt.ylim(yrange)
     plt.close()
     return fig
```

### Comparing `pygama-1.6.0a2/src/pygama/pargen/noise_optimization.py` & `pygama-2.0.0a1/src/pygama/pargen/noise_optimization.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,37 @@
 """
 This module contains the functions for performing the filter optimisation.
 This happens with a grid search performed on ENC peak.
 """
 
-import inspect
-import json
 import logging
-import os
-import pathlib
-import pickle as pkl
-import sys
 import time
-from collections import namedtuple
 
 import lgdo
-import matplotlib as mpl
-
-mpl.use("agg")
 import matplotlib.pyplot as plt
 import numpy as np
-import pandas as pd
 import scipy.stats
-from iminuit import Minuit, cost, util
-from matplotlib.backends.backend_pdf import PdfPages
-from matplotlib.colors import LogNorm
-from scipy.interpolate import splev, splrep
+from scipy.interpolate import BSpline, splev, splrep
 from scipy.optimize import minimize
 
-import pygama.math.peak_fitting as pgf
+from pygama.math.binned_fitting import goodness_of_fit
+from pygama.math.distributions import gauss_on_uniform
 from pygama.math.histogram import get_hist
-from pygama.pargen.cuts import generate_cuts, get_cut_indexes
+from pygama.math.unbinned_fitting import fit_unbinned
 from pygama.pargen.dsp_optimize import run_one_dsp
-from pygama.pargen.energy_optimisation import index_data
 
 log = logging.getLogger(__name__)
 
 
 def noise_optimization(
     tb_data: lgdo.Table,
     dsp_proc_chain: dict,
     par_dsp: dict,
     opt_dict: dict,
     lh5_path: str,
-    verbose: bool = False,
     display: int = 0,
 ) -> dict:
     """
     This function calculates the optimal filter par.
     Parameters
     ----------
     tb_data : str
@@ -78,43 +63,37 @@
         sample_us = float(dsp_data["wf_presum"].dt.nda[0]) / 1000
         freq = np.linspace(0, (1 / sample_us) / 2, len(psd))
         fig, ax = plt.subplots(figsize=(12, 6.75), facecolor="white")
         ax.plot(freq, psd)
         ax.set_xscale("log")
         ax.set_yscale("log")
         ax.set_xlabel("frequency (MHz)")
-        ax.set_ylabel(f"power spectral density")
+        ax.set_ylabel("power spectral density")
 
         plot_dict = {}
         plot_dict["nopt"] = {"fft": {"frequency": freq, "psd": psd, "fig": fig}}
         plt.close()
 
     result_dict = {}
     ene_pars = [par for par in opt_dict_par.keys()]
     log.info(f"\nRunning optimization for {ene_pars}")
-    if verbose:
-        print(f"\nRunning optimization for {ene_pars}")
     for i, x in enumerate(samples):
         x = f"{x:.1f}"
         log.info(f"\nCase {i}, par = {x} us")
-        if verbose:
-            print(f"\nCase {i}, par = {x} us")
         for ene_par in ene_pars:
             dict_str = opt_dict_par[ene_par]["dict_str"]
             filter_par = opt_dict_par[ene_par]["filter_par"]
             if dict_str in par_dsp:
                 par_dsp[dict_str].update({filter_par: f"{x}*us"})
             else:
                 par_dsp[dict_str] = {filter_par: f"{x}*us"}
 
         t1 = time.time()
         dsp_data = run_one_dsp(tb_data, dsp_proc_chain, db_dict=par_dsp)
         log.info(f"Time to process dsp data {time.time()-t1:.2f} s")
-        if verbose:
-            print(f"Time to process dsp data {time.time()-t1:.2f} s")
 
         for ene_par in ene_pars:
             dict_str = opt_dict_par[ene_par]["dict_str"]
             ene_str = opt_dict_par[ene_par]["ene_str"]
             if dict_str not in result_dict:
                 result_dict[dict_str] = {}
             par_dict_res = result_dict[dict_str]
@@ -134,59 +113,47 @@
             par_dict_res[x] = {}
             par_dict_res[x]["energies"] = energies
             par_dict_res[x]["fom"] = fom_results["fom"]
             par_dict_res[x]["fom_err"] = fom_results["fom_err"]
 
     for ene_par in ene_pars:
         log.info(f"\nOptimization for {ene_par}")
-        if verbose:
-            print(f"\nOptimization for {ene_par}")
         dict_str = opt_dict_par[ene_par]["dict_str"]
         par_dict_res = result_dict[dict_str]
         sample_list = np.array([float(x) for x in result_dict[dict_str].keys()])
         fom_list = np.array(
             [result_dict[dict_str][x]["fom"] for x in result_dict[dict_str].keys()]
         )
         fom_err_list = np.array(
             [result_dict[dict_str][x]["fom_err"] for x in result_dict[dict_str].keys()]
         )
 
         guess_par = sample_list[np.nanargmin(fom_list)]
-        if verbose:
-            print(f"guess par: {guess_par:.2f} us")
 
         tck = splrep(sample_list, fom_list, k=opt_dict["fit_deg"])
+        tck = BSpline(tck[0], tck[1], tck[2])
 
-        def spl_func(x_val):
-            return splev(x_val, tck)
-
-        result = minimize(spl_func, guess_par)
+        result = minimize(splev, guess_par, args=(tck))
         best_par = result.x[0]
         if (best_par < np.min(sample_list)) or (best_par > np.max(sample_list)):
             log.info(
                 f"Par from minimization not accepted {best_par:.2f}, setting par to guess"
             )
-            if verbose:
-                print(
-                    f"Par from minimization not accepted {best_par:.2f}, setting par to guess"
-                )
             best_par = guess_par
 
-        best_val = spl_func(best_par)
+        best_val = splev(best_par, tck)
 
         b_best_pars = np.zeros(opt_dict["n_bootstrap_samples"])
         for i in range(opt_dict["n_bootstrap_samples"]):
             indices = np.random.choice(len(sample_list), len(sample_list), replace=True)
             b_sample_list = sample_list[indices]
             b_fom_list = fom_list[indices]
             b_best_pars[i] = b_sample_list[np.nanargmin(b_fom_list)]
         best_par_err = np.std(b_best_pars)
         log.info(f"best par: {best_par:.2f} ± {best_par_err:.2f} us")
-        if verbose:
-            print(f"best par: {best_par:.2f} ± {best_par_err:.2f} us")
 
         par_dict_res["best_par"] = best_par
         par_dict_res["best_par_err"] = best_par_err
         par_dict_res["best_val"] = best_val
 
         filter_par = opt_dict_par[ene_par]["filter_par"]
         res_dict[dict_str] = {
@@ -206,16 +173,14 @@
                 )
                 bc = (bins[:-1] + bins[1:]) / 2.0
                 string_res = (
                     f"par = {x} us, FOM = {fom_list[i]:.3f} ± {fom_err_list[i]:.3f} ADC"
                 )
                 ax.plot(bc, hist, ds="steps", label=string_res)
                 log.info(string_res)
-                if verbose:
-                    print(string_res)
             ax.set_xlabel("energy (ADC)")
             ax.set_ylabel("counts")
             ax.legend(loc="upper right")
             par_dict_res["distribution"] = fig
             if display > 1:
                 plt.show()
             else:
@@ -229,15 +194,15 @@
                 color="b",
                 fmt="x",
                 ms=4,
                 ls="",
                 capsize=4,
                 label="samples",
             )
-            ax.plot(samples_val, spl_func(samples_val), "k:", label="fit")
+            ax.plot(samples_val, splev(samples_val, tck), "k:", label="fit")
             ax.errorbar(
                 best_par,
                 best_val,
                 xerr=best_par_err,
                 color="r",
                 fmt="o",
                 ms=6,
@@ -252,16 +217,14 @@
                 plt.show()
             else:
                 plt.close()
             par_dict_res["optimization"] = fig
             plot_dict["nopt"][dict_str] = par_dict_res
 
     log.info(f"Time to complete the optimization {time.time()-t0:.2f} s")
-    if verbose:
-        print(f"Time to complete the optimization {time.time()-t0:.2f} s")
     if display > 0:
         return res_dict, plot_dict
     else:
         return res_dict
 
 
 def calculate_spread(energies, percentile_low, percentile_high, n_samples):
@@ -282,66 +245,66 @@
     return results
 
 
 def simple_gaussian_fit(energies, dx=1, sigma_thr=4, allowed_p_val=1e-20):
     fit_range = [np.percentile(energies, 0.2), np.percentile(energies, 99.8)]
 
     hist, bins, var = get_hist(energies, range=fit_range, dx=dx)
-    guess, bounds = simple_gaussian_guess(hist, bins, pgf.extended_gauss_pdf)
+    guess, bounds = simple_gaussian_guess(hist, bins, gauss_on_uniform)
     fit_range = [guess[0] - sigma_thr * guess[1], guess[0] + sigma_thr * guess[1]]
 
     energies_fit = energies[(energies > fit_range[0]) & (energies < fit_range[1])]
-    pars, errs, cov = pgf.fit_unbinned(
-        pgf.extended_gauss_pdf,
+    pars, errs, cov = fit_unbinned(
+        gauss_on_uniform.pdf_ext,
         energies_fit,
         guess=guess,
         bounds=bounds,
     )
 
     mu, mu_err = pars[0], errs[0]
     fwhm = pars[1] * 2 * np.sqrt(2 * np.log(2))
     fwhm_err = errs[1] * 2 * np.sqrt(2 * np.log(2))
 
     hist, bins, var = get_hist(energies_fit, range=fit_range, dx=dx)
     gof_pars = pars
     gof_pars[2] *= dx
-    chisq, dof = pgf.goodness_of_fit(
-        hist, bins, None, pgf.gauss_pdf, gof_pars, method="Pearson"
+    chisq, dof = goodness_of_fit(
+        hist, bins, None, gauss_on_uniform.pdf_norm, gof_pars, method="Pearson"
     )
     p_val = scipy.stats.chi2.sf(chisq, dof + len(gof_pars))
 
     if (
-        sum(sum(c) if c is not None else 0 for c in cov[:3, :][:, :3]) == np.inf
-        or sum(sum(c) if c is not None else 0 for c in cov[:3, :][:, :3]) == 0
-        or np.isnan(sum(sum(c) if c is not None else 0 for c in cov[:3, :][:, :3]))
+        sum(sum(c) if c is not None else 0 for c in cov[2:, :][:, 2:]) == np.inf
+        or sum(sum(c) if c is not None else 0 for c in cov[2:, :][:, 2:]) == 0
+        or np.isnan(sum(sum(c) if c is not None else 0 for c in cov[2:, :][:, 2:]))
     ):
         log.debug("fit failed, cov estimation failed")
         fit_failed = True
-    elif (np.abs(np.array(errs)[:3] / np.array(pars)[:3]) < 1e-7).any() or np.isnan(
-        np.array(errs)[:3]
+    elif (np.abs(np.array(errs)[2:] / np.array(pars)[2:]) < 1e-7).any() or np.isnan(
+        np.array(errs)[2:]
     ).any():
         log.debug("fit failed, parameter error too low")
         fit_failed = True
     elif p_val < allowed_p_val or np.isnan(p_val):
         log.debug("fit failed, parameter error too low")
         fit_failed = True
     else:
         fit_failed = False
 
     if fit_failed:
-        log.debug(f"Returning values from guess")
+        log.debug("Returning values from guess")
         mu = guess[0]
         mu_err = 0
         fwhm = guess[1] * 2 * np.sqrt(2 * np.log(2))
         fwhm_err = 0
 
     results = {
-        "pars": pars[:3],
-        "errors": errs[:3],
-        "covariance": cov[:3],
+        "pars": pars,
+        "errors": errs,
+        "covariance": cov,
         "mu": mu,
         "mu_err": mu_err,
         "fom": fwhm,
         "fom_err": fwhm_err,
         "chisq": chisq / dof,
         "p_val": p_val,
     }
@@ -368,22 +331,22 @@
     min_idx = max_idx - n_bins_range
     max_idx = max_idx + n_bins_range
     min_idx = max(0, min_idx)
     max_idx = min(len(hist), max_idx)
 
     n_sig = np.sum(hist[min_idx:max_idx])
 
-    guess = [mu, sigma, n_sig]
-    bounds = [
-        (mu - sigma, mu + sigma),
-        (sigma - sigma * toll, sigma + sigma * toll),
-        (n_sig + n_sig * toll, n_sig + n_sig * toll),
-    ]
-
-    for i, par in enumerate(inspect.getfullargspec(func)[0][1:]):
-        if par == "lower_range" or par == "upper_range":
-            guess.append(np.inf)
-            bounds.append(None)
-        elif par == "n_bkg" or par == "hstep" or par == "components":
-            guess.append(0)
-            bounds.append(None)
+    guess = {"mu": mu, "sigma": sigma, "n_sig": n_sig}
+    bounds = {
+        "mu": (mu - sigma, mu + sigma),
+        "sigma": (sigma - sigma * toll, sigma + sigma * toll),
+        "n_sig": (n_sig + n_sig * toll, n_sig + n_sig * toll),
+    }
+
+    for par in func.required_args():
+        if par == "x_lo" or par == "x_hi":
+            guess[par] = np.inf
+            bounds[par] = None
+        elif par == "n_bkg" or par == "hstep":
+            guess[par] = 0
+            bounds[par] = None
     return guess, bounds
```

### Comparing `pygama-1.6.0a2/src/pygama.egg-info/PKG-INFO` & `pygama-2.0.0a1/src/pygama.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 Metadata-Version: 2.1
 Name: pygama
-Version: 1.6.0a2
-Summary: Python package for decoding and processing digitizer data
-Home-page: https://github.com/legend-exp/pygama
+Version: 2.0.0a1
+Summary: Python package for data processing and analysis
 Author: The LEGEND collaboration
 Maintainer: The LEGEND collaboration
-License: GPL-3.0
-Project-URL: Documentation, https://pygama.readthedocs.io
+Project-URL: Homepage, https://github.com/legend-exp/pygama
+Project-URL: Bug Tracker, https://github.com/legend-exp/pygama/issues
+Project-URL: Discussions, https://github.com/legend-exp/pygama/discussions
+Project-URL: Changelog, https://github.com/legend-exp/pygama/releases
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Software Development
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: hist
 Requires-Dist: colorlog
-Requires-Dist: dspeed>=1.3.0a4
+Requires-Dist: dspeed>=1.3
 Requires-Dist: h5py>=3.2
 Requires-Dist: iminuit
-Requires-Dist: legend-daq2lh5>=1.2.0a1
-Requires-Dist: legend-pydataobj>=1.5.0a5
+Requires-Dist: legend-daq2lh5>=1.2.1
+Requires-Dist: legend-pydataobj>=1.6
 Requires-Dist: matplotlib
 Requires-Dist: numba!=0.53.*,!=0.54.*,!=0.57
 Requires-Dist: numpy>=1.21
 Requires-Dist: pandas>=1.4.4
 Requires-Dist: pint
+Requires-Dist: pyyaml
 Requires-Dist: scikit-learn
 Requires-Dist: scipy>=1.0.1
 Requires-Dist: tables
-Requires-Dist: tqdm>=4.27
+Requires-Dist: tqdm>=4.66
 Provides-Extra: all
 Requires-Dist: pygama[docs,test]; extra == "all"
 Provides-Extra: docs
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: jupyter; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: nbsphinx; extra == "docs"
@@ -67,14 +65,15 @@
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Codecov](https://img.shields.io/codecov/c/github/legend-exp/pygama?logo=codecov)](https://app.codecov.io/gh/legend-exp/pygama)
 [![GitHub issues](https://img.shields.io/github/issues/legend-exp/pygama?logo=github)](https://github.com/legend-exp/pygama/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/legend-exp/pygama?logo=github)](https://github.com/legend-exp/pygama/pulls)
 [![License](https://img.shields.io/github/license/legend-exp/pygama)](https://github.com/legend-exp/pygama/blob/main/LICENSE)
 [![Read the Docs](https://img.shields.io/readthedocs/pygama?logo=readthedocs)](https://pygama.readthedocs.io)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10614246.svg)](https://zenodo.org/doi/10.5281/zenodo.10614246)
 
 *pygama* is a Python package for:
 
 - converting physics data acquisition system output to
   [LH5-format](https://legend-exp.github.io/legend-data-format-specs) HDF5
   files (functionality provided by the
   [legend-pydataobj](https://legend-pydataobj.readthedocs.io) and
@@ -83,11 +82,18 @@
   (functionality provided by the [dspeed](https://dspeed.readthedocs.io)
   package)
 - optimizing DSP routines and tuning associated analysis parameters
 - generating and selecting high-level event data for further analysis
 
 Check out the [online documentation](https://pygama.readthedocs.io).
 
+If you are using this software, consider
+[citing](https://zenodo.org/doi/10.5281/zenodo.10614246)!
+
 ## Related repositories
-- [legend-exp/legend-pydataobj](https://github.com/legend-exp/legend-pydataobj) → LEGEND Python Data Objects
-- [legend-exp/legend-daq2lh5](https://github.com/legend-exp/legend-daq2lh5) → Convert digitizer data to LEGEND HDF5
-- [legend-exp/dspeed](https://github.com/legend-exp/dspeed) → Fast Digital Signal Processing for particle detector signals in Python
+
+- [legend-exp/legend-pydataobj](https://github.com/legend-exp/legend-pydataobj)
+  → LEGEND Python Data Objects
+- [legend-exp/legend-daq2lh5](https://github.com/legend-exp/legend-daq2lh5)
+  → Convert digitizer data to LEGEND HDF5
+- [legend-exp/dspeed](https://github.com/legend-exp/dspeed)
+  → Fast Digital Signal Processing for particle detector signals in Python
```

### Comparing `pygama-1.6.0a2/tests/configs/icpc-dsp-config.json` & `pygama-2.0.0a1/tests/configs/icpc-dsp-config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.6.0a2/tests/configs/sipm-dplms-config.json` & `pygama-2.0.0a1/tests/configs/sipm-dplms-config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.6.0a2/tests/configs/sipm-dsp-config.json` & `pygama-2.0.0a1/tests/configs/sipm-dsp-config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.6.0a2/tests/conftest.py` & `pygama-2.0.0a1/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     if exitstatus == 0 and os.path.exists(_tmptestdir):
         shutil.rmtree(_tmptestdir)
 
 
 @pytest.fixture(scope="session")
 def lgnd_test_data():
     ldata = LegendTestData()
-    ldata.checkout("c089a59")
+    ldata.checkout("8f55832")
     return ldata
 
 
 @pytest.fixture(scope="session")
 def dsp_test_file(lgnd_test_data, tmptestdir):
     out_name = f"{tmptestdir}/LDQTA_r117_20200110T105115Z_cal_geds_dsp.lh5"
     build_dsp(
```

### Comparing `pygama-1.6.0a2/tests/evt/configs/basic-evt-config.json` & `pygama-2.0.0a1/tests/evt/configs/vov-test-evt-config.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6693080741068357%*

 * *Differences: {"'channels'": "{'ts_master': 'ch1084803'}",*

 * * "'operations'": "{'multiplicity': {'dtype': 'int16', delete: ['lgdo_attrs']}, 'energy': "*

 * *                 "{'aggregation_mode': 'gather', 'dtype': 'float32', delete: ['initial']}, "*

 * *                 "'energy_id': {'aggregation_mode': 'gather', 'sort': 'ascend_by:dsp.tp_0_est'}, "*

 * *                 "'energy_idx': {'aggregation_mode': 'gather', 'initial': 0, 'sort': "*

 * *                 "'ascend_by:dsp.tp_0_est'}, 'aoe': {delete: ['initial']}, 'timestamp': "*

 * *        […]*

```diff
@@ -1,98 +1,93 @@
 {
     "channels": {
         "geds_on": [
             "ch1084803",
             "ch1084804",
             "ch1121600"
-        ]
+        ],
+        "ts_master": "ch1084803"
     },
     "operations": {
         "aoe": {
             "aggregation_mode": "keep_at_ch:evt.energy_id",
-            "expression": "hit.AoE_Classifier",
-            "initial": "np.nan"
+            "expression": "hit.AoE_Classifier"
         },
-        "energy": {
-            "aggregation_mode": "first_at:dsp.tp_0_est",
-            "channels": "geds_on",
-            "expression": "hit.cuspEmax_ctc_cal",
-            "initial": "np.nan",
-            "query": "hit.cuspEmax_ctc_cal>25"
-        },
-        "energy_all_above1MeV": {
-            "aggregation_mode": "all",
-            "channels": "geds_on",
-            "expression": "hit.cuspEmax_ctc_cal>1000",
-            "initial": false
+        "aoe_idx": {
+            "aggregation_mode": "keep_at_idx:evt.energy_idx",
+            "expression": "hit.AoE_Classifier"
         },
-        "energy_any_above1MeV": {
-            "aggregation_mode": "any",
-            "channels": "geds_on",
-            "expression": "hit.cuspEmax_ctc_cal>1000",
-            "initial": false
-        },
-        "energy_aux": {
-            "aggregation_mode": "last_at:dsp.tp_0_est",
+        "energy": {
+            "aggregation_mode": "gather",
             "channels": "geds_on",
+            "dtype": "float32",
             "expression": "hit.cuspEmax_ctc_cal",
-            "initial": "np.nan",
             "query": "hit.cuspEmax_ctc_cal>25"
         },
         "energy_id": {
-            "aggregation_mode": "first_at:dsp.tp_0_est",
+            "aggregation_mode": "gather",
             "channels": "geds_on",
             "expression": "tcm.array_id",
             "initial": 0,
-            "query": "hit.cuspEmax_ctc_cal>25"
+            "query": "hit.cuspEmax_ctc_cal>25",
+            "sort": "ascend_by:dsp.tp_0_est"
         },
         "energy_idx": {
-            "aggregation_mode": "first_at:dsp.tp_0_est",
+            "aggregation_mode": "gather",
             "channels": "geds_on",
             "expression": "tcm.index",
-            "initial": 999999999999,
-            "query": "hit.cuspEmax_ctc_cal>25"
+            "initial": 0,
+            "query": "hit.cuspEmax_ctc_cal>25",
+            "sort": "ascend_by:dsp.tp_0_est"
         },
         "energy_sum": {
             "aggregation_mode": "sum",
             "channels": "geds_on",
             "expression": "hit.cuspEmax_ctc_cal",
-            "initial": 0.0,
+            "initial": 0,
             "query": "hit.cuspEmax_ctc_cal>25"
         },
-        "is_aoe_rejected": {
-            "aggregation_mode": "keep_at_ch:evt.energy_id",
-            "expression": "~(hit.AoE_Double_Sided_Cut)",
-            "initial": false
+        "energy_times_aoe": {
+            "expression": "evt.energy*evt.aoe"
         },
-        "is_usable_aoe": {
+        "energy_times_multiplicity": {
+            "expression": "evt.energy*evt.multiplicity"
+        },
+        "is_saturated": {
             "aggregation_mode": "keep_at_ch:evt.energy_id",
-            "expression": "True",
-            "initial": false
+            "expression": "hit.is_saturated"
         },
         "multiplicity": {
             "aggregation_mode": "sum",
             "channels": "geds_on",
+            "dtype": "int16",
             "expression": "hit.cuspEmax_ctc_cal > a",
             "initial": 0,
-            "lgdo_attrs": {
-                "statement": "0bb decay is real"
-            },
             "parameters": {
                 "a": 25
             }
+        },
+        "multiplicity_squared": {
+            "expression": "evt.multiplicity*evt.multiplicity"
+        },
+        "timestamp": {
+            "aggregation_mode": "sum",
+            "channels": "ts_master",
+            "expression": "dsp.timestamp",
+            "initial": 0.0
         }
     },
     "outputs": [
-        "multiplicity",
+        "timestamp",
         "energy",
+        "energy_sum",
         "energy_id",
         "energy_idx",
-        "energy_any_above1MeV",
-        "energy_all_above1MeV",
-        "energy_aux",
-        "energy_sum",
-        "is_usable_aoe",
         "aoe",
-        "is_aoe_rejected"
+        "aoe_idx",
+        "multiplicity",
+        "is_saturated",
+        "energy_times_aoe",
+        "energy_times_multiplicity",
+        "multiplicity_squared"
     ]
 }
```

### Comparing `pygama-1.6.0a2/tests/evt/configs/query-test-evt-config.json` & `pygama-2.0.0a1/tests/evt/configs/query-test-evt-config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.6.0a2/tests/evt/test_build_tcm.py` & `pygama-2.0.0a1/tests/evt/test_build_tcm.py`

 * *Files identical despite different names*

### Comparing `pygama-1.6.0a2/tests/flow/configs/filedb-config.json` & `pygama-2.0.0a1/tests/flow/configs/filedb-config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.6.0a2/tests/flow/conftest.py` & `pygama-2.0.0a1/tests/flow/conftest.py`

 * *Files identical despite different names*

### Comparing `pygama-1.6.0a2/tests/flow/test_data_loader.py` & `pygama-2.0.0a1/tests/flow/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `pygama-1.6.0a2/tests/flow/test_filedb.py` & `pygama-2.0.0a1/tests/flow/test_filedb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 from pathlib import Path
 
 import pytest
+from lgdo.lh5.exceptions import LH5EncodeError
 from pandas.testing import assert_frame_equal
 
 from pygama.flow import FileDB
 
 config_dir = Path(__file__).parent / "configs"
 
 
@@ -342,15 +343,15 @@
     ]
 
 
 def test_serialization(test_filedb_full, tmptestdir):
     db = test_filedb_full
     db.to_disk(f"{tmptestdir}/filedb.lh5", wo_mode="of")
 
-    with pytest.raises(RuntimeError):
+    with pytest.raises(LH5EncodeError):
         db.to_disk(f"{tmptestdir}/filedb.lh5")
 
     db2 = FileDB(f"{tmptestdir}/filedb.lh5")
     assert_frame_equal(db.df, db2.df)
 
 
 def test_get_table_columns(test_filedb_full):
```

### Comparing `pygama-1.6.0a2/tests/hit/configs/aggregations-hit-config.json` & `pygama-2.0.0a1/tests/hit/configs/aggregations-hit-config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.6.0a2/tests/hit/configs/spms-hit-a-config.json` & `pygama-2.0.0a1/tests/hit/configs/spms-hit-a-config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.6.0a2/tests/hit/test_build_hit.py` & `pygama-2.0.0a1/tests/hit/test_build_hit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import json
 import os
 from pathlib import Path
 
+import awkward as ak
 import numpy as np
 import pytest
 from lgdo import lh5
 
 from pygama.hit import build_hit
 from pygama.hit.build_hit import _reorder_table_operations
 
@@ -178,18 +180,27 @@
         "ch0/hit/trigger_pos",
     ]
 
 
 def test_build_hit_spms_multiconfig(dsp_test_file_spm, tmptestdir):
     out_file = f"{tmptestdir}/L200-comm-20211130-phy-spms_hit.lh5"
 
+    # append the tmptestdir to the start of paths in the spms-hit-multi-config.json
+    with open(f"{config_dir}/spms-hit-multi-config.json") as f:
+        configdict = json.load(f)
+    for key in configdict.keys():
+        configdict[key] = f"{config_dir}/" + configdict[key].split("/")[-1]
+    newdict = json.dumps(configdict)
+    with open(f"{tmptestdir}/spms-hit-multi-config.json", "w") as file:
+        file.write(newdict)
+
     build_hit(
         dsp_test_file_spm,
         outfile=out_file,
-        lh5_tables_config=f"{config_dir}/spms-hit-multi-config.json",
+        lh5_tables_config=f"{tmptestdir}/spms-hit-multi-config.json",
         wo_mode="overwrite",
     )
     assert lh5.ls(out_file) == ["ch0", "ch1", "ch2"]
     assert lh5.ls(out_file, "ch0/") == ["ch0/hit"]
     assert lh5.ls(out_file, "ch0/hit/") == [
         "ch0/hit/energy_in_pe",
         "ch0/hit/quality_cut",
@@ -222,7 +233,32 @@
     assert len(df0[0]) == 20
     assert len(df1[0]) == 20
     assert len(df2[0]) == 20
 
     assert np.nanmean(df0) == 0
     assert np.nanmean(df1) == 1
     assert np.nanmean(df2) == 2
+
+
+def test_vov_input(lgnd_test_data, tmptestdir):
+    infile = lgnd_test_data.get_path(
+        "lh5/l200-p03-r000-phy-20230312T055349Z-tier_psp.lh5"
+    )
+    outfile = f"{tmptestdir}/LDQTA_r117_20200110T105115Z_cal_geds_hit.lh5"
+
+    hit_config = {
+        "outputs": ["a"],
+        "operations": {
+            "a": {
+                "expression": "a + m * energies",
+                "parameters": {"a": 0, "m": 1},
+            }
+        },
+    }
+
+    build_hit(
+        infile, outfile=outfile, hit_config=hit_config, wo_mode="of", buffer_len=9999999
+    )
+
+    orig = lh5.read_as("ch1067205/dsp/energies", infile, "ak")
+    data = lh5.read_as("ch1067205/hit/a", outfile, "ak")
+    assert ak.all(data == orig)
```

### Comparing `pygama-1.6.0a2/tests/math/test_fwhm.py` & `pygama-2.0.0a1/tests/math/test_hpge_peak_fitting.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import numpy as np
 from pytest import approx
 
-import pygama.math.peak_fitting as pgf
+import pygama.math.hpge_peak_fitting as pgb
 
 
 def test_mostly_gauss_fwhm():
-    pars = [0, 1, 0, 0, 0.1, 0, 1]
+    # parameters need to be in order of n_sig, mu, sigma, htail, tau, n_bkg, hstep
+    pars = [1, 0, 1, 0, 0.1, 0, 0]
     cov = [
-        [1e-16, 0, 0, 0, 0, 0, 0],  # dmu2
-        [0, 1e-02, 0, 0, 0, 0, 0],  # dsig2
-        [0, 0, 1e-16, 0, 0, 0, 0],  # dhstep2
+        [1e-16, 0, 0, 0, 0, 0, 0],  # damp2
+        [0, 1e-16, 0, 0, 0, 0, 0],  # dmu2
+        [0, 0, 1e-02, 0, 0, 0, 0],  # dsig2
         [0, 0, 0, 1e-16, 0, 0, 0],  # dhtail2
         [0, 0, 0, 0, 1e-16, 0, 0],  # dtau2
         [0, 0, 0, 0, 0, 1e-16, 0],  # dbg02
-        [0, 0, 0, 0, 0, 0, 1e-16],
-    ]  # damp2
-    mu, sig, hstep, htail, tau, bg0, amp = pars
-    fwhm, dfwhm = pgf.radford_fwhm(sig, htail, tau, cov)
+        [0, 0, 0, 0, 0, 0, 1e-16],  # dhstep2
+    ]
+    amp, mu, sig, htail, tau, bg0, hstep = pars
+    fwhm, dfwhm = pgb.hpge_peak_fwhm(sig, htail, tau, cov)
     assert fwhm == approx(2.3548, rel=1e-5)
-    assert dfwhm == approx(2.3548e-8, rel=1e-5)
+    assert dfwhm == approx(2.3548e-1, rel=1e-5)
 
 
 def test_mostly_exp_fwhm():
-    pars = [0, 1e-6, 0, 1, 1, 0, 1]
+    # parameters need to be in order of n_sig, mu, sigma, htail, tau, n_bkg, hstep
+    pars = [1, 0, 1e-6, 1, 1, 0, 0]
     cov = [
-        [1e-16, 0, 0, 0, 0, 0, 0],  # dmu2
-        [0, 1e-16, 0, 0, 0, 0, 0],  # dsig2
-        [0, 0, 1e-16, 0, 0, 0, 0],  # dhstep2
+        [1e-16, 0, 0, 0, 0, 0, 0],  # damp2
+        [0, 1e-16, 0, 0, 0, 0, 0],  # dmu2
+        [0, 0, 1e-16, 0, 0, 0, 0],  # dsig2
         [0, 0, 0, 1e-16, 0, 0, 0],  # dhtail2
         [0, 0, 0, 0, 1e-02, 0, 0],  # dtau2
         [0, 0, 0, 0, 0, 1e-16, 0],  # dbg02
-        [0, 0, 0, 0, 0, 0, 1e-16],
-    ]  # damp2
-    mu, sig, hstep, htail, tau, bg0, amp = pars
-    fwhm, dfwhm = pgf.radford_fwhm(sig, htail, tau, cov)
+        [0, 0, 0, 0, 0, 0, 1e-16],  # dhs2
+    ]
+
+    amp, mu, sig, htail, tau, bg0, hstep = pars
+    fwhm, dfwhm = pgb.hpge_peak_fwhm(sig, htail, tau, cov)
     assert fwhm == approx(np.log(2), rel=1e-5)
     assert dfwhm == approx(np.log(2) / 10, rel=1e-5)
```

