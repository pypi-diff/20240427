# Comparing `tmp/froggius-0.1.6.post3.tar.gz` & `tmp/froggius-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "froggius-0.1.6.post3.tar", last modified: Mon Apr  8 16:02:53 2024, max compression
+gzip compressed data, was "froggius-0.1.7.tar", last modified: Sat Apr 27 11:28:00 2024, max compression
```

## Comparing `froggius-0.1.6.post3.tar` & `froggius-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:02:53.065500 froggius-0.1.6.post3/
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-08 16:02:31.000000 froggius-0.1.6.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-08 16:02:53.061500 froggius-0.1.6.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-08 16:02:31.000000 froggius-0.1.6.post3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:02:53.061500 froggius-0.1.6.post3/froggius/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-08 16:02:48.000000 froggius-0.1.6.post3/froggius/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-08 16:02:48.000000 froggius-0.1.6.post3/froggius/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:02:53.061500 froggius-0.1.6.post3/froggius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-08 16:02:53.000000 froggius-0.1.6.post3/froggius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-08 16:02:53.000000 froggius-0.1.6.post3/froggius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:02:53.000000 froggius-0.1.6.post3/froggius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 16:02:53.000000 froggius-0.1.6.post3/froggius.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 16:02:53.065500 froggius-0.1.6.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-08 16:02:48.000000 froggius-0.1.6.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 11:28:00.237716 froggius-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-27 11:27:54.000000 froggius-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-27 11:28:00.237716 froggius-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-04-27 11:27:54.000000 froggius-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 11:28:00.237716 froggius-0.1.7/froggius/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-27 11:27:57.000000 froggius-0.1.7/froggius/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10801 2024-04-27 11:27:57.000000 froggius-0.1.7/froggius/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 11:28:00.237716 froggius-0.1.7/froggius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-27 11:28:00.000000 froggius-0.1.7/froggius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-27 11:28:00.000000 froggius-0.1.7/froggius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 11:28:00.000000 froggius-0.1.7/froggius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-27 11:28:00.000000 froggius-0.1.7/froggius.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 11:28:00.237716 froggius-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-27 11:27:57.000000 froggius-0.1.7/setup.py
```

### Comparing `froggius-0.1.6.post3/LICENSE` & `froggius-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `froggius-0.1.6.post3/PKG-INFO` & `froggius-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: froggius
-Version: 0.1.6.post3
+Version: 0.1.7
 Summary: Froggius is a lightweight and dumb easy logging libary for python
 Home-page: https://github.com/zlElo/Froggius
 Author: zlElo
 Author-email: mail@zlelo.de
 License: MPL-2.0
 Keywords: logging,logger,easy-to-use,log
 Classifier: Intended Audience :: Developers
@@ -20,14 +20,15 @@
 </p>
 
 <p align="center">
   <img src="https://img.shields.io/github/languages/code-size/zlElo/Froggius" alt="GitHub code size in bytes" />
   <img src="https://img.shields.io/github/last-commit/zlElo/Froggius" alt="GitHub last commit" />
   <img src="https://img.shields.io/github/commit-activity/m/zlElo/Froggius" alt="GitHub commit activity month" />
   <img src="https://img.shields.io/github/license/zlElo/Froggius" alt="GitHub license" />
+  <a href="https://pepy.tech/project/structlog"><img src="https://static.pepy.tech/personalized-badge/froggius?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads%20/%20Month" alt="Downloads per month" /></a>
 </p>
 
 # Froggius
 Froggius is a lightweight and dumb easy logging libary for python
 
 ---------
 
@@ -39,19 +40,20 @@
 
 <p align="center">
   <img src="https://github.com/zlElo/Froggius/blob/main/res/tests/froggius_exec.png?raw=true" style="width: 770px">
 </p>
 
 This example runs following debug command 60 times and prints every time the log to the console and stdout:
 ```py
-frogger.debug('Example Debug Message')
+logger.debug('Example Debug Message')
 ```
 
 This massive speed improvement helps your program, to log like you need it without performance disadvantages.
 
+System informations: MacOS Sonoma 14.4.1, MacBook Air M2, Python 3.12.1
 ## Installation
 You can install Froggius with following command:
 ```
 pip install froggius
 ```
 
 Alternatively you can clone this repository and install then:
```

### Comparing `froggius-0.1.6.post3/README.md` & `froggius-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 </p>
 
 <p align="center">
   <img src="https://img.shields.io/github/languages/code-size/zlElo/Froggius" alt="GitHub code size in bytes" />
   <img src="https://img.shields.io/github/last-commit/zlElo/Froggius" alt="GitHub last commit" />
   <img src="https://img.shields.io/github/commit-activity/m/zlElo/Froggius" alt="GitHub commit activity month" />
   <img src="https://img.shields.io/github/license/zlElo/Froggius" alt="GitHub license" />
+  <a href="https://pepy.tech/project/structlog"><img src="https://static.pepy.tech/personalized-badge/froggius?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads%20/%20Month" alt="Downloads per month" /></a>
 </p>
 
 # Froggius
 Froggius is a lightweight and dumb easy logging libary for python
 
 ---------
 
@@ -22,19 +23,20 @@
 
 <p align="center">
   <img src="https://github.com/zlElo/Froggius/blob/main/res/tests/froggius_exec.png?raw=true" style="width: 770px">
 </p>
 
 This example runs following debug command 60 times and prints every time the log to the console and stdout:
 ```py
-frogger.debug('Example Debug Message')
+logger.debug('Example Debug Message')
 ```
 
 This massive speed improvement helps your program, to log like you need it without performance disadvantages.
 
+System informations: MacOS Sonoma 14.4.1, MacBook Air M2, Python 3.12.1
 ## Installation
 You can install Froggius with following command:
 ```
 pip install froggius
 ```
 
 Alternatively you can clone this repository and install then:
```

### Comparing `froggius-0.1.6.post3/froggius/logger.py` & `froggius-0.1.7/froggius/logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,25 +9,20 @@
 
 class Froggius:
     """
     Main class of Froggius
     Includes logging methods
     """
 
-    def __init__(self, file_path=None, print_out=None) -> None:
-        if file_path is not None:
-            self.glob_file_path = file_path
-        else:
-            self.glob_file_path = None
-        if print_out is not None:
-            self.glob_print_out = print_out
-        else:
-            self.glob_print_out = None
+    def __init__(self, file_path=None, print_out=None, date_format=None) -> None:
+        self.glob_file_path = file_path
+        self.glob_print_out = print_out
+        self.glob_date_format = date_format
 
-    def debug(self, log_msg, file_path=None, print_out=None):
+    def debug(self, log_msg, file_path=None, print_out=None, date_format=None):
         """
         Writes logs, optionally to a file.
 
         Parameters
         ----------
         log_msg : str
             The message to be logged.
@@ -35,38 +30,47 @@
             The path to the file where the log should be saved, by default None
         highliting : bool, optional
             Whether the DEBUG tag should be highlighted with ANSI escape sequences, by default True
         print_out : bool, optional
             Whether the log should be printed to the stdout, by default True
         """
         current_date = datetime.datetime.now()
-        log_string = f'[DBG] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
+        if date_format is None:
+            if self.glob_date_format is not None:
+                date_format = self.glob_date_format
+            else:
+                date_format = "%Y/%m/%d %H:%M:%S"
+        log_string = f"[DBG] [{current_date.strftime(date_format)}] {log_msg}"
 
         # check for vars for filepath
         if self.glob_file_path is not None and file_path is None:
             file_path = self.glob_file_path
 
         if file_path is not None:
             with open(file_path, "a") as log:
-                log.write(
-                    f'\n[DBG] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
-                )
+                log.write(f"\n[DBG] [{current_date.strftime(date_format)}] {log_msg}")
 
         if self.glob_print_out:
             if print_out == False:
                 pass
             else:
                 print(log_string, file=sys.stdout)
         if print_out and not self.glob_print_out:
             print(log_string, file=sys.stdout)
         if self.glob_print_out is None and print_out is None:
             print(log_string, file=sys.stdout)
 
     def error(
-        self, log_msg, file_path=None, highlighting=True, print_out=None, line=None
+        self,
+        log_msg,
+        file_path=None,
+        highlighting=True,
+        print_out=None,
+        line=None,
+        date_format=None,
     ):
         """
         Writes errors, optionally to a file.
 
         Parameters
         ----------
         log_msg : str
@@ -82,27 +86,33 @@
             A list containing information about the line where the error occurred,
             by default None. The list should contain [line number, file name,
             function name].
         """
 
         # get datetime
         current_date = datetime.datetime.now()
+        if date_format is None:
+            if self.glob_date_format is not None:
+                date_format = self.glob_date_format
+            else:
+                date_format = "%Y/%m/%d %H:%M:%S"
+
         if highlighting:
-            log_string = f'[\033[91mERR\033[0m] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg} {f"| Occured on line: {line[0]} in {line[1]}, {line[2]}()" if line is not None else ""}'
+            log_string = f'[\033[91mERR\033[0m] [{current_date.strftime(date_format)}] {log_msg} {f"| Occured on line: {line[0]} in {line[1]}, {line[2]}()" if line is not None else ""}'
         else:
-            log_string = f'[ERR] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg} {f"| Occured on line: {line[0]} in {line[1]}, {line[2]}()" if line is not None else ""}'
+            log_string = f'[ERR] [{current_date.strftime(date_format)}] {log_msg} {f"| Occured on line: {line[0]} in {line[1]}, {line[2]}()" if line is not None else ""}'
 
         # check for filepath
         if self.glob_file_path is not None and file_path is None:
             file_path = self.glob_file_path
 
         if file_path is not None:
             with open(file_path, "a") as log:
                 log.write(
-                    f'\n[ERR] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg} {f"| Occured on line: {line[0]} in {line[1]}, {line[2]}()" if line is not None else ""}'
+                    f'\n[ERR] [{current_date.strftime(date_format)}] {log_msg} {f"| Occured on line: {line[0]} in {line[1]}, {line[2]}()" if line is not None else ""}'
                 )
 
         if self.glob_print_out:
             if print_out == False:
                 pass
             else:
                 print(log_string, file=sys.stderr)
@@ -162,85 +172,123 @@
                     if not continue_onexpception:
                         raise e
 
             return wrapper
 
         return decorator
 
-    def information(self, log_msg, file_path=None, highlighting=True, print_out=None):
+    def information(
+        self,
+        log_msg,
+        file_path=None,
+        highlighting=True,
+        print_out=None,
+        date_format=None,
+    ):
         """
         A function to log information with optional file output and highlighting.
 
         Parameters:
             log_msg (str): The message to be logged.
             file_path (str, optional): The file path to log to. Defaults to None.
             highlighting (bool, optional): Whether to highlight the log message. Defaults to True.
             print_out (bool, optional): Whether to print the log message. Defaults to True.
         """
 
         current_date = datetime.datetime.now()
+        if date_format is None:
+            if self.glob_date_format is not None:
+                date_format = self.glob_date_format
+            else:
+                date_format = "%Y/%m/%d %H:%M:%S"
 
         if highlighting:
-            log_string = f'[\033[32mINF\033[0m] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
-        else:
             log_string = (
-                f'[INF] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
+                f"[\033[32mINF\033[0m] [{current_date.strftime(date_format)}] {log_msg}"
             )
+        else:
+            log_string = f"[INF] [{current_date.strftime(date_format)}] {log_msg}"
 
         # check for filepath
         if self.glob_file_path is not None and file_path is None:
             file_path = self.glob_file_path
 
         if file_path is not None:
             with open(file_path, "a") as log:
-                log.write(
-                    f'\n[INF] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
-                )
+                log.write(f"\n[INF] [{current_date.strftime(date_format)}] {log_msg}")
 
         if self.glob_print_out:
             if print_out == False:
                 pass
             else:
                 print(log_string, file=sys.stdout)
         if print_out and not self.glob_print_out:
             print(log_string, file=sys.stdout)
         if self.glob_print_out is None and print_out is None:
             print(log_string, file=sys.stdout)
 
-    def info(self, log_msg, file_path=None, highlighting=True, print_out=None):
-        return self.information(log_msg, file_path, highlighting, print_out)
+    def info(
+        self,
+        log_msg,
+        file_path=None,
+        highlighting=True,
+        print_out=None,
+        date_format=None,
+    ):
+        """
+        A function to log information with optional file output and highlighting.
 
-    def warning(self, log_msg, file_path=None, highlighting=True, print_out=None):
+        Parameters:
+            log_msg (str): The message to be logged.
+            file_path (str, optional): The file path to log to. Defaults to None.
+            highlighting (bool, optional): Whether to highlight the log message. Defaults to True.
+            print_out (bool, optional): Whether to print the log message. Defaults to True.
+        """
+        return self.information(
+            log_msg, file_path, highlighting, print_out, date_format
+        )
+
+    def warning(
+        self,
+        log_msg,
+        file_path=None,
+        highlighting=True,
+        print_out=None,
+        date_format=None,
+    ):
         """
         Logs a warning message with an optional file path, highlighting, and print out.
 
         Parameters:
             log_msg (str): The warning message to be logged.
             file_path (str, optional): The file path to write the log message to. Defaults to None.
             highlighting (bool, optional): Whether to highlight the log message. Defaults to True.
             print_out (bool, optional): Whether to print the log message to the console. Defaults to True.
         """
         current_date = datetime.datetime.now()
+        if date_format is None:
+            if self.glob_date_format is not None:
+                date_format = self.glob_date_format
+            else:
+                date_format = "%Y/%m/%d %H:%M:%S"
 
         if highlighting:
-            log_string = f'[\033[93mWRN\033[0m] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
-        else:
             log_string = (
-                f'[WRN] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
+                f"[\033[93mWRN\033[0m] [{current_date.strftime(date_format)}] {log_msg}"
             )
+        else:
+            log_string = f"[WRN] [{current_date.strftime(date_format)}] {log_msg}"
 
         # check for filepath
         if self.glob_file_path is not None and file_path is None:
             file_path = self.glob_file_path
 
         if file_path is not None:
             with open(file_path, "a") as log:
-                log.write(
-                    f'\n[WRN] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
-                )
+                log.write(f"\n[WRN] [{current_date.strftime(date_format)}] {log_msg}")
 
         if self.glob_print_out:
             if print_out == False:
                 pass
             else:
                 print(log_string, file=sys.stdout)
         if print_out and not self.glob_print_out:
```

### Comparing `froggius-0.1.6.post3/froggius.egg-info/PKG-INFO` & `froggius-0.1.7/froggius.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: froggius
-Version: 0.1.6.post3
+Version: 0.1.7
 Summary: Froggius is a lightweight and dumb easy logging libary for python
 Home-page: https://github.com/zlElo/Froggius
 Author: zlElo
 Author-email: mail@zlelo.de
 License: MPL-2.0
 Keywords: logging,logger,easy-to-use,log
 Classifier: Intended Audience :: Developers
@@ -20,14 +20,15 @@
 </p>
 
 <p align="center">
   <img src="https://img.shields.io/github/languages/code-size/zlElo/Froggius" alt="GitHub code size in bytes" />
   <img src="https://img.shields.io/github/last-commit/zlElo/Froggius" alt="GitHub last commit" />
   <img src="https://img.shields.io/github/commit-activity/m/zlElo/Froggius" alt="GitHub commit activity month" />
   <img src="https://img.shields.io/github/license/zlElo/Froggius" alt="GitHub license" />
+  <a href="https://pepy.tech/project/structlog"><img src="https://static.pepy.tech/personalized-badge/froggius?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads%20/%20Month" alt="Downloads per month" /></a>
 </p>
 
 # Froggius
 Froggius is a lightweight and dumb easy logging libary for python
 
 ---------
 
@@ -39,19 +40,20 @@
 
 <p align="center">
   <img src="https://github.com/zlElo/Froggius/blob/main/res/tests/froggius_exec.png?raw=true" style="width: 770px">
 </p>
 
 This example runs following debug command 60 times and prints every time the log to the console and stdout:
 ```py
-frogger.debug('Example Debug Message')
+logger.debug('Example Debug Message')
 ```
 
 This massive speed improvement helps your program, to log like you need it without performance disadvantages.
 
+System informations: MacOS Sonoma 14.4.1, MacBook Air M2, Python 3.12.1
 ## Installation
 You can install Froggius with following command:
 ```
 pip install froggius
 ```
 
 Alternatively you can clone this repository and install then:
```

### Comparing `froggius-0.1.6.post3/setup.py` & `froggius-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 setup(
     name="froggius",
     packages=find_packages(include=["froggius"]),
     description="Froggius is a lightweight and dumb easy logging libary for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MPL-2.0",
-    version="0.1.6-3",
+    version="0.1.7",
     author="zlElo",
     author_email="mail@zlelo.de",
     url="https://github.com/zlElo/Froggius",
     keywords=["logging", "logger", "easy-to-use", "log"],
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
```

