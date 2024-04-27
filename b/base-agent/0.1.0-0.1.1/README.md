# Comparing `tmp/base-agent-0.1.0.tar.gz` & `tmp/base-agent-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "base-agent-0.1.0.tar", last modified: Fri Apr 26 16:09:08 2024, max compression
+gzip compressed data, was "base-agent-0.1.1.tar", last modified: Sat Apr 27 17:29:09 2024, max compression
```

## Comparing `base-agent-0.1.0.tar` & `base-agent-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-26 16:09:08.562787 base-agent-0.1.0/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1073 2024-04-26 15:56:35.000000 base-agent-0.1.0/LICENSE
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1994 2024-04-26 16:09:08.562653 base-agent-0.1.0/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1441 2024-04-26 16:02:49.000000 base-agent-0.1.0/README.md
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-26 16:09:08.561433 base-agent-0.1.0/base_agent/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      399 2024-04-26 15:59:12.000000 base-agent-0.1.0/base_agent/__init__.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-26 16:09:08.562134 base-agent-0.1.0/base_agent.egg-info/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1994 2024-04-26 16:09:08.000000 base-agent-0.1.0/base_agent.egg-info/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      228 2024-04-26 16:09:08.000000 base-agent-0.1.0/base_agent.egg-info/SOURCES.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2024-04-26 16:09:08.000000 base-agent-0.1.0/base_agent.egg-info/dependency_links.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       17 2024-04-26 16:09:08.000000 base-agent-0.1.0/base_agent.egg-info/top_level.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-04-26 16:09:08.562828 base-agent-0.1.0/setup.cfg
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      711 2024-04-26 16:02:16.000000 base-agent-0.1.0/setup.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-26 16:09:08.562370 base-agent-0.1.0/tests/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-26 15:58:44.000000 base-agent-0.1.0/tests/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      625 2024-04-26 16:02:16.000000 base-agent-0.1.0/tests/test_base_agent.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-27 17:29:09.294791 base-agent-0.1.1/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1073 2024-04-26 15:56:35.000000 base-agent-0.1.1/LICENSE
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2294 2024-04-27 17:29:09.294639 base-agent-0.1.1/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1741 2024-04-27 17:28:51.000000 base-agent-0.1.1/README.md
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-27 17:29:09.293189 base-agent-0.1.1/base_agent/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      399 2024-04-26 15:59:12.000000 base-agent-0.1.1/base_agent/__init__.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-27 17:29:09.294065 base-agent-0.1.1/base_agent.egg-info/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2294 2024-04-27 17:29:09.000000 base-agent-0.1.1/base_agent.egg-info/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      228 2024-04-27 17:29:09.000000 base-agent-0.1.1/base_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2024-04-27 17:29:09.000000 base-agent-0.1.1/base_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       17 2024-04-27 17:29:09.000000 base-agent-0.1.1/base_agent.egg-info/top_level.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-04-27 17:29:09.294838 base-agent-0.1.1/setup.cfg
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      711 2024-04-27 17:29:05.000000 base-agent-0.1.1/setup.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-27 17:29:09.294293 base-agent-0.1.1/tests/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-26 15:58:44.000000 base-agent-0.1.1/tests/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      625 2024-04-26 16:02:16.000000 base-agent-0.1.1/tests/test_base_agent.py
```

### Comparing `base-agent-0.1.0/LICENSE` & `base-agent-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `base-agent-0.1.0/PKG-INFO` & `base-agent-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: base-agent
-Version: 0.1.0
+Version: 0.1.1
 Summary: An abstract base class for building various agent-based systems.
 Home-page: https://github.com/chigwell/BaseAgent
 Author: Eugene Evstafev
 Author-email: chigwel@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/base-agent.svg)](https://badge.fury.io/py/base-agent)
+[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
+[![Downloads](https://static.pepy.tech/badge/base-agent)](https://pepy.tech/project/base-agent)
+
 # BaseAgent
 
 `BaseAgent` is an abstract base class designed to support the development of various agent-based systems. It provides a structured approach to creating agents with initialization, execution, and cleanup phases.
 
 ## Installation
 
 To install `BaseAgent`, you can use pip directly from GitHub:
```

### Comparing `base-agent-0.1.0/README.md` & `base-agent-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+[![PyPI version](https://badge.fury.io/py/base-agent.svg)](https://badge.fury.io/py/base-agent)
+[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
+[![Downloads](https://static.pepy.tech/badge/base-agent)](https://pepy.tech/project/base-agent)
+
 # BaseAgent
 
 `BaseAgent` is an abstract base class designed to support the development of various agent-based systems. It provides a structured approach to creating agents with initialization, execution, and cleanup phases.
 
 ## Installation
 
 To install `BaseAgent`, you can use pip directly from GitHub:
```

### Comparing `base-agent-0.1.0/base_agent.egg-info/PKG-INFO` & `base-agent-0.1.1/base_agent.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: base-agent
-Version: 0.1.0
+Version: 0.1.1
 Summary: An abstract base class for building various agent-based systems.
 Home-page: https://github.com/chigwell/BaseAgent
 Author: Eugene Evstafev
 Author-email: chigwel@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/base-agent.svg)](https://badge.fury.io/py/base-agent)
+[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
+[![Downloads](https://static.pepy.tech/badge/base-agent)](https://pepy.tech/project/base-agent)
+
 # BaseAgent
 
 `BaseAgent` is an abstract base class designed to support the development of various agent-based systems. It provides a structured approach to creating agents with initialization, execution, and cleanup phases.
 
 ## Installation
 
 To install `BaseAgent`, you can use pip directly from GitHub:
```

### Comparing `base-agent-0.1.0/setup.py` & `base-agent-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='base-agent',
-    version='0.1.0',
+    version='0.1.1',
     author='Eugene Evstafev',
     author_email='chigwel@gmail.com',
     description='An abstract base class for building various agent-based systems.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/chigwell/BaseAgent',
     packages=find_packages(),
```

### Comparing `base-agent-0.1.0/tests/test_base_agent.py` & `base-agent-0.1.1/tests/test_base_agent.py`

 * *Files identical despite different names*

