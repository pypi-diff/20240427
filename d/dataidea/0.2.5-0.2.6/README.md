# Comparing `tmp/dataidea-0.2.5.tar.gz` & `tmp/dataidea-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataidea-0.2.5.tar", max compression
+gzip compressed data, was "dataidea-0.2.6.tar", max compression
```

## Comparing `dataidea-0.2.5.tar` & `dataidea-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     7496 2024-04-21 19:53:53.642815 dataidea-0.2.5/README.md
--rw-r--r--   0        0        0      229 2024-04-19 06:31:05.013813 dataidea-0.2.5/dataidea/datasets/cluster.csv
--rw-r--r--   0        0        0     4645 2024-04-19 06:33:56.213774 dataidea-0.2.5/dataidea/datasets/demo.csv
--rw-r--r--   0        0        0    47391 2024-04-19 06:31:05.017817 dataidea-0.2.5/dataidea/datasets/fpl.csv
--rw-r--r--   0        0        0      370 2024-04-19 06:31:05.021821 dataidea-0.2.5/dataidea/datasets/homeprices.csv
--rw-r--r--   0        0        0  2091239 2024-04-19 06:31:05.025825 dataidea-0.2.5/dataidea/datasets/melbourne.csv
--rw-r--r--   0        0        0      302 2024-04-19 06:31:05.029829 dataidea-0.2.5/dataidea/datasets/music.csv
--rw-r--r--   0        0        0      656 2024-04-19 06:31:05.029829 dataidea-0.2.5/dataidea/datasets/salaries.csv
--rw-r--r--   0        0        0   108285 2024-04-19 06:31:05.029829 dataidea-0.2.5/dataidea/datasets/titanic.csv
--rw-r--r--   0        0        0  1355781 2024-04-19 06:31:05.033833 dataidea-0.2.5/dataidea/datasets/vgsales.csv
--rw-r--r--   0        0        0      217 2024-04-19 06:31:05.033833 dataidea-0.2.5/dataidea/datasets/weather.csv
--rw-r--r--   0        0        0     3767 2024-04-21 10:09:01.374308 dataidea-0.2.5/dataidea/datasets.py
--rw-r--r--   0        0        0      210 2024-04-19 05:07:03.723401 dataidea-0.2.5/dataidea/feature_selection.py
--rw-r--r--   0        0        0     2816 2024-04-21 19:11:14.394771 dataidea-0.2.5/dataidea/models.py
--rw-r--r--   0        0        0      167 2024-04-21 19:28:54.845536 dataidea-0.2.5/dataidea/packages.py
--rw-r--r--   0        0        0      284 2024-04-20 15:08:51.951883 dataidea-0.2.5/dataidea/statistics.py
--rw-r--r--   0        0        0      129 2024-04-23 19:34:49.942481 dataidea-0.2.5/dataidea/tabular.py
--rw-r--r--   0        0        0      481 2024-04-23 19:35:34.466480 dataidea-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     8295 1970-01-01 00:00:00.000000 dataidea-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     7496 2024-04-21 19:53:53.642815 dataidea-0.2.6/README.md
+-rw-r--r--   0        0        0      202 2024-04-27 09:53:08.511903 dataidea-0.2.6/dataidea/__init__.py
+-rw-r--r--   0        0        0      229 2024-04-19 06:31:05.013813 dataidea-0.2.6/dataidea/datasets/cluster.csv
+-rw-r--r--   0        0        0     4645 2024-04-19 06:33:56.213774 dataidea-0.2.6/dataidea/datasets/demo.csv
+-rw-r--r--   0        0        0    47391 2024-04-19 06:31:05.017817 dataidea-0.2.6/dataidea/datasets/fpl.csv
+-rw-r--r--   0        0        0      370 2024-04-19 06:31:05.021821 dataidea-0.2.6/dataidea/datasets/homeprices.csv
+-rw-r--r--   0        0        0     3780 2024-04-27 09:00:34.018881 dataidea-0.2.6/dataidea/datasets/mall.csv
+-rw-r--r--   0        0        0  2091239 2024-04-19 06:31:05.025825 dataidea-0.2.6/dataidea/datasets/melbourne.csv
+-rw-r--r--   0        0        0      302 2024-04-19 06:31:05.029829 dataidea-0.2.6/dataidea/datasets/music.csv
+-rw-r--r--   0        0        0      656 2024-04-19 06:31:05.029829 dataidea-0.2.6/dataidea/datasets/salaries.csv
+-rw-r--r--   0        0        0    41983 2024-04-27 09:39:55.284672 dataidea-0.2.6/dataidea/datasets/student-mat.csv
+-rw-r--r--   0        0        0    68558 2024-04-27 09:39:44.916354 dataidea-0.2.6/dataidea/datasets/student-por.csv
+-rw-r--r--   0        0        0   108285 2024-04-19 06:31:05.029829 dataidea-0.2.6/dataidea/datasets/titanic.csv
+-rw-r--r--   0        0        0  1355781 2024-04-19 06:31:05.033833 dataidea-0.2.6/dataidea/datasets/vgsales.csv
+-rw-r--r--   0        0        0      217 2024-04-19 06:31:05.033833 dataidea-0.2.6/dataidea/datasets/weather.csv
+-rw-r--r--   0        0        0     1030 2024-04-27 09:51:24.344571 dataidea-0.2.6/dataidea/datasets.py
+-rw-r--r--   0        0        0      167 2024-04-27 09:39:06.489400 dataidea-0.2.6/dataidea/packages.py
+-rw-r--r--   0        0        0      481 2024-04-27 09:44:14.426101 dataidea-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     8295 1970-01-01 00:00:00.000000 dataidea-0.2.6/PKG-INFO
```

### Comparing `dataidea-0.2.5/README.md` & `dataidea-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.5/dataidea/datasets/demo.csv` & `dataidea-0.2.6/dataidea/datasets/demo.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.5/dataidea/datasets/fpl.csv` & `dataidea-0.2.6/dataidea/datasets/fpl.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.5/dataidea/datasets/melbourne.csv` & `dataidea-0.2.6/dataidea/datasets/melbourne.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.5/dataidea/datasets/salaries.csv` & `dataidea-0.2.6/dataidea/datasets/salaries.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.5/dataidea/datasets/titanic.csv` & `dataidea-0.2.6/dataidea/datasets/titanic.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.5/dataidea/datasets/vgsales.csv` & `dataidea-0.2.6/dataidea/datasets/vgsales.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.5/PKG-INFO` & `dataidea-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataidea
-Version: 0.2.5
+Version: 0.2.6
 Summary: Package to ease data analysis for DATAIDEA students
 License: MIT
 Author: jumashafara
 Author-email: jumashafara0@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

