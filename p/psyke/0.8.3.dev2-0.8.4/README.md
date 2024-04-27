# Comparing `tmp/psyke-0.8.3.dev2.tar.gz` & `tmp/psyke-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyke-0.8.3.dev2.tar", last modified: Fri Apr 26 01:22:01 2024, max compression
+gzip compressed data, was "psyke-0.8.4.tar", last modified: Sat Apr 27 17:11:45 2024, max compression
```

## Comparing `psyke-0.8.3.dev2.tar` & `psyke-0.8.4.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.030802 psyke-0.8.3.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-26 01:22:01.030802 psyke-0.8.3.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 01:22:00.000000 psyke-0.8.3.dev2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.018802 psyke-0.8.3.dev2/psyke/
--rw-r--r--   0 runner    (1001) docker     (127)    18155 2024-04-26 01:21:59.000000 psyke-0.8.3.dev2/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.018802 psyke-0.8.3.dev2/psyke/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.018802 psyke-0.8.3.dev2/psyke/clustering/cream/
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/clustering/cream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.018802 psyke-0.8.3.dev2/psyke/clustering/exact/
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/clustering/exact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/clustering/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.018802 psyke-0.8.3.dev2/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.018802 psyke-0.8.3.dev2/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/extraction/cart/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.022802 psyke-0.8.3.dev2/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.022802 psyke-0.8.3.dev2/psyke/extraction/hypercubic/cosmik/
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/extraction/hypercubic/cosmik/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.022802 psyke-0.8.3.dev2/psyke/extraction/hypercubic/creepy/
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/extraction/hypercubic/creepy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.022802 psyke-0.8.3.dev2/psyke/extraction/hypercubic/divine/
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/extraction/hypercubic/divine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.022802 psyke-0.8.3.dev2/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/extraction/hypercubic/gridex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.022802 psyke-0.8.3.dev2/psyke/extraction/hypercubic/gridrex/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/extraction/hypercubic/gridrex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.022802 psyke-0.8.3.dev2/psyke/extraction/hypercubic/hex/
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/extraction/hypercubic/hex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24510 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/extraction/hypercubic/hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.022802 psyke-0.8.3.dev2/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/extraction/hypercubic/iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/extraction/hypercubic/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/extraction/hypercubic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.022802 psyke-0.8.3.dev2/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/extraction/real/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.022802 psyke-0.8.3.dev2/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/extraction/trepan/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/hypercubepredictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.022802 psyke-0.8.3.dev2/psyke/schema/
--rw-r--r--   0 runner    (1001) docker     (127)    15760 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.022802 psyke-0.8.3.dev2/psyke/tuning/
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/tuning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.022802 psyke-0.8.3.dev2/psyke/tuning/crash/
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/tuning/crash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.022802 psyke-0.8.3.dev2/psyke/tuning/orchid/
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/tuning/orchid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.022802 psyke-0.8.3.dev2/psyke/tuning/pedro/
--rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/tuning/pedro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.026802 psyke-0.8.3.dev2/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/utils/logic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/psyke/utils/sorted.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.030802 psyke-0.8.3.dev2/psyke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-26 01:22:00.000000 psyke-0.8.3.dev2/psyke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-26 01:22:01.000000 psyke-0.8.3.dev2/psyke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 01:22:00.000000 psyke-0.8.3.dev2/psyke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 01:22:00.000000 psyke-0.8.3.dev2/psyke.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-26 01:22:00.000000 psyke-0.8.3.dev2/psyke.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 01:22:00.000000 psyke-0.8.3.dev2/psyke.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 01:22:01.030802 psyke-0.8.3.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.014802 psyke-0.8.3.dev2/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.026802 psyke-0.8.3.dev2/test/psyke/
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/test/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.026802 psyke-0.8.3.dev2/test/psyke/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/test/psyke/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.026802 psyke-0.8.3.dev2/test/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/test/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.026802 psyke-0.8.3.dev2/test/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/test/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/test/psyke/extraction/cart/test_cart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/test/psyke/extraction/cart/test_simplified_cart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.026802 psyke-0.8.3.dev2/test/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/test/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.026802 psyke-0.8.3.dev2/test/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/test/psyke/extraction/hypercubic/gridex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/test/psyke/extraction/hypercubic/gridex/test_gridex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.026802 psyke-0.8.3.dev2/test/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/test/psyke/extraction/hypercubic/iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/test/psyke/extraction/hypercubic/iter/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14255 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/test/psyke/extraction/hypercubic/test_hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.026802 psyke-0.8.3.dev2/test/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/test/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/test/psyke/extraction/real/test_real.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/test/psyke/extraction/real/test_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.026802 psyke-0.8.3.dev2/test/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/test/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/test/psyke/extraction/trepan/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/test/psyke/extraction/trepan/test_split.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/test/psyke/extraction/trepan/test_trepan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.030802 psyke-0.8.3.dev2/test/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/test/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/test/psyke/utils/test_prune.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/test/psyke/utils/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-26 01:19:49.000000 psyke-0.8.3.dev2/test/psyke/utils/test_simplify_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.030802 psyke-0.8.3.dev2/test/resources/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 01:19:51.000000 psyke-0.8.3.dev2/test/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.030802 psyke-0.8.3.dev2/test/resources/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-26 01:19:51.000000 psyke-0.8.3.dev2/test/resources/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.030802 psyke-0.8.3.dev2/test/resources/predictors/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-26 01:19:51.000000 psyke-0.8.3.dev2/test/resources/predictors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:22:01.030802 psyke-0.8.3.dev2/test/resources/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-26 01:19:51.000000 psyke-0.8.3.dev2/test/resources/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.772245 psyke-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-04-27 17:10:31.000000 psyke-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-27 17:10:31.000000 psyke-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-04-27 17:11:45.772245 psyke-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-27 17:10:31.000000 psyke-0.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-27 17:11:45.000000 psyke-0.8.4/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.760245 psyke-0.8.4/psyke/
+-rw-r--r--   0 runner    (1001) docker     (127)    18155 2024-04-27 17:11:43.000000 psyke-0.8.4/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.760245 psyke-0.8.4/psyke/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.760245 psyke-0.8.4/psyke/clustering/cream/
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/clustering/cream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.760245 psyke-0.8.4/psyke/clustering/exact/
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/clustering/exact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/clustering/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.760245 psyke-0.8.4/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.760245 psyke-0.8.4/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/cart/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/extraction/hypercubic/cosmik/
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/hypercubic/cosmik/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/extraction/hypercubic/creepy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/hypercubic/creepy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/extraction/hypercubic/divine/
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/hypercubic/divine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/hypercubic/gridex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/extraction/hypercubic/gridrex/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/hypercubic/gridrex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/extraction/hypercubic/hex/
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/hypercubic/hex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25430 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/hypercubic/hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/hypercubic/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/hypercubic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/real/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/trepan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/hypercubepredictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)    17306 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/tuning/
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/tuning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/tuning/crash/
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/tuning/crash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/tuning/orchid/
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/tuning/orchid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/tuning/pedro/
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/tuning/pedro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/utils/logic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/utils/sorted.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.772245 psyke-0.8.4/psyke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-04-27 17:11:45.000000 psyke-0.8.4/psyke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-27 17:11:45.000000 psyke-0.8.4/psyke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:11:45.000000 psyke-0.8.4/psyke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:11:45.000000 psyke-0.8.4/psyke.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-27 17:11:45.000000 psyke-0.8.4/psyke.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-27 17:11:45.000000 psyke-0.8.4/psyke.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-27 17:10:31.000000 psyke-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 17:11:45.772245 psyke-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-27 17:10:31.000000 psyke-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.756245 psyke-0.8.4/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/psyke/
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/psyke/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/cart/test_cart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/cart/test_simplified_cart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/hypercubic/gridex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/hypercubic/gridex/test_gridex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/hypercubic/iter/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14255 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/hypercubic/test_hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/real/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/real/test_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/trepan/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/trepan/test_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/trepan/test_trepan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/utils/test_prune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/utils/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/utils/test_simplify_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-27 17:10:33.000000 psyke-0.8.4/test/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/resources/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-27 17:10:33.000000 psyke-0.8.4/test/resources/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.772245 psyke-0.8.4/test/resources/predictors/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-27 17:10:33.000000 psyke-0.8.4/test/resources/predictors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.772245 psyke-0.8.4/test/resources/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-27 17:10:33.000000 psyke-0.8.4/test/resources/tests/__init__.py
```

### Comparing `psyke-0.8.3.dev2/LICENSE` & `psyke-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/PKG-INFO` & `psyke-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.8.3.dev2
+Version: 0.8.4
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.8.3.dev2/README.md` & `psyke-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/__init__.py` & `psyke-0.8.4/psyke/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/clustering/__init__.py` & `psyke-0.8.4/psyke/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/clustering/cream/__init__.py` & `psyke-0.8.4/psyke/clustering/cream/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/clustering/exact/__init__.py` & `psyke-0.8.4/psyke/clustering/exact/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/clustering/utils.py` & `psyke-0.8.4/psyke/clustering/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/extraction/__init__.py` & `psyke-0.8.4/psyke/extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/extraction/cart/__init__.py` & `psyke-0.8.4/psyke/extraction/cart/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/extraction/cart/predictor.py` & `psyke-0.8.4/psyke/extraction/cart/predictor.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/extraction/hypercubic/__init__.py` & `psyke-0.8.4/psyke/extraction/hypercubic/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import math
 from abc import ABC
 import numpy as np
 import pandas as pd
 from sklearn.base import ClassifierMixin
 from sklearn.feature_selection import SelectKBest, f_regression, f_classif
 from sklearn.linear_model import LinearRegression
 from tuprolog.core import Var, Struct, clause
@@ -92,76 +93,52 @@
                         output += f"\n     {d} decreses below {round(upper, 1)}"
                         different_prediction_reasons.append((d, '<=', upper))
         if verbose:
             print(output)
         return prediction, different_prediction_reasons
 
     def __get_local_conditions(self, data: dict[str, float], cube: GenericCube) -> dict[list[Value]]:
-        conditions = {d: [Between(*cube.dimensions[d])] for d in cube.dimensions}
+        conditions = {d: [cube.interval_to_value(d, self.unscale)] for d in data.keys()}
         subcubes = cube.subcubes(self._hypercubes)
-        for c in [c for c in subcubes if sum(c in sc and c != sc for sc in subcubes) == 0]:
-            for d in [d for d in c.dimensions if d in data]:
-                if c.dimensions[d][0] > data[d] or c.dimensions[d][1] < data[d]:
-                    conditions[d].append(Outside(*c.dimensions[d]))
+        subsubcubes = [c for cube_list in [c.subcubes(self._hypercubes) for c in subcubes] for c in cube_list]
+        for c in [c for c in subcubes if c not in subsubcubes]:
+            for d in conditions:
+                condition = c.interval_to_value(d, self.unscale)
+                if condition is None:
+                    continue
+                elif conditions[d][-1] is None:
+                    conditions[d][-1] = -condition
+                elif (-condition).is_in(data[d]):
+                    try:
+                        conditions[d][-1] *= -condition
+                    except Exception:
+                        conditions[d].append(-condition)
         return conditions
 
     def predict_why(self, data: dict[str, float]):
         cube = self._find_cube(data.copy())
         if cube is None:
             print("The extracted knowledge is not exhaustive; impossible to predict this instance")
         else:
             output = self._predict_from_cubes(data)
             print(f"The output is {output} because")
             conditions = self.__get_local_conditions(data, cube)
-            for d in data.keys():
-                simplified = HyperCubeExtractor.__simplify(conditions[d])
-                for i, condition in enumerate(simplified):
-                    if i == 0:
+            for d in conditions:
+                for i, condition in enumerate(conditions[d]):
+                    if condition is None:
+                        continue
+                    elif i == 0:
                         print('    ', d, 'is', end=' ')
                     else:
                         print('and', end=' ')
-                    if isinstance(condition, Outside):
-                        print('not', end=' ')
-                    print('between', round(condition.lower, 1), 'and', round(condition.upper, 1), end=' ')
-                    if i + 1 == len(simplified):
+                    print(condition.print(), end='')
+                    if i + 1 == len(conditions[d]):
                         print()
 
     @staticmethod
-    def __simplify(conditions):
-        simplified = []
-        for condition in conditions:
-            to_add = True
-            for i, simple in enumerate(simplified):
-                if isinstance(condition, Outside) and isinstance(simple, Outside):
-                    if simple.lower <= condition.lower <= simple.upper or \
-                            simple.lower <= condition.upper <= simple.upper or \
-                            condition.lower <= simple.lower <= simple.upper <= condition.upper:
-                        simplified[i].upper = max(condition.upper, simple.upper)
-                        simplified[i].lower = min(condition.lower, simple.lower)
-                        to_add = False
-                        break
-                elif isinstance(condition, Outside) and isinstance(simple, Between):
-                    if simple.lower >= condition.upper or simple.upper <= condition.lower:
-                        to_add = False
-                        break
-                    elif condition.lower <= simple.lower <= condition.upper <= simple.upper:
-                        simplified[i].lower = condition.upper
-                        to_add = False
-                        break
-                    elif simple.lower <= condition.lower <= simple.upper <= condition.upper:
-                        simplified[i].upper = condition.lower
-                        to_add = False
-                        break
-                    elif condition.lower <= simple.lower <= simple.upper <= condition.upper:
-                        raise ValueError
-            if to_add:
-                simplified.append(condition)
-        return simplified
-
-    @staticmethod
     def _create_head(dataframe: pd.DataFrame, variables: list[Var], output: float | LinearRegression) -> Struct:
         return create_head(dataframe.columns[-1], variables[:-1], output) \
             if not isinstance(output, LinearRegression) else \
             create_head(dataframe.columns[-1], variables[:-1], variables[-1])
 
     def __drop(self, dataframe: pd.DataFrame):
         self._hypercubes = [cube for cube in self._hypercubes if cube.count(dataframe) > 1]
```

### Comparing `psyke-0.8.3.dev2/psyke/extraction/hypercubic/cosmik/__init__.py` & `psyke-0.8.4/psyke/extraction/hypercubic/cosmik/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/extraction/hypercubic/creepy/__init__.py` & `psyke-0.8.4/psyke/extraction/hypercubic/creepy/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/extraction/hypercubic/divine/__init__.py` & `psyke-0.8.4/psyke/extraction/hypercubic/divine/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/extraction/hypercubic/gridex/__init__.py` & `psyke-0.8.4/psyke/extraction/hypercubic/gridex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/extraction/hypercubic/gridrex/__init__.py` & `psyke-0.8.4/psyke/extraction/hypercubic/gridrex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/extraction/hypercubic/hex/__init__.py` & `psyke-0.8.4/psyke/extraction/hypercubic/hex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/extraction/hypercubic/hypercube.py` & `psyke-0.8.4/psyke/extraction/hypercubic/hypercube.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 from psyke.extraction.hypercubic.utils import Dimension, Dimensions, MinUpdate, ZippedDimension, Limit, Expansion
 from psyke.schema import Between, GreaterThan, LessThan
 from psyke.utils import get_default_precision, get_int_precision, Target, get_default_random_seed
 from psyke.utils.logic import create_term, to_rounded_real, linear_function_creator
 from sklearn.linear_model import LinearRegression
 from tuprolog.core import Var, Struct
-from random import Random
 import numpy as np
 
 
 class FeatureNotFoundException(Exception):
 
     def __init__(self, feature: str):
         super().__init__(f'Feature {feature} not found.')
@@ -145,14 +144,17 @@
 
     def set_infinite(self, dimension: str, direction: str):
         if dimension in self._infinite_dimensions:
             self._infinite_dimensions[dimension].append(direction)
         else:
             self._infinite_dimensions[dimension] = [direction]
 
+    def copy_infinite_dimensions(self, dimensions: dict[str, str]):
+        self._infinite_dimensions = dimensions.copy()
+
     @property
     def dimensions(self) -> Dimensions:
         return self._dimensions
 
     @property
     def limit_count(self) -> int:
         return len(self._limits)
@@ -227,31 +229,33 @@
             for hypercube in hypercubes:
                 if hypercube not in checked and cube.overlap(hypercube):
                     return True
             checked += [cube]
         return False
 
     def copy(self) -> HyperCube:
-        return HyperCube(self.dimensions.copy(), self._limits.copy(), self.output)
+        new_cube = HyperCube(self.dimensions.copy(), self._limits.copy(), self.output)
+        new_cube.copy_infinite_dimensions(self._infinite_dimensions)
+        return new_cube
 
     def count(self, dataset: pd.DataFrame) -> int:
         return self.filter_dataframe(dataset.iloc[:, :-1]).shape[0]
 
-    def _interval_to_value(self, dimension, unscale):
+    def interval_to_value(self, dimension, unscale=None):
         if dimension not in self._infinite_dimensions:
             return Between(unscale(self[dimension][0], dimension), unscale(self[dimension][1], dimension))
         if len(self._infinite_dimensions[dimension]) == 2:
             return
         if '+' in self._infinite_dimensions[dimension]:
             return GreaterThan(unscale(self[dimension][0], dimension))
         if '-' in self._infinite_dimensions[dimension]:
             return LessThan(unscale(self[dimension][1], dimension))
 
     def body(self, variables: dict[str, Var], ignore: list[str], unscale=None, normalization=None) -> Iterable[Struct]:
-        values = [(dim, self._interval_to_value(dim, unscale)) for dim in self.dimensions if dim not in ignore]
+        values = [(dim, self.interval_to_value(dim, unscale)) for dim in self.dimensions if dim not in ignore]
         return [create_term(variables[name], value) for name, value in values
                 if not self.is_default and value is not None]
 
     @staticmethod
     def create_surrounding_cube(dataset: pd.DataFrame, closed: bool = False,
                                 output=None) -> GenericCube:
         output = Target.CONSTANT if output is None else output
@@ -435,16 +439,16 @@
 
     # TODO: why this is not a property?
     def init_diversity(self, std: float) -> None:
         self._diversity = std
 
 
 class RegressionCube(HyperCube):
-    def __init__(self, dimension: dict[str, tuple] = None, output=None):
-        super().__init__(dimension=dimension, output=LinearRegression() if output is None else output)
+    def __init__(self, dimension: dict[str, tuple] = None, limits: set[Limit] = None, output=None):
+        super().__init__(dimension=dimension, limits=limits, output=LinearRegression() if output is None else output)
 
     def update(self, dataset: pd.DataFrame, predictor) -> None:
         filtered = self.filter_dataframe(dataset.iloc[:, :-1])
         if len(filtered > 0):
             predictions = predictor.predict(filtered)
             self._output.fit(filtered, predictions)
             self._diversity = self._error = (abs(self._output.predict(filtered) - predictions)).mean()
@@ -454,15 +458,17 @@
     def copy(self) -> RegressionCube:
         output = LinearRegression()
         try:
             output.coef_ = self.output.coef_.copy()
             output.intercept_ = self.output.intercept_
         except AttributeError:
             pass
-        return RegressionCube(self.dimensions.copy(), output=output)
+        new_cube = RegressionCube(self.dimensions.copy(), self._limits.copy(), output)
+        new_cube.copy_infinite_dimensions(self._infinite_dimensions)
+        return new_cube
 
     def body(self, variables: dict[str, Var], ignore: list[str], unscale=None, normalization=None) -> Iterable[Struct]:
         intercept = self.output.intercept_ if normalization is None else unscale(sum(
             [-self.output.coef_[i] * normalization[name][0] / normalization[name][1] for i, name in
              enumerate(self.dimensions.keys())], self.output.intercept_), list(normalization.keys())[-1])
         coefs = self.output.coef_ if normalization is None else [
             self.output.coef_[i] / normalization[name][1] * normalization[list(normalization.keys())[-1]][1] for
@@ -483,20 +489,23 @@
             predictions = predictor.predict(filtered)
             self._output = mode(predictions)
             self._diversity = self._error = 1 - sum(p == self.output for p in predictions) / len(predictions)
             means = filtered.describe().loc['mean']
             self._barycenter = Point(means.index.values, means.values)
 
     def copy(self) -> ClassificationCube:
-        return ClassificationCube(self.dimensions.copy(), self._limits.copy(), self._output)
+        new_cube = ClassificationCube(self.dimensions.copy(), self._limits.copy(), self.output)
+        new_cube.copy_infinite_dimensions(self._infinite_dimensions)
+        return new_cube
 
 
 class ClosedCube(HyperCube):
-    def __init__(self, dimension: dict[str, tuple] = None, output: str | LinearRegression | float = 0.0):
-        super().__init__(dimension=dimension, output=output)
+    def __init__(self, dimension: dict[str, tuple] = None, limits: set[Limit] = None,
+                 output: str | LinearRegression | float = 0.0):
+        super().__init__(dimension=dimension, limits=limits, output=output)
 
     def __contains__(self, obj: dict[str, float] | ClosedCube) -> bool:
         """
        Note that an object is inside a hypercube if ALL its dimensions' values satisfy:
            min_dim <= object dimension <= max_dim
        :param obj: an N-dimensional object (point or hypercube)
        :return: true if the object is inside the hypercube, false otherwise
@@ -529,34 +538,40 @@
 
     def filter_indices(self, dataset: pd.DataFrame) -> ndarray:
         v = np.array([v for _, v in self._dimensions.items()])
         ds = dataset.to_numpy(copy=True)
         return np.all((v[:, 0] <= ds) & (ds <= v[:, 1]), axis=1)
 
     def copy(self) -> ClosedCube:
-        return ClosedCube(self.dimensions.copy(), output=self._output)
+        new_cube = ClosedCube(self.dimensions.copy(), self._limits.copy(), self.output)
+        new_cube.copy_infinite_dimensions(self._infinite_dimensions)
+        return new_cube
 
 
 class ClosedRegressionCube(ClosedCube, RegressionCube):
-    def __init__(self, dimension: dict[str, tuple] = None, output=None):
-        super().__init__(dimension=dimension, output=LinearRegression() if output is None else output)
+    def __init__(self, dimension: dict[str, tuple] = None, limits: set[Limit] = None, output=None):
+        super().__init__(dimension=dimension, limits=limits, output=LinearRegression() if output is None else output)
 
     def copy(self) -> ClosedRegressionCube:
         output = LinearRegression()
         try:
             output.coef_ = self.output.coef_.copy()
             output.intercept_ = self.output.intercept_
         except AttributeError:
             pass
-        return ClosedRegressionCube(self.dimensions.copy(), output=output)
+        new_cube = ClosedRegressionCube(self.dimensions.copy(), self._limits.copy(), output)
+        new_cube.copy_infinite_dimensions(self._infinite_dimensions)
+        return new_cube
 
 
 class ClosedClassificationCube(ClosedCube, ClassificationCube):
-    def __init__(self, dimension: dict[str, tuple] = None, output: str = None):
-        super().__init__(dimension=dimension, output=output)
+    def __init__(self, dimension: dict[str, tuple] = None, limits: set[Limit] = None, output: str = None):
+        super().__init__(dimension=dimension, limits=limits, output=output)
 
     def copy(self) -> ClosedClassificationCube:
-        return ClosedClassificationCube(self.dimensions.copy(), output=self._output)
+        new_cube = ClosedClassificationCube(self.dimensions.copy(), self._limits.copy(), self.output)
+        new_cube.copy_infinite_dimensions(self._infinite_dimensions)
+        return new_cube
 
 
 GenericCube = Union[HyperCube, ClassificationCube, RegressionCube,
                     ClosedCube, ClosedRegressionCube, ClosedClassificationCube]
```

### Comparing `psyke-0.8.3.dev2/psyke/extraction/hypercubic/iter/__init__.py` & `psyke-0.8.4/psyke/extraction/hypercubic/iter/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/extraction/hypercubic/strategy.py` & `psyke-0.8.4/psyke/extraction/hypercubic/strategy.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/extraction/hypercubic/utils.py` & `psyke-0.8.4/psyke/extraction/hypercubic/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/extraction/real/__init__.py` & `psyke-0.8.4/psyke/extraction/real/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/extraction/real/utils.py` & `psyke-0.8.4/psyke/extraction/real/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/extraction/trepan/__init__.py` & `psyke-0.8.4/psyke/extraction/trepan/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/extraction/trepan/utils.py` & `psyke-0.8.4/psyke/extraction/trepan/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/hypercubepredictor.py` & `psyke-0.8.4/psyke/hypercubepredictor.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/schema/__init__.py` & `psyke-0.8.4/psyke/schema/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -81,65 +81,82 @@
             if type(self) is type(other):
                 return self.is_in_or_is_boundary(other.lower) and self.is_in_or_is_boundary(other.upper)
             else:
                 return self.is_in(other.lower) and self.is_in(other.upper)
         else:
             return False
 
+    def __neg__(self) -> Value:
+        if isinstance(self, Constant):
+            return self
+        elif isinstance(self, GreaterThan):
+            return LessThan(self.value, self.standard)
+        elif isinstance(self, LessThan):
+            return GreaterThan(self.value, self.standard)
+        elif isinstance(self, Between):
+            return Outside(self.lower, self.upper, self.standard)
+        elif isinstance(self, Outside):
+            return Between(self.lower, self.upper, self.standard)
+        else:
+            raise TypeError
+
     # TODO: handle convention (low priority).
     def __mul__(self, other) -> Value:
 
         def intersection_with_constant(first_value: Constant, second_value: Value) -> Value:
             if isinstance(first_value, Constant):
-                if second_value.is_in(first_value.value):
+                if first_value in second_value:
                     return first_value
                 else:
                     raise _EMPTY_INTERSECTION_EXCEPTION(first_value, second_value)
             else:
                 raise _INTERSECTION_WITH_WRONG_TYPE(first_value, second_value)
 
         def intersection_with_outside(first_value: Outside, second_value: Value) -> Value:
             if isinstance(first_value, Outside):
                 if isinstance(second_value, LessThan):
-                    if second_value.value <= first_value.lower:
-                        return second_value
-                    elif first_value.is_in(second_value.value):
+                    if second_value.value > first_value.upper:
+                        # LessThan(first_value.lower) + Between(first_value.lower, second_value.value)
+                        raise _NOT_IMPLEMENTED_INTERSECTION(first_value, second_value)
+                    elif second_value.value > first_value.lower:
                         return LessThan(first_value.lower)
                     else:
-                        raise _NOT_IMPLEMENTED_INTERSECTION(first_value, second_value)
+                        return second_value
                 elif isinstance(second_value, GreaterThan):
-                    if second_value.value >= first_value.lower:
+                    if second_value.value < first_value.lower:
+                        # Between(second_value.value, first_value.lower) + GreaterThan(first_value.upper)
+                        raise _NOT_IMPLEMENTED_INTERSECTION(first_value, second_value)
+                    elif second_value.value < first_value.upper:
                         return GreaterThan(first_value.upper)
-                    elif first_value.is_in(second_value.value):
-                        return second_value
                     else:
-                        raise _NOT_IMPLEMENTED_INTERSECTION(first_value, second_value)
-                elif isinstance(second_value, Constant):
-                    if not first_value.is_in(second_value.value):
                         return second_value
-                    else:
-                        raise _EMPTY_INTERSECTION_EXCEPTION(first_value, second_value)
                 elif isinstance(second_value, Between):
-                    if second_value in first_value:
+                    if second_value.upper <= first_value.lower or second_value.lower >= first_value.upper:
                         return second_value
                     elif second_value.lower <= first_value.lower <= second_value.upper <= first_value.upper:
                         return Between(second_value.lower, first_value.lower)
                     elif first_value.lower <= second_value.lower <= first_value.upper <= second_value.upper:
                         return Between(first_value.upper, second_value.upper)
-                    else:
+                    elif second_value.lower <= first_value.lower <= first_value.upper <= second_value.upper:
                         raise _NOT_IMPLEMENTED_INTERSECTION(first_value, second_value)
+                    else:
+                        raise _EMPTY_INTERSECTION_EXCEPTION(first_value, second_value)
                 elif isinstance(second_value, Outside):
-                    if second_value.lower <= first_value.lower and second_value.upper >= first_value.upper:
+                    if second_value.lower <= first_value.lower <= first_value.upper <= second_value.upper:
                         return second_value
-                    elif first_value.lower <= second_value.lower and first_value.upper >= second_value.upper:
+                    elif first_value.lower <= second_value.lower <= second_value.upper <= first_value.upper:
                         return first_value
+                    elif second_value.lower <= first_value.lower <= second_value.upper <= first_value.upper:
+                        return Outside(second_value.lower, first_value.upper)
+                    elif first_value.lower <= second_value.lower <= first_value.upper <= second_value.upper:
+                        return Outside(first_value.lower, second_value.upper)
                     else:
                         raise _EMPTY_INTERSECTION_EXCEPTION(first_value, second_value)
                 elif isinstance(second_value, Constant):
-                    intersection_with_constant(second_value, first_value)
+                    return intersection_with_constant(second_value, first_value)
                 else:
                     raise _INTERSECTION_WITH_WRONG_TYPE(first_value, second_value)
             else:
                 raise _INTERSECTION_WITH_WRONG_TYPE(first_value, second_value)
 
         def intersection_with_between(first_value: Between, second_value: Value) -> Value:
             if isinstance(first_value, Between):
@@ -169,15 +186,15 @@
                     elif first_value.lower <= second_value.upper <= first_value.upper:
                         return Between(first_value.lower, second_value.upper)
                     elif second_value.lower <= first_value.upper <= second_value.upper:
                         return Between(second_value.lower, first_value.upper)
                     else:
                         raise _EMPTY_INTERSECTION_EXCEPTION(first_value, second_value)
                 elif isinstance(second_value, Constant):
-                    intersection_with_constant(second_value, first_value)
+                    return intersection_with_constant(second_value, first_value)
                 elif isinstance(second_value, Outside):
                     return intersection_with_outside(second_value, first_value)
                 else:
                     raise _INTERSECTION_WITH_WRONG_TYPE(first_value, second_value)
             else:
                 raise _INTERSECTION_WITH_WRONG_TYPE(first_value, second_value)
 
@@ -260,14 +277,17 @@
     def is_in(self, other: float) -> bool:
         return other <= self.upper if self.standard else other < self.upper
 
     @property
     def value(self) -> float:
         return self.upper
 
+    def print(self) -> str:
+        return f"below {round(self.upper, 1)}"
+
     def __str__(self):
         return f"]-∞, {self.upper:.2f}" + ("]" if self.standard else "[")
 
     def __repr__(self):
         return f"LessThan({self.upper:.2f})"
 
     def __eq__(self, other: LessThan) -> bool:
@@ -282,14 +302,17 @@
     def is_in(self, other: float) -> bool:
         return other > self.lower if self.standard else other >= self.lower
 
     @property
     def value(self) -> float:
         return self.lower
 
+    def print(self) -> str:
+        return f"above {round(self.lower, 1)}"
+
     def __str__(self):
         return ("]" if self.standard else "[") + f"{self.lower:.2f}, ∞["
 
     def __repr__(self):
         return f"GreaterThan({self.lower:.2f})"
 
     def __eq__(self, other: GreaterThan) -> bool:
@@ -300,14 +323,17 @@
 
     def __init__(self, lowerbound: float, upperbound: float, standard: bool = True):
         super().__init__(lowerbound, upperbound, standard)
 
     def is_in(self, other: float) -> bool:
         return self.lower <= other < self.upper if self.standard else self.lower < other <= self.upper
 
+    def print(self) -> str:
+        return f"between {round(self.lower, 1)} and {round(self.upper, 1)}"
+
     def __str__(self):
         return ("[" if self.standard else "]") + f"{self.lower:.2f}, {self.upper:.2f}" + ("[" if self.standard else "]")
 
     def __repr__(self):
         return f"Between({self.lower:.2f}, {self.upper:.2f})"
 
 
@@ -315,14 +341,17 @@
 
     def __init__(self, lowerbound: float, upperbound: float, standard: bool = True):
         super().__init__(lowerbound, upperbound, standard)
 
     def is_in(self, other: float) -> bool:
         return other < self.lower or self.upper <= other if self.standard else other <= self.lower or self.upper < other
 
+    def print(self) -> str:
+        return f"not between {round(self.lower, 1)} and {round(self.upper, 1)}"
+
     def __str__(self):
         return f"]-∞, {self.lower:.2f}" + ("[" if self.standard else "]") + ' U '\
                + ("[" if self.standard else "]") + f"{self.upper:.2f}, ∞["
 
     def __repr__(self):
         return f"Outside({self.lower:.2f}, {self.upper:.2f})"
 
@@ -332,14 +361,17 @@
     def __init__(self, value: float):
         super().__init__()
         self.value = round(value, get_int_precision())
 
     def is_in(self, other: float) -> bool:
         return math.isclose(other, self.value)
 
+    def print(self) -> str:
+        return f"equal {round(self.value, 1)}"
+
     def __str__(self):
         return "{" + str(self.value) + "}"
 
     def __repr__(self):
         return f"Constant({self.value})"
```

### Comparing `psyke-0.8.3.dev2/psyke/tuning/__init__.py` & `psyke-0.8.4/psyke/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/tuning/crash/__init__.py` & `psyke-0.8.4/psyke/tuning/crash/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/tuning/orchid/__init__.py` & `psyke-0.8.4/psyke/tuning/orchid/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/tuning/pedro/__init__.py` & `psyke-0.8.4/psyke/tuning/pedro/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/utils/__init__.py` & `psyke-0.8.4/psyke/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/utils/dataframe.py` & `psyke-0.8.4/psyke/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/utils/logic.py` & `psyke-0.8.4/psyke/utils/logic.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/utils/metrics.py` & `psyke-0.8.4/psyke/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/utils/plot.py` & `psyke-0.8.4/psyke/utils/plot.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke/utils/sorted.py` & `psyke-0.8.4/psyke/utils/sorted.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/psyke.egg-info/PKG-INFO` & `psyke-0.8.4/psyke.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.8.3.dev2
+Version: 0.8.4
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.8.3.dev2/psyke.egg-info/SOURCES.txt` & `psyke-0.8.4/psyke.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/setup.py` & `psyke-0.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/test/psyke/__init__.py` & `psyke-0.8.4/test/psyke/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/test/psyke/extraction/cart/test_cart.py` & `psyke-0.8.4/test/psyke/extraction/cart/test_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/test/psyke/extraction/cart/test_simplified_cart.py` & `psyke-0.8.4/test/psyke/extraction/cart/test_simplified_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/test/psyke/extraction/hypercubic/gridex/test_gridex.py` & `psyke-0.8.4/test/psyke/extraction/hypercubic/gridex/test_gridex.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/test/psyke/extraction/hypercubic/iter/test_iter.py` & `psyke-0.8.4/test/psyke/extraction/hypercubic/iter/test_iter.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/test/psyke/extraction/hypercubic/test_hypercube.py` & `psyke-0.8.4/test/psyke/extraction/hypercubic/test_hypercube.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/test/psyke/extraction/real/test_real.py` & `psyke-0.8.4/test/psyke/extraction/real/test_real.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/test/psyke/extraction/real/test_rule.py` & `psyke-0.8.4/test/psyke/extraction/real/test_rule.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/test/psyke/extraction/trepan/test_node.py` & `psyke-0.8.4/test/psyke/extraction/trepan/test_node.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/test/psyke/extraction/trepan/test_split.py` & `psyke-0.8.4/test/psyke/extraction/trepan/test_split.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/test/psyke/extraction/trepan/test_trepan.py` & `psyke-0.8.4/test/psyke/extraction/trepan/test_trepan.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/test/psyke/utils/test_prune.py` & `psyke-0.8.4/test/psyke/utils/test_prune.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/test/psyke/utils/test_simplify.py` & `psyke-0.8.4/test/psyke/utils/test_simplify.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/test/psyke/utils/test_simplify_formatter.py` & `psyke-0.8.4/test/psyke/utils/test_simplify_formatter.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.3.dev2/test/resources/tests/__init__.py` & `psyke-0.8.4/test/resources/tests/__init__.py`

 * *Files identical despite different names*

