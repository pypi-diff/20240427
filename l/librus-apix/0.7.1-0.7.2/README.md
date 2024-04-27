# Comparing `tmp/librus_apix-0.7.1.tar.gz` & `tmp/librus_apix-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librus_apix-0.7.1.tar", last modified: Fri Apr 26 09:33:58 2024, max compression
+gzip compressed data, was "librus_apix-0.7.2.tar", last modified: Sat Apr 27 12:51:02 2024, max compression
```

## Comparing `librus_apix-0.7.1.tar` & `librus_apix-0.7.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:33:58.098080 librus_apix-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-26 09:33:55.000000 librus_apix-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-26 09:33:58.098080 librus_apix-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-26 09:33:55.000000 librus_apix-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:33:58.098080 librus_apix-0.7.1/librus_apix/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-26 09:33:55.000000 librus_apix-0.7.1/librus_apix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-26 09:33:55.000000 librus_apix-0.7.1/librus_apix/announcements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-26 09:33:55.000000 librus_apix-0.7.1/librus_apix/attendance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-26 09:33:55.000000 librus_apix-0.7.1/librus_apix/completed_lessons.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-26 09:33:55.000000 librus_apix-0.7.1/librus_apix/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-26 09:33:55.000000 librus_apix-0.7.1/librus_apix/get_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     9541 2024-04-26 09:33:55.000000 librus_apix-0.7.1/librus_apix/grades.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-26 09:33:55.000000 librus_apix-0.7.1/librus_apix/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-26 09:33:55.000000 librus_apix-0.7.1/librus_apix/homework.py
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-04-26 09:33:55.000000 librus_apix-0.7.1/librus_apix/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-26 09:33:55.000000 librus_apix-0.7.1/librus_apix/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-26 09:33:55.000000 librus_apix-0.7.1/librus_apix/student_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-26 09:33:55.000000 librus_apix-0.7.1/librus_apix/timetable.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-26 09:33:55.000000 librus_apix-0.7.1/librus_apix/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:33:58.098080 librus_apix-0.7.1/librus_apix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-26 09:33:58.000000 librus_apix-0.7.1/librus_apix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-26 09:33:58.000000 librus_apix-0.7.1/librus_apix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:33:58.000000 librus_apix-0.7.1/librus_apix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 09:33:58.000000 librus_apix-0.7.1/librus_apix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 09:33:58.000000 librus_apix-0.7.1/librus_apix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-26 09:33:55.000000 librus_apix-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-26 09:33:58.098080 librus_apix-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 09:33:55.000000 librus_apix-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:51:02.499705 librus_apix-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-27 12:50:55.000000 librus_apix-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-27 12:51:02.499705 librus_apix-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-27 12:50:55.000000 librus_apix-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:51:02.495705 librus_apix-0.7.2/librus_apix/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/announcements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/attendance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/completed_lessons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/get_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9541 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/grades.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/homework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/student_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/timetable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:51:02.495705 librus_apix-0.7.2/librus_apix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-27 12:51:02.000000 librus_apix-0.7.2/librus_apix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-27 12:51:02.000000 librus_apix-0.7.2/librus_apix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 12:51:02.000000 librus_apix-0.7.2/librus_apix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 12:51:02.000000 librus_apix-0.7.2/librus_apix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-27 12:51:02.000000 librus_apix-0.7.2/librus_apix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-27 12:50:55.000000 librus_apix-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-27 12:51:02.499705 librus_apix-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 12:50:55.000000 librus_apix-0.7.2/setup.py
```

### Comparing `librus_apix-0.7.1/LICENSE` & `librus_apix-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.1/README.md` & `librus_apix-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.1/librus_apix/announcements.py` & `librus_apix-0.7.2/librus_apix/announcements.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.1/librus_apix/attendance.py` & `librus_apix-0.7.2/librus_apix/attendance.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.1/librus_apix/completed_lessons.py` & `librus_apix-0.7.2/librus_apix/completed_lessons.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.1/librus_apix/get_token.py` & `librus_apix-0.7.2/librus_apix/get_token.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.1/librus_apix/grades.py` & `librus_apix-0.7.2/librus_apix/grades.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.1/librus_apix/homework.py` & `librus_apix-0.7.2/librus_apix/homework.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.1/librus_apix/messages.py` & `librus_apix-0.7.2/librus_apix/messages.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.1/librus_apix/schedule.py` & `librus_apix-0.7.2/librus_apix/schedule.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.1/librus_apix/student_information.py` & `librus_apix-0.7.2/librus_apix/student_information.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.1/librus_apix/timetable.py` & `librus_apix-0.7.2/librus_apix/timetable.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.1/librus_apix/urls.py` & `librus_apix-0.7.2/librus_apix/urls.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.1/librus_apix.egg-info/SOURCES.txt` & `librus_apix-0.7.2/librus_apix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.1/setup.cfg` & `librus_apix-0.7.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [darglint]
 strictness = long
 docstring_style = google
 
 [metadata]
 name = librus_apix
-version = 0.7.1
+version = 0.7.2
 license = MIT
 description = Web Scraper for Librus Synergia
 long_description = ""
 author = Pascal Jodłowski
 url = https://github.com/poroknights/librus-apix
 keywords = librus, scraper, api, synergia
 classifiers =
```

