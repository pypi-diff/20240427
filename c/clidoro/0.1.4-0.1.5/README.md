# Comparing `tmp/clidoro-0.1.4.tar.gz` & `tmp/clidoro-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clidoro-0.1.4.tar", last modified: Mon Apr 22 05:37:52 2024, max compression
+gzip compressed data, was "clidoro-0.1.5.tar", last modified: Sat Apr 27 03:33:36 2024, max compression
```

## Comparing `clidoro-0.1.4.tar` & `clidoro-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-22 05:37:52.098888 clidoro-0.1.4/
--rw-rw-r--   0 juno      (1000) juno      (1000)     1065 2024-04-18 03:48:24.000000 clidoro-0.1.4/LICENSE.MD
--rw-r--r--   0 juno      (1000) juno      (1000)     2579 2024-04-22 05:37:52.098888 clidoro-0.1.4/PKG-INFO
--rw-rw-r--   0 juno      (1000) juno      (1000)     1343 2024-04-18 08:13:36.000000 clidoro-0.1.4/README.md
-drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-22 05:37:52.094888 clidoro-0.1.4/clidoro/
--rw-rw-r--   0 juno      (1000) juno      (1000)        0 2024-04-18 05:42:39.000000 clidoro-0.1.4/clidoro/__init__.py
--rw-rw-r--   0 juno      (1000) juno      (1000)     2870 2024-04-18 08:05:45.000000 clidoro-0.1.4/clidoro/_utils.py
--rw-rw-r--   0 juno      (1000) juno      (1000)     3903 2024-04-22 05:36:24.000000 clidoro-0.1.4/clidoro/chart.py
--rw-rw-r--   0 juno      (1000) juno      (1000)    57042 2024-04-18 07:45:05.000000 clidoro-0.1.4/clidoro/clidoro.png
--rw-------   0 juno      (1000) juno      (1000)     3717 2024-04-22 05:25:54.000000 clidoro-0.1.4/clidoro/clidoro.py
--rw-rw-r--   0 juno      (1000) juno      (1000)      642 2024-04-18 08:11:45.000000 clidoro-0.1.4/clidoro/data.py
-drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-22 05:37:52.098888 clidoro-0.1.4/clidoro/termgraph/
--rw-rw-r--   0 juno      (1000) juno      (1000)      205 2024-04-17 14:24:17.000000 clidoro-0.1.4/clidoro/termgraph/__init__.py
--rw-rw-r--   0 juno      (1000) juno      (1000)    24073 2024-04-17 14:20:38.000000 clidoro-0.1.4/clidoro/termgraph/_termgraph.py
--rw-rw-r--   0 juno      (1000) juno      (1000)    12733 2024-04-17 14:42:37.000000 clidoro-0.1.4/clidoro/termgraph/module.py
--rw-rw-r--   0 juno      (1000) juno      (1000)      546 2024-04-17 14:26:13.000000 clidoro-0.1.4/clidoro/termgraph/utils.py
-drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-22 05:37:52.098888 clidoro-0.1.4/clidoro.egg-info/
--rw-r--r--   0 juno      (1000) juno      (1000)     2579 2024-04-22 05:37:52.000000 clidoro-0.1.4/clidoro.egg-info/PKG-INFO
--rw-rw-r--   0 juno      (1000) juno      (1000)      484 2024-04-22 05:37:52.000000 clidoro-0.1.4/clidoro.egg-info/SOURCES.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)        1 2024-04-22 05:37:52.000000 clidoro-0.1.4/clidoro.egg-info/dependency_links.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)       49 2024-04-22 05:37:52.000000 clidoro-0.1.4/clidoro.egg-info/entry_points.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)        1 2024-04-18 04:35:24.000000 clidoro-0.1.4/clidoro.egg-info/not-zip-safe
--rw-rw-r--   0 juno      (1000) juno      (1000)       70 2024-04-22 05:37:52.000000 clidoro-0.1.4/clidoro.egg-info/requires.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)        8 2024-04-22 05:37:52.000000 clidoro-0.1.4/clidoro.egg-info/top_level.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)      102 2024-04-22 05:37:52.098888 clidoro-0.1.4/setup.cfg
--rw-rw-r--   0 juno      (1000) juno      (1000)     1887 2024-04-22 05:36:48.000000 clidoro-0.1.4/setup.py
+drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-27 03:33:36.489755 clidoro-0.1.5/
+-rw-rw-r--   0 juno      (1000) juno      (1000)     1065 2024-04-18 03:48:24.000000 clidoro-0.1.5/LICENSE.MD
+-rw-r--r--   0 juno      (1000) juno      (1000)     2579 2024-04-27 03:33:36.489755 clidoro-0.1.5/PKG-INFO
+-rw-rw-r--   0 juno      (1000) juno      (1000)     1343 2024-04-18 08:13:36.000000 clidoro-0.1.5/README.md
+drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-27 03:33:36.489755 clidoro-0.1.5/clidoro/
+-rw-rw-r--   0 juno      (1000) juno      (1000)        0 2024-04-18 05:42:39.000000 clidoro-0.1.5/clidoro/__init__.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)     2870 2024-04-18 08:05:45.000000 clidoro-0.1.5/clidoro/_utils.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)     3903 2024-04-27 03:32:34.000000 clidoro-0.1.5/clidoro/chart.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)    57042 2024-04-18 07:45:05.000000 clidoro-0.1.5/clidoro/clidoro.png
+-rw-------   0 juno      (1000) juno      (1000)     3777 2024-04-27 03:32:22.000000 clidoro-0.1.5/clidoro/clidoro.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)      642 2024-04-18 08:11:45.000000 clidoro-0.1.5/clidoro/data.py
+drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-27 03:33:36.489755 clidoro-0.1.5/clidoro/termgraph/
+-rw-rw-r--   0 juno      (1000) juno      (1000)      205 2024-04-17 14:24:17.000000 clidoro-0.1.5/clidoro/termgraph/__init__.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)    24073 2024-04-17 14:20:38.000000 clidoro-0.1.5/clidoro/termgraph/_termgraph.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)    12733 2024-04-17 14:42:37.000000 clidoro-0.1.5/clidoro/termgraph/module.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)      546 2024-04-17 14:26:13.000000 clidoro-0.1.5/clidoro/termgraph/utils.py
+drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-27 03:33:36.489755 clidoro-0.1.5/clidoro.egg-info/
+-rw-r--r--   0 juno      (1000) juno      (1000)     2579 2024-04-27 03:33:36.000000 clidoro-0.1.5/clidoro.egg-info/PKG-INFO
+-rw-rw-r--   0 juno      (1000) juno      (1000)      484 2024-04-27 03:33:36.000000 clidoro-0.1.5/clidoro.egg-info/SOURCES.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)        1 2024-04-27 03:33:36.000000 clidoro-0.1.5/clidoro.egg-info/dependency_links.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)       49 2024-04-27 03:33:36.000000 clidoro-0.1.5/clidoro.egg-info/entry_points.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)        1 2024-04-18 04:35:24.000000 clidoro-0.1.5/clidoro.egg-info/not-zip-safe
+-rw-rw-r--   0 juno      (1000) juno      (1000)       70 2024-04-27 03:33:36.000000 clidoro-0.1.5/clidoro.egg-info/requires.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)        8 2024-04-27 03:33:36.000000 clidoro-0.1.5/clidoro.egg-info/top_level.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)      102 2024-04-27 03:33:36.489755 clidoro-0.1.5/setup.cfg
+-rw-rw-r--   0 juno      (1000) juno      (1000)     1887 2024-04-27 03:32:47.000000 clidoro-0.1.5/setup.py
```

### Comparing `clidoro-0.1.4/LICENSE.MD` & `clidoro-0.1.5/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.4/PKG-INFO` & `clidoro-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clidoro
-Version: 0.1.4
+Version: 0.1.5
 Summary: clidoro: pomodoro in your cli
 Home-page: https://github.com/kingjuno/clidoro
 License: MIT
 Keywords: Productivity,Pomodoro
 Platform: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Customer Service
```

### Comparing `clidoro-0.1.4/README.md` & `clidoro-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.4/clidoro/_utils.py` & `clidoro-0.1.5/clidoro/_utils.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.4/clidoro/chart.py` & `clidoro-0.1.5/clidoro/chart.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.4/clidoro/clidoro.png` & `clidoro-0.1.5/clidoro/clidoro.png`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.4/clidoro/clidoro.py` & `clidoro-0.1.5/clidoro/clidoro.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     start_time = timestamp_to_datetime(time.time())
     while True:
         menu_entry_index = menu.show()
         if menu_entry_index == len(menu._menu_entries) - 1:
             break
         else:
             _time = times[menu_entry_index]
+            start_time = timestamp_to_datetime(time.time())
             stats = _timer(
                 _time, "simple-notification", CACHE_DIR, "pomodoro" if _save else "break"
             )
         if _save and stats > 0:
             save_to_db([[start_time, _time]], CACHE_DIR)
```

### Comparing `clidoro-0.1.4/clidoro/data.py` & `clidoro-0.1.5/clidoro/data.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.4/clidoro/termgraph/_termgraph.py` & `clidoro-0.1.5/clidoro/termgraph/_termgraph.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.4/clidoro/termgraph/module.py` & `clidoro-0.1.5/clidoro/termgraph/module.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.4/clidoro/termgraph/utils.py` & `clidoro-0.1.5/clidoro/termgraph/utils.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.4/clidoro.egg-info/PKG-INFO` & `clidoro-0.1.5/clidoro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clidoro
-Version: 0.1.4
+Version: 0.1.5
 Summary: clidoro: pomodoro in your cli
 Home-page: https://github.com/kingjuno/clidoro
 License: MIT
 Keywords: Productivity,Pomodoro
 Platform: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Customer Service
```

### Comparing `clidoro-0.1.4/setup.py` & `clidoro-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = "\n" + f.read()
 
 MAJOR_VERSION = "0"
 MINOR_VERSION = "1"
-MICRO_VERSION = "4"
+MICRO_VERSION = "5"
 VERSION = "{}.{}.{}".format(MAJOR_VERSION, MINOR_VERSION, MICRO_VERSION)
 
 
 setup(
     name="clidoro",
     packages=find_packages(exclude=["docs", "tests*", "examples"]),
     version=VERSION,
```

