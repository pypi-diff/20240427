# Comparing `tmp/srt_to_vtt-1.0.0.tar.gz` & `tmp/srt_to_vtt-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srt_to_vtt-1.0.0.tar", last modified: Thu Apr 25 20:32:41 2024, max compression
+gzip compressed data, was "srt_to_vtt-1.1.0.tar", last modified: Fri Apr 26 19:15:41 2024, max compression
```

## Comparing `srt_to_vtt-1.0.0.tar` & `srt_to_vtt-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-25 20:32:41.531621 srt_to_vtt-1.0.0/
--rw-r--r--   0 joshuahamilton   (501) staff       (20)     1071 2024-04-24 19:42:32.000000 srt_to_vtt-1.0.0/LICENSE
--rw-r--r--   0 joshuahamilton   (501) staff       (20)      451 2024-04-25 20:32:41.531418 srt_to_vtt-1.0.0/PKG-INFO
--rw-r--r--   0 joshuahamilton   (501) staff       (20)       69 2024-04-24 19:31:44.000000 srt_to_vtt-1.0.0/README.md
--rw-r--r--   0 joshuahamilton   (501) staff       (20)       38 2024-04-25 20:32:41.531665 srt_to_vtt-1.0.0/setup.cfg
--rw-r--r--   0 joshuahamilton   (501) staff       (20)      625 2024-04-25 20:31:21.000000 srt_to_vtt-1.0.0/setup.py
-drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-25 20:32:41.530310 srt_to_vtt-1.0.0/srt_to_vtt/
--rw-r--r--   0 joshuahamilton   (501) staff       (20)       34 2024-04-25 19:50:08.000000 srt_to_vtt-1.0.0/srt_to_vtt/__init__.py
--rw-r--r--   0 joshuahamilton   (501) staff       (20)      673 2024-04-25 20:19:22.000000 srt_to_vtt-1.0.0/srt_to_vtt/srt_to_vtt.py
-drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-25 20:32:41.531212 srt_to_vtt-1.0.0/srt_to_vtt.egg-info/
--rw-r--r--   0 joshuahamilton   (501) staff       (20)      451 2024-04-25 20:32:41.000000 srt_to_vtt-1.0.0/srt_to_vtt.egg-info/PKG-INFO
--rw-r--r--   0 joshuahamilton   (501) staff       (20)      235 2024-04-25 20:32:41.000000 srt_to_vtt-1.0.0/srt_to_vtt.egg-info/SOURCES.txt
--rw-r--r--   0 joshuahamilton   (501) staff       (20)        1 2024-04-25 20:32:41.000000 srt_to_vtt-1.0.0/srt_to_vtt.egg-info/dependency_links.txt
--rw-r--r--   0 joshuahamilton   (501) staff       (20)       11 2024-04-25 20:32:41.000000 srt_to_vtt-1.0.0/srt_to_vtt.egg-info/top_level.txt
-drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-25 20:32:41.530957 srt_to_vtt-1.0.0/tests/
--rw-r--r--   0 joshuahamilton   (501) staff       (20)      113 2024-04-25 20:15:33.000000 srt_to_vtt-1.0.0/tests/test_srt_to_vtt.py
+drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-26 19:15:41.706467 srt_to_vtt-1.1.0/
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)     1071 2024-04-24 19:42:32.000000 srt_to_vtt-1.1.0/LICENSE
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)     3272 2024-04-26 19:15:41.706238 srt_to_vtt-1.1.0/PKG-INFO
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)     1487 2024-04-26 19:14:04.000000 srt_to_vtt-1.1.0/README.md
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)      693 2024-04-26 19:14:21.000000 srt_to_vtt-1.1.0/pyproject.toml
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)       38 2024-04-26 19:15:41.707425 srt_to_vtt-1.1.0/setup.cfg
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)       37 2024-04-26 17:25:00.000000 srt_to_vtt-1.1.0/setup.py
+drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-26 19:15:41.705107 srt_to_vtt-1.1.0/srt_to_vtt/
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)       34 2024-04-25 19:50:08.000000 srt_to_vtt-1.1.0/srt_to_vtt/__init__.py
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)      673 2024-04-26 18:07:21.000000 srt_to_vtt-1.1.0/srt_to_vtt/srt_to_vtt.py
+drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-26 19:15:41.705996 srt_to_vtt-1.1.0/srt_to_vtt.egg-info/
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)     3272 2024-04-26 19:15:41.000000 srt_to_vtt-1.1.0/srt_to_vtt.egg-info/PKG-INFO
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)      250 2024-04-26 19:15:41.000000 srt_to_vtt-1.1.0/srt_to_vtt.egg-info/SOURCES.txt
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)        1 2024-04-26 19:15:41.000000 srt_to_vtt-1.1.0/srt_to_vtt.egg-info/dependency_links.txt
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)       11 2024-04-26 19:15:41.000000 srt_to_vtt-1.1.0/srt_to_vtt.egg-info/top_level.txt
+drwxr-xr-x   0 joshuahamilton   (501) staff       (20)        0 2024-04-26 19:15:41.705634 srt_to_vtt-1.1.0/tests/
+-rw-r--r--   0 joshuahamilton   (501) staff       (20)      653 2024-04-25 20:59:42.000000 srt_to_vtt-1.1.0/tests/test_srt_to_vtt.py
```

### Comparing `srt_to_vtt-1.0.0/LICENSE` & `srt_to_vtt-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `srt_to_vtt-1.0.0/srt_to_vtt/srt_to_vtt.py` & `srt_to_vtt-1.1.0/srt_to_vtt/srt_to_vtt.py`

 * *Files identical despite different names*

