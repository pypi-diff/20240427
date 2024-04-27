# Comparing `tmp/funix-0.5.6.tar.gz` & `tmp/funix-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funix-0.5.6.tar", last modified: Sun Apr 21 08:59:44 2024, max compression
+gzip compressed data, was "funix-0.5.7.tar", last modified: Sat Apr 27 10:27:29 2024, max compression
```

## Comparing `funix-0.5.6.tar` & `funix-0.5.7.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-21 08:59:44.149843 funix-0.5.6/
--rw-r--r--   0 yazawazi   (501) staff       (20)     1073 2023-03-14 06:41:17.000000 funix-0.5.6/LICENSE
--rw-r--r--   0 yazawazi   (501) staff       (20)       26 2023-03-14 06:41:17.000000 funix-0.5.6/MANIFEST.in
--rw-r--r--   0 yazawazi   (501) staff       (20)    24396 2024-04-21 08:59:44.149768 funix-0.5.6/PKG-INFO
--rw-r--r--   0 yazawazi   (501) staff       (20)    21517 2024-04-21 08:51:41.000000 funix-0.5.6/README.md
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-21 08:59:44.134766 funix-0.5.6/backend/
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-21 08:59:44.136346 funix-0.5.6/backend/funix/
--rw-r--r--   0 yazawazi   (501) staff       (20)    15566 2024-04-21 08:51:41.000000 funix-0.5.6/backend/funix/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     2889 2024-04-21 08:51:41.000000 funix-0.5.6/backend/funix/__main__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-21 08:59:44.137427 funix-0.5.6/backend/funix/app/
--rw-r--r--   0 yazawazi   (501) staff       (20)     5281 2024-03-06 15:50:54.000000 funix-0.5.6/backend/funix/app/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)      928 2024-02-28 11:05:47.000000 funix-0.5.6/backend/funix/app/websocket.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-21 08:59:44.138098 funix-0.5.6/backend/funix/build/
--rw-r--r--   0 yazawazi   (501) staff       (20)      240 2024-04-21 08:59:36.000000 funix-0.5.6/backend/funix/build/asset-manifest.json
--rw-r--r--   0 yazawazi   (501) staff       (20)     3870 2024-04-21 08:59:09.000000 funix-0.5.6/backend/funix/build/favicon.ico
--rw-r--r--   0 yazawazi   (501) staff       (20)      908 2024-04-21 08:59:36.000000 funix-0.5.6/backend/funix/build/index.html
--rw-r--r--   0 yazawazi   (501) staff       (20)     5347 2024-04-21 08:59:09.000000 funix-0.5.6/backend/funix/build/logo192.png
--rw-r--r--   0 yazawazi   (501) staff       (20)     9664 2024-04-21 08:59:09.000000 funix-0.5.6/backend/funix/build/logo512.png
--rw-r--r--   0 yazawazi   (501) staff       (20)      492 2024-04-21 08:59:09.000000 funix-0.5.6/backend/funix/build/manifest.json
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-21 08:59:44.135022 funix-0.5.6/backend/funix/build/static/
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-21 08:59:44.138216 funix-0.5.6/backend/funix/build/static/css/
--rw-r--r--   0 yazawazi   (501) staff       (20)      292 2024-04-21 08:59:36.000000 funix-0.5.6/backend/funix/build/static/css/main.4efb37a3.css
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-21 08:59:44.144923 funix-0.5.6/backend/funix/build/static/js/
--rw-r--r--   0 yazawazi   (501) staff       (20)   515704 2024-04-21 08:59:36.000000 funix-0.5.6/backend/funix/build/static/js/d3.v5.js
--rw-r--r--   0 yazawazi   (501) staff       (20)    87533 2024-04-21 08:59:36.000000 funix-0.5.6/backend/funix/build/static/js/jquery-3.7.1.min.js
--rw-r--r--   0 yazawazi   (501) staff       (20)  7402218 2024-04-21 08:59:36.000000 funix-0.5.6/backend/funix/build/static/js/main.0af491b9.js
--rw-r--r--   0 yazawazi   (501) staff       (20)     3956 2024-04-21 08:59:36.000000 funix-0.5.6/backend/funix/build/static/js/main.0af491b9.js.LICENSE.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)    63820 2024-04-21 08:59:36.000000 funix-0.5.6/backend/funix/build/static/js/mpld3.v0.5.8.js
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-21 08:59:44.145160 funix-0.5.6/backend/funix/config/
--rw-r--r--   0 yazawazi   (501) staff       (20)     1931 2024-02-28 11:05:47.000000 funix-0.5.6/backend/funix/config/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     1348 2024-02-28 11:05:47.000000 funix-0.5.6/backend/funix/config/switch.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-21 08:59:44.146831 funix-0.5.6/backend/funix/decorator/
--rw-r--r--   0 yazawazi   (501) staff       (20)    22172 2024-04-21 08:51:41.000000 funix-0.5.6/backend/funix/decorator/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)      958 2024-02-28 11:05:47.000000 funix-0.5.6/backend/funix/decorator/all_of.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     4396 2024-02-28 11:05:47.000000 funix-0.5.6/backend/funix/decorator/annnotation_analyzer.py
--rw-r--r--   0 yazawazi   (501) staff       (20)    12930 2024-04-21 08:51:41.000000 funix-0.5.6/backend/funix/decorator/call.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     6201 2024-04-21 08:51:41.000000 funix-0.5.6/backend/funix/decorator/file.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     3355 2024-02-28 11:05:47.000000 funix-0.5.6/backend/funix/decorator/layout.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     5898 2024-02-28 11:05:47.000000 funix-0.5.6/backend/funix/decorator/limit.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     3608 2024-02-28 11:05:47.000000 funix-0.5.6/backend/funix/decorator/lists.py
--rw-r--r--   0 yazawazi   (501) staff       (20)    29288 2024-04-21 08:51:41.000000 funix-0.5.6/backend/funix/decorator/magic.py
--rw-r--r--   0 yazawazi   (501) staff       (20)    14042 2024-04-21 08:51:41.000000 funix-0.5.6/backend/funix/decorator/param.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     1396 2024-04-21 08:51:41.000000 funix-0.5.6/backend/funix/decorator/pre_fill.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     2814 2024-02-28 11:05:47.000000 funix-0.5.6/backend/funix/decorator/reactive.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     7877 2024-03-26 05:59:46.000000 funix-0.5.6/backend/funix/decorator/runtime.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     2633 2024-04-21 08:51:41.000000 funix-0.5.6/backend/funix/decorator/secret.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     2782 2024-02-28 11:05:47.000000 funix-0.5.6/backend/funix/decorator/theme.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     9228 2024-02-28 11:05:47.000000 funix-0.5.6/backend/funix/decorator/widget.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-21 08:59:44.146939 funix-0.5.6/backend/funix/frontend/
--rw-r--r--   0 yazawazi   (501) staff       (20)     3462 2023-12-30 15:45:03.000000 funix-0.5.6/backend/funix/frontend/__init__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-21 08:59:44.147170 funix-0.5.6/backend/funix/hint/
--rw-r--r--   0 yazawazi   (501) staff       (20)    14979 2024-03-26 06:15:40.000000 funix-0.5.6/backend/funix/hint/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     3842 2023-08-26 09:53:24.000000 funix-0.5.6/backend/funix/hint/layout.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-21 08:59:44.147369 funix-0.5.6/backend/funix/prep/
--rw-r--r--   0 yazawazi   (501) staff       (20)        0 2023-05-23 09:39:39.000000 funix-0.5.6/backend/funix/prep/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     5374 2024-04-21 08:51:41.000000 funix-0.5.6/backend/funix/prep/global_to_session.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-21 08:59:44.147470 funix-0.5.6/backend/funix/session/
--rw-r--r--   0 yazawazi   (501) staff       (20)     2310 2024-03-06 15:26:16.000000 funix-0.5.6/backend/funix/session/__init__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-21 08:59:44.147575 funix-0.5.6/backend/funix/test/
--rw-r--r--   0 yazawazi   (501) staff       (20)     5415 2023-08-25 18:04:39.000000 funix-0.5.6/backend/funix/test/test_magic.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-21 08:59:44.147685 funix-0.5.6/backend/funix/theme/
--rw-r--r--   0 yazawazi   (501) staff       (20)    11239 2024-02-28 11:05:47.000000 funix-0.5.6/backend/funix/theme/__init__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-21 08:59:44.148458 funix-0.5.6/backend/funix/util/
--rw-r--r--   0 yazawazi   (501) staff       (20)        0 2023-05-23 03:43:55.000000 funix-0.5.6/backend/funix/util/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     2852 2024-02-28 11:05:47.000000 funix-0.5.6/backend/funix/util/file.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     3518 2024-02-28 11:05:47.000000 funix-0.5.6/backend/funix/util/module.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     4132 2024-02-28 11:05:47.000000 funix-0.5.6/backend/funix/util/network.py
--rw-r--r--   0 yazawazi   (501) staff       (20)      973 2024-02-28 11:05:47.000000 funix-0.5.6/backend/funix/util/secret.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     1067 2024-02-28 11:05:47.000000 funix-0.5.6/backend/funix/util/text.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     1436 2024-02-28 11:05:47.000000 funix-0.5.6/backend/funix/util/uri.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-21 08:59:44.148649 funix-0.5.6/backend/funix/widget/
--rw-r--r--   0 yazawazi   (501) staff       (20)     6516 2024-02-28 11:05:47.000000 funix-0.5.6/backend/funix/widget/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     5067 2023-09-25 00:17:50.000000 funix-0.5.6/backend/funix/widget/builtin.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-21 08:59:44.148807 funix-0.5.6/backend/funix.egg-info/
--rw-r--r--   0 yazawazi   (501) staff       (20)    24396 2024-04-21 08:59:44.000000 funix-0.5.6/backend/funix.egg-info/PKG-INFO
--rw-r--r--   0 yazawazi   (501) staff       (20)     2031 2024-04-21 08:59:44.000000 funix-0.5.6/backend/funix.egg-info/SOURCES.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)        1 2024-04-21 08:59:44.000000 funix-0.5.6/backend/funix.egg-info/dependency_links.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)       50 2024-04-21 08:59:44.000000 funix-0.5.6/backend/funix.egg-info/entry_points.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)      397 2024-04-21 08:59:44.000000 funix-0.5.6/backend/funix.egg-info/requires.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)        6 2024-04-21 08:59:44.000000 funix-0.5.6/backend/funix.egg-info/top_level.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)     1269 2024-04-21 08:51:41.000000 funix-0.5.6/pyproject.toml
--rw-r--r--   0 yazawazi   (501) staff       (20)      114 2024-04-21 08:59:44.150049 funix-0.5.6/setup.cfg
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.438594 funix-0.5.7/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     1073 2023-03-14 06:41:17.000000 funix-0.5.7/LICENSE
+-rw-r--r--   0 yazawazi   (501) staff       (20)       26 2023-03-14 06:41:17.000000 funix-0.5.7/MANIFEST.in
+-rw-r--r--   0 yazawazi   (501) staff       (20)    24396 2024-04-27 10:27:29.438483 funix-0.5.7/PKG-INFO
+-rw-r--r--   0 yazawazi   (501) staff       (20)    21517 2024-04-21 08:51:41.000000 funix-0.5.7/README.md
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.369733 funix-0.5.7/backend/
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.371875 funix-0.5.7/backend/funix/
+-rw-r--r--   0 yazawazi   (501) staff       (20)    15566 2024-04-21 08:51:41.000000 funix-0.5.7/backend/funix/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     2889 2024-04-27 10:26:28.000000 funix-0.5.7/backend/funix/__main__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.373265 funix-0.5.7/backend/funix/app/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     5281 2024-03-06 15:50:54.000000 funix-0.5.7/backend/funix/app/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)      928 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/app/websocket.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.374304 funix-0.5.7/backend/funix/build/
+-rw-r--r--   0 yazawazi   (501) staff       (20)      240 2024-04-27 10:27:09.000000 funix-0.5.7/backend/funix/build/asset-manifest.json
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3870 2024-04-27 10:26:42.000000 funix-0.5.7/backend/funix/build/favicon.ico
+-rw-r--r--   0 yazawazi   (501) staff       (20)      908 2024-04-27 10:27:09.000000 funix-0.5.7/backend/funix/build/index.html
+-rw-r--r--   0 yazawazi   (501) staff       (20)     5347 2024-04-27 10:26:42.000000 funix-0.5.7/backend/funix/build/logo192.png
+-rw-r--r--   0 yazawazi   (501) staff       (20)     9664 2024-04-27 10:26:42.000000 funix-0.5.7/backend/funix/build/logo512.png
+-rw-r--r--   0 yazawazi   (501) staff       (20)      492 2024-04-27 10:26:42.000000 funix-0.5.7/backend/funix/build/manifest.json
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.369989 funix-0.5.7/backend/funix/build/static/
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.374426 funix-0.5.7/backend/funix/build/static/css/
+-rw-r--r--   0 yazawazi   (501) staff       (20)      292 2024-04-27 10:27:09.000000 funix-0.5.7/backend/funix/build/static/css/main.4efb37a3.css
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.425317 funix-0.5.7/backend/funix/build/static/js/
+-rw-r--r--   0 yazawazi   (501) staff       (20)   515704 2024-04-27 10:27:09.000000 funix-0.5.7/backend/funix/build/static/js/d3.v5.js
+-rw-r--r--   0 yazawazi   (501) staff       (20)    87533 2024-04-27 10:27:09.000000 funix-0.5.7/backend/funix/build/static/js/jquery-3.7.1.min.js
+-rw-r--r--   0 yazawazi   (501) staff       (20)  7402218 2024-04-27 10:27:09.000000 funix-0.5.7/backend/funix/build/static/js/main.0af491b9.js
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3956 2024-04-27 10:27:09.000000 funix-0.5.7/backend/funix/build/static/js/main.0af491b9.js.LICENSE.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)    63820 2024-04-27 10:27:09.000000 funix-0.5.7/backend/funix/build/static/js/mpld3.v0.5.8.js
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.426500 funix-0.5.7/backend/funix/config/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     1931 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/config/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     1348 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/config/switch.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.432939 funix-0.5.7/backend/funix/decorator/
+-rw-r--r--   0 yazawazi   (501) staff       (20)    22172 2024-04-21 08:51:41.000000 funix-0.5.7/backend/funix/decorator/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)      958 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/decorator/all_of.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     4396 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/decorator/annnotation_analyzer.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)    12930 2024-04-21 08:51:41.000000 funix-0.5.7/backend/funix/decorator/call.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     6201 2024-04-21 08:51:41.000000 funix-0.5.7/backend/funix/decorator/file.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3355 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/decorator/layout.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     5898 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/decorator/limit.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3608 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/decorator/lists.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)    29288 2024-04-21 08:51:41.000000 funix-0.5.7/backend/funix/decorator/magic.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)    14042 2024-04-21 08:51:41.000000 funix-0.5.7/backend/funix/decorator/param.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     1396 2024-04-21 08:51:41.000000 funix-0.5.7/backend/funix/decorator/pre_fill.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     2814 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/decorator/reactive.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     7877 2024-03-26 05:59:46.000000 funix-0.5.7/backend/funix/decorator/runtime.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     2633 2024-04-21 08:51:41.000000 funix-0.5.7/backend/funix/decorator/secret.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     2782 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/decorator/theme.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     9228 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/decorator/widget.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.433174 funix-0.5.7/backend/funix/frontend/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3462 2023-12-30 15:45:03.000000 funix-0.5.7/backend/funix/frontend/__init__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.433697 funix-0.5.7/backend/funix/hint/
+-rw-r--r--   0 yazawazi   (501) staff       (20)    14979 2024-03-26 06:15:40.000000 funix-0.5.7/backend/funix/hint/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3842 2023-08-26 09:53:24.000000 funix-0.5.7/backend/funix/hint/layout.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.434009 funix-0.5.7/backend/funix/prep/
+-rw-r--r--   0 yazawazi   (501) staff       (20)        0 2023-05-23 09:39:39.000000 funix-0.5.7/backend/funix/prep/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     5374 2024-04-21 08:51:41.000000 funix-0.5.7/backend/funix/prep/global_to_session.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.434299 funix-0.5.7/backend/funix/session/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     2310 2024-03-06 15:26:16.000000 funix-0.5.7/backend/funix/session/__init__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.434523 funix-0.5.7/backend/funix/test/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     5415 2023-08-25 18:04:39.000000 funix-0.5.7/backend/funix/test/test_magic.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.434759 funix-0.5.7/backend/funix/theme/
+-rw-r--r--   0 yazawazi   (501) staff       (20)    11239 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/theme/__init__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.436514 funix-0.5.7/backend/funix/util/
+-rw-r--r--   0 yazawazi   (501) staff       (20)        0 2023-05-23 03:43:55.000000 funix-0.5.7/backend/funix/util/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     2852 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/util/file.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3518 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/util/module.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     4132 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/util/network.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)      973 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/util/secret.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     1067 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/util/text.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     1436 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/util/uri.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.436998 funix-0.5.7/backend/funix/widget/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     6516 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/widget/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     5067 2023-09-25 00:17:50.000000 funix-0.5.7/backend/funix/widget/builtin.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.437317 funix-0.5.7/backend/funix.egg-info/
+-rw-r--r--   0 yazawazi   (501) staff       (20)    24396 2024-04-27 10:27:29.000000 funix-0.5.7/backend/funix.egg-info/PKG-INFO
+-rw-r--r--   0 yazawazi   (501) staff       (20)     2031 2024-04-27 10:27:29.000000 funix-0.5.7/backend/funix.egg-info/SOURCES.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)        1 2024-04-27 10:27:29.000000 funix-0.5.7/backend/funix.egg-info/dependency_links.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)       50 2024-04-27 10:27:29.000000 funix-0.5.7/backend/funix.egg-info/entry_points.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)      397 2024-04-27 10:27:29.000000 funix-0.5.7/backend/funix.egg-info/requires.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)        6 2024-04-27 10:27:29.000000 funix-0.5.7/backend/funix.egg-info/top_level.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)     1269 2024-04-27 10:26:28.000000 funix-0.5.7/pyproject.toml
+-rw-r--r--   0 yazawazi   (501) staff       (20)      114 2024-04-27 10:27:29.438874 funix-0.5.7/setup.cfg
```

### Comparing `funix-0.5.6/LICENSE` & `funix-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/PKG-INFO` & `funix-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funix
-Version: 0.5.6
+Version: 0.5.7
 Summary: Building web apps without manually creating widgets
 Author-email: "Textea Inc." <hello@funix.io>
 License: MIT License
         
         Copyright (c) 2022-2023 Textea Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,15 +36,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: flask>=2.2.2
 Requires-Dist: functions-framework==3.*
 Requires-Dist: requests>=2.28.1
 Requires-Dist: plac>=1.3.5
-Requires-Dist: gitignore_parser>=0.1.9
+Requires-Dist: gitignore-parser>=0.1.9
 Requires-Dist: flask-sock>=0.7.0
 Requires-Dist: SQLAlchemy>=2.0.23
 Provides-Extra: plot
 Requires-Dist: matplotlib>=3.4.3; extra == "plot"
 Requires-Dist: mpld3>=0.5.8; extra == "plot"
 Provides-Extra: git
 Requires-Dist: GitPython>=3.1.31; extra == "git"
```

### Comparing `funix-0.5.6/README.md` & `funix-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/__init__.py` & `funix-0.5.7/backend/funix/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/__main__.py` & `funix-0.5.7/backend/funix/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,12 +77,12 @@
 
 def cli_main():
     """
     The entry point for the command line interface.
 
     This function is called when you run `python -m funix` or `funix` from the command line.
     """
-    plac.call(main, version="Funix 0.5.6")
+    plac.call(main, version="Funix 0.5.7")
 
 
 if __name__ == "__main__":
     cli_main()
```

### Comparing `funix-0.5.6/backend/funix/app/__init__.py` & `funix-0.5.7/backend/funix/app/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/app/websocket.py` & `funix-0.5.7/backend/funix/app/websocket.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/build/favicon.ico` & `funix-0.5.7/backend/funix/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/build/index.html` & `funix-0.5.7/backend/funix/build/index.html`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/build/logo192.png` & `funix-0.5.7/backend/funix/build/logo192.png`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/build/logo512.png` & `funix-0.5.7/backend/funix/build/logo512.png`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/build/static/js/d3.v5.js` & `funix-0.5.7/backend/funix/build/static/js/d3.v5.js`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/build/static/js/jquery-3.7.1.min.js` & `funix-0.5.7/backend/funix/build/static/js/jquery-3.7.1.min.js`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/build/static/js/main.0af491b9.js` & `funix-0.5.7/backend/funix/build/static/js/main.0af491b9.js`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/build/static/js/main.0af491b9.js.LICENSE.txt` & `funix-0.5.7/backend/funix/build/static/js/main.0af491b9.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/build/static/js/mpld3.v0.5.8.js` & `funix-0.5.7/backend/funix/build/static/js/mpld3.v0.5.8.js`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/config/__init__.py` & `funix-0.5.7/backend/funix/config/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/config/switch.py` & `funix-0.5.7/backend/funix/config/switch.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/decorator/__init__.py` & `funix-0.5.7/backend/funix/decorator/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/decorator/all_of.py` & `funix-0.5.7/backend/funix/decorator/all_of.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/decorator/annnotation_analyzer.py` & `funix-0.5.7/backend/funix/decorator/annnotation_analyzer.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/decorator/call.py` & `funix-0.5.7/backend/funix/decorator/call.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/decorator/file.py` & `funix-0.5.7/backend/funix/decorator/file.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/decorator/layout.py` & `funix-0.5.7/backend/funix/decorator/layout.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/decorator/limit.py` & `funix-0.5.7/backend/funix/decorator/limit.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/decorator/lists.py` & `funix-0.5.7/backend/funix/decorator/lists.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/decorator/magic.py` & `funix-0.5.7/backend/funix/decorator/magic.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/decorator/param.py` & `funix-0.5.7/backend/funix/decorator/param.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/decorator/pre_fill.py` & `funix-0.5.7/backend/funix/decorator/pre_fill.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/decorator/reactive.py` & `funix-0.5.7/backend/funix/decorator/reactive.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/decorator/runtime.py` & `funix-0.5.7/backend/funix/decorator/runtime.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/decorator/secret.py` & `funix-0.5.7/backend/funix/decorator/secret.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/decorator/theme.py` & `funix-0.5.7/backend/funix/decorator/theme.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/decorator/widget.py` & `funix-0.5.7/backend/funix/decorator/widget.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/frontend/__init__.py` & `funix-0.5.7/backend/funix/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/hint/__init__.py` & `funix-0.5.7/backend/funix/hint/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/hint/layout.py` & `funix-0.5.7/backend/funix/hint/layout.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/prep/global_to_session.py` & `funix-0.5.7/backend/funix/prep/global_to_session.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/session/__init__.py` & `funix-0.5.7/backend/funix/session/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/test/test_magic.py` & `funix-0.5.7/backend/funix/test/test_magic.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/theme/__init__.py` & `funix-0.5.7/backend/funix/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/util/file.py` & `funix-0.5.7/backend/funix/util/file.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/util/module.py` & `funix-0.5.7/backend/funix/util/module.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/util/network.py` & `funix-0.5.7/backend/funix/util/network.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/util/secret.py` & `funix-0.5.7/backend/funix/util/secret.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/util/text.py` & `funix-0.5.7/backend/funix/util/text.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/util/uri.py` & `funix-0.5.7/backend/funix/util/uri.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/widget/__init__.py` & `funix-0.5.7/backend/funix/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix/widget/builtin.py` & `funix-0.5.7/backend/funix/widget/builtin.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/backend/funix.egg-info/PKG-INFO` & `funix-0.5.7/backend/funix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funix
-Version: 0.5.6
+Version: 0.5.7
 Summary: Building web apps without manually creating widgets
 Author-email: "Textea Inc." <hello@funix.io>
 License: MIT License
         
         Copyright (c) 2022-2023 Textea Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,15 +36,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: flask>=2.2.2
 Requires-Dist: functions-framework==3.*
 Requires-Dist: requests>=2.28.1
 Requires-Dist: plac>=1.3.5
-Requires-Dist: gitignore_parser>=0.1.9
+Requires-Dist: gitignore-parser>=0.1.9
 Requires-Dist: flask-sock>=0.7.0
 Requires-Dist: SQLAlchemy>=2.0.23
 Provides-Extra: plot
 Requires-Dist: matplotlib>=3.4.3; extra == "plot"
 Requires-Dist: mpld3>=0.5.8; extra == "plot"
 Provides-Extra: git
 Requires-Dist: GitPython>=3.1.31; extra == "git"
```

### Comparing `funix-0.5.6/backend/funix.egg-info/SOURCES.txt` & `funix-0.5.7/backend/funix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funix-0.5.6/pyproject.toml` & `funix-0.5.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "funix"
-version = "0.5.6"
+version = "0.5.7"
 authors = [
   {name = "Textea Inc.", email = "hello@funix.io"}
 ]
 license = {file = "LICENSE"}
 description = "Building web apps without manually creating widgets"
 readme = "README.md"
 requires-python = ">=3.10"
@@ -18,15 +18,15 @@
   "Framework :: Matplotlib"
 ]
 dependencies = [
   "flask>=2.2.2",
   "functions-framework==3.*",
   "requests>=2.28.1",
   "plac>=1.3.5",
-  "gitignore_parser>=0.1.9",
+  "gitignore-parser>=0.1.9",
   "flask-sock>=0.7.0",
   "SQLAlchemy>=2.0.23"
 ]
 
 [project.optional-dependencies]
 plot = [
   "matplotlib>=3.4.3",
```

