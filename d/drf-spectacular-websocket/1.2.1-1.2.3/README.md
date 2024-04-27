# Comparing `tmp/drf_spectacular_websocket-1.2.1.tar.gz` & `tmp/drf_spectacular_websocket-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_spectacular_websocket-1.2.1.tar", last modified: Fri Apr 26 18:08:09 2024, max compression
+gzip compressed data, was "drf_spectacular_websocket-1.2.3.tar", last modified: Fri Apr 26 18:26:14 2024, max compression
```

## Comparing `drf_spectacular_websocket-1.2.1.tar` & `drf_spectacular_websocket-1.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:08:09.153668 drf_spectacular_websocket-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-26 18:08:05.000000 drf_spectacular_websocket-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-26 18:08:09.153668 drf_spectacular_websocket-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-26 18:08:05.000000 drf_spectacular_websocket-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    11319 2024-04-26 18:08:05.000000 drf_spectacular_websocket-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 18:08:09.153668 drf_spectacular_websocket-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:08:09.145668 drf_spectacular_websocket-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:08:09.149668 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 18:08:05.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-26 18:08:05.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-26 18:08:05.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:08:09.149668 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 18:08:05.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-04-26 18:08:05.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/schemas/consumer_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-26 18:08:05.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/schemas/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-26 18:08:05.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:08:09.149668 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-26 18:08:09.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-26 18:08:09.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 18:08:09.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-26 18:08:09.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 18:08:09.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:08:09.149668 drf_spectacular_websocket-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-26 18:08:05.000000 drf_spectacular_websocket-1.2.1/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:26:14.873380 drf_spectacular_websocket-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-26 18:26:11.000000 drf_spectacular_websocket-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-04-26 18:26:14.873380 drf_spectacular_websocket-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-26 18:26:11.000000 drf_spectacular_websocket-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-26 18:26:11.000000 drf_spectacular_websocket-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 18:26:14.873380 drf_spectacular_websocket-1.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:26:14.869380 drf_spectacular_websocket-1.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:26:14.869380 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 18:26:11.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-26 18:26:11.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-26 18:26:11.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:26:14.873380 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 18:26:11.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-04-26 18:26:11.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/schemas/consumer_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-26 18:26:11.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/schemas/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-26 18:26:11.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:26:14.873380 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-04-26 18:26:14.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-26 18:26:14.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 18:26:14.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-26 18:26:14.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 18:26:14.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:26:14.873380 drf_spectacular_websocket-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-26 18:26:11.000000 drf_spectacular_websocket-1.2.3/tests/test_schema.py
```

### Comparing `drf_spectacular_websocket-1.2.1/LICENSE` & `drf_spectacular_websocket-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.1/PKG-INFO` & `drf_spectacular_websocket-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf_spectacular_websocket
-Version: 1.2.1
+Version: 1.2.3
 Summary: Extend websocket schema decorator for Django Channels
 Author-email: Friskes <friskesx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Friskes
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,15 +22,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/Friskes/drf-spectacular-websocket
-Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
+Project-URL: Bug Reports, https://github.com/Friskes/drf-spectacular-websocket/issues
 Project-URL: Source, https://github.com/Friskes/drf-spectacular-websocket/
 Keywords: Django,DRF,Spectacular,Swagger,Channels
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `drf_spectacular_websocket-1.2.1/README.md` & `drf_spectacular_websocket-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.1/pyproject.toml` & `drf_spectacular_websocket-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "drf_spectacular_websocket"
 # https://packaging.python.org/en/latest/guides/writing-pyproject-toml/#version
 # https://packaging.python.org/en/latest/guides/single-sourcing-package-version/#single-sourcing-the-version
-version = "1.2.1"
+version = "1.2.3"
 license = {file = "LICENSE"}
 authors = [
   {name="Friskes", email="friskesx@gmail.com"},
 ]
 description = "Extend websocket schema decorator for Django Channels"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -52,15 +52,15 @@
     "ruff==0.4.1",
     "pytest>=7.0.1",
 ]
 
 
 [project.urls]
 "Homepage" = "https://github.com/Friskes/drf-spectacular-websocket"
-"Bug Reports" = "https://github.com/pypa/sampleproject/issues"
+"Bug Reports" = "https://github.com/Friskes/drf-spectacular-websocket/issues"
 "Source" = "https://github.com/Friskes/drf-spectacular-websocket/"
 
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
```

### Comparing `drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/decorators.py` & `drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/decorators.py`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/schemas/consumer_schema.py` & `drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/schemas/consumer_schema.py`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/schemas/schema.py` & `drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/schemas/schema.py`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/settings.py` & `drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/settings.py`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket.egg-info/PKG-INFO` & `drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf_spectacular_websocket
-Version: 1.2.1
+Version: 1.2.3
 Summary: Extend websocket schema decorator for Django Channels
 Author-email: Friskes <friskesx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Friskes
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,15 +22,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/Friskes/drf-spectacular-websocket
-Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
+Project-URL: Bug Reports, https://github.com/Friskes/drf-spectacular-websocket/issues
 Project-URL: Source, https://github.com/Friskes/drf-spectacular-websocket/
 Keywords: Django,DRF,Spectacular,Swagger,Channels
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket.egg-info/SOURCES.txt` & `drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

