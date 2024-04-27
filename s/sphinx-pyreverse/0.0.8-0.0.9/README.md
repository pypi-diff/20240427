# Comparing `tmp/sphinx-pyreverse-0.0.8.tar.gz` & `tmp/sphinx-pyreverse-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sphinx-pyreverse-0.0.8.tar", last modified: Tue Oct  2 14:34:47 2012, max compression
+gzip compressed data, was "dist/sphinx-pyreverse-0.0.9.tar", last modified: Tue Oct  2 14:44:02 2012, max compression
```

## Comparing `sphinx-pyreverse-0.0.8.tar` & `sphinx-pyreverse-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 alendit   (1000) alendit   (1000)        0 2012-10-02 14:34:47.000000 sphinx-pyreverse-0.0.8/
--rw-rw-r--   0 alendit   (1000) alendit   (1000)     1211 2012-10-02 14:34:47.000000 sphinx-pyreverse-0.0.8/PKG-INFO
--rw-rw-r--   0 alendit   (1000) alendit   (1000)       59 2012-10-02 14:34:47.000000 sphinx-pyreverse-0.0.8/setup.cfg
-drwxrwxr-x   0 alendit   (1000) alendit   (1000)        0 2012-10-02 14:34:47.000000 sphinx-pyreverse-0.0.8/sphinx-pyreverse/
--rw-rw-r--   0 alendit   (1000) alendit   (1000)        0 2012-10-02 09:59:23.000000 sphinx-pyreverse-0.0.8/sphinx-pyreverse/__init__.py
--rw-rw-r--   0 alendit   (1000) alendit   (1000)     1485 2012-10-02 14:32:41.000000 sphinx-pyreverse-0.0.8/sphinx-pyreverse/sphinx-pyreverse.py
--rw-rw-r--   0 alendit   (1000) alendit   (1000)       19 2012-10-02 13:49:24.000000 sphinx-pyreverse-0.0.8/MANIFEST.in
-drwxrwxr-x   0 alendit   (1000) alendit   (1000)        0 2012-10-02 14:34:47.000000 sphinx-pyreverse-0.0.8/sphinx_pyreverse.egg-info/
--rw-rw-r--   0 alendit   (1000) alendit   (1000)     1211 2012-10-02 14:34:47.000000 sphinx-pyreverse-0.0.8/sphinx_pyreverse.egg-info/PKG-INFO
--rw-rw-r--   0 alendit   (1000) alendit   (1000)      257 2012-10-02 14:34:47.000000 sphinx-pyreverse-0.0.8/sphinx_pyreverse.egg-info/SOURCES.txt
--rw-rw-r--   0 alendit   (1000) alendit   (1000)       17 2012-10-02 14:34:47.000000 sphinx-pyreverse-0.0.8/sphinx_pyreverse.egg-info/top_level.txt
--rw-rw-r--   0 alendit   (1000) alendit   (1000)        1 2012-10-02 14:34:47.000000 sphinx-pyreverse-0.0.8/sphinx_pyreverse.egg-info/dependency_links.txt
--rwxrwxr-x   0 alendit   (1000) alendit   (1000)     1009 2012-10-02 14:33:55.000000 sphinx-pyreverse-0.0.8/setup.py
--rw-rw-r--   0 alendit   (1000) alendit   (1000)      438 2012-10-02 12:26:06.000000 sphinx-pyreverse-0.0.8/README.rst
+drwxrwxr-x   0 alendit   (1000) alendit   (1000)        0 2012-10-02 14:44:02.000000 sphinx-pyreverse-0.0.9/
+-rw-rw-r--   0 alendit   (1000) alendit   (1000)     1211 2012-10-02 14:44:02.000000 sphinx-pyreverse-0.0.9/PKG-INFO
+-rw-rw-r--   0 alendit   (1000) alendit   (1000)       59 2012-10-02 14:44:02.000000 sphinx-pyreverse-0.0.9/setup.cfg
+drwxrwxr-x   0 alendit   (1000) alendit   (1000)        0 2012-10-02 14:44:02.000000 sphinx-pyreverse-0.0.9/sphinx_pyreverse/
+-rw-rw-r--   0 alendit   (1000) alendit   (1000)        0 2012-10-02 09:59:23.000000 sphinx-pyreverse-0.0.9/sphinx_pyreverse/__init__.py
+-rw-rw-r--   0 alendit   (1000) alendit   (1000)     1485 2012-10-02 14:32:41.000000 sphinx-pyreverse-0.0.9/sphinx_pyreverse/sphinx_pyreverse.py
+-rw-rw-r--   0 alendit   (1000) alendit   (1000)       19 2012-10-02 13:49:24.000000 sphinx-pyreverse-0.0.9/MANIFEST.in
+drwxrwxr-x   0 alendit   (1000) alendit   (1000)        0 2012-10-02 14:44:02.000000 sphinx-pyreverse-0.0.9/sphinx_pyreverse.egg-info/
+-rw-rw-r--   0 alendit   (1000) alendit   (1000)     1211 2012-10-02 14:44:02.000000 sphinx-pyreverse-0.0.9/sphinx_pyreverse.egg-info/PKG-INFO
+-rw-rw-r--   0 alendit   (1000) alendit   (1000)      257 2012-10-02 14:44:02.000000 sphinx-pyreverse-0.0.9/sphinx_pyreverse.egg-info/SOURCES.txt
+-rw-rw-r--   0 alendit   (1000) alendit   (1000)       17 2012-10-02 14:44:02.000000 sphinx-pyreverse-0.0.9/sphinx_pyreverse.egg-info/top_level.txt
+-rw-rw-r--   0 alendit   (1000) alendit   (1000)        1 2012-10-02 14:44:02.000000 sphinx-pyreverse-0.0.9/sphinx_pyreverse.egg-info/dependency_links.txt
+-rwxrwxr-x   0 alendit   (1000) alendit   (1000)     1009 2012-10-02 14:43:38.000000 sphinx-pyreverse-0.0.9/setup.py
+-rw-rw-r--   0 alendit   (1000) alendit   (1000)      438 2012-10-02 12:26:06.000000 sphinx-pyreverse-0.0.9/README.rst
```

### Comparing `sphinx-pyreverse-0.0.8/PKG-INFO` & `sphinx-pyreverse-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sphinx-pyreverse
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple sphinx extension to generate UML diagrams with pyreverse
 Home-page: https://github.com/alendit/sphinx-pyreverse
 Author: Dimitri Vorona
 Author-email: vorona@in.tum.de
 License: GPLv3
 Description: Sphinx-pyreverse
         =================
```

### Comparing `sphinx-pyreverse-0.0.8/sphinx-pyreverse/sphinx-pyreverse.py` & `sphinx-pyreverse-0.0.9/sphinx_pyreverse/sphinx_pyreverse.py`

 * *Files identical despite different names*

### Comparing `sphinx-pyreverse-0.0.8/sphinx_pyreverse.egg-info/PKG-INFO` & `sphinx-pyreverse-0.0.9/sphinx_pyreverse.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sphinx-pyreverse
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple sphinx extension to generate UML diagrams with pyreverse
 Home-page: https://github.com/alendit/sphinx-pyreverse
 Author: Dimitri Vorona
 Author-email: vorona@in.tum.de
 License: GPLv3
 Description: Sphinx-pyreverse
         =================
```

### Comparing `sphinx-pyreverse-0.0.8/setup.py` & `sphinx-pyreverse-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 from setuptools import setup
 import os
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(name="sphinx-pyreverse",
-      version="0.0.8",
+      version="0.0.9",
       author="Dimitri Vorona",
       author_email="vorona@in.tum.de",
       description=("A simple sphinx extension to generate "
                     "UML diagrams with pyreverse"),
       license="GPLv3",
       keywords="sphinx extension uml pyreverse",
       url="https://github.com/alendit/sphinx-pyreverse",
       long_description=read('README.rst'),
-      packages=['sphinx-pyreverse'],
+      packages=['sphinx_pyreverse'],
       classifiers=[
                    'Development Status :: 2 - Pre-Alpha',
                    'Intended Audience :: Information Technology',
                    'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
                    'Programming Language :: Python',
                    'Topic :: Utilities',
                    ]
```

