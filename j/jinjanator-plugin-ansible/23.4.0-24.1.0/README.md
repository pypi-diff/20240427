# Comparing `tmp/jinjanator_plugin_ansible-23.4.0.tar.gz` & `tmp/jinjanator_plugin_ansible-24.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Oct  7 12:01:29 2023, max compression
+gzip compressed data, last modified: Sat Apr 27 15:46:07 2024, max compression
```

## Comparing `jinjanator_plugin_ansible-23.4.0.tar` & `jinjanator_plugin_ansible-24.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1937 2023-10-07 12:01:29.000000 jinjanator_plugin_ansible-23.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     2866 2023-10-07 12:01:29.000000 jinjanator_plugin_ansible-23.4.0/README.md
--rw-r--r--   0        0        0        0 2023-10-07 12:01:29.000000 jinjanator_plugin_ansible-23.4.0/src/jinjanator_plugin_ansible/__init__.py
--rw-r--r--   0        0        0     1612 2023-10-07 12:01:29.000000 jinjanator_plugin_ansible-23.4.0/src/jinjanator_plugin_ansible/plugin.py
--rw-r--r--   0        0        0        0 2023-10-07 12:01:29.000000 jinjanator_plugin_ansible-23.4.0/src/jinjanator_plugin_ansible/py.typed
--rw-r--r--   0        0        0      638 2023-10-07 12:01:29.000000 jinjanator_plugin_ansible-23.4.0/tests/test_plugin.py
--rw-r--r--   0        0        0       32 2023-10-07 12:01:29.000000 jinjanator_plugin_ansible-23.4.0/.gitignore
--rw-r--r--   0        0        0    11357 2023-10-07 12:01:29.000000 jinjanator_plugin_ansible-23.4.0/LICENSE
--rw-r--r--   0        0        0     6438 2023-10-07 12:01:29.000000 jinjanator_plugin_ansible-23.4.0/pyproject.toml
--rw-r--r--   0        0        0     1885 2023-10-07 12:01:29.000000 jinjanator_plugin_ansible-23.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2098 2024-04-27 15:46:07.000000 jinjanator_plugin_ansible-24.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2866 2024-04-27 15:46:07.000000 jinjanator_plugin_ansible-24.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-27 15:46:07.000000 jinjanator_plugin_ansible-24.1.0/src/jinjanator_plugin_ansible/__init__.py
+-rw-r--r--   0        0        0     1676 2024-04-27 15:46:07.000000 jinjanator_plugin_ansible-24.1.0/src/jinjanator_plugin_ansible/plugin.py
+-rw-r--r--   0        0        0        0 2024-04-27 15:46:07.000000 jinjanator_plugin_ansible-24.1.0/src/jinjanator_plugin_ansible/py.typed
+-rw-r--r--   0        0        0      638 2024-04-27 15:46:07.000000 jinjanator_plugin_ansible-24.1.0/tests/test_plugin.py
+-rw-r--r--   0        0        0       32 2024-04-27 15:46:07.000000 jinjanator_plugin_ansible-24.1.0/.gitignore
+-rw-r--r--   0        0        0    11357 2024-04-27 15:46:07.000000 jinjanator_plugin_ansible-24.1.0/LICENSE
+-rw-r--r--   0        0        0     6404 2024-04-27 15:46:07.000000 jinjanator_plugin_ansible-24.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1767 2024-04-27 15:46:07.000000 jinjanator_plugin_ansible-24.1.0/PKG-INFO
```

### Comparing `jinjanator_plugin_ansible-23.4.0/CHANGELOG.md` & `jinjanator_plugin_ansible-24.1.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,21 @@
 This changelog is managed by towncrier and is compiled at release time.
 
 See https://github.com/kpfleming/jinjanator-plugin-ansible/blob/main/.github/CONTRIBUTING.md#changelog for details.
 -->
 
 <!-- towncrier release notes start -->
 
+## [24.1.0](https://github.com/kpfleming/jinjanator-plugin-ansible/tree/24.1.0) - 2024-04-27
+
+### Changes
+
+- Upgraded to version 24.1 of jinjanator-plugins.
+  
+
 ## [23.4.0](https://github.com/kpfleming/jinjanator-plugin-ansible/tree/23.4.0) - 2023-10-07
 
 ### Additions
 
 - Added Python 3.12 support.
   [#5](https://github.com/kpfleming/jinjanator-plugin-ansible/issues/5)
```

### Comparing `jinjanator_plugin_ansible-23.4.0/README.md` & `jinjanator_plugin_ansible-24.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 [![Types - Mypy](https://img.shields.io/badge/Types-Mypy-blue.svg)](https://github.com/python/mypy)
 [![Code Quality - Ruff](https://img.shields.io/badge/Code%20Quality-Ruff-red.svg)](https://github.com/astral-sh/ruff)
 [![Project Management - Hatch](https://img.shields.io/badge/Project%20Management-Hatch-purple.svg)](https://github.com/pypa/hatch)
 [![Testing - Pytest](https://img.shields.io/badge/Testing-Pytest-orange.svg)](https://github.com/pytest-dev/pytest)
 
 This repo contains `jinjanator-plugin-ansible`, a plugin which
 provides access to Ansible's filters to templates rendered using the
-[Jinjanator](https://github.com/kpfleming/jinjanator) tool.
+[jinjanator](https://github.com/kpfleming/jinjanator) tool.
 
 Open Source software: [Apache License 2.0](https://spdx.org/licenses/Apache-2.0.html)
 
 ## &nbsp;
 <!-- fancy-readme start -->
 
 This plugin makes all of the filters and tests from the Ansible 'core'
-collection available to templates being rendered using the Jinjanator
+collection available to templates being rendered using the jinjanator
 tool.
 
 ## Installation
 
 ```
 pip install jinjanator-plugin-ansible
 ```
@@ -34,15 +34,15 @@
 The Ansible filters and tests can be used in templates using the same
 names that would be used if the template was rendered by Ansible
 itself.
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
@@ -10,22 +10,22 @@
 blue.svg)](https://github.com/python/mypy) [![Code Quality - Ruff](https://
 img.shields.io/badge/Code%20Quality-Ruff-red.svg)](https://github.com/astral-
 sh/ruff) [![Project Management - Hatch](https://img.shields.io/badge/
 Project%20Management-Hatch-purple.svg)](https://github.com/pypa/hatch) [!
 [Testing - Pytest](https://img.shields.io/badge/Testing-Pytest-orange.svg)]
 (https://github.com/pytest-dev/pytest) This repo contains `jinjanator-plugin-
 ansible`, a plugin which provides access to Ansible's filters to templates
-rendered using the [Jinjanator](https://github.com/kpfleming/jinjanator) tool.
+rendered using the [jinjanator](https://github.com/kpfleming/jinjanator) tool.
 Open Source software: [Apache License 2.0](https://spdx.org/licenses/Apache-
 2.0.html) ##   This plugin makes all of the filters and tests from the Ansible
-'core' collection available to templates being rendered using the Jinjanator
+'core' collection available to templates being rendered using the jinjanator
 tool. ## Installation ``` pip install jinjanator-plugin-ansible ``` ## Usage
 The Ansible filters and tests can be used in templates using the same names
 that would be used if the template was rendered by Ansible itself. ## Chat If
-you'd like to chat with the Jinjanator community, join us on [Matrix](https://
+you'd like to chat with the jinjanator community, join us on [Matrix](https://
 matrix.to/#/#jinjanator:km6g.us)! ## Credits ["Standing on the shoulders of
 giants"](https://en.wikipedia.org/wiki/Standing_on_the_shoulders_of_giants)
 could not be more true than it is in the Python community; this project relies
 on many wonderful tools and libraries produced by the global open source
 software community, in addition to Python itself. I've listed many of them
 below, but if I've overlooked any please do not be offended :-) * [Black]
 (https://pypi.org/project/black) * [Hatch-Fancy-PyPI-Readme](https://pypi.org/
```

### Comparing `jinjanator_plugin_ansible-23.4.0/src/jinjanator_plugin_ansible/plugin.py` & `jinjanator_plugin_ansible-24.1.0/src/jinjanator_plugin_ansible/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import importlib
 
 from typing import cast
 
-import ansible.plugins.filter.core as filter_core  # type: ignore[import]
-import ansible.plugins.filter.mathstuff as filter_mathstuff  # type: ignore[import]
-import ansible.plugins.filter.urls as filter_urls  # type: ignore[import]
-import ansible.plugins.filter.urlsplit as filter_urlsplit  # type: ignore[import]
-import ansible.plugins.test.core as test_core  # type: ignore[import]
-import ansible.plugins.test.files as test_files  # type: ignore[import]
-import ansible.plugins.test.mathstuff as test_mathstuff  # type: ignore[import]
-import ansible.plugins.test.uri as test_uri  # type: ignore[import]
+import ansible.plugins.filter.core as filter_core  # type: ignore[import-untyped]
+import ansible.plugins.filter.mathstuff as filter_mathstuff  # type: ignore[import-untyped]
+import ansible.plugins.filter.urls as filter_urls  # type: ignore[import-untyped]
+import ansible.plugins.filter.urlsplit as filter_urlsplit  # type: ignore[import-untyped]
+import ansible.plugins.test.core as test_core  # type: ignore[import-untyped]
+import ansible.plugins.test.files as test_files  # type: ignore[import-untyped]
+import ansible.plugins.test.mathstuff as test_mathstuff  # type: ignore[import-untyped]
+import ansible.plugins.test.uri as test_uri  # type: ignore[import-untyped]
 
 from jinjanator_plugins import (
     Filters,
     Identity,
     Tests,
     plugin_filters_hook,
     plugin_identity_hook,
```

### Comparing `jinjanator_plugin_ansible-23.4.0/tests/test_plugin.py` & `jinjanator_plugin_ansible-24.1.0/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `jinjanator_plugin_ansible-23.4.0/LICENSE` & `jinjanator_plugin_ansible-24.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jinjanator_plugin_ansible-23.4.0/pyproject.toml` & `jinjanator_plugin_ansible-24.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-fancy-pypi-readme",
   "hatch-vcs",
   "hatchling",
 ]
 
 [project]
 name = "jinjanator-plugin-ansible"
-description = "Plugin which provides Ansible filters and tests to the Jinjanator tool"
+description = "Plugin which provides Ansible filters and tests to the jinjanator tool"
 license = { text="Apache-2.0" }
 authors = [
   { name="Kevin P. Fleming", email="jinjanator@kevin.km6g.us" },
 ]
 requires-python = ">=3.9"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
@@ -30,15 +30,15 @@
 ]
 dynamic = [
   "readme",
   "version",
 ]
 dependencies = [
   "ansible-core",
-  "jinjanator-plugins==23.4.*",
+  "jinjanator-plugins==24.1.*",
 ]
 [project.urls]
 "Bug Tracker" = "https://github.com/kpfleming/jinjanator-plugin-ansible/issues"
 "Homepage" = "https://github.com/kpfleming/jinjanator-plugin-ansible"
 [project.entry-points.jinjanator]
 ansible = "jinjanator_plugin_ansible.plugin"
 
@@ -80,32 +80,31 @@
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
 ]
 
 [tool.hatch.envs.lint.scripts]
 lint = [
-     "ruff check --fix --show-fixes .",
-     "black --preview .",
+     "ruff format",
+     "ruff check --output-format=full --fix --show-fixes",
      "mypy --package jinjanator_plugin_ansible",
      "mypy tests",
      "shellcheck workflow-support/*.sh",
      "pyproject-fmt pyproject.toml",
 ]
 lint-action = [
-     "ruff check --output-format=github .",
-     "black --check --diff --preview .",
+     "ruff format --check --diff",
+     "ruff check --output-format=github",
      "mypy --package jinjanator_plugin_ansible",
      "mypy tests",
      "shellcheck workflow-support/*.sh",
      "pyproject-fmt --check pyproject.toml",
 ]
 
 [tool.hatch.envs.ci]
@@ -135,15 +134,15 @@
 allow-direct-references = true
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 text = """
-# *jinjanator-plugin-ansible*: Makes Ansible's filters and tests available in Jinjanator
+# *jinjanator-plugin-ansible*: Makes Ansible's filters and tests available in jinjanator
 
 """
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "README.md"
 start-after = "<!-- fancy-readme start -->"
 end-before = "<!-- fancy-readme end -->"
@@ -168,77 +167,55 @@
 pattern = '\[(.+?)\]\(((?!https?://)\S+?)\)'
 replacement = '[\1](https://github.com/kpfleming/jinjanator-plugin-ansible/tree/main/\g<2>)'
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.substitutions]]
 pattern = "#(\\d+)"
 replacement = "[#\\1](https://github.com/kpfleming/jinjanator-plugin-ansible/issues/\\1)"
 
-[tool.black]
-line-length = 90
-target-version = ["py39"]
-
 [tool.ruff]
 src = ["src", "tests"]
-format = "grouped"
-target-version = "py39"
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
-python_version = 3.9
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
 name = "jinjanator-plugin-ansible"
 package = "jinjanator_plugin_ansible"
 directory = "changelog.d"
 filename = "CHANGELOG.md"
 start_string = "<!-- towncrier release notes start -->\n"
 template = "changelog.d/towncrier_template.md.jinja"
@@ -269,7 +246,26 @@
 name = "Changes"
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "fixing"
 name = "Fixes"
 showcontent = true
+
+[tool.mypy]
+python_version = 3.9
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

### Comparing `jinjanator_plugin_ansible-23.4.0/PKG-INFO` & `jinjanator_plugin_ansible-24.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jinjanator-plugin-ansible
-Version: 23.4.0
-Summary: Plugin which provides Ansible filters and tests to the Jinjanator tool
+Version: 24.1.0
+Summary: Plugin which provides Ansible filters and tests to the jinjanator tool
 Project-URL: Bug Tracker, https://github.com/kpfleming/jinjanator-plugin-ansible/issues
 Project-URL: Homepage, https://github.com/kpfleming/jinjanator-plugin-ansible
 Author-email: "Kevin P. Fleming" <jinjanator@kevin.km6g.us>
 License: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -17,38 +17,37 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Requires-Dist: ansible-core
-Requires-Dist: jinjanator-plugins==23.4.*
+Requires-Dist: jinjanator-plugins==24.1.*
 Description-Content-Type: text/markdown
 
-# *jinjanator-plugin-ansible*: Makes Ansible's filters and tests available in Jinjanator
+# *jinjanator-plugin-ansible*: Makes Ansible's filters and tests available in jinjanator
 
 
 
 This plugin makes all of the filters and tests from the Ansible 'core'
-collection available to templates being rendered using the Jinjanator
+collection available to templates being rendered using the jinjanator
 tool.
 
 ## Installation
 
 ```
 pip install jinjanator-plugin-ansible
 ```
 
 ## Usage
 
 The Ansible filters and tests can be used in templates using the same
 names that would be used if the template was rendered by Ansible
 itself.
 ## Release Information
-### Additions
-
-- Added Python 3.12 support.
-  [[#5](https://github.com/kpfleming/jinjanator-plugin-ansible/issues/5)](https://github.com/kpfleming/jinjanator-plugin-ansible/issues/5)
+### Changes
 
+- Upgraded to version 24.1 of jinjanator-plugins.
+  
 
 ---
 [→ Full Changelog](https://github.com/kpfleming/jinjanator-plugin-ansible/blob/main/CHANGELOG.md)
```

