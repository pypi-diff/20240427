# Comparing `tmp/nijtaio-1.1.8.tar.gz` & `tmp/nijtaio-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nijtaio-1.1.8.tar", last modified: Thu Apr 25 09:29:56 2024, max compression
+gzip compressed data, was "nijtaio-1.1.9.tar", last modified: Thu Apr 25 17:47:18 2024, max compression
```

## Comparing `nijtaio-1.1.8.tar` & `nijtaio-1.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-25 09:29:56.620210 nijtaio-1.1.8/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2206 2024-04-25 09:29:56.620210 nijtaio-1.1.8/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1722 2023-10-27 13:17:30.000000 nijtaio-1.1.8/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-25 09:29:56.620210 nijtaio-1.1.8/nijtaio/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6873 2024-04-25 08:45:28.000000 nijtaio-1.1.8/nijtaio/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2024-04-11 17:18:02.000000 nijtaio-1.1.8/nijtaio/_version.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3388 2024-01-22 14:46:02.000000 nijtaio-1.1.8/nijtaio/cli.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-25 09:29:56.620210 nijtaio-1.1.8/nijtaio.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2206 2024-04-25 09:29:56.000000 nijtaio-1.1.8/nijtaio.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      337 2024-04-25 09:29:56.000000 nijtaio-1.1.8/nijtaio.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-25 09:29:56.000000 nijtaio-1.1.8/nijtaio.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2024-04-25 09:29:56.000000 nijtaio-1.1.8/nijtaio.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       41 2024-04-25 09:29:56.000000 nijtaio-1.1.8/nijtaio.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2024-04-25 09:29:56.000000 nijtaio-1.1.8/nijtaio.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      567 2024-04-25 08:56:32.000000 nijtaio-1.1.8/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-25 09:29:56.620210 nijtaio-1.1.8/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      471 2023-11-28 13:18:36.000000 nijtaio-1.1.8/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-25 09:29:56.620210 nijtaio-1.1.8/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      891 2023-12-01 13:56:45.000000 nijtaio-1.1.8/tests/test_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      628 2023-11-28 13:18:36.000000 nijtaio-1.1.8/tests/test_nijtaio.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1427 2023-11-08 17:25:26.000000 nijtaio-1.1.8/tests/test_s3.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-25 17:47:18.087142 nijtaio-1.1.9/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2206 2024-04-25 17:47:18.087142 nijtaio-1.1.9/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1722 2023-10-27 13:17:30.000000 nijtaio-1.1.9/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-25 17:47:18.087142 nijtaio-1.1.9/nijtaio/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6516 2024-04-25 14:44:11.000000 nijtaio-1.1.9/nijtaio/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2024-04-25 17:46:16.000000 nijtaio-1.1.9/nijtaio/_version.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3388 2024-01-22 14:46:02.000000 nijtaio-1.1.9/nijtaio/cli.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-25 17:47:18.087142 nijtaio-1.1.9/nijtaio.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2206 2024-04-25 17:47:18.000000 nijtaio-1.1.9/nijtaio.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      337 2024-04-25 17:47:18.000000 nijtaio-1.1.9/nijtaio.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-25 17:47:18.000000 nijtaio-1.1.9/nijtaio.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2024-04-25 17:47:18.000000 nijtaio-1.1.9/nijtaio.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       41 2024-04-25 17:47:18.000000 nijtaio-1.1.9/nijtaio.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2024-04-25 17:47:18.000000 nijtaio-1.1.9/nijtaio.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      567 2024-04-25 17:46:26.000000 nijtaio-1.1.9/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-25 17:47:18.087142 nijtaio-1.1.9/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      471 2023-11-28 13:18:36.000000 nijtaio-1.1.9/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-25 17:47:18.087142 nijtaio-1.1.9/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      891 2023-12-01 13:56:45.000000 nijtaio-1.1.9/tests/test_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      628 2023-11-28 13:18:36.000000 nijtaio-1.1.9/tests/test_nijtaio.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1427 2023-11-08 17:25:26.000000 nijtaio-1.1.9/tests/test_s3.py
```

### Comparing `nijtaio-1.1.8/PKG-INFO` & `nijtaio-1.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nijtaio
-Version: 1.1.8
+Version: 1.1.9
 Summary: Helper module to streamline access to Nijta's API
 Project-URL: Documentation, https://docs.nijta.com
 Project-URL: Bug Tracker, https://github.com/Nijta/nijta-samples/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `nijtaio-1.1.8/README.md` & `nijtaio-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `nijtaio-1.1.8/nijtaio/__init__.py` & `nijtaio-1.1.9/nijtaio/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -161,18 +161,12 @@
         return content['data']['task_status'], None
 
     anon_batch_in_bytes = bytes.fromhex(content['data']['task_result']['response'])
     anon_batch = ast.literal_eval(anon_batch_in_bytes.decode())['data']
 
     result = {}
     for filename in anon_batch:
-        result[filename] = {}
+        result[filename] = anon_batch[filename]
         if 'audio' in anon_batch[filename]:
             result[filename]['audio'] = bytes.fromhex(anon_batch[filename]['audio'])
-        if 'transcription' in anon_batch[filename]:
-            result[filename]['transcription'] = anon_batch[filename]['transcription']
-        if 'words' in anon_batch[filename]:
-            result[filename]['words'] = anon_batch[filename]['words']
-        if 'sequence' in anon_batch[filename]:
-            result[filename]['sequence'] = anon_batch[filename]['sequence']
 
     return content['data']['task_status'], result
```

### Comparing `nijtaio-1.1.8/nijtaio/cli.py` & `nijtaio-1.1.9/nijtaio/cli.py`

 * *Files identical despite different names*

### Comparing `nijtaio-1.1.8/nijtaio.egg-info/PKG-INFO` & `nijtaio-1.1.9/nijtaio.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nijtaio
-Version: 1.1.8
+Version: 1.1.9
 Summary: Helper module to streamline access to Nijta's API
 Project-URL: Documentation, https://docs.nijta.com
 Project-URL: Bug Tracker, https://github.com/Nijta/nijta-samples/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `nijtaio-1.1.8/pyproject.toml` & `nijtaio-1.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nijtaio"
-version = "1.1.8"
+version = "1.1.9"
 description = "Helper module to streamline access to Nijta's API"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Developers",
     "License :: Other/Proprietary License"
 ]
 dependencies = ['requests', 'soundfile', 'librosa', 'datasets', 'fire']
```

### Comparing `nijtaio-1.1.8/tests/test_dataset.py` & `nijtaio-1.1.9/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `nijtaio-1.1.8/tests/test_nijtaio.py` & `nijtaio-1.1.9/tests/test_nijtaio.py`

 * *Files identical despite different names*

### Comparing `nijtaio-1.1.8/tests/test_s3.py` & `nijtaio-1.1.9/tests/test_s3.py`

 * *Files identical despite different names*

