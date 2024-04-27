# Comparing `tmp/whatshow_phy_mod_otfs-1.0.1.tar.gz` & `tmp/whatshow_phy_mod_otfs-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatshow_phy_mod_otfs-1.0.1.tar", last modified: Thu Mar 14 04:40:10 2024, max compression
+gzip compressed data, was "whatshow_phy_mod_otfs-2.0.1.tar", last modified: Sat Apr 27 11:29:47 2024, max compression
```

## Comparing `whatshow_phy_mod_otfs-1.0.1.tar` & `whatshow_phy_mod_otfs-2.0.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 04:40:10.227013 whatshow_phy_mod_otfs-1.0.1/
--rw-rw-rw-   0        0        0     3706 2024-03-14 04:40:10.221018 whatshow_phy_mod_otfs-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3595 2024-03-14 04:40:08.000000 whatshow_phy_mod_otfs-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-03-14 04:40:10.227013 whatshow_phy_mod_otfs-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      408 2024-03-14 04:40:08.000000 whatshow_phy_mod_otfs-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-14 04:40:10.207496 whatshow_phy_mod_otfs-1.0.1/whatshow_phy_mod_otfs/
--rw-rw-rw-   0        0        0    24508 2024-03-14 04:40:08.000000 whatshow_phy_mod_otfs-1.0.1/whatshow_phy_mod_otfs/OTFS.py
--rw-rw-rw-   0        0        0       22 2024-03-14 04:40:08.000000 whatshow_phy_mod_otfs-1.0.1/whatshow_phy_mod_otfs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 04:40:10.220015 whatshow_phy_mod_otfs-1.0.1/whatshow_phy_mod_otfs.egg-info/
--rw-rw-rw-   0        0        0     3706 2024-03-14 04:40:09.000000 whatshow_phy_mod_otfs-1.0.1/whatshow_phy_mod_otfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2024-03-14 04:40:09.000000 whatshow_phy_mod_otfs-1.0.1/whatshow_phy_mod_otfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 04:40:09.000000 whatshow_phy_mod_otfs-1.0.1/whatshow_phy_mod_otfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-03-14 04:40:09.000000 whatshow_phy_mod_otfs-1.0.1/whatshow_phy_mod_otfs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-03-14 04:40:09.000000 whatshow_phy_mod_otfs-1.0.1/whatshow_phy_mod_otfs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 11:29:47.860392 whatshow_phy_mod_otfs-2.0.1/
+-rw-rw-rw-   0        0        0    12548 2024-04-27 11:29:47.858391 whatshow_phy_mod_otfs-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    12432 2024-04-27 11:29:47.000000 whatshow_phy_mod_otfs-2.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 11:29:47.860392 whatshow_phy_mod_otfs-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      408 2024-04-27 11:29:47.000000 whatshow_phy_mod_otfs-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:29:47.833670 whatshow_phy_mod_otfs-2.0.1/whatshow_phy_mod_otfs/
+-rw-rw-rw-   0        0        0    19980 2024-04-27 11:29:47.000000 whatshow_phy_mod_otfs-2.0.1/whatshow_phy_mod_otfs/OTFS.py
+-rw-rw-rw-   0        0        0    27830 2024-04-27 11:29:47.000000 whatshow_phy_mod_otfs-2.0.1/whatshow_phy_mod_otfs/OTFSResGrid.py
+-rw-rw-rw-   0        0        0      100 2024-04-27 11:29:47.000000 whatshow_phy_mod_otfs-2.0.1/whatshow_phy_mod_otfs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:29:47.856212 whatshow_phy_mod_otfs-2.0.1/whatshow_phy_mod_otfs.egg-info/
+-rw-rw-rw-   0        0        0    12548 2024-04-27 11:29:47.000000 whatshow_phy_mod_otfs-2.0.1/whatshow_phy_mod_otfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2024-04-27 11:29:47.000000 whatshow_phy_mod_otfs-2.0.1/whatshow_phy_mod_otfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 11:29:47.000000 whatshow_phy_mod_otfs-2.0.1/whatshow_phy_mod_otfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-27 11:29:47.000000 whatshow_phy_mod_otfs-2.0.1/whatshow_phy_mod_otfs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-27 11:29:47.000000 whatshow_phy_mod_otfs-2.0.1/whatshow_phy_mod_otfs.egg-info/top_level.txt
```

