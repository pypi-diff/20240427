# Comparing `tmp/nested_grid_plotter-1.1.1.tar.gz` & `tmp/nested_grid_plotter-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nested_grid_plotter-1.1.1.tar", last modified: Fri Mar 22 12:34:42 2024, max compression
+gzip compressed data, was "nested_grid_plotter-1.1.2.tar", last modified: Sat Apr 27 17:49:43 2024, max compression
```

## Comparing `nested_grid_plotter-1.1.1.tar` & `nested_grid_plotter-1.1.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2024-03-22 12:34:42.478572 nested_grid_plotter-1.1.1/
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      165 2021-11-09 14:28:03.000000 nested_grid_plotter-1.1.1/AUTHORS.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1356 2024-03-22 12:11:28.000000 nested_grid_plotter-1.1.1/CHANGELOG.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     5486 2023-06-30 21:33:38.000000 nested_grid_plotter-1.1.1/CONTRIBUTING.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1072 2024-01-31 15:44:45.000000 nested_grid_plotter-1.1.1/LICENSE
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      264 2021-11-09 14:28:03.000000 nested_grid_plotter-1.1.1/MANIFEST.in
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     6533 2024-03-22 12:34:42.478572 nested_grid_plotter-1.1.1/PKG-INFO
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     3055 2024-01-31 15:44:45.000000 nested_grid_plotter-1.1.1/README.rst
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2024-03-22 12:34:42.470573 nested_grid_plotter-1.1.1/docs/
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      624 2022-10-10 12:41:59.000000 nested_grid_plotter-1.1.1/docs/Makefile
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      787 2022-10-10 12:41:47.000000 nested_grid_plotter-1.1.1/docs/make.bat
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2024-03-22 12:34:42.470573 nested_grid_plotter-1.1.1/docs/source/
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2024-03-22 12:34:42.474573 nested_grid_plotter-1.1.1/docs/source/_static/
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     6924 2022-03-28 10:02:24.000000 nested_grid_plotter-1.1.1/docs/source/_static/index_api.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    17525 2022-03-28 10:02:40.000000 nested_grid_plotter-1.1.1/docs/source/_static/index_contribute.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    21639 2022-03-28 10:02:55.000000 nested_grid_plotter-1.1.1/docs/source/_static/index_getting_started.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    39514 2022-03-28 10:03:09.000000 nested_grid_plotter-1.1.1/docs/source/_static/index_user_guide.png
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2024-03-22 12:34:42.474573 nested_grid_plotter-1.1.1/docs/source/_templates/
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2024-03-22 12:34:42.474573 nested_grid_plotter-1.1.1/docs/source/_templates/autosummary/
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      106 2022-07-23 10:46:18.000000 nested_grid_plotter-1.1.1/docs/source/_templates/autosummary/base.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      735 2022-07-23 10:46:18.000000 nested_grid_plotter-1.1.1/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1098 2022-07-23 10:46:18.000000 nested_grid_plotter-1.1.1/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      735 2022-07-23 10:46:18.000000 nested_grid_plotter-1.1.1/docs/source/_templates/class.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1079 2022-07-23 10:46:18.000000 nested_grid_plotter-1.1.1/docs/source/_templates/custom-module-template.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1098 2022-07-23 10:46:18.000000 nested_grid_plotter-1.1.1/docs/source/_templates/module.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      121 2022-10-10 13:55:09.000000 nested_grid_plotter-1.1.1/docs/source/api_reference.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       31 2022-10-10 12:43:34.000000 nested_grid_plotter-1.1.1/docs/source/authors.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       33 2022-10-10 12:43:31.000000 nested_grid_plotter-1.1.1/docs/source/changelog.rst
--rwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)    13802 2024-01-31 15:44:45.000000 nested_grid_plotter-1.1.1/docs/source/conf.py
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       59 2022-10-10 12:43:42.000000 nested_grid_plotter-1.1.1/docs/source/contributing.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      336 2022-10-10 14:10:39.000000 nested_grid_plotter-1.1.1/docs/source/index.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1510 2023-06-30 21:34:49.000000 nested_grid_plotter-1.1.1/docs/source/installation.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      362 2022-10-10 13:53:10.000000 nested_grid_plotter-1.1.1/docs/source/user_guide.rst
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2024-03-22 12:34:42.474573 nested_grid_plotter-1.1.1/nested_grid_plotter/
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      125 2024-03-22 12:10:45.000000 nested_grid_plotter-1.1.1/nested_grid_plotter/__about__.py
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     2448 2024-03-22 11:04:56.000000 nested_grid_plotter-1.1.1/nested_grid_plotter/__init__.py
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    16773 2024-02-01 05:56:57.000000 nested_grid_plotter-1.1.1/nested_grid_plotter/animated_plotter.py
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    21318 2024-03-22 12:23:31.000000 nested_grid_plotter-1.1.1/nested_grid_plotter/base_plotter.py
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     9084 2024-03-01 18:25:50.000000 nested_grid_plotter-1.1.1/nested_grid_plotter/imshow.py
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    23444 2024-03-22 11:04:56.000000 nested_grid_plotter-1.1.1/nested_grid_plotter/utils.py
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2024-03-22 12:34:42.478572 nested_grid_plotter-1.1.1/nested_grid_plotter.egg-info/
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     6533 2024-03-22 12:34:42.000000 nested_grid_plotter-1.1.1/nested_grid_plotter.egg-info/PKG-INFO
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1343 2024-03-22 12:34:42.000000 nested_grid_plotter-1.1.1/nested_grid_plotter.egg-info/SOURCES.txt
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)        1 2024-03-22 12:34:42.000000 nested_grid_plotter-1.1.1/nested_grid_plotter.egg-info/dependency_links.txt
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)        1 2024-03-22 12:34:41.000000 nested_grid_plotter-1.1.1/nested_grid_plotter.egg-info/not-zip-safe
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       25 2024-03-22 12:34:42.000000 nested_grid_plotter-1.1.1/nested_grid_plotter.egg-info/requires.txt
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       26 2024-03-22 12:34:42.000000 nested_grid_plotter-1.1.1/nested_grid_plotter.egg-info/top_level.txt
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      142 2024-01-31 15:44:45.000000 nested_grid_plotter-1.1.1/pyproject.toml
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1545 2024-03-22 12:34:42.478572 nested_grid_plotter-1.1.1/setup.cfg
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2024-03-22 12:34:42.478572 nested_grid_plotter-1.1.1/tests/
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       49 2021-11-09 14:28:03.000000 nested_grid_plotter-1.1.1/tests/__init__.py
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    11923 2024-02-01 05:56:57.000000 nested_grid_plotter-1.1.1/tests/test_animated_plotter.py
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    19667 2024-03-22 10:41:10.000000 nested_grid_plotter-1.1.1/tests/test_base_plotter.py
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)        0 2022-08-04 11:34:40.000000 nested_grid_plotter-1.1.1/tests/test_examples.py
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     5873 2024-02-01 05:56:57.000000 nested_grid_plotter-1.1.1/tests/test_imshow.py
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    17406 2024-03-22 12:09:37.000000 nested_grid_plotter-1.1.1/tests/test_utils.py
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2024-04-27 17:49:43.938114 nested_grid_plotter-1.1.2/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      165 2021-11-09 14:28:03.000000 nested_grid_plotter-1.1.2/AUTHORS.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1449 2024-04-27 17:42:56.000000 nested_grid_plotter-1.1.2/CHANGELOG.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     5486 2023-06-30 21:33:38.000000 nested_grid_plotter-1.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1072 2024-01-31 15:44:45.000000 nested_grid_plotter-1.1.2/LICENSE
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      264 2021-11-09 14:28:03.000000 nested_grid_plotter-1.1.2/MANIFEST.in
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     6626 2024-04-27 17:49:43.938114 nested_grid_plotter-1.1.2/PKG-INFO
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     3055 2024-01-31 15:44:45.000000 nested_grid_plotter-1.1.2/README.rst
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2024-04-27 17:49:43.930114 nested_grid_plotter-1.1.2/docs/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      624 2022-10-10 12:41:59.000000 nested_grid_plotter-1.1.2/docs/Makefile
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      787 2022-10-10 12:41:47.000000 nested_grid_plotter-1.1.2/docs/make.bat
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2024-04-27 17:49:43.930114 nested_grid_plotter-1.1.2/docs/source/
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2024-04-27 17:49:43.930114 nested_grid_plotter-1.1.2/docs/source/_static/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     6924 2022-03-28 10:02:24.000000 nested_grid_plotter-1.1.2/docs/source/_static/index_api.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    17525 2022-03-28 10:02:40.000000 nested_grid_plotter-1.1.2/docs/source/_static/index_contribute.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    21639 2022-03-28 10:02:55.000000 nested_grid_plotter-1.1.2/docs/source/_static/index_getting_started.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    39514 2022-03-28 10:03:09.000000 nested_grid_plotter-1.1.2/docs/source/_static/index_user_guide.png
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2024-04-27 17:49:43.930114 nested_grid_plotter-1.1.2/docs/source/_templates/
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2024-04-27 17:49:43.930114 nested_grid_plotter-1.1.2/docs/source/_templates/autosummary/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      106 2022-07-23 10:46:18.000000 nested_grid_plotter-1.1.2/docs/source/_templates/autosummary/base.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      735 2022-07-23 10:46:18.000000 nested_grid_plotter-1.1.2/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1098 2022-07-23 10:46:18.000000 nested_grid_plotter-1.1.2/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      735 2022-07-23 10:46:18.000000 nested_grid_plotter-1.1.2/docs/source/_templates/class.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1079 2022-07-23 10:46:18.000000 nested_grid_plotter-1.1.2/docs/source/_templates/custom-module-template.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1098 2022-07-23 10:46:18.000000 nested_grid_plotter-1.1.2/docs/source/_templates/module.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      121 2022-10-10 13:55:09.000000 nested_grid_plotter-1.1.2/docs/source/api_reference.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       31 2022-10-10 12:43:34.000000 nested_grid_plotter-1.1.2/docs/source/authors.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       33 2022-10-10 12:43:31.000000 nested_grid_plotter-1.1.2/docs/source/changelog.rst
+-rwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)    13802 2024-01-31 15:44:45.000000 nested_grid_plotter-1.1.2/docs/source/conf.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       59 2022-10-10 12:43:42.000000 nested_grid_plotter-1.1.2/docs/source/contributing.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      336 2022-10-10 14:10:39.000000 nested_grid_plotter-1.1.2/docs/source/index.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1510 2023-06-30 21:34:49.000000 nested_grid_plotter-1.1.2/docs/source/installation.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      362 2022-10-10 13:53:10.000000 nested_grid_plotter-1.1.2/docs/source/user_guide.rst
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2024-04-27 17:49:43.934114 nested_grid_plotter-1.1.2/nested_grid_plotter/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      125 2024-04-27 17:19:20.000000 nested_grid_plotter-1.1.2/nested_grid_plotter/__about__.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     2448 2024-04-27 17:19:04.000000 nested_grid_plotter-1.1.2/nested_grid_plotter/__init__.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    16773 2024-04-27 17:00:11.000000 nested_grid_plotter-1.1.2/nested_grid_plotter/animated_plotter.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    21645 2024-04-27 17:19:05.000000 nested_grid_plotter-1.1.2/nested_grid_plotter/base_plotter.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     9084 2024-04-27 17:00:11.000000 nested_grid_plotter-1.1.2/nested_grid_plotter/imshow.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    23444 2024-04-27 17:19:04.000000 nested_grid_plotter-1.1.2/nested_grid_plotter/utils.py
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2024-04-27 17:49:43.938114 nested_grid_plotter-1.1.2/nested_grid_plotter.egg-info/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     6626 2024-04-27 17:49:43.000000 nested_grid_plotter-1.1.2/nested_grid_plotter.egg-info/PKG-INFO
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1343 2024-04-27 17:49:43.000000 nested_grid_plotter-1.1.2/nested_grid_plotter.egg-info/SOURCES.txt
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)        1 2024-04-27 17:49:43.000000 nested_grid_plotter-1.1.2/nested_grid_plotter.egg-info/dependency_links.txt
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)        1 2024-04-27 17:49:43.000000 nested_grid_plotter-1.1.2/nested_grid_plotter.egg-info/not-zip-safe
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       25 2024-04-27 17:49:43.000000 nested_grid_plotter-1.1.2/nested_grid_plotter.egg-info/requires.txt
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       26 2024-04-27 17:49:43.000000 nested_grid_plotter-1.1.2/nested_grid_plotter.egg-info/top_level.txt
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      142 2024-01-31 15:44:45.000000 nested_grid_plotter-1.1.2/pyproject.toml
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1545 2024-04-27 17:49:43.938114 nested_grid_plotter-1.1.2/setup.cfg
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2024-04-27 17:49:43.938114 nested_grid_plotter-1.1.2/tests/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       49 2021-11-09 14:28:03.000000 nested_grid_plotter-1.1.2/tests/__init__.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    11923 2024-04-27 17:00:11.000000 nested_grid_plotter-1.1.2/tests/test_animated_plotter.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    22781 2024-04-27 17:19:05.000000 nested_grid_plotter-1.1.2/tests/test_base_plotter.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)        0 2022-08-04 11:34:40.000000 nested_grid_plotter-1.1.2/tests/test_examples.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     5873 2024-04-27 17:00:11.000000 nested_grid_plotter-1.1.2/tests/test_imshow.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    17406 2024-04-27 17:19:04.000000 nested_grid_plotter-1.1.2/tests/test_utils.py
```

### Comparing `nested_grid_plotter-1.1.1/CHANGELOG.rst` & `nested_grid_plotter-1.1.2/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 ==============
 Changelog
 ==============
 
+1.1.2 (2024-04-27)
+------------------
+
+* FIX: bbox_extra_artists when using savefig method.
+
 1.1.1 (2024-03-22)
 ------------------
 
 * ENH: Add a `get_axes` interface to `NestedGridPlotter` class.
 * ENH: Provide a `add_letter_to_frames` utility function.
 * FIX: RunTimeError Can not put single artist in more than one figure when using
 * NestedGridPlotter `add_fig_legend` method and using the main figure.
```

### Comparing `nested_grid_plotter-1.1.1/CONTRIBUTING.rst` & `nested_grid_plotter-1.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/LICENSE` & `nested_grid_plotter-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/PKG-INFO` & `nested_grid_plotter-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nested_grid_plotter
-Version: 1.1.1
+Version: 1.1.2
 Summary: NestedGridPlotter is based on matplotlib and intends to simplify the plotting of nestedgrid by providing a objected oriented class.
 Home-page: https://github.com/antoinecollet5/nested_grid_plotter
 Author: attr: nested_grid_plotter.__author__
 Author-email: antoinecollet5@gmail.com
 License: MIT license
 Keywords: nested_grid_plotter,matplotlib,plotter,nested grid
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -86,14 +86,19 @@
 .. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.8215056.svg
    :target: https://doi.org/10.5281/zenodo.8215056
 
 ==============
 Changelog
 ==============
 
+1.1.2 (2024-04-27)
+------------------
+
+* FIX: bbox_extra_artists when using savefig method.
+
 1.1.1 (2024-03-22)
 ------------------
 
 * ENH: Add a `get_axes` interface to `NestedGridPlotter` class.
 * ENH: Provide a `add_letter_to_frames` utility function.
 * FIX: RunTimeError Can not put single artist in more than one figure when using
 * NestedGridPlotter `add_fig_legend` method and using the main figure.
```

### Comparing `nested_grid_plotter-1.1.1/README.rst` & `nested_grid_plotter-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/docs/Makefile` & `nested_grid_plotter-1.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/docs/make.bat` & `nested_grid_plotter-1.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/docs/source/_static/index_api.png` & `nested_grid_plotter-1.1.2/docs/source/_static/index_api.png`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/docs/source/_static/index_contribute.png` & `nested_grid_plotter-1.1.2/docs/source/_static/index_contribute.png`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/docs/source/_static/index_getting_started.png` & `nested_grid_plotter-1.1.2/docs/source/_static/index_getting_started.png`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/docs/source/_static/index_user_guide.png` & `nested_grid_plotter-1.1.2/docs/source/_static/index_user_guide.png`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/docs/source/_templates/autosummary/class.rst` & `nested_grid_plotter-1.1.2/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/docs/source/_templates/autosummary/module.rst` & `nested_grid_plotter-1.1.2/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/docs/source/_templates/class.rst` & `nested_grid_plotter-1.1.2/docs/source/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/docs/source/_templates/custom-module-template.rst` & `nested_grid_plotter-1.1.2/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/docs/source/_templates/module.rst` & `nested_grid_plotter-1.1.2/docs/source/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/docs/source/conf.py` & `nested_grid_plotter-1.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/docs/source/installation.rst` & `nested_grid_plotter-1.1.2/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/nested_grid_plotter/__init__.py` & `nested_grid_plotter-1.1.2/nested_grid_plotter/__init__.py`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/nested_grid_plotter/animated_plotter.py` & `nested_grid_plotter-1.1.2/nested_grid_plotter/animated_plotter.py`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/nested_grid_plotter/base_plotter.py` & `nested_grid_plotter-1.1.2/nested_grid_plotter/base_plotter.py`

 * *Files 4% similar despite different names*

```diff
@@ -312,23 +312,27 @@
         None
         """
         # Ensure that all artists are saved (nothing should be cropped)
         # https://stackoverflow.com/questions/9651092/my-matplotlib-pyplot-legend-is-being-cut-off/42303455
         bbox_inches = kwargs.pop("bbox_inches", "tight")
         # make sure that if a fig legend as been added, it won't be cutoff by
         # the figure box
-        kwargs.update(
-            {
-                "bbox_extra_artists": (
-                    *kwargs.get("bbox_extra_artists", ()),
-                    *self.fig.legends,
-                    *[lgd for fig in self.subfigs.values() for lgd in fig.legends],
-                )
-            }
-        )
+        bbox_extra_artists = [
+            *kwargs.get("bbox_extra_artists", ()),
+            *self.fig.legends,
+            *[lgd for fig in self.subfigs.values() for lgd in fig.legends],
+        ]
+        for fig in [self.fig, *self.subfigs.values()]:
+            if fig._supxlabel is not None:
+                bbox_extra_artists.append(fig._supxlabel)
+            if fig._supylabel is not None:
+                bbox_extra_artists.append(fig._supylabel)
+            if fig._suptitle is not None:
+                bbox_extra_artists.append(fig._suptitle)
+        kwargs.update({"bbox_extra_artists": tuple(bbox_extra_artists)})
         res = self.fig.savefig(*args, **kwargs, bbox_inches=bbox_inches)
         # need this if 'transparent=True' to reset colors
         self.fig.canvas.draw_idle()
         return res
 
     def identify_axes(self, fontsize: int = 48) -> None:
         """
```

### Comparing `nested_grid_plotter-1.1.1/nested_grid_plotter/imshow.py` & `nested_grid_plotter-1.1.2/nested_grid_plotter/imshow.py`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/nested_grid_plotter/utils.py` & `nested_grid_plotter-1.1.2/nested_grid_plotter/utils.py`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/nested_grid_plotter.egg-info/PKG-INFO` & `nested_grid_plotter-1.1.2/nested_grid_plotter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nested_grid_plotter
-Version: 1.1.1
+Version: 1.1.2
 Summary: NestedGridPlotter is based on matplotlib and intends to simplify the plotting of nestedgrid by providing a objected oriented class.
 Home-page: https://github.com/antoinecollet5/nested_grid_plotter
 Author: attr: nested_grid_plotter.__author__
 Author-email: antoinecollet5@gmail.com
 License: MIT license
 Keywords: nested_grid_plotter,matplotlib,plotter,nested grid
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -86,14 +86,19 @@
 .. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.8215056.svg
    :target: https://doi.org/10.5281/zenodo.8215056
 
 ==============
 Changelog
 ==============
 
+1.1.2 (2024-04-27)
+------------------
+
+* FIX: bbox_extra_artists when using savefig method.
+
 1.1.1 (2024-03-22)
 ------------------
 
 * ENH: Add a `get_axes` interface to `NestedGridPlotter` class.
 * ENH: Provide a `add_letter_to_frames` utility function.
 * FIX: RunTimeError Can not put single artist in more than one figure when using
 * NestedGridPlotter `add_fig_legend` method and using the main figure.
```

### Comparing `nested_grid_plotter-1.1.1/nested_grid_plotter.egg-info/SOURCES.txt` & `nested_grid_plotter-1.1.2/nested_grid_plotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/setup.cfg` & `nested_grid_plotter-1.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/tests/test_animated_plotter.py` & `nested_grid_plotter-1.1.2/tests/test_animated_plotter.py`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/tests/test_base_plotter.py` & `nested_grid_plotter-1.1.2/tests/test_base_plotter.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 Note that the tests are very similar to the examples found in the tutorial and
 follow the same order. The
 
 @author: Antoine COLLET
 """
 
+import struct
 from contextlib import contextmanager
 from itertools import product
 
 import numpy as np
 import pytest
 from matplotlib.axes import Axes
 from matplotlib.figure import SubFigure
@@ -309,24 +310,106 @@
                 "the_right_sub_figure": dict(
                     mosaic=[["ax21", "ax11"]],
                 ),
             },
         )
 
 
-def test_savefig(tmp_path_factory):
+def test_savefig(tmp_path_factory) -> None:
     tmp_folder = tmp_path_factory.mktemp("data")
     plotter = NestedGridPlotter()
     ax = plotter.ax_dict["ax1-1"]
     x = np.linspace(0, 2, 100)  # Sample data.
     ax.plot(x, x, label="linear")
     ax.legend()
+
     plotter.savefig(tmp_folder.joinpath("test_fig"))
 
 
+def test_savefif_with_legend(tmp_path_factory) -> None:
+    tmp_folder = tmp_path_factory.mktemp("data")
+
+    plotter = gen_complex_example_fig()
+    x = np.linspace(0, 2, 100)  # Sample data.
+    for ax_name, ax in plotter.ax_dict.items():
+        ax.plot(x, x, label=f"linear {ax_name}")  # Plot some data on the axes.
+        ax.plot(
+            x, x**2, label=f"quadratic {ax_name}"
+        )  # Plot more data on the axes...
+        ax.plot(x, x**3, label=f"cubic {ax_name}")  # ... and some more.
+
+    # Add some lines and spans and add it to the legend
+    handle = plotter.ax_dict["lt1"].axvline(
+        x=1.0, color="k", linewidth=3, linestyle="--"
+    )
+    plotter.add_extra_legend_item("lt1", handle, "My left extra legend item")
+
+    handle = plotter.ax_dict["lb1"].axvspan(xmin=0.25, xmax=0.75, color="yellow")
+    plotter.add_extra_legend_item("lt1", handle, "My left span")
+
+    handle = plotter.ax_dict["l2"].axhline(
+        y=4.0, xmin=0.2, xmax=0.8, color="r", linewidth=3, linestyle="--"
+    )
+    plotter.add_extra_legend_item("l2", handle, "My right extra legend item")
+
+    handle = plotter.ax_dict["l2"].axhspan(ymin=1.0, ymax=7.0, color="blue", alpha=0.3)
+    plotter.add_extra_legend_item("l2", handle, "My right span")
+
+    # Add the legend to subfigures (we place it to the bottom)
+    plotter.add_fig_legend(
+        name="the_left_sub_figure",
+        fontsize=10,
+        ncol=2,
+        bbox_x_shift=-0.25,
+        bbox_y_shift=-0.06,
+    )
+    plotter.add_fig_legend(
+        name="the_right_sub_figure",
+        fontsize=10,
+        ncol=2,
+        bbox_x_shift=+0.25,
+        bbox_y_shift=-0.06,
+    )
+
+    # Add a title
+    plotter.fig.suptitle("Main figure suptitle")
+    plotter.subfigs["the_left_sub_figure"].supxlabel("Left figure supxlabel")
+    plotter.subfigs["the_left_sub_figure"].supylabel("Left sub figure supylabel")
+
+    # Add the "full" fig legend just for the example (we place it to the top)
+    _ = plotter.add_fig_legend(fontsize=10, loc="top", ncol=4, bbox_y_shift=+0.06)
+
+    # Now we save the figure.
+    dpi = 72
+    savepath = tmp_folder.joinpath("with_plt_savefig.png")
+    # save the figure with matplotlib built-in method
+    plotter.fig.savefig(savepath, dpi=dpi)
+
+    # This size of the figure should be unchanged => the figure legends are ignored.
+    with open(savepath, "rb") as f:
+        data = f.read()
+    w, h = struct.unpack(">LL", data[16:24])
+    expected_fig_size = plotter.fig.get_size_inches()
+    np.testing.assert_equal(expected_fig_size * dpi, np.array([int(w), int(h)]))
+
+    # Now we use our implementation
+    savepath2 = tmp_folder.joinpath("with_plotter_savefig.png")
+    # save the figure
+    plotter.savefig(savepath2, dpi=dpi)
+
+    # Assert the size of the save figure with native python
+    with open(savepath2, "rb") as f2:
+        data2 = f2.read()
+    w2, h2 = struct.unpack(">LL", data2[16:24])
+    # The default behavior is to use tight_layout = True. So the added figure are taken
+    # into account and the figure size is increased.
+    assert int(w2) > int(w)
+    assert int(h2) > int(h)
+
+
 def test_close() -> None:
     plotter = NestedGridPlotter()
     plotter.close()
 
 
 def gen_complex_example_fig() -> NestedGridPlotter:
     return NestedGridPlotter(
```

### Comparing `nested_grid_plotter-1.1.1/tests/test_imshow.py` & `nested_grid_plotter-1.1.2/tests/test_imshow.py`

 * *Files identical despite different names*

### Comparing `nested_grid_plotter-1.1.1/tests/test_utils.py` & `nested_grid_plotter-1.1.2/tests/test_utils.py`

 * *Files identical despite different names*

