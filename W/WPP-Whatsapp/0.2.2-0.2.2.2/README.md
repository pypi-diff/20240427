# Comparing `tmp/WPP_Whatsapp-0.2.2.tar.gz` & `tmp/wpp_whatsapp-0.2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WPP_Whatsapp-0.2.2.tar", last modified: Tue Mar 26 07:01:14 2024, max compression
+gzip compressed data, was "wpp_whatsapp-0.2.2.2.tar", last modified: Sat Apr 27 03:18:31 2024, max compression
```

## Comparing `WPP_Whatsapp-0.2.2.tar` & `wpp_whatsapp-0.2.2.2.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:01:14.083465 WPP_Whatsapp-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-03-26 07:01:14.083465 WPP_Whatsapp-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:01:14.075465 WPP_Whatsapp-0.2.2/WPP_Whatsapp/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:01:14.075465 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/Whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:01:14.075465 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/helpers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/helpers/download_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/helpers/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/helpers/jsFunction.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/helpers/scrap-img.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/helpers/wa_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:01:14.079465 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/BusinessLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/CatalogLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/ControlsLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/GroupLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    30318 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/HostLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/LabelsLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12185 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/ListenerLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/ProfileLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12929 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/RetrieverLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19331 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/SenderLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/StatusLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/UILayer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:01:14.079465 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/model/status_find.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:01:14.079465 WPP_Whatsapp-0.2.2/WPP_Whatsapp/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/controllers/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/controllers/browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/controllers/initializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:01:14.079465 WPP_Whatsapp-0.2.2/WPP_Whatsapp/js_lib/
--rw-r--r--   0 runner    (1001) docker     (127)    89768 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/js_lib/wapi.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:01:14.079465 WPP_Whatsapp-0.2.2/WPP_Whatsapp/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp/utils/ffmpeg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:01:14.083465 WPP_Whatsapp-0.2.2/WPP_Whatsapp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-03-26 07:01:14.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-03-26 07:01:14.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 07:01:14.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-26 07:01:14.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-26 07:01:14.000000 WPP_Whatsapp-0.2.2/WPP_Whatsapp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 07:01:14.083465 WPP_Whatsapp-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:01:14.083465 WPP_Whatsapp-0.2.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/test/test_hiden.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-26 07:01:10.000000 WPP_Whatsapp-0.2.2/test/test_setinterval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:31.274876 wpp_whatsapp-0.2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-27 03:18:31.274876 wpp_whatsapp-0.2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:31.266876 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:31.266876 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/Whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:31.266876 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/download_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/jsFunction.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/scrap-img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/wa_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:31.270876 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/BusinessLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/CatalogLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/ControlsLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/GroupLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31817 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/HostLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/LabelsLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/ListenerLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/ProfileLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13361 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/RetrieverLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19632 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/SenderLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/StatusLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/UILayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:31.270876 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/model/status_find.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:31.270876 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/controllers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/controllers/browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/controllers/init_multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10304 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/controllers/initializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:31.270876 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/js_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)    89768 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/js_lib/wapi.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:31.270876 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/utils/ffmpeg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:31.270876 wpp_whatsapp-0.2.2.2/WPP_Whatsapp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-27 03:18:31.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-27 03:18:31.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 03:18:31.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-27 03:18:31.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-27 03:18:31.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 03:18:31.274876 wpp_whatsapp-0.2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:31.270876 wpp_whatsapp-0.2.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/test/test_hiden.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/test/test_setinterval.py
```

### Comparing `WPP_Whatsapp-0.2.2/LICENSE` & `wpp_whatsapp-0.2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.2.2/PKG-INFO` & `wpp_whatsapp-0.2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: WPP_Whatsapp
-Version: 0.2.2
+Version: 0.2.2.2
 Summary: WPP_Whatsapp aim of exporting functions from WhatsApp Web to the python, which can be used to support the creation of any interaction, such as customer service, media sending, intelligence recognition based on phrases artificial and many other things, use your imagination
 Home-page: https://github.com/3mora2/WPP_Whatsapp
 Author: Ammar Alkotb
 Author-email: ammar.alkotb@gmail.com
 License: MIT License
 Project-URL: Bug Report, https://github.com/3mora2/WPP_Whatsapp/issues/new
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: event-emitter-js
 Requires-Dist: greenlet
-Requires-Dist: playwright
+Requires-Dist: playwright>=1.43.0
 Requires-Dist: Pillow
 Requires-Dist: psutil
 Requires-Dist: pyee
 Requires-Dist: segno
 Requires-Dist: typing_extensions
 Requires-Dist: playwright-stealth
 Requires-Dist: node-semver
 Requires-Dist: aiohttp
-Requires-Dist: PlaywrightSafeThread>=0.5.2.1
+Requires-Dist: PlaywrightSafeThread>=0.5.4.1
 
 # WPP_Whatsapp
 <p align="center">
   <a href="https://pypi.org/project/WPP-Whatsapp"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/WPP_Whatsapp.svg?maxAge=86400" /></a>
   <a href="https://pypi.org/project/WPP-Whatsapp"><img alt="View" src="https://static.pepy.tech/personalized-badge/WPP_Whatsapp?period=total&units=international_system&left_text=Downloads"/></a>
 </p>
```

### Comparing `WPP_Whatsapp-0.2.2/README.md` & `wpp_whatsapp-0.2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/Whatsapp.py` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/Whatsapp.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,42 +5,43 @@
 from WPP_Whatsapp.api.layers.BusinessLayer import BusinessLayer
 from WPP_Whatsapp.api.layers.ListenerLayer import ListenerLayer
 
 
 class Whatsapp(BusinessLayer):
     interval: asyncio.Event
 
-    def __init__(self, session, threadsafe_browser, version=None, wa_js_version=None, **kwargs):
+    def __init__(self, session, threadsafe_browser, page, loop=None, version=None, wa_js_version=None, **kwargs):
         self.connected = None
         self.options = {}
         self.options.update(defaultOptions)
         for key, value in kwargs.items():
             if key in self.options:
                 self.options[key] = value
 
         # self.autoCloseInterval = None
-        self.version = version
+        self.version = version or self.options.get('whatsappVersion')
         self.wa_js_version = wa_js_version
         self.autoCloseCalled = False
         self.isInitialized = False
         self.isInjected = False
         self.isStarted = False
         self.isLogged = False
         self.isInChat = False
         # self.checkStartInterval = None
         self.urlCode = ''
         self.status = ''
         self.attempt = 0
         self.lastPercent = ""
         self.lastPercentMessage = ""
         self.session = session
-        self.page = threadsafe_browser.page
-        self.browser = threadsafe_browser.browser
+
+        self.page = page
         self.ThreadsafeBrowser = threadsafe_browser
-        self.loop = threadsafe_browser.loop
+        self.loop = loop or self.ThreadsafeBrowser.loop
+
         self.logger = self.options.get("logger") or Logger
         self.logger.info(f'{self.session}: Initializing...')
         self.logQR = kwargs.get("logQR") or False
         self.autoClose = kwargs.get("autoClose") or self.options.get("autoClose") or 60
         HostLayer.__init__(self)
         ListenerLayer.__init__(self)
         self.handel()
@@ -73,15 +74,16 @@
     #     th.start()
     #     return stopped
 
     async def __intervalHandel(self):
         try:
             # Add window, when WPP not  create yet
             newConnected = await self.ThreadsafeBrowser.page_evaluate(
-                "() => typeof window.WPP !== 'undefined' && window.WPP.conn.isRegistered()")
+                "() => typeof window.WPP !== 'undefined' && window.WPP.conn.isRegistered()", page=self.page
+            )
         except:
             newConnected = None
 
         if newConnected is None or newConnected == self.connected:
             return
         self.connected = newConnected
 
@@ -90,15 +92,15 @@
             if self.statusFind:
                 self.statusFind('disconnectedMobile', self.session)
 
     async def afterPageScriptInjected(self):
         await self._afterPageScriptInjectedHost()
         await self._afterPageScriptInjectedListener()
         is_authenticated = await self.ThreadsafeBrowser.page_evaluate(
-            "() => typeof window.WPP !== 'undefined' &&  WPP.conn.isRegistered()")
+            "() => typeof window.WPP !== 'undefined' &&  WPP.conn.isRegistered()", page=self.page)
         self.connected = is_authenticated
 
     def useHere(self, timeout=120):
         return self.ThreadsafeBrowser.run_threadsafe(self.useHere_, timeout_=timeout)
 
     def logout(self, timeout=120):
         return self.ThreadsafeBrowser.run_threadsafe(self.logout_, timeout_=timeout)
@@ -115,30 +117,30 @@
         return self.ThreadsafeBrowser.run_threadsafe(self.getMessages_, chatId, params, timeout_=timeout)
 
     def rejectCall(self, callId, timeout=120):
         return self.ThreadsafeBrowser.run_threadsafe(self.rejectCall_, callId, timeout_=timeout)
 
     #############################
     async def useHere_(self):
-        return await self.ThreadsafeBrowser.page_evaluate("() => WAPI.takeOver()")
+        return await self.ThreadsafeBrowser.page_evaluate("() => WAPI.takeOver()", page=self.page)
 
     async def logout_(self):
-        return await self.ThreadsafeBrowser.page_evaluate("() => WPP.conn.logout()")
+        return await self.ThreadsafeBrowser.page_evaluate("() => WPP.conn.logout()", page=self.page)
 
     async def getMessageById_(self, messageId):
-        return await self.ThreadsafeBrowser.page_evaluate("(messageId) => WAPI.getMessageById(messageId)", messageId)
+        return await self.ThreadsafeBrowser.page_evaluate("(messageId) => WAPI.getMessageById(messageId)", messageId, page=self.page)
 
     async def getMessages_(self, chatId, params=None):
         """
         :param chatId:
         :param params: (count, id, direction)
         :return:
         """
         if not params:
             params = {}
         chatId = self.valid_chatId(chatId)
         return await self.ThreadsafeBrowser.page_evaluate("({ chatId, params }) => WAPI.getMessages(chatId, params)",
-                                                          {"chatId": chatId, "params": params})
+                                                          {"chatId": chatId, "params": params}, page=self.page)
 
     async def rejectCall_(self, callId):
         return await self.ThreadsafeBrowser.page_evaluate(
-            "({callId}) => WPP.call.rejectCall(callId)", callId)
+            "({callId}) => WPP.call.rejectCall(callId)", callId, page=self.page)
```

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/const.py` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/const.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 import logging
+import os
+import tempfile
 
-useragentOverride = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/102.0.5005.63 Safari/537.36'
+logging.basicConfig(level=logging.ERROR, format='%(asctime)s - %(levelname)s - %(message)s',
+                    datefmt='%d-%b-%y %H:%M:%S')
+Logger = logging.getLogger(name="WPP_Whatsapp")
+
+
+useragentOverride = ('Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) '
+                     'Chrome/102.0.5005.63 Safari/537.36')
 whatsappUrl = 'https://web.whatsapp.com'
 chromiumArgs = [
     '--log-level=3',
     '--start-maximized',
     '--no-default-browser-check',
     '--disable-site-isolation-trials',
     '--no-experiments',
@@ -35,20 +43,22 @@
     '--disable-accelerated-jpeg-decoding',
     '--disable-accelerated-mjpeg-decode',
     '--disable-app-list-dismiss-on-blur',
     '--disable-accelerated-video-decode',
     '--disable-dev-shm-usage',
 ]
 
-logging.basicConfig(level=logging.ERROR, format='%(asctime)s - %(levelname)s - %(message)s',
-                    datefmt='%d-%b-%y %H:%M:%S')
-Logger = logging.getLogger(name="WPP_Whatsapp")
+
+TemporaryTokens = os.path.join(tempfile.gettempdir(), "Tokens")
+if not os.path.exists(TemporaryTokens):
+    os.mkdir(TemporaryTokens)
+
 
 defaultOptions = {
-    "folderNameToken": r"E:\Projects\Python\_Libs_\tokens",
+    "folderNameToken": TemporaryTokens,
     "headless": True,
     "devtools": False,
     "useChrome": True,
     "debug": False,
     "logQR": True,
     "browserWS": '',
     "browserArgs": [''],
@@ -57,14 +67,14 @@
     "updatesLog": True,
     "autoClose": 0,
     "deviceSyncTimeout": 180000,
     "createPathFileToken": True,
     "waitForLogin": True,
     "logger": Logger,
     "tokenStore": 'file',
-    'whatsappVersion': '2.2326.x',
+    'whatsappVersion': '2.2411.x',
     'deviceName': False,
     'linkPreviewApiServers': None,
     'disableGoogleAnalytics': True,
     'googleAnalyticsId': None,
     'poweredBy': 'WPPConnect',
 }
```

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/helpers/decorators.py` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/helpers/download_file.py` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/download_file.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/helpers/jsFunction.py` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/jsFunction.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/helpers/wa_version.py` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/wa_version.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/CatalogLayer.py` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/CatalogLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/ControlsLayer.py` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/ControlsLayer.py`

 * *Files 18% similar despite different names*

```diff
@@ -58,58 +58,58 @@
 
     async def setLimit(self, key, value: bool | int, timeout=60):
         return self.ThreadsafeBrowser.run_threadsafe(self.setLimit_, key, value, timeout_=timeout)
 
     ######################################
     async def unblockContact_(self, contactId):
         contactId = self.valid_chatId(contactId)
-        await self.ThreadsafeBrowser.page_evaluate("(contactId) => WPP.blocklist.unblockContact(contactId)", contactId)
+        await self.ThreadsafeBrowser.page_evaluate("(contactId) => WPP.blocklist.unblockContact(contactId)", contactId, page=self.page)
         return True
 
     async def blockContact_(self, contactId):
         contactId = self.valid_chatId(contactId)
-        await self.ThreadsafeBrowser.page_evaluate("(contactId) => WPP.blocklist.blockContact(contactId)", contactId)
+        await self.ThreadsafeBrowser.page_evaluate("(contactId) => WPP.blocklist.blockContact(contactId)", contactId, page=self.page)
         return True
 
     async def markUnseenMessage_(self, contactId):
         contactId = self.valid_chatId(contactId)
-        await self.ThreadsafeBrowser.page_evaluate("(contactId) => WPP.chat.markIsUnread(contactId)", contactId)
+        await self.ThreadsafeBrowser.page_evaluate("(contactId) => WPP.chat.markIsUnread(contactId)", contactId, page=self.page)
 
     async def deleteChat_(self, chatId):
         chatId = self.valid_chatId(chatId)
-        result = await self.ThreadsafeBrowser.page_evaluate("(chatId) => WPP.chat.delete(chatId)", chatId)
+        result = await self.ThreadsafeBrowser.page_evaluate("(chatId) => WPP.chat.delete(chatId)", chatId, page=self.page)
         return result and result.get("status") == 200
 
     async def archiveChat_(self, chatId, option=True):
         chatId = self.valid_chatId(chatId)
         return await self.ThreadsafeBrowser.page_evaluate("({ chatId, option }) => WPP.chat.archive(chatId, option)",
-                                                          {"chatId": chatId, "option": option})
+                                                          {"chatId": chatId, "option": option}, page=self.page)
 
     async def pinChat_(self, chatId, option, nonExistent=False):
         chatId = self.valid_chatId(chatId)
         if nonExistent:
-            await self.ThreadsafeBrowser.page_evaluate("({ chatId }) => WPP.chat.find(chatId)", chatId)
+            await self.ThreadsafeBrowser.page_evaluate("({ chatId }) => WPP.chat.find(chatId)", chatId, page=self.page)
 
         return await self.ThreadsafeBrowser.page_evaluate("({ chatId, option }) => WPP.chat.pin(chatId, option)",
-                                                          {"chatId": chatId, "option": option})
+                                                          {"chatId": chatId, "option": option}, page=self.page)
 
     async def clearChat_(self, chatId: str, keepStarred=True):
         """
           /**
            * Deletes all messages of given chat
            * @category Chat
            * @param chatId
            * @param keepStarred Keep starred messages
            * @returns boolean
            */
         """
 
         result = await self.ThreadsafeBrowser.page_evaluate(
             "({ chatId, keepStarred }) => WPP.chat.clear(chatId, keepStarred)",
-            {"chatId": chatId, "keepStarred": keepStarred})
+            {"chatId": chatId, "keepStarred": keepStarred}, page=self.page)
 
         return result.get("status") == 200
 
     async def deleteMessage_(self, chatId: str, messageId: list[str] | str, onlyLocal=False, deleteMediaInDevice=True):
         """
           /**
            * Deletes message of given message id
@@ -121,35 +121,35 @@
            */
         """
         await self.ThreadsafeBrowser.page_evaluate(
             """({ chatId, messageId, onlyLocal, deleteMediaInDevice }) => WPP.chat.deleteMessage(
             chatId,messageId,deleteMediaInDevice,!onlyLocal
             )""",
             {"chatId": chatId, "messageId": messageId, "onlyLocal": onlyLocal,
-             "deleteMediaInDevice": deleteMediaInDevice})
+             "deleteMediaInDevice": deleteMediaInDevice}, page=self.page)
         return True
 
     async def editMessage_(self, msgId: str, newText: str, options=None):
         if options is None:
             options = {}
         editResult = await self.ThreadsafeBrowser.page_evaluate(
             "({ msgId, newText, options }) =>  WPP.chat.editMessage(msgId, newText, options)",
-            {"msgId": msgId, "newText": newText, "options": options}
+            {"msgId": msgId, "newText": newText, "options": options}, page=self.page
         )
         result = await self.ThreadsafeBrowser.page_evaluate(
             "async ({ messageId }) => { return JSON.parse(JSON.stringify(await WAPI.getMessageById(messageId)));}",
-            {"messageId": editResult.get("id")}
+            {"messageId": editResult.get("id")}, page=self.page
         )
         if result.get("body") != newText:
             raise Exception(editResult)
 
         return result
 
     async def starMessage_(self, messagesId, star=True):
         return await self.ThreadsafeBrowser.page_evaluate("({ messagesId, star }) => WAPI.starMessages(messagesId, star)",
-                                                   {"messagesId": messagesId, "star": star})
+                                                   {"messagesId": messagesId, "star": star}, page=self.page)
 
     async def setLimit_(self, key, value: bool | int):
         return await self.ThreadsafeBrowser.page_evaluate(
             "({ key, value }) => WPP.conn.setLimit(key as any, value)",
-            {"key": key, "value": value}
+            {"key": key, "value": value}, page=self.page
         )
```

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/GroupLayer.py` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/GroupLayer.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,68 +34,68 @@
 
     def joinGroup(self, invite_code, timeout=60):
         return self.ThreadsafeBrowser.run_threadsafe(self.joinGroup_, invite_code, timeout_=timeout)
 
     ##################################################################################
     async def leaveGroup_(self, groupId):
         groupId = self.valid_chatId(groupId)
-        return await self.ThreadsafeBrowser.page_evaluate("(groupId) => WPP.group.leave(groupId)", groupId)
+        return await self.ThreadsafeBrowser.page_evaluate("(groupId) => WPP.group.leave(groupId)", groupId, page=self.page)
 
     async def getGroupMembersIds_(self, groupId):
         groupId = self.valid_chatId(groupId)
         return await self.ThreadsafeBrowser.page_evaluate("""(groupId) => Promise.resolve(WPP.group.getParticipants(groupId)).then(
-          (participants) => participants.map((p) => p.id))""", groupId)
+          (participants) => participants.map((p) => p.id))""", groupId, page=self.page)
 
     async def getGroupMembers_(self, groupId):
         groupId = self.valid_chatId(groupId)
         membersIds = self.getGroupMembersIds(groupId)
         return [self.getContact(memberId.get("_serialized")) for memberId in membersIds]
 
     async def getGroupInviteLink_(self, chatId):
         chatId = self.valid_chatId(chatId)
-        code = await self.ThreadsafeBrowser.page_evaluate("(chatId) => WPP.group.getInviteCode(chatId)", chatId)
+        code = await self.ThreadsafeBrowser.page_evaluate("(chatId) => WPP.group.getInviteCode(chatId)", chatId, page=self.page)
 
         return f"https://chat.whatsapp.com/{code}" if code else None
 
     async def revokeGroupInviteLink_(self, chatId):
         chatId = self.valid_chatId(chatId)
-        code = await self.ThreadsafeBrowser.page_evaluate("(chatId) => WPP.group.revokeInviteCode(chatId)", chatId)
+        code = await self.ThreadsafeBrowser.page_evaluate("(chatId) => WPP.group.revokeInviteCode(chatId)", chatId, page=self.page)
 
         return f"https://chat.whatsapp.com/{code}" if code else None
 
     async def getGroupInfoFromInviteLink_(self, invite_code):
         invite_code = invite_code.replace('chat.whatsapp.com/', '')
         invite_code = invite_code.replace('invite/', '')
         invite_code = invite_code.replace('https://', '')
         invite_code = invite_code.replace('http://', '')
-        return await self.ThreadsafeBrowser.page_evaluate("(inviteCode) => WPP.group.getGroupInfoFromInviteCode(inviteCode)", invite_code)
+        return await self.ThreadsafeBrowser.page_evaluate("(inviteCode) => WPP.group.getGroupInfoFromInviteCode(inviteCode)", invite_code, page=self.page)
 
     async def createGroup_(self, groupName, contacts=[]):
         return await self.ThreadsafeBrowser.page_evaluate("({ groupName, contacts }) => WPP.group.create(groupName, contacts)",
-                                        {"groupName": groupName, "contacts": contacts})
+                                        {"groupName": groupName, "contacts": contacts}, page=self.page)
 
     async def removeParticipant_(self, groupId, participantId):
         groupId = self.valid_chatId(groupId)
         await self.ThreadsafeBrowser.page_evaluate("""({ groupId, participantId }) =>
-        WPP.group.removeParticipants(groupId, participantId)""", {"groupId": groupId, "participantId": participantId})
+        WPP.group.removeParticipants(groupId, participantId)""", {"groupId": groupId, "participantId": participantId}, page=self.page)
         return True
 
     async def addParticipant_(self, groupId, participantId):
         groupId = self.valid_chatId(groupId)
         return await self.ThreadsafeBrowser.page_evaluate("""({ groupId, participantId }) =>
-        WPP.group.addParticipants(groupId, participantId)""", {"groupId": groupId, "participantId": participantId})
+        WPP.group.addParticipants(groupId, participantId)""", {"groupId": groupId, "participantId": participantId}, page=self.page)
 
     async def getGroupAdmins_(self, chatId):
         chatId = self.valid_chatId(chatId)
         participants = await self.ThreadsafeBrowser.page_evaluate("""(chatId) =>
         Promise.resolve(WPP.group.getParticipants(chatId)).then(
           (participants) => participants.map((p) => p.toJSON())
-        )""", chatId)
+        )""", chatId, page=self.page)
         # return [participant for participant in participants if participant.get("isAdmin")]
         return [participant.get("id") for participant in participants if participant.get("isAdmin")]
 
     async def joinGroup_(self, invite_code):
         invite_code = invite_code.replace('chat.whatsapp.com/', '')
         invite_code = invite_code.replace('invite/', '')
         invite_code = invite_code.replace('https://', '')
         invite_code = invite_code.replace('http://', '')
-        return await self.ThreadsafeBrowser.page_evaluate("(inviteCode) => WPP.group.joinGroup(inviteCode)", invite_code)
+        return await self.ThreadsafeBrowser.page_evaluate("(inviteCode) => WPP.group.joinGroup(inviteCode)", invite_code, page=self.page)
```

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/HostLayer.py` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/HostLayer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import asyncio
 import logging
 import base64 as base64_model
 import mimetypes
 import os
 import re
-import threading
 from datetime import datetime
 from pathlib import Path
 from playwright.async_api import Page
 from WPP_Whatsapp.api.const import whatsappUrl, Logger
 from WPP_Whatsapp.api.helpers.function import asciiQr
 from WPP_Whatsapp.controllers.browser import ThreadsafeBrowser
 from WPP_Whatsapp.api.helpers.jsFunction import setInterval
@@ -17,33 +16,34 @@
 
 class HostLayer:
     page: Page
     session: str
     logger: logging
     ThreadsafeBrowser: "ThreadsafeBrowser"
     options: dict
-    autoCloseInterval: threading.Event
+    autoCloseInterval: asyncio.Event
     autoCloseCalled: bool
     isInitialized: bool
     isInjected: bool
     isStarted: bool
     isLogged: bool
     isInChat: bool
     urlCode: str
     status: str
     attempt: int
     lastPercent: str
     lastPercentMessage: str
     session: str
     autoClose: int
-    checkStartInterval: threading.Event
+    checkStartInterval: asyncio.Event
     logQR: bool
     remain: int
     version: str
     wa_js_version: str
+    loop: object
 
     def __init__(self):
         self.__initialize()
 
     def catchQR(self, **kwargs):
         # self.catchQR_dict = kwargs
         pass
@@ -55,34 +55,35 @@
         pass
 
     def __initialize(self):
         self.page.on('close', self.on_close)
         self.page.on('load', self.on_load)
         self.isInitialized = True
 
-    async def on_close(self):
+    async def on_close(self, _):
         self.logger.info(f'{self.session}: Page Closed')
         self.cancelAutoClose()
 
-    async def on_load(self):
+    async def on_load(self, _):
         self.logger.info(f'{self.session}: Page loaded')
         await self._afterPageLoad()
 
     async def _afterPageLoad(self):
         self.logger.info(f'{self.session}: Injecting wapi.js')
         options = {
             "deviceName": self.options.get("deviceName"),
             "disableGoogleAnalytics": self.options.get("disableGoogleAnalytics"),
             "googleAnalyticsId": self.options.get("googleAnalyticsId"),
             "linkPreviewApiServers": self.options.get("linkPreviewApiServers"),
             "poweredBy": self.options.get("poweredBy"),
         }
         self.logger.info(f'{self.session}: Start WPPConfig')
-        await self.ThreadsafeBrowser.page_evaluate("""(options) => {window.WPPConfig = options;}""", options)
-        # await self.ThreadsafeBrowser.page.page_evaluate("""(options) => {window.WPPConfig = options;}""", options)
+        await self.ThreadsafeBrowser.page_evaluate("""(options) => {window.WPPConfig = options;}""", options,
+                                                   page=self.page)
+        # await self.page.page_evaluate("""(options) => {window.WPPConfig = options;}""", options)
         self.logger.info(f'{self.session}: WPPConfig')
         self.isInjected = False
         # TODO:
 
         if await self.inject_api():
             self.isInjected = True
             self.logger.info(f'{self.session}: wapi.js injected')
@@ -92,48 +93,52 @@
 
     async def _afterPageScriptInjectedHost(self):
         version = await self.getWAVersion()
         self.logger.info(f'{self.session}: WhatsApp WEB version: {version}')
         version = await self.getWAJSVersion()
         self.logger.info(f'{self.session}: WA-JS version: {version}')
         try:
-            await self.ThreadsafeBrowser.page_evaluate("() => {WPP.on('conn.auth_code_change', window.checkQrCode);}")
-            await self.ThreadsafeBrowser.page_evaluate("() => {WPP.on('conn.main_ready', window.checkInChat);}")
+            await self.ThreadsafeBrowser.page_evaluate("() => {WPP.on('conn.auth_code_change', window.checkQrCode);}",
+                                                       page=self.page)
+            await self.ThreadsafeBrowser.page_evaluate("() => {WPP.on('conn.main_ready', window.checkInChat);}",
+                                                       page=self.page)
         except:
             Logger.exception("window.checkQrCode")
         await self.__checkQrCode()
         await self.__checkInChat()
 
     async def start(self):
         if self.isStarted:
             return
 
         self.isStarted = True
         # ToDo:
         await self.initWhatsapp()
 
-        await self.ThreadsafeBrowser.expose_function('checkQrCode', self.__checkQrCode)
-        await self.ThreadsafeBrowser.expose_function('checkInChat', self.__checkInChat)
+        await self.ThreadsafeBrowser.expose_function('checkQrCode', self.__checkQrCode, page=self.page)
+        await self.ThreadsafeBrowser.expose_function('checkInChat', self.__checkInChat, page=self.page)
         # ToDo:
         self.logger.info(f'{self.session}: setInterval__checkStart')
         self.checkStartInterval = setInterval(self.loop, self.__checkStart, 10)
         # self.page.on('close', lambda: self.clearInterval(self.checkStartInterval))
-        return True
+        # return True
 
     ############################### initWhatsapp ####################################################
     async def initWhatsapp(self):
         # await page.setUserAgent(useragentOverride);
         self.logger.info(f'{self.session}: unregisterServiceWorker')
         await self.unregisterServiceWorker()
         if self.version:
             self.logger.info(f'{self.session}: Setting WhatsApp WEB version to {self.version}')
             await self.setWhatsappVersion(self.version)
         self.logger.info(f'{self.session}: Loading WhatsApp WEB')
         # TODO: Unkown Error
-        await self.ThreadsafeBrowser.goto(whatsappUrl, wait_until="domcontentloaded")
+        await self.ThreadsafeBrowser.goto(
+            whatsappUrl, wait_until="load", timeout=0, referer='https://whatsapp.com/', page=self.page
+        )
         # self.ThreadsafeBrowser.sync_goto(whatsappUrl, wait_until="domcontentloaded")
         self.logger.info(f'{self.session}: WhatsApp WEB loaded')
 
     async def unregisterServiceWorker(self):
         try:
             await self.ThreadsafeBrowser.page_evaluate("""() => {
                     setInterval(() => {
@@ -150,15 +155,15 @@
                         }
                       })
                       .catch((err) => null);
                 
                     // Disable service worker registration
                     // @ts-ignore
                     navigator.serviceWorker.register = new Promise(() => {});
-                  }""")
+                  }""", page=self.page)
         except:
             pass
 
     async def setWhatsappVersion(self, version):
         body = ""
         try:
             body = await getPageContent(version)
@@ -221,27 +226,29 @@
         self.statusFind('inChat', self.session)
 
     async def tryAutoClose(self):
         if self.autoCloseInterval:
             self.cancelAutoClose()
 
         if (self.autoClose > 0 or self.options.get(
-                "deviceSyncTimeout") > 0) and (not self.autoCloseInterval or self.autoCloseInterval.is_set()) and not self.page.is_closed():
+                "deviceSyncTimeout") > 0) and (
+                not self.autoCloseInterval or self.autoCloseInterval.is_set()) and not self.page.is_closed():
             self.logger.info(f'{self.session}: Closing the page')
             self.autoCloseCalled = True
             self.statusFind('autocloseCalled', self.session)
             if not self.page.is_closed():
                 await self.ThreadsafeBrowser.close()
 
     def sync_tryAutoClose(self):
         if self.autoCloseInterval:
             self.cancelAutoClose()
 
         if (self.autoClose > 0 or self.options.get(
-                "deviceSyncTimeout") > 0) and (not self.autoCloseInterval or self.autoCloseInterval.is_set()) and not self.page.is_closed():
+                "deviceSyncTimeout") > 0) and (
+                not self.autoCloseInterval or self.autoCloseInterval.is_set()) and not self.page.is_closed():
             self.logger.info(f'{self.session}: Closing the page')
             self.autoCloseCalled = True
             self.statusFind('autocloseCalled', self.session)
             if not self.page.is_closed():
                 self.ThreadsafeBrowser.sync_close()
 
     def startAutoClose(self, _time=None):
@@ -361,24 +368,24 @@
     def waitForPageLoad(self):
         while not self.isInjected:
             if self.page.is_closed():
                 return
             # TODO::
             self.ThreadsafeBrowser.sleep(.2)
 
-        self.ThreadsafeBrowser.page_wait_for_function_sync("() => WPP.isReady")
+        self.ThreadsafeBrowser.page_wait_for_function_sync("() => window.WPP.isReady", page=self.page)
 
     async def waitForPageLoad_(self):
         while not self.isInjected:
             if self.page.is_closed():
                 return
             # TODO::
             await asyncio.sleep(.2)
 
-        await self.ThreadsafeBrowser.page_wait_for_function("() => WPP.isReady")
+        await self.ThreadsafeBrowser.page_wait_for_function("() => window.WPP.isReady", page=self.page)
 
     async def waitForLogin_(self):
         self.logger.info(f'{self.session}: http => Waiting page load')
         await self.waitForPageLoad_()
         self.logger.info(f'{self.session}: http => Checking is logged...')
         authenticated = await self.isAuthenticated()
         self.isLogged = authenticated
@@ -504,65 +511,69 @@
             raise Exception("Page Closed")
 
         self.logger.error(f'{self.session}: Unknow error')
         raise Exception("Unknow error")
 
     def getHostDevice(self):
         """@returns Current host device details"""
-        return self.ThreadsafeBrowser.page_evaluate_sync("() => WAPI.getHost()")
+        return self.ThreadsafeBrowser.page_evaluate_sync("() => WAPI.getHost()", page=self.page)
 
     def getWid(self):
         """@returns Current wid connected"""
-        return self.ThreadsafeBrowser.page_evaluate_sync("() => WAPI.getWid()")
+        return self.ThreadsafeBrowser.page_evaluate_sync("() => WAPI.getWid()", page=self.page)
 
     async def getWAVersion(self):
         """Retrieves WA version"""
-        await self.ThreadsafeBrowser.page_wait_for_function("() => WAPI.getWAVersion()")
-        return await self.ThreadsafeBrowser.page_evaluate("() => WAPI.getWAVersion()")
+        await self.ThreadsafeBrowser.page_wait_for_function("() => WAPI.getWAVersion()", page=self.page)
+        return await self.ThreadsafeBrowser.page_evaluate("() => WAPI.getWAVersion()", page=self.page)
 
     async def getWAJSVersion(self):
-        await self.ThreadsafeBrowser.page_wait_for_function("() => WPP.version")
-        return await self.ThreadsafeBrowser.page_evaluate("() => WPP.version")
+        await self.ThreadsafeBrowser.page_wait_for_function("() => window.WPP.version", page=self.page)
+        return await self.ThreadsafeBrowser.page_evaluate("() => window.WPP.version", page=self.page)
 
     def getConnectionState(self):
-        return self.ThreadsafeBrowser.page_evaluate_sync("() => {return WPP.whatsapp.Socket.state;}")
+        return self.ThreadsafeBrowser.page_evaluate_sync("() => {return window.WPP.whatsapp.Socket.state;}",
+                                                         page=self.page)
 
     def isConnected(self):
         """Retrieves if the phone is online. Please note that this may not be real time."""
-        return self.ThreadsafeBrowser.page_evaluate_sync("() => WAPI.isConnected()")
+        return self.ThreadsafeBrowser.page_evaluate_sync("() => WAPI.isConnected()", page=self.page)
 
     def isLoggedIn(self):
-        return self.ThreadsafeBrowser.page_evaluate_sync("() => WAPI.isLoggedIn()")
+        return self.ThreadsafeBrowser.page_evaluate_sync("() => WAPI.isLoggedIn()", page=self.page)
 
     def getBatteryLevel(self):
-        return self.ThreadsafeBrowser.page_evaluate_sync("() => WAPI.getBatteryLevel()")
+        return self.ThreadsafeBrowser.page_evaluate_sync("() => WAPI.getBatteryLevel()", page=self.page)
 
     def startPhoneWatchdog(self, interval=15000):
-        return self.ThreadsafeBrowser.page_evaluate_sync("(interval) => WAPI.startPhoneWatchdog(interval)", interval)
+        return self.ThreadsafeBrowser.page_evaluate_sync("(interval) => WAPI.startPhoneWatchdog(interval)", interval,
+                                                         page=self.page)
 
     def stopPhoneWatchdog(self):
-        return self.ThreadsafeBrowser.page_evaluate_sync("() => WAPI.stopPhoneWatchdog()")
+        return self.ThreadsafeBrowser.page_evaluate_sync("() => WAPI.stopPhoneWatchdog()", page=self.page)
 
     def isMultiDevice(self):
-        return self.ThreadsafeBrowser.page_evaluate_sync("() => WPP.conn.isMultiDevice()")
+        return self.ThreadsafeBrowser.page_evaluate_sync("() => window.WPP.conn.isMultiDevice()", page=self.page)
 
     async def isAuthenticated(self):
         try:
             if self.page.is_closed():
                 return False
-            return await self.ThreadsafeBrowser.page_evaluate("() => typeof window.WPP !== 'undefined' && WPP.conn.isRegistered()")
+            return await self.ThreadsafeBrowser.page_evaluate(
+                "() => typeof window.WPP !== 'undefined' && window.WPP.conn.isRegistered()", page=self.page)
         except Exception as e:
             self.logger.debug(e)
             return False
 
     def sync_isAuthenticated(self):
         try:
             if self.page.is_closed():
                 return False
-            return self.ThreadsafeBrowser.page_evaluate_sync("() => typeof window.WPP !== 'undefined' && WPP.conn.isRegistered()")
+            return self.ThreadsafeBrowser.page_evaluate_sync(
+                "() => typeof window.WPP !== 'undefined' && window.WPP.conn.isRegistered()", page=self.page)
         except Exception as e:
             self.logger.debug(e)
             return False
 
     async def __needsToScan(self):
         return not await self.isAuthenticated()
 
@@ -570,118 +581,125 @@
         return not self.sync_isAuthenticated()
 
     @staticmethod
     def asciiQr(code):
         return asciiQr(code=code)
 
     async def scrapeImg(self):
-        await self.ThreadsafeBrowser.page_wait_for_function("()=>document.querySelector('canvas')?.closest")
+        await self.ThreadsafeBrowser.page_wait_for_function("()=>document.querySelector('canvas')?.closest",
+                                                            page=self.page)
         click = await self.ThreadsafeBrowser.page_evaluate("""() => {
               const selectorImg = document.querySelector('canvas');
               const selectorUrl = selectorImg.closest('[data-ref]');
               //const buttonReload = selectorUrl.querySelector('[role="button"]') as HTMLButtonElement;
               const buttonReload = selectorUrl.querySelector('button');
               if (buttonReload != null) {
                 buttonReload.click();
                 return true;
               }
               return false;
-            }""")
+            }""", page=self.page)
         if click:
             await self.ThreadsafeBrowser.page_wait_for_function("""() => {
               const selectorImg = document.querySelector('canvas');
               const selectorUrl = selectorImg.closest('[data-ref]');
               return selectorUrl.getAttribute('data-ref');
-            }""")
+            }""", page=self.page)
 
         result = await self.ThreadsafeBrowser.page_evaluate("""() => {
               const selectorImg = document.querySelector('canvas');
               const selectorUrl = selectorImg.closest('[data-ref]');
         
               if (selectorImg != null && selectorUrl != null) {
                 let data = {
                   base64Image: selectorImg.toDataURL(),
                   urlCode: selectorUrl.getAttribute('data-ref'),
                 };
                 return data;
               } else {
                 return undefined;
               }
-            }""")
+            }""", page=self.page)
         return result
 
     async def isInsideChat(self):
-        result = await self.ThreadsafeBrowser.page_evaluate("() => typeof window.WPP !== 'undefined' && WPP.conn.isMainReady()")
+        result = await self.ThreadsafeBrowser.page_evaluate(
+            "() => typeof window.WPP !== 'undefined' && window.WPP.conn.isMainReady()", page=self.page)
         return result if result else False
 
     def sync_isInsideChat(self):
-        result = self.ThreadsafeBrowser.page_evaluate_sync("() => typeof window.WPP !== 'undefined' && window.WPP.conn.isMainReady()")
+        result = self.ThreadsafeBrowser.page_evaluate_sync(
+            "() => typeof window.WPP !== 'undefined' && window.WPP.conn.isMainReady()", page=self.page)
         return result if result else False
 
     async def inject_api(self):
         self.logger.debug(f'{self.session}: start inject')
         try:
             injected = await self.ThreadsafeBrowser.page_evaluate("""() => {
                         return (typeof window.WAPI !== 'undefined' &&typeof window.Store !== 'undefined');}"""
-                                                                  )
+                                                                  , page=self.page)
         except:
             injected = False
 
         if injected:
             self.logger.info(f'{self.session}: already injected')
             return
 
         self.logger.info(f'{self.session}: injected state: {injected}')
+        self.logger.info(f'{self.session}: wait for load webpackChunkwhatsapp_web_client')
         try:
-            await self.ThreadsafeBrowser.page_evaluate(
-                "() => (window?.webpackChunkwhatsapp_web_client?.length || 0) > 3")
+            # await self.ThreadsafeBrowser.page_evaluate(
+            #     "() => (window?.webpackChunkwhatsapp_web_client?.length || 0) > 3", page=self.page)
             await self.ThreadsafeBrowser.page_wait_for_function(
-                "() => (window?.webpackChunkwhatsapp_web_client?.length || 0) > 3")
+                "() => (window?.webpackChunkwhatsapp_web_client?.length || 0) > 3", timeout=10000, page=self.page)
         except:
             pass
-        await asyncio.sleep(1)
-        # TODO::
+        await asyncio.sleep(0.1)
+        self.logger.info(f'{self.session}: inject wppconnect-wa.js')
         # await self.ThreadsafeBrowser.add_script_tag(
         #     url="https://github.com/wppconnect-team/wa-js/releases/download/nightly/wppconnect-wa.js")
-        await self.ThreadsafeBrowser.add_script_tag(** (await getWaJs(self.wa_js_version)))
-        # await self.ThreadsafeBrowser.page_wait_for_function("() => window.WPP?.isReady")
+        await self.ThreadsafeBrowser.add_script_tag(**(await getWaJs(self.wa_js_version)), page=self.page)
+        # await self.ThreadsafeBrowser.page_wait_for_function("() => window.WPP?.isReady", page=self.page)
         try:
             await self.ThreadsafeBrowser.page_evaluate("""() => {
-                                  WPP.chat.defaultSendMessageOptions.createChat = true;
-                                  WPP.conn.setKeepAlive(true);
-                                }""")
+                                  window.WPP.chat.defaultSendMessageOptions.createChat = true;
+                                  window.WPP.conn.setKeepAlive(true);
+                                }""", page=self.page)
         except:
             pass
+        self.logger.info(f'{self.session}: inject wapi.js')
         base_dir = Path(__file__).resolve().parent.parent.parent
-        await self.ThreadsafeBrowser.add_script_tag(path=os.path.join(base_dir, 'js_lib', 'wapi.js'))
+        await self.ThreadsafeBrowser.add_script_tag(path=os.path.join(base_dir, 'js_lib', 'wapi.js'), page=self.page)
         # await self.ThreadsafeBrowser.add_script_tag(
         #     url="https://raw.githubusercontent.com/3mora2/WPP_Whatsapp/main/WPP_Whatsapp/js_lib/wapi.js")
         await self._onLoadingScreen()
+
         try:
+            self.logger.info(f'{self.session}: wait window.WPP.isReady')
             # Make sure WAPI is initialized
             await self.ThreadsafeBrowser.page_wait_for_function("""() => {
             return (typeof window.WAPI !== 'undefined' && typeof window.Store !== 'undefined' && window.WPP.isReady);
-            }""")
+            }""", page=self.page)
         except:
             pass
         return True
 
     def loadingScreen(self, percent, message):
         self.logger.info(f'{self.session}: loadingScreen: {percent}, {message}')
         if self.lastPercent != percent or self.lastPercentMessage != message:
             self.onLoadingScreen(percent, message)
             self.lastPercent = percent
             self.lastPercentMessage = message
 
     async def _onLoadingScreen(self):
         await self.ThreadsafeBrowser.page_evaluate("""function getElementByXpath(path) {
         return document.evaluate(path, document, null, XPathResult.FIRST_ORDERED_NODE_TYPE, null).singleNodeValue;
-            }""")
+            }""", page=self.page)
         try:
-            await self.ThreadsafeBrowser.expose_function('loadingScreen', self.loadingScreen)
+            await self.ThreadsafeBrowser.expose_function('loadingScreen', self.loadingScreen, page=self.page)
         except:
             # Function "loadingScreen" has been already registered
             pass
         await self.ThreadsafeBrowser.page_evaluate("""
         function (selectors) {
               let observer = new MutationObserver(function () {
                 let window2 = window;
@@ -709,15 +727,15 @@
                 characterData: true,
                 subtree: true,
               });
             }""",
                                                    {
                                                        "PROGRESS": "//*[@id='app']/div/div/div[2]/progress",
                                                        "PROGRESS_MESSAGE": "//*[@id='app']/div/div/div[3]",
-                                                   })
+                                                   }, page=self.page)
 
     @staticmethod
     def valid_chatId(chatId):
         chatId = chatId.replace("+", "")
         if chatId and (
                 not chatId.endswith('@c.us') and not chatId.endswith('@g.us') and not chatId.endswith('@newsletter')):
             chatId += '@g.us' if len(chatId) > 15 else '@c.us'
```

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/LabelsLayer.py` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/LabelsLayer.py`

 * *Files 23% similar despite different names*

```diff
@@ -43,15 +43,15 @@
            * ```
            * @param name Name of label
            * @param options options of label
            */
         """
         return await self.ThreadsafeBrowser.page_evaluate("""({ name, options }) => {
         WPP.labels.addNewLabel(name, options);
-      }""", {"name": name, "options": options})
+      }""", {"name": name, "options": options}, page=self.page)
 
     async def addOrRemoveLabels_(self, chatIds, options):
         """
           /**
            * Add or delete label of chatId
            * @category Labels
            *
@@ -63,20 +63,20 @@
            * ```
            * @param chatIds ChatIds
            * @param options options to remove or add
            */
         """
         return await self.ThreadsafeBrowser.page_evaluate("""({ chatIds, options }) => {
         WPP.labels.addOrRemoveLabels(chatIds, options);
-      }""", {"chatIds": chatIds, "options": options})
+      }""", {"chatIds": chatIds, "options": options}, page=self.page)
 
     async def getAllLabels_(self):
-        return await self.ThreadsafeBrowser.page_evaluate("() => WPP.labels.getAllLabels()")
+        return await self.ThreadsafeBrowser.page_evaluate("() => WPP.labels.getAllLabels()", page=self.page)
 
     async def getLabelById_(self, Id):
-        return await self.ThreadsafeBrowser.page_evaluate("""({ id }) => {WPP.labels.getLabelById(id); }""", {"id": Id})
+        return await self.ThreadsafeBrowser.page_evaluate("""({ id }) => {WPP.labels.getLabelById(id); }""", {"id": Id}, page=self.page)
 
     async def deleteAllLabels_(self):
-        return await self.ThreadsafeBrowser.page_evaluate("""() => {WPP.labels.deleteAllLabels();}""")
+        return await self.ThreadsafeBrowser.page_evaluate("""() => {WPP.labels.deleteAllLabels();}""", page=self.page)
 
     async def deleteLabel_(self, Id):
-        return await self.ThreadsafeBrowser.page_evaluate("""({ id }) => {WPP.labels.deleteLabel(id); }""", {"id": Id})
+        return await self.ThreadsafeBrowser.page_evaluate("""({ id }) => {WPP.labels.deleteLabel(id); }""", {"id": Id}, page=self.page)
```

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/ListenerLayer.py` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/ListenerLayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,19 +62,19 @@
             'onIncomingCall',
             'onRevokedMessage',
             'onReactionMessage',
             'onPollResponse'
         ]
 
         for func in functions:
-            has = await self.ThreadsafeBrowser.page_evaluate("(func) => typeof window[func] === 'function'", func)
+            has = await self.ThreadsafeBrowser.page_evaluate("(func) => typeof window[func] === 'function'", func, page=self.page)
             if not has:
                 self.logger.debug(f'{self.session}: Exposing {func} function')
                 handel_func = HandelFunc(func, self.session, self.logger, self.__listenerEmitter).handel_func
-                await self.ThreadsafeBrowser.expose_function(func, handel_func)
+                await self.ThreadsafeBrowser.expose_function(func, handel_func, page=self.page)
 
         await self.ThreadsafeBrowser.page_evaluate("""() => {
         try {
           if (!window['onMessage'].exposed) {
             WPP.on('chat.new_message', (msg) => {
               if (msg.isSentByMe || msg.isStatusV3) {
                 return;
@@ -237,15 +237,15 @@
             });
             window['onParticipantsChanged'].exposed = true;
           }
         } catch (error) {
           console.error(error);
         }
         */
-      }""")
+      }""", page=self.page)
 
     def __registerEvent(self, event, listener):
         """
         /**
         * Register the event and create a disposable object to stop the listening
         * @param event Name of event
         * @param listener The function to execute
@@ -338,18 +338,18 @@
            * }
            * ```
            *
            * @param id contact id (xxxxx@c.us) or group id: xxxxx-yyyy@g.us
            * @returns number of subscribed
            */
         """
-        await self.ThreadsafeBrowser.page_evaluate("(id) => WAPI.subscribePresence(id)", id_)
+        await self.ThreadsafeBrowser.page_evaluate("(id) => WAPI.subscribePresence(id)", id_, page=self.page)
 
     async def unsubscribePresence(self, id_):
-        await self.ThreadsafeBrowser.page_evaluate("(id) => WAPI.unsubscribePresence(id)", id_)
+        await self.ThreadsafeBrowser.page_evaluate("(id) => WAPI.unsubscribePresence(id)", id_, page=self.page)
 
     def onRevokedMessage(self, callback):
         """ """
         return self.__registerEvent("onRevokedMessage", callback)
 
     def onReactionMessage(self, callback):
         """ """
```

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/ProfileLayer.py` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/ProfileLayer.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,35 +42,35 @@
            * @param time duration of silence
            * @param type kind of silence "hours" "minutes" "year"
            * To remove the silence, just enter the contact parameter
            */
         """
         chatId = self.valid_chatId(chatId)
         return await self.ThreadsafeBrowser.page_evaluate("(id, time, type) => WAPI.sendMute(id, time, type)",
-                                                          {"id": chatId, "time": time, "type": type})
+                                                          {"id": chatId, "time": time, "type": type}, page=self.page)
 
     async def setTheme_(self, type_):
         """
            * Change the theme
            * @category Host
            * @param string types "dark" or "light"
         """
-        return await self.ThreadsafeBrowser.page_evaluate("(type_) => WAPI.setTheme(type_)", type_)
+        return await self.ThreadsafeBrowser.page_evaluate("(type_) => WAPI.setTheme(type_)", type_, page=self.page)
 
     async def setProfileStatus_(self, status):
         """
           /**
            * Sets current user profile status
            * @category Profile
            * @param status
            */
         """
         return await self.ThreadsafeBrowser.page_evaluate("""({ status }) => {
             WPP.profile.setMyStatus(status);
-          }""", status)
+          }""", status, page=self.page)
 
     async def setProfilePic_(self, pathOrBase64, to):
         pass
         # ToDO:
         # base64 = ''
         # if pathOrBase64.startswith('data:'):
         #     base64 = pathOrBase64
@@ -83,11 +83,11 @@
         #     return
         # mimeInfo = base64.split(";base64")[0].split(":")[-1]
         # if 'image' not in mimeInfo:
         #     print('Not an image, allowed formats png, jpeg and webp')
         #     return
 
     async def setProfileName_(self, name):
-        return await self.ThreadsafeBrowser.page_evaluate("({ name }) => {WAPI.setMyName(name);}", name)
+        return await self.ThreadsafeBrowser.page_evaluate("({ name }) => {WAPI.setMyName(name);}", name, page=self.page)
 
     async def removeMyProfilePicture_(self):
-        return await self.ThreadsafeBrowser.page_evaluate("() => WPP.profile.removeMyProfilePicture()")
+        return await self.ThreadsafeBrowser.page_evaluate("() => WPP.profile.removeMyProfilePicture()", page=self.page)
```

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/RetrieverLayer.py` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/RetrieverLayer.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 
     def getTheme(self, timeout=60):
         return self.ThreadsafeBrowser.run_threadsafe(
             self.getTheme_, timeout_=timeout)
 
     def getAllChats(self, withNewMessageOnly=False, timeout=60):
         return self.ThreadsafeBrowser.run_threadsafe(
-            self.getAllChats_, self, withNewMessageOnly, timeout_=timeout)
+            self.getAllChats_, withNewMessageOnly, timeout_=timeout)
 
     def checkNumberStatus(self, contactId, timeout=60):
         return self.ThreadsafeBrowser.run_threadsafe(
             self.checkNumberStatus_, contactId, timeout_=timeout)
 
     def getAllChatsWithMessages(self, withNewMessageOnly=False, timeout=60):
         return self.ThreadsafeBrowser.run_threadsafe(
             self.getAllChatsWithMessages_, withNewMessageOnly, timeout_=timeout)
 
-    def getAllGroups(self, withNewMessagesOnly, timeout=60):
+    def getAllGroups(self, withNewMessagesOnly=False, timeout=60):
         return self.ThreadsafeBrowser.run_threadsafe(
             self.getAllGroups_, withNewMessagesOnly, timeout_=timeout)
 
     def getAllBroadcastList(self, timeout=60):
         return self.ThreadsafeBrowser.run_threadsafe(
             self.getAllBroadcastList_, timeout_=timeout)
 
@@ -102,177 +102,177 @@
         return self.ThreadsafeBrowser.run_threadsafe(
             self.getVotes_, msgId, timeout_=timeout)
 
     ########################################################
     async def getSessionTokenBrowser_(self, removePath):
         # @returns obj [token]
         if removePath:
-            await self.ThreadsafeBrowser.page_evaluate("() => {window['pathSession'] = true;}")
+            await self.ThreadsafeBrowser.page_evaluate("() => {window['pathSession'] = true;}", page=self.page)
 
         if self.isMultiDevice():
             return await self.ThreadsafeBrowser.page_evaluate("""() => {
           if (window.localStorage) {
             return {
               WABrowserId:
                 window.localStorage.getItem('WABrowserId') || 'MultiDevice',
               WASecretBundle: 'MultiDevice',
               WAToken1: 'MultiDevice',
               WAToken2: 'MultiDevice',
             };
           }
           return null;
-        }""")
+        }""", page=self.page)
         return await self.ThreadsafeBrowser.page_evaluate("""() => {
         if (window.localStorage) {
           return {
             WABrowserId: window.localStorage.getItem('WABrowserId'),
             WASecretBundle: window.localStorage.getItem('WASecretBundle'),
             WAToken1: window.localStorage.getItem('WAToken1'),
             WAToken2: window.localStorage.getItem('WAToken2'),
           };
         }
         return null;
-      }""")
+      }""", page=self.page)
 
     async def getTheme_(self):
         # @returns string light or dark
-        return await self.ThreadsafeBrowser.page_evaluate("() => WAPI.getTheme()")
+        return await self.ThreadsafeBrowser.page_evaluate("() => WAPI.getTheme()", page=self.page)
 
     async def getAllChats_(self, withNewMessageOnly=False):
         # @returns array of [Chat]
         if withNewMessageOnly:
-            return await self.ThreadsafeBrowser.page_evaluate("() => WAPI.getAllChatsWithNewMsg()")
+            return await self.ThreadsafeBrowser.page_evaluate("() => WAPI.getAllChatsWithNewMsg()", page=self.page)
 
-        return await self.ThreadsafeBrowser.page_evaluate("() => WAPI.getAllChats()")
+        return await self.ThreadsafeBrowser.page_evaluate("() => WAPI.getAllChats()", page=self.page)
 
     async def checkNumberStatus_(self, contactId):
         # @returns contact detial as promise
         contactId = self.valid_chatId(contactId)
-        return await self.ThreadsafeBrowser.page_evaluate("(contactId) => WAPI.checkNumberStatus(contactId)", contactId)
+        return await self.ThreadsafeBrowser.page_evaluate("(contactId) => WAPI.checkNumberStatus(contactId)", contactId, page=self.page)
 
     async def getAllChatsWithMessages_(self, withNewMessageOnly=False):
         # @returns array of [Chat]
         return await self.ThreadsafeBrowser.page_evaluate("""(withNewMessageOnly: boolean) =>
-        WAPI.getAllChatsWithMessages(withNewMessageOnly)""", withNewMessageOnly)
+        WAPI.getAllChatsWithMessages(withNewMessageOnly)""", withNewMessageOnly, page=self.page)
 
     async def getAllGroups_(self, withNewMessagesOnly):
         # @returns array of groups
         return await self.ThreadsafeBrowser.page_evaluate("""async ({ withNewMessagesOnly }) => {
         const chats = await WPP.chat.list({
           onlyGroups: true,
           onlyWithUnreadMessage: withNewMessagesOnly,
         });
 
         const groups = await Promise.all(
           chats.map((c) => WPP.group.ensureGroup(c.id))
         );
 
         return groups.map((g) => WAPI._serializeChatObj(g));
-      }""", withNewMessagesOnly)
+      }""", withNewMessagesOnly, page=self.page)
 
     async def getAllBroadcastList_(self):
         # @returns array of broadcast list
-        chats = await self.ThreadsafeBrowser.page_evaluate("""() => WAPI.getAllChats()""")
+        chats = await self.ThreadsafeBrowser.page_evaluate("""() => WAPI.getAllChats()""", page=self.page)
         if chats:
             return list(
                 filter(lambda x: x.get("isBroadcast") and x.get("id").get("_serialized") != 'status@broadcast', chats))
 
     async def getContact_(self, contactId):
         # @returns contact detial as promise
         contactId = self.valid_chatId(contactId)
-        return await self.ThreadsafeBrowser.page_evaluate("(contactId) => WAPI.getContact(contactId)", contactId)
+        return await self.ThreadsafeBrowser.page_evaluate("(contactId) => WAPI.getContact(contactId)", contactId, page=self.page)
 
     async def getAllContacts_(self):
         # @returns array of [Contact]
-        return await self.ThreadsafeBrowser.page_evaluate("() => WAPI.getAllContacts()")
+        return await self.ThreadsafeBrowser.page_evaluate("() => WAPI.getAllContacts()", page=self.page)
 
     async def getChatById_(self, contactId):
         contactId = self.valid_chatId(contactId)
-        return await self.ThreadsafeBrowser.page_evaluate("(contactId) => WAPI.getChatById(contactId)", contactId)
+        return await self.ThreadsafeBrowser.page_evaluate("(contactId) => WAPI.getChatById(contactId)", contactId, page=self.page)
 
     async def getChat_(self, contactId):
         contactId = self.valid_chatId(contactId)
         return self.getChatById(contactId)
 
     async def getProfilePicFromServer_(self, chatId):
         # @returns url of the chat picture or unasync defined if there is no picture for the chat.
         chatId = self.valid_chatId(chatId)
-        return await self.ThreadsafeBrowser.page_evaluate("(chatId) => WAPI._profilePicfunc(chatId)", chatId)
+        return await self.ThreadsafeBrowser.page_evaluate("(chatId) => WAPI._profilePicfunc(chatId)", chatId, page=self.page)
 
     async def loadEarlierMessages_(self, contactId):
         contactId = self.valid_chatId(contactId)
         return await self.ThreadsafeBrowser.page_evaluate("(contactId) => WAPI.loadEarlierMessages(contactId)",
-                                                          contactId)
+                                                          contactId, page=self.page)
 
     async def getStatus_(self, contactId):
         contactId = self.valid_chatId(contactId)
         return await self.ThreadsafeBrowser.page_evaluate("""async (contactId) => {
                                         const status = await WPP.contact.getStatus(contactId);
                                 
                                         return {
                                           id: contactId,
                                           status: (status as any)?.status || status,
                                         };
-                                      }""", contactId)
+                                      }""", contactId, page=self.page)
 
     async def getNumberProfile_(self, contactId):
         contactId = self.valid_chatId(contactId)
-        return await self.ThreadsafeBrowser.page_evaluate("(contactId) => WAPI.getNumberProfile(contactId)", contactId)
+        return await self.ThreadsafeBrowser.page_evaluate("(contactId) => WAPI.getNumberProfile(contactId)", contactId, page=self.page)
 
     async def getUnreadMessages_(self, includeMe, includeNotifications, useUnreadCount):
         return await self.ThreadsafeBrowser.page_evaluate(
             """({ includeMe, includeNotifications, useUnreadCount }) =>
         WAPI.getUnreadMessages(includeMe, includeNotifications, useUnreadCount)""",
-            {"includeMe": includeMe, "includeNotifications": includeNotifications, "useUnreadCount": useUnreadCount})
+            {"includeMe": includeMe, "includeNotifications": includeNotifications, "useUnreadCount": useUnreadCount}, page=self.page)
 
     async def getAllUnreadMessages_(self):
-        return await self.ThreadsafeBrowser.page_evaluate("() => WAPI.getAllUnreadMessages()")
+        return await self.ThreadsafeBrowser.page_evaluate("() => WAPI.getAllUnreadMessages()", page=self.page)
 
     async def getAllNewMessages_(self):
         # @deprecated Use getAllUnreadMessages
-        return await self.ThreadsafeBrowser.page_evaluate("() => WAPI.getAllNewMessages()")
+        return await self.ThreadsafeBrowser.page_evaluate("() => WAPI.getAllNewMessages()", page=self.page)
 
     async def getAllMessagesInChat_(self, chatId, includeMe=False, includeNotifications=False):
         chatId = self.valid_chatId(chatId)
         """
         * Retrieves all messages already loaded in a chat
         * For loading every message use loadAndGetAllMessagesInChat
         """
         return await self.ThreadsafeBrowser.page_evaluate("""({ chatId, includeMe, includeNotifications }) =>
         WAPI.getAllMessagesInChat(chatId, includeMe, includeNotifications)""",
                                                           {"chatId": chatId, "includeMe": includeMe,
-                                                           "includeNotifications": includeNotifications})
+                                                           "includeNotifications": includeNotifications}, page=self.page)
 
     async def loadAndGetAllMessagesInChat_(self, chatId, includeMe=False, includeNotifications=False):
         chatId = self.valid_chatId(chatId)
         """
         * Loads and Retrieves all Messages in a chat
         """
         return await self.ThreadsafeBrowser.page_evaluate("""({ chatId, includeMe, includeNotifications }) =>
         WAPI.loadAndGetAllMessagesInChat(chatId, includeMe, includeNotifications)""",
                                                           {"chatId": chatId, "includeMe": includeMe,
-                                                           "includeNotifications": includeNotifications})
+                                                           "includeNotifications": includeNotifications}, page=self.page)
 
     async def getChatIsOnline_(self, chatId):
         chatId = self.valid_chatId(chatId)
-        return await self.ThreadsafeBrowser.page_evaluate("(chatId) => WAPI.getChatIsOnline(chatId)", chatId)
+        return await self.ThreadsafeBrowser.page_evaluate("(chatId) => WAPI.getChatIsOnline(chatId)", chatId, page=self.page)
 
     async def getLastSeen_(self, chatId):
         chatId = self.valid_chatId(chatId)
-        return await self.ThreadsafeBrowser.page_evaluate("(chatId) => WAPI.getLastSeen(chatId)", chatId)
+        return await self.ThreadsafeBrowser.page_evaluate("(chatId) => WAPI.getLastSeen(chatId)", chatId, page=self.page)
 
     async def getPlatformFromMessage_(self, msgId):
         """
         * Get the platform message from message ID
         * The platform can be:
             * android
             * iphone
             * web
             * unknown
         """
-        return await self.ThreadsafeBrowser.page_evaluate("(msgId) => WPP.chat.getPlatformFromMessage(msgId)", msgId)
+        return await self.ThreadsafeBrowser.page_evaluate("(msgId) => WPP.chat.getPlatformFromMessage(msgId)", msgId, page=self.page)
 
     async def getReactions_(self, msgId):
-        return await self.ThreadsafeBrowser.page_evaluate("(msgId) => WPP.chat.getReactions(msgId)", msgId)
+        return await self.ThreadsafeBrowser.page_evaluate("(msgId) => WPP.chat.getReactions(msgId)", msgId, page=self.page)
 
     async def getVotes_(self, msgId):
-        return await self.ThreadsafeBrowser.page_evaluate("(msgId) => WPP.chat.getVotes(msgId)", msgId)
+        return await self.ThreadsafeBrowser.page_evaluate("(msgId) => WPP.chat.getVotes(msgId)", msgId, page=self.page)
```

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/SenderLayer.py` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/SenderLayer.py`

 * *Files 7% similar despite different names*

```diff
@@ -148,38 +148,38 @@
     ####################################################### async ######################################################
 
     async def sendLinkPreview_(self, chatId, url, text=''):
         message = text if url in text else f"{text}\n{url}"
         chatId = self.valid_chatId(chatId)
         result = await self.ThreadsafeBrowser.page_evaluate("""({ chatId, message }) => {
                     return WPP.chat.sendTextMessage(chatId, message, { linkPreview: true });
-                    }""", {"chatId": chatId, "message": message})
+                    }""", {"chatId": chatId, "message": message}, page=self.page)
         return result
 
     async def sendText_(self, to, content, options=None):
         if not options:
             options = {}
         to = self.valid_chatId(to)
         send_result = await self.ThreadsafeBrowser.page_evaluate("""({ to, content, options }) =>
                             WPP.chat.sendTextMessage(to, content, {
                               ...options,
                               waitForAck: true,
-                            })""", {"to": to, "content": content, "options": options})
+                            })""", {"to": to, "content": content, "options": options}, page=self.page)
         self.logger.debug(f'{self.session}: Send Message {send_result=}')
 
         return send_result
 
     async def sendMessageOptions_(self, chat, content, options=None):
         if not options:
             options = {}
         message_id = await self.ThreadsafeBrowser.page_evaluate("""({ chat, content, options }) => {
         return WAPI.sendMessageOptions(chat, content, options);
-      }""", {"chat": chat, "content": content, "options": options})
+      }""", {"chat": chat, "content": content, "options": options}, page=self.page)
         result = await self.ThreadsafeBrowser.page_evaluate("""(messageId) => WAPI.getMessageById(messageId)""",
-                                                            message_id)
+                                                            message_id, page=self.page)
         return result
 
     async def sendImage_(self, to, filePath, filename="", caption="", quotedMessageId=None, isViewOnce=None):
         to = self.valid_chatId(to)
         if filePath and os.path.exists(filePath):
             _base64 = self.convert_to_base64(filePath)
             filename = os.path.basename(filePath) if not filename else filename
@@ -216,31 +216,31 @@
         return {
           ack: result.ack,
           id: result.id,
           sendMsgResult: await result.sendMsgResult,
           error: result.message,
         };
       }""", {"to": to, "base64": _base64, "filename": filename, "caption": caption, "quotedMessageId": quotedMessageId,
-             "isViewOnce": isViewOnce})
+             "isViewOnce": isViewOnce}, page=self.page)
         return result
 
     async def reply_(self, to, content, quotedMsg):
         """
             @param to chat to: xxxxx@us.c
             @param content text message
             @param quotedMsg: @param quotedMsg Message id to reply to.
             @example
            // Simple message
            client.reply('<number>@c.us', 'A simple message', '<message-id>')
         """
         to = self.valid_chatId(to)
         result = await self.ThreadsafeBrowser.page_evaluate("""({ to, content, quotedMsg }) => {
                                     return WPP.chat.sendTextMessage(to, content, { quotedMsg });
-                                  }""", {"to": to, "content": content, "quotedMsg": quotedMsg})
-        # message = await self.ThreadsafeBrowser.page_evaluate()("(messageId) => WAPI.getMessageById(messageId)", result.get("id"))
+                                  }""", {"to": to, "content": content, "quotedMsg": quotedMsg}, page=self.page)
+        # message = await self.ThreadsafeBrowser.page_evaluate()("(messageId) => WAPI.getMessageById(messageId)", result.get("id"), page=self.page)
         return result
 
     async def sendFile_(self, to, pathOrBase64, nameOrOptions, caption):
         to = self.valid_chatId(to)
         options = {"type": 'auto-detect'}
         if type(nameOrOptions) is str:
             options["filename"] = nameOrOptions
@@ -264,15 +264,15 @@
         return await self.ThreadsafeBrowser.page_evaluate("""async ({ to, base64, options }) => {
         const result = await WPP.chat.sendFileMessage(to, base64, options);
         return {
           ack: result.ack,
           id: result.id,
           sendMsgResult: await result.sendMsgResult,
         };
-      }""", {"to": to, "base64": _base64, "options": options})
+      }""", {"to": to, "base64": _base64, "options": options}, page=self.page)
 
     async def sendVideoAsGif_(self, to: str, filePath: str, filename: str = "", caption: str = ""):
         """
           /**
            * Sends a video to given chat as a gif, with caption or not
            * @category Chat
            * @param to Chat id
@@ -322,14 +322,15 @@
                   ack: result.ack,
                   id: result.id,
                   sendMsgResult: await result.sendMsgResult,
                 };
               }
       """,
             {"to": to, "base64": base64, "filename": filename, "caption": caption, "quotedMessageId": quotedMessageId}
+            , page=self.page
         )
         return result
 
     async def sendGif_(self, to, filePath, filename="", caption=""):
         """
           /**
            * Sends a video to given chat as a gif, with caption or not, using base64
@@ -379,22 +380,22 @@
         """
         to = self.valid_chatId(to)
         return await self.ThreadsafeBrowser.page_evaluate("""({ to, contactsId, name }) => {
         return WPP.chat.sendVCardContactMessage(to, {
           id: contactsId,
           name: name,
         });
-      }""", {"to": to, "contactsId": contactsId, "name": name})
+      }""", {"to": to, "contactsId": contactsId, "name": name}, page=self.page)
 
     async def forwardMessages_(self, to, messages, skipMyMessages):
         to = self.valid_chatId(to)
         return await self.ThreadsafeBrowser.page_evaluate("""({ to, messages, skipMyMessages }) =>
         WAPI.forwardMessages(to, messages, skipMyMessages)""",
                                                           {"to": to, "messages": messages,
-                                                           "skipMyMessages": skipMyMessages})
+                                                           "skipMyMessages": skipMyMessages}, page=self.page)
 
     async def sendLocation_(self, to, options):
         to = self.valid_chatId(to)
         options = {
             "lat": options.get("latitude"),
             "lng": options.get("longitude"),
             "title": options.get("title"),
@@ -403,32 +404,32 @@
         const result = await WPP.chat.sendLocationMessage(to, options);
 
         return {
           ack: result.ack,
           id: result.id,
           sendMsgResult: await result.sendMsgResult,
         };
-      }""", {"to": to, "options": options})
+      }""", {"to": to, "options": options}, page=self.page)
 
     async def sendSeen_(self, chatId):
         chatId = self.valid_chatId(chatId)
-        return await self.ThreadsafeBrowser.page_evaluate("(chatId) => WPP.chat.markIsRead(chatId)", chatId)
+        return await self.ThreadsafeBrowser.page_evaluate("(chatId) => WPP.chat.markIsRead(chatId)", chatId, page=self.page)
 
     async def startTyping_(self, to, duration=None):
         to = self.valid_chatId(to)
         return await self.ThreadsafeBrowser.page_evaluate(
             "({ to, duration }) => WPP.chat.markIsComposing(to, duration)",
-            {"to": to, "duration": duration})
+            {"to": to, "duration": duration}, page=self.page)
 
     async def stopTyping_(self, to):
         to = self.valid_chatId(to)
-        return await self.ThreadsafeBrowser.page_evaluate("(to) => WPP.chat.markIsPaused(to)", to)
+        return await self.ThreadsafeBrowser.page_evaluate("(to) => WPP.chat.markIsPaused(to)", to, page=self.page)
 
     async def setOnlinePresence_(self, online=True):
-        return await self.ThreadsafeBrowser.page_evaluate("(online) => WPP.conn.markAvailable(online)", online)
+        return await self.ThreadsafeBrowser.page_evaluate("(online) => WPP.conn.markAvailable(online)", online, page=self.page)
 
     async def sendListMessage_(self, to, options):
         to = self.valid_chatId(to)
         """
           /**
            * Sends a list message
            *
@@ -458,15 +459,15 @@
            * ```
            *
            * @category Chat
            */
         """
         sendResult = await self.ThreadsafeBrowser.page_evaluate(
             "({ to, options }) => WPP.chat.sendListMessage(to, options)",
-            {"to": to, "options": options})
+            {"to": to, "options": options}, page=self.page)
         # result = await self.ThreadsafeBrowser.page_evaluate("""async ({ messageId }) => {
         #                 return JSON.parse(JSON.stringify(await WAPI.getMessageById(messageId)));
         #               }""", sendResult.get("id"))
         return sendResult
 
     async def setChatState_(self, chatId, chatState):
         """
@@ -478,8 +479,8 @@
            * @param chatId
            * @deprecated Deprecated in favor of Use startTyping or startRecording functions
            */
         """
         chatId = self.valid_chatId(chatId)
         return await self.ThreadsafeBrowser.page_evaluate("""({ chatState, chatId }) => {
                 WAPI.sendChatstate(chatState, chatId);
-              }""", {"chatState": chatState, "chatId": chatId})
+              }""", {"chatState": chatState, "chatId": chatId}, page=self.page)
```

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/StatusLayer.py` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/StatusLayer.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         if not mime_info or 'image' not in mime_info:
             error = ValueError('Not an image, allowed formats png, jpeg and webp')
             error.code = 'invalid_image'
             raise error
 
         return await self.ThreadsafeBrowser.page_evaluate(
             """({base64}) => WPP.status.sendImageStatus(base64);""",
-            {"base64": base64}
+            {"base64": base64}, page=self.page
         )
 
     async def sendVideoStatus_(self, pathOrBase64: str):
         """
           /**
            * Send a video message to status stories
            * @category Status
@@ -138,15 +138,15 @@
         if not base64:
             error = ValueError('Empty or invalid file or base64')
             error.code = 'empty_file'
             raise error
 
         return await self.ThreadsafeBrowser.page_evaluate(
             """({base64}) => WPP.status.sendVideoStatus(base64);""",
-            {"base64": base64}
+            {"base64": base64}, page=self.page
         )
 
     async def sendTextStatus_(self, text: str, options: str):
         """
           /**
            * Send a text to status stories
            * @category Status
@@ -156,15 +156,15 @@
            * client.sendTextStatus(`Bootstrap primary color: #0275d8`, { backgroundColor: '#0275d8', font: 2});
            * ```
            * @param pathOrBase64 Path or base 64 image
            */
         """
         return await self.ThreadsafeBrowser.page_evaluate(
             """({text, options}) => WPP.status.sendTextStatus(text, options);""",
-            {"text": text, "options": options}
+            {"text": text, "options": options}, page=self.page
         )
 
     async def sendReadStatus_(self, chatId: str, statusId: str):
         """/**
            * Mark status as read/seen
            * @category Status
            *
@@ -173,9 +173,9 @@
            * client.sendReadStatus('[phone_number]@c.us', 'false_status@broadcast_3A169E0FD4BC6E92212F_[]@c.us');
            * ```
            * @param chatId Chat ID of contact
            * @param statusId ID of status msg
            */"""
         return await self.ThreadsafeBrowser.page_evaluate(
             """({ chatId, statusId }) => WPP.status.sendReadStatus(chatId, statusId);""",
-            {"chatId": chatId, "statusId": statusId}
+            {"chatId": chatId, "statusId": statusId}, page=self.page
         )
```

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/layers/UILayer.py` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/UILayer.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,27 +33,27 @@
         """
         Opens given chat at last message (bottom)
         Will fire natural workflow events of whatsapp web
         @category UI
         @param chatId
         """
         chatId = self.valid_chatId(chatId)
-        return await self.ThreadsafeBrowser.page_evaluate("(chatId) => WPP.chat.openChatBottom(chatId)", chatId)
+        return await self.ThreadsafeBrowser.page_evaluate("(chatId) => WPP.chat.openChatBottom(chatId)", chatId, page=self.page)
 
     async def openChatAt_(self, chatId, messageId):
         """
         Opens chat at given message position
         @category UI
         @param chatId Chat id
         @param messageId Message id (For example: '06D3AB3D0EEB9D077A3F9A3EFF4DD030')
         """
         chatId = self.valid_chatId(chatId)
         return await self.ThreadsafeBrowser.page_evaluate(
             "({chatId, messageId}) => WPP.chat.openChatAt(chatId, messageId)",
-            {"chatId": chatId, "messageId": messageId})
+            {"chatId": chatId, "messageId": messageId}, page=self.page)
 
     async def getActiveChat_(self):
         """
         Return the current active chat
         @category UI
         """
-        return await self.ThreadsafeBrowser.page_evaluate("() => WPP.chat.getActiveChat()")
+        return await self.ThreadsafeBrowser.page_evaluate("() => WPP.chat.getActiveChat()", page=self.page)
```

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp/api/model/status_find.py` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/model/status_find.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp/controllers/browser.py` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/controllers/browser.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp/controllers/initializer.py` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/controllers/initializer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import os
 import types
 from typing import Optional
 from WPP_Whatsapp.controllers.browser import SUPPORTED_BROWSERS
 from WPP_Whatsapp.controllers.browser import ThreadsafeBrowser
 from WPP_Whatsapp.api.Whatsapp import Whatsapp
-from WPP_Whatsapp.api.const import Logger
+from WPP_Whatsapp.api.const import Logger, useragentOverride
 
 
 class Create:
     client: Optional[Whatsapp]
     ThreadsafeBrowser: "ThreadsafeBrowser"
 
     def __init__(
@@ -74,16 +74,17 @@
     def sync_close(self):
         if hasattr(self, "ThreadsafeBrowser"):
             self.ThreadsafeBrowser.sync_close()
         self._onStateChange("CLOSED")
 
     def _onStateChange(self, state):
         self.state = state
-        if hasattr(self, "ThreadsafeBrowser") and not self.ThreadsafeBrowser.page.is_closed():
-            connected = self.ThreadsafeBrowser.page_evaluate_sync("() => WPP.conn.isRegistered()")
+        if hasattr(self, "ThreadsafeBrowser") and not self.client.page.is_closed():
+            # TODO::
+            connected = self.ThreadsafeBrowser.page_evaluate_sync("() => WPP.conn.isRegistered()", page=self.client.page)
             if not connected:
                 self.ThreadsafeBrowser.sleep(2)
                 if not self.waitLoginPromise:
                     try:
                         self.waitLoginPromise = self.client.waitForLogin
                     except:
                         Logger.exception("waitForLogin")
@@ -140,34 +141,38 @@
 
         return self.client
 
     def create_sync(self) -> Whatsapp:
         self.state = "STARTING"
         default = {
             "no_viewport": True, "bypass_csp": True, "headless": False,
-            "browser": "chromium", "install": True,
+            "browser": "chromium", "install": True, "user_agent": useragentOverride
         }
-
-        for key in default:
-            if key not in self.__kwargs:
-                self.__kwargs[key] = default[key]
+        default.update(self.__kwargs)
+        self.__kwargs = default
+        # for key in default:
+        #     if key not in self.__kwargs:
+        #         self.__kwargs[key] = default[key]
 
         # Use Default channel as chrome
         if self.__kwargs.get("browser") == "chrome" or self.__kwargs.get("browser") not in SUPPORTED_BROWSERS:
             self.__kwargs["browser"] = "chromium"
             self.__kwargs["channel"] = "chrome"
 
         self.ThreadsafeBrowser = ThreadsafeBrowser(user_data_dir=self.user_data_dir, **self.__kwargs)
 
         self.ThreadsafeBrowser.page.on("close", self.close)
         self.ThreadsafeBrowser.page.on("crash", self.close)
         self.ThreadsafeBrowser.browser.on("disconnected", lambda: self.statusFind('browserClose', self.session))
 
-        self.client = Whatsapp(self.session, self.ThreadsafeBrowser, logQR=self.logQR,
+        self.client = Whatsapp(self.session,
+                               threadsafe_browser=self.ThreadsafeBrowser, page=self.ThreadsafeBrowser.page,
+                               loop=self.loop, logQR=self.logQR,
                                autoClose=self.autoClose, version=self.version, wa_js_version=self.wa_js_version)
+
         self.client.catchQR = self.catchQR
         self.client.statusFind = self.statusFind
         self.client.onLoadingScreen = self.onLoadingScreen
         self.ThreadsafeBrowser.run_threadsafe(self.client.start, timeout_=120)
         self.client.onStateChange(self._onStateChange)
         if self.waitForLogin:
             is_logged = self.client.waitForLogin()
@@ -196,16 +201,18 @@
 
         self.ThreadsafeBrowser = ThreadsafeBrowser(user_data_dir=self.user_data_dir, **self.__kwargs)
 
         self.ThreadsafeBrowser.page.on("close", self.close)
         self.ThreadsafeBrowser.page.on("crash", self.close)
         self.ThreadsafeBrowser.browser.on("disconnected", lambda: self.statusFind('browserClose', self.session))
 
-        self.client = Whatsapp(self.session, self.ThreadsafeBrowser, logQR=self.logQR,
-                               autoClose=self.autoClose, version=self.version)
+        self.client = Whatsapp(self.session,
+                               threadsafe_browser=self.ThreadsafeBrowser, page=self.ThreadsafeBrowser.page,
+                               loop=self.ThreadsafeBrowser.loop, logQR=self.logQR,
+                               autoClose=self.autoClose, version=self.version, wa_js_version=self.wa_js_version)
         self.client.catchQR = self.catchQR
         self.client.statusFind = self.statusFind
         self.client.onLoadingScreen = self.onLoadingScreen
         await self.client.start()
         # self.ThreadsafeBrowser.run_threadsafe(self.client.start, timeout_=120)
         self.client.onStateChange(self._onStateChange)
         if self.waitForLogin:
```

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp/js_lib/wapi.js` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/js_lib/wapi.js`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp/utils/ffmpeg.py` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp.egg-info/PKG-INFO` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: WPP_Whatsapp
-Version: 0.2.2
+Version: 0.2.2.2
 Summary: WPP_Whatsapp aim of exporting functions from WhatsApp Web to the python, which can be used to support the creation of any interaction, such as customer service, media sending, intelligence recognition based on phrases artificial and many other things, use your imagination
 Home-page: https://github.com/3mora2/WPP_Whatsapp
 Author: Ammar Alkotb
 Author-email: ammar.alkotb@gmail.com
 License: MIT License
 Project-URL: Bug Report, https://github.com/3mora2/WPP_Whatsapp/issues/new
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: event-emitter-js
 Requires-Dist: greenlet
-Requires-Dist: playwright
+Requires-Dist: playwright>=1.43.0
 Requires-Dist: Pillow
 Requires-Dist: psutil
 Requires-Dist: pyee
 Requires-Dist: segno
 Requires-Dist: typing_extensions
 Requires-Dist: playwright-stealth
 Requires-Dist: node-semver
 Requires-Dist: aiohttp
-Requires-Dist: PlaywrightSafeThread>=0.5.2.1
+Requires-Dist: PlaywrightSafeThread>=0.5.4.1
 
 # WPP_Whatsapp
 <p align="center">
   <a href="https://pypi.org/project/WPP-Whatsapp"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/WPP_Whatsapp.svg?maxAge=86400" /></a>
   <a href="https://pypi.org/project/WPP-Whatsapp"><img alt="View" src="https://static.pepy.tech/personalized-badge/WPP_Whatsapp?period=total&units=international_system&left_text=Downloads"/></a>
 </p>
```

### Comparing `WPP_Whatsapp-0.2.2/WPP_Whatsapp.egg-info/SOURCES.txt` & `wpp_whatsapp-0.2.2.2/WPP_Whatsapp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 ./WPP_Whatsapp/api/layers/UILayer.py
 ./WPP_Whatsapp/api/layers/__init__.py
 ./WPP_Whatsapp/api/model/__init__.py
 ./WPP_Whatsapp/api/model/status_find.py
 ./WPP_Whatsapp/controllers/__init__.py
 ./WPP_Whatsapp/controllers/auth.py
 ./WPP_Whatsapp/controllers/browser.py
+./WPP_Whatsapp/controllers/init_multi.py
 ./WPP_Whatsapp/controllers/initializer.py
 ./WPP_Whatsapp/js_lib/wapi.js
 ./WPP_Whatsapp/utils/__init__.py
 ./WPP_Whatsapp/utils/ffmpeg.py
 WPP_Whatsapp.egg-info/PKG-INFO
 WPP_Whatsapp.egg-info/SOURCES.txt
 WPP_Whatsapp.egg-info/dependency_links.txt
```

### Comparing `WPP_Whatsapp-0.2.2/setup.py` & `wpp_whatsapp-0.2.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,39 +2,39 @@
 from setuptools import setup
 
 long_description = open("README.md", encoding="utf-8").read()
 description = ("WPP_Whatsapp aim of exporting functions from WhatsApp Web to the python, which can be used to support "
                "the creation of any interaction, such as customer service, media sending, intelligence recognition "
                "based on phrases artificial and many other things, use your imagination")
 
-version = "0.2.2"
+version = "0.2.2.2"
 
 setup(
     name="WPP_Whatsapp",
     version=version,
     license="MIT License",
     author="Ammar Alkotb",
     author_email="ammar.alkotb@gmail.com",
     description=description,
     packages=find_packages(),
     url="https://github.com/3mora2/WPP_Whatsapp",
     project_urls={"Bug Report": "https://github.com/3mora2/WPP_Whatsapp/issues/new"},
     install_requires=[
         "event-emitter-js",
         "greenlet",
-        "playwright",
+        "playwright>=1.43.0",
         "Pillow",
         "psutil",
         "pyee",
         'segno',
         'typing_extensions',
         "playwright-stealth",
         "node-semver",
         "aiohttp",
-        "PlaywrightSafeThread>=0.5.2.1"
+        "PlaywrightSafeThread>=0.5.4.1"
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir={"": "."},
     package_data={"WPP_Whatsapp": ["*/*.js", "*.md"]},
     classifiers=[
         "License :: OSI Approved :: MIT License",
```

### Comparing `WPP_Whatsapp-0.2.2/test/test_hiden.py` & `wpp_whatsapp-0.2.2.2/test/test_hiden.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.2.2/test/test_setinterval.py` & `wpp_whatsapp-0.2.2.2/test/test_setinterval.py`

 * *Files identical despite different names*

