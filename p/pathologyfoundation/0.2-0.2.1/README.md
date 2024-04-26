# Comparing `tmp/pathologyfoundation-0.2.tar.gz` & `tmp/pathologyfoundation-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathologyfoundation-0.2.tar", last modified: Fri Apr 26 22:07:35 2024, max compression
+gzip compressed data, was "pathologyfoundation-0.2.1.tar", last modified: Fri Apr 26 22:14:26 2024, max compression
```

## Comparing `pathologyfoundation-0.2.tar` & `pathologyfoundation-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-04-26 22:07:35.243886 pathologyfoundation-0.2/
--rw-r--r--   0 zhihuang   (501) staff       (20)     1048 2024-04-26 21:38:18.000000 pathologyfoundation-0.2/LICENSE
--rw-r--r--   0 zhihuang   (501) staff       (20)      540 2024-04-26 22:07:35.242998 pathologyfoundation-0.2/PKG-INFO
--rw-r--r--   0 zhihuang   (501) staff       (20)     2730 2024-04-26 21:38:18.000000 pathologyfoundation-0.2/README.md
-drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-04-26 22:07:35.218821 pathologyfoundation-0.2/pathologyfoundation/
--rw-r--r--   0 zhihuang   (501) staff       (20)      112 2024-04-26 21:38:18.000000 pathologyfoundation-0.2/pathologyfoundation/__init__.py
-drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-04-26 22:07:35.240489 pathologyfoundation-0.2/pathologyfoundation/dataset/
--rw-r--r--   0 zhihuang   (501) staff       (20)       25 2024-04-26 21:38:18.000000 pathologyfoundation-0.2/pathologyfoundation/dataset/__init__.py
--rw-r--r--   0 zhihuang   (501) staff       (20)     2813 2024-04-26 21:38:18.000000 pathologyfoundation-0.2/pathologyfoundation/dataset/load_data.py
--rw-r--r--   0 zhihuang   (501) staff       (20)      460 2024-04-26 21:38:18.000000 pathologyfoundation-0.2/pathologyfoundation/model_zoo.py
-drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-04-26 22:07:35.242314 pathologyfoundation-0.2/pathologyfoundation/models/
--rw-r--r--   0 zhihuang   (501) staff       (20)       64 2024-04-26 21:38:18.000000 pathologyfoundation-0.2/pathologyfoundation/models/__init__.py
--rw-r--r--   0 zhihuang   (501) staff       (20)    11065 2024-04-26 21:40:33.000000 pathologyfoundation-0.2/pathologyfoundation/models/finetuner.py
--rw-r--r--   0 zhihuang   (501) staff       (20)     6619 2024-04-26 21:38:18.000000 pathologyfoundation-0.2/pathologyfoundation/models/plip_vit.py
--rw-r--r--   0 zhihuang   (501) staff       (20)      700 2024-04-26 21:38:18.000000 pathologyfoundation-0.2/pathologyfoundation/utils.py
-drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-04-26 22:07:35.230251 pathologyfoundation-0.2/pathologyfoundation.egg-info/
--rw-r--r--   0 zhihuang   (501) staff       (20)      540 2024-04-26 22:07:35.000000 pathologyfoundation-0.2/pathologyfoundation.egg-info/PKG-INFO
--rw-r--r--   0 zhihuang   (501) staff       (20)      533 2024-04-26 22:07:35.000000 pathologyfoundation-0.2/pathologyfoundation.egg-info/SOURCES.txt
--rw-r--r--   0 zhihuang   (501) staff       (20)        1 2024-04-26 22:07:35.000000 pathologyfoundation-0.2/pathologyfoundation.egg-info/dependency_links.txt
--rw-r--r--   0 zhihuang   (501) staff       (20)       92 2024-04-26 22:07:35.000000 pathologyfoundation-0.2/pathologyfoundation.egg-info/requires.txt
--rw-r--r--   0 zhihuang   (501) staff       (20)       20 2024-04-26 22:07:35.000000 pathologyfoundation-0.2/pathologyfoundation.egg-info/top_level.txt
--rw-r--r--   0 zhihuang   (501) staff       (20)       38 2024-04-26 22:07:35.243987 pathologyfoundation-0.2/setup.cfg
--rw-r--r--   0 zhihuang   (501) staff       (20)      979 2024-04-26 22:00:28.000000 pathologyfoundation-0.2/setup.py
+drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-04-26 22:14:26.616737 pathologyfoundation-0.2.1/
+-rw-r--r--   0 zhihuang   (501) staff       (20)     1048 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.1/LICENSE
+-rw-r--r--   0 zhihuang   (501) staff       (20)      542 2024-04-26 22:14:26.615677 pathologyfoundation-0.2.1/PKG-INFO
+-rw-r--r--   0 zhihuang   (501) staff       (20)     2730 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.1/README.md
+drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-04-26 22:14:26.579663 pathologyfoundation-0.2.1/pathologyfoundation/
+-rw-r--r--   0 zhihuang   (501) staff       (20)      112 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.1/pathologyfoundation/__init__.py
+drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-04-26 22:14:26.599339 pathologyfoundation-0.2.1/pathologyfoundation/dataset/
+-rw-r--r--   0 zhihuang   (501) staff       (20)       25 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.1/pathologyfoundation/dataset/__init__.py
+-rw-r--r--   0 zhihuang   (501) staff       (20)     2813 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.1/pathologyfoundation/dataset/load_data.py
+-rw-r--r--   0 zhihuang   (501) staff       (20)      461 2024-04-26 22:13:48.000000 pathologyfoundation-0.2.1/pathologyfoundation/model_zoo.py
+drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-04-26 22:14:26.615030 pathologyfoundation-0.2.1/pathologyfoundation/models/
+-rw-r--r--   0 zhihuang   (501) staff       (20)       64 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.1/pathologyfoundation/models/__init__.py
+-rw-r--r--   0 zhihuang   (501) staff       (20)    11065 2024-04-26 21:40:33.000000 pathologyfoundation-0.2.1/pathologyfoundation/models/finetuner.py
+-rw-r--r--   0 zhihuang   (501) staff       (20)     6619 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.1/pathologyfoundation/models/plip_vit.py
+-rw-r--r--   0 zhihuang   (501) staff       (20)      700 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.1/pathologyfoundation/utils.py
+drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-04-26 22:14:26.594833 pathologyfoundation-0.2.1/pathologyfoundation.egg-info/
+-rw-r--r--   0 zhihuang   (501) staff       (20)      542 2024-04-26 22:14:26.000000 pathologyfoundation-0.2.1/pathologyfoundation.egg-info/PKG-INFO
+-rw-r--r--   0 zhihuang   (501) staff       (20)      533 2024-04-26 22:14:26.000000 pathologyfoundation-0.2.1/pathologyfoundation.egg-info/SOURCES.txt
+-rw-r--r--   0 zhihuang   (501) staff       (20)        1 2024-04-26 22:14:26.000000 pathologyfoundation-0.2.1/pathologyfoundation.egg-info/dependency_links.txt
+-rw-r--r--   0 zhihuang   (501) staff       (20)       92 2024-04-26 22:14:26.000000 pathologyfoundation-0.2.1/pathologyfoundation.egg-info/requires.txt
+-rw-r--r--   0 zhihuang   (501) staff       (20)       20 2024-04-26 22:14:26.000000 pathologyfoundation-0.2.1/pathologyfoundation.egg-info/top_level.txt
+-rw-r--r--   0 zhihuang   (501) staff       (20)       38 2024-04-26 22:14:26.616883 pathologyfoundation-0.2.1/setup.cfg
+-rw-r--r--   0 zhihuang   (501) staff       (20)      981 2024-04-26 22:14:10.000000 pathologyfoundation-0.2.1/setup.py
```

### Comparing `pathologyfoundation-0.2/LICENSE` & `pathologyfoundation-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pathologyfoundation-0.2/PKG-INFO` & `pathologyfoundation-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathologyfoundation
-Version: 0.2
+Version: 0.2.1
 Summary: A package of pathology foundation models.
 Home-page: https://github.com/PathologyFoundation/pathologyfoundation
 Author: Zhi Huang
 Author-email: hz9423@gmail.com
 Keywords: Pathology,Foundation model,PLIP,OpenPath
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pathologyfoundation-0.2/README.md` & `pathologyfoundation-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pathologyfoundation-0.2/pathologyfoundation/dataset/load_data.py` & `pathologyfoundation-0.2.1/pathologyfoundation/dataset/load_data.py`

 * *Files identical despite different names*

### Comparing `pathologyfoundation-0.2/pathologyfoundation/models/finetuner.py` & `pathologyfoundation-0.2.1/pathologyfoundation/models/finetuner.py`

 * *Files identical despite different names*

### Comparing `pathologyfoundation-0.2/pathologyfoundation/models/plip_vit.py` & `pathologyfoundation-0.2.1/pathologyfoundation/models/plip_vit.py`

 * *Files identical despite different names*

### Comparing `pathologyfoundation-0.2/pathologyfoundation/utils.py` & `pathologyfoundation-0.2.1/pathologyfoundation/utils.py`

 * *Files identical despite different names*

### Comparing `pathologyfoundation-0.2/pathologyfoundation.egg-info/PKG-INFO` & `pathologyfoundation-0.2.1/pathologyfoundation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathologyfoundation
-Version: 0.2
+Version: 0.2.1
 Summary: A package of pathology foundation models.
 Home-page: https://github.com/PathologyFoundation/pathologyfoundation
 Author: Zhi Huang
 Author-email: hz9423@gmail.com
 Keywords: Pathology,Foundation model,PLIP,OpenPath
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pathologyfoundation-0.2/pathologyfoundation.egg-info/SOURCES.txt` & `pathologyfoundation-0.2.1/pathologyfoundation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pathologyfoundation-0.2/setup.py` & `pathologyfoundation-0.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         "appdirs",
         "pandas",
         "numpy",
         "tqdm",
         "gdown",
         "scikit-learn",
     ],
-    version = '0.2',  # Ideally should be same as the GitHub release tag varsion
+    version = '0.2.1',  # Ideally should be same as the GitHub release tag varsion
     description="A package of pathology foundation models.",
     long_description="Please check our github page: https://github.com/PathologyFoundation/pathologyfoundation",
     author = 'Zhi Huang',
     author_email = 'hz9423@gmail.com',
     url = 'https://github.com/PathologyFoundation/pathologyfoundation',
     keywords = ['Pathology', 'Foundation model', "PLIP", "OpenPath"],
     classifiers=[
```

