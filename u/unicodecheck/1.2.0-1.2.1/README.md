# Comparing `tmp/unicodecheck-1.2.0.tar.gz` & `tmp/unicodecheck-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicodecheck-1.2.0.tar", last modified: Thu Apr 11 15:48:38 2024, max compression
+gzip compressed data, was "unicodecheck-1.2.1.tar", last modified: Sat Apr 27 17:41:21 2024, max compression
```

## Comparing `unicodecheck-1.2.0.tar` & `unicodecheck-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-04-11 15:48:38.455134 unicodecheck-1.2.0/
--rw-r--r--   0 shunsuke   (501) staff       (20)     1064 2023-10-24 08:35:07.000000 unicodecheck-1.2.0/LICENSE
--rw-r--r--   0 shunsuke   (501) staff       (20)     3004 2024-04-11 15:48:38.454905 unicodecheck-1.2.0/PKG-INFO
--rw-r--r--   0 shunsuke   (501) staff       (20)     2066 2024-04-09 06:48:33.000000 unicodecheck-1.2.0/README.md
--rw-r--r--   0 shunsuke   (501) staff       (20)     1043 2024-03-20 16:01:49.000000 unicodecheck-1.2.0/pyproject.toml
--rw-r--r--   0 shunsuke   (501) staff       (20)       38 2024-04-11 15:48:38.455183 unicodecheck-1.2.0/setup.cfg
-drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-04-11 15:48:38.453384 unicodecheck-1.2.0/unicodecheck/
--rw-r--r--   0 shunsuke   (501) staff       (20)       22 2024-04-09 06:48:33.000000 unicodecheck-1.2.0/unicodecheck/__init__.py
--rw-r--r--   0 shunsuke   (501) staff       (20)       82 2023-11-11 17:10:51.000000 unicodecheck-1.2.0/unicodecheck/__main__.py
--rw-r--r--   0 shunsuke   (501) staff       (20)      704 2024-04-01 09:57:53.000000 unicodecheck-1.2.0/unicodecheck/args.py
--rw-r--r--   0 shunsuke   (501) staff       (20)     9228 2024-04-09 06:48:33.000000 unicodecheck-1.2.0/unicodecheck/cli.py
--rw-r--r--   0 shunsuke   (501) staff       (20)     2388 2024-03-11 14:57:18.000000 unicodecheck-1.2.0/unicodecheck/core.py
-drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-04-11 15:48:38.454407 unicodecheck-1.2.0/unicodecheck.egg-info/
--rw-r--r--   0 shunsuke   (501) staff       (20)     3004 2024-04-11 15:48:38.000000 unicodecheck-1.2.0/unicodecheck.egg-info/PKG-INFO
--rw-r--r--   0 shunsuke   (501) staff       (20)      362 2024-04-11 15:48:38.000000 unicodecheck-1.2.0/unicodecheck.egg-info/SOURCES.txt
--rw-r--r--   0 shunsuke   (501) staff       (20)        1 2024-04-11 15:48:38.000000 unicodecheck-1.2.0/unicodecheck.egg-info/dependency_links.txt
--rw-r--r--   0 shunsuke   (501) staff       (20)       55 2024-04-11 15:48:38.000000 unicodecheck-1.2.0/unicodecheck.egg-info/entry_points.txt
--rw-r--r--   0 shunsuke   (501) staff       (20)       58 2024-04-11 15:48:38.000000 unicodecheck-1.2.0/unicodecheck.egg-info/requires.txt
--rw-r--r--   0 shunsuke   (501) staff       (20)       13 2024-04-11 15:48:38.000000 unicodecheck-1.2.0/unicodecheck.egg-info/top_level.txt
+drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-04-27 17:41:21.918497 unicodecheck-1.2.1/
+-rw-r--r--   0 shunsuke   (501) staff       (20)     1064 2024-04-25 03:41:29.000000 unicodecheck-1.2.1/LICENSE
+-rw-r--r--   0 shunsuke   (501) staff       (20)     3004 2024-04-27 17:41:21.918295 unicodecheck-1.2.1/PKG-INFO
+-rw-r--r--   0 shunsuke   (501) staff       (20)     2066 2024-04-25 03:41:29.000000 unicodecheck-1.2.1/README.md
+-rw-r--r--   0 shunsuke   (501) staff       (20)     1043 2024-04-25 03:41:29.000000 unicodecheck-1.2.1/pyproject.toml
+-rw-r--r--   0 shunsuke   (501) staff       (20)       38 2024-04-27 17:41:21.918540 unicodecheck-1.2.1/setup.cfg
+drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-04-27 17:41:21.916887 unicodecheck-1.2.1/unicodecheck/
+-rw-r--r--   0 shunsuke   (501) staff       (20)       22 2024-04-25 03:42:37.000000 unicodecheck-1.2.1/unicodecheck/__init__.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)       82 2024-04-25 03:41:29.000000 unicodecheck-1.2.1/unicodecheck/__main__.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)      704 2024-04-25 03:41:29.000000 unicodecheck-1.2.1/unicodecheck/args.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)     9228 2024-04-25 03:41:29.000000 unicodecheck-1.2.1/unicodecheck/cli.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)     2388 2024-04-25 03:41:29.000000 unicodecheck-1.2.1/unicodecheck/core.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)        0 2024-04-25 03:41:53.000000 unicodecheck-1.2.1/unicodecheck/py.typed
+drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-04-27 17:41:21.917833 unicodecheck-1.2.1/unicodecheck.egg-info/
+-rw-r--r--   0 shunsuke   (501) staff       (20)     3004 2024-04-27 17:41:21.000000 unicodecheck-1.2.1/unicodecheck.egg-info/PKG-INFO
+-rw-r--r--   0 shunsuke   (501) staff       (20)      384 2024-04-27 17:41:21.000000 unicodecheck-1.2.1/unicodecheck.egg-info/SOURCES.txt
+-rw-r--r--   0 shunsuke   (501) staff       (20)        1 2024-04-27 17:41:21.000000 unicodecheck-1.2.1/unicodecheck.egg-info/dependency_links.txt
+-rw-r--r--   0 shunsuke   (501) staff       (20)       55 2024-04-27 17:41:21.000000 unicodecheck-1.2.1/unicodecheck.egg-info/entry_points.txt
+-rw-r--r--   0 shunsuke   (501) staff       (20)       58 2024-04-27 17:41:21.000000 unicodecheck-1.2.1/unicodecheck.egg-info/requires.txt
+-rw-r--r--   0 shunsuke   (501) staff       (20)       13 2024-04-27 17:41:21.000000 unicodecheck-1.2.1/unicodecheck.egg-info/top_level.txt
```

### Comparing `unicodecheck-1.2.0/LICENSE` & `unicodecheck-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unicodecheck-1.2.0/PKG-INFO` & `unicodecheck-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicodecheck
-Version: 1.2.0
+Version: 1.2.1
 Summary: Check if Unicode text files are Unicode-normalized
 Maintainer-email: curegit <contact@curegit.jp>
 License: MIT
 Project-URL: homepage, https://github.com/curegit/unicodecheck
 Project-URL: repository, https://github.com/curegit/unicodecheck.git
 Keywords: Unicode,character encoding
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `unicodecheck-1.2.0/README.md` & `unicodecheck-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `unicodecheck-1.2.0/pyproject.toml` & `unicodecheck-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unicodecheck-1.2.0/unicodecheck/args.py` & `unicodecheck-1.2.1/unicodecheck/args.py`

 * *Files identical despite different names*

### Comparing `unicodecheck-1.2.0/unicodecheck/cli.py` & `unicodecheck-1.2.1/unicodecheck/cli.py`

 * *Files identical despite different names*

### Comparing `unicodecheck-1.2.0/unicodecheck/core.py` & `unicodecheck-1.2.1/unicodecheck/core.py`

 * *Files identical despite different names*

### Comparing `unicodecheck-1.2.0/unicodecheck.egg-info/PKG-INFO` & `unicodecheck-1.2.1/unicodecheck.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicodecheck
-Version: 1.2.0
+Version: 1.2.1
 Summary: Check if Unicode text files are Unicode-normalized
 Maintainer-email: curegit <contact@curegit.jp>
 License: MIT
 Project-URL: homepage, https://github.com/curegit/unicodecheck
 Project-URL: repository, https://github.com/curegit/unicodecheck.git
 Keywords: Unicode,character encoding
 Classifier: Programming Language :: Python :: 3 :: Only
```

