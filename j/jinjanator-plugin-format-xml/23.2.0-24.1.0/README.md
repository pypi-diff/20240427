# Comparing `tmp/jinjanator_plugin_format_xml-23.2.0.tar.gz` & `tmp/jinjanator_plugin_format_xml-24.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Oct  7 12:07:27 2023, max compression
+gzip compressed data, last modified: Sat Apr 27 15:52:39 2024, max compression
```

## Comparing `jinjanator_plugin_format_xml-23.2.0.tar` & `jinjanator_plugin_format_xml-24.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1281 2023-10-07 12:07:27.000000 jinjanator_plugin_format_xml-23.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     3393 2023-10-07 12:07:27.000000 jinjanator_plugin_format_xml-23.2.0/README.md
--rw-r--r--   0        0        0        0 2023-10-07 12:07:27.000000 jinjanator_plugin_format_xml-23.2.0/src/jinjanator_plugin_format_xml/__init__.py
--rw-r--r--   0        0        0      786 2023-10-07 12:07:27.000000 jinjanator_plugin_format_xml-23.2.0/src/jinjanator_plugin_format_xml/plugin.py
--rw-r--r--   0        0        0        0 2023-10-07 12:07:27.000000 jinjanator_plugin_format_xml-23.2.0/src/jinjanator_plugin_format_xml/py.typed
--rw-r--r--   0        0        0     1171 2023-10-07 12:07:27.000000 jinjanator_plugin_format_xml-23.2.0/tests/test_plugin.py
--rw-r--r--   0        0        0       32 2023-10-07 12:07:27.000000 jinjanator_plugin_format_xml-23.2.0/.gitignore
--rw-r--r--   0        0        0    11357 2023-10-07 12:07:27.000000 jinjanator_plugin_format_xml-23.2.0/LICENSE
--rw-r--r--   0        0        0     6552 2023-10-07 12:07:27.000000 jinjanator_plugin_format_xml-23.2.0/pyproject.toml
--rw-r--r--   0        0        0     2551 2023-10-07 12:07:27.000000 jinjanator_plugin_format_xml-23.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1445 2024-04-27 15:52:39.000000 jinjanator_plugin_format_xml-24.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3393 2024-04-27 15:52:39.000000 jinjanator_plugin_format_xml-24.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-27 15:52:39.000000 jinjanator_plugin_format_xml-24.1.0/src/jinjanator_plugin_format_xml/__init__.py
+-rw-r--r--   0        0        0      786 2024-04-27 15:52:39.000000 jinjanator_plugin_format_xml-24.1.0/src/jinjanator_plugin_format_xml/plugin.py
+-rw-r--r--   0        0        0        0 2024-04-27 15:52:39.000000 jinjanator_plugin_format_xml-24.1.0/src/jinjanator_plugin_format_xml/py.typed
+-rw-r--r--   0        0        0     1143 2024-04-27 15:52:39.000000 jinjanator_plugin_format_xml-24.1.0/tests/test_plugin.py
+-rw-r--r--   0        0        0       32 2024-04-27 15:52:39.000000 jinjanator_plugin_format_xml-24.1.0/.gitignore
+-rw-r--r--   0        0        0    11357 2024-04-27 15:52:39.000000 jinjanator_plugin_format_xml-24.1.0/LICENSE
+-rw-r--r--   0        0        0     6518 2024-04-27 15:52:39.000000 jinjanator_plugin_format_xml-24.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2427 2024-04-27 15:52:39.000000 jinjanator_plugin_format_xml-24.1.0/PKG-INFO
```

### Comparing `jinjanator_plugin_format_xml-23.2.0/CHANGELOG.md` & `jinjanator_plugin_format_xml-24.1.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,21 @@
 This changelog is managed by towncrier and is compiled at release time.
 
 See https://github.com/kpfleming/jinjanator-plugin-format-xml/blob/main/.github/CONTRIBUTING.md#changelog for details.
 -->
 
 <!-- towncrier release notes start -->
 
+## [24.1.0](https://github.com/kpfleming/jinjanator-plugin-format-xml/tree/24.1.0) - 2024-04-27
+
+### Changes
+
+- Upgraded to version 24.1 of jinjanator-plugins.
+  
+
 ## [23.2.0](https://github.com/kpfleming/jinjanator-plugin-format-xml/tree/23.2.0) - 2023-10-07
 
 ### Additions
 
 - Added Python 3.12 support.
   [#2](https://github.com/kpfleming/jinjanator-plugin-format-xml/issues/2)
```

### Comparing `jinjanator_plugin_format_xml-23.2.0/README.md` & `jinjanator_plugin_format_xml-24.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 [![Code Style - Black](https://img.shields.io/badge/Code%20Style-Black-000000.svg)](https://github.com/psf/black)
 [![Types - Mypy](https://img.shields.io/badge/Types-Mypy-blue.svg)](https://github.com/python/mypy)
 [![Code Quality - Ruff](https://img.shields.io/badge/Code%20Quality-Ruff-red.svg)](https://github.com/astral-sh/ruff)
 [![Project Management - Hatch](https://img.shields.io/badge/Project%20Management-Hatch-purple.svg)](https://github.com/pypa/hatch)
 [![Testing - Pytest](https://img.shields.io/badge/Testing-Pytest-orange.svg)](https://github.com/pytest-dev/pytest)
 
 This repo contains `jinjanator-plugin-format-xml`, a plugin which
-provides an XML parser for the [Jinjanator](https://github.com/kpfleming/jinjanator) tool.
+provides an XML parser for the [jinjanator](https://github.com/kpfleming/jinjanator) tool.
 
 Open Source software: [Apache License 2.0](https://spdx.org/licenses/Apache-2.0.html)
 
 ## &nbsp;
 <!-- fancy-readme start -->
 
-This plugin allows Jinjanator to parse XML data for processing in
+This plugin allows jinjanator to parse XML data for processing in
 templates. The format can be selected using `--format xml` or
 autoselected by using a data file with a name ending with `.xml`.
 
 ## Installation
 
 ```
 pip install jinjanator-plugin-format-xml
@@ -66,15 +66,15 @@
 * `process-namespaces`: configures the XML parser to replace namespace
   references in element names with the corresponding namespaces from
   `xmlns` attributes in the top-level element in the document.
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
@@ -9,29 +9,29 @@
 (https://github.com/psf/black) [![Types - Mypy](https://img.shields.io/badge/
 Types-Mypy-blue.svg)](https://github.com/python/mypy) [![Code Quality - Ruff]
 (https://img.shields.io/badge/Code%20Quality-Ruff-red.svg)](https://github.com/
 astral-sh/ruff) [![Project Management - Hatch](https://img.shields.io/badge/
 Project%20Management-Hatch-purple.svg)](https://github.com/pypa/hatch) [!
 [Testing - Pytest](https://img.shields.io/badge/Testing-Pytest-orange.svg)]
 (https://github.com/pytest-dev/pytest) This repo contains `jinjanator-plugin-
-format-xml`, a plugin which provides an XML parser for the [Jinjanator](https:/
+format-xml`, a plugin which provides an XML parser for the [jinjanator](https:/
 /github.com/kpfleming/jinjanator) tool. Open Source software: [Apache License
 2.0](https://spdx.org/licenses/Apache-2.0.html) ##   This plugin allows
-Jinjanator to parse XML data for processing in templates. The format can be
+jinjanator to parse XML data for processing in templates. The format can be
 selected using `--format xml` or autoselected by using a data file with a name
 ending with `.xml`. ## Installation ``` pip install jinjanator-plugin-format-
 xml ``` ## Usage Suppose you have an NGINX configuration file template,
 `nginx.j2`: ```jinja2 server { listen 80; server_name {{ nginx.hostname }};
 root {{ nginx.webroot }}; index index.htm; } ``` And you have an XML file with
 the data, `nginx.xml`: ```xml localhost /var/www/project ``` This is how you
 render it into a working configuration file: ```bash $ jinjanate nginx.j2
 nginx.xml > nginx.conf ``` ## Options * `process-namespaces`: configures the
 XML parser to replace namespace references in element names with the
 corresponding namespaces from `xmlns` attributes in the top-level element in
-the document. ## Chat If you'd like to chat with the Jinjanator community, join
+the document. ## Chat If you'd like to chat with the jinjanator community, join
 us on [Matrix](https://matrix.to/#/#jinjanator:km6g.us)! ## Credits ["Standing
 on the shoulders of giants"](https://en.wikipedia.org/wiki/
 Standing_on_the_shoulders_of_giants) could not be more true than it is in the
 Python community; this project relies on many wonderful tools and libraries
 produced by the global open source software community, in addition to Python
 itself. I've listed many of them below, but if I've overlooked any please do
 not be offended :-) * [Black](https://github.com/psf/black) * [Hatch-Fancy-
```

### Comparing `jinjanator_plugin_format_xml-23.2.0/src/jinjanator_plugin_format_xml/plugin.py` & `jinjanator_plugin_format_xml-24.1.0/src/jinjanator_plugin_format_xml/plugin.py`

 * *Files identical despite different names*

### Comparing `jinjanator_plugin_format_xml-23.2.0/tests/test_plugin.py` & `jinjanator_plugin_format_xml-24.1.0/tests/test_plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,23 +15,19 @@
     assert "testdoc" in result
     assert "cheese" in result["testdoc"]
     assert "bleu" == result["testdoc"]["cheese"]
 
 
 def test_format_namespaces() -> None:
     fmt = plugin.XMLFormat("process-namespaces")
-    result = fmt.parse(
-        '<testdoc xmlns:a="http://a.com/"><a:cheese>bleu</a:cheese></testdoc>'
-    )
+    result = fmt.parse('<testdoc xmlns:a="http://a.com/"><a:cheese>bleu</a:cheese></testdoc>')
     assert "testdoc" in result
     assert "http://a.com/:cheese" in result["testdoc"]
     assert "bleu" == result["testdoc"]["http://a.com/:cheese"]
 
 
 def test_format_ignore_namespaces() -> None:
     fmt = plugin.XMLFormat(None)
-    result = fmt.parse(
-        '<testdoc xmlns:a="http://a.com/"><a:cheese>bleu</a:cheese></testdoc>'
-    )
+    result = fmt.parse('<testdoc xmlns:a="http://a.com/"><a:cheese>bleu</a:cheese></testdoc>')
     assert "testdoc" in result
     assert "a:cheese" in result["testdoc"]
     assert "bleu" == result["testdoc"]["a:cheese"]
```

### Comparing `jinjanator_plugin_format_xml-23.2.0/LICENSE` & `jinjanator_plugin_format_xml-24.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jinjanator_plugin_format_xml-23.2.0/pyproject.toml` & `jinjanator_plugin_format_xml-24.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-fancy-pypi-readme",
   "hatch-vcs",
   "hatchling",
 ]
 
 [project]
 name = "jinjanator-plugin-format-xml"
-description = "Plugin which provides XML format (data input) support for Jinjanator"
+description = "Plugin which provides XML format (data input) support for jinjanator"
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
   "xmltodict",
 ]
 [project.urls]
 "Bug Tracker" = "https://github.com/kpfleming/jinjanator-plugin-format-xml/issues"
 "Homepage" = "https://github.com/kpfleming/jinjanator-plugin-format-xml"
 [project.entry-points.jinjanator]
 format_xml = "jinjanator_plugin_format_xml.plugin"
@@ -81,33 +81,32 @@
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
     "types-xmltodict",
 ]
 
 [tool.hatch.envs.lint.scripts]
 lint = [
-     "ruff check --fix --show-fixes .",
-     "black --preview .",
+     "ruff format",
+     "ruff check --output-format=full --fix --show-fixes",
      "mypy --package jinjanator_plugin_format_xml",
      "mypy tests",
      "shellcheck workflow-support/*.sh",
      "pyproject-fmt pyproject.toml",
 ]
 lint-action = [
-     "ruff check --output-format=github .",
-     "black --check --diff --preview .",
+     "ruff format --check --diff",
+     "ruff check --output-format=github",
      "mypy --package jinjanator_plugin_format_xml",
      "mypy tests",
      "shellcheck workflow-support/*.sh",
      "pyproject-fmt --check pyproject.toml",
 ]
 
 [tool.hatch.envs.ci]
@@ -138,15 +137,15 @@
 allow-direct-references = true
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 text = """
-# *jinjanator-plugin-format-xml*: Provides XML format (data input) support for Jinjanator
+# *jinjanator-plugin-format-xml*: Provides XML format (data input) support for jinjanator
 
 """
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "README.md"
 start-after = "<!-- fancy-readme start -->"
 end-before = "<!-- fancy-readme end -->"
@@ -171,77 +170,55 @@
 pattern = '\[(.+?)\]\(((?!https?://)\S+?)\)'
 replacement = '[\1](https://github.com/kpfleming/jinjanator-plugin-format-xml/tree/main/\g<2>)'
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.substitutions]]
 pattern = "#(\\d+)"
 replacement = "[#\\1](https://github.com/kpfleming/jinjanator-plugin-format-xml/issues/\\1)"
 
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
 name = "jinjanator-plugin-format-xml"
 package = "jinjanator_plugin_format_xml"
 directory = "changelog.d"
 filename = "CHANGELOG.md"
 start_string = "<!-- towncrier release notes start -->\n"
 template = "changelog.d/towncrier_template.md.jinja"
@@ -272,7 +249,26 @@
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

### Comparing `jinjanator_plugin_format_xml-23.2.0/PKG-INFO` & `jinjanator_plugin_format_xml-24.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jinjanator-plugin-format-xml
-Version: 23.2.0
-Summary: Plugin which provides XML format (data input) support for Jinjanator
+Version: 24.1.0
+Summary: Plugin which provides XML format (data input) support for jinjanator
 Project-URL: Bug Tracker, https://github.com/kpfleming/jinjanator-plugin-format-xml/issues
 Project-URL: Homepage, https://github.com/kpfleming/jinjanator-plugin-format-xml
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
 Requires-Dist: xmltodict
 Description-Content-Type: text/markdown
 
-# *jinjanator-plugin-format-xml*: Provides XML format (data input) support for Jinjanator
+# *jinjanator-plugin-format-xml*: Provides XML format (data input) support for jinjanator
 
 
 
-This plugin allows Jinjanator to parse XML data for processing in
+This plugin allows jinjanator to parse XML data for processing in
 templates. The format can be selected using `--format xml` or
 autoselected by using a data file with a name ending with `.xml`.
 
 ## Installation
 
 ```
 pip install jinjanator-plugin-format-xml
@@ -74,15 +74,14 @@
 
 ## Options
 
 * `process-namespaces`: configures the XML parser to replace namespace
   references in element names with the corresponding namespaces from
   `xmlns` attributes in the top-level element in the document.
 ## Release Information
-### Additions
-
-- Added Python 3.12 support.
-  [[#2](https://github.com/kpfleming/jinjanator-plugin-format-xml/issues/2)](https://github.com/kpfleming/jinjanator-plugin-format-xml/issues/2)
+### Changes
 
+- Upgraded to version 24.1 of jinjanator-plugins.
+  
 
 ---
 [→ Full Changelog](https://github.com/kpfleming/jinjanator-plugin-format-xml/blob/main/CHANGELOG.md)
```

