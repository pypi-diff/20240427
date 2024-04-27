# Comparing `tmp/SimpleTKMessageBox-0.1.1.tar.gz` & `tmp/SimpleTKMessageBox-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleTKMessageBox-0.1.1.tar", last modified: Sat Apr 27 10:37:01 2024, max compression
+gzip compressed data, was "SimpleTKMessageBox-0.1.2.tar", last modified: Sat Apr 27 10:48:16 2024, max compression
```

## Comparing `SimpleTKMessageBox-0.1.1.tar` & `SimpleTKMessageBox-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 10:37:01.214576 SimpleTKMessageBox-0.1.1/
--rw-rw-rw-   0        0        0      400 2024-04-27 10:37:01.211577 SimpleTKMessageBox-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-27 10:37:01.208578 SimpleTKMessageBox-0.1.1/SimpleTKMessageBox.egg-info/
--rw-rw-rw-   0        0        0      400 2024-04-27 10:37:00.000000 SimpleTKMessageBox-0.1.1/SimpleTKMessageBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-04-27 10:37:01.000000 SimpleTKMessageBox-0.1.1/SimpleTKMessageBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 10:37:00.000000 SimpleTKMessageBox-0.1.1/SimpleTKMessageBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-27 10:37:00.000000 SimpleTKMessageBox-0.1.1/SimpleTKMessageBox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-27 10:37:01.202582 SimpleTKMessageBox-0.1.1/SimpleTkMessageBox/
--rw-rw-rw-   0        0        0     3230 2024-04-27 10:00:48.000000 SimpleTKMessageBox-0.1.1/SimpleTkMessageBox/SimpleTkMessageBox.py
--rw-rw-rw-   0        0        0       59 2024-04-27 10:36:23.000000 SimpleTKMessageBox-0.1.1/SimpleTkMessageBox/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-27 10:37:01.215575 SimpleTKMessageBox-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      490 2024-04-27 10:36:31.000000 SimpleTKMessageBox-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:48:16.961308 SimpleTKMessageBox-0.1.2/
+-rw-rw-rw-   0        0        0      400 2024-04-27 10:48:16.956309 SimpleTKMessageBox-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-27 10:48:16.953311 SimpleTKMessageBox-0.1.2/SimpleTKMessageBox.egg-info/
+-rw-rw-rw-   0        0        0      400 2024-04-27 10:48:16.000000 SimpleTKMessageBox-0.1.2/SimpleTKMessageBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-04-27 10:48:16.000000 SimpleTKMessageBox-0.1.2/SimpleTKMessageBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 10:48:16.000000 SimpleTKMessageBox-0.1.2/SimpleTKMessageBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-27 10:48:16.000000 SimpleTKMessageBox-0.1.2/SimpleTKMessageBox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 10:48:16.949315 SimpleTKMessageBox-0.1.2/SimpleTkMessageBox/
+-rw-rw-rw-   0        0        0     3411 2024-04-27 10:47:54.000000 SimpleTKMessageBox-0.1.2/SimpleTkMessageBox/SimpleTkMessageBox.py
+-rw-rw-rw-   0        0        0       59 2024-04-27 10:36:23.000000 SimpleTKMessageBox-0.1.2/SimpleTkMessageBox/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-27 10:48:16.961308 SimpleTKMessageBox-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      490 2024-04-27 10:48:07.000000 SimpleTKMessageBox-0.1.2/setup.py
```

### Comparing `SimpleTKMessageBox-0.1.1/SimpleTkMessageBox/SimpleTkMessageBox.py` & `SimpleTKMessageBox-0.1.2/SimpleTkMessageBox/SimpleTkMessageBox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from tkinter import ttk
 import tkinter
 import os
-
+import sys
 def ShowMSBox(master, Icon="Information", Title="Message Box", IconStyle="Windows 10", button1="", button2="", button3="", text="This is an info"):
     MsB = tkinter.Toplevel(master)
     StyleList = ["Windows 11","Windows 10", "Windows 7", "Personalized"]
     if not IconStyle in StyleList:
         raise ValueError("Invalid Style : " + IconStyle + ". It should be one of 'Windows 11', 'Windows 10', 'Windows 7' or 'Personalized'.")
 
     if IconStyle == "Windows 11":
@@ -27,15 +27,18 @@
         IconPath = "5.png"
     else:
         raise ValueError("Invalid Icon : " + Icon + ". It should be one of 'Warning', 'Check', 'Error', 'Question', or 'Information'.")
     
     if IconStyle == "Personalized":
         Path = Icon
     else:
-        Path = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'icons/' + Style + '/' + IconPath)
+        if sys.platform == "win32":
+            Path = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'icons/' + Style + '/' + IconPath)
+        else:
+            Path = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'icons\\' + Style + '\\' + IconPath)
     photo = tkinter.PhotoImage(file=Path)
     image = ttk.Label(master=MsB, text="", image=photo)
     image.place(x=20, y=35)
 
     colorFrame = tkinter.Frame(master=MsB, bg="#e2e2e2", width=400, height=100)
     colorFrame.place(x=0, y=140)
```

