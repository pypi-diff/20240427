# Comparing `tmp/wise_utils-1.1.1.tar.gz` & `tmp/wise_utils-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wise_utils-1.1.1.tar", last modified: Sat Apr 27 08:55:34 2024, max compression
+gzip compressed data, was "wise_utils-1.1.2.tar", last modified: Sat Apr 27 09:20:14 2024, max compression
```

## Comparing `wise_utils-1.1.1.tar` & `wise_utils-1.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 08:55:34.970656 wise_utils-1.1.1/
--rw-rw-rw-   0        0        0     1091 2022-09-17 11:47:05.000000 wise_utils-1.1.1/LICENSE
--rw-rw-rw-   0        0        0       44 2022-09-17 11:47:05.000000 wise_utils-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1678 2024-04-27 08:55:34.838679 wise_utils-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      857 2022-09-17 11:47:05.000000 wise_utils-1.1.1/README.md
--rw-rw-rw-   0        0        0      108 2022-09-17 11:47:05.000000 wise_utils-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-27 08:55:34.970656 wise_utils-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1186 2024-04-27 08:51:10.000000 wise_utils-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 08:55:33.650501 wise_utils-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-27 08:55:33.954331 wise_utils-1.1.1/src/wise_utils/
--rw-rw-rw-   0        0        0       58 2023-08-01 06:36:46.000000 wise_utils-1.1.1/src/wise_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 08:55:34.313770 wise_utils-1.1.1/src/wise_utils/common/
--rw-rw-rw-   0        0        0      324 2024-04-27 08:50:15.000000 wise_utils-1.1.1/src/wise_utils/common/__init__.py
--rw-rw-rw-   0        0        0      119 2022-10-08 02:17:40.000000 wise_utils-1.1.1/src/wise_utils/common/exceptions.py
--rw-rw-rw-   0        0        0     4488 2024-04-27 06:14:49.000000 wise_utils-1.1.1/src/wise_utils/common/ftp.py
--rw-rw-rw-   0        0        0     7684 2022-10-08 02:17:40.000000 wise_utils-1.1.1/src/wise_utils/common/log.py
--rw-rw-rw-   0        0        0     2425 2022-10-08 02:17:40.000000 wise_utils-1.1.1/src/wise_utils/common/retry_decorator.py
-drwxrwxrwx   0        0        0        0 2024-04-27 08:55:34.421584 wise_utils-1.1.1/src/wise_utils/db/
--rw-rw-rw-   0        0        0      185 2022-10-08 02:17:40.000000 wise_utils-1.1.1/src/wise_utils/db/__init__.py
--rw-rw-rw-   0        0        0    12291 2022-10-08 02:17:40.000000 wise_utils-1.1.1/src/wise_utils/db/db_mysql.py
--rw-rw-rw-   0        0        0      238 2022-10-08 02:17:40.000000 wise_utils-1.1.1/src/wise_utils/db/db_redis.py
-drwxrwxrwx   0        0        0        0 2024-04-27 08:55:34.750868 wise_utils-1.1.1/src/wise_utils/spider/
--rw-rw-rw-   0        0        0      194 2022-10-08 02:17:40.000000 wise_utils-1.1.1/src/wise_utils/spider/__init__.py
--rw-rw-rw-   0        0        0      475 2024-02-28 09:03:38.000000 wise_utils-1.1.1/src/wise_utils/spider/basespider.py
--rw-rw-rw-   0        0        0        2 2024-02-28 08:59:12.000000 wise_utils-1.1.1/src/wise_utils/spider/demo.py
--rw-rw-rw-   0        0        0    11814 2024-02-28 13:02:43.000000 wise_utils-1.1.1/src/wise_utils/spider/selenium_base_spider.py
--rw-rw-rw-   0        0        0    24625 2024-04-27 06:19:50.000000 wise_utils-1.1.1/src/wise_utils/spider/selenium_spider.py
--rw-rw-rw-   0        0        0   162046 2022-10-08 02:17:40.000000 wise_utils-1.1.1/src/wise_utils/spider/stealth.js
-drwxrwxrwx   0        0        0        0 2024-04-27 08:55:34.836733 wise_utils-1.1.1/src/wise_utils.egg-info/
--rw-rw-rw-   0        0        0     1678 2024-04-27 08:55:33.000000 wise_utils-1.1.1/src/wise_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      748 2024-04-27 08:55:33.000000 wise_utils-1.1.1/src/wise_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 08:55:33.000000 wise_utils-1.1.1/src/wise_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      180 2024-04-27 08:55:33.000000 wise_utils-1.1.1/src/wise_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-27 08:55:33.000000 wise_utils-1.1.1/src/wise_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 09:20:14.023737 wise_utils-1.1.2/
+-rw-rw-rw-   0        0        0     1091 2022-09-17 11:47:05.000000 wise_utils-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0       44 2022-09-17 11:47:05.000000 wise_utils-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1678 2024-04-27 09:20:14.023737 wise_utils-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      857 2022-09-17 11:47:05.000000 wise_utils-1.1.2/README.md
+-rw-rw-rw-   0        0        0      108 2022-09-17 11:47:05.000000 wise_utils-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-27 09:20:14.023737 wise_utils-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1186 2024-04-27 09:19:48.000000 wise_utils-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 09:20:13.990978 wise_utils-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-27 09:20:13.998767 wise_utils-1.1.2/src/wise_utils/
+-rw-rw-rw-   0        0        0       58 2023-08-01 06:36:46.000000 wise_utils-1.1.2/src/wise_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 09:20:14.010896 wise_utils-1.1.2/src/wise_utils/common/
+-rw-rw-rw-   0        0        0      324 2024-04-27 08:50:15.000000 wise_utils-1.1.2/src/wise_utils/common/__init__.py
+-rw-rw-rw-   0        0        0      119 2022-10-08 02:17:40.000000 wise_utils-1.1.2/src/wise_utils/common/exceptions.py
+-rw-rw-rw-   0        0        0     4488 2024-04-27 06:14:49.000000 wise_utils-1.1.2/src/wise_utils/common/ftp.py
+-rw-rw-rw-   0        0        0     7684 2022-10-08 02:17:40.000000 wise_utils-1.1.2/src/wise_utils/common/log.py
+-rw-rw-rw-   0        0        0     2425 2022-10-08 02:17:40.000000 wise_utils-1.1.2/src/wise_utils/common/retry_decorator.py
+drwxrwxrwx   0        0        0        0 2024-04-27 09:20:14.014793 wise_utils-1.1.2/src/wise_utils/db/
+-rw-rw-rw-   0        0        0      185 2022-10-08 02:17:40.000000 wise_utils-1.1.2/src/wise_utils/db/__init__.py
+-rw-rw-rw-   0        0        0    12291 2022-10-08 02:17:40.000000 wise_utils-1.1.2/src/wise_utils/db/db_mysql.py
+-rw-rw-rw-   0        0        0      238 2022-10-08 02:17:40.000000 wise_utils-1.1.2/src/wise_utils/db/db_redis.py
+drwxrwxrwx   0        0        0        0 2024-04-27 09:20:14.019838 wise_utils-1.1.2/src/wise_utils/spider/
+-rw-rw-rw-   0        0        0      194 2022-10-08 02:17:40.000000 wise_utils-1.1.2/src/wise_utils/spider/__init__.py
+-rw-rw-rw-   0        0        0      473 2024-04-27 09:18:37.000000 wise_utils-1.1.2/src/wise_utils/spider/basespider.py
+-rw-rw-rw-   0        0        0        2 2024-02-28 08:59:12.000000 wise_utils-1.1.2/src/wise_utils/spider/demo.py
+-rw-rw-rw-   0        0        0    11814 2024-02-28 13:02:43.000000 wise_utils-1.1.2/src/wise_utils/spider/selenium_base_spider.py
+-rw-rw-rw-   0        0        0    24625 2024-04-27 06:19:50.000000 wise_utils-1.1.2/src/wise_utils/spider/selenium_spider.py
+-rw-rw-rw-   0        0        0   162046 2022-10-08 02:17:40.000000 wise_utils-1.1.2/src/wise_utils/spider/stealth.js
+drwxrwxrwx   0        0        0        0 2024-04-27 09:20:14.021791 wise_utils-1.1.2/src/wise_utils.egg-info/
+-rw-rw-rw-   0        0        0     1678 2024-04-27 09:20:13.000000 wise_utils-1.1.2/src/wise_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      748 2024-04-27 09:20:13.000000 wise_utils-1.1.2/src/wise_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 09:20:13.000000 wise_utils-1.1.2/src/wise_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      180 2024-04-27 09:20:13.000000 wise_utils-1.1.2/src/wise_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-27 09:20:13.000000 wise_utils-1.1.2/src/wise_utils.egg-info/top_level.txt
```

### Comparing `wise_utils-1.1.1/LICENSE` & `wise_utils-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wise_utils-1.1.1/PKG-INFO` & `wise_utils-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wise-utils
-Version: 1.1.1
+Version: 1.1.2
 Home-page: http://code.wise-inc.com/spider/wise-utils.git
 Author: wise-python
 Author-email: duke.du@uifox.com.cn
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wise_utils-1.1.1/README.md` & `wise_utils-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `wise_utils-1.1.1/setup.py` & `wise_utils-1.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-VERSION = "1.1.1"
+VERSION = "1.1.2"
 
 setuptools.setup(
     name="wise-utils",
     version=VERSION,
     author="wise-python",
     author_email="duke.du@uifox.com.cn",
     description="",
```

### Comparing `wise_utils-1.1.1/src/wise_utils/common/ftp.py` & `wise_utils-1.1.2/src/wise_utils/common/ftp.py`

 * *Files identical despite different names*

### Comparing `wise_utils-1.1.1/src/wise_utils/common/log.py` & `wise_utils-1.1.2/src/wise_utils/common/log.py`

 * *Files identical despite different names*

### Comparing `wise_utils-1.1.1/src/wise_utils/common/retry_decorator.py` & `wise_utils-1.1.2/src/wise_utils/common/retry_decorator.py`

 * *Files identical despite different names*

### Comparing `wise_utils-1.1.1/src/wise_utils/db/db_mysql.py` & `wise_utils-1.1.2/src/wise_utils/db/db_mysql.py`

 * *Files identical despite different names*

### Comparing `wise_utils-1.1.1/src/wise_utils/spider/selenium_base_spider.py` & `wise_utils-1.1.2/src/wise_utils/spider/selenium_base_spider.py`

 * *Files identical despite different names*

### Comparing `wise_utils-1.1.1/src/wise_utils/spider/selenium_spider.py` & `wise_utils-1.1.2/src/wise_utils/spider/selenium_spider.py`

 * *Files identical despite different names*

### Comparing `wise_utils-1.1.1/src/wise_utils/spider/stealth.js` & `wise_utils-1.1.2/src/wise_utils/spider/stealth.js`

 * *Files identical despite different names*

### Comparing `wise_utils-1.1.1/src/wise_utils.egg-info/PKG-INFO` & `wise_utils-1.1.2/src/wise_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wise-utils
-Version: 1.1.1
+Version: 1.1.2
 Home-page: http://code.wise-inc.com/spider/wise-utils.git
 Author: wise-python
 Author-email: duke.du@uifox.com.cn
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wise_utils-1.1.1/src/wise_utils.egg-info/SOURCES.txt` & `wise_utils-1.1.2/src/wise_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

