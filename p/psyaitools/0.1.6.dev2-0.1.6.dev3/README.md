# Comparing `tmp/psyaitools-0.1.6.dev2.tar.gz` & `tmp/psyaitools-0.1.6.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyaitools-0.1.6.dev2.tar", max compression
+gzip compressed data, was "psyaitools-0.1.6.dev3.tar", max compression
```

## Comparing `psyaitools-0.1.6.dev2.tar` & `psyaitools-0.1.6.dev3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0    35149 2024-04-19 18:30:19.184238 psyaitools-0.1.6.dev2/LICENSE
--rw-r--r--   0        0        0      989 2024-04-27 10:16:07.785454 psyaitools-0.1.6.dev2/README.md
--rw-r--r--   0        0        0     6148 2024-04-26 16:27:46.412536 psyaitools-0.1.6.dev2/psyaitools/.DS_Store
--rw-r--r--   0        0        0        0 2024-04-26 17:38:19.164142 psyaitools-0.1.6.dev2/psyaitools/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 09:29:19.590033 psyaitools-0.1.6.dev2/psyaitools/func/IOs/__init__.py
--rw-r--r--   0        0        0     1775 2024-04-26 19:25:04.361766 psyaitools-0.1.6.dev2/psyaitools/func/IOs/base64_wav.py
--rw-r--r--   0        0        0      800 2024-04-27 11:59:15.003211 psyaitools-0.1.6.dev2/psyaitools/func/IOs/base64_xfccs.py
--rw-r--r--   0        0        0      218 2024-04-26 19:09:46.876182 psyaitools-0.1.6.dev2/psyaitools/func/IOs/readFiles.py
--rw-r--r--   0        0        0        0 2024-04-26 17:36:54.161932 psyaitools-0.1.6.dev2/psyaitools/func/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 17:37:47.798436 psyaitools-0.1.6.dev2/psyaitools/func/ext/__init__.py
--rw-r--r--   0        0        0      997 2024-04-26 15:06:50.275222 psyaitools-0.1.6.dev2/psyaitools/func/ext/shInst.py
--rw-r--r--   0        0        0        0 2024-04-26 17:37:24.367135 psyaitools-0.1.6.dev2/psyaitools/func/representation/__init__.py
--rw-r--r--   0        0        0     1527 2024-04-26 16:28:20.020756 psyaitools-0.1.6.dev2/psyaitools/func/representation/factDecomMachine.py
--rw-r--r--   0        0        0      166 2024-04-27 11:58:45.857987 psyaitools-0.1.6.dev2/psyaitools/func/representation/loud.py
--rw-r--r--   0        0        0     1908 2024-04-27 11:00:06.971921 psyaitools-0.1.6.dev2/psyaitools/func/representation/xfccs.py
--rw-r--r--   0        0        0     1518 2024-04-27 10:13:40.867570 psyaitools-0.1.6.dev2/psyaitools/res/BSD_3_LICENSE_spafe
--rw-r--r--   0        0        0       23 2024-04-19 18:36:31.305642 psyaitools-0.1.6.dev2/psyaitools/res/res.py
--rw-r--r--   0        0        0      454 2024-04-27 11:59:50.388874 psyaitools-0.1.6.dev2/pyproject.toml
--rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 psyaitools-0.1.6.dev2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-19 18:30:19.184238 psyaitools-0.1.6.dev3/LICENSE
+-rw-r--r--   0        0        0      989 2024-04-27 10:16:07.785454 psyaitools-0.1.6.dev3/README.md
+-rw-r--r--   0        0        0     6148 2024-04-26 16:27:46.412536 psyaitools-0.1.6.dev3/psyaitools/.DS_Store
+-rw-r--r--   0        0        0        0 2024-04-26 17:38:19.164142 psyaitools-0.1.6.dev3/psyaitools/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:29:19.590033 psyaitools-0.1.6.dev3/psyaitools/func/IO/__init__.py
+-rw-r--r--   0        0        0     1775 2024-04-26 19:25:04.361766 psyaitools-0.1.6.dev3/psyaitools/func/IO/base64_wav.py
+-rw-r--r--   0        0        0      878 2024-04-27 12:23:56.371782 psyaitools-0.1.6.dev3/psyaitools/func/IO/base64_xfccs.py
+-rw-r--r--   0        0        0      237 2024-04-27 12:21:56.157883 psyaitools-0.1.6.dev3/psyaitools/func/IO/readFiles.py
+-rw-r--r--   0        0        0        0 2024-04-26 17:36:54.161932 psyaitools-0.1.6.dev3/psyaitools/func/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 17:37:47.798436 psyaitools-0.1.6.dev3/psyaitools/func/ext/__init__.py
+-rw-r--r--   0        0        0      997 2024-04-26 15:06:50.275222 psyaitools-0.1.6.dev3/psyaitools/func/ext/shInst.py
+-rw-r--r--   0        0        0        0 2024-04-26 17:37:24.367135 psyaitools-0.1.6.dev3/psyaitools/func/representation/__init__.py
+-rw-r--r--   0        0        0     1527 2024-04-26 16:28:20.020756 psyaitools-0.1.6.dev3/psyaitools/func/representation/factDecomMachine.py
+-rw-r--r--   0        0        0      166 2024-04-27 11:58:45.857987 psyaitools-0.1.6.dev3/psyaitools/func/representation/loud.py
+-rw-r--r--   0        0        0     1908 2024-04-27 11:00:06.971921 psyaitools-0.1.6.dev3/psyaitools/func/representation/xfccs.py
+-rw-r--r--   0        0        0     1518 2024-04-27 10:13:40.867570 psyaitools-0.1.6.dev3/psyaitools/res/BSD_3_LICENSE_spafe
+-rw-r--r--   0        0        0       23 2024-04-19 18:36:31.305642 psyaitools-0.1.6.dev3/psyaitools/res/res.py
+-rw-r--r--   0        0        0      284 2024-04-27 12:25:37.048007 psyaitools-0.1.6.dev3/psyaitools/test.py
+-rw-r--r--   0        0        0      454 2024-04-27 12:25:54.737419 psyaitools-0.1.6.dev3/pyproject.toml
+-rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 psyaitools-0.1.6.dev3/PKG-INFO
```

### Comparing `psyaitools-0.1.6.dev2/LICENSE` & `psyaitools-0.1.6.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.6.dev2/README.md` & `psyaitools-0.1.6.dev3/README.md`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.6.dev2/psyaitools/.DS_Store` & `psyaitools-0.1.6.dev3/psyaitools/.DS_Store`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.6.dev2/psyaitools/func/IOs/base64_wav.py` & `psyaitools-0.1.6.dev3/psyaitools/func/IO/base64_wav.py`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.6.dev2/psyaitools/func/ext/shInst.py` & `psyaitools-0.1.6.dev3/psyaitools/func/ext/shInst.py`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.6.dev2/psyaitools/func/representation/factDecomMachine.py` & `psyaitools-0.1.6.dev3/psyaitools/func/representation/factDecomMachine.py`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.6.dev2/psyaitools/func/representation/xfccs.py` & `psyaitools-0.1.6.dev3/psyaitools/func/representation/xfccs.py`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.6.dev2/psyaitools/res/BSD_3_LICENSE_spafe` & `psyaitools-0.1.6.dev3/psyaitools/res/BSD_3_LICENSE_spafe`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.6.dev2/PKG-INFO` & `psyaitools-0.1.6.dev3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyaitools
-Version: 0.1.6.dev2
+Version: 0.1.6.dev3
 Summary: Loudness added.
 Author: moomoofarm1
 Author-email: 46774289+moomoofarm1@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

