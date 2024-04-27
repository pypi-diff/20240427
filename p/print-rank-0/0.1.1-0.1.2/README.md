# Comparing `tmp/print_rank_0-0.1.1.tar.gz` & `tmp/print_rank_0-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "print_rank_0-0.1.1.tar", last modified: Sat Jan  6 17:23:10 2024, max compression
+gzip compressed data, was "print_rank_0-0.1.2.tar", last modified: Sat Apr 27 17:52:14 2024, max compression
```

## Comparing `print_rank_0-0.1.1.tar` & `print_rank_0-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yuan      (1000) yuan      (1000)        0 2024-01-06 17:23:10.716083 print_rank_0-0.1.1/
--rw-r--r--   0 yuan      (1000) yuan      (1000)     1069 2024-01-06 15:16:41.000000 print_rank_0-0.1.1/LICENSE
--rw-r--r--   0 yuan      (1000) yuan      (1000)      658 2024-01-06 17:23:10.716083 print_rank_0-0.1.1/PKG-INFO
--rw-r--r--   0 yuan      (1000) yuan      (1000)       99 2024-01-06 17:21:11.000000 print_rank_0-0.1.1/README.md
-drwxr-xr-x   0 yuan      (1000) yuan      (1000)        0 2024-01-06 17:23:10.716083 print_rank_0-0.1.1/print_rank_0/
--rw-r--r--   0 yuan      (1000) yuan      (1000)      609 2024-01-06 17:17:12.000000 print_rank_0-0.1.1/print_rank_0/__init__.py
-drwxr-xr-x   0 yuan      (1000) yuan      (1000)        0 2024-01-06 17:23:10.716083 print_rank_0-0.1.1/print_rank_0.egg-info/
--rw-r--r--   0 yuan      (1000) yuan      (1000)      658 2024-01-06 17:23:10.000000 print_rank_0-0.1.1/print_rank_0.egg-info/PKG-INFO
--rw-r--r--   0 yuan      (1000) yuan      (1000)      195 2024-01-06 17:23:10.000000 print_rank_0-0.1.1/print_rank_0.egg-info/SOURCES.txt
--rw-r--r--   0 yuan      (1000) yuan      (1000)        1 2024-01-06 17:23:10.000000 print_rank_0-0.1.1/print_rank_0.egg-info/dependency_links.txt
--rw-r--r--   0 yuan      (1000) yuan      (1000)       13 2024-01-06 17:23:10.000000 print_rank_0-0.1.1/print_rank_0.egg-info/top_level.txt
--rw-r--r--   0 yuan      (1000) yuan      (1000)       38 2024-01-06 17:23:10.716083 print_rank_0-0.1.1/setup.cfg
--rw-r--r--   0 yuan      (1000) yuan      (1000)      783 2024-01-06 17:17:06.000000 print_rank_0-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 17:52:14.447806 print_rank_0-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-01-06 15:16:41.000000 print_rank_0-0.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      658 2024-04-27 17:52:14.447806 print_rank_0-0.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       99 2024-01-06 17:21:11.000000 print_rank_0-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 17:52:14.447806 print_rank_0-0.1.2/print_rank_0/
+-rw-r--r--   0 root         (0) root         (0)      597 2024-04-27 17:44:33.000000 print_rank_0-0.1.2/print_rank_0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 17:52:14.447806 print_rank_0-0.1.2/print_rank_0.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      658 2024-04-27 17:52:14.000000 print_rank_0-0.1.2/print_rank_0.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      195 2024-04-27 17:52:14.000000 print_rank_0-0.1.2/print_rank_0.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 17:52:14.000000 print_rank_0-0.1.2/print_rank_0.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-27 17:52:14.000000 print_rank_0-0.1.2/print_rank_0.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 17:52:14.447806 print_rank_0-0.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      783 2024-04-27 17:49:03.000000 print_rank_0-0.1.2/setup.py
```

### Comparing `print_rank_0-0.1.1/LICENSE` & `print_rank_0-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `print_rank_0-0.1.1/PKG-INFO` & `print_rank_0-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: print_rank_0
-Version: 0.1.1
+Version: 0.1.2
 Summary: Print on rank 0
 Home-page: https://github.com/yuantailing/print_rank_0
 Author: Tailing Yuan
 Author-email: yuantailing@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `print_rank_0-0.1.1/print_rank_0/__init__.py` & `print_rank_0-0.1.2/print_rank_0/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import sys
 
 
-def print_rank_0(self, *args, **kwargs):
+def print_rank_0(*args, **kwargs):
     """Print only on rank 0."""
     import torch
     if torch.distributed.get_rank() == 0:
         print(*args, **kwargs)
 
 
-def print_rank_last(self, *args, **kwargs):
+def print_rank_last(*args, **kwargs):
     """Print only on last rank."""
     import torch
     last_rank = torch.distributed.get_world_size() - 1
     if torch.distributed.get_rank() == last_rank:
         print(*args, **kwargs)
```

### Comparing `print_rank_0-0.1.1/print_rank_0.egg-info/PKG-INFO` & `print_rank_0-0.1.2/print_rank_0.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: print-rank-0
-Version: 0.1.1
+Version: 0.1.2
 Summary: Print on rank 0
 Home-page: https://github.com/yuantailing/print_rank_0
 Author: Tailing Yuan
 Author-email: yuantailing@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `print_rank_0-0.1.1/setup.py` & `print_rank_0-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
 
 
 setup(name="print_rank_0",
-      version="0.1.1",
+      version="0.1.2",
       author="Tailing Yuan",
       author_email="yuantailing@gmail.com",
       url="https://github.com/yuantailing/print_rank_0",
       tests_require=["pytest", "torch"],
       description="Print on rank 0",
       long_description=long_description,
       license="MIT",
```

