# Comparing `tmp/oresat_dxwifi-0.3.5.tar.gz` & `tmp/oresat_dxwifi-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat_dxwifi-0.3.5.tar", last modified: Mon Apr 22 05:05:21 2024, max compression
+gzip compressed data, was "oresat_dxwifi-0.3.6.tar", last modified: Sat Apr 27 04:04:18 2024, max compression
```

## Comparing `oresat_dxwifi-0.3.5.tar` & `oresat_dxwifi-0.3.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:05:21.528456 oresat_dxwifi-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:05:21.512456 oresat_dxwifi-0.3.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:05:21.516456 oresat_dxwifi-0.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-04-22 05:05:21.524456 oresat_dxwifi-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2384 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/build-deb.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:05:21.512456 oresat_dxwifi-0.3.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:05:21.516456 oresat_dxwifi-0.3.5/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   100917 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/docs/images/hgs-browser.png
--rw-r--r--   0 runner    (1001) docker     (127)    90640 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/docs/images/olaf-browser.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      176 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/kill-olaf
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/oresat-dxwifi-software-server.service
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/oresat-mon-iface.service
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/oresat-vcan-iface.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:05:21.516456 oresat_dxwifi-0.3.5/oresat_dxwifi/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/oresat_dxwifi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/oresat_dxwifi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-22 05:05:21.000000 oresat_dxwifi-0.3.5/oresat_dxwifi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:05:21.520456 oresat_dxwifi-0.3.5/oresat_dxwifi/camera/
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/oresat_dxwifi/camera/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/oresat_dxwifi/camera/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/oresat_dxwifi/camera/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/oresat_dxwifi/camera/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:05:21.520456 oresat_dxwifi-0.3.5/oresat_dxwifi/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/oresat_dxwifi/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/oresat_dxwifi/resources/temperature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:05:21.520456 oresat_dxwifi-0.3.5/oresat_dxwifi/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:05:21.520456 oresat_dxwifi-0.3.5/oresat_dxwifi/services/configs/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/oresat_dxwifi/services/configs/camera_configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7565 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/oresat_dxwifi/services/oresat_live.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:05:21.520456 oresat_dxwifi-0.3.5/oresat_dxwifi/services/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/oresat_dxwifi/services/static/SMPTE_Color_Bars.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:05:21.520456 oresat_dxwifi-0.3.5/oresat_dxwifi/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/oresat_dxwifi/templates/oresat_live.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:05:21.520456 oresat_dxwifi-0.3.5/oresat_dxwifi/transmission/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/oresat_dxwifi/transmission/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:05:21.524456 oresat_dxwifi-0.3.5/oresat_dxwifi/transmission/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/oresat_dxwifi/transmission/configs/transmission_configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/oresat_dxwifi/transmission/defaults.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      661 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/oresat_dxwifi/transmission/startmonitor.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/oresat_dxwifi/transmission/transmission.py
--rw-r--r--   0 runner    (1001) docker     (127)  4381644 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/oresat_dxwifi/transmission/tx_module.so
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:05:21.524456 oresat_dxwifi-0.3.5/oresat_dxwifi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-04-22 05:05:21.000000 oresat_dxwifi-0.3.5/oresat_dxwifi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-22 05:05:21.000000 oresat_dxwifi-0.3.5/oresat_dxwifi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 05:05:21.000000 oresat_dxwifi-0.3.5/oresat_dxwifi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 05:05:21.000000 oresat_dxwifi-0.3.5/oresat_dxwifi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-22 05:05:21.000000 oresat_dxwifi-0.3.5/oresat_dxwifi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-22 05:05:21.000000 oresat_dxwifi-0.3.5/oresat_dxwifi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 05:05:21.528456 oresat_dxwifi-0.3.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      336 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/start-vcan
--rwxr-xr-x   0 runner    (1001) docker     (127)      660 2024-04-22 05:05:17.000000 oresat_dxwifi-0.3.5/startmonitor.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:04:18.992970 oresat_dxwifi-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:04:18.980970 oresat_dxwifi-0.3.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:04:18.984969 oresat_dxwifi-0.3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-04-27 04:04:18.992970 oresat_dxwifi-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2384 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/build-deb.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:04:18.980970 oresat_dxwifi-0.3.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:04:18.984969 oresat_dxwifi-0.3.6/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   100917 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/docs/images/hgs-browser.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90640 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/docs/images/olaf-browser.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      176 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/kill-olaf
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/oresat-dxwifi-software-server.service
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/oresat-mon-iface.service
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/oresat-vcan-iface.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:04:18.984969 oresat_dxwifi-0.3.6/oresat_dxwifi/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/oresat_dxwifi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/oresat_dxwifi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-27 04:04:18.000000 oresat_dxwifi-0.3.6/oresat_dxwifi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:04:18.984969 oresat_dxwifi-0.3.6/oresat_dxwifi/camera/
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/oresat_dxwifi/camera/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/oresat_dxwifi/camera/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/oresat_dxwifi/camera/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/oresat_dxwifi/camera/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:04:18.984969 oresat_dxwifi-0.3.6/oresat_dxwifi/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/oresat_dxwifi/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/oresat_dxwifi/resources/temperature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:04:18.984969 oresat_dxwifi-0.3.6/oresat_dxwifi/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:04:18.984969 oresat_dxwifi-0.3.6/oresat_dxwifi/services/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/oresat_dxwifi/services/configs/camera_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/oresat_dxwifi/services/oresat_live.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:04:18.988969 oresat_dxwifi-0.3.6/oresat_dxwifi/services/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/oresat_dxwifi/services/static/SMPTE_Color_Bars.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:04:18.988969 oresat_dxwifi-0.3.6/oresat_dxwifi/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/oresat_dxwifi/templates/oresat_live.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:04:18.988969 oresat_dxwifi-0.3.6/oresat_dxwifi/transmission/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/oresat_dxwifi/transmission/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:04:18.992970 oresat_dxwifi-0.3.6/oresat_dxwifi/transmission/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/oresat_dxwifi/transmission/configs/transmission_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/oresat_dxwifi/transmission/defaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      661 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/oresat_dxwifi/transmission/startmonitor.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/oresat_dxwifi/transmission/transmission.py
+-rw-r--r--   0 runner    (1001) docker     (127)  4381644 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/oresat_dxwifi/transmission/tx_module.so
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 04:04:18.992970 oresat_dxwifi-0.3.6/oresat_dxwifi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-04-27 04:04:18.000000 oresat_dxwifi-0.3.6/oresat_dxwifi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-27 04:04:18.000000 oresat_dxwifi-0.3.6/oresat_dxwifi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 04:04:18.000000 oresat_dxwifi-0.3.6/oresat_dxwifi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-27 04:04:18.000000 oresat_dxwifi-0.3.6/oresat_dxwifi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-27 04:04:18.000000 oresat_dxwifi-0.3.6/oresat_dxwifi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-27 04:04:18.000000 oresat_dxwifi-0.3.6/oresat_dxwifi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 04:04:18.992970 oresat_dxwifi-0.3.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      336 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/start-vcan
+-rwxr-xr-x   0 runner    (1001) docker     (127)      660 2024-04-27 04:04:14.000000 oresat_dxwifi-0.3.6/startmonitor.sh
```

### Comparing `oresat_dxwifi-0.3.5/.github/workflows/pypi.yaml` & `oresat_dxwifi-0.3.6/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.5/.gitignore` & `oresat_dxwifi-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.5/LICENSE` & `oresat_dxwifi-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.5/PKG-INFO` & `oresat_dxwifi-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-dxwifi
-Version: 0.3.5
+Version: 0.3.6
 Summary: OreSat DxWiFi OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `oresat_dxwifi-0.3.5/README.md` & `oresat_dxwifi-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.5/build-deb.sh` & `oresat_dxwifi-0.3.6/build-deb.sh`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.5/docs/images/hgs-browser.png` & `oresat_dxwifi-0.3.6/docs/images/hgs-browser.png`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.5/docs/images/olaf-browser.png` & `oresat_dxwifi-0.3.6/docs/images/olaf-browser.png`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.5/oresat_dxwifi/__main__.py` & `oresat_dxwifi-0.3.6/oresat_dxwifi/__main__.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.5/oresat_dxwifi/camera/CMakeLists.txt` & `oresat_dxwifi-0.3.6/oresat_dxwifi/camera/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.5/oresat_dxwifi/camera/README.md` & `oresat_dxwifi-0.3.6/oresat_dxwifi/camera/README.md`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.5/oresat_dxwifi/camera/frame.py` & `oresat_dxwifi-0.3.6/oresat_dxwifi/camera/frame.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.5/oresat_dxwifi/camera/interface.py` & `oresat_dxwifi-0.3.6/oresat_dxwifi/camera/interface.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.5/oresat_dxwifi/resources/temperature.py` & `oresat_dxwifi-0.3.6/oresat_dxwifi/resources/temperature.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.5/oresat_dxwifi/services/oresat_live.py` & `oresat_dxwifi-0.3.6/oresat_dxwifi/services/oresat_live.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,17 +45,14 @@
     """Service for capturing and transmitting video"""
 
     def __init__(self):
         """Initializes camera interface and sets state"""
         super().__init__()
         self.state = State.BOOT
 
-        # start mon0
-        self.start_monitor()
-
         self.firmware_folder = "/lib/firmware/ath9k_htc"
         self.firmware_file = os.path.join(self.firmware_folder, "htc_9271-1.dev.0.fw")
         
         self.IMAGE_OUPUT_DIRECTORY = "/oresat-live-output/frames"
 
         if not os.path.isdir(self.IMAGE_OUPUT_DIRECTORY):
             os.mkdir(self.IMAGE_OUPUT_DIRECTORY)
@@ -64,14 +61,22 @@
 
         self.camera = CameraInterface(
             configs["width"],
             configs["height"],
             self.IMAGE_OUPUT_DIRECTORY,
         )
 
+    def monitor_is_valid(self):
+        monitor_path = "/sys/class/net/mon0"
+        if os.path.isdir(monitor_path):
+            with open(os.path.join(monitor_path, "type")) as f:
+                if f.read() != "1":
+                    return True
+        return False
+
     def start_monitor(self):
         cur_dir = os.path.dirname(os.path.abspath(__file__))
         subprocess.call([f"{cur_dir}/../transmission/startmonitor.sh"])
 
     def load_configs(self):
         """Loads the camera configs from the YAML file"""
         dirname = os.path.dirname(os.path.abspath(__file__))
@@ -165,14 +170,17 @@
         self.transmit_file(os.path.join(cur_dir, "static/SMPTE_Color_Bars.gif"))
         self.state = State.STANDBY
 
     def transmit(self) -> None:
         """Transmits all the images in the image output directory."""
         self.state = State.TRANSMISSION
 
+        if not self.monitor_is_valid():
+            self.start_monitor()
+
         files = os.listdir(self.IMAGE_OUPUT_DIRECTORY)
 
         for f in files:
             f = os.path.join(self.IMAGE_OUPUT_DIRECTORY, f)
             self.transmit_file(f)
 
         self.state = State.STANDBY
```

### Comparing `oresat_dxwifi-0.3.5/oresat_dxwifi/services/static/SMPTE_Color_Bars.gif` & `oresat_dxwifi-0.3.6/oresat_dxwifi/services/static/SMPTE_Color_Bars.gif`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.5/oresat_dxwifi/templates/oresat_live.html` & `oresat_dxwifi-0.3.6/oresat_dxwifi/templates/oresat_live.html`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.5/oresat_dxwifi/transmission/configs/transmission_configs.yaml` & `oresat_dxwifi-0.3.6/oresat_dxwifi/transmission/configs/transmission_configs.yaml`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.5/oresat_dxwifi/transmission/defaults.py` & `oresat_dxwifi-0.3.6/oresat_dxwifi/transmission/defaults.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.5/oresat_dxwifi/transmission/startmonitor.sh` & `oresat_dxwifi-0.3.6/oresat_dxwifi/transmission/startmonitor.sh`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.5/oresat_dxwifi/transmission/transmission.py` & `oresat_dxwifi-0.3.6/oresat_dxwifi/transmission/transmission.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.5/oresat_dxwifi/transmission/tx_module.so` & `oresat_dxwifi-0.3.6/oresat_dxwifi/transmission/tx_module.so`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.5/oresat_dxwifi.egg-info/PKG-INFO` & `oresat_dxwifi-0.3.6/oresat_dxwifi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-dxwifi
-Version: 0.3.5
+Version: 0.3.6
 Summary: OreSat DxWiFi OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `oresat_dxwifi-0.3.5/oresat_dxwifi.egg-info/SOURCES.txt` & `oresat_dxwifi-0.3.6/oresat_dxwifi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.5/pyproject.toml` & `oresat_dxwifi-0.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.5/startmonitor.sh` & `oresat_dxwifi-0.3.6/startmonitor.sh`

 * *Files identical despite different names*

