# Comparing `tmp/SimpleTKMessageBox-0.1.2.tar.gz` & `tmp/SimpleTKMessageBox-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleTKMessageBox-0.1.2.tar", last modified: Sat Apr 27 10:48:16 2024, max compression
+gzip compressed data, was "SimpleTKMessageBox-0.1.3.tar", last modified: Sat Apr 27 10:51:48 2024, max compression
```

## Comparing `SimpleTKMessageBox-0.1.2.tar` & `SimpleTKMessageBox-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 10:48:16.961308 SimpleTKMessageBox-0.1.2/
--rw-rw-rw-   0        0        0      400 2024-04-27 10:48:16.956309 SimpleTKMessageBox-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-27 10:48:16.953311 SimpleTKMessageBox-0.1.2/SimpleTKMessageBox.egg-info/
--rw-rw-rw-   0        0        0      400 2024-04-27 10:48:16.000000 SimpleTKMessageBox-0.1.2/SimpleTKMessageBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-04-27 10:48:16.000000 SimpleTKMessageBox-0.1.2/SimpleTKMessageBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 10:48:16.000000 SimpleTKMessageBox-0.1.2/SimpleTKMessageBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-27 10:48:16.000000 SimpleTKMessageBox-0.1.2/SimpleTKMessageBox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-27 10:48:16.949315 SimpleTKMessageBox-0.1.2/SimpleTkMessageBox/
--rw-rw-rw-   0        0        0     3411 2024-04-27 10:47:54.000000 SimpleTKMessageBox-0.1.2/SimpleTkMessageBox/SimpleTkMessageBox.py
--rw-rw-rw-   0        0        0       59 2024-04-27 10:36:23.000000 SimpleTKMessageBox-0.1.2/SimpleTkMessageBox/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-27 10:48:16.961308 SimpleTKMessageBox-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      490 2024-04-27 10:48:07.000000 SimpleTKMessageBox-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:51:48.942956 SimpleTKMessageBox-0.1.3/
+-rw-rw-rw-   0        0        0      400 2024-04-27 10:51:48.939957 SimpleTKMessageBox-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-27 10:51:48.936959 SimpleTKMessageBox-0.1.3/SimpleTKMessageBox.egg-info/
+-rw-rw-rw-   0        0        0      400 2024-04-27 10:51:48.000000 SimpleTKMessageBox-0.1.3/SimpleTKMessageBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-04-27 10:51:48.000000 SimpleTKMessageBox-0.1.3/SimpleTKMessageBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 10:51:48.000000 SimpleTKMessageBox-0.1.3/SimpleTKMessageBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-27 10:51:48.000000 SimpleTKMessageBox-0.1.3/SimpleTKMessageBox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 10:51:48.931962 SimpleTKMessageBox-0.1.3/SimpleTkMessageBox/
+-rw-rw-rw-   0        0        0     3411 2024-04-27 10:51:34.000000 SimpleTKMessageBox-0.1.3/SimpleTkMessageBox/SimpleTkMessageBox.py
+-rw-rw-rw-   0        0        0       59 2024-04-27 10:36:23.000000 SimpleTKMessageBox-0.1.3/SimpleTkMessageBox/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-27 10:51:48.943954 SimpleTKMessageBox-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      490 2024-04-27 10:51:40.000000 SimpleTKMessageBox-0.1.3/setup.py
```

### Comparing `SimpleTKMessageBox-0.1.2/SimpleTkMessageBox/SimpleTkMessageBox.py` & `SimpleTKMessageBox-0.1.3/SimpleTkMessageBox/SimpleTkMessageBox.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -28,17 +28,17 @@
     else:
         raise ValueError("Invalid Icon : " + Icon + ". It should be one of 'Warning', 'Check', 'Error', 'Question', or 'Information'.")
     
     if IconStyle == "Personalized":
         Path = Icon
     else:
         if sys.platform == "win32":
-            Path = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'icons/' + Style + '/' + IconPath)
-        else:
             Path = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'icons\\' + Style + '\\' + IconPath)
+        else:
+            Path = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'icons/' + Style + '/' + IconPath)
     photo = tkinter.PhotoImage(file=Path)
     image = ttk.Label(master=MsB, text="", image=photo)
     image.place(x=20, y=35)
 
     colorFrame = tkinter.Frame(master=MsB, bg="#e2e2e2", width=400, height=100)
     colorFrame.place(x=0, y=140)
```

