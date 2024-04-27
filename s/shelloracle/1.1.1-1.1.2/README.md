# Comparing `tmp/shelloracle-1.1.1.tar.gz` & `tmp/shelloracle-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shelloracle-1.1.1.tar", last modified: Sat Apr 27 16:30:28 2024, max compression
+gzip compressed data, was "shelloracle-1.1.2.tar", last modified: Sat Apr 27 16:41:36 2024, max compression
```

## Comparing `shelloracle-1.1.1.tar` & `shelloracle-1.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:30:28.201349 shelloracle-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:30:28.197349 shelloracle-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:30:28.197349 shelloracle-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-27 16:30:20.000000 shelloracle-1.1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-27 16:30:20.000000 shelloracle-1.1.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-27 16:30:20.000000 shelloracle-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 16:30:20.000000 shelloracle-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-04-27 16:30:28.201349 shelloracle-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-04-27 16:30:20.000000 shelloracle-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-27 16:30:20.000000 shelloracle-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 16:30:28.201349 shelloracle-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:30:28.197349 shelloracle-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:30:28.197349 shelloracle-1.1.1/src/shelloracle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 16:30:20.000000 shelloracle-1.1.1/src/shelloracle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-27 16:30:20.000000 shelloracle-1.1.1/src/shelloracle/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-27 16:30:20.000000 shelloracle-1.1.1/src/shelloracle/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-04-27 16:30:20.000000 shelloracle-1.1.1/src/shelloracle/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:30:28.201349 shelloracle-1.1.1/src/shelloracle/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-27 16:30:20.000000 shelloracle-1.1.1/src/shelloracle/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-27 16:30:20.000000 shelloracle-1.1.1/src/shelloracle/providers/localai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-27 16:30:20.000000 shelloracle-1.1.1/src/shelloracle/providers/ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-27 16:30:20.000000 shelloracle-1.1.1/src/shelloracle/providers/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:30:28.201349 shelloracle-1.1.1/src/shelloracle/shell/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-27 16:30:20.000000 shelloracle-1.1.1/src/shelloracle/shell/shelloracle.bash
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-27 16:30:20.000000 shelloracle-1.1.1/src/shelloracle/shell/shelloracle.zsh
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-27 16:30:20.000000 shelloracle-1.1.1/src/shelloracle/shelloracle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:30:28.201349 shelloracle-1.1.1/src/shelloracle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-04-27 16:30:28.000000 shelloracle-1.1.1/src/shelloracle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-27 16:30:28.000000 shelloracle-1.1.1/src/shelloracle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:30:28.000000 shelloracle-1.1.1/src/shelloracle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-27 16:30:28.000000 shelloracle-1.1.1/src/shelloracle.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-27 16:30:28.000000 shelloracle-1.1.1/src/shelloracle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-27 16:30:28.000000 shelloracle-1.1.1/src/shelloracle.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:30:28.201349 shelloracle-1.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:30:28.201349 shelloracle-1.1.1/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-27 16:30:20.000000 shelloracle-1.1.1/tests/providers/test_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-27 16:30:20.000000 shelloracle-1.1.1/tests/providers/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-27 16:30:20.000000 shelloracle-1.1.1/tests/test_shelloracle.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-27 16:30:20.000000 shelloracle-1.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:41:36.178812 shelloracle-1.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:41:36.174812 shelloracle-1.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:41:36.174812 shelloracle-1.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-27 16:41:29.000000 shelloracle-1.1.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-27 16:41:29.000000 shelloracle-1.1.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-27 16:41:29.000000 shelloracle-1.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 16:41:29.000000 shelloracle-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-04-27 16:41:36.178812 shelloracle-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-04-27 16:41:29.000000 shelloracle-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-27 16:41:29.000000 shelloracle-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 16:41:36.178812 shelloracle-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:41:36.174812 shelloracle-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:41:36.178812 shelloracle-1.1.2/src/shelloracle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 16:41:29.000000 shelloracle-1.1.2/src/shelloracle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-27 16:41:29.000000 shelloracle-1.1.2/src/shelloracle/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-27 16:41:29.000000 shelloracle-1.1.2/src/shelloracle/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-04-27 16:41:29.000000 shelloracle-1.1.2/src/shelloracle/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:41:36.178812 shelloracle-1.1.2/src/shelloracle/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-27 16:41:29.000000 shelloracle-1.1.2/src/shelloracle/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-27 16:41:29.000000 shelloracle-1.1.2/src/shelloracle/providers/localai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-27 16:41:29.000000 shelloracle-1.1.2/src/shelloracle/providers/ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-27 16:41:29.000000 shelloracle-1.1.2/src/shelloracle/providers/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:41:36.178812 shelloracle-1.1.2/src/shelloracle/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-27 16:41:29.000000 shelloracle-1.1.2/src/shelloracle/shell/shelloracle.bash
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-27 16:41:29.000000 shelloracle-1.1.2/src/shelloracle/shell/shelloracle.zsh
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-27 16:41:29.000000 shelloracle-1.1.2/src/shelloracle/shelloracle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:41:36.178812 shelloracle-1.1.2/src/shelloracle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-04-27 16:41:36.000000 shelloracle-1.1.2/src/shelloracle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-27 16:41:36.000000 shelloracle-1.1.2/src/shelloracle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:41:36.000000 shelloracle-1.1.2/src/shelloracle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-27 16:41:36.000000 shelloracle-1.1.2/src/shelloracle.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-27 16:41:36.000000 shelloracle-1.1.2/src/shelloracle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-27 16:41:36.000000 shelloracle-1.1.2/src/shelloracle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:41:36.178812 shelloracle-1.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:41:36.178812 shelloracle-1.1.2/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-27 16:41:29.000000 shelloracle-1.1.2/tests/providers/test_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-27 16:41:29.000000 shelloracle-1.1.2/tests/providers/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-27 16:41:29.000000 shelloracle-1.1.2/tests/test_shelloracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-27 16:41:29.000000 shelloracle-1.1.2/tox.ini
```

### Comparing `shelloracle-1.1.1/.github/workflows/release.yml` & `shelloracle-1.1.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.1/.github/workflows/tests.yml` & `shelloracle-1.1.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.1/.gitignore` & `shelloracle-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.1/LICENSE` & `shelloracle-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.1/PKG-INFO` & `shelloracle-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shelloracle
-Version: 1.1.1
+Version: 1.1.2
 Summary: ShellOracle is a pluggable terminal utility that takes a natural language description of a command and substitutes it into your terminal buffer.
 Author-email: Daniel Copley <djcopley@proton.me>
 Project-URL: Homepage, https://github.com/djcopley/ShellOracle
 Project-URL: Repository, https://github.com/djcopley/ShellOracle.git
 Project-URL: Issues, https://github.com/djcopley/ShellOracle/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `shelloracle-1.1.1/README.md` & `shelloracle-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.1/pyproject.toml` & `shelloracle-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.1/src/shelloracle/__main__.py` & `shelloracle-1.1.2/src/shelloracle/__main__.py`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.1/src/shelloracle/config.py` & `shelloracle-1.1.2/src/shelloracle/config.py`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.1/src/shelloracle/configure.py` & `shelloracle-1.1.2/src/shelloracle/configure.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import tomlkit
 from prompt_toolkit import print_formatted_text, prompt
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.formatted_text import FormattedText
 from prompt_toolkit.shortcuts import confirm
 
-from .config import Configuration
+from .config import Configuration, data_home
 from .providers import Provider, Setting, list_providers, get_provider
 
 
 class UserError(Exception):
     ...
 
 
@@ -114,15 +114,15 @@
     config.add("provider", provider_table)
 
     provider_configuration_table = tomlkit.table()
     for setting, value in settings.items():
         provider_configuration_table.add(setting, value)
     provider_table.add(provider.name, provider_configuration_table)
 
-    Configuration.filepath.mkdir(exist_ok=True)
+    data_home.mkdir(exist_ok=True)
     with Configuration.filepath.open("w") as config_file:
         tomlkit.dump(config, config_file)
 
 
 def install_keybindings() -> None:
     if not (shells := get_installed_shells()):
         print_warning("Cannot install keybindings: no compatible shells found. "
```

### Comparing `shelloracle-1.1.1/src/shelloracle/providers/__init__.py` & `shelloracle-1.1.2/src/shelloracle/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.1/src/shelloracle/providers/localai.py` & `shelloracle-1.1.2/src/shelloracle/providers/localai.py`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.1/src/shelloracle/providers/ollama.py` & `shelloracle-1.1.2/src/shelloracle/providers/ollama.py`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.1/src/shelloracle/providers/openai.py` & `shelloracle-1.1.2/src/shelloracle/providers/openai.py`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.1/src/shelloracle/shell/shelloracle.bash` & `shelloracle-1.1.2/src/shelloracle/shell/shelloracle.bash`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.1/src/shelloracle/shell/shelloracle.zsh` & `shelloracle-1.1.2/src/shelloracle/shell/shelloracle.zsh`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.1/src/shelloracle/shelloracle.py` & `shelloracle-1.1.2/src/shelloracle/shelloracle.py`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.1/src/shelloracle.egg-info/PKG-INFO` & `shelloracle-1.1.2/src/shelloracle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shelloracle
-Version: 1.1.1
+Version: 1.1.2
 Summary: ShellOracle is a pluggable terminal utility that takes a natural language description of a command and substitutes it into your terminal buffer.
 Author-email: Daniel Copley <djcopley@proton.me>
 Project-URL: Homepage, https://github.com/djcopley/ShellOracle
 Project-URL: Repository, https://github.com/djcopley/ShellOracle.git
 Project-URL: Issues, https://github.com/djcopley/ShellOracle/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `shelloracle-1.1.1/src/shelloracle.egg-info/SOURCES.txt` & `shelloracle-1.1.2/src/shelloracle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.1/tests/test_shelloracle.py` & `shelloracle-1.1.2/tests/test_shelloracle.py`

 * *Files identical despite different names*

