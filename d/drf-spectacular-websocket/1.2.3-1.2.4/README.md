# Comparing `tmp/drf_spectacular_websocket-1.2.3.tar.gz` & `tmp/drf_spectacular_websocket-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_spectacular_websocket-1.2.3.tar", last modified: Fri Apr 26 18:26:14 2024, max compression
+gzip compressed data, was "drf_spectacular_websocket-1.2.4.tar", last modified: Sat Apr 27 08:49:20 2024, max compression
```

## Comparing `drf_spectacular_websocket-1.2.3.tar` & `drf_spectacular_websocket-1.2.4.tar`

### file list

```diff
@@ -1,24 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:26:14.873380 drf_spectacular_websocket-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-26 18:26:11.000000 drf_spectacular_websocket-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-04-26 18:26:14.873380 drf_spectacular_websocket-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-26 18:26:11.000000 drf_spectacular_websocket-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-26 18:26:11.000000 drf_spectacular_websocket-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 18:26:14.873380 drf_spectacular_websocket-1.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:26:14.869380 drf_spectacular_websocket-1.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:26:14.869380 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 18:26:11.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-26 18:26:11.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-26 18:26:11.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:26:14.873380 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 18:26:11.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-04-26 18:26:11.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/schemas/consumer_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-26 18:26:11.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/schemas/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-26 18:26:11.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:26:14.873380 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-04-26 18:26:14.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-26 18:26:14.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 18:26:14.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-26 18:26:14.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 18:26:14.000000 drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:26:14.873380 drf_spectacular_websocket-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-26 18:26:11.000000 drf_spectacular_websocket-1.2.3/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:49:20.009702 drf_spectacular_websocket-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:49:20.001702 drf_spectacular_websocket-1.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:49:20.001702 drf_spectacular_websocket-1.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-04-27 08:49:20.009702 drf_spectacular_websocket-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:49:20.001702 drf_spectacular_websocket-1.2.4/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    66494 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/images/example_receive.png
+-rw-r--r--   0 runner    (1001) docker     (127)    89056 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/images/example_send.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 08:49:20.009702 drf_spectacular_websocket-1.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:49:20.001702 drf_spectacular_websocket-1.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:49:20.005702 drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:49:20.005702 drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket/schemas/consumer_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket/schemas/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:49:20.001702 drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:49:20.005702 drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket/templates/drf_spectacular/
+-rw-r--r--   0 runner    (1001) docker     (127)    20795 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket/templates/drf_spectacular/swagger_ui.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:49:20.005702 drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-04-27 08:49:19.000000 drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-27 08:49:19.000000 drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 08:49:19.000000 drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-27 08:49:19.000000 drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-27 08:49:19.000000 drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-27 08:49:19.000000 drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:49:20.005702 drf_spectacular_websocket-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/tests/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/tests/consumers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/tests/expected_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/tests/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-27 08:49:15.000000 drf_spectacular_websocket-1.2.4/tests/urls.py
```

### Comparing `drf_spectacular_websocket-1.2.3/LICENSE` & `drf_spectacular_websocket-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.3/PKG-INFO` & `drf_spectacular_websocket-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf_spectacular_websocket
-Version: 1.2.3
+Version: 1.2.4
 Summary: Extend websocket schema decorator for Django Channels
 Author-email: Friskes <friskesx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Friskes
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `drf_spectacular_websocket-1.2.3/README.md` & `drf_spectacular_websocket-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.3/pyproject.toml` & `drf_spectacular_websocket-1.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [project]
 name = "drf_spectacular_websocket"
 # https://packaging.python.org/en/latest/guides/writing-pyproject-toml/#version
 # https://packaging.python.org/en/latest/guides/single-sourcing-package-version/#single-sourcing-the-version
-version = "1.2.3"
+# version = "1.2.3"
+dynamic = ["version"]
 license = {file = "LICENSE"}
 authors = [
   {name="Friskes", email="friskesx@gmail.com"},
 ]
 description = "Extend websocket schema decorator for Django Channels"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -57,18 +58,30 @@
 [project.urls]
 "Homepage" = "https://github.com/Friskes/drf-spectacular-websocket"
 "Bug Reports" = "https://github.com/Friskes/drf-spectacular-websocket/issues"
 "Source" = "https://github.com/Friskes/drf-spectacular-websocket/"
 
 
 [build-system]
-requires = ["setuptools"]
+requires = ["setuptools>=64", "setuptools_scm[toml]>=8"]
 build-backend = "setuptools.build_meta"
 
 
+[tool.setuptools_scm]
+# Empty is fine
+
+
+[project.entry-points."setuptools.finalize_distribution_options"]
+setuptools_scm = "setuptools_scm._integration.setuptools:infer_version"
+
+
+# [tool.setuptools.dynamic]
+# version = {attr = "src.drf_spectacular_websocket.__version__"}
+
+
 # https://setuptools.pypa.io/en/latest/userguide/datafiles.html
 # https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/#package-data
 # Данная настройка позволяет заменить MANIFEST.in файл для добавления дополнительных файлов в пакет
 [tool.setuptools.package-data]
 "drf_spectacular_websocket" = ["drf_spectacular_websocket/templates/swagger_ui.js"]
```

### Comparing `drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/decorators.py` & `drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket/decorators.py`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/schemas/consumer_schema.py` & `drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket/schemas/consumer_schema.py`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/schemas/schema.py` & `drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket/schemas/schema.py`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket/settings.py` & `drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket/settings.py`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.3/src/drf_spectacular_websocket.egg-info/PKG-INFO` & `drf_spectacular_websocket-1.2.4/src/drf_spectacular_websocket.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf_spectacular_websocket
-Version: 1.2.3
+Version: 1.2.4
 Summary: Extend websocket schema decorator for Django Channels
 Author-email: Friskes <friskesx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Friskes
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

