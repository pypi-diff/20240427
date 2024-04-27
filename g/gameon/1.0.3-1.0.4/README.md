# Comparing `tmp/gameon-1.0.3.tar.gz` & `tmp/gameon-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameon-1.0.3.tar", last modified: Fri Apr 26 12:07:27 2024, max compression
+gzip compressed data, was "gameon-1.0.4.tar", last modified: Sat Apr 27 20:45:31 2024, max compression
```

## Comparing `gameon-1.0.3.tar` & `gameon-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 12:07:27.942114 gameon-1.0.3/
--rw-rw-rw-   0        0        0      288 2024-04-26 12:06:36.000000 gameon-1.0.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1060 2022-07-06 14:58:58.000000 gameon-1.0.3/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2022-07-06 14:59:00.000000 gameon-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      262 2024-04-26 12:07:27.941111 gameon-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      172 2022-07-06 14:47:52.000000 gameon-1.0.3/README.txt
-drwxrwxrwx   0        0        0        0 2024-04-26 12:07:27.928102 gameon-1.0.3/gameon/
--rw-rw-rw-   0        0        0    18987 2024-04-26 10:14:47.000000 gameon-1.0.3/gameon/__init__.py
--rw-rw-rw-   0        0        0    21502 2024-04-26 09:50:01.000000 gameon-1.0.3/gameon/__init__.txt
--rw-rw-rw-   0        0        0     1000 2024-04-26 10:07:37.000000 gameon-1.0.3/gameon/engine.txt
--rw-rw-rw-   0        0        0       72 2024-04-26 12:07:12.000000 gameon-1.0.3/gameon/game.py
--rw-rw-rw-   0        0        0     5968 2024-04-26 10:13:16.000000 gameon-1.0.3/gameon/pyeasygame.py
-drwxrwxrwx   0        0        0        0 2024-04-26 12:07:27.941111 gameon-1.0.3/gameon.egg-info/
--rw-rw-rw-   0        0        0      262 2024-04-26 12:07:27.000000 gameon-1.0.3/gameon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2024-04-26 12:07:27.000000 gameon-1.0.3/gameon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 12:07:27.000000 gameon-1.0.3/gameon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-26 12:07:27.000000 gameon-1.0.3/gameon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-26 12:07:27.000000 gameon-1.0.3/gameon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 12:07:27.942114 gameon-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      396 2024-04-25 15:12:35.000000 gameon-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 20:45:31.677612 gameon-1.0.4/
+-rw-rw-rw-   0        0        0      367 2024-04-27 20:45:21.000000 gameon-1.0.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1060 2022-07-06 14:58:58.000000 gameon-1.0.4/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2022-07-06 14:59:00.000000 gameon-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      262 2024-04-27 20:45:31.676612 gameon-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2022-07-06 14:47:52.000000 gameon-1.0.4/README.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 20:45:31.661408 gameon-1.0.4/gameon/
+-rw-rw-rw-   0        0        0    19058 2024-04-27 20:44:49.000000 gameon-1.0.4/gameon/__init__.py
+-rw-rw-rw-   0        0        0    11661 2024-04-25 10:58:03.000000 gameon-1.0.4/gameon/icon.ico
+drwxrwxrwx   0        0        0        0 2024-04-27 20:45:31.676612 gameon-1.0.4/gameon.egg-info/
+-rw-rw-rw-   0        0        0      262 2024-04-27 20:45:31.000000 gameon-1.0.4/gameon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2024-04-27 20:45:31.000000 gameon-1.0.4/gameon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 20:45:31.000000 gameon-1.0.4/gameon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-27 20:45:31.000000 gameon-1.0.4/gameon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-27 20:45:31.000000 gameon-1.0.4/gameon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 20:45:31.677612 gameon-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      396 2024-04-27 20:45:01.000000 gameon-1.0.4/setup.py
```

### Comparing `gameon-1.0.3/LICENCE.txt` & `gameon-1.0.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `gameon-1.0.3/gameon/__init__.py` & `gameon-1.0.4/gameon/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,17 @@
 }
 
 #time
 clock = pygame.time.Clock()
 frames = 120
 
 #window
-pygame.display.set_icon(pygame.image.load('icon.png'))
+icon_path = os.path.join(package_dir, 'logo.ico')
+icon_img = pygame.image.load(icon_path)
+pygame.display.set_icon(icon_img)
 pygame.display.set_caption('GameOn')
 
 #mouse_click
 left_click = False
 right_click = False
 
 #key_pressed
```

