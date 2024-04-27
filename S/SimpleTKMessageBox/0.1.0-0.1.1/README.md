# Comparing `tmp/SimpleTKMessageBox-0.1.0.tar.gz` & `tmp/SimpleTKMessageBox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleTKMessageBox-0.1.0.tar", last modified: Sat Apr 27 10:27:54 2024, max compression
+gzip compressed data, was "SimpleTKMessageBox-0.1.1.tar", last modified: Sat Apr 27 10:37:01 2024, max compression
```

## Comparing `SimpleTKMessageBox-0.1.0.tar` & `SimpleTKMessageBox-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 10:27:54.448515 SimpleTKMessageBox-0.1.0/
--rw-rw-rw-   0        0        0      400 2024-04-27 10:27:54.445517 SimpleTKMessageBox-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-27 10:27:54.442518 SimpleTKMessageBox-0.1.0/SimpleTKMessageBox.egg-info/
--rw-rw-rw-   0        0        0      400 2024-04-27 10:27:54.000000 SimpleTKMessageBox-0.1.0/SimpleTKMessageBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-04-27 10:27:54.000000 SimpleTKMessageBox-0.1.0/SimpleTKMessageBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 10:27:54.000000 SimpleTKMessageBox-0.1.0/SimpleTKMessageBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-27 10:27:54.000000 SimpleTKMessageBox-0.1.0/SimpleTKMessageBox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-27 10:27:54.437521 SimpleTKMessageBox-0.1.0/SimpleTkMessageBox/
--rw-rw-rw-   0        0        0     3230 2024-04-27 10:00:48.000000 SimpleTKMessageBox-0.1.0/SimpleTkMessageBox/SimpleTkMessageBox.py
--rw-rw-rw-   0        0        0       59 2024-04-25 17:17:01.000000 SimpleTKMessageBox-0.1.0/SimpleTkMessageBox/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-27 10:27:54.448515 SimpleTKMessageBox-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      490 2024-04-27 10:05:28.000000 SimpleTKMessageBox-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:37:01.214576 SimpleTKMessageBox-0.1.1/
+-rw-rw-rw-   0        0        0      400 2024-04-27 10:37:01.211577 SimpleTKMessageBox-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-27 10:37:01.208578 SimpleTKMessageBox-0.1.1/SimpleTKMessageBox.egg-info/
+-rw-rw-rw-   0        0        0      400 2024-04-27 10:37:00.000000 SimpleTKMessageBox-0.1.1/SimpleTKMessageBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-04-27 10:37:01.000000 SimpleTKMessageBox-0.1.1/SimpleTKMessageBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 10:37:00.000000 SimpleTKMessageBox-0.1.1/SimpleTKMessageBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-27 10:37:00.000000 SimpleTKMessageBox-0.1.1/SimpleTKMessageBox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 10:37:01.202582 SimpleTKMessageBox-0.1.1/SimpleTkMessageBox/
+-rw-rw-rw-   0        0        0     3230 2024-04-27 10:00:48.000000 SimpleTKMessageBox-0.1.1/SimpleTkMessageBox/SimpleTkMessageBox.py
+-rw-rw-rw-   0        0        0       59 2024-04-27 10:36:23.000000 SimpleTKMessageBox-0.1.1/SimpleTkMessageBox/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-27 10:37:01.215575 SimpleTKMessageBox-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      490 2024-04-27 10:36:31.000000 SimpleTKMessageBox-0.1.1/setup.py
```

### Comparing `SimpleTKMessageBox-0.1.0/SimpleTkMessageBox/SimpleTkMessageBox.py` & `SimpleTKMessageBox-0.1.1/SimpleTkMessageBox/SimpleTkMessageBox.py`

 * *Files identical despite different names*

