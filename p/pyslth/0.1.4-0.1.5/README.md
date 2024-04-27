# Comparing `tmp/pyslth-0.1.4.tar.gz` & `tmp/pyslth-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.1.4.tar", last modified: Fri Apr 26 11:24:52 2024, max compression
+gzip compressed data, was "pyslth-0.1.5.tar", last modified: Sat Apr 27 19:59:22 2024, max compression
```

## Comparing `pyslth-0.1.4.tar` & `pyslth-0.1.5.tar`

### file list

```diff
@@ -1,55 +1,76 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-26 11:24:52.788712 pyslth-0.1.4/
--rw-r--r--   0 breno      (501) staff       (20)       59 2024-04-13 21:50:18.000000 pyslth-0.1.4/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-26 11:24:52.788466 pyslth-0.1.4/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-26 11:24:52.769671 pyslth-0.1.4/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-26 11:24:52.000000 pyslth-0.1.4/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)     1072 2024-04-26 11:24:52.000000 pyslth-0.1.4/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-26 11:24:52.000000 pyslth-0.1.4/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      146 2024-04-26 11:24:52.000000 pyslth-0.1.4/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-26 11:24:52.000000 pyslth-0.1.4/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      138 2024-04-14 18:56:42.000000 pyslth-0.1.4/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-26 11:24:52.788777 pyslth-0.1.4/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-26 11:24:18.000000 pyslth-0.1.4/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-26 11:24:52.776750 pyslth-0.1.4/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3774 2024-04-23 12:02:55.000000 pyslth-0.1.4/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6947 2024-04-26 09:39:45.000000 pyslth-0.1.4/slth/components.py
--rw-r--r--   0 breno      (501) staff       (20)     2149 2024-04-14 19:04:32.000000 pyslth-0.1.4/slth/conf.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-26 11:24:52.777379 pyslth-0.1.4/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.1.4/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.1.4/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    20240 2024-04-26 09:40:03.000000 pyslth-0.1.4/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.1.4/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)     2174 2024-04-22 07:56:01.000000 pyslth-0.1.4/slth/factory.py
--rw-r--r--   0 breno      (501) staff       (20)    25162 2024-04-25 15:16:26.000000 pyslth-0.1.4/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-26 11:24:52.777677 pyslth-0.1.4/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.4/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-26 11:24:52.778449 pyslth-0.1.4/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.4/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.1.4/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.1.4/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-26 11:24:52.781050 pyslth-0.1.4/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.1.4/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.1.4/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)      602 2024-04-18 19:49:54.000000 pyslth-0.1.4/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
--rw-r--r--   0 breno      (501) staff       (20)      452 2024-04-23 08:05:28.000000 pyslth-0.1.4/slth/migrations/0004_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      451 2024-04-23 12:54:25.000000 pyslth-0.1.4/slth/migrations/0005_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.4/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     5330 2024-04-23 11:48:55.000000 pyslth-0.1.4/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.1.4/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.1.4/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    19210 2024-04-25 14:39:52.000000 pyslth-0.1.4/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.1.4/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-26 11:24:52.781693 pyslth-0.1.4/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     8995 2024-04-14 00:29:15.000000 pyslth-0.1.4/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    10955 2024-04-14 10:37:29.000000 pyslth-0.1.4/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    14390 2024-04-22 11:20:25.000000 pyslth-0.1.4/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-26 11:24:52.768189 pyslth-0.1.4/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-26 11:24:52.787534 pyslth-0.1.4/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.1.4/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.1.4/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.1.4/slth/static/images/user.png
--rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.1.4/slth/statistics.py
--rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.1.4/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      893 2024-04-12 02:07:28.000000 pyslth-0.1.4/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1112 2024-04-24 15:04:09.000000 pyslth-0.1.4/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     1995 2024-04-18 12:26:48.000000 pyslth-0.1.4/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 19:59:22.125495 pyslth-0.1.5/
+-rw-r--r--   0 breno      (501) staff       (20)       59 2024-04-13 21:50:18.000000 pyslth-0.1.5/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-27 19:59:22.125284 pyslth-0.1.5/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 19:59:22.093938 pyslth-0.1.5/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-27 19:59:22.000000 pyslth-0.1.5/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)     1697 2024-04-27 19:59:22.000000 pyslth-0.1.5/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-27 19:59:22.000000 pyslth-0.1.5/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      163 2024-04-27 19:59:22.000000 pyslth-0.1.5/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-27 19:59:22.000000 pyslth-0.1.5/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.1.5/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-27 19:59:22.125554 pyslth-0.1.5/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-27 19:57:06.000000 pyslth-0.1.5/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 19:59:22.100333 pyslth-0.1.5/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3774 2024-04-23 12:02:55.000000 pyslth-0.1.5/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6947 2024-04-26 09:39:45.000000 pyslth-0.1.5/slth/components.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 19:59:22.100934 pyslth-0.1.5/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.1.5/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.1.5/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    20236 2024-04-27 15:13:10.000000 pyslth-0.1.5/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.1.5/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)     2379 2024-04-26 12:42:49.000000 pyslth-0.1.5/slth/factory.py
+-rw-r--r--   0 breno      (501) staff       (20)    25162 2024-04-25 15:16:26.000000 pyslth-0.1.5/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 19:59:22.101313 pyslth-0.1.5/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.5/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 19:59:22.101972 pyslth-0.1.5/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.5/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.1.5/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.1.5/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 19:59:22.104416 pyslth-0.1.5/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.1.5/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.1.5/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)      602 2024-04-18 19:49:54.000000 pyslth-0.1.5/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+-rw-r--r--   0 breno      (501) staff       (20)      452 2024-04-23 08:05:28.000000 pyslth-0.1.5/slth/migrations/0004_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      451 2024-04-23 12:54:25.000000 pyslth-0.1.5/slth/migrations/0005_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.5/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     5330 2024-04-23 11:48:55.000000 pyslth-0.1.5/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.1.5/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.1.5/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    19210 2024-04-25 14:39:52.000000 pyslth-0.1.5/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.1.5/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 19:59:22.104971 pyslth-0.1.5/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     8995 2024-04-14 00:29:15.000000 pyslth-0.1.5/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    10955 2024-04-14 10:37:29.000000 pyslth-0.1.5/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    14390 2024-04-22 11:20:25.000000 pyslth-0.1.5/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 19:59:22.105321 pyslth-0.1.5/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 19:59:22.106761 pyslth-0.1.5/slth/static/css/
+-rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.1.5/slth/static/css/fontawesome.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 19:59:22.112574 pyslth-0.1.5/slth/static/css/fonts/
+-rw-r--r--   0 breno      (501) staff       (20)   107280 2024-04-27 15:01:32.000000 pyslth-0.1.5/slth/static/css/fonts/Eina02-Bold.f8011405.ttf
+-rw-r--r--   0 breno      (501) staff       (20)   116316 2024-04-27 15:01:32.000000 pyslth-0.1.5/slth/static/css/fonts/Eina02-Regular.2e682693.ttf
+-rw-r--r--   0 breno      (501) staff       (20)   112880 2024-04-27 15:01:32.000000 pyslth-0.1.5/slth/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
+-rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.1.5/slth/static/css/fonts/fa-solid-900.woff2
+-rw-r--r--   0 breno      (501) staff       (20)      861 2024-04-27 15:14:58.000000 pyslth-0.1.5/slth/static/css/slth.css
+-rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.1.5/slth/static/css/solid.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 19:59:22.115118 pyslth-0.1.5/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.1.5/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.1.5/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.1.5/slth/static/images/user.png
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.1.5/slth/static/index.html
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 19:59:22.124961 pyslth-0.1.5/slth/static/js/
+-rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.1.5/slth/static/js/echarts.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      755 2024-04-27 19:03:35.000000 pyslth-0.1.5/slth/static/js/index.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    80435 2024-04-27 19:03:35.000000 pyslth-0.1.5/slth/static/js/lib.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   117723 2024-04-27 15:01:32.000000 pyslth-0.1.5/slth/static/js/peerjs.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.1.5/slth/static/js/qrcode.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.1.5/slth/static/js/react-trigger-change.js
+-rw-r--r--   0 breno      (501) staff       (20)   141741 2024-04-27 19:03:35.000000 pyslth-0.1.5/slth/static/js/react.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.1.5/slth/static/js/service-worker.js
+-rw-r--r--   0 breno      (501) staff       (20)      129 2024-04-27 15:01:32.000000 pyslth-0.1.5/slth/static/js/slth.js
+-rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.1.5/slth/static/js/vanilla-masker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.1.5/slth/static/js/vanilla-masker.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.1.5/slth/statistics.py
+-rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.1.5/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      893 2024-04-27 15:06:10.000000 pyslth-0.1.5/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1000 2024-04-27 19:14:01.000000 pyslth-0.1.5/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     2264 2024-04-27 19:07:43.000000 pyslth-0.1.5/slth/views.py
```

### Comparing `pyslth-0.1.4/PKG-INFO` & `pyslth-0.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.1.4
+Version: 0.1.5
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.1.4/pyslth.egg-info/PKG-INFO` & `pyslth-0.1.5/pyslth.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.1.4
+Version: 0.1.5
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.1.4/setup.py` & `pyslth-0.1.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.1.4/slth/__init__.py` & `pyslth-0.1.5/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.4/slth/components.py` & `pyslth-0.1.5/slth/components.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.4/slth/db/models.py` & `pyslth-0.1.5/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.4/slth/endpoints.py` & `pyslth-0.1.5/slth/endpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -513,15 +513,15 @@
                     else:
                         print(v)
             for k, v in APPLICATON['menu'].items():
                 item = get_item(k, v)
                 if item:
                     items.append(item)
             profile = Profile.objects.filter(user=self.request.user).first()
-            photo_url = profile.photo.url if profile and profile.photo else '/api/static/images/user.png'
+            photo_url = profile.photo.url if profile and profile.photo else '/static/images/user.png'
             menu = Menu(items, user=self.request.user.username, image=build_url(self.request, photo_url))
         footer = Footer(APPLICATON['version'])
         return Application_(icon=icon, navbar=navbar, menu=menu, footer=footer)
     
 class Manifest(PublicEndpoint):
 
     class Meta:
```

### Comparing `pyslth-0.1.4/slth/factory.py` & `pyslth-0.1.5/slth/factory.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,17 +5,22 @@
         self._values = {}
         self._fieldlist = []
         self._serializer = None
         self._title = None
         self._info = None
         self._actions = {}
         self._delete = delete
+        self._empty = False
 
-    def fields(self, *names) -> 'FormFactory':
+    def fields(self, *names, **values) -> 'FormFactory':
         self._fieldlist.extend(names)
+        for k, v in values.items():
+            self._fieldlist.append(k)
+            self.setvalue(**values)
+        self._empty = not self._fieldlist
         return self
 
     def fieldset(self, title, fields) -> 'FormFactory':
         self._fieldsets[title] = fields
         for field in fields:
             if isinstance(field, str):
                 self._fieldlist.append(field)
@@ -48,15 +53,15 @@
         class Form(ModelForm):
             class Meta:
                 title = self._title or '{} {}'.format(
                     'Excluir' if self._delete else ('Editar' if self._instance.pk else 'Cadastrar'),
                     type(self._instance)._meta.verbose_name
                 )
                 model = type(self._instance)
-                fields = () if self._delete else (self._fieldlist or '__all__')
+                fields = () if self._delete or self._empty else (self._fieldlist or '__all__')
     
         form = Form(instance=self._instance, request=request, delete=self._delete)
         form.fieldsets = self._fieldsets
         if self._serializer:
             form.display(self._serializer)
         if self._info:
             form.info(self._info)
```

### Comparing `pyslth-0.1.4/slth/forms.py` & `pyslth-0.1.5/slth/forms.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.4/slth/management/commands/integration_test.py` & `pyslth-0.1.5/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.4/slth/management/commands/sync.py` & `pyslth-0.1.5/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.4/slth/migrations/0001_initial.py` & `pyslth-0.1.5/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.4/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.1.5/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.4/slth/migrations/0003_rename_photo_profile_alter_profile_options.py` & `pyslth-0.1.5/slth/migrations/0003_rename_photo_profile_alter_profile_options.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.4/slth/models.py` & `pyslth-0.1.5/slth/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.4/slth/permissions.py` & `pyslth-0.1.5/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.4/slth/queryset.py` & `pyslth-0.1.5/slth/queryset.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.4/slth/roles.py` & `pyslth-0.1.5/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.4/slth/selenium/__init__.py` & `pyslth-0.1.5/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.4/slth/selenium/browser.py` & `pyslth-0.1.5/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.4/slth/serializer.py` & `pyslth-0.1.5/slth/serializer.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.4/slth/static/images/logo.png` & `pyslth-0.1.5/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.4/slth/static/images/logo.svg` & `pyslth-0.1.5/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.4/slth/static/images/user.png` & `pyslth-0.1.5/slth/static/images/user.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.4/slth/statistics.py` & `pyslth-0.1.5/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.4/slth/tests.py` & `pyslth-0.1.5/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.4/slth/urls.py` & `pyslth-0.1.5/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.4/slth/utils.py` & `pyslth-0.1.5/slth/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 from django.conf import settings
 
 def build_url(request, path=None):
-    if path and path.startswith('http'):
-        return path
-    elif request:
-        return '{}{}'.format(settings.SITE_URL, path or request.path)
-    return ''
+    return path or request.path if request else ''
 
 def absolute_url(request, *querystrings):
     url = build_url(request)
     if url:
         querstring = request.META.get('QUERY_STRING')
         url = append_url(url, querstring)
         for querystring in querystrings:
```

### Comparing `pyslth-0.1.4/slth/views.py` & `pyslth-0.1.5/slth/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 
 import sys
 import slth
+import socket
 import traceback
+from django.conf import settings
 from .models import Token
 from django.http import JsonResponse
 from django.views.decorators.csrf import csrf_exempt
 from .exceptions import JsonResponseException
 from .serializer import serialize
 from .utils import build_url
 
+from django.shortcuts import render
+
+def index(request, path=None):
+    vite = not socket.socket(socket.AF_INET, socket.SOCK_STREAM).connect_ex(('127.0.0.1',5173))
+    return render(request, 'index.html', dict(vite=vite))
 
 @csrf_exempt
 def dispatcher(request, **kwargs):
     if request.method == 'OPTIONS':
         return ApiResponse({})
     else:
         if(1 and 'application' not in request.path and 'test' not in sys.argv): import time; time.sleep(0)
```

