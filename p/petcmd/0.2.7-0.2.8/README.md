# Comparing `tmp/petcmd-0.2.7.tar.gz` & `tmp/petcmd-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petcmd-0.2.7.tar", last modified: Thu Mar 28 15:21:46 2024, max compression
+gzip compressed data, was "petcmd-0.2.8.tar", last modified: Sat Apr 27 18:50:05 2024, max compression
```

## Comparing `petcmd-0.2.7.tar` & `petcmd-0.2.8.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 maks       (501) staff       (20)        0 2024-03-28 15:21:46.656162 petcmd-0.2.7/
--rw-r--r--   0 maks       (501) staff       (20)     1063 2024-02-24 19:42:34.000000 petcmd-0.2.7/LICENSE
--rw-r--r--   0 maks       (501) staff       (20)     1666 2024-03-28 15:21:46.655962 petcmd-0.2.7/PKG-INFO
--rw-r--r--   0 maks       (501) staff       (20)     1218 2024-03-22 12:39:44.000000 petcmd-0.2.7/README.md
-drwxr-xr-x   0 maks       (501) staff       (20)        0 2024-03-28 15:21:46.655101 petcmd-0.2.7/petcmd/
--rw-r--r--   0 maks       (501) staff       (20)       97 2024-02-25 14:14:55.000000 petcmd-0.2.7/petcmd/__init__.py
--rw-r--r--   0 maks       (501) staff       (20)     8301 2024-03-22 12:30:30.000000 petcmd-0.2.7/petcmd/argparser.py
--rw-r--r--   0 maks       (501) staff       (20)     1033 2024-03-22 12:30:30.000000 petcmd-0.2.7/petcmd/command.py
--rw-r--r--   0 maks       (501) staff       (20)     3415 2024-03-28 11:26:11.000000 petcmd-0.2.7/petcmd/commander.py
--rw-r--r--   0 maks       (501) staff       (20)       86 2024-02-28 21:22:14.000000 petcmd-0.2.7/petcmd/exceptions.py
--rw-r--r--   0 maks       (501) staff       (20)     3206 2024-03-22 12:37:58.000000 petcmd-0.2.7/petcmd/interface.py
--rw-r--r--   0 maks       (501) staff       (20)      555 2024-02-28 22:39:47.000000 petcmd-0.2.7/petcmd/utils.py
-drwxr-xr-x   0 maks       (501) staff       (20)        0 2024-03-28 15:21:46.655810 petcmd-0.2.7/petcmd.egg-info/
--rw-r--r--   0 maks       (501) staff       (20)     1666 2024-03-28 15:21:46.000000 petcmd-0.2.7/petcmd.egg-info/PKG-INFO
--rw-r--r--   0 maks       (501) staff       (20)      286 2024-03-28 15:21:46.000000 petcmd-0.2.7/petcmd.egg-info/SOURCES.txt
--rw-r--r--   0 maks       (501) staff       (20)        1 2024-03-28 15:21:46.000000 petcmd-0.2.7/petcmd.egg-info/dependency_links.txt
--rw-r--r--   0 maks       (501) staff       (20)        7 2024-03-28 15:21:46.000000 petcmd-0.2.7/petcmd.egg-info/top_level.txt
--rw-r--r--   0 maks       (501) staff       (20)      569 2024-03-28 11:27:59.000000 petcmd-0.2.7/pyproject.toml
--rw-r--r--   0 maks       (501) staff       (20)       38 2024-03-28 15:21:46.656203 petcmd-0.2.7/setup.cfg
+drwxr-xr-x   0 maks       (501) staff       (20)        0 2024-04-27 18:50:05.338539 petcmd-0.2.8/
+-rw-r--r--   0 maks       (501) staff       (20)     1063 2024-02-24 19:42:34.000000 petcmd-0.2.8/LICENSE
+-rw-r--r--   0 maks       (501) staff       (20)     1666 2024-04-27 18:50:05.338285 petcmd-0.2.8/PKG-INFO
+-rw-r--r--   0 maks       (501) staff       (20)     1218 2024-03-22 12:39:44.000000 petcmd-0.2.8/README.md
+drwxr-xr-x   0 maks       (501) staff       (20)        0 2024-04-27 18:50:05.337207 petcmd-0.2.8/petcmd/
+-rw-r--r--   0 maks       (501) staff       (20)      179 2024-04-27 18:42:43.000000 petcmd-0.2.8/petcmd/__init__.py
+-rw-r--r--   0 maks       (501) staff       (20)     8301 2024-03-22 12:30:30.000000 petcmd-0.2.8/petcmd/argparser.py
+-rw-r--r--   0 maks       (501) staff       (20)     1033 2024-03-22 12:30:30.000000 petcmd-0.2.8/petcmd/command.py
+-rw-r--r--   0 maks       (501) staff       (20)     2643 2024-04-27 18:35:15.000000 petcmd-0.2.8/petcmd/commander.py
+-rw-r--r--   0 maks       (501) staff       (20)       86 2024-02-28 21:22:14.000000 petcmd-0.2.8/petcmd/exceptions.py
+-rw-r--r--   0 maks       (501) staff       (20)     3334 2024-04-27 18:39:06.000000 petcmd-0.2.8/petcmd/interface.py
+-rw-r--r--   0 maks       (501) staff       (20)     1225 2024-04-27 18:48:02.000000 petcmd-0.2.8/petcmd/single_command.py
+-rw-r--r--   0 maks       (501) staff       (20)     1282 2024-04-27 18:41:43.000000 petcmd-0.2.8/petcmd/utils.py
+drwxr-xr-x   0 maks       (501) staff       (20)        0 2024-04-27 18:50:05.338062 petcmd-0.2.8/petcmd.egg-info/
+-rw-r--r--   0 maks       (501) staff       (20)     1666 2024-04-27 18:50:05.000000 petcmd-0.2.8/petcmd.egg-info/PKG-INFO
+-rw-r--r--   0 maks       (501) staff       (20)      311 2024-04-27 18:50:05.000000 petcmd-0.2.8/petcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 maks       (501) staff       (20)        1 2024-04-27 18:50:05.000000 petcmd-0.2.8/petcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 maks       (501) staff       (20)        7 2024-04-27 18:50:05.000000 petcmd-0.2.8/petcmd.egg-info/top_level.txt
+-rw-r--r--   0 maks       (501) staff       (20)      569 2024-04-27 18:49:54.000000 petcmd-0.2.8/pyproject.toml
+-rw-r--r--   0 maks       (501) staff       (20)       38 2024-04-27 18:50:05.338594 petcmd-0.2.8/setup.cfg
```

### Comparing `petcmd-0.2.7/LICENSE` & `petcmd-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `petcmd-0.2.7/PKG-INFO` & `petcmd-0.2.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petcmd
-Version: 0.2.7
+Version: 0.2.8
 Summary: Library for creating a command line tools
 Author-email: Maks Vinnytskyi <ownerofforest@gmail.com>
 Project-URL: Homepage, https://gitlab.com/Tullp/petcmd
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
```

### Comparing `petcmd-0.2.7/README.md` & `petcmd-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `petcmd-0.2.7/petcmd/argparser.py` & `petcmd-0.2.8/petcmd/argparser.py`

 * *Files identical despite different names*

### Comparing `petcmd-0.2.7/petcmd/command.py` & `petcmd-0.2.8/petcmd/command.py`

 * *Files identical despite different names*

### Comparing `petcmd-0.2.7/petcmd/interface.py` & `petcmd-0.2.8/petcmd/interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 
+from __main__ import __file__ as main_file
+
 import os
 import re
 import sys
 import inspect
-from typing import Callable, Optional
+from typing import Optional
 
 from .command import Command
 from .utils import get_signature
 
 class Interface:
 
 	@classmethod
@@ -27,14 +29,16 @@
 
 	@classmethod
 	def command_usage(cls, command: Command):
 		positionals, keyword, defaults, spec = get_signature(command.func)
 		docs, args_docs = cls.__parse_doc(command.func.__doc__)
 
 		def command_name_view() -> str:
+			if command.cmds[0] == "__main__":
+				return os.path.basename(main_file).rsplit(".", 1)[0]
 			return command.cmds[0]
 
 		def positionals_view() -> str:
 			return " ".join(positionals)
 
 		def keywords_list_view() -> str:
 			return " ".join(f"[-{arg}]" for arg in keyword)
```

### Comparing `petcmd-0.2.7/petcmd.egg-info/PKG-INFO` & `petcmd-0.2.8/petcmd.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petcmd
-Version: 0.2.7
+Version: 0.2.8
 Summary: Library for creating a command line tools
 Author-email: Maks Vinnytskyi <ownerofforest@gmail.com>
 Project-URL: Homepage, https://gitlab.com/Tullp/petcmd
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
```

### Comparing `petcmd-0.2.7/pyproject.toml` & `petcmd-0.2.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "petcmd"
-version = "0.2.7"
+version = "0.2.8"
 authors = [
     { name = "Maks Vinnytskyi", email = "ownerofforest@gmail.com" },
 ]
 description = "Library for creating a command line tools"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

