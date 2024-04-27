# Comparing `tmp/jinjanator-23.7.0.tar.gz` & `tmp/jinjanator-24.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Oct  7 11:55:26 2023, max compression
+gzip compressed data, last modified: Sat Apr 27 15:34:19 2024, max compression
```

## Comparing `jinjanator-23.7.0.tar` & `jinjanator-24.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2878 2023-10-07 11:55:26.000000 jinjanator-23.7.0/CHANGELOG.md
--rw-r--r--   0        0        0    10454 2023-10-07 11:55:26.000000 jinjanator-23.7.0/README.md
--rw-r--r--   0        0        0       81 2023-10-07 11:55:26.000000 jinjanator-23.7.0/src/jinjanator/__init__.py
--rw-r--r--   0        0        0    12008 2023-10-07 11:55:26.000000 jinjanator-23.7.0/src/jinjanator/cli.py
--rw-r--r--   0        0        0      692 2023-10-07 11:55:26.000000 jinjanator-23.7.0/src/jinjanator/context.py
--rw-r--r--   0        0        0     1186 2023-10-07 11:55:26.000000 jinjanator-23.7.0/src/jinjanator/filters.py
--rw-r--r--   0        0        0     6858 2023-10-07 11:55:26.000000 jinjanator-23.7.0/src/jinjanator/formats.py
--rw-r--r--   0        0        0        0 2023-10-07 11:55:26.000000 jinjanator-23.7.0/src/jinjanator/py.typed
--rw-r--r--   0        0        0      413 2023-10-07 11:55:26.000000 jinjanator-23.7.0/src/jinjanator/version.py
--rw-r--r--   0        0        0     1614 2023-10-07 11:55:26.000000 jinjanator-23.7.0/tests/__init__.py
--rw-r--r--   0        0        0      675 2023-10-07 11:55:26.000000 jinjanator-23.7.0/tests/conftest.py
--rw-r--r--   0        0        0     1683 2023-10-07 11:55:26.000000 jinjanator-23.7.0/tests/test_argparse.py
--rw-r--r--   0        0        0     2819 2023-10-07 11:55:26.000000 jinjanator-23.7.0/tests/test_cli.py
--rw-r--r--   0        0        0     2723 2023-10-07 11:55:26.000000 jinjanator-23.7.0/tests/test_env.py
--rw-r--r--   0        0        0      248 2023-10-07 11:55:26.000000 jinjanator-23.7.0/tests/test_extension.py
--rw-r--r--   0        0        0     1101 2023-10-07 11:55:26.000000 jinjanator-23.7.0/tests/test_format_options.py
--rw-r--r--   0        0        0      842 2023-10-07 11:55:26.000000 jinjanator-23.7.0/tests/test_invalid_data.py
--rw-r--r--   0        0        0     1886 2023-10-07 11:55:26.000000 jinjanator-23.7.0/tests/test_json_input.py
--rw-r--r--   0        0        0     3461 2023-10-07 11:55:26.000000 jinjanator-23.7.0/tests/test_nginx_config.py
--rw-r--r--   0        0        0      780 2023-10-07 11:55:26.000000 jinjanator-23.7.0/tests/test_output_file.py
--rw-r--r--   0        0        0      435 2023-10-07 11:55:26.000000 jinjanator-23.7.0/tests/test_template_not_found.py
--rw-r--r--   0        0        0      501 2023-10-07 11:55:26.000000 jinjanator-23.7.0/tests/test_undefined.py
--rw-r--r--   0        0        0      728 2023-10-07 11:55:26.000000 jinjanator-23.7.0/tests/test_unicode.py
--rw-r--r--   0        0        0     1912 2023-10-07 11:55:26.000000 jinjanator-23.7.0/tests/test_yaml_input.py
--rw-r--r--   0        0        0     1541 2023-10-07 11:55:26.000000 jinjanator-23.7.0/tests/test_plugin/jinjanator_test_plugin.py
--rw-r--r--   0        0        0      588 2023-10-07 11:55:26.000000 jinjanator-23.7.0/tests/test_plugin/pyproject.toml
--rw-r--r--   0        0        0       58 2023-10-07 11:55:26.000000 jinjanator-23.7.0/.gitignore
--rw-r--r--   0        0        0    11357 2023-10-07 11:55:26.000000 jinjanator-23.7.0/LICENSE.apache-2.0
--rw-r--r--   0        0        0     1321 2023-10-07 11:55:26.000000 jinjanator-23.7.0/LICENSE.bsd-2-clause
--rw-r--r--   0        0        0     7098 2023-10-07 11:55:26.000000 jinjanator-23.7.0/pyproject.toml
--rw-r--r--   0        0        0     9119 2023-10-07 11:55:26.000000 jinjanator-23.7.0/PKG-INFO
+-rw-r--r--   0        0        0     3123 2024-04-27 15:34:19.000000 jinjanator-24.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0    10319 2024-04-27 15:34:19.000000 jinjanator-24.1.0/README.md
+-rw-r--r--   0        0        0       81 2024-04-27 15:34:19.000000 jinjanator-24.1.0/src/jinjanator/__init__.py
+-rw-r--r--   0        0        0    12213 2024-04-27 15:34:19.000000 jinjanator-24.1.0/src/jinjanator/cli.py
+-rw-r--r--   0        0        0      692 2024-04-27 15:34:19.000000 jinjanator-24.1.0/src/jinjanator/context.py
+-rw-r--r--   0        0        0     1186 2024-04-27 15:34:19.000000 jinjanator-24.1.0/src/jinjanator/filters.py
+-rw-r--r--   0        0        0     7166 2024-04-27 15:34:19.000000 jinjanator-24.1.0/src/jinjanator/formats.py
+-rw-r--r--   0        0        0        0 2024-04-27 15:34:19.000000 jinjanator-24.1.0/src/jinjanator/py.typed
+-rw-r--r--   0        0        0      413 2024-04-27 15:34:19.000000 jinjanator-24.1.0/src/jinjanator/version.py
+-rw-r--r--   0        0        0     1614 2024-04-27 15:34:19.000000 jinjanator-24.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      675 2024-04-27 15:34:19.000000 jinjanator-24.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     1723 2024-04-27 15:34:19.000000 jinjanator-24.1.0/tests/test_argparse.py
+-rw-r--r--   0        0        0     2888 2024-04-27 15:34:19.000000 jinjanator-24.1.0/tests/test_cli.py
+-rw-r--r--   0        0        0     2723 2024-04-27 15:34:19.000000 jinjanator-24.1.0/tests/test_env.py
+-rw-r--r--   0        0        0      248 2024-04-27 15:34:19.000000 jinjanator-24.1.0/tests/test_extension.py
+-rw-r--r--   0        0        0     1101 2024-04-27 15:34:19.000000 jinjanator-24.1.0/tests/test_format_options.py
+-rw-r--r--   0        0        0      865 2024-04-27 15:34:19.000000 jinjanator-24.1.0/tests/test_invalid_data.py
+-rw-r--r--   0        0        0     1886 2024-04-27 15:34:19.000000 jinjanator-24.1.0/tests/test_json_input.py
+-rw-r--r--   0        0        0     3461 2024-04-27 15:34:19.000000 jinjanator-24.1.0/tests/test_nginx_config.py
+-rw-r--r--   0        0        0      780 2024-04-27 15:34:19.000000 jinjanator-24.1.0/tests/test_output_file.py
+-rw-r--r--   0        0        0      435 2024-04-27 15:34:19.000000 jinjanator-24.1.0/tests/test_template_not_found.py
+-rw-r--r--   0        0        0      501 2024-04-27 15:34:19.000000 jinjanator-24.1.0/tests/test_undefined.py
+-rw-r--r--   0        0        0      728 2024-04-27 15:34:19.000000 jinjanator-24.1.0/tests/test_unicode.py
+-rw-r--r--   0        0        0     1912 2024-04-27 15:34:19.000000 jinjanator-24.1.0/tests/test_yaml_input.py
+-rw-r--r--   0        0        0     1679 2024-04-27 15:34:19.000000 jinjanator-24.1.0/tests/test_plugin/jinjanator_test_plugin.py
+-rw-r--r--   0        0        0      588 2024-04-27 15:34:19.000000 jinjanator-24.1.0/tests/test_plugin/pyproject.toml
+-rw-r--r--   0        0        0       70 2024-04-27 15:34:19.000000 jinjanator-24.1.0/.gitignore
+-rw-r--r--   0        0        0    11357 2024-04-27 15:34:19.000000 jinjanator-24.1.0/LICENSE.apache-2.0
+-rw-r--r--   0        0        0     1321 2024-04-27 15:34:19.000000 jinjanator-24.1.0/LICENSE.bsd-2-clause
+-rw-r--r--   0        0        0     7064 2024-04-27 15:34:19.000000 jinjanator-24.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9191 2024-04-27 15:34:19.000000 jinjanator-24.1.0/PKG-INFO
```

### Comparing `jinjanator-23.7.0/CHANGELOG.md` & `jinjanator-24.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,21 @@
 This changelog is managed by towncrier and is compiled at release time.
 
 See https://github.com/kpfleming/jinjanator/blob/main/.github/CONTRIBUTING.md#changelog for details.
 -->
 
 <!-- towncrier release notes start -->
 
+## [24.1.0](https://github.com/kpfleming/jinjanator/tree/24.1.0) - 2024-04-27
+
+### Additions
+
+- Support for 'extensions' plugins which enable Jinja2 extensions (contributed by @llange)
+  [#29](https://github.com/kpfleming/jinjanator/issues/29)
+
 ## [23.7.0](https://github.com/kpfleming/jinjanator/tree/23.7.0) - 2023-10-07
 
 ### Additions
 
 - Added Python 3.12 support.
   [#23](https://github.com/kpfleming/jinjanator/issues/23)
```

### Comparing `jinjanator-23.7.0/README.md` & `jinjanator-24.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # jinjanator
 
 <a href="https://opensource.org"><img height="150" align="left" src="https://opensource.org/files/OSIApprovedCropped.png" alt="Open Source Initiative Approved License logo"></a>
 [![CI](https://github.com/kpfleming/jinjanator/workflows/CI%20checks/badge.svg)](https://github.com/kpfleming/jinjanator/actions?query=workflow%3ACI%20checks)
 [![Python](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-3812/)
 [![License - Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-9400d3.svg)](https://spdx.org/licenses/Apache-2.0.html)
-[![Code Style - Black](https://img.shields.io/badge/Code%20Style-Black-000000.svg)](https://github.com/psf/black)
 [![Types - Mypy](https://img.shields.io/badge/Types-Mypy-blue.svg)](https://github.com/python/mypy)
-[![Code Quality - Ruff](https://img.shields.io/badge/Code%20Quality-Ruff-red.svg)](https://github.com/astral-sh/ruff)
+[![Code Style and Quality - Ruff](https://img.shields.io/badge/Code%20Quality-Ruff-red.svg)](https://github.com/astral-sh/ruff)
 [![Project Management - Hatch](https://img.shields.io/badge/Project%20Management-Hatch-purple.svg)](https://github.com/pypa/hatch)
 [![Testing - Pytest](https://img.shields.io/badge/Testing-Pytest-orange.svg)](https://github.com/pytest-dev/pytest)
 
 This repo contains `jinjanator`, a CLI tool to render
 [Jinja2](https://github.com/pallets/jinja/) templates. It is a fork of
 `j2cli`, which itself was a fork of `jinja2-cli`, both of which are no
 longer actively maintained.
@@ -21,15 +20,15 @@
 
 <!-- fancy-readme start -->
 Features:
 
 * Jinja2 templating
 * INI, YAML, JSON data sources supported
 * Environment variables can be used with or without data files
-* Plugins can provide additional formats, filters, tests, and global
+* Plugins can provide additional formats, filters, tests, extensions and global
   functions (see
   [jinjanator-plugins](https://github.com/kpfleming/jinjanator-plugins)
   for details)
 
 ## Installation
 
 ```
@@ -351,15 +350,15 @@
 
 Notice that there must be quotes around the environment variable name
 when it is a literal string.
 <!-- fancy-readme end -->
 
 ## Chat
 
-If you'd like to chat with the Jinjanator community, join us on
+If you'd like to chat with the jinjanator community, join us on
 [Matrix](https://matrix.to/#/#jinjanator:km6g.us)!
 
 ## Credits
 
 This tool was created from [j2cli](https://github.com/kolypto/j2cli),
 which itself was created from
 [jinja2-cli](https://github.com/mattrobenolt/jinja2-cli). It was
@@ -372,15 +371,14 @@
 could not be more true than it is in the Python community; this
 project relies on many wonderful tools and libraries produced by the
 global open source software community, in addition to Python
 itself. I've listed many of them below, but if I've overlooked any
 please do not be offended :-)
 
 * [Attrs](https://pypi.org/project/attrs)
-* [Black](https://pypi.org/project/black)
 * [Hatch-Fancy-PyPI-Readme](https://pypi.org/project/hatch-fancy-pypi-readme)
 * [Hatch](https://pypi.org/project/hatch)
 * [Jinja2](https://pypi.org/project/jinja2/)
 * [Mypy](https://pypi.org/project/mypy)
 * [Pluggy](https://pypi.org/project/pluggy)
 * [pyproject-fmt](https://pypi.org/project/pyproject-fmt)
 * [Pytest](https://pypi.org/project/pytest)
```

#### html2text {}

```diff
@@ -1,29 +1,28 @@
 # jinjanator _[_O_p_e_n_ _S_o_u_r_c_e_ _I_n_i_t_i_a_t_i_v_e_ _A_p_p_r_o_v_e_d_ _L_i_c_e_n_s_e_ _l_o_g_o_][![CI](https://
 github.com/kpfleming/jinjanator/workflows/CI%20checks/badge.svg)](https://
 github.com/kpfleming/jinjanator/actions?query=workflow%3ACI%20checks) [!
 [Python](https://img.shields.io/badge/python-3.8+-blue.svg)](https://
 www.python.org/downloads/release/python-3812/) [![License - Apache 2.0](https:/
 /img.shields.io/badge/License-Apache%202.0-9400d3.svg)](https://spdx.org/
-licenses/Apache-2.0.html) [![Code Style - Black](https://img.shields.io/badge/
-Code%20Style-Black-000000.svg)](https://github.com/psf/black) [![Types - Mypy]
-(https://img.shields.io/badge/Types-Mypy-blue.svg)](https://github.com/python/
-mypy) [![Code Quality - Ruff](https://img.shields.io/badge/Code%20Quality-Ruff-
-red.svg)](https://github.com/astral-sh/ruff) [![Project Management - Hatch]
-(https://img.shields.io/badge/Project%20Management-Hatch-purple.svg)](https://
+licenses/Apache-2.0.html) [![Types - Mypy](https://img.shields.io/badge/Types-
+Mypy-blue.svg)](https://github.com/python/mypy) [![Code Style and Quality -
+Ruff](https://img.shields.io/badge/Code%20Quality-Ruff-red.svg)](https://
+github.com/astral-sh/ruff) [![Project Management - Hatch](https://
+img.shields.io/badge/Project%20Management-Hatch-purple.svg)](https://
 github.com/pypa/hatch) [![Testing - Pytest](https://img.shields.io/badge/
 Testing-Pytest-orange.svg)](https://github.com/pytest-dev/pytest) This repo
 contains `jinjanator`, a CLI tool to render [Jinja2](https://github.com/
 pallets/jinja/) templates. It is a fork of `j2cli`, which itself was a fork of
 `jinja2-cli`, both of which are no longer actively maintained. Open Source
 software: [Apache License 2.0](https://spdx.org/licenses/Apache-2.0.html) ##  
 Features: * Jinja2 templating * INI, YAML, JSON data sources supported *
 Environment variables can be used with or without data files * Plugins can
-provide additional formats, filters, tests, and global functions (see
-[jinjanator-plugins](https://github.com/kpfleming/jinjanator-plugins) for
+provide additional formats, filters, tests, extensions and global functions
+(see [jinjanator-plugins](https://github.com/kpfleming/jinjanator-plugins) for
 details) ## Installation ``` pip install jinjanator ``` ## Available Plugins *
 [jinjanator-plugin-ansible](https://pypi.org/project/jinjanator-plugin-ansible)
 - makes Ansible's 'core' filters and tests available during template rendering
 * [jinjanator-plugin-format-toml](https://pypi.org/project/jinjanator-plugin-
 format-toml) - provides a TOML parser for input data files * [jinjanator-
 plugin-format-xml](https://pypi.org/project/jinjanator-plugin-format-xml) -
 provides an XML parser for input data files ## Tutorial Suppose you have an
@@ -105,26 +104,25 @@
 variable's value in the template. This filter is available even when your data
 source is something other than the environment. Example: ```jinja2 User: {
 { user_login }} Pass: {{ "USER_PASSWORD" | env }} ``` You can provide a default
 value: ```jinja2 Pass: {{ "USER_PASSWORD" | env("-none-") }} ``` For your
 convenience, it's also available as a global function: ```jinja2 User: {
 { user_login }} Pass: {{ env("USER_PASSWORD") }} ``` Notice that there must be
 quotes around the environment variable name when it is a literal string. ##
-Chat If you'd like to chat with the Jinjanator community, join us on [Matrix]
+Chat If you'd like to chat with the jinjanator community, join us on [Matrix]
 (https://matrix.to/#/#jinjanator:km6g.us)! ## Credits This tool was created
 from [j2cli](https://github.com/kolypto/j2cli), which itself was created from
 [jinja2-cli](https://github.com/mattrobenolt/jinja2-cli). It was created to
 bring the project up to 'modern' Python coding, packaging, and project-
 management standards, and to support plugins to provide extensibility.
 ["Standing on the shoulders of giants"](https://en.wikipedia.org/wiki/
 Standing_on_the_shoulders_of_giants) could not be more true than it is in the
 Python community; this project relies on many wonderful tools and libraries
 produced by the global open source software community, in addition to Python
 itself. I've listed many of them below, but if I've overlooked any please do
-not be offended :-) * [Attrs](https://pypi.org/project/attrs) * [Black](https:/
-/pypi.org/project/black) * [Hatch-Fancy-PyPI-Readme](https://pypi.org/project/
-hatch-fancy-pypi-readme) * [Hatch](https://pypi.org/project/hatch) * [Jinja2]
-(https://pypi.org/project/jinja2/) * [Mypy](https://pypi.org/project/mypy) *
-[Pluggy](https://pypi.org/project/pluggy) * [pyproject-fmt](https://pypi.org/
-project/pyproject-fmt) * [Pytest](https://pypi.org/project/pytest) * [Ruff]
-(https://pypi.org/project/ruff) * [Towncrier](https://pypi.org/project/
-towncrier)
+not be offended :-) * [Attrs](https://pypi.org/project/attrs) * [Hatch-Fancy-
+PyPI-Readme](https://pypi.org/project/hatch-fancy-pypi-readme) * [Hatch](https:
+//pypi.org/project/hatch) * [Jinja2](https://pypi.org/project/jinja2/) * [Mypy]
+(https://pypi.org/project/mypy) * [Pluggy](https://pypi.org/project/pluggy) *
+[pyproject-fmt](https://pypi.org/project/pyproject-fmt) * [Pytest](https://
+pypi.org/project/pytest) * [Ruff](https://pypi.org/project/ruff) * [Towncrier]
+(https://pypi.org/project/towncrier)
```

### Comparing `jinjanator-23.7.0/src/jinjanator/cli.py` & `jinjanator-24.1.0/src/jinjanator/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,18 @@
 
         for plugin_filters in plugin_hook_callers.plugin_filters():
             self._env.filters.update(plugin_filters)
 
         for plugin_tests in plugin_hook_callers.plugin_tests():
             self._env.tests.update(plugin_tests)
 
+        for plugin_extensions in plugin_hook_callers.plugin_extensions():
+            for extension in plugin_extensions:
+                self._env.add_extension(extension)
+
     def render(self, template_name: str, context: Mapping[str, str]) -> str:
         return self._env.get_template(template_name).render(context)
 
 
 class UniqueStore(argparse.Action):
     """argparse action to restrict options to appearing only once."""
 
@@ -105,19 +109,20 @@
         if self.already_seen and option_string:
             parser.error(option_string + " cannot be specified more than once.")
         setattr(namespace, self.dest, values)
         self.already_seen = True
 
 
 def print_version_info(
-    stream: TextIO = sys.stderr, *, plugin_identities: Iterable[str]
+    stream: TextIO = sys.stderr,
+    *,
+    plugin_identities: Iterable[str],
 ) -> None:
     print(
-        f"{Path(sys.argv[0]).name} {version}, Jinja2"
-        f" {importlib.metadata.version('jinja2')}",
+        f"{Path(sys.argv[0]).name} {version}, Jinja2" f" {importlib.metadata.version('jinja2')}",
         file=stream,
     )
     header_printed = False
     for plugin in plugin_identities:
         if not header_printed:
             print("Plugins:", file=stream)
             header_printed = True
@@ -131,15 +136,19 @@
         option_strings: list[str],
         plugin_identities: Iterable[str],
         dest: str = argparse.SUPPRESS,
         default: str = argparse.SUPPRESS,
         help: str = "",  # noqa: A002
     ):
         super().__init__(
-            option_strings=option_strings, dest=dest, default=default, nargs=0, help=help
+            option_strings=option_strings,
+            dest=dest,
+            default=default,
+            nargs=0,
+            help=help,
         )
         self.plugin_identities = plugin_identities
 
     def __call__(
         self,
         parser: argparse.ArgumentParser,
         namespace: argparse.Namespace,  # noqa: ARG002
@@ -241,15 +250,16 @@
     pm.register(filters)
     pm.register(formats)
     pm.load_setuptools_entrypoints("jinjanator")
     return cast(jinjanator_plugins.PluginHookCallers, pm.hook)
 
 
 def validate_format_options(
-    fmt: type[jinjanator_plugins.Format], options: Sequence[str] | None
+    fmt: type[jinjanator_plugins.Format],
+    options: Sequence[str] | None,
 ) -> jinjanator_plugins.Format:
     if options:
         if not fmt.option_names:
             raise jinjanator_plugins.FormatOptionUnknownError(fmt, options[0])
 
         for opt in options:
             if opt.split("=")[0] not in fmt.option_names:
@@ -316,17 +326,15 @@
         if str(args.data) == "-":
             input_data_f = stdin
         elif args.data is None:
             input_data_f = None
         else:
             input_data_f = args.data.open()
     else:
-        input_data_f = (
-            stdin if args.data is None or str(args.data) == "-" else args.data.open()
-        )
+        input_data_f = stdin if args.data is None or str(args.data) == "-" else args.data.open()
 
     fmt = validate_format_options(available_formats[args.format], args.format_options)
 
     if args.format == "env" and input_data_f is None:
         context = environ
     else:
         context = read_context_data(
```

### Comparing `jinjanator-23.7.0/src/jinjanator/context.py` & `jinjanator-24.1.0/src/jinjanator/context.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.7.0/src/jinjanator/filters.py` & `jinjanator-24.1.0/src/jinjanator/filters.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.7.0/src/jinjanator/formats.py` & `jinjanator-24.1.0/src/jinjanator/formats.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,20 +65,26 @@
         self.array_name: str | None = None
         if options:
             for option in options:
                 try:
                     opt, val = option.split("=")
                 except ValueError as exc:
                     raise FormatOptionValueError(
-                        self, option, "", "contains more than one '='"
+                        self,
+                        option,
+                        "",
+                        "contains more than one '='",
                     ) from exc
 
                 if not val.isidentifier():
                     raise FormatOptionValueError(
-                        self, opt, val, "is not a valid Python identifier"
+                        self,
+                        opt,
+                        val,
+                        "is not a valid Python identifier",
                     )
 
                 if keyword.iskeyword(val):
                     raise FormatOptionValueError(self, opt, val, "is a Python keyword")
 
                 self.array_name = val
 
@@ -117,15 +123,17 @@
                     "cannot be used with object (dictionary) input",
                 )
 
             return context
 
         if not self.array_name:
             raise FormatOptionUnsupportedError(
-                self, "array-name", "must be specified for array (list) input"
+                self,
+                "array-name",
+                "must be specified for array (list) input",
             )
 
         return {self.array_name: context}
 
 
 class YAMLFormat:
     name = "yaml"
@@ -136,20 +144,26 @@
         self.sequence_name: str | None = None
         if options:
             for option in options:
                 try:
                     opt, val = option.split("=")
                 except ValueError as exc:
                     raise FormatOptionValueError(
-                        self, option, "", "contains more than one '='"
+                        self,
+                        option,
+                        "",
+                        "contains more than one '='",
                     ) from exc
 
                 if not val.isidentifier():
                     raise FormatOptionValueError(
-                        self, opt, val, "is not a valid Python identifier"
+                        self,
+                        opt,
+                        val,
+                        "is not a valid Python identifier",
                     )
 
                 if keyword.iskeyword(val):
                     raise FormatOptionValueError(self, opt, val, "is a Python keyword")
 
                 self.sequence_name = val
 
@@ -185,15 +199,17 @@
                 )
 
             return context
 
         if isinstance(context, list):
             if not self.sequence_name:
                 raise FormatOptionUnsupportedError(
-                    self, "sequence-name", "must be specified for sequence (array) input"
+                    self,
+                    "sequence-name",
+                    "must be specified for sequence (array) input",
                 )
 
             return {self.sequence_name: context}
 
         msg = "YAML input is neither a mapping nor a sequence"
         raise TypeError(msg)
 
@@ -231,18 +247,15 @@
 
         $ j2 config.j2 - < data.env
         """
 
         return dict(
             filter(
                 lambda line: len(line) == 2,  # noqa: PLR2004
-                (
-                    list(map(str.strip, line.split("=", 1)))
-                    for line in data_string.split("\n")
-                ),
+                (list(map(str.strip, line.split("=", 1))) for line in data_string.split("\n")),
             ),
         )
 
 
 @plugin_formats_hook
 def plugin_formats() -> Formats:
     return {
```

### Comparing `jinjanator-23.7.0/tests/__init__.py` & `jinjanator-24.1.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.7.0/tests/conftest.py` & `jinjanator-24.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.7.0/tests/test_argparse.py` & `jinjanator-24.1.0/tests/test_argparse.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,17 @@
         self,
         data_string: str,  # noqa: ARG002
     ) -> Mapping[str, str]:
         return {"foo": "bar"}
 
 
 def test_invalid_arg() -> None:
-    """Ensure that an invalid argument is not accepted."""
+    """
+    Ensure that an invalid argument is not accepted.
+    """
     with pytest.raises(SystemExit):
         parse_args({}, [], ["--test-invalid-arg"])
 
 
 @pytest.mark.parametrize(
     "args",
     [
@@ -39,29 +41,35 @@
         ["--undefined"],
         ["-e", "env"],
         ["-f", "env"],
         ["-o", "output"],
     ],
 )
 def test_args(args: list[str]) -> None:
-    """Ensure that known arguments are accepted."""
+    """
+    Ensure that known arguments are accepted.
+    """
     parse_args({"env": FakeFormat}, [], [*args, "template"])
 
 
 def test_version() -> None:
-    """Ensure that '--version' argument is accepted and program exits without an error."""
+    """
+    Ensure that '--version' argument is accepted and program exits without an error.
+    """
     with pytest.raises(SystemExit) as excinfo:
         parse_args({}, [], ["--version"])
     assert 0 == excinfo.value.code
 
 
 @pytest.mark.xfail()
 @pytest.mark.parametrize(
     "args",
     [
         ["--format", "env", "-f", "env"],
         ["--import-env", "env", "-e", "env"],
     ],
 )
 def test_duplicate_args(args: list[str]) -> None:
-    """Ensure that duplicate arguments are not accepted."""
+    """
+    Ensure that duplicate arguments are not accepted.
+    """
     parse_args({"env": FakeFormat}, [], [*args, "template"])
```

### Comparing `jinjanator-23.7.0/tests/test_cli.py` & `jinjanator-24.1.0/tests/test_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,61 +21,68 @@
 
 def test_unavailable_suffix(make_file_pair: FilePairFactory, capsys: Any) -> None:
     files = make_file_pair("Hello {{name}}!", "name=Blart", "xyz")
     with pytest.raises(
         SystemExit,
     ):
         render_file(files, [])
-    assert (
-        "No format which can read '.xyz' files available"
-        == capsys.readouterr().err.strip()
-    )
+    assert "No format which can read '.xyz' files available" == capsys.readouterr().err.strip()
 
 
 def test_main_normal(make_file_pair: FilePairFactory, capsys: Any) -> None:
     files = make_file_pair("Hello {{name}}!", "name=Blart", "env")
-    assert (
-        jinjanator.cli.main(["", str(files.template_file), str(files.data_file)]) is None
-    )
+    assert jinjanator.cli.main(["", str(files.template_file), str(files.data_file)]) is None
     assert "Hello Blart!" == capsys.readouterr().out
 
 
 def test_main_failure(make_file_pair: FilePairFactory) -> None:
     files = make_file_pair("Hello {{name}}!", "name=Blart", "xyz")
-    assert 1 == jinjanator.cli.main(["", str(files.template_file), str(files.data_file)])
+    assert 1 == jinjanator.cli.main(
+        ["", str(files.template_file), str(files.data_file)],
+    )
 
 
 def test_main_version(capsys: Any) -> None:
-    """Ensure that the 'test' plugin's identity string is included in the '--version' output."""
+    """
+    Ensure that the 'test' plugin's identity string is included in the '--version' output.
+    """
     assert 0 == jinjanator.cli.main(["", "--version"])
     outlines = capsys.readouterr().out.splitlines()
     assert "Plugins:" == outlines[1]
     assert "   test" == outlines[2]
 
 
 @pytest.mark.noplugin()
 def test_main_version_no_plugins(capsys: Any) -> None:
-    """Ensure that the 'test' plugin's identity string is not included in the '--version' output."""
+    """
+    Ensure that the 'test' plugin's identity string is not included in the '--version' output.
+    """
     assert 0 == jinjanator.cli.main(["", "--version"])
     outlines = capsys.readouterr().out.splitlines()
     assert 1 == len(outlines)
 
 
 def test_main_format_option_unknown(make_file_pair: FilePairFactory) -> None:
     files = make_file_pair("Hello {{name}}!", "name=Blart", "null")
     assert 2 == jinjanator.cli.main(  # noqa: PLR2004
-        ["", "--format-option", "midge", str(files.template_file), str(files.data_file)]
+        [
+            "",
+            "--format-option",
+            "midge",
+            str(files.template_file),
+            str(files.data_file),
+        ],
     )
 
 
 def test_main_format_option_unsupported(make_file_pair: FilePairFactory) -> None:
     files = make_file_pair("Hello {{name}}!", "name=Blart", "null")
     assert 3 == jinjanator.cli.main(  # noqa: PLR2004
-        ["", "--format-option", "uns", str(files.template_file), str(files.data_file)]
+        ["", "--format-option", "uns", str(files.template_file), str(files.data_file)],
     )
 
 
 def test_main_format_option_value_error(make_file_pair: FilePairFactory) -> None:
     files = make_file_pair("Hello {{name}}!", "name=Blart", "null")
     assert 4 == jinjanator.cli.main(  # noqa: PLR2004
-        ["", "--format-option", "val", str(files.template_file), str(files.data_file)]
+        ["", "--format-option", "val", str(files.template_file), str(files.data_file)],
     )
```

### Comparing `jinjanator-23.7.0/tests/test_env.py` & `jinjanator-24.1.0/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.7.0/tests/test_format_options.py` & `jinjanator-24.1.0/tests/test_format_options.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.7.0/tests/test_invalid_data.py` & `jinjanator-24.1.0/tests/test_invalid_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,18 @@
     with pytest.raises(TypeError, match="JSON input is neither an object nor an array"):
         assert render_file(files, [])
 
 
 def test_invalid_yaml(make_file_pair: FilePairFactory) -> None:
     files = make_file_pair("", "midge", "yaml")
 
-    with pytest.raises(TypeError, match="YAML input is neither a mapping nor a sequence"):
+    with pytest.raises(
+        TypeError,
+        match="YAML input is neither a mapping nor a sequence",
+    ):
         assert render_file(files, [])
 
 
 def test_no_input_data(make_file_pair: FilePairFactory) -> None:
     files = make_file_pair("", "", "yaml")
 
     with pytest.raises(ValueError, match="no input supplied"):
```

### Comparing `jinjanator-23.7.0/tests/test_json_input.py` & `jinjanator-24.1.0/tests/test_json_input.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.7.0/tests/test_nginx_config.py` & `jinjanator-24.1.0/tests/test_nginx_config.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.7.0/tests/test_output_file.py` & `jinjanator-24.1.0/tests/test_output_file.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.7.0/tests/test_unicode.py` & `jinjanator-24.1.0/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.7.0/tests/test_yaml_input.py` & `jinjanator-24.1.0/tests/test_yaml_input.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.7.0/tests/test_plugin/jinjanator_test_plugin.py` & `jinjanator-24.1.0/tests/test_plugin/jinjanator_test_plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from __future__ import annotations
 
 from typing import Iterable, Mapping
 
 from jinjanator_plugins import (
+    Extensions,
     Filters,
     FormatOptionUnsupportedError,
     FormatOptionValueError,
     Formats,
     Globals,
     Identity,
     Tests,
+    plugin_extensions_hook,
     plugin_filters_hook,
     plugin_formats_hook,
     plugin_globals_hook,
     plugin_identity_hook,
     plugin_tests_hook,
 )
 
@@ -69,7 +71,12 @@
 def plugin_formats() -> Formats:
     return {NullFormat.name: NullFormat}
 
 
 @plugin_globals_hook
 def plugin_globals() -> Globals:
     return {"null": null_filter}
+
+
+@plugin_extensions_hook
+def plugin_extensions() -> Extensions:
+    return ["jinja2.ext.do"]
```

### Comparing `jinjanator-23.7.0/tests/test_plugin/pyproject.toml` & `jinjanator-24.1.0/tests/test_plugin/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jinjanator-23.7.0/LICENSE.apache-2.0` & `jinjanator-24.1.0/LICENSE.apache-2.0`

 * *Files identical despite different names*

### Comparing `jinjanator-23.7.0/LICENSE.bsd-2-clause` & `jinjanator-24.1.0/LICENSE.bsd-2-clause`

 * *Files identical despite different names*

### Comparing `jinjanator-23.7.0/pyproject.toml` & `jinjanator-24.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 dynamic = [
   "readme",
   "version",
 ]
 dependencies = [
   "attrs",
   "jinja2>=2.7.2",
-  "jinjanator-plugins==23.4.*",
+  "jinjanator-plugins==24.1.*",
   "PyYAML",
   "typing-extensions",
 ]
 [project.urls]
 "Bug Tracker" = "https://github.com/kpfleming/jinjanator/issues"
 "Homepage" = "https://github.com/kpfleming/jinjanator"
 [project.scripts]
@@ -91,34 +91,33 @@
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
     "pytest", # needed for type-checking tests
     "types-PyYAML",
 ]
 
 [tool.hatch.envs.lint.scripts]
 lint = [
-     "ruff check --fix --show-fixes .",
-     "black --preview .",
+     "ruff format",
+     "ruff check --output-format=full --fix --show-fixes",
      "mypy --package jinjanator",
      "mypy tests",
      "shellcheck workflow-support/*.sh",
      "pyproject-fmt pyproject.toml tests/test_plugin/pyproject.toml",
 ]
 lint-action = [
-     "ruff check --output-format=github .",
-     "black --check --diff --preview .",
+     "ruff format --check --diff",
+     "ruff check --output-format=github",
      "mypy --package jinjanator",
      "mypy tests",
      "shellcheck workflow-support/*.sh",
      "pyproject-fmt --check pyproject.toml tests/test_plugin/pyproject.toml",
 ]
 
 [tool.hatch.envs.ci]
@@ -188,48 +187,45 @@
 pattern = '\[(.+?)\]\(((?!https?://)\S+?)\)'
 replacement = '[\1](https://github.com/kpfleming/jinjanator/tree/main/\g<2>)'
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.substitutions]]
 pattern = "#(\\d+)"
 replacement = "[#\\1](https://github.com/kpfleming/jinjanator/issues/\\1)"
 
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
 "src/jinjanator/cli.py" = ["T201"]
 "tests/*" = [
   "PLC1901", # empty strings are falsey, but are less specific in tests
   "PT005",   # we use always underscores and explicit names
   "S101",    # assert
   "SIM300",  # Yoda rocks in tests
 ]
 "tests/test_plugin/*" = [
   "INP001",  # we don't care that these are in implicit namespace packages
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 lines-between-types = 1
 lines-after-imports = 2
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 xfail_strict = true
 testpaths = [
@@ -239,34 +235,14 @@
     "-ra",
     "--strict-markers",
 ]
 markers = [
     "noplugin: tests which must run without plugins installed",
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
-exclude = ['tests/test_plugin/build']
-
 [tool.towncrier]
 name = "jinjanator"
 package = "jinjanator"
 directory = "changelog.d"
 filename = "CHANGELOG.md"
 start_string = "<!-- towncrier release notes start -->\n"
 template = "changelog.d/towncrier_template.md.jinja"
@@ -297,7 +273,27 @@
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
+exclude = ['tests/test_plugin/build']
```

### Comparing `jinjanator-23.7.0/PKG-INFO` & `jinjanator-24.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jinjanator
-Version: 23.7.0
+Version: 24.1.0
 Summary: Command-line interface to Jinja2 for templating in shell scripts.
 Project-URL: Bug Tracker, https://github.com/kpfleming/jinjanator/issues
 Project-URL: Homepage, https://github.com/kpfleming/jinjanator
 Author-email: "Kevin P. Fleming" <jinjanator@kevin.km6g.us>, Mark Vartanyan <kolypto@gmail.com>
 License: Apache-2.0
 License-File: LICENSE.apache-2.0
 License-File: LICENSE.bsd-2-clause
@@ -20,28 +20,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: attrs
 Requires-Dist: jinja2>=2.7.2
-Requires-Dist: jinjanator-plugins==23.4.*
+Requires-Dist: jinjanator-plugins==24.1.*
 Requires-Dist: pyyaml
 Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # *jinjanator*: CLI tool for rendering Jinja2 templates
 
 
 Features:
 
 * Jinja2 templating
 * INI, YAML, JSON data sources supported
 * Environment variables can be used with or without data files
-* Plugins can provide additional formats, filters, tests, and global
+* Plugins can provide additional formats, filters, tests, extensions and global
   functions (see
   [jinjanator-plugins](https://github.com/kpfleming/jinjanator-plugins)
   for details)
 
 ## Installation
 
 ```
@@ -362,13 +362,12 @@
 ```
 
 Notice that there must be quotes around the environment variable name
 when it is a literal string.
 ## Release Information
 ### Additions
 
-- Added Python 3.12 support.
-  [[#23](https://github.com/kpfleming/jinjanator/issues/23)](https://github.com/kpfleming/jinjanator/issues/23)
-
+- Support for 'extensions' plugins which enable Jinja2 extensions (contributed by @llange)
+  [[#29](https://github.com/kpfleming/jinjanator/issues/29)](https://github.com/kpfleming/jinjanator/issues/29)
 
 ---
 [→ Full Changelog](https://github.com/kpfleming/jinjanator/blob/main/CHANGELOG.md)
```

