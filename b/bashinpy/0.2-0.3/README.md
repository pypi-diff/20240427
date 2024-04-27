# Comparing `tmp/bashinpy-0.2.tar.gz` & `tmp/bashinpy-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bashinpy-0.2.tar", last modified: Sat Apr 27 13:26:48 2024, max compression
+gzip compressed data, was "bashinpy-0.3.tar", last modified: Sat Apr 27 15:14:39 2024, max compression
```

## Comparing `bashinpy-0.2.tar` & `bashinpy-0.3.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-27 13:26:48.415176 bashinpy-0.2/
--rw-r--r--   0 u0_a191  (10191) u0_a191  (10191)      231 2024-04-27 13:26:48.415176 bashinpy-0.2/PKG-INFO
--rw-------   0 u0_a191  (10191) u0_a191  (10191)      143 2024-04-27 13:02:42.000000 bashinpy-0.2/README.rst
--rw-------   0 u0_a191  (10191) u0_a191  (10191)       38 2024-04-27 13:26:48.415176 bashinpy-0.2/setup.cfg
--rw-------   0 u0_a191  (10191) u0_a191  (10191)      534 2024-04-27 13:26:32.000000 bashinpy-0.2/setup.py
-drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-27 13:26:48.381842 bashinpy-0.2/src/
-drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-27 13:26:48.391842 bashinpy-0.2/src/bashinpy/
--rw-------   0 u0_a191  (10191) u0_a191  (10191)       58 2024-04-27 13:25:19.000000 bashinpy-0.2/src/bashinpy/__init__.py
-drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-27 13:26:48.401842 bashinpy-0.2/src/bashinpy/bash/
--rw-------   0 u0_a191  (10191) u0_a191  (10191)       20 2024-04-27 13:03:25.000000 bashinpy-0.2/src/bashinpy/bash/__init__.py
--rw-------   0 u0_a191  (10191) u0_a191  (10191)      190 2024-04-27 12:55:16.000000 bashinpy-0.2/src/bashinpy/bash/bash.py
-drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-27 13:26:48.405176 bashinpy-0.2/src/bashinpy/git/
--rw-------   0 u0_a191  (10191) u0_a191  (10191)       19 2024-04-27 13:23:29.000000 bashinpy-0.2/src/bashinpy/git/__init__.py
--rw-------   0 u0_a191  (10191) u0_a191  (10191)      103 2024-04-27 13:25:03.000000 bashinpy-0.2/src/bashinpy/git/git.py
-drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-27 13:26:48.408509 bashinpy-0.2/src/bashinpy/system/
--rw-------   0 u0_a191  (10191) u0_a191  (10191)       22 2024-04-27 13:03:40.000000 bashinpy-0.2/src/bashinpy/system/__init__.py
--rw-------   0 u0_a191  (10191) u0_a191  (10191)      213 2024-04-27 13:22:54.000000 bashinpy-0.2/src/bashinpy/system/system.py
-drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-27 13:26:48.411842 bashinpy-0.2/src/bashinpy.egg-info/
--rw-r--r--   0 u0_a191  (10191) u0_a191  (10191)      231 2024-04-27 13:26:48.000000 bashinpy-0.2/src/bashinpy.egg-info/PKG-INFO
--rw-------   0 u0_a191  (10191) u0_a191  (10191)      359 2024-04-27 13:26:48.000000 bashinpy-0.2/src/bashinpy.egg-info/SOURCES.txt
--rw-------   0 u0_a191  (10191) u0_a191  (10191)        1 2024-04-27 13:26:48.000000 bashinpy-0.2/src/bashinpy.egg-info/dependency_links.txt
--rw-------   0 u0_a191  (10191) u0_a191  (10191)        9 2024-04-27 13:26:48.000000 bashinpy-0.2/src/bashinpy.egg-info/top_level.txt
+drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-27 15:14:39.349399 bashinpy-0.3/
+-rw-r--r--   0 u0_a191  (10191) u0_a191  (10191)      231 2024-04-27 15:14:39.346066 bashinpy-0.3/PKG-INFO
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)      143 2024-04-27 13:02:42.000000 bashinpy-0.3/README.rst
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)       38 2024-04-27 15:14:39.349399 bashinpy-0.3/setup.cfg
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)      534 2024-04-27 15:14:25.000000 bashinpy-0.3/setup.py
+drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-27 15:14:39.296066 bashinpy-0.3/src/
+drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-27 15:14:39.309400 bashinpy-0.3/src/bashinpy/
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)       80 2024-04-27 15:14:00.000000 bashinpy-0.3/src/bashinpy/__init__.py
+drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-27 15:14:39.326066 bashinpy-0.3/src/bashinpy/bash/
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)       20 2024-04-27 13:03:25.000000 bashinpy-0.3/src/bashinpy/bash/__init__.py
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)      190 2024-04-27 12:55:16.000000 bashinpy-0.3/src/bashinpy/bash/bash.py
+drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-27 15:14:39.332733 bashinpy-0.3/src/bashinpy/git/
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)       19 2024-04-27 13:23:29.000000 bashinpy-0.3/src/bashinpy/git/__init__.py
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)      103 2024-04-27 13:25:03.000000 bashinpy-0.3/src/bashinpy/git/git.py
+drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-27 15:14:39.336066 bashinpy-0.3/src/bashinpy/ncurses/
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)       23 2024-04-27 15:10:32.000000 bashinpy-0.3/src/bashinpy/ncurses/__init__.py
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)      288 2024-04-27 15:13:42.000000 bashinpy-0.3/src/bashinpy/ncurses/ncurses.py
+drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-27 15:14:39.342733 bashinpy-0.3/src/bashinpy/system/
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)       22 2024-04-27 13:03:40.000000 bashinpy-0.3/src/bashinpy/system/__init__.py
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)      267 2024-04-27 15:09:58.000000 bashinpy-0.3/src/bashinpy/system/system.py
+drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-27 15:14:39.342733 bashinpy-0.3/src/bashinpy.egg-info/
+-rw-r--r--   0 u0_a191  (10191) u0_a191  (10191)      231 2024-04-27 15:14:39.000000 bashinpy-0.3/src/bashinpy.egg-info/PKG-INFO
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)      424 2024-04-27 15:14:39.000000 bashinpy-0.3/src/bashinpy.egg-info/SOURCES.txt
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)        1 2024-04-27 15:14:39.000000 bashinpy-0.3/src/bashinpy.egg-info/dependency_links.txt
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)        9 2024-04-27 15:14:39.000000 bashinpy-0.3/src/bashinpy.egg-info/top_level.txt
```

### Comparing `bashinpy-0.2/setup.py` & `bashinpy-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 
 # Die Long Description aus der README.rst einlesen
 with open('README.rst', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='bashinpy',
-    version='0.2',
+    version='0.3',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[],  # Fügen Sie hier erforderliche Abhängigkeiten hinzu
     long_description=long_description,  # Hinzufügen der Long Description
     long_description_content_type='text/x-rst',  # Angeben des Inhaltsformats
 )
```

