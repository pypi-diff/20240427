# Comparing `tmp/mergoo-0.0.7.tar.gz` & `tmp/mergoo-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mergoo-0.0.7.tar", last modified: Sat Apr 13 19:04:46 2024, max compression
+gzip compressed data, was "mergoo-0.0.8.tar", last modified: Sat Apr 27 21:50:51 2024, max compression
```

## Comparing `mergoo-0.0.7.tar` & `mergoo-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,24 @@
-drwxrwxr-x   0 alirezamsh  (1000) alirezamsh  (1000)        0 2024-04-13 19:04:46.463332 mergoo-0.0.7/
--rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)     7651 2024-04-13 18:59:15.000000 mergoo-0.0.7/LICENSE
--rw-r--r--   0 alirezamsh  (1000) alirezamsh  (1000)     9732 2024-04-13 19:04:46.463332 mergoo-0.0.7/PKG-INFO
-drwxrwxr-x   0 alirezamsh  (1000) alirezamsh  (1000)        0 2024-04-13 19:04:46.463332 mergoo-0.0.7/mergoo/
--rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)     1412 2024-04-13 18:59:15.000000 mergoo-0.0.7/mergoo/compose_experts.py
--rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)     9272 2024-04-13 18:59:15.000000 mergoo-0.0.7/mergoo/compose_layers.py
--rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)     9649 2024-04-13 18:59:15.000000 mergoo-0.0.7/mergoo/safe_saving.py
-drwxrwxr-x   0 alirezamsh  (1000) alirezamsh  (1000)        0 2024-04-13 19:04:46.463332 mergoo-0.0.7/mergoo.egg-info/
--rw-r--r--   0 alirezamsh  (1000) alirezamsh  (1000)     9732 2024-04-13 19:04:46.000000 mergoo-0.0.7/mergoo.egg-info/PKG-INFO
--rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)      244 2024-04-13 19:04:46.000000 mergoo-0.0.7/mergoo.egg-info/SOURCES.txt
--rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)        1 2024-04-13 19:04:46.000000 mergoo-0.0.7/mergoo.egg-info/dependency_links.txt
--rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)      163 2024-04-13 19:04:46.000000 mergoo-0.0.7/mergoo.egg-info/requires.txt
--rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)        7 2024-04-13 19:04:46.000000 mergoo-0.0.7/mergoo.egg-info/top_level.txt
--rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)      978 2024-04-13 19:00:36.000000 mergoo-0.0.7/pyproject.toml
--rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)       38 2024-04-13 19:04:46.463332 mergoo-0.0.7/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-27 21:50:51.696316 mergoo-0.0.8/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7651 2024-04-27 21:28:42.000000 mergoo-0.0.8/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9732 2024-04-27 21:50:51.696316 mergoo-0.0.8/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-27 21:50:51.696316 mergoo-0.0.8/mergoo/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1412 2024-04-27 21:28:42.000000 mergoo-0.0.8/mergoo/compose_experts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9272 2024-04-27 21:28:42.000000 mergoo-0.0.8/mergoo/compose_layers.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-27 21:50:51.696316 mergoo-0.0.8/mergoo/composers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-27 21:28:42.000000 mergoo-0.0.8/mergoo/composers/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7253 2024-04-27 21:28:42.000000 mergoo-0.0.8/mergoo/composers/composer_lora_moe.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8279 2024-04-27 21:28:42.000000 mergoo-0.0.8/mergoo/composers/composer_moe.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-27 21:50:51.696316 mergoo-0.0.8/mergoo/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-27 21:28:42.000000 mergoo-0.0.8/mergoo/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    85074 2024-04-27 21:28:42.000000 mergoo-0.0.8/mergoo/models/modeling_bert.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    71732 2024-04-27 21:28:42.000000 mergoo-0.0.8/mergoo/models/modeling_llama.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    64002 2024-04-27 21:28:42.000000 mergoo-0.0.8/mergoo/models/modeling_mistral.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9649 2024-04-27 21:28:42.000000 mergoo-0.0.8/mergoo/safe_saving.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-27 21:50:51.696316 mergoo-0.0.8/mergoo.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9732 2024-04-27 21:50:51.000000 mergoo-0.0.8/mergoo.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      467 2024-04-27 21:50:51.000000 mergoo-0.0.8/mergoo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-27 21:50:51.000000 mergoo-0.0.8/mergoo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      163 2024-04-27 21:50:51.000000 mergoo-0.0.8/mergoo.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2024-04-27 21:50:51.000000 mergoo-0.0.8/mergoo.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1013 2024-04-27 21:50:32.000000 mergoo-0.0.8/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-27 21:50:51.696316 mergoo-0.0.8/setup.cfg
```

### Comparing `mergoo-0.0.7/LICENSE` & `mergoo-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mergoo-0.0.7/PKG-INFO` & `mergoo-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mergoo
-Version: 0.0.7
+Version: 0.0.8
 Summary: Impelementation of Leeroo LLM composer.
 Author-email: Leeroo Team <support@leeroo.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `mergoo-0.0.7/mergoo/compose_experts.py` & `mergoo-0.0.8/mergoo/compose_experts.py`

 * *Files identical despite different names*

### Comparing `mergoo-0.0.7/mergoo/compose_layers.py` & `mergoo-0.0.8/mergoo/compose_layers.py`

 * *Files identical despite different names*

### Comparing `mergoo-0.0.7/mergoo/safe_saving.py` & `mergoo-0.0.8/mergoo/safe_saving.py`

 * *Files identical despite different names*

### Comparing `mergoo-0.0.7/mergoo.egg-info/PKG-INFO` & `mergoo-0.0.8/mergoo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mergoo
-Version: 0.0.7
+Version: 0.0.8
 Summary: Impelementation of Leeroo LLM composer.
 Author-email: Leeroo Team <support@leeroo.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `mergoo-0.0.7/pyproject.toml` & `mergoo-0.0.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mergoo"
-version = "0.0.7"
+version = "0.0.8"
 description = "Impelementation of Leeroo LLM composer."
 authors = [{ name = "Leeroo Team", email = "support@leeroo.com" }]
 readme = "README.md"
 keywords = ["LLM", "compose", "MoE", "router", "mixture-of-adapters", "merge"]
 license = {file = "LICENSE"}
 dependencies = [
     "torch>=2.0.0",
@@ -33,10 +33,8 @@
 python_version = "3.10"
 strict = false
 
 [project.optional-dependencies]
 dev = ["super-lint"]
 
 [tool.setuptools]
-packages = ["mergoo"]
-
-
+packages = ["mergoo", "mergoo.composers", "mergoo.models"]
```

