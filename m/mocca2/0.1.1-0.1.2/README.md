# Comparing `tmp/mocca2-0.1.1.tar.gz` & `tmp/mocca2-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mocca2-0.1.1.tar", last modified: Wed Apr 10 23:06:00 2024, max compression
+gzip compressed data, was "mocca2-0.1.2.tar", last modified: Sat Apr 27 04:07:59 2024, max compression
```

## Comparing `mocca2-0.1.1.tar` & `mocca2-0.1.2.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:06:00.333606 mocca2-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-10 23:05:51.000000 mocca2-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-10 23:06:00.333606 mocca2-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-10 23:05:51.000000 mocca2-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-10 23:05:51.000000 mocca2-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 23:06:00.333606 mocca2-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:06:00.321606 mocca2-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:06:00.325606 mocca2-0.1.1/src/mocca2/
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:06:00.325606 mocca2-0.1.1/src/mocca2/baseline/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/baseline/arpls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/baseline/asls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/baseline/flatfit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/baseline/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:06:00.325606 mocca2-0.1.1/src/mocca2/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/classes/chromatogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/classes/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/classes/compound.py
--rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/classes/data2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/classes/deconvolved_peak.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/classes/peak.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:06:00.329606 mocca2-0.1.1/src/mocca2/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/clustering/cluster_components.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:06:00.329606 mocca2-0.1.1/src/mocca2/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24559 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/dataset/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:06:00.329606 mocca2-0.1.1/src/mocca2/deconvolution/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/deconvolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/deconvolution/alternating_lstsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/deconvolution/deconvolve.py
--rw-r--r--   0 runner    (1001) docker     (127)     9640 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/deconvolution/fit_peak_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/deconvolution/guess_spectra.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/deconvolution/nnls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/deconvolution/nonnegative_lstsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     9822 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/deconvolution/peak_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:06:00.329606 mocca2-0.1.1/src/mocca2/example_data/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-10 23:05:51.000000 mocca2-0.1.1/src/mocca2/example_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14331 2024-04-10 23:05:56.000000 mocca2-0.1.1/src/mocca2/example_data/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-10 23:05:56.000000 mocca2-0.1.1/src/mocca2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-10 23:05:56.000000 mocca2-0.1.1/src/mocca2/math.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:06:00.329606 mocca2-0.1.1/src/mocca2/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-10 23:05:56.000000 mocca2-0.1.1/src/mocca2/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-10 23:05:56.000000 mocca2-0.1.1/src/mocca2/parsers/chemstation.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-10 23:05:56.000000 mocca2-0.1.1/src/mocca2/parsers/empower.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-10 23:05:56.000000 mocca2-0.1.1/src/mocca2/parsers/labsolutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-10 23:05:56.000000 mocca2-0.1.1/src/mocca2/parsers/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:06:00.329606 mocca2-0.1.1/src/mocca2/peaks/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-10 23:05:56.000000 mocca2-0.1.1/src/mocca2/peaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-10 23:05:56.000000 mocca2-0.1.1/src/mocca2/peaks/find_peaks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-10 23:05:56.000000 mocca2-0.1.1/src/mocca2/peaks/merge_overlapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-10 23:05:56.000000 mocca2-0.1.1/src/mocca2/peaks/split.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 23:05:56.000000 mocca2-0.1.1/src/mocca2/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:06:00.333606 mocca2-0.1.1/src/mocca2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-10 23:06:00.000000 mocca2-0.1.1/src/mocca2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-10 23:06:00.000000 mocca2-0.1.1/src/mocca2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:06:00.000000 mocca2-0.1.1/src/mocca2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-10 23:06:00.000000 mocca2-0.1.1/src/mocca2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 23:06:00.000000 mocca2-0.1.1/src/mocca2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:06:00.329606 mocca2-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-10 23:05:56.000000 mocca2-0.1.1/tests/test_example_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-10 23:05:56.000000 mocca2-0.1.1/tests/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:07:59.214523 mocca2-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-27 04:07:44.000000 mocca2-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-27 04:07:59.214523 mocca2-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-27 04:07:44.000000 mocca2-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-27 04:07:44.000000 mocca2-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 04:07:59.214523 mocca2-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:07:59.202523 mocca2-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:07:59.206523 mocca2-0.1.2/src/mocca2/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:07:59.206523 mocca2-0.1.2/src/mocca2/baseline/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/baseline/arpls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/baseline/asls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/baseline/flatfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/baseline/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:07:59.210523 mocca2-0.1.2/src/mocca2/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18539 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/classes/chromatogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/classes/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/classes/compound.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/classes/data2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/classes/deconvolved_peak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/classes/peak.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:07:59.210523 mocca2-0.1.2/src/mocca2/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/clustering/cluster_components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:07:59.210523 mocca2-0.1.2/src/mocca2/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25062 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/dataset/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:07:59.210523 mocca2-0.1.2/src/mocca2/deconvolution/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/deconvolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/deconvolution/alternating_lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/deconvolution/deconvolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9640 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/deconvolution/fit_peak_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/deconvolution/guess_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/deconvolution/nnls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/deconvolution/nonnegative_lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9822 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/deconvolution/peak_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:07:59.214523 mocca2-0.1.2/src/mocca2/example_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-27 04:07:44.000000 mocca2-0.1.2/src/mocca2/example_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14331 2024-04-27 04:07:49.000000 mocca2-0.1.2/src/mocca2/example_data/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-27 04:07:49.000000 mocca2-0.1.2/src/mocca2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-27 04:07:49.000000 mocca2-0.1.2/src/mocca2/math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:07:59.214523 mocca2-0.1.2/src/mocca2/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-27 04:07:49.000000 mocca2-0.1.2/src/mocca2/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-27 04:07:49.000000 mocca2-0.1.2/src/mocca2/parsers/chemstation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-27 04:07:49.000000 mocca2-0.1.2/src/mocca2/parsers/empower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-27 04:07:49.000000 mocca2-0.1.2/src/mocca2/parsers/labsolutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-27 04:07:49.000000 mocca2-0.1.2/src/mocca2/parsers/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:07:59.214523 mocca2-0.1.2/src/mocca2/peaks/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-27 04:07:49.000000 mocca2-0.1.2/src/mocca2/peaks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-27 04:07:49.000000 mocca2-0.1.2/src/mocca2/peaks/find_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-27 04:07:49.000000 mocca2-0.1.2/src/mocca2/peaks/merge_overlapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-27 04:07:49.000000 mocca2-0.1.2/src/mocca2/peaks/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 04:07:49.000000 mocca2-0.1.2/src/mocca2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-27 04:07:49.000000 mocca2-0.1.2/src/mocca2/serializing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:07:59.214523 mocca2-0.1.2/src/mocca2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-27 04:07:59.000000 mocca2-0.1.2/src/mocca2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-27 04:07:59.000000 mocca2-0.1.2/src/mocca2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 04:07:59.000000 mocca2-0.1.2/src/mocca2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-27 04:07:59.000000 mocca2-0.1.2/src/mocca2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-27 04:07:59.000000 mocca2-0.1.2/src/mocca2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:07:59.214523 mocca2-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-27 04:07:49.000000 mocca2-0.1.2/tests/test_example_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-27 04:07:49.000000 mocca2-0.1.2/tests/test_serialization.py
```

### Comparing `mocca2-0.1.1/LICENSE.txt` & `mocca2-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/PKG-INFO` & `mocca2-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mocca2
-Version: 0.1.1
+Version: 0.1.2
 Summary: MOCCA2 is an open-source Python project to analyze HPLC-DAD raw data
 Author-email: Jan Oboril <jan.oboril@gmail.com>
 Project-URL: Homepage, https://oboril.github.io/mocca/
-Project-URL: Issues, https://github.com/oboril/mocca/issues
+Project-URL: Issues, https://github.com/oboril/MOCCA/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy>1.20
@@ -16,17 +16,17 @@
 Requires-Dist: scikit-learn>1.3
 Requires-Dist: pyyaml>6.0
 Requires-Dist: pandas>2.1
 Requires-Dist: matplotlib>3.6
 Requires-Dist: pyarrow>15.0
 
 [![PyPI](https://img.shields.io/pypi/v/mocca2.svg)](https://pypi.org/project/mocca2/)
-![pytest](https://github.com/oboril/mocca/actions/workflows/ci.yaml/badge.svg)
-[![Docs Pages](https://github.com/oboril/mocca/actions/workflows/deploy_pages.yaml/badge.svg)](https://oboril.github.io/mocca/)
-[![Example Data](https://github.com/oboril/mocca/actions/workflows/package_data.yaml/badge.svg)](https://github.com/oboril/mocca/tree/example-data)
+![pytest](https://github.com/oboril/MOCCA/actions/workflows/ci.yaml/badge.svg)
+[![Docs Pages](https://github.com/oboril/MOCCA/actions/workflows/deploy_pages.yaml/badge.svg)](https://oboril.github.io/mocca/)
+[![Example Data](https://github.com/oboril/MOCCA/actions/workflows/package_data.yaml/badge.svg)](https://github.com/oboril/MOCCA/tree/example-data)
 
 # Welcome to MOCCA2
 
 MOCCA2 is a Python package for automatic processing of HPLC chromatograms.
 
 To automate your workflow and get accurate results, MOCCA2 features:
  - support for raw data files from Agilent, Shimadzu and Waters
@@ -35,15 +35,15 @@
  - automatic purity checking and peak deconvolution
  - compound tracking across chromatograms
  - fully automatic processing of any number of chromatograms
 
 
 ## Documentation
 
-Examples and detailed documentation are documented at [https://oboril.github.io/mocca](https://oboril.github.io/mocca).
+Examples and detailed documentation are documented at [https://oboril.github.io/MOCCA](https://oboril.github.io/MOCCA).
 
 ## Getting Started
 
 The latest version of MOCCA2 can be installed simply using pip:
 
 ```
 pip install mocca2
@@ -116,12 +116,12 @@
  - and various standalone chromatograms
 
 Since these datasets don't fit into the PyPI package size limit, they are automatically compressed and published onto `example-data` branch on push to `main`. 
 
 The data can be automatically downloaded using ``python -m mocca2 --download-data``.
 
 ### Publishing to PyPI and GitHub
-On push to `main`, the MOCCA2 package is automatically published to [PyPI](https://pypi.org/project/mocca2/) and [GitHub Releases](https://github.com/oboril/mocca/releases).
+On push to `main`, the MOCCA2 package is automatically published to [PyPI](https://pypi.org/project/mocca2/) and [GitHub Releases](https://github.com/oboril/MOCCA/releases).
 
 ## Contributing
 
-The process for contributing is outlined in [CONTRIBUTING.md](https://github.com/oboril/mocca/blob/main/CONTRIBUTING.md).
+The process for contributing is outlined in [CONTRIBUTING.md](https://github.com/oboril/MOCCA/blob/main/CONTRIBUTING.md).
```

### Comparing `mocca2-0.1.1/README.md` & `mocca2-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [![PyPI](https://img.shields.io/pypi/v/mocca2.svg)](https://pypi.org/project/mocca2/)
-![pytest](https://github.com/oboril/mocca/actions/workflows/ci.yaml/badge.svg)
-[![Docs Pages](https://github.com/oboril/mocca/actions/workflows/deploy_pages.yaml/badge.svg)](https://oboril.github.io/mocca/)
-[![Example Data](https://github.com/oboril/mocca/actions/workflows/package_data.yaml/badge.svg)](https://github.com/oboril/mocca/tree/example-data)
+![pytest](https://github.com/oboril/MOCCA/actions/workflows/ci.yaml/badge.svg)
+[![Docs Pages](https://github.com/oboril/MOCCA/actions/workflows/deploy_pages.yaml/badge.svg)](https://oboril.github.io/mocca/)
+[![Example Data](https://github.com/oboril/MOCCA/actions/workflows/package_data.yaml/badge.svg)](https://github.com/oboril/MOCCA/tree/example-data)
 
 # Welcome to MOCCA2
 
 MOCCA2 is a Python package for automatic processing of HPLC chromatograms.
 
 To automate your workflow and get accurate results, MOCCA2 features:
  - support for raw data files from Agilent, Shimadzu and Waters
@@ -14,15 +14,15 @@
  - automatic purity checking and peak deconvolution
  - compound tracking across chromatograms
  - fully automatic processing of any number of chromatograms
 
 
 ## Documentation
 
-Examples and detailed documentation are documented at [https://oboril.github.io/mocca](https://oboril.github.io/mocca).
+Examples and detailed documentation are documented at [https://oboril.github.io/MOCCA](https://oboril.github.io/MOCCA).
 
 ## Getting Started
 
 The latest version of MOCCA2 can be installed simply using pip:
 
 ```
 pip install mocca2
@@ -95,12 +95,12 @@
  - and various standalone chromatograms
 
 Since these datasets don't fit into the PyPI package size limit, they are automatically compressed and published onto `example-data` branch on push to `main`. 
 
 The data can be automatically downloaded using ``python -m mocca2 --download-data``.
 
 ### Publishing to PyPI and GitHub
-On push to `main`, the MOCCA2 package is automatically published to [PyPI](https://pypi.org/project/mocca2/) and [GitHub Releases](https://github.com/oboril/mocca/releases).
+On push to `main`, the MOCCA2 package is automatically published to [PyPI](https://pypi.org/project/mocca2/) and [GitHub Releases](https://github.com/oboril/MOCCA/releases).
 
 ## Contributing
 
-The process for contributing is outlined in [CONTRIBUTING.md](https://github.com/oboril/mocca/blob/main/CONTRIBUTING.md).
+The process for contributing is outlined in [CONTRIBUTING.md](https://github.com/oboril/MOCCA/blob/main/CONTRIBUTING.md).
```

### Comparing `mocca2-0.1.1/pyproject.toml` & `mocca2-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mocca2"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Jan Oboril", email="jan.oboril@gmail.com" },
 ]
 description = "MOCCA2 is an open-source Python project to analyze HPLC-DAD raw data"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -24,8 +24,8 @@
   'pandas > 2.1',
   'matplotlib > 3.6',
   'pyarrow > 15.0'
 ]
 
 [project.urls]
 Homepage = "https://oboril.github.io/mocca/"
-Issues = "https://github.com/oboril/mocca/issues"
+Issues = "https://github.com/oboril/MOCCA/issues"
```

### Comparing `mocca2-0.1.1/src/mocca2/__init__.py` & `mocca2-0.1.2/src/mocca2/__init__.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/src/mocca2/__main__.py` & `mocca2-0.1.2/src/mocca2/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     directory = impresources.files(example_data).joinpath("data")
     if directory.exists():
         raise ValueError("Data has been already downloaded.")
     directory.mkdir()
 
     for file in files:
-        url = f"https://github.com/oboril/mocca/raw/example-data/{file}.tar.bz2"
+        url = f"https://github.com/oboril/MOCCA/raw/example-data/{file}.tar.bz2"
         filename = directory.joinpath(f"{file}.tar.bz2")
 
         print(f"Downloading {file} data to {filename}")
         download_file(url, filename)
         print(f"Extracting {file} data")
         extract_bz2(filename, directory)
```

### Comparing `mocca2-0.1.1/src/mocca2/baseline/arpls.py` & `mocca2-0.1.2/src/mocca2/baseline/arpls.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/src/mocca2/baseline/asls.py` & `mocca2-0.1.2/src/mocca2/baseline/asls.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/src/mocca2/baseline/flatfit.py` & `mocca2-0.1.2/src/mocca2/baseline/flatfit.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/src/mocca2/baseline/wrapper.py` & `mocca2-0.1.2/src/mocca2/baseline/wrapper.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/src/mocca2/classes/chromatogram.py` & `mocca2-0.1.2/src/mocca2/classes/chromatogram.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from mocca2.deconvolution.peak_models import (
     PeakModel,
     Bemg,
     FraserSuzuki,
     BiGaussian,
     BiGaussianTailing,
 )
+from mocca2.serializing import dict_encoder
 
 
 class Chromatogram(Data2D):
     """Information about single chromatogram, based on Data2D"""
 
     peaks: List[Peak | DeconvolvedPeak]
     """Peaks in the chromatogram"""
@@ -470,21 +471,21 @@
         self.peaks = [peak for peak in self.peaks if len(peak.components) > 0]
 
         return self
 
     # serialization and deserialization
     def to_dict(self) -> Dict[str, Any]:
         """Converts the data to a dictionary for serialization"""
-        data = super().to_dict().copy()
+        data = super().to_dict()
         data["peaks"] = [peak.to_dict().copy() for peak in self.peaks]
         data["sample_path"] = self.sample_path
         data["blank_path"] = self.blank_path
         data["name"] = self.name
 
-        return data | {"__classname__": "Chromatogram"}
+        return dict_encoder(data | {"__classname__": "Chromatogram"})
 
     @staticmethod
     def from_dict(data: Dict[str, Any]) -> Chromatogram:
         """Creates a Chromatogram object from a dictionary"""
         assert data["__classname__"] == "Chromatogram"
         data2d = Data2D.from_dict(data | {"__classname__": "Data2D"})
         peaks = [
```

### Comparing `mocca2-0.1.1/src/mocca2/classes/component.py` & `mocca2-0.1.2/src/mocca2/classes/component.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 from typing import Any, Dict
 from numpy.typing import NDArray
 
 import numpy as np
 
+from mocca2.serializing import dict_encoder
+
 
 class Component:
     """Information about single deconvolved component of a peak"""
 
     concentration: NDArray
     """Concentration profile in the selected range"""
 
@@ -45,26 +47,26 @@
         """Returns peak area at given wavelength (specified by index)"""
 
         return self.integral * self.spectrum[wl_idx]
 
     def to_dict(self) -> Dict[str, Any]:
         """Converts the data to a dictionary for serialization"""
         data = self.__dict__.copy()
-        data["spectrum"] = data["spectrum"].tolist()
-        data["concentration"] = data["concentration"].tolist()
-        return data | {"__classname__": "Component"}
+        data["spectrum"] = data["spectrum"]
+        data["concentration"] = data["concentration"]
+        return dict_encoder(data | {"__classname__": "Component"})
 
     @staticmethod
     def from_dict(data: Dict[str, Any]) -> Component:
         """Creates a Component object from a dictionary"""
         assert data["__classname__"] == "Component"
 
         component = Component(
-            np.array(data["concentration"]),
-            np.array(data["spectrum"]),
-            int(data["elution_time"]),
-            float(data["peak_fraction"]),
-            data["compound_id"],
+            concentration=np.array(data["concentration"]),
+            spectrum=np.array(data["spectrum"]),
+            compound_id=(
+                int(data["compound_id"]) if data["compound_id"] is not None else None
+            ),
         )
-        component.integral = data["integral"]
+        component.integral = float(data["integral"])
         component.elution_time = int(data["elution_time"])
         return component
```

### Comparing `mocca2-0.1.1/src/mocca2/classes/compound.py` & `mocca2-0.1.2/src/mocca2/classes/compound.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from typing import List, Tuple, Dict, Any
 from numpy.typing import NDArray
 
 from scipy.ndimage import gaussian_filter  # type: ignore
 from scipy.signal import find_peaks  # type: ignore
 import numpy as np
 
+from mocca2.serializing import dict_encoder
+
 
 class Compound:
     """Information about single chemical compound"""
 
     elution_time: int
     """Index of the elution time on the time scale"""
 
@@ -63,22 +65,30 @@
                     self._absorption_maxima.append((p, h))
 
         return self._absorption_maxima
 
     def to_dict(self) -> Dict[str, Any]:
         """Converts the data to a dictionary for serialization"""
         data = self.__dict__.copy()
-        data["spectrum"] = data["spectrum"].tolist()
-        return data | {"__classname__": "Compound"}
+        data["spectrum"] = data["spectrum"]
+        return dict_encoder(data | {"__classname__": "Compound"})
 
     @staticmethod
     def from_dict(data: Dict[str, Any]) -> Compound:
         """Creates a Compound object from a dictionary"""
         assert data["__classname__"] == "Compound"
 
         return Compound(
             int(data["elution_time"]),
             np.array(data["spectrum"]),
             data["name"],
-            data["concentration_factor"],
-            data["concentration_factor_vs_istd"],
+            (
+                float(data["concentration_factor"])
+                if data["concentration_factor"] is not None
+                else None
+            ),
+            (
+                float(data["concentration_factor_vs_istd"])
+                if data["concentration_factor_vs_istd"] is not None
+                else None
+            ),
         )
```

### Comparing `mocca2-0.1.1/src/mocca2/classes/data2d.py` & `mocca2-0.1.2/src/mocca2/classes/data2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from numpy.typing import NDArray
 
 import numpy as np
 from scipy.interpolate import interp1d
 import matplotlib
 from matplotlib import pyplot as plt
 
+from mocca2.serializing import dict_encoder
+
 
 class Data2D:
     """2D chromatogram data"""
 
     time: NDArray
     """Time points at which data was sampled"""
     wavelength: NDArray
@@ -237,20 +239,20 @@
 
         return Data2D(self.time, self.wavelength, self.data - other)
 
     # Methods for serializing and deserializing the data
     def to_dict(self) -> Dict[str, Any]:
         """Converts the data to a dictionary for serialization"""
         dic = {
-            "time": self.time.tolist(),
-            "wavelength": self.wavelength.tolist(),
-            "data": self.data.tolist(),
+            "time": self.time,
+            "wavelength": self.wavelength,
+            "data": self.data,
             "__classname__": "Data2D",
         }
-        return dic
+        return dict_encoder(dic)
 
     @staticmethod
     def from_dict(data: Dict[str, Any]) -> Data2D:
         """Creates a Data2D object from a dictionary"""
         assert data["__classname__"] == "Data2D"
 
         return Data2D(
```

### Comparing `mocca2-0.1.1/src/mocca2/classes/deconvolved_peak.py` & `mocca2-0.1.2/src/mocca2/classes/deconvolved_peak.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from typing import List, Dict, Any
 from numpy.typing import NDArray
 
 import numpy as np
 
 from mocca2.classes import Peak, Component
+from mocca2.serializing import dict_encoder
 
 
 class DeconvolvedPeak(Peak):
     """Information about peak and its deconvolved components"""
 
     components: List[Component]
     """Deconvolved components of the peak"""
@@ -115,25 +116,25 @@
         data = super().to_dict().copy()
         data["components"] = [c.to_dict().copy() for c in self.components]
         data["residual_mse"] = self.residual_mse
         data["r2"] = self.r2
         data["resolved"] = self.resolved
 
         data["__classname__"] = "DeconvolvedPeak"
-        return data
+        return dict_encoder(data)
 
     @staticmethod
     def from_dict(data: Dict[str, Any]) -> DeconvolvedPeak:
         """Creates a DeconvolvedPeak object from a dictionary"""
         assert data["__classname__"] == "DeconvolvedPeak"
 
         peak = Peak.from_dict(data | {"__classname__": "Peak"})
-        residual_mse = data["residual_mse"]
-        r2 = data["r2"]
-        resolved = data["resolved"]
+        residual_mse = float(data["residual_mse"])
+        r2 = float(data["r2"])
+        resolved = bool(data["resolved"])
         components = [Component.from_dict(c) for c in data["components"]]
         concs = np.array([c.concentration for c in components])
         specs = np.array([c.spectrum for c in components])
 
         deconvolved_peak = DeconvolvedPeak(
             peak, concs, specs, residual_mse, r2, resolved
         )
```

### Comparing `mocca2-0.1.1/src/mocca2/classes/peak.py` & `mocca2-0.1.2/src/mocca2/classes/peak.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 from typing import List, Any, Dict
 from numpy.typing import NDArray
 
 from mocca2.classes import Data2D
+from mocca2.serializing import dict_encoder
 
 
 class Peak:
     """Information about single peak"""
 
     left: int
     """Index of peak start"""
@@ -45,15 +46,15 @@
     def time(self, data: NDArray | Data2D) -> NDArray:
         """Returns part of the timescale that contains this peak"""
         y = data.time if isinstance(data, Data2D) else data
         return y[self.left : self.right]
 
     def to_dict(self) -> Dict[str, Any]:
         """Converts the data to a dictionary for serialization"""
-        return self.__dict__.copy() | {"__classname__": "Peak"}
+        return dict_encoder(self.__dict__.copy() | {"__classname__": "Peak"})
 
     @staticmethod
     def from_dict(data: Dict[str, Any]) -> Peak:
         """Creates a Peak object from a dictionary"""
         assert data["__classname__"] == "Peak"
 
         return Peak(
```

### Comparing `mocca2-0.1.1/src/mocca2/clustering/cluster_components.py` & `mocca2-0.1.2/src/mocca2/clustering/cluster_components.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/src/mocca2/dataset/dataset.py` & `mocca2-0.1.2/src/mocca2/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from mocca2.classes.chromatogram import Chromatogram
 from mocca2.classes.data2d import Data2D
 from mocca2.classes import Compound, Component
 from mocca2.dataset.settings import ProcessingSettings
 from mocca2.clustering.cluster_components import cluster_components
 from mocca2.math import cosine_similarity
+from mocca2.serializing import dict_encoder
 
 
 class MoccaDataset:
     """Collection of chromatograms, compounds, and other information"""
 
     _raw_2d_data: Dict[int, Data2D]
     """2D chromatogram data without wavelength cropping"""
@@ -645,15 +646,15 @@
             "compounds": {k: v.to_dict() for k, v in self.compounds.items()},
             "compound_references": self.compound_references,
             "istd_concentrations": self.istd_concentrations,
             "istd_chromatogram": self._istd_chromatogram,
             "istd_compound": self.istd_compound,
             "settings": self.settings.to_dict(),
         }
-        return dic | {"__classname__": "MoccaDataset"}
+        return dict_encoder(dic | {"__classname__": "MoccaDataset"})
 
     @staticmethod
     def from_dict(data: Dict[str, Any]) -> MoccaDataset:
         """Creates a MoccaDataset object from a dictionary"""
         assert data["__classname__"] == "MoccaDataset"
 
         dataset = MoccaDataset()
@@ -662,17 +663,32 @@
         }
         dataset._raw_2d_data = {
             int(k): Data2D.from_dict(v) for k, v in data["_raw_2d_data"].items()
         }
         dataset.compounds = {
             int(k): Compound.from_dict(v) for k, v in data["compounds"].items()
         }
-        dataset.compound_references = data["compound_references"]
-        dataset.istd_concentrations = data["istd_concentrations"]
-        dataset._istd_chromatogram = data["istd_chromatogram"]
-        dataset.istd_compound = data["istd_compound"]
-        dataset.settings = ProcessingSettings.from_dict(data["settings"])
+        dataset.compound_references = {
+            int(k): (v[0], float(v[1]) if v[1] is not None else None)
+            for k, v in data["compound_references"].items()
+        }
+        dataset.istd_concentrations = {
+            int(k): float(v) for k, v in data["istd_concentrations"].items()
+        }
+        dataset._istd_chromatogram = (
+            int(data["istd_chromatogram"])
+            if data["istd_chromatogram"] is not None
+            else None
+        )
+        dataset.istd_compound = (
+            int(data["istd_compound"]) if data["istd_compound"] is not None else None
+        )
+        dataset.settings = (
+            ProcessingSettings.from_dict(data["settings"])
+            if data["settings"] is not None
+            else None
+        )
         return dataset
 
 
 def _double_star_args(func, kwargs):
     return func(**kwargs)
```

### Comparing `mocca2-0.1.1/src/mocca2/dataset/settings.py` & `mocca2-0.1.2/src/mocca2/dataset/settings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 from typing import Literal, Dict, Any
 from dataclasses import dataclass
 import yaml  # type: ignore
 
+from mocca2.serializing import dict_encoder
+
 
 @dataclass(init=True)
 class ProcessingSettings:
     """Collection of all settings required for automatic chromatogram processing in MoccaDataset"""
 
     baseline_model: Literal["asls", "arpls", "flatfit"] = "flatfit"
     """Name of baseline estimator"""
@@ -54,22 +56,35 @@
     def from_yaml(data: str) -> ProcessingSettings:
         loaded = yaml.safe_load(data)
         settings = ProcessingSettings(**loaded)
         return settings
 
     def to_dict(self) -> Dict[str, Any]:
         """Converts the data to a dictionary for serialization"""
-        return self.__dict__ | {"__classname__": "ProcessingSettings"}
+        return dict_encoder(self.__dict__ | {"__classname__": "ProcessingSettings"})
 
     @staticmethod
     def from_dict(data: Dict[str, Any]) -> ProcessingSettings:
         """Creates a ProcessingSettings object from a dictionary"""
         assert data["__classname__"] == "ProcessingSettings"
 
-        return ProcessingSettings(
-            int(data["left"]),
-            int(data["right"]),
-            int(data["maximum"]),
-            float(data["height"]),
-            float(data["prominence"]),
-            [int(d) for d in data["all_maxima"]],
+        data.pop("__classname__")
+        settings = ProcessingSettings(
+            baseline_model=str(data["baseline_model"]),
+            baseline_smoothness=float(data["baseline_smoothness"]),
+            min_rel_prominence=float(data["min_rel_prominence"]),
+            min_prominence=float(data["min_prominence"]),
+            border_max_peak_cutoff=float(data["border_max_peak_cutoff"]),
+            split_threshold=float(data["split_threshold"]),
+            explained_threshold=float(data["explained_threshold"]),
+            peak_model=str(data["peak_model"]),
+            max_peak_comps=int(data["max_peak_comps"]),
+            max_peak_distance=float(data["max_peak_distance"]),
+            min_spectrum_correl=float(data["min_spectrum_correl"]),
+            min_elution_time=float(data["min_elution_time"]),
+            max_elution_time=float(data["max_elution_time"]),
+            min_wavelength=float(data["min_wavelength"]),
+            max_wavelength=float(data["max_wavelength"]),
+            min_rel_integral=float(data["min_rel_integral"]),
+            relaxe_concs=bool(data["relaxe_concs"]),
         )
+        return settings
```

### Comparing `mocca2-0.1.1/src/mocca2/deconvolution/__init__.py` & `mocca2-0.1.2/src/mocca2/deconvolution/__init__.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/src/mocca2/deconvolution/alternating_lstsq.py` & `mocca2-0.1.2/src/mocca2/deconvolution/alternating_lstsq.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/src/mocca2/deconvolution/deconvolve.py` & `mocca2-0.1.2/src/mocca2/deconvolution/deconvolve.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/src/mocca2/deconvolution/fit_peak_model.py` & `mocca2-0.1.2/src/mocca2/deconvolution/fit_peak_model.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/src/mocca2/deconvolution/guess_spectra.py` & `mocca2-0.1.2/src/mocca2/deconvolution/guess_spectra.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/src/mocca2/deconvolution/nnls.py` & `mocca2-0.1.2/src/mocca2/deconvolution/nnls.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/src/mocca2/deconvolution/nonnegative_lstsq.py` & `mocca2-0.1.2/src/mocca2/deconvolution/nonnegative_lstsq.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/src/mocca2/deconvolution/peak_models.py` & `mocca2-0.1.2/src/mocca2/deconvolution/peak_models.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/src/mocca2/example_data/loaders.py` & `mocca2-0.1.2/src/mocca2/example_data/loaders.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/src/mocca2/math.py` & `mocca2-0.1.2/src/mocca2/math.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/src/mocca2/parsers/empower.py` & `mocca2-0.1.2/src/mocca2/parsers/empower.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/src/mocca2/parsers/labsolutions.py` & `mocca2-0.1.2/src/mocca2/parsers/labsolutions.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/src/mocca2/parsers/wrapper.py` & `mocca2-0.1.2/src/mocca2/parsers/wrapper.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/src/mocca2/peaks/find_peaks.py` & `mocca2-0.1.2/src/mocca2/peaks/find_peaks.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/src/mocca2/peaks/merge_overlapping.py` & `mocca2-0.1.2/src/mocca2/peaks/merge_overlapping.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/src/mocca2/peaks/split.py` & `mocca2-0.1.2/src/mocca2/peaks/split.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/src/mocca2.egg-info/PKG-INFO` & `mocca2-0.1.2/src/mocca2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mocca2
-Version: 0.1.1
+Version: 0.1.2
 Summary: MOCCA2 is an open-source Python project to analyze HPLC-DAD raw data
 Author-email: Jan Oboril <jan.oboril@gmail.com>
 Project-URL: Homepage, https://oboril.github.io/mocca/
-Project-URL: Issues, https://github.com/oboril/mocca/issues
+Project-URL: Issues, https://github.com/oboril/MOCCA/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy>1.20
@@ -16,17 +16,17 @@
 Requires-Dist: scikit-learn>1.3
 Requires-Dist: pyyaml>6.0
 Requires-Dist: pandas>2.1
 Requires-Dist: matplotlib>3.6
 Requires-Dist: pyarrow>15.0
 
 [![PyPI](https://img.shields.io/pypi/v/mocca2.svg)](https://pypi.org/project/mocca2/)
-![pytest](https://github.com/oboril/mocca/actions/workflows/ci.yaml/badge.svg)
-[![Docs Pages](https://github.com/oboril/mocca/actions/workflows/deploy_pages.yaml/badge.svg)](https://oboril.github.io/mocca/)
-[![Example Data](https://github.com/oboril/mocca/actions/workflows/package_data.yaml/badge.svg)](https://github.com/oboril/mocca/tree/example-data)
+![pytest](https://github.com/oboril/MOCCA/actions/workflows/ci.yaml/badge.svg)
+[![Docs Pages](https://github.com/oboril/MOCCA/actions/workflows/deploy_pages.yaml/badge.svg)](https://oboril.github.io/mocca/)
+[![Example Data](https://github.com/oboril/MOCCA/actions/workflows/package_data.yaml/badge.svg)](https://github.com/oboril/MOCCA/tree/example-data)
 
 # Welcome to MOCCA2
 
 MOCCA2 is a Python package for automatic processing of HPLC chromatograms.
 
 To automate your workflow and get accurate results, MOCCA2 features:
  - support for raw data files from Agilent, Shimadzu and Waters
@@ -35,15 +35,15 @@
  - automatic purity checking and peak deconvolution
  - compound tracking across chromatograms
  - fully automatic processing of any number of chromatograms
 
 
 ## Documentation
 
-Examples and detailed documentation are documented at [https://oboril.github.io/mocca](https://oboril.github.io/mocca).
+Examples and detailed documentation are documented at [https://oboril.github.io/MOCCA](https://oboril.github.io/MOCCA).
 
 ## Getting Started
 
 The latest version of MOCCA2 can be installed simply using pip:
 
 ```
 pip install mocca2
@@ -116,12 +116,12 @@
  - and various standalone chromatograms
 
 Since these datasets don't fit into the PyPI package size limit, they are automatically compressed and published onto `example-data` branch on push to `main`. 
 
 The data can be automatically downloaded using ``python -m mocca2 --download-data``.
 
 ### Publishing to PyPI and GitHub
-On push to `main`, the MOCCA2 package is automatically published to [PyPI](https://pypi.org/project/mocca2/) and [GitHub Releases](https://github.com/oboril/mocca/releases).
+On push to `main`, the MOCCA2 package is automatically published to [PyPI](https://pypi.org/project/mocca2/) and [GitHub Releases](https://github.com/oboril/MOCCA/releases).
 
 ## Contributing
 
-The process for contributing is outlined in [CONTRIBUTING.md](https://github.com/oboril/mocca/blob/main/CONTRIBUTING.md).
+The process for contributing is outlined in [CONTRIBUTING.md](https://github.com/oboril/MOCCA/blob/main/CONTRIBUTING.md).
```

### Comparing `mocca2-0.1.1/src/mocca2.egg-info/SOURCES.txt` & `mocca2-0.1.2/src/mocca2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 src/mocca2/__init__.py
 src/mocca2/__main__.py
 src/mocca2/exceptions.py
 src/mocca2/math.py
 src/mocca2/py.typed
+src/mocca2/serializing.py
 src/mocca2.egg-info/PKG-INFO
 src/mocca2.egg-info/SOURCES.txt
 src/mocca2.egg-info/dependency_links.txt
 src/mocca2.egg-info/requires.txt
 src/mocca2.egg-info/top_level.txt
 src/mocca2/baseline/__init__.py
 src/mocca2/baseline/arpls.py
```

### Comparing `mocca2-0.1.1/tests/test_example_data.py` & `mocca2-0.1.2/tests/test_example_data.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.1.1/tests/test_serialization.py` & `mocca2-0.1.2/tests/test_serialization.py`

 * *Files identical despite different names*

