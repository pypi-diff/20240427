# Comparing `tmp/naucse_render-2.0.tar.gz` & `tmp/naucse_render-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naucse_render-2.0.tar", last modified: Sat Apr 27 16:51:25 2024, max compression
+gzip compressed data, was "naucse_render-2.0.1.tar", last modified: Sat Apr 27 14:43:08 2024, max compression
```

## Comparing `naucse_render-2.0.tar` & `naucse_render-2.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 pviktori  (1000) pviktori  (1000)        0 2024-04-27 16:51:25.083078 naucse_render-2.0/
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)     1174 2021-03-18 20:26:01.000000 naucse_render-2.0/LICENSE.MIT
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     7235 2024-04-27 16:51:25.083078 naucse_render-2.0/PKG-INFO
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     6482 2024-04-27 12:52:49.000000 naucse_render-2.0/README.md
-drwxr-xr-x   0 pviktori  (1000) pviktori  (1000)        0 2024-04-27 16:51:25.082078 naucse_render-2.0/naucse_render/
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)      110 2024-04-27 11:00:57.000000 naucse_render-2.0/naucse_render/__init__.py
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)       43 2021-03-18 20:26:01.000000 naucse_render-2.0/naucse_render/__main__.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     3557 2024-04-27 11:00:57.000000 naucse_render-2.0/naucse_render/cli.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     5931 2024-04-27 11:00:57.000000 naucse_render-2.0/naucse_render/compile.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     9451 2024-04-27 11:00:57.000000 naucse_render-2.0/naucse_render/course.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     1337 2024-04-27 11:00:57.000000 naucse_render-2.0/naucse_render/encode.py
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)     2552 2021-03-18 20:26:01.000000 naucse_render-2.0/naucse_render/lesson.py
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)     1876 2021-03-18 20:26:01.000000 naucse_render-2.0/naucse_render/load.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     5422 2024-04-27 16:50:53.000000 naucse_render-2.0/naucse_render/markdown.py
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)     1355 2021-03-18 20:26:01.000000 naucse_render-2.0/naucse_render/notebook.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     6119 2024-04-27 11:00:57.000000 naucse_render-2.0/naucse_render/page.py
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)     4163 2024-04-27 14:28:35.000000 naucse_render-2.0/naucse_render/templates.py
-drwxr-xr-x   0 pviktori  (1000) pviktori  (1000)        0 2024-04-27 16:51:25.083078 naucse_render-2.0/naucse_render.egg-info/
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     7235 2024-04-27 16:51:25.000000 naucse_render-2.0/naucse_render.egg-info/PKG-INFO
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)      559 2024-04-27 16:51:25.000000 naucse_render-2.0/naucse_render.egg-info/SOURCES.txt
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)        1 2024-04-27 16:51:25.000000 naucse_render-2.0/naucse_render.egg-info/dependency_links.txt
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)        1 2024-04-27 16:51:24.000000 naucse_render-2.0/naucse_render.egg-info/not-zip-safe
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)      128 2024-04-27 16:51:25.000000 naucse_render-2.0/naucse_render.egg-info/requires.txt
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)       14 2024-04-27 16:51:25.000000 naucse_render-2.0/naucse_render.egg-info/top_level.txt
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)      784 2024-04-27 15:48:37.000000 naucse_render-2.0/pyproject.toml
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)       93 2024-04-27 16:51:25.084078 naucse_render-2.0/setup.cfg
+drwxr-xr-x   0 pviktori  (1000) pviktori  (1000)        0 2024-04-27 14:43:08.870594 naucse_render-2.0.1/
+-rw-rw-r--   0 pviktori  (1000) pviktori  (1000)     1174 2021-03-18 20:26:01.000000 naucse_render-2.0.1/LICENSE.MIT
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)     7237 2024-04-27 14:43:08.870594 naucse_render-2.0.1/PKG-INFO
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)     6482 2024-04-27 12:52:49.000000 naucse_render-2.0.1/README.md
+drwxr-xr-x   0 pviktori  (1000) pviktori  (1000)        0 2024-04-27 14:43:08.868594 naucse_render-2.0.1/naucse_render/
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)      110 2024-04-27 11:00:57.000000 naucse_render-2.0.1/naucse_render/__init__.py
+-rw-rw-r--   0 pviktori  (1000) pviktori  (1000)       43 2021-03-18 20:26:01.000000 naucse_render-2.0.1/naucse_render/__main__.py
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)     3557 2024-04-27 11:00:57.000000 naucse_render-2.0.1/naucse_render/cli.py
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)     5931 2024-04-27 11:00:57.000000 naucse_render-2.0.1/naucse_render/compile.py
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)     9451 2024-04-27 11:00:57.000000 naucse_render-2.0.1/naucse_render/course.py
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)     1337 2024-04-27 11:00:57.000000 naucse_render-2.0.1/naucse_render/encode.py
+-rw-rw-r--   0 pviktori  (1000) pviktori  (1000)     2552 2021-03-18 20:26:01.000000 naucse_render-2.0.1/naucse_render/lesson.py
+-rw-rw-r--   0 pviktori  (1000) pviktori  (1000)     1876 2021-03-18 20:26:01.000000 naucse_render-2.0.1/naucse_render/load.py
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)     5421 2024-04-27 12:22:15.000000 naucse_render-2.0.1/naucse_render/markdown.py
+-rw-rw-r--   0 pviktori  (1000) pviktori  (1000)     1355 2021-03-18 20:26:01.000000 naucse_render-2.0.1/naucse_render/notebook.py
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)     6119 2024-04-27 11:00:57.000000 naucse_render-2.0.1/naucse_render/page.py
+-rw-rw-r--   0 pviktori  (1000) pviktori  (1000)     4163 2024-04-27 14:28:35.000000 naucse_render-2.0.1/naucse_render/templates.py
+drwxr-xr-x   0 pviktori  (1000) pviktori  (1000)        0 2024-04-27 14:43:08.869594 naucse_render-2.0.1/naucse_render.egg-info/
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)     7237 2024-04-27 14:43:08.000000 naucse_render-2.0.1/naucse_render.egg-info/PKG-INFO
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)      559 2024-04-27 14:43:08.000000 naucse_render-2.0.1/naucse_render.egg-info/SOURCES.txt
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)        1 2024-04-27 14:43:08.000000 naucse_render-2.0.1/naucse_render.egg-info/dependency_links.txt
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)        1 2024-04-27 12:22:59.000000 naucse_render-2.0.1/naucse_render.egg-info/not-zip-safe
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)      128 2024-04-27 14:43:08.000000 naucse_render-2.0.1/naucse_render.egg-info/requires.txt
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)       14 2024-04-27 14:43:08.000000 naucse_render-2.0.1/naucse_render.egg-info/top_level.txt
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)      786 2024-04-27 14:43:04.000000 naucse_render-2.0.1/pyproject.toml
+-rw-r--r--   0 pviktori  (1000) pviktori  (1000)       93 2024-04-27 14:43:08.870594 naucse_render-2.0.1/setup.cfg
```

### Comparing `naucse_render-2.0/LICENSE.MIT` & `naucse_render-2.0.1/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `naucse_render-2.0/PKG-INFO` & `naucse_render-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naucse_render
-Version: 2.0
+Version: 2.0.1
 Summary: Converts course material to naucse.python.cz API
 Maintainer-email: Petr Viktorin <encukou@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/pyvec/naucse_render
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `naucse_render-2.0/README.md` & `naucse_render-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `naucse_render-2.0/naucse_render/cli.py` & `naucse_render-2.0.1/naucse_render/cli.py`

 * *Files identical despite different names*

### Comparing `naucse_render-2.0/naucse_render/compile.py` & `naucse_render-2.0.1/naucse_render/compile.py`

 * *Files identical despite different names*

### Comparing `naucse_render-2.0/naucse_render/course.py` & `naucse_render-2.0.1/naucse_render/course.py`

 * *Files identical despite different names*

### Comparing `naucse_render-2.0/naucse_render/encode.py` & `naucse_render-2.0.1/naucse_render/encode.py`

 * *Files identical despite different names*

### Comparing `naucse_render-2.0/naucse_render/lesson.py` & `naucse_render-2.0.1/naucse_render/lesson.py`

 * *Files identical despite different names*

### Comparing `naucse_render-2.0/naucse_render/load.py` & `naucse_render-2.0.1/naucse_render/load.py`

 * *Files identical despite different names*

### Comparing `naucse_render-2.0/naucse_render/markdown.py` & `naucse_render-2.0.1/naucse_render/markdown.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     ADMONITION_NAME_PATTERN = re.compile(r' *\[(\S+)\]([^\n]*)\n')
 
     def parse_naucse_admonition(block, m, state):
 
         text, end_pos = block.extract_block_quote(m, state)
         name_match = ADMONITION_NAME_PATTERN.match(text)
         if name_match:
-            # It's an admonition
+            # It's an amonition
             token = {
                 'type': 'naucse_admonition',
                 'attrs': {
                     'name': name_match[1].strip(),
                     'title': name_match[2].strip(),
                 },
             }
```

### Comparing `naucse_render-2.0/naucse_render/notebook.py` & `naucse_render-2.0.1/naucse_render/notebook.py`

 * *Files identical despite different names*

### Comparing `naucse_render-2.0/naucse_render/page.py` & `naucse_render-2.0.1/naucse_render/page.py`

 * *Files identical despite different names*

### Comparing `naucse_render-2.0/naucse_render/templates.py` & `naucse_render-2.0.1/naucse_render/templates.py`

 * *Files identical despite different names*

### Comparing `naucse_render-2.0/naucse_render.egg-info/PKG-INFO` & `naucse_render-2.0.1/naucse_render.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naucse_render
-Version: 2.0
+Version: 2.0.1
 Summary: Converts course material to naucse.python.cz API
 Maintainer-email: Petr Viktorin <encukou@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/pyvec/naucse_render
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `naucse_render-2.0/naucse_render.egg-info/SOURCES.txt` & `naucse_render-2.0.1/naucse_render.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naucse_render-2.0/pyproject.toml` & `naucse_render-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "naucse_render"
-version = '2.0'
+version = '2.0.1'
 description = 'Converts course material to naucse.python.cz API'
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
```

