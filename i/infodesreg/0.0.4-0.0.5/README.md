# Comparing `tmp/infodesreg-0.0.4.tar.gz` & `tmp/infodesreg-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infodesreg-0.0.4.tar", last modified: Fri Apr 26 18:28:52 2024, max compression
+gzip compressed data, was "infodesreg-0.0.5.tar", last modified: Fri Apr 26 18:35:50 2024, max compression
```

## Comparing `infodesreg-0.0.4.tar` & `infodesreg-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-26 18:28:52.501952 infodesreg-0.0.4/
--rw-r--r--   0 firuzjuraev   (501) staff       (20)     1073 2024-04-26 17:42:23.000000 infodesreg-0.0.4/LICENSE
--rw-r--r--   0 firuzjuraev   (501) staff       (20)      713 2024-04-26 18:28:52.501764 infodesreg-0.0.4/PKG-INFO
--rw-r--r--   0 firuzjuraev   (501) staff       (20)      202 2024-04-26 17:42:07.000000 infodesreg-0.0.4/README.md
--rw-r--r--   0 firuzjuraev   (501) staff       (20)      491 2024-04-26 18:28:41.000000 infodesreg-0.0.4/pyproject.toml
--rw-r--r--   0 firuzjuraev   (501) staff       (20)       38 2024-04-26 18:28:52.501996 infodesreg-0.0.4/setup.cfg
-drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-26 18:28:52.500120 infodesreg-0.0.4/src/
-drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-26 18:28:52.500942 infodesreg-0.0.4/src/infodesreg/
--rw-r--r--   0 firuzjuraev   (501) staff       (20)       41 2024-04-26 18:28:03.000000 infodesreg-0.0.4/src/infodesreg/__init__.py
--rw-r--r--   0 firuzjuraev   (501) staff       (20)     4994 2024-04-26 18:27:53.000000 infodesreg-0.0.4/src/infodesreg/base.py
-drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-26 18:28:52.501591 infodesreg-0.0.4/src/infodesreg.egg-info/
--rw-r--r--   0 firuzjuraev   (501) staff       (20)      713 2024-04-26 18:28:52.000000 infodesreg-0.0.4/src/infodesreg.egg-info/PKG-INFO
--rw-r--r--   0 firuzjuraev   (501) staff       (20)      234 2024-04-26 18:28:52.000000 infodesreg-0.0.4/src/infodesreg.egg-info/SOURCES.txt
--rw-r--r--   0 firuzjuraev   (501) staff       (20)        1 2024-04-26 18:28:52.000000 infodesreg-0.0.4/src/infodesreg.egg-info/dependency_links.txt
--rw-r--r--   0 firuzjuraev   (501) staff       (20)       11 2024-04-26 18:28:52.000000 infodesreg-0.0.4/src/infodesreg.egg-info/top_level.txt
+drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-26 18:35:50.767770 infodesreg-0.0.5/
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)     1073 2024-04-26 17:42:23.000000 infodesreg-0.0.5/LICENSE
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)      713 2024-04-26 18:35:50.767606 infodesreg-0.0.5/PKG-INFO
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)      202 2024-04-26 17:42:07.000000 infodesreg-0.0.5/README.md
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)      491 2024-04-26 18:33:19.000000 infodesreg-0.0.5/pyproject.toml
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)       38 2024-04-26 18:35:50.767804 infodesreg-0.0.5/setup.cfg
+drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-26 18:35:50.765664 infodesreg-0.0.5/src/
+drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-26 18:35:50.766654 infodesreg-0.0.5/src/infodesreg/
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)       43 2024-04-26 18:34:05.000000 infodesreg-0.0.5/src/infodesreg/__init__.py
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)     4994 2024-04-26 18:27:53.000000 infodesreg-0.0.5/src/infodesreg/base.py
+drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-26 18:35:50.767465 infodesreg-0.0.5/src/infodesreg.egg-info/
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)      713 2024-04-26 18:35:50.000000 infodesreg-0.0.5/src/infodesreg.egg-info/PKG-INFO
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)      234 2024-04-26 18:35:50.000000 infodesreg-0.0.5/src/infodesreg.egg-info/SOURCES.txt
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)        1 2024-04-26 18:35:50.000000 infodesreg-0.0.5/src/infodesreg.egg-info/dependency_links.txt
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)       11 2024-04-26 18:35:50.000000 infodesreg-0.0.5/src/infodesreg.egg-info/top_level.txt
```

### Comparing `infodesreg-0.0.4/LICENSE` & `infodesreg-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `infodesreg-0.0.4/PKG-INFO` & `infodesreg-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infodesreg
-Version: 0.0.4
+Version: 0.0.5
 Summary: Dynamic Ensemble Selectio for Regression tasks
 Author-email: Panda <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `infodesreg-0.0.4/src/infodesreg/base.py` & `infodesreg-0.0.5/src/infodesreg/base.py`

 * *Files identical despite different names*

### Comparing `infodesreg-0.0.4/src/infodesreg.egg-info/PKG-INFO` & `infodesreg-0.0.5/src/infodesreg.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infodesreg
-Version: 0.0.4
+Version: 0.0.5
 Summary: Dynamic Ensemble Selectio for Regression tasks
 Author-email: Panda <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

