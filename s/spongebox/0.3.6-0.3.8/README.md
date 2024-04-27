# Comparing `tmp/spongebox-0.3.6.tar.gz` & `tmp/spongebox-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\spongebox-0.3.6.tar", last modified: Fri Dec  9 09:59:41 2022, max compression
+gzip compressed data, was "spongebox-0.3.8.tar", last modified: Sat Apr 27 10:57:39 2024, max compression
```

## Comparing `spongebox-0.3.6.tar` & `spongebox-0.3.8.tar`

### file list

```diff
@@ -1,50 +1,58 @@
-drwxrwxrwx   0        0        0        0 2022-12-09 09:59:41.000000 spongebox-0.3.6/
--rw-rw-rw-   0        0        0     1089 2020-10-15 09:00:37.000000 spongebox-0.3.6/LICENSE
--rw-rw-rw-   0        0        0      606 2022-12-09 09:59:41.000000 spongebox-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0       85 2020-10-15 08:59:47.000000 spongebox-0.3.6/README.md
--rw-rw-rw-   0        0        0       42 2022-12-09 09:59:41.000000 spongebox-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0      742 2022-12-09 09:58:00.000000 spongebox-0.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-09 09:59:41.000000 spongebox-0.3.6/spongebox/
--rw-rw-rw-   0        0        0        0 2020-04-21 01:47:49.000000 spongebox-0.3.6/spongebox/__init__.py
--rw-rw-rw-   0        0        0     1328 2020-04-20 11:29:01.000000 spongebox-0.3.6/spongebox/encoding.py
-drwxrwxrwx   0        0        0        0 2022-12-09 09:59:41.000000 spongebox-0.3.6/spongebox/financebox/
--rw-rw-rw-   0        0        0        0 2020-09-18 17:51:19.000000 spongebox-0.3.6/spongebox/financebox/__init__.py
--rw-rw-rw-   0        0        0     1701 2020-10-15 09:45:47.000000 spongebox-0.3.6/spongebox/financebox/loanbox.py
--rw-rw-rw-   0        0        0     5114 2020-09-20 09:13:34.000000 spongebox-0.3.6/spongebox/financebox/monetarybox.py
--rw-rw-rw-   0        0        0     3560 2021-10-23 12:27:36.000000 spongebox-0.3.6/spongebox/iobox.py
--rw-rw-rw-   0        0        0     2990 2020-10-24 13:29:42.000000 spongebox-0.3.6/spongebox/mediabox.py
--rw-rw-rw-   0        0        0     3300 2022-03-02 00:57:49.000000 spongebox-0.3.6/spongebox/plotbox.py
--rw-rw-rw-   0        0        0     1669 2022-12-09 09:56:14.000000 spongebox-0.3.6/spongebox/rebox.py
--rw-rw-rw-   0        0        0      108 2020-09-18 17:26:02.000000 spongebox-0.3.6/spongebox/structbox.py
--rw-rw-rw-   0        0        0     6383 2022-03-06 16:15:39.000000 spongebox-0.3.6/spongebox/timebox.py
-drwxrwxrwx   0        0        0        0 2022-12-09 09:59:41.000000 spongebox-0.3.6/spongebox.egg-info/
--rw-rw-rw-   0        0        0      606 2022-12-09 09:59:40.000000 spongebox-0.3.6/spongebox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1217 2022-12-09 09:59:40.000000 spongebox-0.3.6/spongebox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-09 09:59:40.000000 spongebox-0.3.6/spongebox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2022-12-09 09:59:40.000000 spongebox-0.3.6/spongebox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-12-09 09:59:41.000000 spongebox-0.3.6/spongeboxtest/
--rw-rw-rw-   0        0        0        0 2020-10-15 08:59:47.000000 spongebox-0.3.6/spongeboxtest/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-09 09:59:41.000000 spongebox-0.3.6/spongeboxtest/financeboxtest/
--rw-rw-rw-   0        0        0        0 2020-10-15 09:01:44.000000 spongebox-0.3.6/spongeboxtest/financeboxtest/__init__.py
--rw-rw-rw-   0        0        0      859 2020-10-15 11:27:29.000000 spongebox-0.3.6/spongeboxtest/financeboxtest/gen_repay_plan_test.py
-drwxrwxrwx   0        0        0        0 2022-12-09 09:59:41.000000 spongebox-0.3.6/spongeboxtest/ioboxtest/
--rw-rw-rw-   0        0        0        0 2020-11-11 14:42:29.000000 spongebox-0.3.6/spongeboxtest/ioboxtest/__init__.py
--rw-rw-rw-   0        0        0      701 2021-10-18 12:33:05.000000 spongebox-0.3.6/spongeboxtest/ioboxtest/list_dir_test.py
--rw-rw-rw-   0        0        0      344 2021-10-16 16:39:35.000000 spongebox-0.3.6/spongeboxtest/ioboxtest/mkdir_test.py
--rw-rw-rw-   0        0        0      316 2020-11-11 14:46:13.000000 spongebox-0.3.6/spongeboxtest/ioboxtest/read_overwrite_test.py
--rw-rw-rw-   0        0        0      552 2021-10-23 12:26:18.000000 spongebox-0.3.6/spongeboxtest/ioboxtest/to_excel_test.py
--rw-rw-rw-   0        0        0      507 2020-11-17 08:50:35.000000 spongebox-0.3.6/spongeboxtest/ioboxtest/zip_dir_test.py
-drwxrwxrwx   0        0        0        0 2022-12-09 09:59:41.000000 spongebox-0.3.6/spongeboxtest/mediaboxtest/
--rw-rw-rw-   0        0        0      383 2021-08-10 04:17:09.000000 spongebox-0.3.6/spongeboxtest/mediaboxtest/Tailortest.py
--rw-rw-rw-   0        0        0        0 2020-10-24 12:41:49.000000 spongebox-0.3.6/spongeboxtest/mediaboxtest/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-09 09:59:41.000000 spongebox-0.3.6/spongeboxtest/reboxtest/
--rw-rw-rw-   0        0        0        0 2020-11-17 09:56:45.000000 spongebox-0.3.6/spongeboxtest/reboxtest/__init__.py
--rw-rw-rw-   0        0        0      400 2020-11-17 09:56:20.000000 spongebox-0.3.6/spongeboxtest/reboxtest/filter_list_test.py
-drwxrwxrwx   0        0        0        0 2022-12-09 09:59:41.000000 spongebox-0.3.6/spongeboxtest/structboxtest/
--rw-rw-rw-   0        0        0        0 2020-10-24 12:41:49.000000 spongebox-0.3.6/spongeboxtest/structboxtest/__init__.py
--rw-rw-rw-   0        0        0      278 2020-10-24 12:41:49.000000 spongebox-0.3.6/spongeboxtest/structboxtest/flatten_list_test.py
-drwxrwxrwx   0        0        0        0 2022-12-09 09:59:41.000000 spongebox-0.3.6/spongeboxtest/timeboxtest/
--rw-rw-rw-   0        0        0        0 2020-10-15 08:59:47.000000 spongebox-0.3.6/spongeboxtest/timeboxtest/__init__.py
--rw-rw-rw-   0        0        0      626 2022-03-06 16:16:43.000000 spongebox-0.3.6/spongeboxtest/timeboxtest/chinesecalendar_test.py
--rw-rw-rw-   0        0        0      845 2020-10-15 08:59:47.000000 spongebox-0.3.6/spongeboxtest/timeboxtest/format_match_test.py
--rw-rw-rw-   0        0        0      392 2022-03-02 01:12:48.000000 spongebox-0.3.6/spongeboxtest/timeboxtest/strftime_test.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:57:39.466817 spongebox-0.3.8/
+-rw-rw-rw-   0        0        0     1089 2020-10-15 09:00:37.000000 spongebox-0.3.8/LICENSE
+-rw-rw-rw-   0        0        0      566 2024-04-27 10:57:39.459489 spongebox-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0       85 2020-10-15 08:59:47.000000 spongebox-0.3.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 10:57:39.468818 spongebox-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0      743 2024-04-27 10:45:00.000000 spongebox-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:57:39.207403 spongebox-0.3.8/spongebox/
+-rw-rw-rw-   0        0        0        0 2020-04-21 01:47:49.000000 spongebox-0.3.8/spongebox/__init__.py
+-rw-rw-rw-   0        0        0     1328 2020-04-20 11:29:01.000000 spongebox-0.3.8/spongebox/encoding.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:57:39.262816 spongebox-0.3.8/spongebox/financebox/
+-rw-rw-rw-   0        0        0        0 2020-09-18 17:51:19.000000 spongebox-0.3.8/spongebox/financebox/__init__.py
+-rw-rw-rw-   0        0        0     1701 2020-10-15 09:45:47.000000 spongebox-0.3.8/spongebox/financebox/loanbox.py
+-rw-rw-rw-   0        0        0     5114 2020-09-20 09:13:34.000000 spongebox-0.3.8/spongebox/financebox/monetarybox.py
+-rw-rw-rw-   0        0        0     3560 2021-10-23 12:27:36.000000 spongebox-0.3.8/spongebox/iobox.py
+-rw-rw-rw-   0        0        0     2242 2024-03-07 02:49:15.000000 spongebox-0.3.8/spongebox/loanbox.py
+-rw-rw-rw-   0        0        0     2990 2020-10-24 13:29:42.000000 spongebox-0.3.8/spongebox/mediabox.py
+-rw-rw-rw-   0        0        0    13752 2024-04-27 10:36:32.000000 spongebox-0.3.8/spongebox/plotbox.py
+-rw-rw-rw-   0        0        0     1669 2022-12-09 09:56:14.000000 spongebox-0.3.8/spongebox/rebox.py
+-rw-rw-rw-   0        0        0      108 2020-09-18 17:26:02.000000 spongebox-0.3.8/spongebox/structbox.py
+-rw-rw-rw-   0        0        0     6383 2022-03-06 16:15:39.000000 spongebox-0.3.8/spongebox/timebox.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:57:39.449817 spongebox-0.3.8/spongebox.egg-info/
+-rw-rw-rw-   0        0        0      566 2024-04-27 10:57:38.000000 spongebox-0.3.8/spongebox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1443 2024-04-27 10:57:39.000000 spongebox-0.3.8/spongebox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 10:57:38.000000 spongebox-0.3.8/spongebox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-27 10:57:38.000000 spongebox-0.3.8/spongebox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 10:57:39.270149 spongebox-0.3.8/spongeboxtest/
+-rw-rw-rw-   0        0        0        0 2020-10-15 08:59:47.000000 spongebox-0.3.8/spongeboxtest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:57:39.284005 spongebox-0.3.8/spongeboxtest/financeboxtest/
+-rw-rw-rw-   0        0        0        0 2020-10-15 09:01:44.000000 spongebox-0.3.8/spongeboxtest/financeboxtest/__init__.py
+-rw-rw-rw-   0        0        0      859 2020-10-15 11:27:29.000000 spongebox-0.3.8/spongeboxtest/financeboxtest/gen_repay_plan_test.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:57:39.330824 spongebox-0.3.8/spongeboxtest/ioboxtest/
+-rw-rw-rw-   0        0        0        0 2020-11-11 14:42:29.000000 spongebox-0.3.8/spongeboxtest/ioboxtest/__init__.py
+-rw-rw-rw-   0        0        0      701 2021-10-18 12:33:05.000000 spongebox-0.3.8/spongeboxtest/ioboxtest/list_dir_test.py
+-rw-rw-rw-   0        0        0      344 2021-10-16 16:39:35.000000 spongebox-0.3.8/spongeboxtest/ioboxtest/mkdir_test.py
+-rw-rw-rw-   0        0        0      316 2020-11-11 14:46:13.000000 spongebox-0.3.8/spongeboxtest/ioboxtest/read_overwrite_test.py
+-rw-rw-rw-   0        0        0      552 2021-10-23 12:26:18.000000 spongebox-0.3.8/spongeboxtest/ioboxtest/to_excel_test.py
+-rw-rw-rw-   0        0        0      507 2020-11-17 08:50:35.000000 spongebox-0.3.8/spongeboxtest/ioboxtest/zip_dir_test.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:57:39.355824 spongebox-0.3.8/spongeboxtest/loanboxtest/
+-rw-rw-rw-   0        0        0        0 2024-03-06 08:11:38.000000 spongebox-0.3.8/spongeboxtest/loanboxtest/__init__.py
+-rw-rw-rw-   0        0        0      395 2024-03-07 02:50:10.000000 spongebox-0.3.8/spongeboxtest/loanboxtest/profit_test.py
+-rw-rw-rw-   0        0        0      629 2024-03-06 09:15:52.000000 spongebox-0.3.8/spongeboxtest/loanboxtest/repayplan_test.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:57:39.371823 spongebox-0.3.8/spongeboxtest/mediaboxtest/
+-rw-rw-rw-   0        0        0      383 2021-08-10 04:17:09.000000 spongebox-0.3.8/spongeboxtest/mediaboxtest/Tailortest.py
+-rw-rw-rw-   0        0        0        0 2020-10-24 12:41:49.000000 spongebox-0.3.8/spongeboxtest/mediaboxtest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:57:39.383933 spongebox-0.3.8/spongeboxtest/plotboxtest/
+-rw-rw-rw-   0        0        0        0 2024-03-20 08:12:41.000000 spongebox-0.3.8/spongeboxtest/plotboxtest/__init__.py
+-rw-rw-rw-   0        0        0     1625 2024-03-26 07:29:45.000000 spongebox-0.3.8/spongeboxtest/plotboxtest/grid_plot_test.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:57:39.400820 spongebox-0.3.8/spongeboxtest/reboxtest/
+-rw-rw-rw-   0        0        0        0 2020-11-17 09:56:45.000000 spongebox-0.3.8/spongeboxtest/reboxtest/__init__.py
+-rw-rw-rw-   0        0        0      400 2020-11-17 09:56:20.000000 spongebox-0.3.8/spongeboxtest/reboxtest/filter_list_test.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:57:39.412822 spongebox-0.3.8/spongeboxtest/structboxtest/
+-rw-rw-rw-   0        0        0        0 2020-10-24 12:41:49.000000 spongebox-0.3.8/spongeboxtest/structboxtest/__init__.py
+-rw-rw-rw-   0        0        0      278 2020-10-24 12:41:49.000000 spongebox-0.3.8/spongeboxtest/structboxtest/flatten_list_test.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:57:39.440811 spongebox-0.3.8/spongeboxtest/timeboxtest/
+-rw-rw-rw-   0        0        0        0 2020-10-15 08:59:47.000000 spongebox-0.3.8/spongeboxtest/timeboxtest/__init__.py
+-rw-rw-rw-   0        0        0      626 2022-03-06 16:16:43.000000 spongebox-0.3.8/spongeboxtest/timeboxtest/chinesecalendar_test.py
+-rw-rw-rw-   0        0        0      845 2020-10-15 08:59:47.000000 spongebox-0.3.8/spongeboxtest/timeboxtest/format_match_test.py
+-rw-rw-rw-   0        0        0      392 2022-03-02 01:12:48.000000 spongebox-0.3.8/spongeboxtest/timeboxtest/strftime_test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `spongebox-0.3.6/LICENSE` & `spongebox-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spongebox-0.3.6/PKG-INFO` & `spongebox-0.3.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: spongebox
-Version: 0.3.6
+Version: 0.3.8
 Summary: A high-level wrapped tool-chest with frequently-used functionalities
 Home-page: https://github.com/23spongebob/spongebox
 Author: spongebob
 Author-email: author@example.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # spongebox
 A high-level wrapped tool-chest within frequently used functionalities
-
-
```

### Comparing `spongebox-0.3.6/setup.py` & `spongebox-0.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spongebox", # 届时使用pip install {}的包名
-    version="0.3.6",
+    version="0.3.8",
     author="spongebob",
     author_email="author@example.com",
     description="A high-level wrapped tool-chest with frequently-used functionalities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/23spongebob/spongebox",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.5',
+    python_requires='>=3.11',
 )
```

### Comparing `spongebox-0.3.6/spongebox/encoding.py` & `spongebox-0.3.8/spongebox/encoding.py`

 * *Files identical despite different names*

### Comparing `spongebox-0.3.6/spongebox/financebox/loanbox.py` & `spongebox-0.3.8/spongebox/financebox/loanbox.py`

 * *Files identical despite different names*

### Comparing `spongebox-0.3.6/spongebox/financebox/monetarybox.py` & `spongebox-0.3.8/spongebox/financebox/monetarybox.py`

 * *Files identical despite different names*

### Comparing `spongebox-0.3.6/spongebox/iobox.py` & `spongebox-0.3.8/spongebox/iobox.py`

 * *Files identical despite different names*

### Comparing `spongebox-0.3.6/spongebox/mediabox.py` & `spongebox-0.3.8/spongebox/mediabox.py`

 * *Files identical despite different names*

### Comparing `spongebox-0.3.6/spongebox/rebox.py` & `spongebox-0.3.8/spongebox/rebox.py`

 * *Files identical despite different names*

### Comparing `spongebox-0.3.6/spongebox/timebox.py` & `spongebox-0.3.8/spongebox/timebox.py`

 * *Files identical despite different names*

### Comparing `spongebox-0.3.6/spongebox.egg-info/PKG-INFO` & `spongebox-0.3.8/spongebox.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: spongebox
-Version: 0.3.6
+Version: 0.3.8
 Summary: A high-level wrapped tool-chest with frequently-used functionalities
 Home-page: https://github.com/23spongebob/spongebox
 Author: spongebob
 Author-email: author@example.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # spongebox
 A high-level wrapped tool-chest within frequently used functionalities
-
-
```

### Comparing `spongebox-0.3.6/spongebox.egg-info/SOURCES.txt` & `spongebox-0.3.8/spongebox.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.py
 spongebox/__init__.py
 spongebox/encoding.py
 spongebox/iobox.py
+spongebox/loanbox.py
 spongebox/mediabox.py
 spongebox/plotbox.py
 spongebox/rebox.py
 spongebox/structbox.py
 spongebox/timebox.py
 spongebox.egg-info/PKG-INFO
 spongebox.egg-info/SOURCES.txt
@@ -21,16 +22,21 @@
 spongeboxtest/financeboxtest/gen_repay_plan_test.py
 spongeboxtest/ioboxtest/__init__.py
 spongeboxtest/ioboxtest/list_dir_test.py
 spongeboxtest/ioboxtest/mkdir_test.py
 spongeboxtest/ioboxtest/read_overwrite_test.py
 spongeboxtest/ioboxtest/to_excel_test.py
 spongeboxtest/ioboxtest/zip_dir_test.py
+spongeboxtest/loanboxtest/__init__.py
+spongeboxtest/loanboxtest/profit_test.py
+spongeboxtest/loanboxtest/repayplan_test.py
 spongeboxtest/mediaboxtest/Tailortest.py
 spongeboxtest/mediaboxtest/__init__.py
+spongeboxtest/plotboxtest/__init__.py
+spongeboxtest/plotboxtest/grid_plot_test.py
 spongeboxtest/reboxtest/__init__.py
 spongeboxtest/reboxtest/filter_list_test.py
 spongeboxtest/structboxtest/__init__.py
 spongeboxtest/structboxtest/flatten_list_test.py
 spongeboxtest/timeboxtest/__init__.py
 spongeboxtest/timeboxtest/chinesecalendar_test.py
 spongeboxtest/timeboxtest/format_match_test.py
```

### Comparing `spongebox-0.3.6/spongeboxtest/financeboxtest/gen_repay_plan_test.py` & `spongebox-0.3.8/spongeboxtest/financeboxtest/gen_repay_plan_test.py`

 * *Files identical despite different names*

### Comparing `spongebox-0.3.6/spongeboxtest/ioboxtest/list_dir_test.py` & `spongebox-0.3.8/spongeboxtest/ioboxtest/list_dir_test.py`

 * *Files identical despite different names*

### Comparing `spongebox-0.3.6/spongeboxtest/ioboxtest/to_excel_test.py` & `spongebox-0.3.8/spongeboxtest/ioboxtest/to_excel_test.py`

 * *Files identical despite different names*

### Comparing `spongebox-0.3.6/spongeboxtest/timeboxtest/chinesecalendar_test.py` & `spongebox-0.3.8/spongeboxtest/timeboxtest/chinesecalendar_test.py`

 * *Files identical despite different names*

### Comparing `spongebox-0.3.6/spongeboxtest/timeboxtest/format_match_test.py` & `spongebox-0.3.8/spongeboxtest/timeboxtest/format_match_test.py`

 * *Files identical despite different names*

