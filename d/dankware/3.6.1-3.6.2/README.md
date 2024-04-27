# Comparing `tmp/dankware-3.6.1.tar.gz` & `tmp/dankware-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dankware-3.6.1.tar", last modified: Tue Apr 16 05:56:54 2024, max compression
+gzip compressed data, was "dankware-3.6.2.tar", last modified: Sat Apr 27 05:44:46 2024, max compression
```

## Comparing `dankware-3.6.1.tar` & `dankware-3.6.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:56:54.500334 dankware-3.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-16 05:56:50.000000 dankware-3.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17083 2024-04-16 05:56:54.500334 dankware-3.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15942 2024-04-16 05:56:50.000000 dankware-3.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:56:54.500334 dankware-3.6.1/dankware/
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-16 05:56:50.000000 dankware-3.6.1/dankware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-16 05:56:50.000000 dankware-3.6.1/dankware/ctypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-16 05:56:50.000000 dankware-3.6.1/dankware/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-16 05:56:50.000000 dankware-3.6.1/dankware/multithread.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-16 05:56:50.000000 dankware-3.6.1/dankware/pillow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-16 05:56:50.000000 dankware-3.6.1/dankware/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-16 05:56:50.000000 dankware-3.6.1/dankware/terminal.py
--rw-r--r--   0 runner    (1001) docker     (127)    16764 2024-04-16 05:56:50.000000 dankware-3.6.1/dankware/text.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-16 05:56:50.000000 dankware-3.6.1/dankware/tkinter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-16 05:56:50.000000 dankware-3.6.1/dankware/traceback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-04-16 05:56:50.000000 dankware-3.6.1/dankware/winreg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:56:54.500334 dankware-3.6.1/dankware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17083 2024-04-16 05:56:54.000000 dankware-3.6.1/dankware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-16 05:56:54.000000 dankware-3.6.1/dankware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 05:56:54.000000 dankware-3.6.1/dankware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-16 05:56:54.000000 dankware-3.6.1/dankware.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 05:56:54.000000 dankware-3.6.1/dankware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 05:56:54.500334 dankware-3.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-16 05:56:50.000000 dankware-3.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 05:44:46.510240 dankware-3.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 05:44:42.000000 dankware-3.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17083 2024-04-27 05:44:46.510240 dankware-3.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15942 2024-04-27 05:44:42.000000 dankware-3.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 05:44:46.506240 dankware-3.6.2/dankware/
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-27 05:44:42.000000 dankware-3.6.2/dankware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-27 05:44:42.000000 dankware-3.6.2/dankware/ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-27 05:44:42.000000 dankware-3.6.2/dankware/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-27 05:44:42.000000 dankware-3.6.2/dankware/multithread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-27 05:44:42.000000 dankware-3.6.2/dankware/pillow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-27 05:44:42.000000 dankware-3.6.2/dankware/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-27 05:44:42.000000 dankware-3.6.2/dankware/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16764 2024-04-27 05:44:42.000000 dankware-3.6.2/dankware/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-27 05:44:42.000000 dankware-3.6.2/dankware/tkinter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-27 05:44:42.000000 dankware-3.6.2/dankware/traceback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-04-27 05:44:42.000000 dankware-3.6.2/dankware/winreg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 05:44:46.510240 dankware-3.6.2/dankware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17083 2024-04-27 05:44:46.000000 dankware-3.6.2/dankware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-27 05:44:46.000000 dankware-3.6.2/dankware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 05:44:46.000000 dankware-3.6.2/dankware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-27 05:44:46.000000 dankware-3.6.2/dankware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-27 05:44:46.000000 dankware-3.6.2/dankware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 05:44:46.510240 dankware-3.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-27 05:44:42.000000 dankware-3.6.2/setup.py
```

### Comparing `dankware-3.6.1/LICENSE` & `dankware-3.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dankware-3.6.1/PKG-INFO` & `dankware-3.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dankware
-Version: 3.6.1
+Version: 3.6.2
 Summary: Python package with various features!
 Home-page: https://github.com/SirDank/dankware
 Author: SirDank
 Author-email: SirDankenstein@protonmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/SirDank/dankware
 Project-URL: Bug Tracker, https://github.com/SirDank/dankware/issues
```

### Comparing `dankware-3.6.1/README.md` & `dankware-3.6.2/README.md`

 * *Files identical despite different names*

### Comparing `dankware-3.6.1/dankware/__init__.py` & `dankware-3.6.2/dankware/__init__.py`

 * *Files identical despite different names*

### Comparing `dankware-3.6.1/dankware/ctypes.py` & `dankware-3.6.2/dankware/ctypes.py`

 * *Files identical despite different names*

### Comparing `dankware-3.6.1/dankware/datetime.py` & `dankware-3.6.2/dankware/datetime.py`

 * *Files identical despite different names*

### Comparing `dankware-3.6.1/dankware/multithread.py` & `dankware-3.6.2/dankware/multithread.py`

 * *Files identical despite different names*

### Comparing `dankware-3.6.1/dankware/pillow.py` & `dankware-3.6.2/dankware/pillow.py`

 * *Files identical despite different names*

### Comparing `dankware-3.6.1/dankware/requests.py` & `dankware-3.6.2/dankware/requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,18 +13,18 @@
     [ EXAMPLE ]
     ```python
     from dankware import github_downloads
     for _ in github_downloads("SirDank/dank.tool"): print(_)
     ```
     """
 
-    response = requests.get(f"https://api.github.com/repos/{user_repo}/releases/latest", headers = {"User-Agent": "dankware"}, timeout=3).json()
+    response = requests.get(f"https://api.github.com/repos/{user_repo}/releases/latest", headers = {"User-Agent": "dankware"}, timeout=3)
 
     if response.status_code == 200:
-        return tuple(data["browser_download_url"] for data in response["assets"])
+        return tuple(data["browser_download_url"] for data in response.json()["assets"])
     raise RuntimeError(f"Failed to get latest release from github: [{response.status_code}] {response.reason}")
 
 def github_file_selector(user_repo: str, filter_mode: str, filter_iterable: list[str] | tuple[str]) -> tuple[str]:
 
     """
     
     This function is used to filter the output from github_downloads()
```

### Comparing `dankware-3.6.1/dankware/terminal.py` & `dankware-3.6.2/dankware/terminal.py`

 * *Files identical despite different names*

### Comparing `dankware-3.6.1/dankware/text.py` & `dankware-3.6.2/dankware/text.py`

 * *Files identical despite different names*

### Comparing `dankware-3.6.1/dankware/tkinter.py` & `dankware-3.6.2/dankware/tkinter.py`

 * *Files identical despite different names*

### Comparing `dankware-3.6.1/dankware/traceback.py` & `dankware-3.6.2/dankware/traceback.py`

 * *Files identical despite different names*

### Comparing `dankware-3.6.1/dankware/winreg.py` & `dankware-3.6.2/dankware/winreg.py`

 * *Files identical despite different names*

### Comparing `dankware-3.6.1/dankware.egg-info/PKG-INFO` & `dankware-3.6.2/dankware.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dankware
-Version: 3.6.1
+Version: 3.6.2
 Summary: Python package with various features!
 Home-page: https://github.com/SirDank/dankware
 Author: SirDank
 Author-email: SirDankenstein@protonmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/SirDank/dankware
 Project-URL: Bug Tracker, https://github.com/SirDank/dankware/issues
```

### Comparing `dankware-3.6.1/setup.py` & `dankware-3.6.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
 
     license = "MIT",
     name = "dankware",
-    version = "3.6.1",
+    version = "3.6.2",
     author = "SirDank",
 
     author_email = "SirDankenstein@protonmail.com",
     description = "Python package with various features!",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type = "text/markdown",
     url = "https://github.com/SirDank/dankware",
```

