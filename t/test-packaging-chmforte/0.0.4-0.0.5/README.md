# Comparing `tmp/test_packaging_chmforte-0.0.4.tar.gz` & `tmp/test_packaging_chmforte-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_packaging_chmforte-0.0.4.tar", last modified: Wed Sep 14 03:00:30 2022, max compression
+gzip compressed data, was "test_packaging_chmforte-0.0.5.tar", last modified: Sat Apr 27 15:51:20 2024, max compression
```

## Comparing `test_packaging_chmforte-0.0.4.tar` & `test_packaging_chmforte-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 cforte    (1000) cforte    (1000)        0 2022-09-14 03:00:30.958164 test_packaging_chmforte-0.0.4/
--rw-rw-r--   0 cforte    (1000) cforte    (1000)     1069 2022-09-14 02:49:18.000000 test_packaging_chmforte-0.0.4/LICENSE
--rw-rw-r--   0 cforte    (1000) cforte    (1000)      483 2022-09-14 03:00:30.958164 test_packaging_chmforte-0.0.4/PKG-INFO
--rw-rw-r--   0 cforte    (1000) cforte    (1000)       17 2022-09-14 02:48:28.000000 test_packaging_chmforte-0.0.4/README.md
--rw-rw-r--   0 cforte    (1000) cforte    (1000)      458 2022-09-14 02:59:39.000000 test_packaging_chmforte-0.0.4/pyproject.toml
--rw-rw-r--   0 cforte    (1000) cforte    (1000)       38 2022-09-14 03:00:30.958164 test_packaging_chmforte-0.0.4/setup.cfg
-drwxrwxr-x   0 cforte    (1000) cforte    (1000)        0 2022-09-14 03:00:30.958164 test_packaging_chmforte-0.0.4/test_packaging_chmforte/
--rw-rw-r--   0 cforte    (1000) cforte    (1000)        0 2022-09-12 02:19:56.000000 test_packaging_chmforte-0.0.4/test_packaging_chmforte/__init__.py
--rw-rw-r--   0 cforte    (1000) cforte    (1000)       43 2022-09-12 02:20:02.000000 test_packaging_chmforte-0.0.4/test_packaging_chmforte/example.py
-drwxrwxr-x   0 cforte    (1000) cforte    (1000)        0 2022-09-14 03:00:30.958164 test_packaging_chmforte-0.0.4/test_packaging_chmforte.egg-info/
--rw-rw-r--   0 cforte    (1000) cforte    (1000)      483 2022-09-14 03:00:30.000000 test_packaging_chmforte-0.0.4/test_packaging_chmforte.egg-info/PKG-INFO
--rw-rw-r--   0 cforte    (1000) cforte    (1000)      291 2022-09-14 03:00:30.000000 test_packaging_chmforte-0.0.4/test_packaging_chmforte.egg-info/SOURCES.txt
--rw-rw-r--   0 cforte    (1000) cforte    (1000)        1 2022-09-14 03:00:30.000000 test_packaging_chmforte-0.0.4/test_packaging_chmforte.egg-info/dependency_links.txt
--rw-rw-r--   0 cforte    (1000) cforte    (1000)       24 2022-09-14 03:00:30.000000 test_packaging_chmforte-0.0.4/test_packaging_chmforte.egg-info/top_level.txt
+drwxr-xr-x   0 chrisforte   (501) staff       (20)        0 2024-04-27 15:51:20.195442 test_packaging_chmforte-0.0.5/
+-rw-r--r--   0 chrisforte   (501) staff       (20)     1069 2024-04-27 15:16:33.000000 test_packaging_chmforte-0.0.5/LICENSE
+-rw-r--r--   0 chrisforte   (501) staff       (20)      483 2024-04-27 15:51:20.194948 test_packaging_chmforte-0.0.5/PKG-INFO
+-rw-r--r--   0 chrisforte   (501) staff       (20)       17 2024-04-27 15:16:33.000000 test_packaging_chmforte-0.0.5/README.md
+-rw-r--r--   0 chrisforte   (501) staff       (20)      516 2024-04-27 15:50:20.000000 test_packaging_chmforte-0.0.5/pyproject.toml
+-rw-r--r--   0 chrisforte   (501) staff       (20)       38 2024-04-27 15:51:20.195563 test_packaging_chmforte-0.0.5/setup.cfg
+drwxr-xr-x   0 chrisforte   (501) staff       (20)        0 2024-04-27 15:51:20.192358 test_packaging_chmforte-0.0.5/test_packaging_chmforte/
+-rw-r--r--   0 chrisforte   (501) staff       (20)        0 2024-04-27 15:02:04.000000 test_packaging_chmforte-0.0.5/test_packaging_chmforte/__init__.py
+-rw-r--r--   0 chrisforte   (501) staff       (20)      112 2024-04-27 15:51:16.000000 test_packaging_chmforte-0.0.5/test_packaging_chmforte/example.py
+drwxr-xr-x   0 chrisforte   (501) staff       (20)        0 2024-04-27 15:51:20.194379 test_packaging_chmforte-0.0.5/test_packaging_chmforte.egg-info/
+-rw-r--r--   0 chrisforte   (501) staff       (20)      483 2024-04-27 15:51:20.000000 test_packaging_chmforte-0.0.5/test_packaging_chmforte.egg-info/PKG-INFO
+-rw-r--r--   0 chrisforte   (501) staff       (20)      291 2024-04-27 15:51:20.000000 test_packaging_chmforte-0.0.5/test_packaging_chmforte.egg-info/SOURCES.txt
+-rw-r--r--   0 chrisforte   (501) staff       (20)        1 2024-04-27 15:51:20.000000 test_packaging_chmforte-0.0.5/test_packaging_chmforte.egg-info/dependency_links.txt
+-rw-r--r--   0 chrisforte   (501) staff       (20)       24 2024-04-27 15:51:20.000000 test_packaging_chmforte-0.0.5/test_packaging_chmforte.egg-info/top_level.txt
```

### Comparing `test_packaging_chmforte-0.0.4/LICENSE` & `test_packaging_chmforte-0.0.5/LICENSE`

 * *Files identical despite different names*

