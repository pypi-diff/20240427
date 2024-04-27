# Comparing `tmp/kandinsky-2.7.1.tar.gz` & `tmp/kandinsky-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kandinsky-2.7.1.tar", last modified: Fri Dec 22 09:52:06 2023, max compression
+gzip compressed data, was "kandinsky-2.7.2.tar", last modified: Sat Apr 27 11:20:19 2024, max compression
```

## Comparing `kandinsky-2.7.1.tar` & `kandinsky-2.7.2.tar`

### file list

```diff
@@ -1,40 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-12-22 09:52:06.342755 kandinsky-2.7.1/
--rw-rw-rw-   0        0        0     7559 2023-12-22 09:52:06.337788 kandinsky-2.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     6705 2023-12-22 09:52:05.000000 kandinsky-2.7.1/README.md
--rw-rw-rw-   0        0        0       42 2023-12-22 09:52:06.342755 kandinsky-2.7.1/setup.cfg
--rw-rw-rw-   0        0        0     3143 2023-12-22 09:50:57.000000 kandinsky-2.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-22 09:52:05.856382 kandinsky-2.7.1/src/
-drwxrwxrwx   0        0        0        0 2023-12-22 09:52:05.952481 kandinsky-2.7.1/src/kandinsky/
--rw-rw-rw-   0        0        0     3047 2023-09-14 20:12:46.000000 kandinsky-2.7.1/src/kandinsky/FAQ.md
--rw-rw-rw-   0        0        0     6705 2023-09-14 20:17:23.000000 kandinsky-2.7.1/src/kandinsky/README.md
--rw-rw-rw-   0        0        0     5124 2023-12-22 09:52:05.000000 kandinsky-2.7.1/src/kandinsky/__init__.py
--rw-rw-rw-   0        0        0     1368 2023-10-12 18:56:10.000000 kandinsky-2.7.1/src/kandinsky/__init__.pyi
--rw-rw-rw-   0        0        0      243 2023-08-04 11:47:50.000000 kandinsky-2.7.1/src/kandinsky/__main__.py
-drwxrwxrwx   0        0        0        0 2023-12-22 09:52:06.097661 kandinsky-2.7.1/src/kandinsky/util/
--rw-rw-rw-   0        0        0     4710 2023-09-19 22:15:03.000000 kandinsky-2.7.1/src/kandinsky/util/3d_demo.py
--rw-rw-rw-   0        0        0    13344 2023-12-22 09:48:30.000000 kandinsky-2.7.1/src/kandinsky/util/core.py
-drwxrwxrwx   0        0        0        0 2023-12-22 09:52:06.210323 kandinsky-2.7.1/src/kandinsky/util/data/
--rw-rw-rw-   0        0        0     4286 2022-11-03 16:32:20.000000 kandinsky-2.7.1/src/kandinsky/util/data/app.ico
--rw-rw-rw-   0        0        0     1544 2023-03-08 20:36:09.000000 kandinsky-2.7.1/src/kandinsky/util/data/app.png
--rw-rw-rw-   0        0        0      146 2023-03-28 16:47:34.000000 kandinsky-2.7.1/src/kandinsky/util/data/battery0.png
--rw-rw-rw-   0        0        0      159 2023-04-04 18:53:23.000000 kandinsky-2.7.1/src/kandinsky/util/data/battery1.png
--rw-rw-rw-   0        0        0   226352 2022-08-25 19:34:57.000000 kandinsky-2.7.1/src/kandinsky/util/data/large_font.ttf
--rw-rw-rw-   0        0        0     5805 2023-03-27 21:29:01.000000 kandinsky-2.7.1/src/kandinsky/util/data/old_icons.zip
--rw-rw-rw-   0        0        0   220448 2023-03-27 20:37:08.000000 kandinsky-2.7.1/src/kandinsky/util/data/small_font.ttf
--rw-rw-rw-   0        0        0     7223 2023-10-17 19:08:27.000000 kandinsky-2.7.1/src/kandinsky/util/demo.py
--rw-rw-rw-   0        0        0     3201 2023-08-01 18:20:49.000000 kandinsky-2.7.1/src/kandinsky/util/mac_patcher.py
--rw-rw-rw-   0        0        0     3470 2022-08-20 21:28:54.000000 kandinsky-2.7.1/src/kandinsky/util/old_config.ini
-drwxrwxrwx   0        0        0        0 2023-12-22 09:52:06.322290 kandinsky-2.7.1/src/kandinsky/util/stuff/
--rw-rw-rw-   0        0        0      128 2023-05-03 14:32:56.000000 kandinsky-2.7.1/src/kandinsky/util/stuff/__init__.py
--rw-rw-rw-   0        0        0     2597 2023-12-22 09:42:41.000000 kandinsky-2.7.1/src/kandinsky/util/stuff/color.py
--rw-rw-rw-   0        0        0     1545 2023-12-22 09:48:08.000000 kandinsky-2.7.1/src/kandinsky/util/stuff/draw.py
--rw-rw-rw-   0        0        0    16116 2023-12-22 09:44:14.000000 kandinsky-2.7.1/src/kandinsky/util/stuff/gui.py
--rw-rw-rw-   0        0        0     6006 2023-08-02 19:57:06.000000 kandinsky-2.7.1/src/kandinsky/util/stuff/limiter.py
--rw-rw-rw-   0        0        0     1377 2023-07-16 14:36:13.000000 kandinsky-2.7.1/src/kandinsky/util/stuff/tests.py
--rw-rw-rw-   0        0        0     3003 2023-09-24 21:22:08.000000 kandinsky-2.7.1/src/kandinsky/util/stuff/vars.py
-drwxrwxrwx   0        0        0        0 2023-12-22 09:52:06.334415 kandinsky-2.7.1/src/kandinsky.egg-info/
--rw-rw-rw-   0        0        0     7559 2023-12-22 09:52:05.000000 kandinsky-2.7.1/src/kandinsky.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      971 2023-12-22 09:52:05.000000 kandinsky-2.7.1/src/kandinsky.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-22 09:52:05.000000 kandinsky-2.7.1/src/kandinsky.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-12-22 09:52:05.000000 kandinsky-2.7.1/src/kandinsky.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-12-22 09:52:05.000000 kandinsky-2.7.1/src/kandinsky.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 11:20:19.381934 kandinsky-2.7.2/
+-rw-rw-rw-   0        0        0     7894 2024-04-27 11:20:19.373923 kandinsky-2.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7038 2024-04-27 11:20:18.000000 kandinsky-2.7.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 11:20:19.384436 kandinsky-2.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     3003 2024-04-26 13:42:27.000000 kandinsky-2.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:20:18.929287 kandinsky-2.7.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-27 11:20:19.001323 kandinsky-2.7.2/src/kandinsky/
+-rw-rw-rw-   0        0        0     3047 2023-09-14 20:12:46.000000 kandinsky-2.7.2/src/kandinsky/FAQ.md
+-rw-rw-rw-   0        0        0     7038 2024-04-26 14:07:54.000000 kandinsky-2.7.2/src/kandinsky/README.md
+-rw-rw-rw-   0        0        0     5128 2024-04-27 11:20:18.000000 kandinsky-2.7.2/src/kandinsky/__init__.py
+-rw-rw-rw-   0        0        0     1368 2023-10-12 18:56:10.000000 kandinsky-2.7.2/src/kandinsky/__init__.pyi
+-rw-rw-rw-   0        0        0      244 2024-04-24 17:30:23.000000 kandinsky-2.7.2/src/kandinsky/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:20:19.134853 kandinsky-2.7.2/src/kandinsky/util/
+-rw-rw-rw-   0        0        0     4710 2023-09-19 22:15:03.000000 kandinsky-2.7.2/src/kandinsky/util/3d_demo.py
+-rw-rw-rw-   0        0        0    13631 2024-04-26 14:00:57.000000 kandinsky-2.7.2/src/kandinsky/util/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:20:19.225887 kandinsky-2.7.2/src/kandinsky/util/data/
+-rw-rw-rw-   0        0        0     4286 2022-11-03 16:32:20.000000 kandinsky-2.7.2/src/kandinsky/util/data/app.ico
+-rw-rw-rw-   0        0        0     1544 2023-03-08 20:36:09.000000 kandinsky-2.7.2/src/kandinsky/util/data/app.png
+-rw-rw-rw-   0        0        0      146 2023-03-28 16:47:34.000000 kandinsky-2.7.2/src/kandinsky/util/data/battery0.png
+-rw-rw-rw-   0        0        0      159 2023-04-04 18:53:23.000000 kandinsky-2.7.2/src/kandinsky/util/data/battery1.png
+-rw-rw-rw-   0        0        0   226352 2022-08-25 19:34:57.000000 kandinsky-2.7.2/src/kandinsky/util/data/large_font.ttf
+-rw-rw-rw-   0        0        0   220448 2023-03-27 20:37:08.000000 kandinsky-2.7.2/src/kandinsky/util/data/small_font.ttf
+-rw-rw-rw-   0        0        0     7851 2024-04-26 16:34:18.000000 kandinsky-2.7.2/src/kandinsky/util/demo.py
+-rw-rw-rw-   0        0        0     3202 2024-04-24 17:26:47.000000 kandinsky-2.7.2/src/kandinsky/util/mac_patcher.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:20:19.355922 kandinsky-2.7.2/src/kandinsky/util/stuff/
+-rw-rw-rw-   0        0        0      128 2023-05-03 14:32:56.000000 kandinsky-2.7.2/src/kandinsky/util/stuff/__init__.py
+-rw-rw-rw-   0        0        0     2597 2023-12-22 09:42:41.000000 kandinsky-2.7.2/src/kandinsky/util/stuff/color.py
+-rw-rw-rw-   0        0        0     1545 2023-12-22 09:48:08.000000 kandinsky-2.7.2/src/kandinsky/util/stuff/draw.py
+-rw-rw-rw-   0        0        0    16830 2024-04-26 18:09:39.000000 kandinsky-2.7.2/src/kandinsky/util/stuff/gui.py
+-rw-rw-rw-   0        0        0     5192 2024-04-24 19:11:50.000000 kandinsky-2.7.2/src/kandinsky/util/stuff/limiter.py
+-rw-rw-rw-   0        0        0     1377 2023-07-16 14:36:13.000000 kandinsky-2.7.2/src/kandinsky/util/stuff/tests.py
+-rw-rw-rw-   0        0        0     3005 2024-04-24 16:46:43.000000 kandinsky-2.7.2/src/kandinsky/util/stuff/vars.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:20:19.363424 kandinsky-2.7.2/src/kandinsky.egg-info/
+-rw-rw-rw-   0        0        0     7894 2024-04-27 11:20:18.000000 kandinsky-2.7.2/src/kandinsky.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      899 2024-04-27 11:20:18.000000 kandinsky-2.7.2/src/kandinsky.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 11:20:18.000000 kandinsky-2.7.2/src/kandinsky.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2024-04-27 11:20:18.000000 kandinsky-2.7.2/src/kandinsky.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-27 11:20:18.000000 kandinsky-2.7.2/src/kandinsky.egg-info/top_level.txt
```

### Comparing `kandinsky-2.7.1/PKG-INFO` & `kandinsky-2.7.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kandinsky
-Version: 2.7.1
+Version: 2.7.2
 Summary: A small module allowing to link the kandinsky module, from the Numworks, to a window.
 Home-page: https://github.com/ZetaMap/Kandinsky-Numworks
 Author: ZetaMap
 License: MIT
 Project-URL: GitHub Project, https://github.com/ZetaMap/Kandinsky-Numworks
 Project-URL: My GitHub Page, https://github.com/ZetaMap/
 Classifier: Programming Language :: Python :: 3
@@ -25,15 +25,15 @@
 
 This module allowing to link the kandinsky module, from the Numworks, to a window. Useful if you want to test your program without putting it on the calculator. <br>
 In addition, this module also emulates the drawing speed, and has [many other features](https://github.com/ZetaMap/Kandinsky-Numworks/blob/pysdl2/README.md#additional-features).
 
 
 ### Installation
 You now have the option to install this module on [pypi.org](https://pypi.org/project/kandinsky/). For that, follow the steps [here](https://github.com/ZetaMap/Kandinsky-Numworks/blob/pysdl2/FAQ.md#how-to-install-this-module). <br>
-Or if you want, you can build it yourself, just run the command ``./setup``. <br>
+Or if you want, you can build it yourself, just clone the repo and run the command ``./setup``. <br>
 
 ### More
 I also recreated the ion module of the Numworks, check it out here: [Ion module of Numworks](https://github.com/ZetaMap/Ion-numworks)<br>
 If you have a question, check out the [FAQ](https://github.com/ZetaMap/Kandinsky-Numworks/blob/pysdl2/FAQ.md). And if you have a suggestion or your question is not answered, open an [Issue](https://github.com/ZetaMap/Kandinsky-Numworks/issues/new).
 
 
 ### Usable content
@@ -171,7 +171,21 @@
 ```
 
 * Zoom the window:
 ```python
 # from 1 to 4
 os.environ['KANDINSKY_ZOOM_RATIO'] = "<number>"
 ```
+
+
+**Experiental features:**
+
+* Will try to limit the thread heap to get a better emulation:
+```python
+# Note: Cannot be enabled on some python versions
+os.environ['KANDINSKY_USE_HEAP'] = ''
+```
+
+* Add a button in GUI to allow window resising:
+```python
+os.environ['KANDINSKY_ENABLE_RESIZING'] = ''
+```
```

### Comparing `kandinsky-2.7.1/README.md` & `kandinsky-2.7.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 This module allowing to link the kandinsky module, from the Numworks, to a window. Useful if you want to test your program without putting it on the calculator. <br>
 In addition, this module also emulates the drawing speed, and has [many other features](https://github.com/ZetaMap/Kandinsky-Numworks/blob/pysdl2/README.md#additional-features).
 
 
 ### Installation
 You now have the option to install this module on [pypi.org](https://pypi.org/project/kandinsky/). For that, follow the steps [here](https://github.com/ZetaMap/Kandinsky-Numworks/blob/pysdl2/FAQ.md#how-to-install-this-module). <br>
-Or if you want, you can build it yourself, just run the command ``./setup``. <br>
+Or if you want, you can build it yourself, just clone the repo and run the command ``./setup``. <br>
 
 ### More
 I also recreated the ion module of the Numworks, check it out here: [Ion module of Numworks](https://github.com/ZetaMap/Ion-numworks)<br>
 If you have a question, check out the [FAQ](https://github.com/ZetaMap/Kandinsky-Numworks/blob/pysdl2/FAQ.md). And if you have a suggestion or your question is not answered, open an [Issue](https://github.com/ZetaMap/Kandinsky-Numworks/issues/new).
 
 
 ### Usable content
@@ -150,7 +150,21 @@
 ```
 
 * Zoom the window:
 ```python
 # from 1 to 4
 os.environ['KANDINSKY_ZOOM_RATIO'] = "<number>"
 ```
+
+
+**Experiental features:**
+
+* Will try to limit the thread heap to get a better emulation:
+```python
+# Note: Cannot be enabled on some python versions
+os.environ['KANDINSKY_USE_HEAP'] = ''
+```
+
+* Add a button in GUI to allow window resising:
+```python
+os.environ['KANDINSKY_ENABLE_RESIZING'] = ''
+```
```

### Comparing `kandinsky-2.7.1/setup.py` & `kandinsky-2.7.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,35 @@
-import sys, os
+import sys, os, shutil
 from setuptools import setup
 
 # Used by setup script to restore the version to 'null' in __init__.py after builded the library
 RESTORE_VERSION = "--version-null" in sys.argv
 
 # Version of library
-VERSION = "2.7.1"
+VERSION = "2.7.2"
 
 # Get the absolute path
 PATH = __file__[:__file__.rfind('\\')+1 or __file__.rfind('/')+1]
 
 # Copy README and FAQ
-with open(PATH+"src/kandinsky/README.md", "rt", encoding="utf-8") as new:
-  DOC = new.read()
-  with open(PATH+"README.md", "wt", encoding="utf-8") as old:
-    old.write(DOC)
-
-with open(PATH+"src/kandinsky/FAQ.md", "rt", encoding="utf-8") as new:
-  with open(PATH+"FAQ.md", "wt", encoding="utf-8") as old:
-    old.write(new.read())
+shutil.copy(PATH+"src/kandinsky/README.md", PATH+"README.md")
+with open(PATH+"README.md", "rt", encoding="utf-8") as f: DOC = f.read()
+shutil.copy(PATH+"src/kandinsky/FAQ.md", PATH+"FAQ.md")
 
 # Set the version in __init__.py
-with open(PATH+"src/kandinsky/__init__.py", "r+t", encoding="utf-8") as f:
-  lines = f.readlines()
-  for i in range(len(lines)):
-    if "__version__" in lines[i]:
-      if RESTORE_VERSION:
-        if VERSION in lines[i]: lines[i] = lines[i].replace(VERSION, "null")
-        else: lines[i] = f"__version__ = \"null\"\n"
-      elif "null" in lines[i]: lines[i] = lines[i].replace("null", VERSION)  
-      else: lines[i] = f"__version__ = \"{VERSION}\"\n"
-
-      f.seek(0)
-      f.writelines(lines)      
-      break
+with open(PATH+"src/kandinsky/__init__.py", "rt", encoding="utf-8") as f: buffer = f.readlines()
+for i, l in enumerate(buffer):
+  if "__version__" in l:
+    if RESTORE_VERSION:
+      if VERSION in l: buffer[i] = l.replace(VERSION, "null")
+      else: buffer[i] = f"__version__ = \"null\"\n"
+    elif "null" in l: buffer[i] = l.replace("null", VERSION)  
+    else: buffer[i] = f"__version__ = \"{VERSION}\"\n"
+    break
+with open(PATH+"src/kandinsky/__init__.py", "wt", encoding="utf-8") as f: f.writelines(buffer)
 
 # Stop here if restore version to 'null'
 if RESTORE_VERSION: exit()
 
 # Remove __pycache__ everywhere
 def clean_pycache(path="."):
   """Clean __pycache__ directories recursively. Call this before setup()."""
```

### Comparing `kandinsky-2.7.1/src/kandinsky/FAQ.md` & `kandinsky-2.7.2/src/kandinsky/FAQ.md`

 * *Files identical despite different names*

### Comparing `kandinsky-2.7.1/src/kandinsky/README.md` & `kandinsky-2.7.2/src/kandinsky/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 This module allowing to link the kandinsky module, from the Numworks, to a window. Useful if you want to test your program without putting it on the calculator. <br>
 In addition, this module also emulates the drawing speed, and has [many other features](https://github.com/ZetaMap/Kandinsky-Numworks/blob/pysdl2/README.md#additional-features).
 
 
 ### Installation
 You now have the option to install this module on [pypi.org](https://pypi.org/project/kandinsky/). For that, follow the steps [here](https://github.com/ZetaMap/Kandinsky-Numworks/blob/pysdl2/FAQ.md#how-to-install-this-module). <br>
-Or if you want, you can build it yourself, just run the command ``./setup``. <br>
+Or if you want, you can build it yourself, just clone the repo and run the command ``./setup``. <br>
 
 ### More
 I also recreated the ion module of the Numworks, check it out here: [Ion module of Numworks](https://github.com/ZetaMap/Ion-numworks)<br>
 If you have a question, check out the [FAQ](https://github.com/ZetaMap/Kandinsky-Numworks/blob/pysdl2/FAQ.md). And if you have a suggestion or your question is not answered, open an [Issue](https://github.com/ZetaMap/Kandinsky-Numworks/issues/new).
 
 
 ### Usable content
@@ -150,7 +150,21 @@
 ```
 
 * Zoom the window:
 ```python
 # from 1 to 4
 os.environ['KANDINSKY_ZOOM_RATIO'] = "<number>"
 ```
+
+
+**Experiental features:**
+
+* Will try to limit the thread heap to get a better emulation:
+```python
+# Note: Cannot be enabled on some python versions
+os.environ['KANDINSKY_USE_HEAP'] = ''
+```
+
+* Add a button in GUI to allow window resising:
+```python
+os.environ['KANDINSKY_ENABLE_RESIZING'] = ''
+```
```

### Comparing `kandinsky-2.7.1/src/kandinsky/__init__.py` & `kandinsky-2.7.2/src/kandinsky/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 except ImportError as e:
   if "relative import" not in e.msg:
     raise
   if sys.platform == 'darwin': from util.mac_patcher import Core as __Core, display
   else: from util.core import Core as __Core
 
 __name__ = "kandinsky"
-__version__ = "2.7.1"
+__version__ = "2.7.2"
 try: 
   with open("README.md", encoding="utf-8") as f: __doc__ = f.read()
   del f
 except (FileNotFoundError, OSError): __doc__ = "<unknown>"
 __all__ = [
   #numworks
   "get_pixel",
@@ -90,15 +90,15 @@
   _, err = __Core.event_fire(__Core.fill_rect, x, y, width, height, color)
   if err != None:
     raise err
 
 # new method of kandinsky, only on PC
 def quit():
   """Close manualy the window without notifying the user"""
-  _, err = __Core.event_fire(__Core.quit_app)
+  _, err = __Core.event_fire(__Core.request_stop)
   if err != None:
     raise err
 
 # omega methods
 def draw_line(x1, y1, x2, y2, color, /):
   """Draw a line at (x1, y1) to (x2, y2)"""
   _, err = __Core.event_fire(__Core.draw_line, x1, y1, x2, y2, color)
```

### Comparing `kandinsky-2.7.1/src/kandinsky/__init__.pyi` & `kandinsky-2.7.2/src/kandinsky/__init__.pyi`

 * *Files identical despite different names*

### Comparing `kandinsky-2.7.1/src/kandinsky/util/3d_demo.py` & `kandinsky-2.7.2/src/kandinsky/util/3d_demo.py`

 * *Files identical despite different names*

### Comparing `kandinsky-2.7.1/src/kandinsky/util/core.py` & `kandinsky-2.7.2/src/kandinsky/util/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -75,15 +75,18 @@
 
 # Experimental way to get more real emulation of numworks
 import threading
 USE_HEAP = 'KANDINSKY_USE_HEAP' in os.environ and hasattr(threading, "get_native_id")
 # same problem than warning of ion
 if USE_HEAP: prettywarn("python heap limitator is an experimental feature, so it can crach python several times", ImportWarning)
 
-# We need to more the import of ion here, to not import it if os mode isn't Omega
+# Enable resizing feature. this feature is experimental for moment
+ENABLE_RESIZING = 'KANDINSKY_ENABLE_RESIZING' in os.environ
+
+# We need to move the import of ion here, to not import it if os mode isn't Omega
 if Vars.selected_os == 2:
   try: 
     with warnings.catch_warnings(record=True):
       import ion
   except ImportError: pass
   else:
     # Another module is called ion, so verify default function to see if it's the right module
@@ -106,26 +109,31 @@
 
 
 ######### Main code #########
 __all__ = ["Core"]
 
 class Core(Thread):
   stopped = False
+  stopping = False
   asknoclose = False
   OS_MODE = Config.default_os
 
   def __init__(self):
     Gui.paused = Gui.already_paused = True # Pause events to give the time of thread to initialize
 
     super().__init__(None, self.event_loop, Vars.app_name.replace(' ', '')+self.__class__.__name__)
     self.start()
     while Gui.paused and self.is_alive(): usleep(100) # Wait a little to synchronize it
 
+  def request_stop(self):
+    self.stopped = True
+
   def quit_app(self, *_):
-    if not self.stopped:
+    if not self.stopping:
+      self.stopping = True
       self.stopped = True
       Gui.paused = False # Now all calls of kandinsky raise an error
 
       usleep(10**4) # Wait a little to give time to draw methods finished
       Gui.destroy()
       sdl_quit()
 
@@ -298,14 +306,15 @@
             "HomeBackground": Colors.white,
             "PrimaryText":    Colors.black,
             "SecondaryText":  (104, 108, 104)}
 ###
 
   def event_loop(self):
     if USE_HEAP: Gui._main_thread_pid = self.native_id
+    if ENABLE_RESIZING: Gui.resizing_enabled = True
 
     try:
       Gui(Tk())
       Gui.config(not NO_GUI)
     except RuntimeError as e:
       # Handle multiple import of library
       # Library cannot open new tkinter root windows while another is opened but it can open another if previous is destroyed
@@ -322,21 +331,21 @@
     Gui.paused = Gui.already_paused = False # Initialization finished, unpause events
 
     while True:
       if self.stopped:
         self.quit_app()
         return
       elif not self.asknoclose and not main_thread().is_alive():
-        if Gui.askscriptend(): self.stopped = True
+        if Gui.askscriptend(): self.request_stop()
         else: self.asknoclose = True
 
       self.refreshed = False
       try: Gui.refresh()
       except AttributeError: pass
-      except RuntimeError: self.stopped = True
+      except RuntimeError: self.request_stop()
       usleep(1000)
       self.refreshed = True
 
   def event_fire(self, method, *arg, **kwargs):
     try:
       self.verify(method, *arg, **kwargs)
       return method(*arg, **kwargs), None
```

### Comparing `kandinsky-2.7.1/src/kandinsky/util/data/app.ico` & `kandinsky-2.7.2/src/kandinsky/util/data/app.ico`

 * *Files identical despite different names*

### Comparing `kandinsky-2.7.1/src/kandinsky/util/data/app.png` & `kandinsky-2.7.2/src/kandinsky/util/data/app.png`

 * *Files identical despite different names*

### Comparing `kandinsky-2.7.1/src/kandinsky/util/data/large_font.ttf` & `kandinsky-2.7.2/src/kandinsky/util/data/large_font.ttf`

 * *Files identical despite different names*

### Comparing `kandinsky-2.7.1/src/kandinsky/util/data/small_font.ttf` & `kandinsky-2.7.2/src/kandinsky/util/data/small_font.ttf`

 * *Files identical despite different names*

### Comparing `kandinsky-2.7.1/src/kandinsky/util/demo.py` & `kandinsky-2.7.2/src/kandinsky/util/demo.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,50 +3,55 @@
 """
 print("""This is a demo code
 Source: https://my.numworks.com/python/zetamap/snake_lite""")
 __all__ = []
 
 #############################################################
 
+import os
+os.environ['KANDINSKY_ENABLE_RESIZING'] = ''
+
 from random import randint as ri
 from kandinsky import fill_rect as fr,draw_string as ds
 from ion import keydown as kd
 from time import monotonic as mt,sleep as sl
 
 DEC=lambda v:((v&0xfff000)>>12,v&0xfff)
 ENC=lambda x,y:x<<12|y
 BOOL=lambda t:(t.lower()if type(t)==str else t) in("yes","on","enabled","activated","true","1",1)
 def wk(*b):
  while 1:
   for i in b:
    if kd(i):
     while kd(i):pass
     return i
+mjust=lambda l,r,s,f=' ': l+f*((s-len(l))//len(f))+r
 class Snake:
- c=["0.2","0.95","#00ff00","green","red","blue","#ffb531"]
+ c=["0.95","0.2","#00ff00","green","red","blue","#ffb531","1.0"]
  try:
   import os
-  u=os.getlogin()
+  u=os.getlogin()or "You"
   try:
    from kandinsky import get_palette as gp
    c[6]=gp()["Toolbar"]
+   c[7]=gp()["HomeBackground"]
   except:c[6]="#c53431"
  except:u="You"
  def __init__(s,leader_board=[],speed=10,power=2,size=10,score=1,inf_snake=False,gost=False,darkmode=True,rainbow=False,walls=True):
   if BOOL(inf_snake):power=float("inf")
-  if not BOOL(darkmode):s.c[0],s.c[1]=s.c[1],s.c[0]
-  s.lb,s.s,s.p,s.m,s.t,s.g,s.go,s.r,s.w=leader_board,1/speed,power,score,size,(320//size-1,220//size-1),BOOL(gost),BOOL(rainbow),BOOL(walls)
+  if BOOL(darkmode):s.c[0],s.c[1]=s.c[1],s.c[0]
+  s.lb,s.s,s.p,s.m,s.t,s.g,s.go,s.r,s.w=leader_board,1/speed,power,score,size,(320//size,220//size),BOOL(gost),BOOL(rainbow),BOOL(walls)
  def nc(s):
-  s.h=[ri(s.w,s.g[i]-s.w)for i in(0,1)]
-  while ENC(s.h[0],s.h[1])in s.b:s.h=[ri(s.w,s.g[i]-s.w)for i in(0,1)]
+  s.h=[ri(s.w,s.g[i]-s.w-1)for i in(0,1)]
+  while ENC(s.h[0],s.h[1])in s.b:s.h=[ri(s.w,s.g[i]-s.w-1)for i in(0,1)]
   fr(s.h[0]*s.t,2+s.h[1]*s.t,s.t,s.t,s.c[4])
  def dl(s):
-  fr(0,2,320,220,"black")
-  fr(0,2,(s.g[0]+1)*s.t,(s.g[1]+1)*s.t,s.c[5 if s.w else 0])
-  if s.w:fr(s.t//2,2+s.t//2,s.g[0]*s.t,s.g[1]*s.t,s.c[0])
+  fr(0,2,320,220,"0.0")
+  fr(0,2,s.g[0]*s.t,s.g[1]*s.t,s.c[5*s.w])
+  if s.w:fr(s.t//2,2+s.t//2,(s.g[0]-1)*s.t,(s.g[1]-1)*s.t,s.c[0])
  def dt(s,t,x,y):
   for i,l in enumerate(t.replace('\t',"    ")):
    ds(l,x+10*i,y,s.c[1],s.c[0])
    if l!=' ':sl(0.02)
  def ub(s,l1,l2):
   fr(20,82,280,50,s.c[4])
   fr(25,87,270,40,s.c[0])
@@ -60,31 +65,31 @@
  def wu(s):
   s.mt=mt()
   s.ta,s.e=(s.b[-1],DEC(s.b[-1])),DEC(s.b[0])
   if kd(0)and s.d[0]!=1:s.d=[-1,0]
   elif kd(1)and s.d[1]!=1:s.d=[0,-1]
   elif kd(2)and s.d[1]!=-1:s.d=[0,1]
   elif kd(3)and s.d[0]!=-1:s.d=[1,0]
-  fr(s.e[0]*s.t,2+s.e[1]*s.t,s.t,s.t,[ri(0,255) for _ in(0,1,2)]if s.r else s.c[3])
+  fr(s.e[0]*s.t,2+s.e[1]*s.t,s.t,s.t,s.r and[ri(0,255) for _ in(0,1,2)]or s.c[3])
   for x in range(len(s.b)-1,0,-1):s.b[x]=s.b[x-1]
-  s.b[0]=ENC((s.e[0]+s.d[0])%(s.g[0]+(not s.w)),(s.e[1]+s.d[1])%(s.g[1]+(not s.w)))
+  s.b[0]=ENC((s.e[0]+s.d[0])%s.g[0],(s.e[1]+s.d[1])%s.g[1])
   if s.a>0:
    s.b.append(s.ta[0])
    s.a-=1
   elif s.ta[0]not in s.b:fr(s.ta[1][0]*s.t,2+s.ta[1][1]*s.t,s.t,s.t,s.c[0])
   if s.b[0]==ENC(s.h[0],s.h[1]):
    s.a,s.sc=s.a+s.p,s.sc+s.m
    s.nc()
   s.e=DEC(s.b[0])
+  fr(s.e[0]*s.t,2+s.e[1]*s.t,s.t,s.t,s.c[2])
+  ds(str(s.sc),7,7,s.c[1],s.c[0])
   if not s.go:
-   if s.w and(s.e[0]==s.g[0]or s.e[1]==s.g[1]or s.e[0]==0 or s.e[1]==0):return 0
+   if s.w and(s.e[0]==s.g[0]-1 or s.e[1]==s.g[1]-1 or s.e[0]==0 or s.e[1]==0):return 0
    for x in range(1,len(s.b)):
     if s.b[x]==s.b[0]:return 0
-  fr(s.e[0]*s.t,2+s.e[1]*s.t,s.t,s.t,s.c[2])
-  ds(str(s.sc),7,7,s.c[1],s.c[0])
   return 1
  def start(s):
   fr(0,0,320,2,s.c[6])
   try:
    while 1:
     s.b,s.a,s.d,s.sc=[ENC(s.g[0]//2,s.g[1]//2)],4,(1,0),0
     s.dl()
@@ -93,133 +98,160 @@
      if kd(17):
       s.ub("\t\tGame Paused!","  (OK, DELETE = Continue)")
       sl(0.2)
       s.dl()
       fr(s.h[0]*s.t,2+s.h[1]*s.t,s.t,s.t,s.c[4])
       for i in s.b:
        s.e=DEC(i)
-       fr(s.e[0]*s.t,2+s.e[1]*s.t,s.t,s.t,[ri(0,255)for _ in(0,1,2)]if s.r else s.c[3])
+       fr(s.e[0]*s.t,2+s.e[1]*s.t,s.t,s.t,s.r and[ri(0,255) for _ in(0,1,2)]or s.c[3])
      while mt()-s.mt<s.s:sl(0.01)
     if not s.ub(' '*(3-len(str(s.sc))//2)+"You lose!\tScore: %d"%s.sc,"(OK = Retry, DELETE = Quit)"):break
-   s.e=0
-   s.lb=sorted(s.lb+((s.u,s.sc),),key=lambda v:v[1],reverse=1)
-   print("Your score:",s.sc,"\nLeader board: (default settings)")
+   e,p,s.lb,x,t=0,0,sorted(s.lb+((s.u,s.sc),),key=lambda v:v[1],reverse=1),"Your score:","Leader board:"
+   print(x,s.sc,"\n",t+" (default settings)")
    for i,sc in enumerate(s.lb):
-    if len(sc[0])>s.e:s.e=len(sc[0])
+    if len(sc[0])>e:e=len(sc[0])+len(str(sc[1]))
+    if sc[0]==s.u:p=i
     print(' %d-'%(i+1),sc[0]+':',sc[1])
    fr(0,2,320,220,s.c[0])
-   s.dt("Your score: %d"%s.sc,5,7)
-   s.dt("Leader board:",5,32)
-   for i,sc in enumerate(s.lb):s.dt(sc[0]+':'+' '*(s.e-len(sc[0])+2)+str(sc[1]),60,52+20*i)
-   l=['>'*i+' '*(4-i)+s.lb[0][0]+':'+' '*(s.e-len(s.lb[0][0])+2)+str(s.lb[0][1])+' '*(4-i)+'<'*i for i in range(4)]
-   while not kd(4) and not kd(17):
-    for i in l:
-     sl(0.2)
+   s.dt(x+" %d"%s.sc,5,7)
+   s.dt(t,5,32)
+   for i,sc in enumerate(s.lb):
+    s.lb[i]=mjust(sc[0]+':',str(sc[1]),e+3)
+    s.dt(s.lb[i],60,52+20*i)
+   while not kd(4)and not kd(17):
+    for i in range(4):
      if kd(4)or kd(17):break
-     ds(i,20,52,s.c[6],s.c[0])
+     ds('>'*i+' '*(4-i),20,52,s.c[6],s.c[0])
+     ds(' '*(4-i)+'<'*i,20+(e+1)*16,52,s.c[6],s.c[0])
+     ds(s.lb[p],60,52+20*p,s.c[bool(i%3)*5+1],s.c[0])
+     sl(0.2)
   except KeyboardInterrupt:pass
 class Menu:
- colors=[Snake.c[1],Snake.c[0],"0.38",Snake.c[6],"#2a78e0"]
- r,u=colors,0
- default=lambda s:[s.p[i][s.c[i]]for i in range(s.s)]
+ colors=[Snake.c[0],Snake.c[1],"0.38",Snake.c[6],"#2a78e0"]
+ r,u=colors,1
+ options=lambda s:[s.p[i][s.c[i]]for i in range(s.s)]
  def __init__(s,title,action,*options):
-  s.t,s.a,s.p=title,action,options
+  s.t,s.a,s.p=title[0:25],action[0:28],options
   s.s=len(s.p)
   s.c,s.b=[],len(s.a)
-  for i in s.p:
-   assert len(i)>2
+  for i in s.p :
+   assert len(i)>2,"need [label,default,values...]"
    s.c.append(int(i[1])+2)
  def mo(s,i,o,u):
   t,l=str(s.p[i][s.c[i]])[0:15],i%6
   ds('<'*u+' '*(17-2*u)+'>'*u,140,65+l*25,s.r[2],s.r[1])
   ds(t,150+(150-10*len(t))//2,65+l*25,o,s.r[1])
  def do(s):
-  u=(s.u-(s.u and s.u==s.u//6*6))//6*6
+  u=s.u-1*(s.u>0)
+  u=(u-(u and u==u//6*6))//6*6
   for i in range(6):
    if u+i<s.s:
     t=str(s.p[u+i][0])[0:12]
     ds(t+' '*(12-len(t)),10,65+i*25,s.r[0],s.r[1])
     s.mo(u+i,s.r[2],0)
    else:fr(10,65+i*25,300,18,s.r[1])
   if s.s>6:s.sb(u)
  def sb(s,u):
   fr(314,65,3,140,s.r[2])
   o=140//((s.s+5)//6)
   p=o*(u//6)
   fr(314,65+p,3,o+(u==s.s//6*6)*(140-o-p),s.r[3])
+ def da(s,i):
+  c=s.r[3*(i==0)]
+  ds("<",10,8,c,s.r[1])
+  fr(13,16,13,1,c)
+  fr(26,10,1,6,c)
+  ds(s.a,160-5*s.b,36,s.r[3*(i==1)],s.r[1])
  def ds(s):
   fr(0,0,320,222,s.r[1])
   ds(s.t,160-5*len(s.t),8,s.r[4],s.r[1])
-  ds(s.a,160-5*s.b,36,s.r[3],s.r[1])
+  s.da(s.u)
   s.do()
+ def close(s,b=0):
+  fr(0,0,320,222,s.r[1])
+  if b:s.u=1
+  return[]if b else s.options()
  def open(s):
   s.ds()
+  r=-1
   while 1:
-   r=wk(0,1,2,3,4,52)
-   if r in(4,52)and s.u==0:return[s.p[i][s.c[i]]for i in range(s.s)]
-   elif r in(1,2):
-    if s.u==0:ds(s.a,160-5*s.b,36,s.r[0],s.r[1])
-    s.u=(s.u-1*(r==1)+1*(r==2))%(s.s+1)
+   if r in(5,17):return s.close(1)
+   elif r in(4,52):
+    if s.u<2:return s.close(s.u==0)
+    r=-2
+   elif r in(-1,1,2):
+    if s.u<2:s.da(s.u+1)
+    s.u=(s.u-1*(r==1)+1*(r==2))%(s.s+2)
     s.do()
-    if s.u:s.mo(s.u-1,s.r[3],1)
-    else:ds(s.a,160-5*s.b,36,s.r[3],s.r[1])
-   elif r in(0,3)and s.u:
-    v=s.u-1
-    s.c[v]=s.c[v]+1*(r==3)-1*(r==0)
-    if s.c[v]==1:s.c[v]=len(s.p[v])-1
-    if s.c[v]==len(s.p[v]):s.c[v]=2
-    if s.p[v][0].lower()=="darkmode":#special
+    if s.u>1:s.mo(s.u-2,s.r[3],1)
+    else:s.da(s.u)
+   if r in(-2,0,3)and s.u>1:
+    v=s.u-2
+    s.c[v],l=s.c[v]+1*(r==3)-1*(r==0)if r>=0 else s.p[v][1]+2,s.c[v]
+    o=s.c[v]
+    if o==1:s.c[v]=len(s.p[v])-1
+    if o==len(s.p[v]):s.c[v]=2
+    if l!=o and s.p[v][0].lower()=="darkmode":#special
      s.r[0],s.r[1]=s.r[1],s.r[0]
      s.ds()
     s.mo(v,s.r[3],1)
+   r=wk(0,1,2,3,4,5,17,52)
 def intro(d):
  def pl(letter,x,y,size,color):
   for i,l in enumerate(letter):
-   if l=='1':fr(x+size*(i%3),y+size*(i//3),size,size,color) 
+   if l=='1':fr(x+size*(i%3),y+size*(i//3),size,size,color)
+ a,x,ax,r,c,b,o,e='1'*9+"44334411",0,-110,0,Snake.c[6],Menu.r[1],["Play","Options","Quit"],0
+ y=ay=120
+ fr(0,0,320,222,b)
  for i,l in enumerate((31597,31725,23469,31207)):
   pl(bin(l)[2:],110+40*i,80,10,"0.0")
   sl(0.008)
- a,x,ax,r,c,o='1'*9+"44334411",0,-110,1,Snake.c[6],["Play","Options"]
- y=ay=120
  for i in range(len(a)):
   f=int(a[i])
   x+=((f==1)-(f==3))*10
   y+=((f==2)-(f==4))*10
   if ax<0:ax+=10
   else:
    i=int(a[i-11])
    ax+=((i==1)-(i==3))*10
    ay+=((i==2)-(i==4))*10
-   fr(ax,ay,10,10,"1.0")
+   fr(ax,ay,10,10,b)
   fr(x,y,10,10,"#00cc00")
   sl(0.05)
  pl("001001000001001",x,y,2,"0.0")
  pl("000001110001",x+10,y,2,"red")
  while 1:
   for i,l in enumerate(o):
-   e=1*(r==1)+2*(r==2)
-   f=e==i+1
-   fr(100,140+i*25,140,18,"1.0")
-   ds("> "*f+l+f*" <",110+(110-10*(len(l)+4*f))//2,140+i*25,c if f else "0.0")
+   f=e==i
+   fr(100,140+i*25,140,18,b)
+   ds("> "*f+l+f*" <",110+(110-10*(len(l)+4*f))//2,140+i*25,c if f else Menu.r[0],b)
   r=wk(1,2,4,17,52)
-  if r==17:raise KeyboardInterrupt
-  if r in(4,52):return[]if e==2 else d
+  e=(e-1*(r==1)+1*(r==2))%3
+  if r==17:return 1
+  if r in(4,52):return[]if e==1 else 1 if e==2 else d
+def game(*lb):
+ o=[]
+ while not o:
+  o=intro(menu.options())or menu.open()
+  if o==1:return
+ Snake(lb,*o).start()
 
 menu = Menu("Game Settings","Start Game",
  ["Speed",9]+list(range(1,26)),
  ["Power",1]+list(range(1,21)),
- ["Size",9]+list(range(1,51)),
+ ["Snake Size",9]+list(range(1,51)),
  ["Added Score",0]+list(range(1,21)),
  ["Expert Mode",1,"Yes","No"],
- ["Gost Snake",1,"Yes","No"],
+ ["Babu Mode",1,"Yes","No"],
  ["Darkmode",0,"Enabled","Disabled"],
  ["Rainbow",1,"On","Off"],
  ["Walls",0,"Yes","No"]
 )
 
-Snake((# Leader board: ("name",score),
+game(# Leader board: ("name",score),
   ("Alteur",38),
-  ("ZetaMap",30),
+  ("Lidl Man",37),
+  ("ZetaMap",31),
   ("Nios",23),
   ("Alpha6Frost",17),
 
-), *(intro(menu.default()) or menu.open())).start()
+)
```

### Comparing `kandinsky-2.7.1/src/kandinsky/util/mac_patcher.py` & `kandinsky-2.7.2/src/kandinsky/util/mac_patcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 def Core_event_fire(self: Core, method, *args, **kwargs):
   """Wrapped method of .event_fire(), refresh the window after called the function"""
   value, err = Core_event_fire_(self, method, *args, **kwargs)
   if not self.stopped: Gui.refresh()
   return value, err
 
 def Core_is_alive(self: Core):
-  """Redefine Thread.is_alive() to return always True, because the Thread never started and doesn't want errors about this"""
+  """Redefine Thread.is_alive() to return always True, because the Thread never started and we don't want errors about this"""
   return True
 
 
 # Set new methods in Core
 Core.__init__ = Core___init__
 Core.event_fire = Core_event_fire
 Core.is_alive = Core_is_alive
```

### Comparing `kandinsky-2.7.1/src/kandinsky/util/stuff/color.py` & `kandinsky-2.7.2/src/kandinsky/util/stuff/color.py`

 * *Files identical despite different names*

### Comparing `kandinsky-2.7.1/src/kandinsky/util/stuff/draw.py` & `kandinsky-2.7.2/src/kandinsky/util/stuff/draw.py`

 * *Files identical despite different names*

### Comparing `kandinsky-2.7.1/src/kandinsky/util/stuff/gui.py` & `kandinsky-2.7.2/src/kandinsky/util/stuff/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 class Gui:
   tkmaster:Tk = None
   paused = False
   already_paused = False
   drawable = None
   _main_thread_pid = None # because thread.native_pid don't exist in python<3.8, so use the other way
   heap_set = False
+  resizing_enabled = False # experimental feature
   resizable = False
 
   def created():
     if not Gui.tkmaster: raise RuntimeError("Gui: an instance must be created")
 
   def _unpause_after_wrapper(method):
     # Avoid wrapping method if is not windows, because on other platform the refresh is not "paused"
@@ -53,28 +54,30 @@
 
   def __init__(_, tkmaster):
     # This is now, the video subsystem of SDL will be initialized
     init(video=True)
 
     Gui.tkmaster = tkmaster
     if Vars.is_linux:
-      Gui.linux_menu_font = Font(tkmaster, family="SegoeUI", size=9)
+      Gui.linux_menu_font = Font(Gui.tkmaster, family="SegoeUI", size=9)
       Gui.tkmaster.option_add("*font", Gui.linux_menu_font)
     Gui.data = StateData()
 
     # Create frame area, sdl2 windows and pack everything
-    Gui.head_frame = Frame(tkmaster)
-    Gui.screen_frame = Frame(tkmaster)
+    Gui.head_frame = Frame(Gui.tkmaster)
+    Gui.screen_frame = Frame(Gui.tkmaster)
     Gui.head_frame.pack()
     Gui.screen_frame.pack()
+    if Vars.is_linux:
+      Gui.tkmaster.geometry(f"{Vars.screen[0]}x{Vars.screen[1]+Vars.head_size}") # default size
     Gui.tkmaster.update()
     Gui.head = Window('',(0,0))
     Gui.screen = Window('',(0,0))
 
-    Gui.menu = Menu(tkmaster)
+    Gui.menu = Menu(Gui.tkmaster)
     # Menus
     ## Help menu
     about = Menu(tearoff=False)
     Gui._add_command(about, label="GitHub project",     command=lambda: open_link("https://github.com/ZetaMap/Kandinsky-Numworks"))
     Gui._add_command(about, label="Documentation",      command=lambda: open_link("https://github.com/ZetaMap/Kandinsky-Numworks#usable-content"))
     Gui._add_command(about, label="An issue? Open one", command=lambda: open_link("https://github.com/ZetaMap/Kandinsky-Numworks/issues/new"))
     Gui._secret_var = 0
@@ -152,16 +155,16 @@
     Gui.options.add_command(accelerator="CTRL+P", label="Pause", command=state)
 
     ## Resizing
     def enable_resizing():
       Gui.tkmaster.resizable(Gui.can_resize.get(), Gui.can_resize.get())
       Gui.resizable = Gui.can_resize.get()
     Gui.can_resize = IntVar(value=0)
-    # Disabled for moment
-    #Gui._add_checkbutton(Gui.options, label="Allow resizing", command=enable_resizing, variable=Gui.can_resize)
+    if Gui.resizing_enabled:
+      Gui._add_checkbutton(Gui.options, label="Allow resizing", command=enable_resizing, variable=Gui.can_resize)
 
     Gui.menu.add_cascade(label="Options", menu=Gui.options)
 
   def set_zoom(*_, force=False):
     Gui.created()
 
     Gui.paused = True # Give time to change var, destroy and rebuild window
@@ -172,16 +175,25 @@
     if not force and last_zoom == Vars.zoom_ratio:
       # No need to continue
       if not Gui.already_paused: Gui.paused = False
       return
 
     SDL_DestroyWindow(Gui.head.window)
     SDL_DestroyWindow(Gui.screen.window)
-    Gui.head_frame.config(width=Vars.screen[0]*Vars.zoom_ratio, height=Vars.head_size*Vars.zoom_ratio)
-    Gui.screen_frame.config(width=Vars.screen[0]*Vars.zoom_ratio, height=Vars.screen[1]*Vars.zoom_ratio)
+    width = Vars.window_size[0] if Gui.resizable else Vars.screen[0]*Vars.zoom_ratio
+    height = Vars.window_size[1]-Vars.head_size if Gui.resizable else Vars.screen[1]*Vars.zoom_ratio
+    Gui.head_frame.config(width=width, height=Vars.head_size*Vars.zoom_ratio)
+    Gui.screen_frame.config(width=width, height=height)
+    
+    # fix for KDE
+    if Vars.is_linux:
+      Gui.tkmaster.resizable(True, True)
+      Gui.tkmaster.geometry(f"{width}x{height if Gui.resizable else (Vars.screen[1]+Vars.head_size)*Vars.zoom_ratio}") 
+      Gui.tkmaster.resizable(Gui.resizable, Gui.resizable)
+      
     Gui.tkmaster.update()
     Vars.window_size = (Gui.tkmaster.winfo_width(), Gui.tkmaster.winfo_height())
     Gui.head.window = SDL_CreateWindowFrom(Gui.get_widget_id(Gui.head_frame))
     Gui.screen.window = SDL_CreateWindowFrom(Gui.get_widget_id(Gui.screen_frame))
     Gui.screen_surf = Gui.screen.get_surface()
 
     last_drawable = Gui.drawable
@@ -190,26 +202,27 @@
     Draw.blit_scaled(Gui.drawable, last_drawable)
     Gui.update_data()
 
     Gui.center_window()
     if not Gui.already_paused: Gui.paused = False
 
   def get_widget_id(widget):
-    """Method to get id of widget, will be replaced by mac_patcher.py if needed"""
+    """Method to get id of widget, will be overrided by mac_patcher.py if needed"""
     return widget.winfo_id()
 
   def destroy():
     Gui.created()
 
     SDL_FreeSurface(Gui.drawable)
     SDL_FreeSurface(Gui.head_surface)
     Gui.head.close()
     Gui.screen.close()
-    Gui.tkmaster.destroy()
-    Gui.tkmaster.quit()
+    if Gui.tkmaster.winfo_exists():
+      Gui.tkmaster.destroy()
+      Gui.tkmaster.quit()
     Gui.tkmaster = None
 
   def update_value(int_var, values, min=0):
     Gui.created()
     v = int_var.get()+1
     if v > len(values)-1: v = min
 
@@ -278,15 +291,16 @@
     if Vars.is_windows:
       # Bind events to pause, if dragged or user interact with gui
       def drag_event(e):
         if e.widget is Gui.tkmaster:
           if Gui._drag_window_event_id:
             Gui.tkmaster.after_cancel(Gui._drag_window_event_id)
             Gui.paused = True
-          Gui._drag_window_event_id = Gui.tkmaster.after(200, drag_event_stop)
+          if Gui.tkmaster.winfo_exists():
+            Gui._drag_window_event_id = Gui.tkmaster.after(200, drag_event_stop)
       def drag_event_stop():
         Gui._drag_window_event_id = ''
         if not Gui.already_paused: Gui.paused = False
       drag_event_stop()
       Gui.tkmaster.bind("<Configure>", drag_event)
 
       # Pause on opening menu and unpause when click on frames
@@ -300,15 +314,16 @@
 
     # Resizing ratio fix
     def resize_event(e):
       if Gui.resizable and e.widget == Gui.tkmaster:
         if Gui._resize_window_event_id:
           Gui.tkmaster.after_cancel(Gui._resize_window_event_id)
           Gui.paused = True
-        Gui._resize_window_event_id = Gui.tkmaster.after(50, resize_event_stop, e)
+        if Gui.tkmaster.winfo_exists():
+          Gui._resize_window_event_id = Gui.tkmaster.after(50, resize_event_stop, e)
 
     def resize_event_stop(e=None):
       Gui._resize_window_event_id = ''
       if not e: return
       w, h = e.width, e.height
       if w != Vars.window_size[0] or h != Vars.window_size[1]:
         Gui.tkmaster.geometry(f"{w//Vars.zoom_ratio*Vars.zoom_ratio}x{h//Vars.zoom_ratio*Vars.zoom_ratio}")
```

### Comparing `kandinsky-2.7.1/src/kandinsky/util/stuff/limiter.py` & `kandinsky-2.7.2/src/kandinsky/util/stuff/limiter.py`

 * *Files 9% similar despite different names*

```diff
@@ -108,51 +108,27 @@
 if platform == "win32":
   # Try to use module win-precise-time to get more sleeps precision
   try:
     import win_precise_time as _wpt
     usleep = lambda us: _wpt.sleep_until_ns(int(_wpt.time_ns()+us*1000))
   except:
     import time as _time
-    prettywarn("win-precise-time module is not installed. Using time module to do usleep (emulation will be less accurate)", RuntimeWarning)
+    prettywarn("win-precise-time module not installed. Fallback to time module, emulation will be less accurate", RuntimeWarning)
     def usleep(us):
       t = _time.perf_counter_ns()+us*1000
       while _time.perf_counter_ns() < t: _time.sleep(1e-9)
 
 elif platform == "linux":
   try:
     import ctypes
     usleep = ctypes.CDLL("libc.so.6").usleep
     del ctypes
   except:
     # On some linux distribution, this library is not installed by default
     import time as _time
-    prettywarn("libc6 library is not installed. Using time module to do usleep (emulation will be less accurate)", RuntimeWarning)
+    prettywarn("libc6 library not installed. Fallback to time module, emulation will be less accurate", RuntimeWarning)
     usleep = lambda us: _time.sleep(us/10e6)
 
 else:
   # MacOS don't have libc6 library and idk for other OS so just do a normal sleep
   import time as _time
   usleep = lambda us: _time.sleep(us/10e6)
-
-
-
-# Other stuff, 
-# because there is a bug when window changing monitor 
-# (only on macos... again... this is a poor platform)
-def get_monitors():
-  import ctypes
-  class RECT(ctypes.Structure):
-    _fields_ = [
-      ('left', ctypes.c_long),
-      ('top', ctypes.c_long),
-      ('right', ctypes.c_long),
-      ('bottom', ctypes.c_long)
-      ]
-    def dump(self):
-      return [int(val) for val in (self.left, self.top, self.right, self.bottom)]
-
-  retval = {}
-  def cb(hMonitor, hdcMonitor, lprcMonitor, dwData):
-    retval.update({hMonitor: lprcMonitor.contents.dump()})
-    return True
-  ctypes.windll.user32.EnumDisplayMonitors(0, 0, ctypes.WINFUNCTYPE(ctypes.c_int, ctypes.c_ulong, ctypes.c_ulong, ctypes.POINTER(RECT), ctypes.c_double)(cb), 0)
-  return retval
```

### Comparing `kandinsky-2.7.1/src/kandinsky/util/stuff/tests.py` & `kandinsky-2.7.2/src/kandinsky/util/stuff/tests.py`

 * *Files identical despite different names*

### Comparing `kandinsky-2.7.1/src/kandinsky/util/stuff/vars.py` & `kandinsky-2.7.2/src/kandinsky/util/stuff/vars.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     {"name": "n0120", "ratio": 0, "disabled": True},
   )
 
   default_os = 1
   default_model = 1
   zoom_max = 4
 
+
 # Class to store some data
 class StateData:
   def __init__(self, **content):
     self(**content)
 
   def __call__(self, **content):
     self.__dict__.update(content)
```

### Comparing `kandinsky-2.7.1/src/kandinsky.egg-info/PKG-INFO` & `kandinsky-2.7.2/src/kandinsky.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kandinsky
-Version: 2.7.1
+Version: 2.7.2
 Summary: A small module allowing to link the kandinsky module, from the Numworks, to a window.
 Home-page: https://github.com/ZetaMap/Kandinsky-Numworks
 Author: ZetaMap
 License: MIT
 Project-URL: GitHub Project, https://github.com/ZetaMap/Kandinsky-Numworks
 Project-URL: My GitHub Page, https://github.com/ZetaMap/
 Classifier: Programming Language :: Python :: 3
@@ -25,15 +25,15 @@
 
 This module allowing to link the kandinsky module, from the Numworks, to a window. Useful if you want to test your program without putting it on the calculator. <br>
 In addition, this module also emulates the drawing speed, and has [many other features](https://github.com/ZetaMap/Kandinsky-Numworks/blob/pysdl2/README.md#additional-features).
 
 
 ### Installation
 You now have the option to install this module on [pypi.org](https://pypi.org/project/kandinsky/). For that, follow the steps [here](https://github.com/ZetaMap/Kandinsky-Numworks/blob/pysdl2/FAQ.md#how-to-install-this-module). <br>
-Or if you want, you can build it yourself, just run the command ``./setup``. <br>
+Or if you want, you can build it yourself, just clone the repo and run the command ``./setup``. <br>
 
 ### More
 I also recreated the ion module of the Numworks, check it out here: [Ion module of Numworks](https://github.com/ZetaMap/Ion-numworks)<br>
 If you have a question, check out the [FAQ](https://github.com/ZetaMap/Kandinsky-Numworks/blob/pysdl2/FAQ.md). And if you have a suggestion or your question is not answered, open an [Issue](https://github.com/ZetaMap/Kandinsky-Numworks/issues/new).
 
 
 ### Usable content
@@ -171,7 +171,21 @@
 ```
 
 * Zoom the window:
 ```python
 # from 1 to 4
 os.environ['KANDINSKY_ZOOM_RATIO'] = "<number>"
 ```
+
+
+**Experiental features:**
+
+* Will try to limit the thread heap to get a better emulation:
+```python
+# Note: Cannot be enabled on some python versions
+os.environ['KANDINSKY_USE_HEAP'] = ''
+```
+
+* Add a button in GUI to allow window resising:
+```python
+os.environ['KANDINSKY_ENABLE_RESIZING'] = ''
+```
```

### Comparing `kandinsky-2.7.1/src/kandinsky.egg-info/SOURCES.txt` & `kandinsky-2.7.2/src/kandinsky.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,21 +10,19 @@
 src/kandinsky.egg-info/dependency_links.txt
 src/kandinsky.egg-info/requires.txt
 src/kandinsky.egg-info/top_level.txt
 src/kandinsky/util/3d_demo.py
 src/kandinsky/util/core.py
 src/kandinsky/util/demo.py
 src/kandinsky/util/mac_patcher.py
-src/kandinsky/util/old_config.ini
 src/kandinsky/util/data/app.ico
 src/kandinsky/util/data/app.png
 src/kandinsky/util/data/battery0.png
 src/kandinsky/util/data/battery1.png
 src/kandinsky/util/data/large_font.ttf
-src/kandinsky/util/data/old_icons.zip
 src/kandinsky/util/data/small_font.ttf
 src/kandinsky/util/stuff/__init__.py
 src/kandinsky/util/stuff/color.py
 src/kandinsky/util/stuff/draw.py
 src/kandinsky/util/stuff/gui.py
 src/kandinsky/util/stuff/limiter.py
 src/kandinsky/util/stuff/tests.py
```

