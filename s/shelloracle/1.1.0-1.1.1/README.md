# Comparing `tmp/shelloracle-1.1.0.tar.gz` & `tmp/shelloracle-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shelloracle-1.1.0.tar", last modified: Tue Feb 13 23:27:51 2024, max compression
+gzip compressed data, was "shelloracle-1.1.1.tar", last modified: Sat Apr 27 16:30:28 2024, max compression
```

## Comparing `shelloracle-1.1.0.tar` & `shelloracle-1.1.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 23:27:51.832438 shelloracle-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 23:27:51.824437 shelloracle-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 23:27:51.828437 shelloracle-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-02-13 23:27:44.000000 shelloracle-1.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-02-13 23:27:44.000000 shelloracle-1.1.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-02-13 23:27:44.000000 shelloracle-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-13 23:27:44.000000 shelloracle-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-02-13 23:27:51.832438 shelloracle-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-02-13 23:27:44.000000 shelloracle-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-02-13 23:27:44.000000 shelloracle-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 23:27:51.832438 shelloracle-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 23:27:51.824437 shelloracle-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 23:27:51.828437 shelloracle-1.1.0/src/shelloracle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 23:27:44.000000 shelloracle-1.1.0/src/shelloracle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-02-13 23:27:44.000000 shelloracle-1.1.0/src/shelloracle/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-02-13 23:27:44.000000 shelloracle-1.1.0/src/shelloracle/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-02-13 23:27:44.000000 shelloracle-1.1.0/src/shelloracle/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 23:27:51.828437 shelloracle-1.1.0/src/shelloracle/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-02-13 23:27:44.000000 shelloracle-1.1.0/src/shelloracle/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-02-13 23:27:44.000000 shelloracle-1.1.0/src/shelloracle/providers/localai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-02-13 23:27:44.000000 shelloracle-1.1.0/src/shelloracle/providers/ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-02-13 23:27:44.000000 shelloracle-1.1.0/src/shelloracle/providers/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 23:27:51.828437 shelloracle-1.1.0/src/shelloracle/shell/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-13 23:27:44.000000 shelloracle-1.1.0/src/shelloracle/shell/shelloracle.bash
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-02-13 23:27:44.000000 shelloracle-1.1.0/src/shelloracle/shell/shelloracle.zsh
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-02-13 23:27:44.000000 shelloracle-1.1.0/src/shelloracle/shelloracle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 23:27:51.832438 shelloracle-1.1.0/src/shelloracle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-02-13 23:27:51.000000 shelloracle-1.1.0/src/shelloracle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-02-13 23:27:51.000000 shelloracle-1.1.0/src/shelloracle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 23:27:51.000000 shelloracle-1.1.0/src/shelloracle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-13 23:27:51.000000 shelloracle-1.1.0/src/shelloracle.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-13 23:27:51.000000 shelloracle-1.1.0/src/shelloracle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-13 23:27:51.000000 shelloracle-1.1.0/src/shelloracle.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 23:27:51.828437 shelloracle-1.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 23:27:51.832438 shelloracle-1.1.0/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-13 23:27:44.000000 shelloracle-1.1.0/tests/providers/test_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-13 23:27:44.000000 shelloracle-1.1.0/tests/providers/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-02-13 23:27:44.000000 shelloracle-1.1.0/tests/test_shelloracle.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-02-13 23:27:44.000000 shelloracle-1.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:30:28.201349 shelloracle-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:30:28.197349 shelloracle-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:30:28.197349 shelloracle-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-27 16:30:20.000000 shelloracle-1.1.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-27 16:30:20.000000 shelloracle-1.1.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-27 16:30:20.000000 shelloracle-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 16:30:20.000000 shelloracle-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-04-27 16:30:28.201349 shelloracle-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-04-27 16:30:20.000000 shelloracle-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-27 16:30:20.000000 shelloracle-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 16:30:28.201349 shelloracle-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:30:28.197349 shelloracle-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:30:28.197349 shelloracle-1.1.1/src/shelloracle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 16:30:20.000000 shelloracle-1.1.1/src/shelloracle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-27 16:30:20.000000 shelloracle-1.1.1/src/shelloracle/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-27 16:30:20.000000 shelloracle-1.1.1/src/shelloracle/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-04-27 16:30:20.000000 shelloracle-1.1.1/src/shelloracle/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:30:28.201349 shelloracle-1.1.1/src/shelloracle/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-27 16:30:20.000000 shelloracle-1.1.1/src/shelloracle/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-27 16:30:20.000000 shelloracle-1.1.1/src/shelloracle/providers/localai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-27 16:30:20.000000 shelloracle-1.1.1/src/shelloracle/providers/ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-27 16:30:20.000000 shelloracle-1.1.1/src/shelloracle/providers/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:30:28.201349 shelloracle-1.1.1/src/shelloracle/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-27 16:30:20.000000 shelloracle-1.1.1/src/shelloracle/shell/shelloracle.bash
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-27 16:30:20.000000 shelloracle-1.1.1/src/shelloracle/shell/shelloracle.zsh
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-27 16:30:20.000000 shelloracle-1.1.1/src/shelloracle/shelloracle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:30:28.201349 shelloracle-1.1.1/src/shelloracle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-04-27 16:30:28.000000 shelloracle-1.1.1/src/shelloracle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-27 16:30:28.000000 shelloracle-1.1.1/src/shelloracle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:30:28.000000 shelloracle-1.1.1/src/shelloracle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-27 16:30:28.000000 shelloracle-1.1.1/src/shelloracle.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-27 16:30:28.000000 shelloracle-1.1.1/src/shelloracle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-27 16:30:28.000000 shelloracle-1.1.1/src/shelloracle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:30:28.201349 shelloracle-1.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:30:28.201349 shelloracle-1.1.1/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-27 16:30:20.000000 shelloracle-1.1.1/tests/providers/test_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-27 16:30:20.000000 shelloracle-1.1.1/tests/providers/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-27 16:30:20.000000 shelloracle-1.1.1/tests/test_shelloracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-27 16:30:20.000000 shelloracle-1.1.1/tox.ini
```

### Comparing `shelloracle-1.1.0/.github/workflows/release.yml` & `shelloracle-1.1.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.0/.github/workflows/tests.yml` & `shelloracle-1.1.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.0/.gitignore` & `shelloracle-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.0/LICENSE` & `shelloracle-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.0/PKG-INFO` & `shelloracle-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shelloracle
-Version: 1.1.0
+Version: 1.1.1
 Summary: ShellOracle is a pluggable terminal utility that takes a natural language description of a command and substitutes it into your terminal buffer.
 Author-email: Daniel Copley <djcopley@proton.me>
 Project-URL: Homepage, https://github.com/djcopley/ShellOracle
 Project-URL: Repository, https://github.com/djcopley/ShellOracle.git
 Project-URL: Issues, https://github.com/djcopley/ShellOracle/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -26,15 +26,15 @@
 Requires-Dist: yaspin
 Requires-Dist: tomlkit
 Requires-Dist: tomli>=1.1.0; python_version < "3.11"
 
 [![Tests](https://github.com/djcopley/ShellOracle/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/djcopley/ShellOracle/actions/workflows/tests.yml)
 [![PyPI version](https://badge.fury.io/py/shelloracle.svg)](https://badge.fury.io/py/shelloracle)
 [![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/shelloracle.svg)](https://pypi.python.org/pypi/shelloracle/)
-[![Downloads](https://static.pepy.tech/badge/shelloracle/month)](https://pepy.tech/project/shelloracle)
+[![Downloads](https://static.pepy.tech/badge/shelloracle)](https://pepy.tech/project/shelloracle)
 
 # ShellOracle
 
 ShellOracle is an innovative terminal utility designed for intelligent shell command generation, bringing a new level of
 efficiency to your command-line interactions. ShellOracle currently supports Ollama, LocalAI, and OpenAI!
 
 ![ShellOracle](https://i.imgur.com/mg1rCzd.gif)
```

### Comparing `shelloracle-1.1.0/README.md` & `shelloracle-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [![Tests](https://github.com/djcopley/ShellOracle/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/djcopley/ShellOracle/actions/workflows/tests.yml)
 [![PyPI version](https://badge.fury.io/py/shelloracle.svg)](https://badge.fury.io/py/shelloracle)
 [![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/shelloracle.svg)](https://pypi.python.org/pypi/shelloracle/)
-[![Downloads](https://static.pepy.tech/badge/shelloracle/month)](https://pepy.tech/project/shelloracle)
+[![Downloads](https://static.pepy.tech/badge/shelloracle)](https://pepy.tech/project/shelloracle)
 
 # ShellOracle
 
 ShellOracle is an innovative terminal utility designed for intelligent shell command generation, bringing a new level of
 efficiency to your command-line interactions. ShellOracle currently supports Ollama, LocalAI, and OpenAI!
 
 ![ShellOracle](https://i.imgur.com/mg1rCzd.gif)
```

### Comparing `shelloracle-1.1.0/pyproject.toml` & `shelloracle-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.0/src/shelloracle/__main__.py` & `shelloracle-1.1.1/src/shelloracle/__main__.py`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.0/src/shelloracle/config.py` & `shelloracle-1.1.1/src/shelloracle/config.py`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.0/src/shelloracle/configure.py` & `shelloracle-1.1.1/src/shelloracle/configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,15 @@
     config.add("provider", provider_table)
 
     provider_configuration_table = tomlkit.table()
     for setting, value in settings.items():
         provider_configuration_table.add(setting, value)
     provider_table.add(provider.name, provider_configuration_table)
 
+    Configuration.filepath.mkdir(exist_ok=True)
     with Configuration.filepath.open("w") as config_file:
         tomlkit.dump(config, config_file)
 
 
 def install_keybindings() -> None:
     if not (shells := get_installed_shells()):
         print_warning("Cannot install keybindings: no compatible shells found. "
```

### Comparing `shelloracle-1.1.0/src/shelloracle/providers/__init__.py` & `shelloracle-1.1.1/src/shelloracle/providers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from ..config import get_config
 
 system_prompt = (
     "Based on the following user description, generate a corresponding Bash command. Focus solely "
     "on interpreting the requirements and translating them into a single, executable Bash command. "
     "Ensure accuracy and relevance to the user's description. The output should be a valid Bash "
     "command that directly aligns with the user's intent, ready for execution in a command-line "
-    "environment. Output nothing except for the command. No code block, no English explanation, "
-    "no start/end tags."
+    "environment. Do not output anything except for the command. No code block, no English explanation, "
+    "no newlines, and no start/end tags."
 )
 
 
 class ProviderError(Exception):
     """LLM providers raise this error to gracefully indicate something has gone wrong."""
```

### Comparing `shelloracle-1.1.0/src/shelloracle/providers/localai.py` & `shelloracle-1.1.1/src/shelloracle/providers/localai.py`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.0/src/shelloracle/providers/ollama.py` & `shelloracle-1.1.1/src/shelloracle/providers/ollama.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 class Ollama(Provider):
     name = "Ollama"
 
     host = Setting(default="localhost")
     port = Setting(default=11434)
-    model = Setting(default="codellama:13b")
+    model = Setting(default="dolphin-mistral")
 
     @property
     def endpoint(self) -> str:
         # computed property because python descriptors need to be bound to an instance before access
         return f"http://{self.host}:{self.port}/api/generate"
 
     async def generate(self, prompt: str) -> AsyncIterator[str]:
```

### Comparing `shelloracle-1.1.0/src/shelloracle/providers/openai.py` & `shelloracle-1.1.1/src/shelloracle/providers/openai.py`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.0/src/shelloracle/shell/shelloracle.bash` & `shelloracle-1.1.1/src/shelloracle/shell/shelloracle.bash`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.0/src/shelloracle/shell/shelloracle.zsh` & `shelloracle-1.1.1/src/shelloracle/shell/shelloracle.zsh`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.0/src/shelloracle/shelloracle.py` & `shelloracle-1.1.1/src/shelloracle/shelloracle.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from __future__ import annotations
 
 import asyncio
 import os
 import sys
 from pathlib import Path
 
-from yaspin import yaspin
-from yaspin.spinners import Spinners
 from prompt_toolkit import PromptSession
 from prompt_toolkit.application import create_app_session_from_tty
 from prompt_toolkit.history import FileHistory
 from prompt_toolkit.patch_stdout import patch_stdout
+from yaspin import yaspin
 
 from .config import get_config
 from .providers import get_provider
 
 
 async def prompt_user(default_prompt: str | None = None) -> str:
     # stdin doesn't exist when running as a zle widget
@@ -58,14 +57,16 @@
     if not (prompt := get_query_from_pipe()):
         default_prompt = os.environ.get("SHOR_DEFAULT_PROMPT")
         prompt = await prompt_user(default_prompt)
 
     shell_command = ""
     with create_app_session_from_tty(), patch_stdout(raw=True), yaspin() as sp:
         async for token in provider.generate(prompt):
+            # some models may erroneously return a newline, which causes issues with the status spinner
+            token = token.replace("\n", "")
             shell_command += token
             sp.text = shell_command
     sys.stdout.write(shell_command)
 
 
 def cli() -> None:
     """Run the ShellOracle command line interface
```

### Comparing `shelloracle-1.1.0/src/shelloracle.egg-info/PKG-INFO` & `shelloracle-1.1.1/src/shelloracle.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shelloracle
-Version: 1.1.0
+Version: 1.1.1
 Summary: ShellOracle is a pluggable terminal utility that takes a natural language description of a command and substitutes it into your terminal buffer.
 Author-email: Daniel Copley <djcopley@proton.me>
 Project-URL: Homepage, https://github.com/djcopley/ShellOracle
 Project-URL: Repository, https://github.com/djcopley/ShellOracle.git
 Project-URL: Issues, https://github.com/djcopley/ShellOracle/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -26,15 +26,15 @@
 Requires-Dist: yaspin
 Requires-Dist: tomlkit
 Requires-Dist: tomli>=1.1.0; python_version < "3.11"
 
 [![Tests](https://github.com/djcopley/ShellOracle/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/djcopley/ShellOracle/actions/workflows/tests.yml)
 [![PyPI version](https://badge.fury.io/py/shelloracle.svg)](https://badge.fury.io/py/shelloracle)
 [![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/shelloracle.svg)](https://pypi.python.org/pypi/shelloracle/)
-[![Downloads](https://static.pepy.tech/badge/shelloracle/month)](https://pepy.tech/project/shelloracle)
+[![Downloads](https://static.pepy.tech/badge/shelloracle)](https://pepy.tech/project/shelloracle)
 
 # ShellOracle
 
 ShellOracle is an innovative terminal utility designed for intelligent shell command generation, bringing a new level of
 efficiency to your command-line interactions. ShellOracle currently supports Ollama, LocalAI, and OpenAI!
 
 ![ShellOracle](https://i.imgur.com/mg1rCzd.gif)
```

### Comparing `shelloracle-1.1.0/src/shelloracle.egg-info/SOURCES.txt` & `shelloracle-1.1.1/src/shelloracle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shelloracle-1.1.0/tests/test_shelloracle.py` & `shelloracle-1.1.1/tests/test_shelloracle.py`

 * *Files identical despite different names*

