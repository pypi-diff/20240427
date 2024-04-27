# Comparing `tmp/amjd-1.0.tar.gz` & `tmp/amjd-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amjd-1.0.tar", last modified: Sat Apr 27 20:36:26 2024, max compression
+gzip compressed data, was "amjd-1.1.tar", last modified: Sat Apr 27 20:45:00 2024, max compression
```

## Comparing `amjd-1.0.tar` & `amjd-1.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
-drwx------   0 u0_a472  (10472) u0_a472  (10472)        0 2024-04-27 20:36:26.311770 amjd-1.0/
--rw-r--r--   0 u0_a472  (10472) u0_a472  (10472)      147 2024-04-27 20:36:26.311770 amjd-1.0/PKG-INFO
-drwx------   0 u0_a472  (10472) u0_a472  (10472)        0 2024-04-27 20:36:26.311770 amjd-1.0/amjd.egg-info/
--rw-r--r--   0 u0_a472  (10472) u0_a472  (10472)      147 2024-04-27 20:36:26.000000 amjd-1.0/amjd.egg-info/PKG-INFO
--rw-------   0 u0_a472  (10472) u0_a472  (10472)      147 2024-04-27 20:36:26.000000 amjd-1.0/amjd.egg-info/SOURCES.txt
--rw-------   0 u0_a472  (10472) u0_a472  (10472)        1 2024-04-27 20:36:26.000000 amjd-1.0/amjd.egg-info/dependency_links.txt
--rw-------   0 u0_a472  (10472) u0_a472  (10472)        7 2024-04-27 20:36:26.000000 amjd-1.0/amjd.egg-info/requires.txt
--rw-------   0 u0_a472  (10472) u0_a472  (10472)        1 2024-04-27 20:36:26.000000 amjd-1.0/amjd.egg-info/top_level.txt
--rw-------   0 u0_a472  (10472) u0_a472  (10472)       38 2024-04-27 20:36:26.311770 amjd-1.0/setup.cfg
--rw-------   0 u0_a472  (10472) u0_a472  (10472)      270 2024-04-27 20:35:56.000000 amjd-1.0/setup.py
+drwx------   0 u0_a472  (10472) u0_a472  (10472)        0 2024-04-27 20:45:00.695770 amjd-1.1/
+-rw-r--r--   0 u0_a472  (10472) u0_a472  (10472)      125 2024-04-27 20:45:00.695770 amjd-1.1/PKG-INFO
+drwx------   0 u0_a472  (10472) u0_a472  (10472)        0 2024-04-27 20:45:00.695770 amjd-1.1/amjd.egg-info/
+-rw-r--r--   0 u0_a472  (10472) u0_a472  (10472)      125 2024-04-27 20:45:00.000000 amjd-1.1/amjd.egg-info/PKG-INFO
+-rw-------   0 u0_a472  (10472) u0_a472  (10472)      120 2024-04-27 20:45:00.000000 amjd-1.1/amjd.egg-info/SOURCES.txt
+-rw-------   0 u0_a472  (10472) u0_a472  (10472)        1 2024-04-27 20:45:00.000000 amjd-1.1/amjd.egg-info/dependency_links.txt
+-rw-------   0 u0_a472  (10472) u0_a472  (10472)        1 2024-04-27 20:45:00.000000 amjd-1.1/amjd.egg-info/top_level.txt
+-rw-------   0 u0_a472  (10472) u0_a472  (10472)       38 2024-04-27 20:45:00.695770 amjd-1.1/setup.cfg
+-rw-------   0 u0_a472  (10472) u0_a472  (10472)      266 2024-04-27 20:43:50.000000 amjd-1.1/setup.py
```

