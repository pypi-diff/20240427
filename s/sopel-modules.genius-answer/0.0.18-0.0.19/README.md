# Comparing `tmp/sopel_modules_genius_answer-0.0.18.tar.gz` & `tmp/sopel_modules_genius_answer-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopel_modules_genius_answer-0.0.18.tar", last modified: Fri Apr 26 17:57:35 2024, max compression
+gzip compressed data, was "sopel_modules_genius_answer-0.0.19.tar", last modified: Sat Apr 27 14:31:12 2024, max compression
```

## Comparing `sopel_modules_genius_answer-0.0.18.tar` & `sopel_modules_genius_answer-0.0.19.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-26 17:57:35.631374 sopel_modules_genius_answer-0.0.18/
--rw-rw-r--   0 user      (1000) user      (1000)      702 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.18/.gitignore
--rw-rw-r--   0 user      (1000) user      (1000)      135 2024-04-26 17:11:45.000000 sopel_modules_genius_answer-0.0.18/NOTE.md
--rw-r--r--   0 user      (1000) user      (1000)     1144 2024-04-26 17:57:35.631374 sopel_modules_genius_answer-0.0.18/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      736 2024-04-26 16:54:45.000000 sopel_modules_genius_answer-0.0.18/README.md
--rw-rw-r--   0 user      (1000) user      (1000)      674 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.18/TODO
--rw-rw-r--   0 user      (1000) user      (1000)      642 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.18/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-26 17:57:35.631374 sopel_modules_genius_answer-0.0.18/setup.cfg
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-26 17:57:35.629375 sopel_modules_genius_answer-0.0.18/sopel_modules/
--rw-rw-r--   0 user      (1000) user      (1000)       56 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.18/sopel_modules/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-26 17:57:35.630375 sopel_modules_genius_answer-0.0.18/sopel_modules/genius-answer/
--rw-rw-r--   0 user      (1000) user      (1000)     2933 2024-04-26 17:55:10.000000 sopel_modules_genius_answer-0.0.18/sopel_modules/genius-answer/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-26 17:57:35.630375 sopel_modules_genius_answer-0.0.18/sopel_modules.genius_answer.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1144 2024-04-26 17:57:35.000000 sopel_modules_genius_answer-0.0.18/sopel_modules.genius_answer.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      368 2024-04-26 17:57:35.000000 sopel_modules_genius_answer-0.0.18/sopel_modules.genius_answer.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-26 17:57:35.000000 sopel_modules_genius_answer-0.0.18/sopel_modules.genius_answer.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       37 2024-04-26 17:57:35.000000 sopel_modules_genius_answer-0.0.18/sopel_modules.genius_answer.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       14 2024-04-26 17:57:35.000000 sopel_modules_genius_answer-0.0.18/sopel_modules.genius_answer.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-27 14:31:12.892825 sopel_modules_genius_answer-0.0.19/
+-rw-rw-r--   0 user      (1000) user      (1000)      702 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.19/.gitignore
+-rw-rw-r--   0 user      (1000) user      (1000)      135 2024-04-26 17:11:45.000000 sopel_modules_genius_answer-0.0.19/NOTE.md
+-rw-r--r--   0 user      (1000) user      (1000)     1144 2024-04-27 14:31:12.892825 sopel_modules_genius_answer-0.0.19/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      736 2024-04-26 16:54:45.000000 sopel_modules_genius_answer-0.0.19/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)      674 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.19/TODO
+-rw-rw-r--   0 user      (1000) user      (1000)      642 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.19/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-27 14:31:12.892825 sopel_modules_genius_answer-0.0.19/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-27 14:31:12.891826 sopel_modules_genius_answer-0.0.19/sopel_modules/
+-rw-rw-r--   0 user      (1000) user      (1000)       56 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.19/sopel_modules/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-27 14:31:12.892825 sopel_modules_genius_answer-0.0.19/sopel_modules/genius-answer/
+-rw-rw-r--   0 user      (1000) user      (1000)     5136 2024-04-27 14:30:20.000000 sopel_modules_genius_answer-0.0.19/sopel_modules/genius-answer/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-27 14:31:12.892825 sopel_modules_genius_answer-0.0.19/sopel_modules.genius_answer.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     1144 2024-04-27 14:31:12.000000 sopel_modules_genius_answer-0.0.19/sopel_modules.genius_answer.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      368 2024-04-27 14:31:12.000000 sopel_modules_genius_answer-0.0.19/sopel_modules.genius_answer.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-27 14:31:12.000000 sopel_modules_genius_answer-0.0.19/sopel_modules.genius_answer.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       37 2024-04-27 14:31:12.000000 sopel_modules_genius_answer-0.0.19/sopel_modules.genius_answer.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       14 2024-04-27 14:31:12.000000 sopel_modules_genius_answer-0.0.19/sopel_modules.genius_answer.egg-info/top_level.txt
```

### Comparing `sopel_modules_genius_answer-0.0.18/.gitignore` & `sopel_modules_genius_answer-0.0.19/.gitignore`

 * *Files identical despite different names*

### Comparing `sopel_modules_genius_answer-0.0.18/PKG-INFO` & `sopel_modules_genius_answer-0.0.19/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel_modules.genius-answer
-Version: 0.0.18
+Version: 0.0.19
 Summary: A sopel plugin (irc-bot) to answer with a quote from rapgenius.com 
 Author-email: eoli3n <eoli3n@runbox.com>
 License: WTFPL
 Project-URL: Source code, https://github.com/eoli3n/sopel-genius-answer
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: sopel<8,>=7.1
```

### Comparing `sopel_modules_genius_answer-0.0.18/README.md` & `sopel_modules_genius_answer-0.0.19/README.md`

 * *Files identical despite different names*

### Comparing `sopel_modules_genius_answer-0.0.18/TODO` & `sopel_modules_genius_answer-0.0.19/TODO`

 * *Files identical despite different names*

### Comparing `sopel_modules_genius_answer-0.0.18/pyproject.toml` & `sopel_modules_genius_answer-0.0.19/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sopel_modules_genius_answer-0.0.18/sopel_modules.genius_answer.egg-info/PKG-INFO` & `sopel_modules_genius_answer-0.0.19/sopel_modules.genius_answer.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel_modules.genius-answer
-Version: 0.0.18
+Version: 0.0.19
 Summary: A sopel plugin (irc-bot) to answer with a quote from rapgenius.com 
 Author-email: eoli3n <eoli3n@runbox.com>
 License: WTFPL
 Project-URL: Source code, https://github.com/eoli3n/sopel-genius-answer
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: sopel<8,>=7.1
```

