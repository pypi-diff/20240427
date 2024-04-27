# Comparing `tmp/SimpleTKMessageBox-0.2.1.tar.gz` & `tmp/SimpleTKMessageBox-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleTKMessageBox-0.2.1.tar", last modified: Sat Apr 27 11:45:51 2024, max compression
+gzip compressed data, was "SimpleTKMessageBox-0.2.2.tar", last modified: Sat Apr 27 11:59:45 2024, max compression
```

## Comparing `SimpleTKMessageBox-0.2.1.tar` & `SimpleTKMessageBox-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 11:45:51.202451 SimpleTKMessageBox-0.2.1/
--rw-rw-rw-   0        0        0       25 2024-04-27 11:31:25.000000 SimpleTKMessageBox-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0      400 2024-04-27 11:45:51.199446 SimpleTKMessageBox-0.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-27 11:45:51.192450 SimpleTKMessageBox-0.2.1/SimpleTKMessageBox.egg-info/
--rw-rw-rw-   0        0        0      400 2024-04-27 11:45:50.000000 SimpleTKMessageBox-0.2.1/SimpleTKMessageBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2024-04-27 11:45:51.000000 SimpleTKMessageBox-0.2.1/SimpleTKMessageBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 11:45:50.000000 SimpleTKMessageBox-0.2.1/SimpleTKMessageBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-27 11:45:50.000000 SimpleTKMessageBox-0.2.1/SimpleTKMessageBox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-27 11:45:51.187453 SimpleTKMessageBox-0.2.1/SimpleTkMessageBox/
--rw-rw-rw-   0        0        0     3309 2024-04-27 11:39:09.000000 SimpleTKMessageBox-0.2.1/SimpleTkMessageBox/SimpleTkMessageBox.py
--rw-rw-rw-   0        0        0       59 2024-04-27 10:36:23.000000 SimpleTKMessageBox-0.2.1/SimpleTkMessageBox/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-27 11:45:51.203444 SimpleTKMessageBox-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      881 2024-04-27 11:45:17.000000 SimpleTKMessageBox-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:59:45.977463 SimpleTKMessageBox-0.2.2/
+-rw-rw-rw-   0        0        0       25 2024-04-27 11:31:25.000000 SimpleTKMessageBox-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      400 2024-04-27 11:59:45.974464 SimpleTKMessageBox-0.2.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-27 11:59:45.971464 SimpleTKMessageBox-0.2.2/SimpleTKMessageBox.egg-info/
+-rw-rw-rw-   0        0        0      400 2024-04-27 11:59:45.000000 SimpleTKMessageBox-0.2.2/SimpleTKMessageBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      821 2024-04-27 11:59:45.000000 SimpleTKMessageBox-0.2.2/SimpleTKMessageBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 11:59:45.000000 SimpleTKMessageBox-0.2.2/SimpleTKMessageBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-27 11:59:45.000000 SimpleTKMessageBox-0.2.2/SimpleTKMessageBox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 11:59:45.770584 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/
+-rw-rw-rw-   0        0        0     3558 2024-04-27 11:59:39.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/SimpleTkMessageBox.py
+-rw-rw-rw-   0        0        0       59 2024-04-27 10:36:23.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:59:45.783572 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/
+drwxrwxrwx   0        0        0        0 2024-04-27 11:59:45.846536 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W10/
+-rw-rw-rw-   0        0        0     1051 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W10/1.png
+-rw-rw-rw-   0        0        0     1395 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W10/2.png
+-rw-rw-rw-   0        0        0      725 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W10/3.png
+-rw-rw-rw-   0        0        0     1423 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W10/4.png
+-rw-rw-rw-   0        0        0     1145 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W10/5.png
+drwxrwxrwx   0        0        0        0 2024-04-27 11:59:45.900506 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W11/
+-rw-rw-rw-   0        0        0     3154 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W11/1.png
+-rw-rw-rw-   0        0        0     1847 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W11/2.png
+-rw-rw-rw-   0        0        0     3264 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W11/3.png
+-rw-rw-rw-   0        0        0     4962 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W11/4.png
+-rw-rw-rw-   0        0        0     4565 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W11/5.png
+drwxrwxrwx   0        0        0        0 2024-04-27 11:59:45.967469 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W7/
+-rw-rw-rw-   0        0        0     6639 2024-04-23 17:03:58.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W7/1.png
+-rw-rw-rw-   0        0        0     2797 2024-04-23 17:01:54.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W7/2.png
+-rw-rw-rw-   0        0        0     5154 2024-04-23 17:01:56.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W7/3.png
+-rw-rw-rw-   0        0        0     6070 2024-04-23 17:01:59.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W7/4.png
+-rw-rw-rw-   0        0        0     5708 2024-04-23 17:02:02.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/W7/5.png
+-rw-rw-rw-   0        0        0     1406 2024-04-24 08:46:15.000000 SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/icons/transparent.ico
+-rw-rw-rw-   0        0        0       42 2024-04-27 11:59:45.978461 SimpleTKMessageBox-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1305 2024-04-27 11:58:22.000000 SimpleTKMessageBox-0.2.2/setup.py
```

### Comparing `SimpleTKMessageBox-0.2.1/SimpleTkMessageBox/SimpleTkMessageBox.py` & `SimpleTKMessageBox-0.2.2/SimpleTkMessageBox/SimpleTkMessageBox.py`

 * *Files 12% similar despite different names*

```diff
@@ -76,16 +76,19 @@
         MsBbtn3.place(x=315, y=155)
         style = ttk.Style()
         style.configure("BW.TButton", background=colorFrame.cget("bg"))
         MsBbtn3.config(style="BW.TButton")
 
     MsBtext = ttk.Label(MsB, text=text)
     MsBtext.place(x=100, y=60)
-    
+    if sys.platform == "win32":
+        WindowIcon = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'icons\\transparent.ico')
+    else:
+        WindowIcon = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'icons/transparent.ico')
     MsB.title(Title)
     MsB.geometry("400x200")
     MsB.resizable(False, False)
-    MsB.iconphoto(False, None)
+    MsB.iconbitmap(WindowIcon)
     MsB.transient(master)
     MsB.grab_set()
     MsB.wait_window(MsB)
     return button_pressed
```

