# Comparing `tmp/hellosp-0.1.0.tar.gz` & `tmp/hellosp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hellosp-0.1.0.tar", last modified: Sat Apr 27 09:21:35 2024, max compression
+gzip compressed data, was "dist/hellosp-0.1.1.tar", last modified: Sat Apr 27 09:46:40 2024, max compression
```

## Comparing `hellosp-0.1.0.tar` & `hellosp-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-04-27 09:21:35.000000 hellosp-0.1.0/
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-04-27 09:21:35.000000 hellosp-0.1.0/hellosp.egg-info/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-04-27 09:21:35.000000 hellosp-0.1.0/hellosp.egg-info/top_level.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-04-27 09:21:35.000000 hellosp-0.1.0/hellosp.egg-info/dependency_links.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      132 2024-04-27 09:21:35.000000 hellosp-0.1.0/hellosp.egg-info/SOURCES.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      426 2024-04-27 09:21:35.000000 hellosp-0.1.0/hellosp.egg-info/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-04-27 09:21:35.000000 hellosp-0.1.0/setup.cfg
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      413 2024-04-27 09:19:56.000000 hellosp-0.1.0/setup.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      426 2024-04-27 09:21:35.000000 hellosp-0.1.0/PKG-INFO
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-04-27 09:46:40.000000 hellosp-0.1.1/
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-04-27 09:46:40.000000 hellosp-0.1.1/hellosp.egg-info/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-04-27 09:46:40.000000 hellosp-0.1.1/hellosp.egg-info/top_level.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-04-27 09:46:40.000000 hellosp-0.1.1/hellosp.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      143 2024-04-27 09:46:40.000000 hellosp-0.1.1/hellosp.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      495 2024-04-27 09:46:40.000000 hellosp-0.1.1/hellosp.egg-info/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       76 2024-04-27 09:45:01.000000 hellosp-0.1.1/README.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-04-27 09:46:40.000000 hellosp-0.1.1/setup.cfg
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      457 2024-04-27 09:46:30.000000 hellosp-0.1.1/setup.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      495 2024-04-27 09:46:40.000000 hellosp-0.1.1/PKG-INFO
```

