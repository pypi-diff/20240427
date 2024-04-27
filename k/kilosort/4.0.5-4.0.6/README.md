# Comparing `tmp/kilosort-4.0.5.tar.gz` & `tmp/kilosort-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kilosort-4.0.5.tar", last modified: Fri Apr 19 18:45:04 2024, max compression
+gzip compressed data, was "kilosort-4.0.6.tar", last modified: Sat Apr 27 00:27:17 2024, max compression
```

## Comparing `kilosort-4.0.5.tar` & `kilosort-4.0.6.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:45:04.359928 kilosort-4.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:45:04.343928 kilosort-4.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:45:04.347928 kilosort-4.0.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-19 18:44:55.000000 kilosort-4.0.5/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-19 18:44:55.000000 kilosort-4.0.5/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-19 18:44:55.000000 kilosort-4.0.5/.github/ISSUE_TEMPLATE/installation_issue.yml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-19 18:44:55.000000 kilosort-4.0.5/.github/ISSUE_TEMPLATE/other.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:45:04.347928 kilosort-4.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-19 18:44:55.000000 kilosort-4.0.5/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-19 18:44:55.000000 kilosort-4.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-19 18:44:55.000000 kilosort-4.0.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-19 18:44:55.000000 kilosort-4.0.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-19 18:44:55.000000 kilosort-4.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10348 2024-04-19 18:45:04.359928 kilosort-4.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-04-19 18:44:55.000000 kilosort-4.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:45:04.347928 kilosort-4.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/drift.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/gui_guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/hardware.rst
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/multi_shank.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/parameters.rst
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:45:04.347928 kilosort-4.0.5/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     9953 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/tutorials/basic_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13669 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/tutorials/load_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/tutorials/make_probe.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/tutorials/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:45:04.351928 kilosort-4.0.5/kilosort/
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/CCG.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/bench.py
--rw-r--r--   0 runner    (1001) docker     (127)    14963 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/clustering_qr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/datashift.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:45:04.355928 kilosort-4.0.5/kilosort/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22103 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/data_view_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/header_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/launch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    19190 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/message_log_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/minor_gui_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/palettes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/probe_view_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/run_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/sanity_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    33239 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/settings_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/sorter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (127)    36575 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    13376 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20479 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/run_kilosort.py
--rw-r--r--   0 runner    (1001) docker     (127)    60034 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9251 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/spikedetect.py
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/swarmsplitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8345 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/template_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/wTEMP.npz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:45:04.359928 kilosort-4.0.5/kilosort.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10348 2024-04-19 18:45:04.000000 kilosort-4.0.5/kilosort.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-19 18:45:04.000000 kilosort-4.0.5/kilosort.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:45:04.000000 kilosort-4.0.5/kilosort.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-19 18:45:04.000000 kilosort-4.0.5/kilosort.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 18:45:04.000000 kilosort-4.0.5/kilosort.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-19 18:44:55.000000 kilosort-4.0.5/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 18:45:04.359928 kilosort-4.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-19 18:44:55.000000 kilosort-4.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:45:04.359928 kilosort-4.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-04-19 18:44:55.000000 kilosort-4.0.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-19 18:44:55.000000 kilosort-4.0.5/tests/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-19 18:44:55.000000 kilosort-4.0.5/tests/test_dtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-19 18:44:55.000000 kilosort-4.0.5/tests/test_full_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-19 18:44:55.000000 kilosort-4.0.5/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-19 18:44:55.000000 kilosort-4.0.5/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-19 18:44:55.000000 kilosort-4.0.5/tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-19 18:44:55.000000 kilosort-4.0.5/tests/test_spikedetect.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-19 18:44:55.000000 kilosort-4.0.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:17.183471 kilosort-4.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:17.167471 kilosort-4.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:17.171471 kilosort-4.0.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-27 00:27:08.000000 kilosort-4.0.6/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-27 00:27:08.000000 kilosort-4.0.6/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-27 00:27:08.000000 kilosort-4.0.6/.github/ISSUE_TEMPLATE/installation_issue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-27 00:27:08.000000 kilosort-4.0.6/.github/ISSUE_TEMPLATE/other.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:17.171471 kilosort-4.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-27 00:27:08.000000 kilosort-4.0.6/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-27 00:27:08.000000 kilosort-4.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-27 00:27:08.000000 kilosort-4.0.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-27 00:27:08.000000 kilosort-4.0.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 00:27:08.000000 kilosort-4.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10348 2024-04-27 00:27:17.183471 kilosort-4.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-04-27 00:27:08.000000 kilosort-4.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:17.171471 kilosort-4.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/drift.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/gui_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/hardware.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/multi_shank.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/parameters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:17.175471 kilosort-4.0.6/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     9953 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/tutorials/basic_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13669 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/tutorials/load_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/tutorials/make_probe.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/tutorials/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:17.175471 kilosort-4.0.6/kilosort/
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/CCG.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14963 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/clustering_qr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/datashift.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:17.179471 kilosort-4.0.6/kilosort/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22103 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/data_view_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/header_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21165 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/message_log_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/minor_gui_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/palettes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/probe_view_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/run_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/sanity_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33239 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/settings_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/sorter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36620 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13376 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20479 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/run_kilosort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60034 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/spikedetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/swarmsplitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8345 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/template_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/wTEMP.npz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:17.179471 kilosort-4.0.6/kilosort.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10348 2024-04-27 00:27:17.000000 kilosort-4.0.6/kilosort.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-27 00:27:17.000000 kilosort-4.0.6/kilosort.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 00:27:17.000000 kilosort-4.0.6/kilosort.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-27 00:27:17.000000 kilosort-4.0.6/kilosort.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-27 00:27:17.000000 kilosort-4.0.6/kilosort.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-27 00:27:08.000000 kilosort-4.0.6/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 00:27:17.183471 kilosort-4.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-27 00:27:08.000000 kilosort-4.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:17.179471 kilosort-4.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-04-27 00:27:08.000000 kilosort-4.0.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-27 00:27:08.000000 kilosort-4.0.6/tests/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-27 00:27:08.000000 kilosort-4.0.6/tests/test_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-27 00:27:08.000000 kilosort-4.0.6/tests/test_full_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-27 00:27:08.000000 kilosort-4.0.6/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-27 00:27:08.000000 kilosort-4.0.6/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-27 00:27:08.000000 kilosort-4.0.6/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-27 00:27:08.000000 kilosort-4.0.6/tests/test_spikedetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-27 00:27:08.000000 kilosort-4.0.6/tox.ini
```

### Comparing `kilosort-4.0.5/.github/ISSUE_TEMPLATE/bug_report.yml` & `kilosort-4.0.6/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/.github/ISSUE_TEMPLATE/feature_request.yml` & `kilosort-4.0.6/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/.github/ISSUE_TEMPLATE/installation_issue.yml` & `kilosort-4.0.6/.github/ISSUE_TEMPLATE/installation_issue.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/.github/workflows/test_and_deploy.yml` & `kilosort-4.0.6/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/.gitignore` & `kilosort-4.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/.readthedocs.yml` & `kilosort-4.0.6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/CODE_OF_CONDUCT.md` & `kilosort-4.0.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/LICENSE` & `kilosort-4.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/PKG-INFO` & `kilosort-4.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kilosort
-Version: 4.0.5
+Version: 4.0.6
 Summary: spike sorting pipeline
 Home-page: https://github.com/MouseLand/kilosort
 Author: Marius Pachitariu
 Author-email: pachitarium@janelia.hhmi.org
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `kilosort-4.0.5/README.md` & `kilosort-4.0.6/README.md`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/docs/Makefile` & `kilosort-4.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/docs/conf.py` & `kilosort-4.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/docs/drift.rst` & `kilosort-4.0.6/docs/drift.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/docs/gui_guide.rst` & `kilosort-4.0.6/docs/gui_guide.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/docs/hardware.rst` & `kilosort-4.0.6/docs/hardware.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/docs/index.rst` & `kilosort-4.0.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/docs/make.bat` & `kilosort-4.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/docs/multi_shank.rst` & `kilosort-4.0.6/docs/multi_shank.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/docs/parameters.rst` & `kilosort-4.0.6/docs/parameters.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/docs/tutorials/basic_example.ipynb` & `kilosort-4.0.6/docs/tutorials/basic_example.ipynb`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/docs/tutorials/load_data.ipynb` & `kilosort-4.0.6/docs/tutorials/load_data.ipynb`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/docs/tutorials/make_probe.ipynb` & `kilosort-4.0.6/docs/tutorials/make_probe.ipynb`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/CCG.py` & `kilosort-4.0.6/kilosort/CCG.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/bench.py` & `kilosort-4.0.6/kilosort/bench.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/clustering_qr.py` & `kilosort-4.0.6/kilosort/clustering_qr.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/datashift.py` & `kilosort-4.0.6/kilosort/datashift.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/gui/__init__.py` & `kilosort-4.0.6/kilosort/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/gui/converter.py` & `kilosort-4.0.6/kilosort/gui/converter.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/gui/data_view_box.py` & `kilosort-4.0.6/kilosort/gui/data_view_box.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/gui/header_box.py` & `kilosort-4.0.6/kilosort/gui/header_box.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/gui/launch.py` & `kilosort-4.0.6/kilosort/gui/launch.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/gui/logger.py` & `kilosort-4.0.6/kilosort/gui/logger.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/gui/main.py` & `kilosort-4.0.6/kilosort/gui/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,24 +81,25 @@
 
         self.num_channels = None
         self.context = None
         self.file_object = None
 
         self.content = QtWidgets.QWidget(self)
         self.content_layout = QtWidgets.QVBoxLayout()
+        self.left_boxes = QtWidgets.QWidget()
+        self.left_boxes_layout = QtWidgets.QVBoxLayout(self.left_boxes)
+        self.right_boxes = QtWidgets.QWidget()
+        self.right_boxes_layout = QtWidgets.QVBoxLayout(self.right_boxes)
+        self.left_right_splitter = QtWidgets.QSplitter(QtCore.Qt.Horizontal)
+        self.settings_probe_splitter = QtWidgets.QSplitter(QtCore.Qt.Horizontal)
+        self.settings_message_splitter = QtWidgets.QSplitter(QtCore.Qt.Vertical)
+        self.settings_area = QtWidgets.QWidget()
+        self.settings_layout = QtWidgets.QVBoxLayout(self.settings_area)
 
         self.header_box = HeaderBox(self)
-
-        self.boxes = QtWidgets.QWidget()
-        self.boxes_layout = QtWidgets.QHBoxLayout(self.boxes)
-        self.first_boxes_layout = QtWidgets.QVBoxLayout()
-        self.second_boxes_layout = QtWidgets.QHBoxLayout()
-        self.third_boxes_layout = QtWidgets.QVBoxLayout()
-        self.fourth_boxes_layout = QtWidgets.QVBoxLayout()
-
         self.converter = DataConversionBox(self)
         self.settings_box = SettingsBox(self)
         self.probe_view_box = ProbeViewBox(self)
         self.data_view_box = DataViewBox(self)
         self.run_box = RunBox(self)
         self.message_log_box = MessageLogBox(self)
 
@@ -198,38 +199,51 @@
         #     if response == QtWidgets.QMessageBox.Yes:
         #         self.settings_box.set_data_file_path_from_drag_and_drop(filename)
 
 
     def setup(self):
         self.setWindowTitle(f"Kilosort4")
 
-        self.third_boxes_layout.addWidget(self.settings_box, 85)
-        self.third_boxes_layout.addWidget(self.run_box, 15)
-
-        self.second_boxes_layout.addLayout(self.third_boxes_layout, 50)
-        self.second_boxes_layout.addWidget(self.probe_view_box, 50)
-
-        self.first_boxes_layout.addLayout(self.second_boxes_layout, 60)
-        self.first_boxes_layout.addWidget(self.message_log_box, 40)
-
-        self.fourth_boxes_layout.addWidget(self.header_box, 3)
-        self.fourth_boxes_layout.addWidget(self.data_view_box, 97)
-
-        self.boxes_layout.addLayout(self.first_boxes_layout, 25)
-        self.boxes_layout.addLayout(self.fourth_boxes_layout, 75)
-
-        self.boxes.setLayout(self.boxes_layout)
-        self.content_layout.addWidget(self.boxes, 90)
+        # Set Wiget positions
+        # Top left, settings plus "load" and "run" buttons.
+        self.settings_layout.addWidget(self.settings_box, 85)
+        self.settings_layout.addWidget(self.run_box, 15)
+        # To right of settings, add probe view
+        self.settings_probe_splitter.addWidget(self.settings_area)
+        self.settings_probe_splitter.addWidget(self.probe_view_box)
+        # Below settings & probe, add message box
+        self.settings_message_splitter.addWidget(self.settings_probe_splitter)
+        self.settings_message_splitter.addWidget(self.message_log_box)
+        self.left_boxes_layout.addWidget(self.settings_message_splitter)
+        # Right-hand side, header plus data view
+        self.right_boxes_layout.addWidget(self.header_box, 3)
+        self.right_boxes_layout.addWidget(self.data_view_box, 97)
+        # Nest left and right within vertical splitter
+        self.left_right_splitter.addWidget(self.left_boxes)
+        self.left_right_splitter.addWidget(self.right_boxes)
 
+        self.content_layout.addWidget(self.left_right_splitter, 90)
         self.content_layout.setContentsMargins(10, 10, 10, 10)
         self.content.setLayout(self.content_layout)
         self.setCentralWidget(self.content)
 
-        self.header_box.reset_gui_button.clicked.connect(self.reset_gui)
+        # Restore splitter positions if saved from previous session
+        if self.qt_settings.contains('settings_probe_splitter'):
+            self.settings_probe_splitter.restoreState(
+                self.qt_settings.value('settings_probe_splitter')
+                )
+            self.settings_message_splitter.restoreState(
+                self.qt_settings.value('settings_message_splitter')
+                )
+            self.left_right_splitter.restoreState(
+                self.qt_settings.value('left_right_splitter')
+                )
 
+        # Connect signals
+        self.header_box.reset_gui_button.clicked.connect(self.reset_gui)
         self.settings_box.settingsUpdated.connect(self.load_data)
         self.settings_box.previewProbe.connect(self.probe_view_box.preview_probe)
         # Don't allow spike sorting to run until new data has actually
         # been loaded.
         self.settings_box.dataChanged.connect(self.disable_run)
 
         self.data_view_box.channelChanged.connect(self.probe_view_box.update_probe_view)
@@ -242,14 +256,28 @@
         self.run_box.disableInput.connect(self.disable_all_input)
         self.run_box.sortingStepStatusUpdate.connect(self.update_sorting_status)
         self.run_box.setupContextForRun.connect(self.setup_context_for_run)
 
         self.converter.disableInput.connect(self.disable_all_input)
         self.converter.fileObjectLoaded.connect(self.add_file_object)
 
+        self.settings_probe_splitter.splitterMoved.connect(self.save_widget_sizes)
+        self.settings_message_splitter.splitterMoved.connect(self.save_widget_sizes)
+        self.left_right_splitter.splitterMoved.connect(self.save_widget_sizes)
+
+    @QtCore.Slot()
+    def save_widget_sizes(self):
+        # Store splitter positions so that resizing persists between sessions.
+        state1 = self.settings_probe_splitter.saveState()
+        self.qt_settings.setValue('settings_probe_splitter', state1)
+        state2 = self.settings_message_splitter.saveState()
+        self.qt_settings.setValue('settings_message_splitter', state2)
+        state3 = self.left_right_splitter.saveState()
+        self.qt_settings.setValue('left_right_splitter', state3)
+
     def change_channel_display(self, direction):
         if self.context is not None:
             self.data_view_box.shift_primary_channel(direction)
 
     def shift_data(self, time_shift):
         if self.context is not None:
             self.data_view_box.shift_current_time(time_shift)
@@ -501,22 +529,24 @@
         self.close_binary_files()
         self.probe_view_box.reset()
         self.data_view_box.reset()
         self.settings_box.reset()
         self.message_log_box.reset()
 
     def closeEvent(self, event: QtGui.QCloseEvent):
+        # Make sure all threads and pop-out windows are closed as well.
         self.message_log_box.save_log_file()
         self.message_log_box.popout_window.close()
         for _, p in self.run_box.plots.items():
             p.close()
         self.run_box.current_worker.terminate()
         if self.converter.conversion_thread is not None:
             self.converter.conversion_thread.terminate()
         self.close_binary_files()
+
         event.accept()
 
 
 class Context(dict):
     """
     Borrowed from:
     https://stackoverflow.com/questions/2352181/how-to-use-a-dot-to-access-members-of-dictionary/32107024#32107024
```

### Comparing `kilosort-4.0.5/kilosort/gui/message_log_box.py` & `kilosort-4.0.6/kilosort/gui/message_log_box.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pathlib import Path
 import pprint
 
+import numpy as np
 from kilosort.gui.logger import XStream
 from qtpy import QtCore, QtGui, QtWidgets
 
 
 class MessageLogBox(QtWidgets.QGroupBox):
     def __init__(self, parent):
         QtWidgets.QGroupBox.__init__(self, parent=parent)
@@ -19,21 +20,21 @@
         self.layout.addWidget(self.log_box, 0, 0, 1, 3)
 
         self.popout_button = QtWidgets.QPushButton('Show More')
         self.popout_button.clicked.connect(self.show_log_popout)
         self.layout.addWidget(self.popout_button, 1, 0, 1, 1)
         self.popout_window = ExpandedLog()
 
-        self.dump_settings_button = QtWidgets.QPushButton('Dump Settings')
-        self.dump_settings_button.clicked.connect(self.dump_settings)
-        self.layout.addWidget(self.dump_settings_button, 1, 1, 1, 1)
-
-        self.dump_probe_button = QtWidgets.QPushButton('Dump Probe')
-        self.dump_probe_button.clicked.connect(self.dump_probe)
-        self.layout.addWidget(self.dump_probe_button, 1, 2, 1, 1)
+        self.print_settings_button = QtWidgets.QPushButton('Print Settings')
+        self.print_settings_button.clicked.connect(self.print_settings)
+        self.layout.addWidget(self.print_settings_button, 1, 1, 1, 1)
+
+        self.print_probe_button = QtWidgets.QPushButton('Print Probe')
+        self.print_probe_button.clicked.connect(self.print_probe)
+        self.layout.addWidget(self.print_probe_button, 1, 2, 1, 1)
 
         log_box_document = self.log_box.document()
         default_font = log_box_document.defaultFont()
         default_font.setPointSize(8)
         log_box_document.setDefaultFont(default_font)
 
         XStream.stdout().messageWritten.connect(self.update_text)
@@ -48,36 +49,44 @@
         self.popout_window.update_text(text)
 
     @QtCore.Slot()
     def show_log_popout(self):
         self.popout_window.show()
 
     @QtCore.Slot()
-    def dump_settings(self):
+    def print_settings(self):
         # For debugging purposes, check for mismatch between displayed parameter
         # values and the values that are actually being used.
         settings_text = "settings = "
         settings = self.gui.settings_box.settings.copy()
         settings['probe'] = '... (use dump probe)'
         s = pprint.pformat(settings, indent=4, sort_dicts=False)
         settings_text += s[0] + '\n ' + s[1:-1] + '\n' + s[-1]
 
         self.update_text(settings_text)
 
     @QtCore.Slot()
-    def dump_probe(self):
+    def print_probe(self):
         # For debugging purposes, make sure probe is loaded correctly.
         probe_text = "probe = "
         probe = self.gui.settings_box.settings['probe']
+        
+        # Set numpy to print full arrays
+        opt = np.get_printoptions()
+        np.set_printoptions(threshold=np.inf)
+        
         p = pprint.pformat(probe, indent=4, sort_dicts=False)
         # insert `np.` so that text can be copied directly to code
         p = 'np.array'.join(p.split('array'))
         p = 'dtype=np.'.join(p.split('dtype='))
         probe_text += p[0] + '\n ' + p[1:-1] + '\n' + p[-1]
 
+        # Revert numpy settings
+        np.set_printoptions(**opt)
+
         self.update_text(probe_text)
 
     def prepare_for_new_context(self):
         self.save_log_file()
         self.log_box.clear()
 
     def save_log_file(self):
```

### Comparing `kilosort-4.0.5/kilosort/gui/minor_gui_elements.py` & `kilosort-4.0.6/kilosort/gui/minor_gui_elements.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/gui/palettes.py` & `kilosort-4.0.6/kilosort/gui/palettes.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/gui/probe_view_box.py` & `kilosort-4.0.6/kilosort/gui/probe_view_box.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/gui/run_box.py` & `kilosort-4.0.6/kilosort/gui/run_box.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/gui/sanity_plots.py` & `kilosort-4.0.6/kilosort/gui/sanity_plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     t = np.arange(wPCA.shape[1])/(settings['fs']/1000)
     for i in range(wPCA.shape[0]):
         color = _COLOR_CODES[i % len(_COLOR_CODES)]
         p1.plot(t, wPCA[i,:], pen=color)
 
     # Spatial features (top right)
     p2 = plot_window.plot_widget.addPlot(
-        row=0, col=1, labels={'bottom': 'Unit Number', 'left': 'Channel Number'}
+        row=0, col=1, labels={'bottom': 'Channel Number', 'left': 'Unit Number'}
         )
     p2.setTitle('Spatial Features')
     features = torch.linalg.norm(Wall0, dim=2).cpu().numpy()
     img = pg.ImageItem(image=features.T)
     img.setLevels([0, 25])
     p2.addItem(img)
```

### Comparing `kilosort-4.0.5/kilosort/gui/settings_box.py` & `kilosort-4.0.6/kilosort/gui/settings_box.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/gui/sorter.py` & `kilosort-4.0.6/kilosort/gui/sorter.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/hierarchical.py` & `kilosort-4.0.6/kilosort/hierarchical.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/io.py` & `kilosort-4.0.6/kilosort/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,15 +545,16 @@
     bytes_per_value = np.dtype(dtype).itemsize
     bytes_per_sample = np.int64(bytes_per_value * n_channels)
     total_bytes = os.path.getsize(filename)
     samples = (total_bytes / bytes_per_sample)
 
     if samples%1 != 0:
         raise ValueError(
-            "Bytes in binary file did not divide evenly, incorrect n_chan_bin."
+            "Bytes in binary file did not divide evenly, "
+            "incorrect n_chan_bin ('number of channels' in GUI)."
         )
     else:
         return int(samples)
 
 
 class BinaryFileGroup:
     def __init__(self, file_objects):
```

### Comparing `kilosort-4.0.5/kilosort/parameters.py` & `kilosort-4.0.6/kilosort/parameters.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/postprocessing.py` & `kilosort-4.0.6/kilosort/postprocessing.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/preprocessing.py` & `kilosort-4.0.6/kilosort/preprocessing.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/run_kilosort.py` & `kilosort-4.0.6/kilosort/run_kilosort.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/simulation.py` & `kilosort-4.0.6/kilosort/simulation.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/spikedetect.py` & `kilosort-4.0.6/kilosort/spikedetect.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                              ops['yc'].min(), ops['yc'].max()
 
     dmin = ops['settings']['dmin']
     if dmin is None:
         # Try to determine a good value automatically based on contact positions.
         dmin = np.median(np.diff(np.unique(ops['yc'])))
     ops['dmin'] = dmin
-    ops['yup'] = np.arange(ymin, ymax+.00001, dmin//2)
+    ops['yup'] = np.arange(ymin, ymax+.00001, dmin/2)
 
     ops['dminx'] = dminx = ops['settings']['dminx']
     nx = np.round((xmax - xmin) / (dminx/2)) + 1
     ops['xup'] = np.linspace(xmin, xmax, int(nx))
 
     # Set max channel distance based on dmin, dminx, use whichever is greater.
     if ops.get('max_channel_distance', None) is None:
@@ -218,26 +218,14 @@
 
     ds_torch = torch.from_numpy(ds).to(device).float()
     template_sizes = sig * (1+torch.arange(nsizes, device=device))
     weigh = torch.exp(-ds_torch.unsqueeze(-1) / template_sizes**2)
     weigh = torch.permute(weigh, (2, 0, 1)).contiguous()
     weigh = weigh / (weigh**2).sum(1).unsqueeze(1)**.5
 
-    nan_weights = torch.isnan(weigh)
-    zero_weights = (weigh == 0)
-    if (nan_weights.sum() > 0) or (zero_weights.sum() > 0):
-        msg = """
-              NaNs and/or zeroes present in weights for spikedetect.run,
-              may need to adjust `min_template_size` and/or `dminx` 
-              for best results.\n
-              If you're using a probe with multiple shanks, see 
-              https://kilosort.readthedocs.io/en/latest/multi_shank.html
-              """
-        warnings.warn(msg, UserWarning)
-
     st = np.zeros((10**6, 6), 'float64')
     tF = np.zeros((10**6, nC , ops['settings']['n_pcs']), 'float32')
 
     k = 0
     nt = ops['nt']
     tarange = torch.arange(-(nt//2),nt//2+1, device = device)
     s = StringIO()
```

### Comparing `kilosort-4.0.5/kilosort/swarmsplitter.py` & `kilosort-4.0.6/kilosort/swarmsplitter.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/template_matching.py` & `kilosort-4.0.6/kilosort/template_matching.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/utils.py` & `kilosort-4.0.6/kilosort/utils.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort/wTEMP.npz` & `kilosort-4.0.6/kilosort/wTEMP.npz`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/kilosort.egg-info/PKG-INFO` & `kilosort-4.0.6/kilosort.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kilosort
-Version: 4.0.5
+Version: 4.0.6
 Summary: spike sorting pipeline
 Home-page: https://github.com/MouseLand/kilosort
 Author: Marius Pachitariu
 Author-email: pachitarium@janelia.hhmi.org
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `kilosort-4.0.5/kilosort.egg-info/SOURCES.txt` & `kilosort-4.0.6/kilosort.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/setup.py` & `kilosort-4.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/tests/conftest.py` & `kilosort-4.0.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/tests/test_clustering.py` & `kilosort-4.0.6/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/tests/test_dtype.py` & `kilosort-4.0.6/tests/test_dtype.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/tests/test_full_pipeline.py` & `kilosort-4.0.6/tests/test_full_pipeline.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/tests/test_io.py` & `kilosort-4.0.6/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/tests/test_parameters.py` & `kilosort-4.0.6/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/tests/test_preprocessing.py` & `kilosort-4.0.6/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.5/tox.ini` & `kilosort-4.0.6/tox.ini`

 * *Files identical despite different names*

