# Comparing `tmp/hellosp-0.1.1.tar.gz` & `tmp/hellosp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hellosp-0.1.1.tar", last modified: Sat Apr 27 09:46:40 2024, max compression
+gzip compressed data, was "dist/hellosp-0.1.2.tar", last modified: Sat Apr 27 09:59:26 2024, max compression
```

## Comparing `hellosp-0.1.1.tar` & `hellosp-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,15 @@
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-04-27 09:46:40.000000 hellosp-0.1.1/
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-04-27 09:46:40.000000 hellosp-0.1.1/hellosp.egg-info/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-04-27 09:46:40.000000 hellosp-0.1.1/hellosp.egg-info/top_level.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-04-27 09:46:40.000000 hellosp-0.1.1/hellosp.egg-info/dependency_links.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      143 2024-04-27 09:46:40.000000 hellosp-0.1.1/hellosp.egg-info/SOURCES.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      495 2024-04-27 09:46:40.000000 hellosp-0.1.1/hellosp.egg-info/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       76 2024-04-27 09:45:01.000000 hellosp-0.1.1/README.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-04-27 09:46:40.000000 hellosp-0.1.1/setup.cfg
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      457 2024-04-27 09:46:30.000000 hellosp-0.1.1/setup.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      495 2024-04-27 09:46:40.000000 hellosp-0.1.1/PKG-INFO
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-04-27 09:59:26.000000 hellosp-0.1.2/
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-04-27 09:59:26.000000 hellosp-0.1.2/hellosp/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       24 2024-04-27 09:55:45.000000 hellosp-0.1.2/hellosp/__init__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      106 2024-04-27 09:55:51.000000 hellosp-0.1.2/hellosp/hello.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       76 2024-04-27 09:45:01.000000 hellosp-0.1.2/README.md
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-04-27 09:59:26.000000 hellosp-0.1.2/hellosp.egg-info/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        8 2024-04-27 09:59:26.000000 hellosp-0.1.2/hellosp.egg-info/top_level.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-04-27 09:59:26.000000 hellosp-0.1.2/hellosp.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      203 2024-04-27 09:59:26.000000 hellosp-0.1.2/hellosp.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      495 2024-04-27 09:59:26.000000 hellosp-0.1.2/hellosp.egg-info/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       37 2024-04-27 09:57:11.000000 hellosp-0.1.2/MANIFEST.in
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-04-27 09:59:26.000000 hellosp-0.1.2/setup.cfg
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      456 2024-04-27 09:57:42.000000 hellosp-0.1.2/setup.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       15 2024-04-27 09:56:54.000000 hellosp-0.1.2/LICENSE.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      495 2024-04-27 09:59:26.000000 hellosp-0.1.2/PKG-INFO
```

