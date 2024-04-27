# Comparing `tmp/SimpleTKMessageBox-0.2.tar.gz` & `tmp/SimpleTKMessageBox-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleTKMessageBox-0.2.tar", last modified: Sat Apr 27 11:32:53 2024, max compression
+gzip compressed data, was "SimpleTKMessageBox-0.2.1.tar", last modified: Sat Apr 27 11:45:51 2024, max compression
```

## Comparing `SimpleTKMessageBox-0.2.tar` & `SimpleTKMessageBox-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 11:32:53.704240 SimpleTKMessageBox-0.2/
--rw-rw-rw-   0        0        0       25 2024-04-27 11:31:25.000000 SimpleTKMessageBox-0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      398 2024-04-27 11:32:53.701242 SimpleTKMessageBox-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-27 11:32:53.698243 SimpleTKMessageBox-0.2/SimpleTKMessageBox.egg-info/
--rw-rw-rw-   0        0        0      398 2024-04-27 11:32:53.000000 SimpleTKMessageBox-0.2/SimpleTKMessageBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2024-04-27 11:32:53.000000 SimpleTKMessageBox-0.2/SimpleTKMessageBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 11:32:53.000000 SimpleTKMessageBox-0.2/SimpleTKMessageBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-27 11:32:53.000000 SimpleTKMessageBox-0.2/SimpleTKMessageBox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-27 11:32:53.695248 SimpleTKMessageBox-0.2/SimpleTkMessageBox/
--rw-rw-rw-   0        0        0     3411 2024-04-27 10:51:34.000000 SimpleTKMessageBox-0.2/SimpleTkMessageBox/SimpleTkMessageBox.py
--rw-rw-rw-   0        0        0       59 2024-04-27 10:36:23.000000 SimpleTKMessageBox-0.2/SimpleTkMessageBox/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-27 11:32:53.704240 SimpleTKMessageBox-0.2/setup.cfg
--rw-rw-rw-   0        0        0      922 2024-04-27 11:32:26.000000 SimpleTKMessageBox-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:45:51.202451 SimpleTKMessageBox-0.2.1/
+-rw-rw-rw-   0        0        0       25 2024-04-27 11:31:25.000000 SimpleTKMessageBox-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      400 2024-04-27 11:45:51.199446 SimpleTKMessageBox-0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-27 11:45:51.192450 SimpleTKMessageBox-0.2.1/SimpleTKMessageBox.egg-info/
+-rw-rw-rw-   0        0        0      400 2024-04-27 11:45:50.000000 SimpleTKMessageBox-0.2.1/SimpleTKMessageBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2024-04-27 11:45:51.000000 SimpleTKMessageBox-0.2.1/SimpleTKMessageBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 11:45:50.000000 SimpleTKMessageBox-0.2.1/SimpleTKMessageBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-27 11:45:50.000000 SimpleTKMessageBox-0.2.1/SimpleTKMessageBox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 11:45:51.187453 SimpleTKMessageBox-0.2.1/SimpleTkMessageBox/
+-rw-rw-rw-   0        0        0     3309 2024-04-27 11:39:09.000000 SimpleTKMessageBox-0.2.1/SimpleTkMessageBox/SimpleTkMessageBox.py
+-rw-rw-rw-   0        0        0       59 2024-04-27 10:36:23.000000 SimpleTKMessageBox-0.2.1/SimpleTkMessageBox/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-27 11:45:51.203444 SimpleTKMessageBox-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      881 2024-04-27 11:45:17.000000 SimpleTKMessageBox-0.2.1/setup.py
```

### Comparing `SimpleTKMessageBox-0.2/SimpleTkMessageBox/SimpleTkMessageBox.py` & `SimpleTKMessageBox-0.2.1/SimpleTkMessageBox/SimpleTkMessageBox.py`

 * *Files 7% similar despite different names*

```diff
@@ -77,16 +77,15 @@
         style = ttk.Style()
         style.configure("BW.TButton", background=colorFrame.cget("bg"))
         MsBbtn3.config(style="BW.TButton")
 
     MsBtext = ttk.Label(MsB, text=text)
     MsBtext.place(x=100, y=60)
     
-    WindowIcon = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'icons\\transparent.ico')
     MsB.title(Title)
     MsB.geometry("400x200")
     MsB.resizable(False, False)
-    MsB.iconbitmap(WindowIcon)
+    MsB.iconphoto(False, None)
     MsB.transient(master)
     MsB.grab_set()
     MsB.wait_window(MsB)
     return button_pressed
```

### Comparing `SimpleTKMessageBox-0.2/setup.py` & `SimpleTKMessageBox-0.2.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from setuptools import setup, find_packages
 setup(
 name='SimpleTKMessageBox',
-version='0.2',
+version='0.2.1',
 author='Gustoon',
 author_email='no.email@gmail.com',
 description='A simple tkinter message box',
 long_description="""
 See documentation at https://github.com/Gustoon/SimpleTkMessageBox
 """,
 packages=find_packages(),
 include_package_data=True,
 data_files=[
-    ('icons', ['icons/transparent.ico']),
     ('icons/W11', ['icons/W11/1.png', 'icons/W11/2.png', 'icons/W11/3.png', 'icons/W11/4.png', 'icons/W11/5.png']),
     ('icons/W10', ['icons/W10/1.png', 'icons/W10/2.png', 'icons/W10/3.png', 'icons/W10/4.png', 'icons/W10/5.png']),
     ('icons/W7', ['icons/W7/1.png', 'icons/W7/2.png', 'icons/W7/3.png', 'icons/W7/4.png', 'icons/W7/5.png']),
 ],
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
```

