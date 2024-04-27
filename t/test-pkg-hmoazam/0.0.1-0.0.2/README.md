# Comparing `tmp/test_pkg_hmoazam-0.0.1.tar.gz` & `tmp/test_pkg_hmoazam-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_pkg_hmoazam-0.0.1.tar", last modified: Sat Apr 27 20:05:40 2024, max compression
+gzip compressed data, was "test_pkg_hmoazam-0.0.2.tar", last modified: Sun Apr 14 18:26:49 2024, max compression
```

## Comparing `test_pkg_hmoazam-0.0.1.tar` & `test_pkg_hmoazam-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,15 @@
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 20:05:40.525355 test_pkg_hmoazam-0.0.1/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     6148 2024-04-14 20:12:34.000000 test_pkg_hmoazam-0.0.1/.DS_Store
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 20:05:40.519173 test_pkg_hmoazam-0.0.1/.github/
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 20:05:40.522014 test_pkg_hmoazam-0.0.1/.github/workflows/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     2644 2024-04-27 20:05:19.000000 test_pkg_hmoazam-0.0.1/.github/workflows/publish-to-test.pypi.yaml
--rw-r--r--   0 hanna.moazam   (502) staff       (20)       30 2024-04-14 19:38:59.000000 test_pkg_hmoazam-0.0.1/.gitignore
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     1073 2024-04-11 21:29:46.000000 test_pkg_hmoazam-0.0.1/LICENSE
--rw-r--r--   0 hanna.moazam   (502) staff       (20)      188 2024-04-27 20:05:40.525013 test_pkg_hmoazam-0.0.1/PKG-INFO
--rw-r--r--   0 hanna.moazam   (502) staff       (20)       22 2024-04-11 21:29:08.000000 test_pkg_hmoazam-0.0.1/README.md
--rw-r--r--   0 hanna.moazam   (502) staff       (20)      279 2024-04-27 20:05:31.000000 test_pkg_hmoazam-0.0.1/pyproject.toml
--rw-r--r--   0 hanna.moazam   (502) staff       (20)       38 2024-04-27 20:05:40.525403 test_pkg_hmoazam-0.0.1/setup.cfg
--rw-r--r--   0 hanna.moazam   (502) staff       (20)      293 2024-04-27 20:05:28.000000 test_pkg_hmoazam-0.0.1/setup.py
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 20:05:40.522590 test_pkg_hmoazam-0.0.1/test_pkg_hmoazam/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)       20 2024-04-10 00:51:15.000000 test_pkg_hmoazam-0.0.1/test_pkg_hmoazam/__init__.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)       43 2024-04-10 00:57:09.000000 test_pkg_hmoazam-0.0.1/test_pkg_hmoazam/hello.py
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 20:05:40.524580 test_pkg_hmoazam-0.0.1/test_pkg_hmoazam.egg-info/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)      188 2024-04-27 20:05:40.000000 test_pkg_hmoazam-0.0.1/test_pkg_hmoazam.egg-info/PKG-INFO
--rw-r--r--   0 hanna.moazam   (502) staff       (20)      321 2024-04-27 20:05:40.000000 test_pkg_hmoazam-0.0.1/test_pkg_hmoazam.egg-info/SOURCES.txt
--rw-r--r--   0 hanna.moazam   (502) staff       (20)        1 2024-04-27 20:05:40.000000 test_pkg_hmoazam-0.0.1/test_pkg_hmoazam.egg-info/dependency_links.txt
--rw-r--r--   0 hanna.moazam   (502) staff       (20)       17 2024-04-27 20:05:40.000000 test_pkg_hmoazam-0.0.1/test_pkg_hmoazam.egg-info/top_level.txt
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-14 18:26:49.957569 test_pkg_hmoazam-0.0.2/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     1073 2024-04-11 21:29:46.000000 test_pkg_hmoazam-0.0.2/LICENSE
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)      188 2024-04-14 18:26:49.957175 test_pkg_hmoazam-0.0.2/PKG-INFO
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)       22 2024-04-11 21:29:08.000000 test_pkg_hmoazam-0.0.2/README.md
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)      279 2024-04-14 18:26:12.000000 test_pkg_hmoazam-0.0.2/pyproject.toml
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)       38 2024-04-14 18:26:49.957638 test_pkg_hmoazam-0.0.2/setup.cfg
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)      172 2024-04-14 18:26:46.000000 test_pkg_hmoazam-0.0.2/setup.py
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-14 18:26:49.955222 test_pkg_hmoazam-0.0.2/test_pkg_hmoazam/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)       20 2024-04-10 00:51:15.000000 test_pkg_hmoazam-0.0.2/test_pkg_hmoazam/__init__.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)       43 2024-04-10 00:57:09.000000 test_pkg_hmoazam-0.0.2/test_pkg_hmoazam/hello.py
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-14 18:26:49.956770 test_pkg_hmoazam-0.0.2/test_pkg_hmoazam.egg-info/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)      188 2024-04-14 18:26:49.000000 test_pkg_hmoazam-0.0.2/test_pkg_hmoazam.egg-info/PKG-INFO
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)      256 2024-04-14 18:26:49.000000 test_pkg_hmoazam-0.0.2/test_pkg_hmoazam.egg-info/SOURCES.txt
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)        1 2024-04-14 18:26:49.000000 test_pkg_hmoazam-0.0.2/test_pkg_hmoazam.egg-info/dependency_links.txt
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)       17 2024-04-14 18:26:49.000000 test_pkg_hmoazam-0.0.2/test_pkg_hmoazam.egg-info/top_level.txt
```

### Comparing `test_pkg_hmoazam-0.0.1/LICENSE` & `test_pkg_hmoazam-0.0.2/LICENSE`

 * *Files identical despite different names*

