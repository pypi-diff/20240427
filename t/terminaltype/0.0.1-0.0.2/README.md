# Comparing `tmp/terminaltype-0.0.1.tar.gz` & `tmp/terminaltype-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminaltype-0.0.1.tar", last modified: Mon Mar  4 18:16:31 2024, max compression
+gzip compressed data, was "terminaltype-0.0.2.tar", last modified: Sat Apr 27 18:36:06 2024, max compression
```

## Comparing `terminaltype-0.0.1.tar` & `terminaltype-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 ramiro    (1000) ramiro    (1000)        0 2024-03-04 18:16:31.411613 terminaltype-0.0.1/
--rw-r--r--   0 ramiro    (1000) ramiro    (1000)    35149 2024-02-26 16:44:18.000000 terminaltype-0.0.1/LICENSE
--rw-r--r--   0 ramiro    (1000) ramiro    (1000)     1330 2024-03-04 18:16:31.411613 terminaltype-0.0.1/PKG-INFO
--rw-r--r--   0 ramiro    (1000) ramiro    (1000)      633 2024-03-04 18:16:02.000000 terminaltype-0.0.1/README.md
--rw-r--r--   0 ramiro    (1000) ramiro    (1000)       87 2024-03-04 15:51:57.000000 terminaltype-0.0.1/pyproject.toml
--rw-r--r--   0 ramiro    (1000) ramiro    (1000)       38 2024-03-04 18:16:31.411613 terminaltype-0.0.1/setup.cfg
--rw-r--r--   0 ramiro    (1000) ramiro    (1000)     1237 2024-03-04 18:14:45.000000 terminaltype-0.0.1/setup.py
-drwxr-xr-x   0 ramiro    (1000) ramiro    (1000)        0 2024-03-04 18:16:31.411613 terminaltype-0.0.1/terminaltype/
--rw-r--r--   0 ramiro    (1000) ramiro    (1000)        0 2024-03-04 00:26:51.000000 terminaltype-0.0.1/terminaltype/__init__.py
--rw-r--r--   0 ramiro    (1000) ramiro    (1000)      105 2024-03-04 18:13:52.000000 terminaltype-0.0.1/terminaltype/__main__.py
--rw-r--r--   0 ramiro    (1000) ramiro    (1000)    13163 2024-03-04 18:13:17.000000 terminaltype-0.0.1/terminaltype/app.py
--rw-r--r--   0 ramiro    (1000) ramiro    (1000)     1440 2024-03-04 18:13:23.000000 terminaltype-0.0.1/terminaltype/arguments.py
--rw-r--r--   0 ramiro    (1000) ramiro    (1000)      161 2024-02-26 16:44:18.000000 terminaltype-0.0.1/terminaltype/colors.py
--rw-r--r--   0 ramiro    (1000) ramiro    (1000)     1864 2024-03-03 20:35:33.000000 terminaltype-0.0.1/terminaltype/history.py
--rw-r--r--   0 ramiro    (1000) ramiro    (1000)      861 2024-03-03 20:35:33.000000 terminaltype-0.0.1/terminaltype/keys.py
--rw-r--r--   0 ramiro    (1000) ramiro    (1000)     2443 2024-03-04 02:01:03.000000 terminaltype-0.0.1/terminaltype/text.py
--rw-r--r--   0 ramiro    (1000) ramiro    (1000)      937 2024-03-03 20:35:33.000000 terminaltype-0.0.1/terminaltype/timer.py
--rw-r--r--   0 ramiro    (1000) ramiro    (1000)     1085 2024-03-04 18:13:35.000000 terminaltype-0.0.1/terminaltype/utils.py
--rw-r--r--   0 ramiro    (1000) ramiro    (1000)     2143 2024-03-04 18:13:42.000000 terminaltype-0.0.1/terminaltype/window.py
-drwxr-xr-x   0 ramiro    (1000) ramiro    (1000)        0 2024-03-04 18:16:31.411613 terminaltype-0.0.1/terminaltype.egg-info/
--rw-r--r--   0 ramiro    (1000) ramiro    (1000)     1330 2024-03-04 18:16:31.000000 terminaltype-0.0.1/terminaltype.egg-info/PKG-INFO
--rw-r--r--   0 ramiro    (1000) ramiro    (1000)      511 2024-03-04 18:16:31.000000 terminaltype-0.0.1/terminaltype.egg-info/SOURCES.txt
--rw-r--r--   0 ramiro    (1000) ramiro    (1000)        1 2024-03-04 18:16:31.000000 terminaltype-0.0.1/terminaltype.egg-info/dependency_links.txt
--rw-r--r--   0 ramiro    (1000) ramiro    (1000)       54 2024-03-04 18:16:31.000000 terminaltype-0.0.1/terminaltype.egg-info/entry_points.txt
--rw-r--r--   0 ramiro    (1000) ramiro    (1000)       20 2024-03-04 18:16:31.000000 terminaltype-0.0.1/terminaltype.egg-info/requires.txt
--rw-r--r--   0 ramiro    (1000) ramiro    (1000)       13 2024-03-04 18:16:31.000000 terminaltype-0.0.1/terminaltype.egg-info/top_level.txt
+drwxr-xr-x   0 ramiro    (1000) ramiro    (1000)        0 2024-04-27 18:36:05.998515 terminaltype-0.0.2/
+-rw-r--r--   0 ramiro    (1000) ramiro    (1000)    35149 2024-02-26 16:44:18.000000 terminaltype-0.0.2/LICENSE
+-rw-r--r--   0 ramiro    (1000) ramiro    (1000)     1330 2024-04-27 18:36:05.998515 terminaltype-0.0.2/PKG-INFO
+-rw-r--r--   0 ramiro    (1000) ramiro    (1000)      633 2024-04-27 18:07:59.000000 terminaltype-0.0.2/README.md
+-rw-r--r--   0 ramiro    (1000) ramiro    (1000)       87 2024-03-04 15:51:57.000000 terminaltype-0.0.2/pyproject.toml
+-rw-r--r--   0 ramiro    (1000) ramiro    (1000)       38 2024-04-27 18:36:05.998515 terminaltype-0.0.2/setup.cfg
+-rw-r--r--   0 ramiro    (1000) ramiro    (1000)     1244 2024-04-27 18:35:45.000000 terminaltype-0.0.2/setup.py
+drwxr-xr-x   0 ramiro    (1000) ramiro    (1000)        0 2024-04-27 18:36:05.995182 terminaltype-0.0.2/terminaltype/
+-rw-r--r--   0 ramiro    (1000) ramiro    (1000)        0 2024-03-04 00:26:51.000000 terminaltype-0.0.2/terminaltype/__init__.py
+-rw-r--r--   0 ramiro    (1000) ramiro    (1000)      105 2024-03-04 18:13:52.000000 terminaltype-0.0.2/terminaltype/__main__.py
+-rw-r--r--   0 ramiro    (1000) ramiro    (1000)    13163 2024-03-04 18:13:17.000000 terminaltype-0.0.2/terminaltype/app.py
+-rw-r--r--   0 ramiro    (1000) ramiro    (1000)     1440 2024-03-13 00:31:58.000000 terminaltype-0.0.2/terminaltype/arguments.py
+-rw-r--r--   0 ramiro    (1000) ramiro    (1000)      161 2024-02-26 16:44:18.000000 terminaltype-0.0.2/terminaltype/colors.py
+-rw-r--r--   0 ramiro    (1000) ramiro    (1000)     1864 2024-03-03 20:35:33.000000 terminaltype-0.0.2/terminaltype/history.py
+-rw-r--r--   0 ramiro    (1000) ramiro    (1000)      861 2024-03-03 20:35:33.000000 terminaltype-0.0.2/terminaltype/keys.py
+-rw-r--r--   0 ramiro    (1000) ramiro    (1000)     2443 2024-04-27 18:03:10.000000 terminaltype-0.0.2/terminaltype/text.py
+-rw-r--r--   0 ramiro    (1000) ramiro    (1000)      937 2024-03-03 20:35:33.000000 terminaltype-0.0.2/terminaltype/timer.py
+-rw-r--r--   0 ramiro    (1000) ramiro    (1000)     1085 2024-03-04 18:13:35.000000 terminaltype-0.0.2/terminaltype/utils.py
+-rw-r--r--   0 ramiro    (1000) ramiro    (1000)     2143 2024-03-04 18:13:42.000000 terminaltype-0.0.2/terminaltype/window.py
+drwxr-xr-x   0 ramiro    (1000) ramiro    (1000)        0 2024-04-27 18:36:05.998515 terminaltype-0.0.2/terminaltype.egg-info/
+-rw-r--r--   0 ramiro    (1000) ramiro    (1000)     1330 2024-04-27 18:36:05.000000 terminaltype-0.0.2/terminaltype.egg-info/PKG-INFO
+-rw-r--r--   0 ramiro    (1000) ramiro    (1000)      511 2024-04-27 18:36:05.000000 terminaltype-0.0.2/terminaltype.egg-info/SOURCES.txt
+-rw-r--r--   0 ramiro    (1000) ramiro    (1000)        1 2024-04-27 18:36:05.000000 terminaltype-0.0.2/terminaltype.egg-info/dependency_links.txt
+-rw-r--r--   0 ramiro    (1000) ramiro    (1000)       61 2024-04-27 18:36:05.000000 terminaltype-0.0.2/terminaltype.egg-info/entry_points.txt
+-rw-r--r--   0 ramiro    (1000) ramiro    (1000)       20 2024-04-27 18:36:05.000000 terminaltype-0.0.2/terminaltype.egg-info/requires.txt
+-rw-r--r--   0 ramiro    (1000) ramiro    (1000)       13 2024-04-27 18:36:05.000000 terminaltype-0.0.2/terminaltype.egg-info/top_level.txt
```

### Comparing `terminaltype-0.0.1/LICENSE` & `terminaltype-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `terminaltype-0.0.1/PKG-INFO` & `terminaltype-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminaltype
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple terminal-based typing test
 Home-page: https://github.com/ramirocabral/terminaltype
 Author: Ramiro Cabral
 Author-email: <ramiro.cabral@alu.ing.unlp.edu.ar>
 License: GPL
 Keywords: python,typing,test,game,curses
 Classifier: Development Status :: 1 - Planning
```

### Comparing `terminaltype-0.0.1/README.md` & `terminaltype-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `terminaltype-0.0.1/setup.py` & `terminaltype-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open ("README.md", "r") as file:
     LONG_DESCRIPTION= file.read()
 
 install_require = []
 if os.name == 'nt':
     install_require.append('windows-curses')
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'A simple terminal-based typing test'
 
 setup(
     name="terminaltype",
     version=VERSION,
     author="Ramiro Cabral",
     author_email="<ramiro.cabral@alu.ing.unlp.edu.ar>",
@@ -33,12 +33,12 @@
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     ],
     entry_points={
         "console_scripts": [
-            "terminaltype=terminaltype.app:App",
+            "terminaltype=terminaltype.app:TypingTest",
         ],
     },
 
 )
```

### Comparing `terminaltype-0.0.1/terminaltype/app.py` & `terminaltype-0.0.2/terminaltype/app.py`

 * *Files identical despite different names*

### Comparing `terminaltype-0.0.1/terminaltype/arguments.py` & `terminaltype-0.0.2/terminaltype/arguments.py`

 * *Files identical despite different names*

### Comparing `terminaltype-0.0.1/terminaltype/history.py` & `terminaltype-0.0.2/terminaltype/history.py`

 * *Files identical despite different names*

### Comparing `terminaltype-0.0.1/terminaltype/keys.py` & `terminaltype-0.0.2/terminaltype/keys.py`

 * *Files identical despite different names*

### Comparing `terminaltype-0.0.1/terminaltype/text.py` & `terminaltype-0.0.2/terminaltype/text.py`

 * *Files identical despite different names*

### Comparing `terminaltype-0.0.1/terminaltype/timer.py` & `terminaltype-0.0.2/terminaltype/timer.py`

 * *Files identical despite different names*

### Comparing `terminaltype-0.0.1/terminaltype/utils.py` & `terminaltype-0.0.2/terminaltype/utils.py`

 * *Files identical despite different names*

### Comparing `terminaltype-0.0.1/terminaltype/window.py` & `terminaltype-0.0.2/terminaltype/window.py`

 * *Files identical despite different names*

### Comparing `terminaltype-0.0.1/terminaltype.egg-info/PKG-INFO` & `terminaltype-0.0.2/terminaltype.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminaltype
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple terminal-based typing test
 Home-page: https://github.com/ramirocabral/terminaltype
 Author: Ramiro Cabral
 Author-email: <ramiro.cabral@alu.ing.unlp.edu.ar>
 License: GPL
 Keywords: python,typing,test,game,curses
 Classifier: Development Status :: 1 - Planning
```

