# Comparing `tmp/vbproblemcomposer-0.1.1.tar.gz` & `tmp/vbproblemcomposer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbproblemcomposer-0.1.1.tar", max compression
+gzip compressed data, was "vbproblemcomposer-0.1.2.tar", max compression
```

## Comparing `vbproblemcomposer-0.1.1.tar` & `vbproblemcomposer-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-27 07:36:49.362347 vbproblemcomposer-0.1.1/README.md
--rw-r--r--   0        0        0      375 2024-04-27 08:47:08.704359 vbproblemcomposer-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-27 07:36:49.362297 vbproblemcomposer-0.1.1/vbproblemcomposer/__init__.py
--rw-r--r--   0        0        0       59 2024-04-27 07:39:39.852664 vbproblemcomposer-0.1.1/vbproblemcomposer/__main__.py
--rw-r--r--   0        0        0     1236 2024-04-27 08:09:40.739203 vbproblemcomposer-0.1.1/vbproblemcomposer/choice_option.py
--rw-r--r--   0        0        0     1145 2024-04-27 08:46:59.990523 vbproblemcomposer-0.1.1/vbproblemcomposer/compose.py
--rw-r--r--   0        0        0     1615 2024-04-27 08:47:00.714808 vbproblemcomposer-0.1.1/vbproblemcomposer/functions.py
--rw-r--r--   0        0        0      230 2024-04-27 08:46:59.102498 vbproblemcomposer-0.1.1/vbproblemcomposer/main.py
--rw-r--r--   0        0        0      339 1970-01-01 00:00:00.000000 vbproblemcomposer-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-27 07:36:49.362347 vbproblemcomposer-0.1.2/README.md
+-rw-r--r--   0        0        0      375 2024-04-27 08:54:26.842664 vbproblemcomposer-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-27 07:36:49.362297 vbproblemcomposer-0.1.2/vbproblemcomposer/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-27 07:39:39.852664 vbproblemcomposer-0.1.2/vbproblemcomposer/__main__.py
+-rw-r--r--   0        0        0     1236 2024-04-27 08:09:40.739203 vbproblemcomposer-0.1.2/vbproblemcomposer/choice_option.py
+-rw-r--r--   0        0        0     1145 2024-04-27 08:46:59.990523 vbproblemcomposer-0.1.2/vbproblemcomposer/compose.py
+-rw-r--r--   0        0        0     1616 2024-04-27 08:54:21.527982 vbproblemcomposer-0.1.2/vbproblemcomposer/functions.py
+-rw-r--r--   0        0        0      230 2024-04-27 08:46:59.102498 vbproblemcomposer-0.1.2/vbproblemcomposer/main.py
+-rw-r--r--   0        0        0      339 1970-01-01 00:00:00.000000 vbproblemcomposer-0.1.2/PKG-INFO
```

### Comparing `vbproblemcomposer-0.1.1/vbproblemcomposer/choice_option.py` & `vbproblemcomposer-0.1.2/vbproblemcomposer/choice_option.py`

 * *Files identical despite different names*

### Comparing `vbproblemcomposer-0.1.1/vbproblemcomposer/compose.py` & `vbproblemcomposer-0.1.2/vbproblemcomposer/compose.py`

 * *Files identical despite different names*

### Comparing `vbproblemcomposer-0.1.1/vbproblemcomposer/functions.py` & `vbproblemcomposer-0.1.2/vbproblemcomposer/functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     except ValueError:
         return None
 
 
 def make_folder_with_basename(filename):
     base = os.path.basename(filename)
     name, ext = os.path.splitext(base)
-    folder_name = os.path.dirname(filename) + r"/" + r"problems" + r"/" + name
+    folder_name = os.path.dirname(filename) + r"./" + r"problems" + r"/" + name
     print(folder_name)
     os.makedirs(folder_name, exist_ok=True)
     return folder_name
 
 
 def make_file_in_folder(folder_name, exam, year, paper, n):
     file_name = folder_name + "/main.tex"
```

