# Comparing `tmp/gameon-1.0.4.tar.gz` & `tmp/gameon-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameon-1.0.4.tar", last modified: Sat Apr 27 20:45:31 2024, max compression
+gzip compressed data, was "gameon-1.0.5.tar", last modified: Sat Apr 27 20:49:35 2024, max compression
```

## Comparing `gameon-1.0.4.tar` & `gameon-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 20:45:31.677612 gameon-1.0.4/
--rw-rw-rw-   0        0        0      367 2024-04-27 20:45:21.000000 gameon-1.0.4/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1060 2022-07-06 14:58:58.000000 gameon-1.0.4/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2022-07-06 14:59:00.000000 gameon-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      262 2024-04-27 20:45:31.676612 gameon-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      172 2022-07-06 14:47:52.000000 gameon-1.0.4/README.txt
-drwxrwxrwx   0        0        0        0 2024-04-27 20:45:31.661408 gameon-1.0.4/gameon/
--rw-rw-rw-   0        0        0    19058 2024-04-27 20:44:49.000000 gameon-1.0.4/gameon/__init__.py
--rw-rw-rw-   0        0        0    11661 2024-04-25 10:58:03.000000 gameon-1.0.4/gameon/icon.ico
-drwxrwxrwx   0        0        0        0 2024-04-27 20:45:31.676612 gameon-1.0.4/gameon.egg-info/
--rw-rw-rw-   0        0        0      262 2024-04-27 20:45:31.000000 gameon-1.0.4/gameon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2024-04-27 20:45:31.000000 gameon-1.0.4/gameon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 20:45:31.000000 gameon-1.0.4/gameon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-27 20:45:31.000000 gameon-1.0.4/gameon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-27 20:45:31.000000 gameon-1.0.4/gameon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 20:45:31.677612 gameon-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      396 2024-04-27 20:45:01.000000 gameon-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 20:49:34.999873 gameon-1.0.5/
+-rw-rw-rw-   0        0        0      456 2024-04-27 20:49:25.000000 gameon-1.0.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1060 2022-07-06 14:58:58.000000 gameon-1.0.5/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2022-07-06 14:59:00.000000 gameon-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      262 2024-04-27 20:49:34.998873 gameon-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2022-07-06 14:47:52.000000 gameon-1.0.5/README.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 20:49:34.988119 gameon-1.0.5/gameon/
+-rw-rw-rw-   0        0        0    19058 2024-04-27 20:48:56.000000 gameon-1.0.5/gameon/__init__.py
+-rw-rw-rw-   0        0        0    11661 2024-04-25 10:58:03.000000 gameon-1.0.5/gameon/icon.ico
+drwxrwxrwx   0        0        0        0 2024-04-27 20:49:34.997873 gameon-1.0.5/gameon.egg-info/
+-rw-rw-rw-   0        0        0      262 2024-04-27 20:49:34.000000 gameon-1.0.5/gameon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2024-04-27 20:49:34.000000 gameon-1.0.5/gameon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 20:49:34.000000 gameon-1.0.5/gameon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-27 20:49:34.000000 gameon-1.0.5/gameon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-27 20:49:34.000000 gameon-1.0.5/gameon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 20:49:34.999873 gameon-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      396 2024-04-27 20:49:07.000000 gameon-1.0.5/setup.py
```

### Comparing `gameon-1.0.4/LICENCE.txt` & `gameon-1.0.5/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `gameon-1.0.4/gameon/__init__.py` & `gameon-1.0.5/gameon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 }
 
 #time
 clock = pygame.time.Clock()
 frames = 120
 
 #window
-icon_path = os.path.join(package_dir, 'logo.ico')
+icon_path = os.path.join(package_dir, 'icon.ico')
 icon_img = pygame.image.load(icon_path)
 pygame.display.set_icon(icon_img)
 pygame.display.set_caption('GameOn')
 
 #mouse_click
 left_click = False
 right_click = False
```

### Comparing `gameon-1.0.4/gameon/icon.ico` & `gameon-1.0.5/gameon/icon.ico`

 * *Files identical despite different names*

