# Comparing `tmp/hellosp-0.2.1.tar.gz` & `tmp/hellosp-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hellosp-0.2.1.tar", last modified: Sat Apr 27 10:46:30 2024, max compression
+gzip compressed data, was "dist/hellosp-0.2.2.tar", last modified: Sat Apr 27 10:49:22 2024, max compression
```

## Comparing `hellosp-0.2.1.tar` & `hellosp-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-04-27 10:46:30.000000 hellosp-0.2.1/
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-04-27 10:46:30.000000 hellosp-0.2.1/hellosp/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     1068 2024-04-27 10:37:47.000000 hellosp-0.2.1/hellosp/cli.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        0 2024-04-27 10:36:24.000000 hellosp-0.2.1/hellosp/__init__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       62 2024-04-27 10:39:53.000000 hellosp-0.2.1/README.md
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-04-27 10:46:30.000000 hellosp-0.2.1/hellosp.egg-info/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        8 2024-04-27 10:46:30.000000 hellosp-0.2.1/hellosp.egg-info/top_level.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-04-27 10:46:30.000000 hellosp-0.2.1/hellosp.egg-info/dependency_links.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       46 2024-04-27 10:46:30.000000 hellosp-0.2.1/hellosp.egg-info/entry_points.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      235 2024-04-27 10:46:30.000000 hellosp-0.2.1/hellosp.egg-info/SOURCES.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      480 2024-04-27 10:46:30.000000 hellosp-0.2.1/hellosp.egg-info/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       37 2024-04-27 09:57:11.000000 hellosp-0.2.1/MANIFEST.in
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-04-27 10:46:30.000000 hellosp-0.2.1/setup.cfg
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      557 2024-04-27 10:46:11.000000 hellosp-0.2.1/setup.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       15 2024-04-27 09:56:54.000000 hellosp-0.2.1/LICENSE.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      480 2024-04-27 10:46:30.000000 hellosp-0.2.1/PKG-INFO
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-04-27 10:49:22.000000 hellosp-0.2.2/
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-04-27 10:49:22.000000 hellosp-0.2.2/hellosp/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     1093 2024-04-27 10:48:49.000000 hellosp-0.2.2/hellosp/cli.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        0 2024-04-27 10:36:24.000000 hellosp-0.2.2/hellosp/__init__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       62 2024-04-27 10:39:53.000000 hellosp-0.2.2/README.md
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-04-27 10:49:22.000000 hellosp-0.2.2/hellosp.egg-info/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        8 2024-04-27 10:49:22.000000 hellosp-0.2.2/hellosp.egg-info/top_level.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-04-27 10:49:22.000000 hellosp-0.2.2/hellosp.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       46 2024-04-27 10:49:22.000000 hellosp-0.2.2/hellosp.egg-info/entry_points.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      235 2024-04-27 10:49:22.000000 hellosp-0.2.2/hellosp.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      480 2024-04-27 10:49:22.000000 hellosp-0.2.2/hellosp.egg-info/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       37 2024-04-27 09:57:11.000000 hellosp-0.2.2/MANIFEST.in
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-04-27 10:49:22.000000 hellosp-0.2.2/setup.cfg
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      557 2024-04-27 10:49:06.000000 hellosp-0.2.2/setup.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       15 2024-04-27 09:56:54.000000 hellosp-0.2.2/LICENSE.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      480 2024-04-27 10:49:22.000000 hellosp-0.2.2/PKG-INFO
```

### Comparing `hellosp-0.2.1/hellosp/cli.py` & `hellosp-0.2.2/hellosp/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     try:
         result = int(a) + int(b)
         print("Sum is ",result)
     except ValueError:
         print("Error: Please provide valid integer arguments.")
 
 def main():
-    if len(argv) == 0:
+    if len(argv) == 1 and argv[0] == "hellosp":
         print("Hello, this is a simple cli tool that adds 2 integers")
     elif len(argv) <2:
         print("Unknown command. Please find the list of commands")
         list_commands()
         exit(1)
     
     command = argv[1]
```

### Comparing `hellosp-0.2.1/setup.py` & `hellosp-0.2.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
 name='hellosp',
-version='0.2.1',
+version='0.2.2',
 author='Shanmuga Priya',
 author_email='shanmugapriya.rs@embedur.com',
 description='This is a simple cli to calculate the sum of 2 numbers',
 long_description=open("README.md").read(),
 packages=find_packages(),
 entry_points={
         "console_scripts": [
```

