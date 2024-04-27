# Comparing `tmp/pass50-0.0.1.tar.gz` & `tmp/pass50-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pass50-0.0.1.tar", last modified: Sat Apr 27 14:18:31 2024, max compression
+gzip compressed data, was "pass50-0.0.2.tar", last modified: Sat Apr 27 15:21:14 2024, max compression
```

## Comparing `pass50-0.0.1.tar` & `pass50-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zivmax    (1002) zivmax    (1002)        0 2024-04-27 14:18:31.021986 pass50-0.0.1/
--rw-r--r--   0 zivmax    (1002) zivmax    (1002)    35149 2024-04-27 12:27:19.000000 pass50-0.0.1/LICENSE
--rw-r--r--   0 zivmax    (1002) zivmax    (1002)     3279 2024-04-27 14:18:31.021986 pass50-0.0.1/PKG-INFO
--rw-r--r--   0 zivmax    (1002) zivmax    (1002)     2649 2024-04-27 13:21:10.000000 pass50-0.0.1/README.md
--rw-r--r--   0 zivmax    (1002) zivmax    (1002)      784 2024-04-27 14:09:07.000000 pass50-0.0.1/pyproject.toml
--rw-r--r--   0 zivmax    (1002) zivmax    (1002)       38 2024-04-27 14:18:31.021986 pass50-0.0.1/setup.cfg
-drwxr-xr-x   0 zivmax    (1002) zivmax    (1002)        0 2024-04-27 14:18:31.021986 pass50-0.0.1/src/
-drwxr-xr-x   0 zivmax    (1002) zivmax    (1002)        0 2024-04-27 14:18:31.021986 pass50-0.0.1/src/pass50/
--rw-r--r--   0 zivmax    (1002) zivmax    (1002)     8730 2024-04-27 14:17:30.000000 pass50-0.0.1/src/pass50/__init__.py
--rw-r--r--   0 zivmax    (1002) zivmax    (1002)     1540 2024-04-27 14:18:20.000000 pass50-0.0.1/src/pass50/args.py
--rw-r--r--   0 zivmax    (1002) zivmax    (1002)     5680 2024-04-27 14:17:30.000000 pass50-0.0.1/src/pass50/cmd50.py
--rw-r--r--   0 zivmax    (1002) zivmax    (1002)     1012 2024-04-27 13:41:17.000000 pass50-0.0.1/src/pass50/color.py
--rw-r--r--   0 zivmax    (1002) zivmax    (1002)     4232 2024-04-27 14:17:27.000000 pass50-0.0.1/src/pass50/runner50.py
-drwxr-xr-x   0 zivmax    (1002) zivmax    (1002)        0 2024-04-27 14:18:31.021986 pass50-0.0.1/src/pass50.egg-info/
--rw-r--r--   0 zivmax    (1002) zivmax    (1002)     3279 2024-04-27 14:18:31.000000 pass50-0.0.1/src/pass50.egg-info/PKG-INFO
--rw-r--r--   0 zivmax    (1002) zivmax    (1002)      343 2024-04-27 14:18:31.000000 pass50-0.0.1/src/pass50.egg-info/SOURCES.txt
--rw-r--r--   0 zivmax    (1002) zivmax    (1002)        1 2024-04-27 14:18:31.000000 pass50-0.0.1/src/pass50.egg-info/dependency_links.txt
--rw-r--r--   0 zivmax    (1002) zivmax    (1002)       64 2024-04-27 14:18:31.000000 pass50-0.0.1/src/pass50.egg-info/entry_points.txt
--rw-r--r--   0 zivmax    (1002) zivmax    (1002)       16 2024-04-27 14:18:31.000000 pass50-0.0.1/src/pass50.egg-info/requires.txt
--rw-r--r--   0 zivmax    (1002) zivmax    (1002)        7 2024-04-27 14:18:31.000000 pass50-0.0.1/src/pass50.egg-info/top_level.txt
+drwxr-xr-x   0 zivmax    (1002) zivmax    (1002)        0 2024-04-27 15:21:14.021632 pass50-0.0.2/
+-rw-r--r--   0 zivmax    (1002) zivmax    (1002)    35149 2024-04-27 12:27:19.000000 pass50-0.0.2/LICENSE
+-rw-r--r--   0 zivmax    (1002) zivmax    (1002)     3150 2024-04-27 15:21:14.021632 pass50-0.0.2/PKG-INFO
+-rw-r--r--   0 zivmax    (1002) zivmax    (1002)     2520 2024-04-27 15:17:54.000000 pass50-0.0.2/README.md
+-rw-r--r--   0 zivmax    (1002) zivmax    (1002)      784 2024-04-27 15:20:23.000000 pass50-0.0.2/pyproject.toml
+-rw-r--r--   0 zivmax    (1002) zivmax    (1002)       38 2024-04-27 15:21:14.021632 pass50-0.0.2/setup.cfg
+drwxr-xr-x   0 zivmax    (1002) zivmax    (1002)        0 2024-04-27 15:21:14.021632 pass50-0.0.2/src/
+drwxr-xr-x   0 zivmax    (1002) zivmax    (1002)        0 2024-04-27 15:21:14.021632 pass50-0.0.2/src/pass50/
+-rw-r--r--   0 zivmax    (1002) zivmax    (1002)     8730 2024-04-27 14:17:30.000000 pass50-0.0.2/src/pass50/__init__.py
+-rw-r--r--   0 zivmax    (1002) zivmax    (1002)     1412 2024-04-27 15:17:36.000000 pass50-0.0.2/src/pass50/args.py
+-rw-r--r--   0 zivmax    (1002) zivmax    (1002)     5680 2024-04-27 14:17:30.000000 pass50-0.0.2/src/pass50/cmd50.py
+-rw-r--r--   0 zivmax    (1002) zivmax    (1002)     1012 2024-04-27 13:41:17.000000 pass50-0.0.2/src/pass50/color.py
+-rw-r--r--   0 zivmax    (1002) zivmax    (1002)     4232 2024-04-27 14:17:27.000000 pass50-0.0.2/src/pass50/runner50.py
+drwxr-xr-x   0 zivmax    (1002) zivmax    (1002)        0 2024-04-27 15:21:14.021632 pass50-0.0.2/src/pass50.egg-info/
+-rw-r--r--   0 zivmax    (1002) zivmax    (1002)     3150 2024-04-27 15:21:14.000000 pass50-0.0.2/src/pass50.egg-info/PKG-INFO
+-rw-r--r--   0 zivmax    (1002) zivmax    (1002)      343 2024-04-27 15:21:14.000000 pass50-0.0.2/src/pass50.egg-info/SOURCES.txt
+-rw-r--r--   0 zivmax    (1002) zivmax    (1002)        1 2024-04-27 15:21:14.000000 pass50-0.0.2/src/pass50.egg-info/dependency_links.txt
+-rw-r--r--   0 zivmax    (1002) zivmax    (1002)       64 2024-04-27 15:21:14.000000 pass50-0.0.2/src/pass50.egg-info/entry_points.txt
+-rw-r--r--   0 zivmax    (1002) zivmax    (1002)       16 2024-04-27 15:21:14.000000 pass50-0.0.2/src/pass50.egg-info/requires.txt
+-rw-r--r--   0 zivmax    (1002) zivmax    (1002)        7 2024-04-27 15:21:14.000000 pass50-0.0.2/src/pass50.egg-info/top_level.txt
```

### Comparing `pass50-0.0.1/LICENSE` & `pass50-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pass50-0.0.1/PKG-INFO` & `pass50-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pass50
-Version: 0.0.1
+Version: 0.0.2
 Summary: A convinent tool to check and submit your codes to "CS50".
 Author-email: zivmax <zivmax@foxmail.com>
 Maintainer-email: zivmax <zivmax@foxmail.com>
 Project-URL: Repository, https://github.com/zivmax/pass50
 Project-URL: Issues, https://github.com/zivmax/pass50/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -23,15 +23,14 @@
 
 - **Auto-check**: Automatically run `check50` on specified assignments.
 - **Auto-submit**: Automatically run `submit50` for submissions.
 - **Custom Path**: Specify a relative or absolute path to the directory containing your project.
 - **Identifier Selection**: Choose whether to identify assignments by directory or file names.
 - **Course Selection**: Specify which CS50 course you are submitting for (e.g., `x` for CS50x).
 - **Logging**: Option to print detailed logs for debugging and verification purposes.
-- **Environment Initialization**: Prepare your environment for using `pass50`.
 
 ## Installation
 
 To install `pass50`, you can use `pip` 
 
 ```bash
 pip install pass50
@@ -56,15 +55,14 @@
   -i {d,f}, --identifier {d,f}
                         choose the identifier (dir's name or files' name) to generate slug.
   -C {x,p}, --course {x,p}
                         choose the course from cs50 you're taking.
   -l, --logs            print the logs of check50 & submit50.
   -upl, --unpassedLogs  print all logs of unpassed works at the bottom.
   -d, --dev             run in developing mode, printing all logs.
-  -I, --init            Init the env for the app.
 ```
 
 ## Example Commands
 
 - **Initialize the environment**:
   ```bash
   pass50 --init
```

### Comparing `pass50-0.0.1/README.md` & `pass50-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 - **Auto-check**: Automatically run `check50` on specified assignments.
 - **Auto-submit**: Automatically run `submit50` for submissions.
 - **Custom Path**: Specify a relative or absolute path to the directory containing your project.
 - **Identifier Selection**: Choose whether to identify assignments by directory or file names.
 - **Course Selection**: Specify which CS50 course you are submitting for (e.g., `x` for CS50x).
 - **Logging**: Option to print detailed logs for debugging and verification purposes.
-- **Environment Initialization**: Prepare your environment for using `pass50`.
 
 ## Installation
 
 To install `pass50`, you can use `pip` 
 
 ```bash
 pip install pass50
@@ -39,15 +38,14 @@
   -i {d,f}, --identifier {d,f}
                         choose the identifier (dir's name or files' name) to generate slug.
   -C {x,p}, --course {x,p}
                         choose the course from cs50 you're taking.
   -l, --logs            print the logs of check50 & submit50.
   -upl, --unpassedLogs  print all logs of unpassed works at the bottom.
   -d, --dev             run in developing mode, printing all logs.
-  -I, --init            Init the env for the app.
 ```
 
 ## Example Commands
 
 - **Initialize the environment**:
   ```bash
   pass50 --init
```

### Comparing `pass50-0.0.1/pyproject.toml` & `pass50-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pass50"
-version = "0.0.1"
+version = "0.0.2"
 authors = [{ name = "zivmax", email = "zivmax@foxmail.com" }]
 maintainers = [{ name = "zivmax", email = "zivmax@foxmail.com" }]
 description = "A convinent tool to check and submit your codes to \"CS50\"."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `pass50-0.0.1/src/pass50/__init__.py` & `pass50-0.0.2/src/pass50/__init__.py`

 * *Files identical despite different names*

### Comparing `pass50-0.0.1/src/pass50/args.py` & `pass50-0.0.2/src/pass50/args.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,16 +51,10 @@
 parser.add_argument(
     "-d",
     "--dev",
     default=False,
     action="store_true",
     help="run in developping mode, printing all logs.",
 )
-parser.add_argument(
-    "-I",
-    "--init",
-    default=False,
-    action="store_true",
-    help="Init the env for the app.",
-)
+
 
 args = parser.parse_args()
```

### Comparing `pass50-0.0.1/src/pass50/cmd50.py` & `pass50-0.0.2/src/pass50/cmd50.py`

 * *Files identical despite different names*

### Comparing `pass50-0.0.1/src/pass50/color.py` & `pass50-0.0.2/src/pass50/color.py`

 * *Files identical despite different names*

### Comparing `pass50-0.0.1/src/pass50/runner50.py` & `pass50-0.0.2/src/pass50/runner50.py`

 * *Files identical despite different names*

### Comparing `pass50-0.0.1/src/pass50.egg-info/PKG-INFO` & `pass50-0.0.2/src/pass50.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pass50
-Version: 0.0.1
+Version: 0.0.2
 Summary: A convinent tool to check and submit your codes to "CS50".
 Author-email: zivmax <zivmax@foxmail.com>
 Maintainer-email: zivmax <zivmax@foxmail.com>
 Project-URL: Repository, https://github.com/zivmax/pass50
 Project-URL: Issues, https://github.com/zivmax/pass50/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -23,15 +23,14 @@
 
 - **Auto-check**: Automatically run `check50` on specified assignments.
 - **Auto-submit**: Automatically run `submit50` for submissions.
 - **Custom Path**: Specify a relative or absolute path to the directory containing your project.
 - **Identifier Selection**: Choose whether to identify assignments by directory or file names.
 - **Course Selection**: Specify which CS50 course you are submitting for (e.g., `x` for CS50x).
 - **Logging**: Option to print detailed logs for debugging and verification purposes.
-- **Environment Initialization**: Prepare your environment for using `pass50`.
 
 ## Installation
 
 To install `pass50`, you can use `pip` 
 
 ```bash
 pip install pass50
@@ -56,15 +55,14 @@
   -i {d,f}, --identifier {d,f}
                         choose the identifier (dir's name or files' name) to generate slug.
   -C {x,p}, --course {x,p}
                         choose the course from cs50 you're taking.
   -l, --logs            print the logs of check50 & submit50.
   -upl, --unpassedLogs  print all logs of unpassed works at the bottom.
   -d, --dev             run in developing mode, printing all logs.
-  -I, --init            Init the env for the app.
 ```
 
 ## Example Commands
 
 - **Initialize the environment**:
   ```bash
   pass50 --init
```

