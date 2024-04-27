# Comparing `tmp/gameserverlister-1.1.2.tar.gz` & `tmp/gameserverlister-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameserverlister-1.1.2.tar", last modified: Wed Apr 24 10:54:23 2024, max compression
+gzip compressed data, was "gameserverlister-2.0.0.tar", last modified: Sat Apr 27 20:22:51 2024, max compression
```

## Comparing `gameserverlister-1.1.2.tar` & `gameserverlister-2.0.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:54:23.076534 gameserverlister-1.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:54:23.064535 gameserverlister-1.1.2/GameserverLister/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:54:23.068534 gameserverlister-1.1.2/GameserverLister/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/commands/battlelog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/commands/bfbc2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/commands/gamespy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/commands/gametools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/commands/medalofhonor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:54:23.068534 gameserverlister-1.1.2/GameserverLister/commands/options/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/commands/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/commands/options/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/commands/options/gameport.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/commands/options/http.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/commands/options/queryport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/commands/quake3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/commands/unreal2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/commands/valve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:54:23.072534 gameserverlister-1.1.2/GameserverLister/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/common/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/common/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    16878 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/common/servers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/common/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/common/weblinks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:54:23.072534 gameserverlister-1.1.2/GameserverLister/games/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/games/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/games/battlelog.py
--rw-r--r--   0 runner    (1001) docker     (127)     9937 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/games/gamespy.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/games/gametools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8787 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/games/quake3.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/games/unreal2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/games/valve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:54:23.072534 gameserverlister-1.1.2/GameserverLister/listers/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/listers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/listers/battlelog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/listers/bfbc2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13346 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/listers/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/listers/gamespy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/listers/gametools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/listers/medalofhonor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/listers/quake3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/listers/unreal2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/GameserverLister/listers/valve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:54:23.072534 gameserverlister-1.1.2/GameserverLister.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18226 2024-04-24 10:54:23.000000 gameserverlister-1.1.2/GameserverLister.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-24 10:54:23.000000 gameserverlister-1.1.2/GameserverLister.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:54:23.000000 gameserverlister-1.1.2/GameserverLister.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-24 10:54:23.000000 gameserverlister-1.1.2/GameserverLister.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-24 10:54:23.000000 gameserverlister-1.1.2/GameserverLister.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 10:54:23.000000 gameserverlister-1.1.2/GameserverLister.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    18226 2024-04-24 10:54:23.072534 gameserverlister-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16768 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-24 10:54:23.076534 gameserverlister-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 10:54:19.000000 gameserverlister-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:22:51.433256 gameserverlister-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:22:51.425255 gameserverlister-2.0.0/GameserverLister/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:22:51.429256 gameserverlister-2.0.0/GameserverLister/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/commands/battlelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/commands/bfbc2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/commands/gamespy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/commands/gametools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/commands/medalofhonor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:22:51.429256 gameserverlister-2.0.0/GameserverLister/commands/options/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/commands/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/commands/options/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/commands/options/gameport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/commands/options/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/commands/options/queryport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/commands/quake3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/commands/unreal2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/commands/valve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:22:51.433256 gameserverlister-2.0.0/GameserverLister/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/common/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/common/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16878 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/common/servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/common/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/common/weblinks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:22:51.433256 gameserverlister-2.0.0/GameserverLister/games/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/games/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/games/battlelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9937 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/games/gamespy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/games/gametools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9056 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/games/quake3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/games/unreal2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/games/valve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:22:51.433256 gameserverlister-2.0.0/GameserverLister/listers/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/listers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/listers/battlelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/listers/bfbc2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/listers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10755 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/listers/gamespy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/listers/gametools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/listers/medalofhonor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/listers/quake3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/listers/unreal2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/GameserverLister/listers/valve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:22:51.433256 gameserverlister-2.0.0/GameserverLister.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20676 2024-04-27 20:22:51.000000 gameserverlister-2.0.0/GameserverLister.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-27 20:22:51.000000 gameserverlister-2.0.0/GameserverLister.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 20:22:51.000000 gameserverlister-2.0.0/GameserverLister.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-27 20:22:51.000000 gameserverlister-2.0.0/GameserverLister.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-27 20:22:51.000000 gameserverlister-2.0.0/GameserverLister.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-27 20:22:51.000000 gameserverlister-2.0.0/GameserverLister.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    20676 2024-04-27 20:22:51.433256 gameserverlister-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19211 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-27 20:22:51.437255 gameserverlister-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 20:22:48.000000 gameserverlister-2.0.0/setup.py
```

### Comparing `gameserverlister-1.1.2/GameserverLister/__main__.py` & `gameserverlister-2.0.0/GameserverLister/__main__.py`

 * *Files identical despite different names*

### Comparing `gameserverlister-1.1.2/GameserverLister/commands/battlelog.py` & `gameserverlister-2.0.0/GameserverLister/commands/gamespy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,124 @@
 import logging
 import sys
-from typing import Optional
 
 import click
 
-from GameserverLister.commands.options import common, http, queryport
+from GameserverLister.commands.options import common, gameport
 from GameserverLister.common.logger import logger
-from GameserverLister.common.types import BattlelogGame
-from GameserverLister.listers import BattlelogServerLister
+from GameserverLister.common.types import GamespyGame, GamespyPrincipal
+from GameserverLister.games.gamespy import GAMESPY_GAME_CONFIGS
+from GameserverLister.listers import GameSpyServerLister
 
 
 @click.command
 @click.option(
     '-g',
     '--game',
-    type=click.Choice(BattlelogGame),
+    type=click.Choice(GamespyGame),
     required=True,
     help='Game to list servers for'
 )
-@http.page_limit
-@http.sleep
-@http.max_attempts
-@http.proxy
-@queryport.find
-@queryport.gamedig_bin
-@queryport.gamedig_concurrency
+@click.option(
+    '-p',
+    '--principal',
+    type=click.Choice(GamespyPrincipal),
+    required=True,
+    help='Principal server to query'
+)
+@click.option(
+    '-b',
+    '--gslist',
+    'gslist_path',
+    type=str,
+    required=True,
+    help='Path to gslist binary'
+)
+@click.option(
+    '-f',
+    '--filter',
+    'gslist_filter',
+    type=str,
+    default='',
+    help='Filter to apply to server list'
+)
+@click.option(
+    '-s',
+    '--super-query',
+    'gslist_super_query',
+    default=False,
+    is_flag=True,
+    help='Query each server in the list for it\'s status'
+)
+@click.option(
+    '-t',
+    '--timeout',
+    'gslist_timeout',
+    type=int,
+    default=10,
+    help='Timeout to use for gslist command'
+)
+@click.option(
+    '-v',
+    '--verify',
+    default=False,
+    is_flag=True,
+    help='(Attempt to) verify game servers returned by principal are game servers for the current game'
+)
+@gameport.add
 @common.expired_ttl
 @common.list_dir
 @common.recover
 @common.add_links
 @common.txt
 @common.debug
 def run(
-        game: BattlelogGame,
-        page_limit: int,
-        sleep: float,
-        max_attempts: int,
-        proxy: Optional[str],
-        find_query_port: bool,
-        gamedig_bin: str,
-        gamedig_concurrency: int,
+        game: GamespyGame,
+        principal: GamespyPrincipal,
+        gslist_path: str,
+        gslist_filter: str,
+        gslist_super_query: bool,
+        gslist_timeout: int,
+        verify: bool,
+        add_game_port: bool,
         expired_ttl: int,
         recover: bool,
         add_links: bool,
         txt: bool,
         list_dir: str,
         debug: bool
 ):
     logging.basicConfig(level=logging.DEBUG if debug else logging.INFO, stream=sys.stdout,
                         format='%(asctime)s %(levelname)-8s %(message)s')
-    logger.info(f'Listing servers for {game} via battlelog')
+    logger.info(f'Listing servers for {game} via gamespy/{principal}')
+
+    # Set principal
+    available_principals = GAMESPY_GAME_CONFIGS[game].principals
+    if principal not in GAMESPY_GAME_CONFIGS[game].principals:
+        # Given principal is invalid => use default principal
+        principal = available_principals[0]
 
-    lister = BattlelogServerLister(
+    lister = GameSpyServerLister(
         game,
-        page_limit,
+        principal,
+        gslist_path,
+        gslist_filter,
+        gslist_super_query,
+        gslist_timeout,
+        verify,
+        add_game_port,
         expired_ttl,
         recover,
         add_links,
         txt,
-        list_dir,
-        sleep,
-        max_attempts,
-        proxy
+        list_dir
     )
 
     before = len(lister.servers)
     lister.update_server_list()
-
-    if find_query_port:
-        lister.find_query_ports(gamedig_bin, gamedig_concurrency, expired_ttl)
-
     removed, recovered = lister.remove_expired_servers()
     lister.write_to_file()
 
     logger.info(f'Server list updated ('
                 f'total: {len(lister.servers)}, '
                 f'added: {len(lister.servers) + removed - before}, '
                 f'removed: {removed}, '
```

### Comparing `gameserverlister-1.1.2/GameserverLister/commands/bfbc2.py` & `gameserverlister-2.0.0/GameserverLister/commands/bfbc2.py`

 * *Files identical despite different names*

### Comparing `gameserverlister-1.1.2/GameserverLister/commands/gamespy.py` & `gameserverlister-2.0.0/GameserverLister/commands/valve.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,114 +1,93 @@
 import logging
 import sys
 
 import click
 
 from GameserverLister.commands.options import common, gameport
 from GameserverLister.common.logger import logger
-from GameserverLister.common.types import GamespyGame, GamespyPrincipal
-from GameserverLister.games.gamespy import GAMESPY_GAME_CONFIGS
-from GameserverLister.listers import GameSpyServerLister
+from GameserverLister.common.types import ValveGame, ValvePrincipal
+from GameserverLister.games.valve import VALVE_GAME_CONFIGS
+from GameserverLister.listers import ValveServerLister
 
 
 @click.command
 @click.option(
     '-g',
     '--game',
-    type=click.Choice(GamespyGame),
+    type=click.Choice(ValveGame),
     required=True,
     help='Game to list servers for'
 )
 @click.option(
     '-p',
     '--principal',
-    type=click.Choice(GamespyPrincipal),
-    required=True,
+    type=click.Choice(ValvePrincipal),
+    default=ValvePrincipal.VALVE,
     help='Principal server to query'
 )
 @click.option(
-    '-b',
-    '--gslist',
-    'gslist_path',
-    type=str,
-    required=True,
-    help='Path to gslist binary'
-)
-@click.option(
     '-f',
     '--filter',
-    'gslist_filter',
+    'filters',
     type=str,
     default='',
     help='Filter to apply to server list'
 )
 @click.option(
-    '-s',
-    '--super-query',
-    'gslist_super_query',
-    default=False,
-    is_flag=True,
-    help='Query each server in the list for it\'s status'
-)
-@click.option(
     '-t',
     '--timeout',
-    'gslist_timeout',
     type=int,
-    default=10,
-    help='Timeout to use for gslist command'
+    default=5,
+    help='Timeout to use for principal query'
 )
 @click.option(
-    '-v',
-    '--verify',
-    default=False,
-    is_flag=True,
-    help='(Attempt to) verify game servers returned by principal are game servers for the current game'
+    '-m',
+    '--max-pages',
+    type=int,
+    default=10,
+    help='Maximum number of pages to retrieve from the server list (per region)'
 )
 @gameport.add
 @common.expired_ttl
 @common.list_dir
 @common.recover
 @common.add_links
 @common.txt
 @common.debug
 def run(
-        game: GamespyGame,
-        principal: GamespyPrincipal,
-        gslist_path: str,
-        gslist_filter: str,
-        gslist_super_query: bool,
-        gslist_timeout: int,
-        verify: bool,
+        game: ValveGame,
+        principal: str,
+        filters: str,
+        timeout: int,
+        max_pages: int,
         add_game_port: bool,
         expired_ttl: int,
         recover: bool,
         add_links: bool,
         txt: bool,
         list_dir: str,
         debug: bool
 ):
     logging.basicConfig(level=logging.DEBUG if debug else logging.INFO, stream=sys.stdout,
                         format='%(asctime)s %(levelname)-8s %(message)s')
-    logger.info(f'Listing servers for {game} via gamespy/{principal}')
+    logger.info(f'Listing servers for {game} via valve/{principal}')
 
     # Set principal
-    available_principals = GAMESPY_GAME_CONFIGS[game].principals
-    if principal not in GAMESPY_GAME_CONFIGS[game].principals:
+    available_principals = VALVE_GAME_CONFIGS[game].principals
+    if principal not in VALVE_GAME_CONFIGS[game].principals:
         # Given principal is invalid => use default principal
         principal = available_principals[0]
 
-    lister = GameSpyServerLister(
+    lister = ValveServerLister(
         game,
         principal,
-        gslist_path,
-        gslist_filter,
-        gslist_super_query,
-        gslist_timeout,
-        verify,
+        timeout,
+        filters,
+        max_pages,
         add_game_port,
         expired_ttl,
         recover,
         add_links,
         txt,
         list_dir
     )
```

### Comparing `gameserverlister-1.1.2/GameserverLister/commands/gametools.py` & `gameserverlister-2.0.0/GameserverLister/commands/gametools.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 import logging
 import sys
 
 import click
 
 from GameserverLister.commands.options import common, http
 from GameserverLister.common.logger import logger
-from GameserverLister.common.types import GametoolsGame
+from GameserverLister.common.types import GametoolsGame, GametoolsPlatform
 from GameserverLister.listers import GametoolsServerLister
 
 
 @click.command
 @click.option(
     '-g',
     '--game',
     type=click.Choice(GametoolsGame),
     required=True,
     help='Game to list servers for'
 )
 @click.option(
+    '-pf',
+    '--platform',
+    type=click.Choice(GametoolsPlatform),
+    required=True,
+    help='Platform to list servers for',
+    default=GametoolsPlatform.PC
+)
+@click.option(
     '--include-official',
     default=False,
     is_flag=True,
     help='Include DICE official servers in list (not recommended due to auto scaling official servers)'
 )
 @http.page_limit
 @http.sleep
@@ -30,14 +38,15 @@
 @common.list_dir
 @common.recover
 @common.add_links
 @common.txt
 @common.debug
 def run(
         game: GametoolsGame,
+        platform: GametoolsPlatform,
         page_limit: int,
         sleep: float,
         max_attempts: int,
         include_official: bool,
         expired_ttl: int,
         recover: bool,
         add_links: bool,
@@ -47,14 +56,15 @@
 ):
     logging.basicConfig(level=logging.DEBUG if debug else logging.INFO, stream=sys.stdout,
                         format='%(asctime)s %(levelname)-8s %(message)s')
     logger.info(f'Listing servers for {game} via gametools')
 
     lister = GametoolsServerLister(
         game,
+        platform,
         page_limit,
         expired_ttl,
         recover,
         add_links,
         txt,
         list_dir,
         sleep,
```

### Comparing `gameserverlister-1.1.2/GameserverLister/commands/medalofhonor.py` & `gameserverlister-2.0.0/GameserverLister/commands/medalofhonor.py`

 * *Files identical despite different names*

### Comparing `gameserverlister-1.1.2/GameserverLister/commands/options/common.py` & `gameserverlister-2.0.0/GameserverLister/commands/options/common.py`

 * *Files identical despite different names*

### Comparing `gameserverlister-1.1.2/GameserverLister/commands/options/http.py` & `gameserverlister-2.0.0/GameserverLister/commands/options/http.py`

 * *Files identical despite different names*

### Comparing `gameserverlister-1.1.2/GameserverLister/commands/quake3.py` & `gameserverlister-2.0.0/GameserverLister/commands/quake3.py`

 * *Files identical despite different names*

### Comparing `gameserverlister-1.1.2/GameserverLister/commands/unreal2.py` & `gameserverlister-2.0.0/GameserverLister/commands/unreal2.py`

 * *Files identical despite different names*

### Comparing `gameserverlister-1.1.2/GameserverLister/commands/valve.py` & `gameserverlister-2.0.0/GameserverLister/commands/battlelog.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,103 +1,95 @@
 import logging
 import sys
+from typing import Optional
 
 import click
 
-from GameserverLister.commands.options import common, gameport
+from GameserverLister.commands.options import common, http, queryport
 from GameserverLister.common.logger import logger
-from GameserverLister.common.types import ValveGame, ValvePrincipal
-from GameserverLister.games.valve import VALVE_GAME_CONFIGS
-from GameserverLister.listers import ValveServerLister
+from GameserverLister.common.types import BattlelogGame, BattlelogPlatform
+from GameserverLister.listers import BattlelogServerLister
 
 
 @click.command
 @click.option(
     '-g',
     '--game',
-    type=click.Choice(ValveGame),
+    type=click.Choice(BattlelogGame),
     required=True,
     help='Game to list servers for'
 )
 @click.option(
-    '-p',
-    '--principal',
-    type=click.Choice(ValvePrincipal),
-    default=ValvePrincipal.VALVE,
-    help='Principal server to query'
-)
-@click.option(
-    '-f',
-    '--filter',
-    'filters',
-    type=str,
-    default='',
-    help='Filter to apply to server list'
-)
-@click.option(
-    '-t',
-    '--timeout',
-    type=int,
-    default=5,
-    help='Timeout to use for principal query'
-)
-@click.option(
-    '-m',
-    '--max-pages',
-    type=int,
-    default=10,
-    help='Maximum number of pages to retrieve from the server list (per region)'
+    '-pf',
+    '--platform',
+    type=click.Choice(BattlelogPlatform),
+    required=True,
+    help='Platform to list servers for',
+    default=BattlelogPlatform.PC
 )
-@gameport.add
+@http.page_limit
+@http.sleep
+@http.max_attempts
+@http.proxy
+@queryport.find
+@queryport.gamedig_bin
+@queryport.gamedig_concurrency
 @common.expired_ttl
 @common.list_dir
 @common.recover
 @common.add_links
 @common.txt
 @common.debug
 def run(
-        game: ValveGame,
-        principal: str,
-        filters: str,
-        timeout: int,
-        max_pages: int,
-        add_game_port: bool,
+        game: BattlelogGame,
+        platform: BattlelogPlatform,
+        page_limit: int,
+        sleep: float,
+        max_attempts: int,
+        proxy: Optional[str],
+        find_query_port: bool,
+        gamedig_bin: str,
+        gamedig_concurrency: int,
         expired_ttl: int,
         recover: bool,
         add_links: bool,
         txt: bool,
         list_dir: str,
         debug: bool
 ):
     logging.basicConfig(level=logging.DEBUG if debug else logging.INFO, stream=sys.stdout,
                         format='%(asctime)s %(levelname)-8s %(message)s')
-    logger.info(f'Listing servers for {game} via valve/{principal}')
 
-    # Set principal
-    available_principals = VALVE_GAME_CONFIGS[game].principals
-    if principal not in VALVE_GAME_CONFIGS[game].principals:
-        # Given principal is invalid => use default principal
-        principal = available_principals[0]
+    if game is BattlelogGame.BF3 and platform is not BattlelogPlatform.PC:
+        logger.warning(f'Platform {platform} is not available for {game}, defaulting to {BattlelogPlatform.PC} instead')
+        platform = BattlelogPlatform.PC
 
-    lister = ValveServerLister(
+    logger.info(f'Listing servers for {game} on {platform} via battlelog')
+    lister = BattlelogServerLister(
         game,
-        principal,
-        timeout,
-        filters,
-        max_pages,
-        add_game_port,
+        platform,
+        page_limit,
         expired_ttl,
         recover,
         add_links,
         txt,
-        list_dir
+        list_dir,
+        sleep,
+        max_attempts,
+        proxy
     )
 
+
+
     before = len(lister.servers)
     lister.update_server_list()
+
+    if find_query_port:
+        lister.find_query_ports(gamedig_bin, gamedig_concurrency, expired_ttl)
+
     removed, recovered = lister.remove_expired_servers()
     lister.write_to_file()
 
     logger.info(f'Server list updated ('
                 f'total: {len(lister.servers)}, '
                 f'added: {len(lister.servers) + removed - before}, '
                 f'removed: {removed}, '
```

### Comparing `gameserverlister-1.1.2/GameserverLister/common/helpers.py` & `gameserverlister-2.0.0/GameserverLister/common/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,18 +80,14 @@
     return 0 < port < 65536
 
 
 def battlelog_server_validator(server: FrostbiteServer, used_query_port: int, parsed_result: dict) -> bool:
     return parsed_result.get('connect') == f'{server.ip}:{server.game_port}'
 
 
-def mohwf_server_validator(server: FrostbiteServer, used_query_port: int, parsed_result: dict) -> bool:
-    return parsed_result.get('connect') == f'{server.ip}:{used_query_port}'
-
-
 def bfbc2_server_validator(server: BadCompany2Server, used_query_port: int, parsed_result: dict) -> bool:
     return battlelog_server_validator(server, used_query_port, parsed_result) or \
            parsed_result.get('connect') == f'0.0.0.0:{server.game_port}' or \
            parsed_result.get('name') == server.name
 
 
 def is_server_for_gamespy_game(game: GamespyGame, game_name: str, parsed_result: dict) -> bool:
```

### Comparing `gameserverlister-1.1.2/GameserverLister/common/servers.py` & `gameserverlister-2.0.0/GameserverLister/common/servers.py`

 * *Files identical despite different names*

### Comparing `gameserverlister-1.1.2/GameserverLister/common/types.py` & `gameserverlister-2.0.0/GameserverLister/common/types.py`

 * *Files 15% similar despite different names*

```diff
@@ -153,22 +153,63 @@
     BFBC2 = 'bfbc2'
 
 
 class BattlelogGame(Game):
     BF3 = 'bf3'
     BF4 = 'bf4'
     BFH = 'bfh'
-    MOHWF = 'mohwf'
 
 
 class GametoolsGame(Game):
     BF1 = 'bf1'
     BFV = 'bfv'
 
 
+class Platform(str, ExtendedEnum):
+    pass
+
+
+class GamespyPlatform(Platform):
+    PC = 'pc'
+
+
+class Quake3Platform(Platform):
+    PC = 'pc'
+
+
+class MedalOfHonorPlatform(Platform):
+    PC = 'pc'
+
+
+class Unreal2Platform(Platform):
+    PC = 'pc'
+
+
+class ValvePlatform(Platform):
+    PC = 'pc'
+
+
+class TheaterPlatform(Platform):
+    PC = 'pc'
+
+
+class BattlelogPlatform(Platform):
+    PC = 'pc'
+    PS3 = 'ps3'
+    PS4 = 'ps4'
+    Xbox360 = 'xbox360'
+    XboxOne = 'xboxone'
+
+
+class GametoolsPlatform(Platform):
+    PC = 'pc'
+    PS4 = 'ps4'
+    XboxOne = 'xboxone'
+
+
 @dataclass
 class GamespyGameConfig:
     game_name: str
     game_key: str
     enc_type: int
     query_type: int
     port: int
```

### Comparing `gameserverlister-1.1.2/GameserverLister/common/weblinks.py` & `gameserverlister-2.0.0/GameserverLister/common/weblinks.py`

 * *Files 22% similar despite different names*

```diff
@@ -71,76 +71,71 @@
     official: bool
 
     def __init__(self, site: str, url_template: str, official: bool):
         self.site = site
         self.url_template = url_template
         self.official = official
 
-    def render(self, game: str, uid: str, ip: Optional[str] = None, port: Optional[int] = None) -> WebLink:
+    def render(self, game: str, platform: str, uid: str, ip: Optional[str] = None, port: Optional[int] = None) -> WebLink:
         return WebLink(
             self.site,
-            self.url_template.format(game, uid, ip, port),
+            self.url_template.format(game=game, platform=platform, uid=uid, ip=ip, port=port),
             self.official
         )
 
 
 """
 For URL templates:
 0: game name/key
 1: server uid
 2: server ip
 3: server port
 """
 WEB_LINK_TEMPLATES: Dict[str, WebLinkTemplate] = {
     'arena.sh': WebLinkTemplate(
         'arena.sh',
-        'https://arena.sh/game/{2}:{3}/',
-        False
-    ),
-    'battlefieldtracker': WebLinkTemplate(
-        'battlefieldtracker.com',
-        'https://battlefieldtracker.com/bf1/servers/pc/{1}',
+        'https://arena.sh/game/{ip}:{port}/',
         False
     ),
     'battlelog': WebLinkTemplate(
         'battlelog.com',
-        'https://battlelog.battlefield.com/{0}/servers/show/pc/{1}',
+        'https://battlelog.battlefield.com/{game}/servers/show/{platform}/{uid}',
         True
     ),
     'bf2.tv': WebLinkTemplate(
         'bf2.tv',
-        'https://bf2.tv/servers/{2}:{3}',
+        'https://bf2.tv/servers/{ip}:{port}',
         False
     ),
     'bf2hub': WebLinkTemplate(
         'bf2hub.com',
-        'https://www.bf2hub.com/server/{2}:{3}/',
+        'https://www.bf2hub.com/server/{ip}:{port}/',
         True
     ),
     'cod.pm': WebLinkTemplate(
       'cod.pm',
-      'https://cod.pm/server/{2}/{3}',
+      'https://cod.pm/server/{ip}/{port}',
       False
     ),
     # deathmask.net shows servers from their own as well as other masters,
     # so they are not the official source for all servers
     'deathmask.net-official': WebLinkTemplate(
         'deathmask.net',
-        'https://dpmaster.deathmask.net/?game={0}&server={2}:{3}',
+        'https://dpmaster.deathmask.net/?game={game}&server={ip}:{port}',
         True
     ),
     'deathmask.net-unofficial': WebLinkTemplate(
         'deathmask.net',
-        'https://dpmaster.deathmask.net/?game={0}&server={2}:{3}',
+        'https://dpmaster.deathmask.net/?game={game}&server={ip}:{port}',
         False
     ),
     'gametools': WebLinkTemplate(
         'gametools.network',
-        'https://gametools.network/servers/{0}/gameid/{1}/pc',
+        'https://gametools.network/servers/{game}/gameid/{uid}/{platform}',
         False
     ),
     'swat4stats.com': WebLinkTemplate(
         'swat4stats.com',
-        'https://swat4stats.com/servers/{2}:{3}/',
+        'https://swat4stats.com/servers/{ip}:{port}/',
         False
     )
 }
```

### Comparing `gameserverlister-1.1.2/GameserverLister/games/gamespy.py` & `gameserverlister-2.0.0/GameserverLister/games/gamespy.py`

 * *Files identical despite different names*

### Comparing `gameserverlister-1.1.2/GameserverLister/games/quake3.py` & `gameserverlister-2.0.0/GameserverLister/games/quake3.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,27 @@
         'protocols': [
             1,  # version 1.1
             2,  # version 1.2
             4,  # version 1.3
             5,  # version 1.4
             6,  # version 1.5
         ],
+        'keywords': '',
         'servers': {
             'activision': {
                 'hostname': 'codmaster.activision.com',
                 'port': 20510
+            },
+            'cod.pm': {
+                'hostname': 'master.cod.pm',
+                'port': 20510
+            },
+            'comu-mvzg.com': {
+                'hostname': 'codmaster.comu-mvzg.com',
+                'port': 20510
             }
         },
         'linkTemplateRefs': {
             'activision': ['cod.pm']
         }
     },
     Quake3Game.CoDUO: {
```

### Comparing `gameserverlister-1.1.2/GameserverLister/games/unreal2.py` & `gameserverlister-2.0.0/GameserverLister/games/unreal2.py`

 * *Files identical despite different names*

### Comparing `gameserverlister-1.1.2/GameserverLister/games/valve.py` & `gameserverlister-2.0.0/GameserverLister/games/valve.py`

 * *Files identical despite different names*

### Comparing `gameserverlister-1.1.2/GameserverLister/listers/__init__.py` & `gameserverlister-2.0.0/GameserverLister/listers/__init__.py`

 * *Files identical despite different names*

### Comparing `gameserverlister-1.1.2/GameserverLister/listers/battlelog.py` & `gameserverlister-2.0.0/GameserverLister/listers/battlelog.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,69 @@
 import logging
 from datetime import datetime
 from typing import List, Tuple, Optional, Union
 
 import requests
 
-from GameserverLister.common.helpers import mohwf_server_validator, battlelog_server_validator
+from GameserverLister.common.helpers import battlelog_server_validator
 from GameserverLister.common.servers import FrostbiteServer
-from GameserverLister.common.types import BattlelogGame
+from GameserverLister.common.types import BattlelogGame, BattlelogPlatform
 from GameserverLister.common.weblinks import WEB_LINK_TEMPLATES, WebLink
 from GameserverLister.games.battlelog import BATTLELOG_GAME_BASE_URIS
 from .common import HttpServerLister, FrostbiteServerLister
 
 
 class BattlelogServerLister(HttpServerLister, FrostbiteServerLister):
     game: BattlelogGame
 
     def __init__(
             self,
             game: BattlelogGame,
+            platform: BattlelogPlatform,
             page_limit: int,
             expired_ttl: float,
             recover: bool,
             add_links: bool,
             txt: bool,
             list_dir: str,
             sleep: float,
             max_attempts: int,
             proxy: str = None
     ):
-        super().__init__(game, FrostbiteServer, page_limit, 60, expired_ttl, recover, add_links, txt, list_dir, sleep, max_attempts)
-        # Medal of Honor: Warfighter servers return the query port as part of the connect string, not the game port
-        # => use different validator
-        if self.game is BattlelogGame.MOHWF:
-            self.server_validator = mohwf_server_validator
-        else:
-            self.server_validator = battlelog_server_validator
+        super().__init__(game, platform, FrostbiteServer, page_limit, 60, expired_ttl, recover, add_links, txt, list_dir, sleep, max_attempts)
+        self.server_validator = battlelog_server_validator
 
         # Set up headers
         self.session.headers = {
             'X-Requested-With': 'XMLHttpRequest'
         }
         # Set up proxy if given
         if proxy is not None:
             # All requests are sent via https, so just set up https proxy
             self.session.proxies = {
                 'https': proxy
             }
 
     def get_server_list_url(self, per_page: int) -> str:
-        return f'{BATTLELOG_GAME_BASE_URIS[self.game]}?count={per_page}&offset=0'
+        return f'{BATTLELOG_GAME_BASE_URIS[self.game]}/{self.platform}/?count={per_page}&offset=0'
 
     def add_page_found_servers(self, found_servers: List[FrostbiteServer], page_response_data: dict) -> List[FrostbiteServer]:
         for server in page_response_data['data']:
             found_server = FrostbiteServer(
                 server['guid'],
                 server['name'],
                 server['ip'],
                 server['port'],
             )
 
             if self.add_links:
                 found_server.add_links(self.build_server_links(found_server.uid))
                 # Gametools uses the gameid for BF4 server URLs, so add that separately
                 if self.game is BattlelogGame.BF4:
-                    found_server.add_links(WEB_LINK_TEMPLATES['gametools'].render(self.game, server['gameId']))
+                    found_server.add_links(WEB_LINK_TEMPLATES['gametools'].render(self.game, self.platform, server['gameId']))
 
             # Add non-private servers (servers with an IP) that are new
             server_uids = [s.uid for s in found_servers]
             if len(found_server.ip) > 0 and found_server.uid not in server_uids:
                 logging.debug(f'Got new server {found_server.uid}, adding it')
                 found_servers.append(found_server)
             elif len(found_server.ip) > 0:
@@ -80,15 +76,15 @@
         return found_servers
 
     def check_if_server_still_exists(self, server: FrostbiteServer, checks_since_last_ok: int) -> Tuple[bool, bool, int]:
         check_ok = True
         found = False
         try:
             response = self.session.get(f'https://battlelog.battlefield.com/{self.game}/'
-                                        f'servers/show/pc/{server.uid}?json=1',
+                                        f'servers/show/{self.platform}/{server.uid}?json=1',
                                         timeout=self.request_timeout)
             if response.status_code == 200:
                 # Server was found on Battlelog => make sure it is still public
                 # TODO use server validator here
                 parsed = response.json()
                 found = parsed['message']['SERVER_INFO']['ip'] != ''
             elif response.status_code == 422:
@@ -112,22 +108,20 @@
 
     def build_server_links(
             self,
             uid: str,
             ip: Optional[str] = None,
             port: Optional[int] = None
     ) -> Union[List[WebLink], WebLink]:
-        # Medal of Honor: Warfighter (mohwf) is just called "mohw" on Battlelog
-        game = 'mohw' if self.game is BattlelogGame.MOHWF else self.game
-        links = [WEB_LINK_TEMPLATES['battlelog'].render(game, uid)]
+        links = [WEB_LINK_TEMPLATES['battlelog'].render(self.game, self.platform, uid)]
 
         # Gametools uses the guid as the "gameid" for BF3 and BFH, so we can add links for those
         # (BF4 uses the real gameid, so we need to handle those links separately)
         if self.game in ['bf3', 'bfh']:
-            links.append(WEB_LINK_TEMPLATES['gametools'].render(self.game, uid))
+            links.append(WEB_LINK_TEMPLATES['gametools'].render(self.game, self.platform, uid))
 
         return links
 
     def build_port_to_try_list(self, game_port: int) -> list:
         """
                 Order of ports to try:
                 1. default query port
```

### Comparing `gameserverlister-1.1.2/GameserverLister/listers/bfbc2.py` & `gameserverlister-2.0.0/GameserverLister/listers/bfbc2.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 from random import randint
 from typing import Tuple
 
 import requests
 
 from GameserverLister.common.helpers import bfbc2_server_validator, guid_from_ip_port
 from GameserverLister.common.servers import BadCompany2Server
-from GameserverLister.common.types import TheaterGame
+from GameserverLister.common.types import TheaterGame, TheaterPlatform
 from .common import FrostbiteServerLister
 
 
 class BadCompany2ServerLister(FrostbiteServerLister):
     game: TheaterGame
+    platform: TheaterPlatform
 
     def __init__(self, expired_ttl: float, recover: bool, add_links: bool, txt: bool, list_dir: str, timeout: float):
-        super().__init__(TheaterGame.BFBC2, BadCompany2Server, expired_ttl, recover, add_links, txt, list_dir, timeout)
+        super().__init__(TheaterGame.BFBC2, TheaterPlatform.PC, BadCompany2Server, expired_ttl, recover, add_links, txt, list_dir, timeout)
         self.server_validator = bfbc2_server_validator
 
     def update_server_list(self):
         request_ok = False
         attempt = 0
         max_attempts = 3
         servers = None
```

### Comparing `gameserverlister-1.1.2/GameserverLister/listers/common.py` & `gameserverlister-2.0.0/GameserverLister/listers/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 
 import gevent
 import requests
 from gevent.pool import Pool
 
 from GameserverLister.common.helpers import is_valid_port, find_query_port
 from GameserverLister.common.servers import Server, ObjectJSONEncoder, FrostbiteServer
-from GameserverLister.common.types import Game
+from GameserverLister.common.types import Game, Platform
 from GameserverLister.common.weblinks import WebLink
 
 
 class ServerLister:
     game: Game
+    platform: Platform
     server_list_dir_path: str
     server_list_file_path: str
     expired_ttl: float
     recover: bool
     add_links: bool
     txt: bool
     ensure_ascii: bool
@@ -31,23 +32,25 @@
 
     session: requests.Session
     request_timeout: float
 
     def __init__(
             self,
             game: Game,
+            platform: Platform,
             server_class: Type[Server],
             expired_ttl: float,
             recover: bool,
             add_links: bool,
             txt: bool,
             list_dir: str,
             request_timeout: float = 5.0
     ):
         self.game = game
+        self.platform = platform
         self.server_list_dir_path = os.path.realpath(list_dir)
         self.server_list_file_path = self.build_server_list_file_path('json')
 
         self.expired_ttl = expired_ttl
         self.recover = recover
         self.add_links = add_links
         self.txt = txt
@@ -154,15 +157,15 @@
         return []
 
     def get_backoff_timeout(self, checks_since_last_ok: int) -> int:
         # Default to no backoff
         return 0
 
     def build_server_list_file_path(self, extension: str) -> str:
-        return os.path.join(self.server_list_dir_path, f'{self.game}-servers.{extension}')
+        return os.path.join(self.server_list_dir_path, f'{self.game}-servers-{self.platform}.{extension}')
 
     def write_to_file(self):
         logging.info(f'Writing {len(self.servers)} servers to output file')
         with open(self.server_list_file_path, 'w') as output_file:
             json.dump(self.servers, output_file, indent=2, ensure_ascii=self.ensure_ascii, cls=ObjectJSONEncoder)
 
         if self.txt:
@@ -174,23 +177,24 @@
 class FrostbiteServerLister(ServerLister):
     servers: List[FrostbiteServer]
     server_validator: Callable
 
     def __init__(
             self,
             game: Game,
+            platform: Platform,
             server_class: Type[Server],
             expired_ttl: float,
             recover: bool,
             add_links: bool,
             txt: bool,
             list_dir: str,
             request_timeout: float = 5.0
     ):
-        super().__init__(game, server_class, expired_ttl, recover, add_links, txt, list_dir, request_timeout)
+        super().__init__(game, platform, server_class, expired_ttl, recover, add_links, txt, list_dir, request_timeout)
 
     def find_query_ports(self, gamedig_bin_path: str, gamedig_concurrency: int, expired_ttl: float):
         logging.info(f'Searching query port for {len(self.servers)} servers')
 
         search_stats = {
             'totalSearches': len(self.servers),
             'queryPortFound': 0,
@@ -239,26 +243,27 @@
     per_page: int
     sleep: float
     max_attempts: int
 
     def __init__(
             self,
             game: Game,
+            platform: Platform,
             server_class: Type[Server],
             page_limit: int,
             per_page: int,
             expired_ttl: float,
             recover: bool,
             add_links: bool,
             txt: bool,
             list_dir: str,
             sleep: float,
             max_attempts: int
     ):
-        super().__init__(game, server_class, expired_ttl, recover, add_links, txt, list_dir, request_timeout=10)
+        super().__init__(game, platform, server_class, expired_ttl, recover, add_links, txt, list_dir, request_timeout=10)
         self.page_limit = page_limit
         self.per_page = per_page
         self.sleep = sleep
         self.max_attempts = max_attempts
 
     def update_server_list(self):
         offset = 0
```

### Comparing `gameserverlister-1.1.2/GameserverLister/listers/gamespy.py` & `gameserverlister-2.0.0/GameserverLister/listers/gamespy.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 import subprocess
 import sys
 from typing import List, Tuple, Optional, Union
 
 from GameserverLister.common.helpers import is_valid_public_ip, is_valid_port, guid_from_ip_port, \
     is_server_for_gamespy_game, resolve_host
 from GameserverLister.common.servers import ClassicServer, ViaStatus
-from GameserverLister.common.types import GamespyGame, GamespyPrincipal, GamespyGameConfig
+from GameserverLister.common.types import GamespyGame, GamespyPrincipal, GamespyGameConfig, GamespyPlatform
 from GameserverLister.common.weblinks import WebLink, WEB_LINK_TEMPLATES
 from GameserverLister.games.gamespy import GAMESPY_PRINCIPAL_CONFIGS, GAMESPY_GAME_CONFIGS
 from .common import ServerLister
 
 
 class GameSpyServerLister(ServerLister):
     game: GamespyGame
+    platform: GamespyPlatform
     servers: List[ClassicServer]
     principal: GamespyPrincipal
     config: GamespyGameConfig
     gslist_bin_path: str
     gslist_filter: str
     gslist_super_query: bool
     gslist_timeout: int
@@ -37,15 +38,15 @@
             add_game_port: bool,
             expired_ttl: float,
             recover: bool,
             add_links: bool,
             txt: bool,
             list_dir: str
     ):
-        super().__init__(game, ClassicServer, expired_ttl, recover, add_links, txt, list_dir)
+        super().__init__(game, GamespyPlatform.PC, ClassicServer, expired_ttl, recover, add_links, txt, list_dir)
         self.principal = principal.lower()
         self.config = GAMESPY_GAME_CONFIGS[self.game]
         self.gslist_bin_path = gslist_bin_path
         self.gslist_filter = gslist_filter
         self.gslist_super_query = gslist_super_query
         self.gslist_timeout = gslist_timeout
         self.verify = verify
@@ -194,15 +195,15 @@
         templates = [
             *[WEB_LINK_TEMPLATES.get(ref) for ref in template_refs.get(self.principal, [])],
             *[WEB_LINK_TEMPLATES.get(ref) for ref in template_refs.get('_any', [])]
         ]
 
         links = []
         for template in templates:
-            links.append(template.render(self.game, uid, ip=ip, port=port))
+            links.append(template.render(self.game, self.platform, uid, ip=ip, port=port))
 
         return links
 
     def query_server(self, server: ClassicServer) -> Tuple[bool, dict]:
         try:
             command = [self.gslist_bin_path, '-d', str(self.config.query_type), server.ip, str(server.query_port), '-0']
             # Timeout should never fire since gslist uses about a three-second timeout for the query
```

### Comparing `gameserverlister-1.1.2/GameserverLister/listers/gametools.py` & `gameserverlister-2.0.0/GameserverLister/listers/gametools.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 import logging
 from datetime import datetime
 from typing import List, Tuple, Optional, Union
 
 import requests
 
 from GameserverLister.common.servers import GametoolsServer
-from GameserverLister.common.types import GametoolsGame
+from GameserverLister.common.types import GametoolsGame, GametoolsPlatform
 from GameserverLister.common.weblinks import WebLink, WEB_LINK_TEMPLATES
 from GameserverLister.games.gametools import GAMETOOLS_BASE_URI
 from .common import HttpServerLister
 
 
 class GametoolsServerLister(HttpServerLister):
     game: GametoolsGame
+    platform: GametoolsPlatform
     include_official: bool
 
     def __init__(
             self,
             game: GametoolsGame,
+            platform: GametoolsPlatform,
             page_limit: int,
             expired_ttl: float,
             recover: bool,
             add_links: bool,
             txt: bool,
             list_dir: str,
             sleep: float,
             max_attempts: int,
             include_official: bool
     ):
         super().__init__(
             game,
+            platform,
             GametoolsServer,
             page_limit,
             100,
             expired_ttl,
             recover,
             add_links,
             txt,
@@ -42,15 +45,15 @@
             max_attempts
         )
         # Allow non-ascii characters in server list (mostly used by server names for Asia servers)
         self.ensure_ascii = False
         self.include_official = include_official
 
     def get_server_list_url(self, per_page: int) -> str:
-        return f'{GAMETOOLS_BASE_URI}/{self.game}/servers/?name=&limit={per_page}' \
+        return f'{GAMETOOLS_BASE_URI}/{self.game}/servers/?platform={self.platform}&region=all&name=&limit={per_page}' \
                f'&nocache={datetime.now().timestamp()}'
 
     def add_page_found_servers(self, found_servers: List[GametoolsServer], page_response_data: dict) -> List[GametoolsServer]:
         for server in page_response_data['servers']:
             found_server = GametoolsServer(
                 server['gameId'],
                 server['prefix'],
@@ -105,13 +108,8 @@
 
     def build_server_links(
             self,
             uid: str,
             ip: Optional[str] = None,
             port: Optional[int] = None
     ) -> Union[List[WebLink], WebLink]:
-        links = [WEB_LINK_TEMPLATES['gametools'].render(self.game, uid)]
-        # BF1 servers are also listed on battlefieldtracker.com
-        if self.game is GametoolsGame.BF1:
-            links.append(WEB_LINK_TEMPLATES['battlefieldtracker'].render(self.game, uid))
-
-        return links
+        return [WEB_LINK_TEMPLATES['gametools'].render(self.game, self.platform, uid)]
```

### Comparing `gameserverlister-1.1.2/GameserverLister/listers/medalofhonor.py` & `gameserverlister-2.0.0/GameserverLister/listers/medalofhonor.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,38 +3,39 @@
 from typing import Tuple
 
 import pyq3serverlist
 import requests
 
 from GameserverLister.common.helpers import is_valid_public_ip, is_valid_port, guid_from_ip_port
 from GameserverLister.common.servers import ClassicServer, ViaStatus
-from GameserverLister.common.types import MedalOfHonorGame
+from GameserverLister.common.types import MedalOfHonorGame, MedalOfHonorPlatform
 from .common import ServerLister
 
 
 class MedalOfHonorServerLister(ServerLister):
     """
     The defacto standard principal server for Medal of Honor games uses a query GameSpy protocol implementation that
     does not work with gslist. However, they also provide server lists as text files, which unfortunately only contain
     the game port. So, instead of extending the GameSpy server lister and trying to find the query port, we use the
     text files to find servers. Since the Medal of Honor games support Quake3-like queries on the game port, we can use
     that to query servers with the information we have.
     """
     game: MedalOfHonorGame
+    platform: MedalOfHonorPlatform
 
     def __init__(
             self,
             game: MedalOfHonorGame,
             expired_ttl: float,
             recover: bool,
             add_links: bool,
             txt: bool,
             list_dir: str
     ):
-        super().__init__(game, ClassicServer, expired_ttl, recover, add_links, txt, list_dir)
+        super().__init__(game, MedalOfHonorPlatform.PC, ClassicServer, expired_ttl, recover, add_links, txt, list_dir)
 
     def update_server_list(self):
         request_ok = False
         attempt = 0
         max_attempts = 3
         raw_server_list = None
         while not request_ok and attempt < max_attempts:
```

### Comparing `gameserverlister-1.1.2/GameserverLister/listers/quake3.py` & `gameserverlister-2.0.0/GameserverLister/listers/quake3.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 import socket
 from typing import List, Tuple, Optional, Union
 
 import pyq3serverlist
 
 from GameserverLister.common.helpers import is_valid_public_ip, is_valid_port, guid_from_ip_port
 from GameserverLister.common.servers import ClassicServer, ViaStatus
-from GameserverLister.common.types import Quake3Game
+from GameserverLister.common.types import Quake3Game, Quake3Platform
 from GameserverLister.common.weblinks import WebLink, WEB_LINK_TEMPLATES
 from GameserverLister.games.quake3 import QUAKE3_CONFIGS
 from .common import ServerLister
 
 
 class Quake3ServerLister(ServerLister):
     game: Quake3Game
+    platform: Quake3Platform
     principal: str
     protocols: List[int]
     network_protocol: int
     game_name: str
     keywords: str
     server_entry_prefix: bytes
 
@@ -27,15 +28,15 @@
             principal: str,
             expired_ttl: float,
             recover: bool,
             add_links: bool,
             txt: bool,
             list_dir: str
     ):
-        super().__init__(game, ClassicServer, expired_ttl, recover, add_links, txt, list_dir)
+        super().__init__(game, Quake3Platform.PC, ClassicServer, expired_ttl, recover, add_links, txt, list_dir)
         # Merge default config with given principal config
         default_config = {
             'keywords': 'full empty',
             'game_name': '',
             'network_protocol': socket.SOCK_DGRAM,
             'server_entry_prefix': b''
         }
@@ -132,10 +133,10 @@
         templates = [
             *[WEB_LINK_TEMPLATES.get(ref) for ref in template_refs.get(self.principal, [])],
             *[WEB_LINK_TEMPLATES.get(ref) for ref in template_refs.get('_any', [])]
         ]
 
         links = []
         for template in templates:
-            links.append(template.render(self.game, uid, ip=ip, port=port))
+            links.append(template.render(self.game, self.platform, uid, ip=ip, port=port))
 
         return links
```

### Comparing `gameserverlister-1.1.2/GameserverLister/listers/unreal2.py` & `gameserverlister-2.0.0/GameserverLister/listers/unreal2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import logging
 from typing import List, Tuple, Optional, Union
 
 import pyut2serverlist
 
 from GameserverLister.common.helpers import is_valid_public_ip, is_valid_port, guid_from_ip_port
 from GameserverLister.common.servers import ClassicServer, ViaStatus
-from GameserverLister.common.types import Unreal2Game
+from GameserverLister.common.types import Unreal2Game, Unreal2Platform
 from GameserverLister.common.weblinks import WebLink, WEB_LINK_TEMPLATES
 from GameserverLister.games.unreal2 import UNREAL2_CONFIGS
 from .common import ServerLister
 
 
 class Unreal2ServerLister(ServerLister):
     game: Unreal2Game
+    platform: Unreal2Platform
     principal: str
     cd_key: str
 
     principal_timeout: float
 
     def __init__(
             self,
@@ -26,15 +27,15 @@
             principal_timeout: float,
             expired_ttl: float,
             recover: bool,
             add_links: bool,
             txt: bool,
             list_dir: str
     ):
-        super().__init__(game, ClassicServer, expired_ttl, recover, add_links, txt, list_dir)
+        super().__init__(game, Unreal2Platform.PC, ClassicServer, expired_ttl, recover, add_links, txt, list_dir)
         self.principal = principal
         self.cd_key = cd_key
         self.principal_timeout = principal_timeout
 
     def update_server_list(self):
         hostname, port = UNREAL2_CONFIGS[self.game]['servers'][self.principal].values()
         principal = pyut2serverlist.PrincipalServer(
@@ -123,10 +124,10 @@
         templates = [
             *[WEB_LINK_TEMPLATES.get(ref) for ref in template_refs.get(self.principal, [])],
             *[WEB_LINK_TEMPLATES.get(ref) for ref in template_refs.get('_any', [])]
         ]
 
         links = []
         for template in templates:
-            links.append(template.render(self.game, uid, ip=ip, port=port))
+            links.append(template.render(self.game, self.platform, uid, ip=ip, port=port))
 
         return links
```

### Comparing `gameserverlister-1.1.2/GameserverLister/listers/valve.py` & `gameserverlister-2.0.0/GameserverLister/listers/valve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import logging
 from typing import List, Tuple, Optional
 
 import pyvpsq
 
 from GameserverLister.common.helpers import is_valid_public_ip, is_valid_port, guid_from_ip_port
 from GameserverLister.common.servers import ClassicServer, ViaStatus
-from GameserverLister.common.types import ValveGame, ValvePrincipal, ValveGameConfig
+from GameserverLister.common.types import ValveGame, ValvePrincipal, ValveGameConfig, ValvePlatform
 from GameserverLister.games.valve import VALVE_PRINCIPAL_CONFIGS, VALVE_GAME_CONFIGS
 from GameserverLister.listers.common import ServerLister
 
 
 class ValveServerLister(ServerLister):
     game: ValveGame
+    platform: ValvePlatform
     servers: List[ClassicServer]
     principal: ValvePrincipal
     config: ValveGameConfig
 
     principal_timeout: float
     filters: str
     max_pages: int
@@ -32,15 +33,15 @@
             add_game_port: bool,
             expired_ttl: float,
             recover: bool,
             add_links: bool,
             txt: bool,
             list_dir: str
     ):
-        super().__init__(game, ClassicServer, expired_ttl, recover, add_links, txt, list_dir)
+        super().__init__(game, ValvePlatform.PC, ClassicServer, expired_ttl, recover, add_links, txt, list_dir)
         self.principal = principal
         self.config = VALVE_GAME_CONFIGS[self.game]
         self.principal_timeout = principal_timeout
         self.filters = filters
         self.max_pages = max_pages
         self.add_game_port = add_game_port
```

### Comparing `gameserverlister-1.1.2/GameserverLister.egg-info/PKG-INFO` & `gameserverlister-2.0.0/GameserverLister.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: GameserverLister
-Version: 1.1.2
+Version: 2.0.0
 Summary: Python command line tool to retrieve game server lists for various games
 Home-page: https://github.com/cetteup/GameserverLister
 Author: cetteup
 Author-email: me@cetteup.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cetteup/GameserverLister/issues
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Internet
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: gevent==23.9.0.post1
+Requires-Dist: gevent==24.2.1
 Requires-Dist: nslookup==1.7.0
 Requires-Dist: requests[socks]==2.31.0
 Requires-Dist: pyq3serverlist==0.3.2
 Requires-Dist: pyut2serverlist==0.2.0
 Requires-Dist: pyvpsq==0.1.2
 Requires-Dist: click==8.1.7
 
@@ -90,89 +90,88 @@
 
 The server list retrieval for GameSpy-games requires an external tool. In order to retrieve GameSpy servers, you need to set up [gslist](http://aluigi.altervista.org/papers.htm#gslist). `gslist` was developed by Luigi Auriemma.
 
 ## Supported games
 
 The scripts support retrieval for following games from the listed sources. If you know more sources for any of the listed games or know other games that support the listed protocols, please create an issue, and I will add them.
 
-| Game                                   | Source type/protocol | Server list source(s)                                                                                             |
-|----------------------------------------|----------------------|-------------------------------------------------------------------------------------------------------------------|
-| 7 Days to Die                          | Valve                | Valve ¹                                                                                                           |
-| America's Army: Proving Grounds        | Valve                | Valve ¹                                                                                                           |
-| ARK: Survival Evolved                  | Valve                | Valve ¹                                                                                                           |
-| Arma 2                                 | Valve                | Valve ¹                                                                                                           |
-| Arma 3                                 | Valve                | Valve ¹                                                                                                           |
-| Battlefield 1942                       | GameSpy              | bf1942.org, openspy.net, qtracker.com                                                                             |
-| Battlefield Vietnam                    | GameSpy              | openspy.net, qtracker.com                                                                                         |
-| Battlefield 2                          | GamsSpy              | bf2hub.com, playbf2.ru                                                                                            |
-| Battlefield 2142                       | GameSpy              | novgames.ru, openspy.net, play2142.ru                                                                             |
-| Battlefield: Bad Company 2             | fesl/theater         | Project Rome (emulatornexus.com)                                                                                  |
-| Battlefield 3                          | Battlelog            | battlelog.com                                                                                                     |
-| Battlefield 4                          | Battlelog            | battlelog.com                                                                                                     |
-| Battlefield Hardline                   | Battlelog            | battlelog.com                                                                                                     |
-| Battlefield 1                          | Gametools API        | api.gametools.network                                                                                             |
-| Battlefield 5                          | Gametools API        | api.gametools.network                                                                                             |
-| Call of Duty                           | Quake3               | Activision                                                                                                        |
-| Call of Duty: United Offensive         | Quake3               | Activision                                                                                                        |
-| Call of Duty 2                         | Quake3               | Activision                                                                                                        |
-| Call of Duty 4: Modern Warfare         | Quake3               | Activision                                                                                                        |
-| CoD4x Mod                              | Quake3               | cod4x.ovh                                                                                                         |
-| Counter Strike                         | Valve                | Valve ¹                                                                                                           |
-| Counter Strike: Condition Zero         | Valve                | Valve ¹                                                                                                           |
-| Counter Strike: Source                 | Valve                | Valve ¹                                                                                                           |
-| Counter Strike: Global Offensive       | Valve                | Valve ¹                                                                                                           |
-| Crysis                                 | GameSpy              | crymp.net                                                                                                         |
-| Crysis Wars                            | GameSpy              | jedi95.us                                                                                                         |
-| Day of Defeat                          | Valve                | Valve ¹                                                                                                           |
-| Day of Defeat: Source                  | Valve                | Valve ¹                                                                                                           |
-| DayZ                                   | Valve                | Valve ¹                                                                                                           |
-| DayZ (Arma 2 mod)                      | Valve                | Valve ¹                                                                                                           |
-| Deus Ex                                | GameSpy              | 333networks.com, errorist.eu, newbiesplayground.net, oldunreal.com                                                |
-| Duke Nukem Forever                     | GameSpy              | 333networks.com                                                                                                   |
-| Forgotten Hope 2                       | GameSpy              | fh2.dev                                                                                                           |
-| Garry's Mod                            | Valve                | Valve ¹                                                                                                           |
-| Insurgency                             | Valve                | Valve ¹                                                                                                           |
-| Insurgency: Sandstorm                  | Valve                | Valve ¹                                                                                                           |
-| James Bond 007: Nightfire              | GameSpy              | openspy.net, nightfirepc.com                                                                                      |
-| Left 4 Dead                            | Valve                | Valve ¹                                                                                                           |
-| Left 4 Dead 2                          | Valve                | Valve ¹                                                                                                           |
-| Medal of Honor Warfighter              | Battlelog            | battlelog.com                                                                                                     |
-| Nexuiz                                 | Quake3               | deathmask.net                                                                                                     |
-| OpenArena                              | Quake3               | deathmask.net                                                                                                     |
-| ParaWorld                              | GameSpy              | openspy.net                                                                                                       |
-| Postal 2                               | GameSpy              | 333networks.com                                                                                                   |
-| Q3Rally                                | Quake3               | deathmask.net                                                                                                     |
-| Quake                                  | Quake3               | deathmask.net                                                                                                     |
-| Quake 3 Arena                          | Quake3               | quake3arena.com, urbanterror.info, excessiveplus.net, ioquake3.org, huxxer.de, maverickservers.com, deathmask.net |
-| Return to Castle Wolfenstein           | Quake3               | id Software                                                                                                       |
-| Rising Storm 2: Vietnam                | Valve                | Valve ¹                                                                                                           |
-| Rune                                   | GameSpy              | 333networks.com, errorist.eu, newbiesplayground.net, oldunreal.com                                                |
-| Rust                                   | Valve                | Valve ¹                                                                                                           |
-| Serious Sam: The First Encounter       | GameSpy              | 333networks.com, errorist.eu, newbiesplayground.net, oldunreal.com                                                |
-| Serious Sam: Second Encounter          | GameSpy              | 333networks.com, errorist.eu, newbiesplayground.net, oldunreal.com                                                |
-| Soldier of Fortune II: Double Helix    | Quake3               | Raven Software                                                                                                    |
-| Squad                                  | Valve                | Valve ¹                                                                                                           |
-| Star Wars Jedi Knight II: Jedi Outcast | Quake3               | Raven Software, jkhub.org                                                                                         |
-| Star Wars Jedi Knight: Jedi Academy    | Quake3               | Raven Software, jkhub.org                                                                                         |
-| SWAT 4                                 | GameSpy              | swat4stats.com                                                                                                    |
-| Team Fortress Classic                  | Valve                | Valve ¹                                                                                                           |
-| Team Fortress 2                        | Valve                | Valve ¹                                                                                                           |
-| Tremulous                              | Quake3               | tremulous.net                                                                                                     |
-| Unreal                                 | GameSpy              | 333networks.com, errorist.eu, openspy.net, oldunreal.com, qtracker.com                                            |
-| Unreal Tournament                      | GameSpy              | 333networks.com, errorist.eu, openspy.net, oldunreal.com, qtracker.com                                            |
-| Unreal Tournament 2003                 | Unreal2              | openspy.net                                                                                                       |
-| Unreal Tournament 2004                 | Unreal2              | openspy.net, 333networks.com, errorist.eu                                                                         |
-| Unreal Tournament 3                    | GameSpy              | openspy.net                                                                                                       |
-| UrbanTerror                            | Quake3               | FrozenSand                                                                                                        |
-| Vietcong                               | GameSpy              | vietcong.tk, vietcong1.eu, qtracker.com                                                                           |
-| Vietcong 2                             | GameSpy              | openspy.net                                                                                                       |
-| Warfork                                | Quake3               | deathmask.net                                                                                                     |
-| Warsow                                 | Quake3               | deathmask.net                                                                                                     |
-| Wheel of Time                          | GameSpy              | 333networks.com, errorist.eu, newbiesplayground.net, oldunreal.com                                                |
-| Wolfenstein: Enemy Territory           | Quake3               | id Software, etlegacy.com                                                                                         |
-| Xonotic                                | Quake3               | deathmask.net, tchr.no                                                                                            |
+| Game                                   | Platforms                        | Source type/protocol | Server list source(s)                                                                                             |
+|----------------------------------------|----------------------------------|----------------------|-------------------------------------------------------------------------------------------------------------------|
+| 7 Days to Die                          | PC                               | Valve                | Valve ¹                                                                                                           |
+| America's Army: Proving Grounds        | PC                               | Valve                | Valve ¹                                                                                                           |
+| ARK: Survival Evolved                  | PC                               | Valve                | Valve ¹                                                                                                           |
+| Arma 2                                 | PC                               | Valve                | Valve ¹                                                                                                           |
+| Arma 3                                 | PC                               | Valve                | Valve ¹                                                                                                           |
+| Battlefield 1942                       | PC                               | GameSpy              | bf1942.org, openspy.net, qtracker.com                                                                             |
+| Battlefield Vietnam                    | PC                               | GameSpy              | openspy.net, qtracker.com                                                                                         |
+| Battlefield 2                          | PC                               | GamsSpy              | bf2hub.com, playbf2.ru                                                                                            |
+| Battlefield 2142                       | PC                               | GameSpy              | novgames.ru, openspy.net, play2142.ru                                                                             |
+| Battlefield: Bad Company 2             | PC                               | fesl/theater         | Project Rome (emulatornexus.com)                                                                                  |
+| Battlefield 3                          | PC                               | Battlelog            | battlelog.com                                                                                                     |
+| Battlefield 4                          | PC, PS3, PS4, Xbox 360, Xbox One | Battlelog            | battlelog.com                                                                                                     |
+| Battlefield Hardline                   | PC, PS3, PS4, Xbox 360, Xbox One | Battlelog            | battlelog.com                                                                                                     |
+| Battlefield 1                          | PC                               | Gametools API        | api.gametools.network                                                                                             |
+| Battlefield 5                          | PC                               | Gametools API        | api.gametools.network                                                                                             |
+| Call of Duty                           | PC                               | Quake3               | Activision                                                                                                        |
+| Call of Duty: United Offensive         | PC                               | Quake3               | Activision                                                                                                        |
+| Call of Duty 2                         | PC                               | Quake3               | Activision                                                                                                        |
+| Call of Duty 4: Modern Warfare         | PC                               | Quake3               | Activision                                                                                                        |
+| CoD4x Mod                              | PC                               | Quake3               | cod4x.ovh                                                                                                         |
+| Counter Strike                         | PC                               | Valve                | Valve ¹                                                                                                           |
+| Counter Strike: Condition Zero         | PC                               | Valve                | Valve ¹                                                                                                           |
+| Counter Strike: Source                 | PC                               | Valve                | Valve ¹                                                                                                           |
+| Counter Strike: Global Offensive       | PC                               | Valve                | Valve ¹                                                                                                           |
+| Crysis                                 | PC                               | GameSpy              | crymp.net                                                                                                         |
+| Crysis Wars                            | PC                               | GameSpy              | jedi95.us                                                                                                         |
+| Day of Defeat                          | PC                               | Valve                | Valve ¹                                                                                                           |
+| Day of Defeat: Source                  | PC                               | Valve                | Valve ¹                                                                                                           |
+| DayZ                                   | PC                               | Valve                | Valve ¹                                                                                                           |
+| DayZ (Arma 2 mod)                      | PC                               | Valve                | Valve ¹                                                                                                           |
+| Deus Ex                                | PC                               | GameSpy              | 333networks.com, errorist.eu, newbiesplayground.net, oldunreal.com                                                |
+| Duke Nukem Forever                     | PC                               | GameSpy              | 333networks.com                                                                                                   |
+| Forgotten Hope 2                       | PC                               | GameSpy              | fh2.dev                                                                                                           |
+| Garry's Mod                            | PC                               | Valve                | Valve ¹                                                                                                           |
+| Insurgency                             | PC                               | Valve                | Valve ¹                                                                                                           |
+| Insurgency: Sandstorm                  | PC                               | Valve                | Valve ¹                                                                                                           |
+| James Bond 007: Nightfire              | PC                               | GameSpy              | openspy.net, nightfirepc.com                                                                                      |
+| Left 4 Dead                            | PC                               | Valve                | Valve ¹                                                                                                           |
+| Left 4 Dead 2                          | PC                               | Valve                | Valve ¹                                                                                                           |
+| Nexuiz                                 | PC                               | Quake3               | deathmask.net                                                                                                     |
+| OpenArena                              | PC                               | Quake3               | deathmask.net                                                                                                     |
+| ParaWorld                              | PC                               | GameSpy              | openspy.net                                                                                                       |
+| Postal 2                               | PC                               | GameSpy              | 333networks.com                                                                                                   |
+| Q3Rally                                | PC                               | Quake3               | deathmask.net                                                                                                     |
+| Quake                                  | PC                               | Quake3               | deathmask.net                                                                                                     |
+| Quake 3 Arena                          | PC                               | Quake3               | quake3arena.com, urbanterror.info, excessiveplus.net, ioquake3.org, huxxer.de, maverickservers.com, deathmask.net |
+| Return to Castle Wolfenstein           | PC                               | Quake3               | id Software                                                                                                       |
+| Rising Storm 2: Vietnam                | PC                               | Valve                | Valve ¹                                                                                                           |
+| Rune                                   | PC                               | GameSpy              | 333networks.com, errorist.eu, newbiesplayground.net, oldunreal.com                                                |
+| Rust                                   | PC                               | Valve                | Valve ¹                                                                                                           |
+| Serious Sam: The First Encounter       | PC                               | GameSpy              | 333networks.com, errorist.eu, newbiesplayground.net, oldunreal.com                                                |
+| Serious Sam: Second Encounter          | PC                               | GameSpy              | 333networks.com, errorist.eu, newbiesplayground.net, oldunreal.com                                                |
+| Soldier of Fortune II: Double Helix    | PC                               | Quake3               | Raven Software                                                                                                    |
+| Squad                                  | PC                               | Valve                | Valve ¹                                                                                                           |
+| Star Wars Jedi Knight II: Jedi Outcast | PC                               | Quake3               | Raven Software, jkhub.org                                                                                         |
+| Star Wars Jedi Knight: Jedi Academy    | PC                               | Quake3               | Raven Software, jkhub.org                                                                                         |
+| SWAT 4                                 | PC                               | GameSpy              | swat4stats.com                                                                                                    |
+| Team Fortress Classic                  | PC                               | Valve                | Valve ¹                                                                                                           |
+| Team Fortress 2                        | PC                               | Valve                | Valve ¹                                                                                                           |
+| Tremulous                              | PC                               | Quake3               | tremulous.net                                                                                                     |
+| Unreal                                 | PC                               | GameSpy              | 333networks.com, errorist.eu, openspy.net, oldunreal.com, qtracker.com                                            |
+| Unreal Tournament                      | PC                               | GameSpy              | 333networks.com, errorist.eu, openspy.net, oldunreal.com, qtracker.com                                            |
+| Unreal Tournament 2003                 | PC                               | Unreal2              | openspy.net                                                                                                       |
+| Unreal Tournament 2004                 | PC                               | Unreal2              | openspy.net, 333networks.com, errorist.eu                                                                         |
+| Unreal Tournament 3                    | PC                               | GameSpy              | openspy.net                                                                                                       |
+| UrbanTerror                            | PC                               | Quake3               | FrozenSand                                                                                                        |
+| Vietcong                               | PC                               | GameSpy              | vietcong.tk, vietcong1.eu, qtracker.com                                                                           |
+| Vietcong 2                             | PC                               | GameSpy              | openspy.net                                                                                                       |
+| Warfork                                | PC                               | Quake3               | deathmask.net                                                                                                     |
+| Warsow                                 | PC                               | Quake3               | deathmask.net                                                                                                     |
+| Wheel of Time                          | PC                               | GameSpy              | 333networks.com, errorist.eu, newbiesplayground.net, oldunreal.com                                                |
+| Wolfenstein: Enemy Territory           | PC                               | Quake3               | id Software, etlegacy.com                                                                                         |
+| Xonotic                                | PC                               | Quake3               | deathmask.net, tchr.no                                                                                            |
 
 ¹ Valve's principal servers are rate limited. If you do not use additional filters to only retrieve matching servers, you will get blocked/timed out. You can pass filters via the `-f`/`--filter` argument, e.g. use `-f "\dedicated\1\password\0\empty\1\full\1"` to only retrieve dedicated servers without a password which are neither full nor empty. You can find a full list of filter options [here](https://developer.valvesoftware.com/wiki/Master_Server_Query_Protocol#Filter) (the `\appid\` filter is applied automatically). 
 
 ## Game server query ports
 
 After obtaining a server list, you may want request current details directly from the game server via different query protocols. However, only the GameSpy and Quake3 principal servers return the game server's query port. Battlelog and the EA fesl/theater do not provide details about the server's query port. So, the respective scripts attempt to find the query port if run with the `--find-query-port` flag.
```

### Comparing `gameserverlister-1.1.2/GameserverLister.egg-info/SOURCES.txt` & `gameserverlister-2.0.0/GameserverLister.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gameserverlister-1.1.2/LICENSE.md` & `gameserverlister-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gameserverlister-1.1.2/PKG-INFO` & `gameserverlister-2.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: GameserverLister
-Version: 1.1.2
+Version: 2.0.0
 Summary: Python command line tool to retrieve game server lists for various games
 Home-page: https://github.com/cetteup/GameserverLister
 Author: cetteup
 Author-email: me@cetteup.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cetteup/GameserverLister/issues
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Internet
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: gevent==23.9.0.post1
+Requires-Dist: gevent==24.2.1
 Requires-Dist: nslookup==1.7.0
 Requires-Dist: requests[socks]==2.31.0
 Requires-Dist: pyq3serverlist==0.3.2
 Requires-Dist: pyut2serverlist==0.2.0
 Requires-Dist: pyvpsq==0.1.2
 Requires-Dist: click==8.1.7
 
@@ -90,89 +90,88 @@
 
 The server list retrieval for GameSpy-games requires an external tool. In order to retrieve GameSpy servers, you need to set up [gslist](http://aluigi.altervista.org/papers.htm#gslist). `gslist` was developed by Luigi Auriemma.
 
 ## Supported games
 
 The scripts support retrieval for following games from the listed sources. If you know more sources for any of the listed games or know other games that support the listed protocols, please create an issue, and I will add them.
 
-| Game                                   | Source type/protocol | Server list source(s)                                                                                             |
-|----------------------------------------|----------------------|-------------------------------------------------------------------------------------------------------------------|
-| 7 Days to Die                          | Valve                | Valve ¹                                                                                                           |
-| America's Army: Proving Grounds        | Valve                | Valve ¹                                                                                                           |
-| ARK: Survival Evolved                  | Valve                | Valve ¹                                                                                                           |
-| Arma 2                                 | Valve                | Valve ¹                                                                                                           |
-| Arma 3                                 | Valve                | Valve ¹                                                                                                           |
-| Battlefield 1942                       | GameSpy              | bf1942.org, openspy.net, qtracker.com                                                                             |
-| Battlefield Vietnam                    | GameSpy              | openspy.net, qtracker.com                                                                                         |
-| Battlefield 2                          | GamsSpy              | bf2hub.com, playbf2.ru                                                                                            |
-| Battlefield 2142                       | GameSpy              | novgames.ru, openspy.net, play2142.ru                                                                             |
-| Battlefield: Bad Company 2             | fesl/theater         | Project Rome (emulatornexus.com)                                                                                  |
-| Battlefield 3                          | Battlelog            | battlelog.com                                                                                                     |
-| Battlefield 4                          | Battlelog            | battlelog.com                                                                                                     |
-| Battlefield Hardline                   | Battlelog            | battlelog.com                                                                                                     |
-| Battlefield 1                          | Gametools API        | api.gametools.network                                                                                             |
-| Battlefield 5                          | Gametools API        | api.gametools.network                                                                                             |
-| Call of Duty                           | Quake3               | Activision                                                                                                        |
-| Call of Duty: United Offensive         | Quake3               | Activision                                                                                                        |
-| Call of Duty 2                         | Quake3               | Activision                                                                                                        |
-| Call of Duty 4: Modern Warfare         | Quake3               | Activision                                                                                                        |
-| CoD4x Mod                              | Quake3               | cod4x.ovh                                                                                                         |
-| Counter Strike                         | Valve                | Valve ¹                                                                                                           |
-| Counter Strike: Condition Zero         | Valve                | Valve ¹                                                                                                           |
-| Counter Strike: Source                 | Valve                | Valve ¹                                                                                                           |
-| Counter Strike: Global Offensive       | Valve                | Valve ¹                                                                                                           |
-| Crysis                                 | GameSpy              | crymp.net                                                                                                         |
-| Crysis Wars                            | GameSpy              | jedi95.us                                                                                                         |
-| Day of Defeat                          | Valve                | Valve ¹                                                                                                           |
-| Day of Defeat: Source                  | Valve                | Valve ¹                                                                                                           |
-| DayZ                                   | Valve                | Valve ¹                                                                                                           |
-| DayZ (Arma 2 mod)                      | Valve                | Valve ¹                                                                                                           |
-| Deus Ex                                | GameSpy              | 333networks.com, errorist.eu, newbiesplayground.net, oldunreal.com                                                |
-| Duke Nukem Forever                     | GameSpy              | 333networks.com                                                                                                   |
-| Forgotten Hope 2                       | GameSpy              | fh2.dev                                                                                                           |
-| Garry's Mod                            | Valve                | Valve ¹                                                                                                           |
-| Insurgency                             | Valve                | Valve ¹                                                                                                           |
-| Insurgency: Sandstorm                  | Valve                | Valve ¹                                                                                                           |
-| James Bond 007: Nightfire              | GameSpy              | openspy.net, nightfirepc.com                                                                                      |
-| Left 4 Dead                            | Valve                | Valve ¹                                                                                                           |
-| Left 4 Dead 2                          | Valve                | Valve ¹                                                                                                           |
-| Medal of Honor Warfighter              | Battlelog            | battlelog.com                                                                                                     |
-| Nexuiz                                 | Quake3               | deathmask.net                                                                                                     |
-| OpenArena                              | Quake3               | deathmask.net                                                                                                     |
-| ParaWorld                              | GameSpy              | openspy.net                                                                                                       |
-| Postal 2                               | GameSpy              | 333networks.com                                                                                                   |
-| Q3Rally                                | Quake3               | deathmask.net                                                                                                     |
-| Quake                                  | Quake3               | deathmask.net                                                                                                     |
-| Quake 3 Arena                          | Quake3               | quake3arena.com, urbanterror.info, excessiveplus.net, ioquake3.org, huxxer.de, maverickservers.com, deathmask.net |
-| Return to Castle Wolfenstein           | Quake3               | id Software                                                                                                       |
-| Rising Storm 2: Vietnam                | Valve                | Valve ¹                                                                                                           |
-| Rune                                   | GameSpy              | 333networks.com, errorist.eu, newbiesplayground.net, oldunreal.com                                                |
-| Rust                                   | Valve                | Valve ¹                                                                                                           |
-| Serious Sam: The First Encounter       | GameSpy              | 333networks.com, errorist.eu, newbiesplayground.net, oldunreal.com                                                |
-| Serious Sam: Second Encounter          | GameSpy              | 333networks.com, errorist.eu, newbiesplayground.net, oldunreal.com                                                |
-| Soldier of Fortune II: Double Helix    | Quake3               | Raven Software                                                                                                    |
-| Squad                                  | Valve                | Valve ¹                                                                                                           |
-| Star Wars Jedi Knight II: Jedi Outcast | Quake3               | Raven Software, jkhub.org                                                                                         |
-| Star Wars Jedi Knight: Jedi Academy    | Quake3               | Raven Software, jkhub.org                                                                                         |
-| SWAT 4                                 | GameSpy              | swat4stats.com                                                                                                    |
-| Team Fortress Classic                  | Valve                | Valve ¹                                                                                                           |
-| Team Fortress 2                        | Valve                | Valve ¹                                                                                                           |
-| Tremulous                              | Quake3               | tremulous.net                                                                                                     |
-| Unreal                                 | GameSpy              | 333networks.com, errorist.eu, openspy.net, oldunreal.com, qtracker.com                                            |
-| Unreal Tournament                      | GameSpy              | 333networks.com, errorist.eu, openspy.net, oldunreal.com, qtracker.com                                            |
-| Unreal Tournament 2003                 | Unreal2              | openspy.net                                                                                                       |
-| Unreal Tournament 2004                 | Unreal2              | openspy.net, 333networks.com, errorist.eu                                                                         |
-| Unreal Tournament 3                    | GameSpy              | openspy.net                                                                                                       |
-| UrbanTerror                            | Quake3               | FrozenSand                                                                                                        |
-| Vietcong                               | GameSpy              | vietcong.tk, vietcong1.eu, qtracker.com                                                                           |
-| Vietcong 2                             | GameSpy              | openspy.net                                                                                                       |
-| Warfork                                | Quake3               | deathmask.net                                                                                                     |
-| Warsow                                 | Quake3               | deathmask.net                                                                                                     |
-| Wheel of Time                          | GameSpy              | 333networks.com, errorist.eu, newbiesplayground.net, oldunreal.com                                                |
-| Wolfenstein: Enemy Territory           | Quake3               | id Software, etlegacy.com                                                                                         |
-| Xonotic                                | Quake3               | deathmask.net, tchr.no                                                                                            |
+| Game                                   | Platforms                        | Source type/protocol | Server list source(s)                                                                                             |
+|----------------------------------------|----------------------------------|----------------------|-------------------------------------------------------------------------------------------------------------------|
+| 7 Days to Die                          | PC                               | Valve                | Valve ¹                                                                                                           |
+| America's Army: Proving Grounds        | PC                               | Valve                | Valve ¹                                                                                                           |
+| ARK: Survival Evolved                  | PC                               | Valve                | Valve ¹                                                                                                           |
+| Arma 2                                 | PC                               | Valve                | Valve ¹                                                                                                           |
+| Arma 3                                 | PC                               | Valve                | Valve ¹                                                                                                           |
+| Battlefield 1942                       | PC                               | GameSpy              | bf1942.org, openspy.net, qtracker.com                                                                             |
+| Battlefield Vietnam                    | PC                               | GameSpy              | openspy.net, qtracker.com                                                                                         |
+| Battlefield 2                          | PC                               | GamsSpy              | bf2hub.com, playbf2.ru                                                                                            |
+| Battlefield 2142                       | PC                               | GameSpy              | novgames.ru, openspy.net, play2142.ru                                                                             |
+| Battlefield: Bad Company 2             | PC                               | fesl/theater         | Project Rome (emulatornexus.com)                                                                                  |
+| Battlefield 3                          | PC                               | Battlelog            | battlelog.com                                                                                                     |
+| Battlefield 4                          | PC, PS3, PS4, Xbox 360, Xbox One | Battlelog            | battlelog.com                                                                                                     |
+| Battlefield Hardline                   | PC, PS3, PS4, Xbox 360, Xbox One | Battlelog            | battlelog.com                                                                                                     |
+| Battlefield 1                          | PC                               | Gametools API        | api.gametools.network                                                                                             |
+| Battlefield 5                          | PC                               | Gametools API        | api.gametools.network                                                                                             |
+| Call of Duty                           | PC                               | Quake3               | Activision                                                                                                        |
+| Call of Duty: United Offensive         | PC                               | Quake3               | Activision                                                                                                        |
+| Call of Duty 2                         | PC                               | Quake3               | Activision                                                                                                        |
+| Call of Duty 4: Modern Warfare         | PC                               | Quake3               | Activision                                                                                                        |
+| CoD4x Mod                              | PC                               | Quake3               | cod4x.ovh                                                                                                         |
+| Counter Strike                         | PC                               | Valve                | Valve ¹                                                                                                           |
+| Counter Strike: Condition Zero         | PC                               | Valve                | Valve ¹                                                                                                           |
+| Counter Strike: Source                 | PC                               | Valve                | Valve ¹                                                                                                           |
+| Counter Strike: Global Offensive       | PC                               | Valve                | Valve ¹                                                                                                           |
+| Crysis                                 | PC                               | GameSpy              | crymp.net                                                                                                         |
+| Crysis Wars                            | PC                               | GameSpy              | jedi95.us                                                                                                         |
+| Day of Defeat                          | PC                               | Valve                | Valve ¹                                                                                                           |
+| Day of Defeat: Source                  | PC                               | Valve                | Valve ¹                                                                                                           |
+| DayZ                                   | PC                               | Valve                | Valve ¹                                                                                                           |
+| DayZ (Arma 2 mod)                      | PC                               | Valve                | Valve ¹                                                                                                           |
+| Deus Ex                                | PC                               | GameSpy              | 333networks.com, errorist.eu, newbiesplayground.net, oldunreal.com                                                |
+| Duke Nukem Forever                     | PC                               | GameSpy              | 333networks.com                                                                                                   |
+| Forgotten Hope 2                       | PC                               | GameSpy              | fh2.dev                                                                                                           |
+| Garry's Mod                            | PC                               | Valve                | Valve ¹                                                                                                           |
+| Insurgency                             | PC                               | Valve                | Valve ¹                                                                                                           |
+| Insurgency: Sandstorm                  | PC                               | Valve                | Valve ¹                                                                                                           |
+| James Bond 007: Nightfire              | PC                               | GameSpy              | openspy.net, nightfirepc.com                                                                                      |
+| Left 4 Dead                            | PC                               | Valve                | Valve ¹                                                                                                           |
+| Left 4 Dead 2                          | PC                               | Valve                | Valve ¹                                                                                                           |
+| Nexuiz                                 | PC                               | Quake3               | deathmask.net                                                                                                     |
+| OpenArena                              | PC                               | Quake3               | deathmask.net                                                                                                     |
+| ParaWorld                              | PC                               | GameSpy              | openspy.net                                                                                                       |
+| Postal 2                               | PC                               | GameSpy              | 333networks.com                                                                                                   |
+| Q3Rally                                | PC                               | Quake3               | deathmask.net                                                                                                     |
+| Quake                                  | PC                               | Quake3               | deathmask.net                                                                                                     |
+| Quake 3 Arena                          | PC                               | Quake3               | quake3arena.com, urbanterror.info, excessiveplus.net, ioquake3.org, huxxer.de, maverickservers.com, deathmask.net |
+| Return to Castle Wolfenstein           | PC                               | Quake3               | id Software                                                                                                       |
+| Rising Storm 2: Vietnam                | PC                               | Valve                | Valve ¹                                                                                                           |
+| Rune                                   | PC                               | GameSpy              | 333networks.com, errorist.eu, newbiesplayground.net, oldunreal.com                                                |
+| Rust                                   | PC                               | Valve                | Valve ¹                                                                                                           |
+| Serious Sam: The First Encounter       | PC                               | GameSpy              | 333networks.com, errorist.eu, newbiesplayground.net, oldunreal.com                                                |
+| Serious Sam: Second Encounter          | PC                               | GameSpy              | 333networks.com, errorist.eu, newbiesplayground.net, oldunreal.com                                                |
+| Soldier of Fortune II: Double Helix    | PC                               | Quake3               | Raven Software                                                                                                    |
+| Squad                                  | PC                               | Valve                | Valve ¹                                                                                                           |
+| Star Wars Jedi Knight II: Jedi Outcast | PC                               | Quake3               | Raven Software, jkhub.org                                                                                         |
+| Star Wars Jedi Knight: Jedi Academy    | PC                               | Quake3               | Raven Software, jkhub.org                                                                                         |
+| SWAT 4                                 | PC                               | GameSpy              | swat4stats.com                                                                                                    |
+| Team Fortress Classic                  | PC                               | Valve                | Valve ¹                                                                                                           |
+| Team Fortress 2                        | PC                               | Valve                | Valve ¹                                                                                                           |
+| Tremulous                              | PC                               | Quake3               | tremulous.net                                                                                                     |
+| Unreal                                 | PC                               | GameSpy              | 333networks.com, errorist.eu, openspy.net, oldunreal.com, qtracker.com                                            |
+| Unreal Tournament                      | PC                               | GameSpy              | 333networks.com, errorist.eu, openspy.net, oldunreal.com, qtracker.com                                            |
+| Unreal Tournament 2003                 | PC                               | Unreal2              | openspy.net                                                                                                       |
+| Unreal Tournament 2004                 | PC                               | Unreal2              | openspy.net, 333networks.com, errorist.eu                                                                         |
+| Unreal Tournament 3                    | PC                               | GameSpy              | openspy.net                                                                                                       |
+| UrbanTerror                            | PC                               | Quake3               | FrozenSand                                                                                                        |
+| Vietcong                               | PC                               | GameSpy              | vietcong.tk, vietcong1.eu, qtracker.com                                                                           |
+| Vietcong 2                             | PC                               | GameSpy              | openspy.net                                                                                                       |
+| Warfork                                | PC                               | Quake3               | deathmask.net                                                                                                     |
+| Warsow                                 | PC                               | Quake3               | deathmask.net                                                                                                     |
+| Wheel of Time                          | PC                               | GameSpy              | 333networks.com, errorist.eu, newbiesplayground.net, oldunreal.com                                                |
+| Wolfenstein: Enemy Territory           | PC                               | Quake3               | id Software, etlegacy.com                                                                                         |
+| Xonotic                                | PC                               | Quake3               | deathmask.net, tchr.no                                                                                            |
 
 ¹ Valve's principal servers are rate limited. If you do not use additional filters to only retrieve matching servers, you will get blocked/timed out. You can pass filters via the `-f`/`--filter` argument, e.g. use `-f "\dedicated\1\password\0\empty\1\full\1"` to only retrieve dedicated servers without a password which are neither full nor empty. You can find a full list of filter options [here](https://developer.valvesoftware.com/wiki/Master_Server_Query_Protocol#Filter) (the `\appid\` filter is applied automatically). 
 
 ## Game server query ports
 
 After obtaining a server list, you may want request current details directly from the game server via different query protocols. However, only the GameSpy and Quake3 principal servers return the game server's query port. Battlelog and the EA fesl/theater do not provide details about the server's query port. So, the respective scripts attempt to find the query port if run with the `--find-query-port` flag.
```

### Comparing `gameserverlister-1.1.2/setup.cfg` & `gameserverlister-2.0.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [metadata]
 name = GameserverLister
-version = 1.1.2
+version = 2.0.0
 description = Python command line tool to retrieve game server lists for various games
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cetteup/GameserverLister
 project_urls = 
 	Bug Tracker = https://github.com/cetteup/GameserverLister/issues
 author = cetteup
 author_email = me@cetteup.com
 license = MIT
 classifiers = 
-	Development Status :: 4 - Beta
+	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: Other Audience
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: Microsoft :: Windows
@@ -29,15 +29,15 @@
 	Topic :: Games/Entertainment
 	Topic :: Internet
 
 [options]
 packages = find:
 python_requires = >=3.8, <3.12
 install_requires = 
-	gevent==23.9.0.post1
+	gevent==24.2.1
 	nslookup==1.7.0
 	requests[socks]==2.31.0
 	pyq3serverlist==0.3.2
 	pyut2serverlist==0.2.0
 	pyvpsq==0.1.2
 	click==8.1.7
```

