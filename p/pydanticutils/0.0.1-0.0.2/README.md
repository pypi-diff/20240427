# Comparing `tmp/pydanticutils-0.0.1.tar.gz` & `tmp/pydanticutils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydanticutils-0.0.1.tar", last modified: Fri Apr 26 18:12:06 2024, max compression
+gzip compressed data, was "pydanticutils-0.0.2.tar", last modified: Fri Apr 26 18:48:34 2024, max compression
```

## Comparing `pydanticutils-0.0.1.tar` & `pydanticutils-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-04-26 18:12:06.473602 pydanticutils-0.0.1/
--rw-r--r--   0 alex      (1000) alex      (1001)     1073 2024-04-26 18:10:34.000000 pydanticutils-0.0.1/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1001)       25 2024-04-26 18:10:34.000000 pydanticutils-0.0.1/MANIFEST.in
--rw-r--r--   0 alex      (1000) alex      (1001)     1215 2024-04-26 18:12:06.473602 pydanticutils-0.0.1/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1001)       42 2024-04-26 18:10:34.000000 pydanticutils-0.0.1/README.md
--rw-r--r--   0 alex      (1000) alex      (1001)        6 2024-04-26 18:10:34.000000 pydanticutils-0.0.1/VERSION
--rw-r--r--   0 alex      (1000) alex      (1001)     1422 2024-04-26 18:10:34.000000 pydanticutils-0.0.1/pyproject.toml
--rw-r--r--   0 alex      (1000) alex      (1001)       38 2024-04-26 18:12:06.473602 pydanticutils-0.0.1/setup.cfg
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-04-26 18:12:06.470269 pydanticutils-0.0.1/src/
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-04-26 18:12:06.470269 pydanticutils-0.0.1/src/pydanticutils/
--rw-r--r--   0 alex      (1000) alex      (1001)      115 2024-04-26 18:10:34.000000 pydanticutils-0.0.1/src/pydanticutils/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1001)     1759 2024-04-26 18:10:34.000000 pydanticutils-0.0.1/src/pydanticutils/yaml.py
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-04-26 18:12:06.470269 pydanticutils-0.0.1/src/pydanticutils.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1001)     1215 2024-04-26 18:12:06.000000 pydanticutils-0.0.1/src/pydanticutils.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1001)      312 2024-04-26 18:12:06.000000 pydanticutils-0.0.1/src/pydanticutils.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1001)        1 2024-04-26 18:12:06.000000 pydanticutils-0.0.1/src/pydanticutils.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1001)      271 2024-04-26 18:12:06.000000 pydanticutils-0.0.1/src/pydanticutils.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1001)       14 2024-04-26 18:12:06.000000 pydanticutils-0.0.1/src/pydanticutils.egg-info/top_level.txt
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-04-26 18:48:34.806856 pydanticutils-0.0.2/
+-rw-r--r--   0 alex      (1000) alex      (1001)     1073 2024-04-26 18:10:34.000000 pydanticutils-0.0.2/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1001)       25 2024-04-26 18:10:34.000000 pydanticutils-0.0.2/MANIFEST.in
+-rw-r--r--   0 alex      (1000) alex      (1001)     2256 2024-04-26 18:48:34.806856 pydanticutils-0.0.2/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1001)     1083 2024-04-26 18:47:33.000000 pydanticutils-0.0.2/README.md
+-rw-r--r--   0 alex      (1000) alex      (1001)        6 2024-04-26 18:48:03.000000 pydanticutils-0.0.2/VERSION
+-rw-r--r--   0 alex      (1000) alex      (1001)     1422 2024-04-26 18:10:34.000000 pydanticutils-0.0.2/pyproject.toml
+-rw-r--r--   0 alex      (1000) alex      (1001)       38 2024-04-26 18:48:34.806856 pydanticutils-0.0.2/setup.cfg
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-04-26 18:48:34.803523 pydanticutils-0.0.2/src/
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-04-26 18:48:34.803523 pydanticutils-0.0.2/src/pydanticutils/
+-rw-r--r--   0 alex      (1000) alex      (1001)      115 2024-04-26 18:10:34.000000 pydanticutils-0.0.2/src/pydanticutils/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     1759 2024-04-26 18:10:34.000000 pydanticutils-0.0.2/src/pydanticutils/yaml.py
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-04-26 18:48:34.803523 pydanticutils-0.0.2/src/pydanticutils.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1001)     2256 2024-04-26 18:48:34.000000 pydanticutils-0.0.2/src/pydanticutils.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1001)      312 2024-04-26 18:48:34.000000 pydanticutils-0.0.2/src/pydanticutils.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)        1 2024-04-26 18:48:34.000000 pydanticutils-0.0.2/src/pydanticutils.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)      271 2024-04-26 18:48:34.000000 pydanticutils-0.0.2/src/pydanticutils.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)       14 2024-04-26 18:48:34.000000 pydanticutils-0.0.2/src/pydanticutils.egg-info/top_level.txt
```

### Comparing `pydanticutils-0.0.1/LICENSE` & `pydanticutils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydanticutils-0.0.1/pyproject.toml` & `pydanticutils-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydanticutils-0.0.1/src/pydanticutils/yaml.py` & `pydanticutils-0.0.2/src/pydanticutils/yaml.py`

 * *Files identical despite different names*

