# Comparing `tmp/evg-2.7.1.tar.gz` & `tmp/evg-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evg-2.7.1.tar", last modified: Fri Apr 19 21:40:22 2024, max compression
+gzip compressed data, was "evg-2.8.0.tar", last modified: Sat Apr 27 13:25:22 2024, max compression
```

## Comparing `evg-2.7.1.tar` & `evg-2.8.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 21:40:22.996633 evg-2.7.1/
--rw-rw-rw-   0        0        0     2133 2024-04-19 21:40:22.995357 evg-2.7.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-19 21:40:22.984867 evg-2.7.1/evg/
--rw-rw-rw-   0        0        0     1518 2023-02-03 11:35:46.000000 evg-2.7.1/evg/__init__.py
--rw-rw-rw-   0        0        0     3665 2024-04-19 21:37:37.000000 evg-2.7.1/evg/core.py
-drwxrwxrwx   0        0        0        0 2024-04-19 21:40:22.995357 evg-2.7.1/evg.egg-info/
--rw-rw-rw-   0        0        0     2133 2024-04-19 21:40:22.000000 evg-2.7.1/evg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2024-04-19 21:40:22.000000 evg-2.7.1/evg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 21:40:22.000000 evg-2.7.1/evg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-19 21:40:22.000000 evg-2.7.1/evg.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        4 2024-04-19 21:40:22.000000 evg-2.7.1/evg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 21:40:22.996633 evg-2.7.1/setup.cfg
--rw-rw-rw-   0        0        0      517 2024-04-19 21:21:19.000000 evg-2.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 13:25:22.777297 evg-2.8.0/
+-rw-rw-rw-   0        0        0     2133 2024-04-27 13:25:22.776300 evg-2.8.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-27 13:25:22.765899 evg-2.8.0/evg/
+-rw-rw-rw-   0        0        0     1552 2024-04-27 12:41:11.000000 evg-2.8.0/evg/__init__.py
+-rw-rw-rw-   0        0        0     4080 2024-04-27 13:16:02.000000 evg-2.8.0/evg/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 13:25:22.776300 evg-2.8.0/evg.egg-info/
+-rw-rw-rw-   0        0        0     2133 2024-04-27 13:25:22.000000 evg-2.8.0/evg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2024-04-27 13:25:22.000000 evg-2.8.0/evg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 13:25:22.000000 evg-2.8.0/evg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-27 13:25:22.000000 evg-2.8.0/evg.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        4 2024-04-27 13:25:22.000000 evg-2.8.0/evg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 13:25:22.777297 evg-2.8.0/setup.cfg
+-rw-rw-rw-   0        0        0      517 2024-04-27 13:24:39.000000 evg-2.8.0/setup.py
```

### Comparing `evg-2.7.1/PKG-INFO` & `evg-2.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evg
-Version: 2.7.1
+Version: 2.8.0
 Summary: Discord translator & translation of Discord functions/interactions
 Home-page: https://github.com/IceOne-i/evg
 Author: Nikita Belan
 Author-email: nikitabelan9@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `evg-2.7.1/evg/core.py` & `evg-2.8.0/evg/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 _script_dir = pathlib.Path(__file__).parent.resolve()
 default_language = "en-US"
 
 languages = {}
 
 default_text = "oOps"
+default_file_types = ["json"]
 
 
 class Helper:
     def __init__(self):
         pass
 
     @staticmethod
@@ -30,49 +31,57 @@
         directories = []
         for x in os.listdir(a):
             if Helper.check_directory(f"{path}/{x}"):
                 directories.append(x)
         return directories
 
     @staticmethod
-    def count_files(path: str, file_type: str = None) -> int:
-        a = f'{path}'
+    def count_files(path: str, file_types: Union[str, list[str], None] = None) -> int:
         count = 0
-        for x in os.listdir(a):
-            if Helper.check_file(f"{path}/{x}"):
-                if file_type is not None:
-                    if not x.endswith(file_type):
-                        continue
+        for x in os.listdir(path):
+            if Helper.check_file(f"{path}/{x}", file_types=file_types) is True:
                 count += 1
         return count
 
     @staticmethod
-    def files(path: str, file_type: str = None) -> list[str]:
-        a = f'{path}'
+    def files(path: str, file_types: Union[str, list[str], None] = None) -> list[str]:
         files = []
-        for x in os.listdir(a):
-            if Helper.check_file(f"{path}/{x}"):
-                if file_type is not None:
-                    if not x.endswith(file_type):
-                        continue
+        for x in os.listdir(path):
+            if Helper.check_file(f"{path}/{x}", file_types=file_types) is True:
                 files.append(x)
         return files
 
     @staticmethod
     def check_directory(path: str) -> bool:
         a = f'{path}'
         return os.path.isdir(a)
 
     @staticmethod
-    def check_file(path: str, file_type: str = None) -> bool:
-        a = f'{path}'
-        if file_type is not None:
-            if not path.endswith(file_type):
-                return False
-        return os.path.isfile(a)
+    def check_file_type(file_name: str, file_types: Union[str, list[str], None] = None) -> bool:
+        if file_types is None:
+            file_types = default_file_types
+        else:
+            if type(file_types) is str:
+                file_types = [file_types]
+        for x in file_types:
+            if file_name.endswith(f".{x}"):
+                return True
+            else:
+                continue
+        return False
+
+    @staticmethod
+    def check_file(file: str, file_types: Union[str, list[str], None] = None) -> bool:
+        if os.path.isfile(file):
+            if file_types is not None:
+                if Helper.check_file_type(file, file_types) is False:
+                    return False
+            return True
+        else:
+            return False
 
     @staticmethod
     def check_language(language: str) -> bool:
         if language in languages:
             return True
         return False
```

### Comparing `evg-2.7.1/evg.egg-info/PKG-INFO` & `evg-2.8.0/evg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evg
-Version: 2.7.1
+Version: 2.8.0
 Summary: Discord translator & translation of Discord functions/interactions
 Home-page: https://github.com/IceOne-i/evg
 Author: Nikita Belan
 Author-email: nikitabelan9@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `evg-2.7.1/setup.py` & `evg-2.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("../README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='evg',
-      version='2.7.1',
+      version='2.8.0',
       url='https://github.com/IceOne-i/evg',
       license='MIT',
       author='Nikita Belan',
       author_email='nikitabelan9@gmail.com',
       description='Discord translator & translation of Discord functions/interactions',
       long_description=long_description,
       long_description_content_type="text/markdown",
```

