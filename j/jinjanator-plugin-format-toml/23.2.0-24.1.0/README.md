# Comparing `tmp/jinjanator_plugin_format_toml-23.2.0.tar.gz` & `tmp/jinjanator_plugin_format_toml-24.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Oct  7 12:04:54 2023, max compression
+gzip compressed data, last modified: Sat Apr 27 15:53:51 2024, max compression
```

## Comparing `jinjanator_plugin_format_toml-23.2.0.tar` & `jinjanator_plugin_format_toml-24.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1286 2023-10-07 12:04:54.000000 jinjanator_plugin_format_toml-23.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     3244 2023-10-07 12:04:54.000000 jinjanator_plugin_format_toml-23.2.0/README.md
--rw-r--r--   0        0        0        0 2023-10-07 12:04:54.000000 jinjanator_plugin_format_toml-23.2.0/src/jinjanator_plugin_format_toml/__init__.py
--rw-r--r--   0        0        0      721 2023-10-07 12:04:54.000000 jinjanator_plugin_format_toml-23.2.0/src/jinjanator_plugin_format_toml/plugin.py
--rw-r--r--   0        0        0        0 2023-10-07 12:04:54.000000 jinjanator_plugin_format_toml-23.2.0/src/jinjanator_plugin_format_toml/py.typed
--rw-r--r--   0        0        0      499 2023-10-07 12:04:54.000000 jinjanator_plugin_format_toml-23.2.0/tests/test_plugin.py
--rw-r--r--   0        0        0       32 2023-10-07 12:04:54.000000 jinjanator_plugin_format_toml-23.2.0/.gitignore
--rw-r--r--   0        0        0    11357 2023-10-07 12:04:54.000000 jinjanator_plugin_format_toml-23.2.0/LICENSE
--rw-r--r--   0        0        0     6677 2023-10-07 12:04:54.000000 jinjanator_plugin_format_toml-23.2.0/pyproject.toml
--rw-r--r--   0        0        0     2384 2023-10-07 12:04:54.000000 jinjanator_plugin_format_toml-23.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1451 2024-04-27 15:53:51.000000 jinjanator_plugin_format_toml-24.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3244 2024-04-27 15:53:51.000000 jinjanator_plugin_format_toml-24.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-27 15:53:51.000000 jinjanator_plugin_format_toml-24.1.0/src/jinjanator_plugin_format_toml/__init__.py
+-rw-r--r--   0        0        0      721 2024-04-27 15:53:51.000000 jinjanator_plugin_format_toml-24.1.0/src/jinjanator_plugin_format_toml/plugin.py
+-rw-r--r--   0        0        0        0 2024-04-27 15:53:51.000000 jinjanator_plugin_format_toml-24.1.0/src/jinjanator_plugin_format_toml/py.typed
+-rw-r--r--   0        0        0      499 2024-04-27 15:53:51.000000 jinjanator_plugin_format_toml-24.1.0/tests/test_plugin.py
+-rw-r--r--   0        0        0       32 2024-04-27 15:53:51.000000 jinjanator_plugin_format_toml-24.1.0/.gitignore
+-rw-r--r--   0        0        0    11357 2024-04-27 15:53:51.000000 jinjanator_plugin_format_toml-24.1.0/LICENSE
+-rw-r--r--   0        0        0     6643 2024-04-27 15:53:51.000000 jinjanator_plugin_format_toml-24.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2258 2024-04-27 15:53:51.000000 jinjanator_plugin_format_toml-24.1.0/PKG-INFO
```

### Comparing `jinjanator_plugin_format_toml-23.2.0/CHANGELOG.md` & `jinjanator_plugin_format_toml-24.1.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,21 @@
 This changelog is managed by towncrier and is compiled at release time.
 
 See https://github.com/kpfleming/jinjanator-plugin-format-toml/blob/main/.github/CONTRIBUTING.md#changelog for details.
 -->
 
 <!-- towncrier release notes start -->
 
+## [24.1.0](https://github.com/kpfleming/jinjanator-plugin-format-toml/tree/24.1.0) - 2024-04-27
+
+### Changes
+
+- Upgraded to version 24.1 of jinjanator-plugins.
+  
+
 ## [23.2.0](https://github.com/kpfleming/jinjanator-plugin-format-toml/tree/23.2.0) - 2023-10-07
 
 ### Additions
 
 - Added Python 3.12 support.
   [#2](https://github.com/kpfleming/jinjanator-plugin-format-toml/issues/2)
```

### Comparing `jinjanator_plugin_format_toml-23.2.0/README.md` & `jinjanator_plugin_format_toml-24.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 [![Types - Mypy](https://img.shields.io/badge/Types-Mypy-blue.svg)](https://github.com/python/mypy)
 [![Code Quality - Ruff](https://img.shields.io/badge/Code%20Quality-Ruff-red.svg)](https://github.com/astral-sh/ruff)
 [![Project Management - Hatch](https://img.shields.io/badge/Project%20Management-Hatch-purple.svg)](https://github.com/pypa/hatch)
 [![Testing - Pytest](https://img.shields.io/badge/Testing-Pytest-orange.svg)](https://github.com/pytest-dev/pytest)
 
 This repo contains `jinjanator-plugin-format-toml`, a plugin which
 provides a TOML parser for the
-[Jinjanator](https://github.com/kpfleming/jinjanator) tool.
+[jinjanator](https://github.com/kpfleming/jinjanator) tool.
 
 Open Source software: [Apache License 2.0](https://spdx.org/licenses/Apache-2.0.html)
 
 ## &nbsp;
 <!-- fancy-readme start -->
 
-This plugin allows Jinjanator to parse TOML data for processing in
+This plugin allows jinjanator to parse TOML data for processing in
 templates. The format can be selected using `--format toml` or
 autoselected by using a data file with a name ending with `.toml`.
 
 ## Installation
 
 ```
 pip install jinjanator-plugin-format-toml
@@ -60,15 +60,15 @@
 ## Options
 
 This format does not support any options.
 <!-- fancy-readme end -->
 
 ## Chat
 
-If you'd like to chat with the Jinjanator community, join us on
+If you'd like to chat with the jinjanator community, join us on
 [Matrix](https://matrix.to/#/#jinjanator:km6g.us)!
 
 ## Credits
 
 ["Standing on the shoulders of
 giants"](https://en.wikipedia.org/wiki/Standing_on_the_shoulders_of_giants)
 could not be more true than it is in the Python community; this
```

#### html2text {}

```diff
@@ -9,27 +9,27 @@
 (https://github.com/psf/black) [![Types - Mypy](https://img.shields.io/badge/
 Types-Mypy-blue.svg)](https://github.com/python/mypy) [![Code Quality - Ruff]
 (https://img.shields.io/badge/Code%20Quality-Ruff-red.svg)](https://github.com/
 astral-sh/ruff) [![Project Management - Hatch](https://img.shields.io/badge/
 Project%20Management-Hatch-purple.svg)](https://github.com/pypa/hatch) [!
 [Testing - Pytest](https://img.shields.io/badge/Testing-Pytest-orange.svg)]
 (https://github.com/pytest-dev/pytest) This repo contains `jinjanator-plugin-
-format-toml`, a plugin which provides a TOML parser for the [Jinjanator](https:
+format-toml`, a plugin which provides a TOML parser for the [jinjanator](https:
 //github.com/kpfleming/jinjanator) tool. Open Source software: [Apache License
 2.0](https://spdx.org/licenses/Apache-2.0.html) ##   This plugin allows
-Jinjanator to parse TOML data for processing in templates. The format can be
+jinjanator to parse TOML data for processing in templates. The format can be
 selected using `--format toml` or autoselected by using a data file with a name
 ending with `.toml`. ## Installation ``` pip install jinjanator-plugin-format-
 toml ``` ## Usage Suppose you have an NGINX configuration file template,
 `nginx.j2`: ```jinja2 server { listen 80; server_name {{ nginx.hostname }};
 root {{ nginx.webroot }}; index index.htm; } ``` And you have a TOML file with
 the data, `nginx.toml`: ```toml [nginx] hostname="localhost" webroot="/var/www/
 project" ``` This is how you render it into a working configuration file:
 ```bash $ jinjanate nginx.j2 nginx.toml > nginx.conf ``` ## Options This format
-does not support any options. ## Chat If you'd like to chat with the Jinjanator
+does not support any options. ## Chat If you'd like to chat with the jinjanator
 community, join us on [Matrix](https://matrix.to/#/#jinjanator:km6g.us)! ##
 Credits ["Standing on the shoulders of giants"](https://en.wikipedia.org/wiki/
 Standing_on_the_shoulders_of_giants) could not be more true than it is in the
 Python community; this project relies on many wonderful tools and libraries
 produced by the global open source software community, in addition to Python
 itself. I've listed many of them below, but if I've overlooked any please do
 not be offended :-) * [Black](https://pypi.org/project/black) * [Hatch-Fancy-
```

### Comparing `jinjanator_plugin_format_toml-23.2.0/src/jinjanator_plugin_format_toml/plugin.py` & `jinjanator_plugin_format_toml-24.1.0/src/jinjanator_plugin_format_toml/plugin.py`

 * *Files identical despite different names*

### Comparing `jinjanator_plugin_format_toml-23.2.0/LICENSE` & `jinjanator_plugin_format_toml-24.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jinjanator_plugin_format_toml-23.2.0/pyproject.toml` & `jinjanator_plugin_format_toml-24.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-fancy-pypi-readme",
   "hatch-vcs",
   "hatchling",
 ]
 
 [project]
 name = "jinjanator-plugin-format-toml"
-description = "Plugin which provides TOML format (data input) support for Jinjanator"
+description = "Plugin which provides TOML format (data input) support for jinjanator"
 license = { text="Apache-2.0" }
 authors = [
   { name="Kevin P. Fleming", email="jinjanator@kevin.km6g.us" },
 ]
 requires-python = ">=3.8"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
@@ -30,15 +30,15 @@
   "Typing :: Typed",
 ]
 dynamic = [
   "readme",
   "version",
 ]
 dependencies = [
-  "jinjanator-plugins==23.4.*",
+  "jinjanator-plugins==24.1.*",
   'tomli>=1.1; python_version < "3.11"',
 ]
 [project.urls]
 "Bug Tracker" = "https://github.com/kpfleming/jinjanator-plugin-format-toml/issues"
 "Homepage" = "https://github.com/kpfleming/jinjanator-plugin-format-toml"
 [project.entry-points.jinjanator]
 format_toml = "jinjanator_plugin_format_toml.plugin"
@@ -81,34 +81,33 @@
 ]
 
 [tool.hatch.envs.default]
 python = "3.12"
 
 [tool.hatch.envs.lint]
 dependencies = [
-    "black",
-    "ruff",
+    "ruff>=0.2.0",
     "mypy",
     "pyproject-fmt",
     # tomli has to be installed because mypy has been told to simulate Python 3.8
     "tomli >= 1.1.0",
 ]
 
 [tool.hatch.envs.lint.scripts]
 lint = [
-     "ruff check --fix --show-fixes .",
-     "black --preview .",
+     "ruff format",
+     "ruff check --output-format=full --fix --show-fixes",
      "mypy --package jinjanator_plugin_format_toml",
      "mypy tests",
      "shellcheck workflow-support/*.sh",
      "pyproject-fmt pyproject.toml",
 ]
 lint-action = [
-     "ruff check --output-format=github .",
-     "black --check --diff --preview .",
+     "ruff format --check --diff",
+     "ruff check --output-format=github",
      "mypy --package jinjanator_plugin_format_toml",
      "mypy tests",
      "shellcheck workflow-support/*.sh",
      "pyproject-fmt --check pyproject.toml",
 ]
 
 [tool.hatch.envs.ci]
@@ -139,15 +138,15 @@
 allow-direct-references = true
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 text = """
-# *jinjanator-plugin-format-toml*: Provides TOML format (data input) support for Jinjanator
+# *jinjanator-plugin-format-toml*: Provides TOML format (data input) support for jinjanator
 
 """
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "README.md"
 start-after = "<!-- fancy-readme start -->"
 end-before = "<!-- fancy-readme end -->"
@@ -172,77 +171,55 @@
 pattern = '\[(.+?)\]\(((?!https?://)\S+?)\)'
 replacement = '[\1](https://github.com/kpfleming/jinjanator-plugin-format-toml/tree/main/\g<2>)'
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.substitutions]]
 pattern = "#(\\d+)"
 replacement = "[#\\1](https://github.com/kpfleming/jinjanator-plugin-format-toml/issues/\\1)"
 
-[tool.black]
-line-length = 90
-target-version = ["py38"]
-
 [tool.ruff]
 src = ["src", "tests"]
-format = "grouped"
-target-version = "py38"
-select = ["ALL"]
+line-length = 100
 
+[tool.ruff.lint]
+ignore-init-module-imports = true
+select = ["ALL"]
 ignore = [
   "ANN",      # Mypy is better at this.
+  "COM812",   # conflicts with formatter
   "C901",     # Leave complexity to me.
-  "COM",      # Leave commas to Black.
   "D",        # We have different ideas about docstrings.
-  "E501",     # leave line-length enforcement to Black
+  "ISC001",   # conflicts with formatter
   "PLR0912",  # Leave complexity to me.
   "TRY301",   # Raise in try blocks can totally make sense.
 ]
 unfixable = ["F401"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/*" = [
   "PLC1901", # empty strings are falsey, but are less specific in tests
   "PT005",   # we use always underscores and explicit names
   "S101",    # assert
   "SIM300",  # Yoda rocks in tests
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 lines-between-types = 1
 lines-after-imports = 2
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 xfail_strict = true
 testpaths = [
     "tests",
 ]
 addopts = [
     "-ra",
     "--strict-markers",
 ]
 
-[tool.mypy]
-python_version = 3.8
-namespace_packages = true
-explicit_package_bases = true
-check_untyped_defs = true
-disallow_any_generics = true
-disallow_incomplete_defs = true
-disallow_subclassing_any = true
-disallow_untyped_calls = true
-disallow_untyped_decorators = true
-disallow_untyped_defs = true
-follow_imports = "normal"
-no_implicit_optional = true
-strict_equality = true
-warn_no_return = true
-warn_redundant_casts = true
-warn_return_any = true
-warn_unused_ignores = true
-
 [tool.towncrier]
 name = "jinjanator-plugin-format-toml"
 package = "jinjanator_plugin_format_toml"
 directory = "changelog.d"
 filename = "CHANGELOG.md"
 start_string = "<!-- towncrier release notes start -->\n"
 template = "changelog.d/towncrier_template.md.jinja"
@@ -273,7 +250,26 @@
 name = "Changes"
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "fixing"
 name = "Fixes"
 showcontent = true
+
+[tool.mypy]
+python_version = 3.8
+namespace_packages = true
+explicit_package_bases = true
+check_untyped_defs = true
+disallow_any_generics = true
+disallow_incomplete_defs = true
+disallow_subclassing_any = true
+disallow_untyped_calls = true
+disallow_untyped_decorators = true
+disallow_untyped_defs = true
+follow_imports = "normal"
+no_implicit_optional = true
+strict_equality = true
+warn_no_return = true
+warn_redundant_casts = true
+warn_return_any = true
+warn_unused_ignores = true
```

### Comparing `jinjanator_plugin_format_toml-23.2.0/PKG-INFO` & `jinjanator_plugin_format_toml-24.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jinjanator-plugin-format-toml
-Version: 23.2.0
-Summary: Plugin which provides TOML format (data input) support for Jinjanator
+Version: 24.1.0
+Summary: Plugin which provides TOML format (data input) support for jinjanator
 Project-URL: Bug Tracker, https://github.com/kpfleming/jinjanator-plugin-format-toml/issues
 Project-URL: Homepage, https://github.com/kpfleming/jinjanator-plugin-format-toml
 Author-email: "Kevin P. Fleming" <jinjanator@kevin.km6g.us>
 License: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -17,23 +17,23 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: jinjanator-plugins==23.4.*
+Requires-Dist: jinjanator-plugins==24.1.*
 Requires-Dist: tomli>=1.1; python_version < '3.11'
 Description-Content-Type: text/markdown
 
-# *jinjanator-plugin-format-toml*: Provides TOML format (data input) support for Jinjanator
+# *jinjanator-plugin-format-toml*: Provides TOML format (data input) support for jinjanator
 
 
 
-This plugin allows Jinjanator to parse TOML data for processing in
+This plugin allows jinjanator to parse TOML data for processing in
 templates. The format can be selected using `--format toml` or
 autoselected by using a data file with a name ending with `.toml`.
 
 ## Installation
 
 ```
 pip install jinjanator-plugin-format-toml
@@ -67,15 +67,14 @@
 $ jinjanate nginx.j2 nginx.toml > nginx.conf
 ```
 
 ## Options
 
 This format does not support any options.
 ## Release Information
-### Additions
-
-- Added Python 3.12 support.
-  [[#2](https://github.com/kpfleming/jinjanator-plugin-format-toml/issues/2)](https://github.com/kpfleming/jinjanator-plugin-format-toml/issues/2)
+### Changes
 
+- Upgraded to version 24.1 of jinjanator-plugins.
+  
 
 ---
 [→ Full Changelog](https://github.com/kpfleming/jinjanator-plugin-format-toml/blob/main/CHANGELOG.md)
```

