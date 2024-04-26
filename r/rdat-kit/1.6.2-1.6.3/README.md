# Comparing `tmp/rdat_kit-1.6.2.tar.gz` & `tmp/rdat_kit-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdat_kit-1.6.2.tar", last modified: Tue Aug 15 21:21:18 2023, max compression
+gzip compressed data, was "/home/runner/work/RDATKit/RDATKit/rdat-kit/dist/.tmp-rpdyo9ti/rdat_kit-1.6.3.tar", last modified: Fri Apr 26 22:31:18 2024, max compression
```

## Comparing `rdat_kit-1.6.2.tar` & `rdat_kit-1.6.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-15 21:21:18.159289 rdat_kit-1.6.2/
--rw-r--r--   0 thomas     (501) staff       (20)     1095 2023-08-04 21:20:38.000000 rdat_kit-1.6.2/LICENSE
--rw-r--r--   0 thomas     (501) staff       (20)     2028 2023-08-15 21:21:18.159025 rdat_kit-1.6.2/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)     1387 2023-08-15 18:46:40.000000 rdat_kit-1.6.2/README.md
--rw-r--r--   0 thomas     (501) staff       (20)      744 2023-08-15 21:20:51.000000 rdat_kit-1.6.2/pyproject.toml
--rw-r--r--   0 thomas     (501) staff       (20)       38 2023-08-15 21:21:18.159346 rdat_kit-1.6.2/setup.cfg
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-15 21:21:18.154154 rdat_kit-1.6.2/src/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-15 21:21:18.157434 rdat_kit-1.6.2/src/rdat_kit/
--rw-r--r--   0 thomas     (501) staff       (20)      103 2023-08-04 21:19:56.000000 rdat_kit-1.6.2/src/rdat_kit/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)    65068 2023-08-04 21:19:56.000000 rdat_kit-1.6.2/src/rdat_kit/handler.py
--rw-r--r--   0 thomas     (501) staff       (20)    12381 2023-08-04 21:19:56.000000 rdat_kit-1.6.2/src/rdat_kit/util.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-15 21:21:18.158654 rdat_kit-1.6.2/src/rdat_kit.egg-info/
--rw-r--r--   0 thomas     (501) staff       (20)     2028 2023-08-15 21:21:18.000000 rdat_kit-1.6.2/src/rdat_kit.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)      281 2023-08-15 21:21:18.000000 rdat_kit-1.6.2/src/rdat_kit.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (501) staff       (20)        1 2023-08-15 21:21:18.000000 rdat_kit-1.6.2/src/rdat_kit.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (501) staff       (20)       10 2023-08-15 21:21:18.000000 rdat_kit-1.6.2/src/rdat_kit.egg-info/requires.txt
--rw-r--r--   0 thomas     (501) staff       (20)        9 2023-08-15 21:21:18.000000 rdat_kit-1.6.2/src/rdat_kit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:31:18.000000 rdat_kit-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-26 22:31:10.000000 rdat_kit-1.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-26 22:31:18.000000 rdat_kit-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-26 22:31:10.000000 rdat_kit-1.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-26 22:31:10.000000 rdat_kit-1.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 22:31:18.000000 rdat_kit-1.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:31:18.000000 rdat_kit-1.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:31:18.000000 rdat_kit-1.6.3/src/rdat_kit/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-26 22:31:10.000000 rdat_kit-1.6.3/src/rdat_kit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65068 2024-04-26 22:31:10.000000 rdat_kit-1.6.3/src/rdat_kit/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-04-26 22:31:10.000000 rdat_kit-1.6.3/src/rdat_kit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:31:18.000000 rdat_kit-1.6.3/src/rdat_kit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-26 22:31:18.000000 rdat_kit-1.6.3/src/rdat_kit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-26 22:31:18.000000 rdat_kit-1.6.3/src/rdat_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 22:31:18.000000 rdat_kit-1.6.3/src/rdat_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 22:31:18.000000 rdat_kit-1.6.3/src/rdat_kit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 22:31:18.000000 rdat_kit-1.6.3/src/rdat_kit.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `rdat_kit-1.6.2/LICENSE` & `rdat_kit-1.6.3/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2011-2017 Leland Stanford Junior University
+Copyright (c) 2011-2024 Leland Stanford Junior University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `rdat_kit-1.6.2/PKG-INFO` & `rdat_kit-1.6.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: rdat_kit
-Version: 1.6.2
+Version: 1.6.3
 Summary: RDATKit is a utility library for reading and writing RDAT files that describe RNA structure mapping experiments
 Author-email: Das Lab <thedaslab@stanford.edu>
 Project-URL: Homepage, https://github.com/ribokit/rdatkit
-Project-URL: Documentation, https://rmdb.stanford.edu/rdatkit
+Project-URL: Documentation, https://ribokit.github.io/RDATKit/
 Project-URL: Bug Tracker, https://github.com/ribokit/rdatkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rdat_kit-1.6.2/README.md` & `rdat_kit-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `rdat_kit-1.6.2/pyproject.toml` & `rdat_kit-1.6.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rdat_kit"
-version = "1.6.2"
+version = "1.6.3"
 authors = [
   { name="Das Lab", email="thedaslab@stanford.edu" },
 ]
 description = "RDATKit is a utility library for reading and writing RDAT files that describe RNA structure mapping experiments"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -15,13 +15,13 @@
 dependencies = [
   "xlwt",
   "xlrd",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ribokit/rdatkit"
-"Documentation" = "https://rmdb.stanford.edu/rdatkit"
+"Documentation" = "https://ribokit.github.io/RDATKit/"
 "Bug Tracker" = "https://github.com/ribokit/rdatkit/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
```

### Comparing `rdat_kit-1.6.2/src/rdat_kit/handler.py` & `rdat_kit-1.6.3/src/rdat_kit/handler.py`

 * *Files identical despite different names*

### Comparing `rdat_kit-1.6.2/src/rdat_kit/util.py` & `rdat_kit-1.6.3/src/rdat_kit/util.py`

 * *Files identical despite different names*

### Comparing `rdat_kit-1.6.2/src/rdat_kit.egg-info/PKG-INFO` & `rdat_kit-1.6.3/src/rdat_kit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: rdat-kit
-Version: 1.6.2
+Version: 1.6.3
 Summary: RDATKit is a utility library for reading and writing RDAT files that describe RNA structure mapping experiments
 Author-email: Das Lab <thedaslab@stanford.edu>
 Project-URL: Homepage, https://github.com/ribokit/rdatkit
-Project-URL: Documentation, https://rmdb.stanford.edu/rdatkit
+Project-URL: Documentation, https://ribokit.github.io/RDATKit/
 Project-URL: Bug Tracker, https://github.com/ribokit/rdatkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

