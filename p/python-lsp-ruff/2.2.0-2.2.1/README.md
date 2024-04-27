# Comparing `tmp/python-lsp-ruff-2.2.0.tar.gz` & `tmp/python_lsp_ruff-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-lsp-ruff-2.2.0.tar", last modified: Fri Mar  1 10:43:29 2024, max compression
+gzip compressed data, was "python_lsp_ruff-2.2.1.tar", last modified: Sat Apr 27 13:05:29 2024, max compression
```

## Comparing `python-lsp-ruff-2.2.0.tar` & `python_lsp_ruff-2.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2024-03-01 10:43:29.874785 python-lsp-ruff-2.2.0/
--rw-r--r--   0 juli      (1000) juli      (1000)     1138 2023-11-16 22:00:31.000000 python-lsp-ruff-2.2.0/LICENSE
--rw-r--r--   0 juli      (1000) juli      (1000)     5869 2024-03-01 10:43:29.874785 python-lsp-ruff-2.2.0/PKG-INFO
--rw-r--r--   0 juli      (1000) juli      (1000)     5190 2024-02-09 09:37:43.000000 python-lsp-ruff-2.2.0/README.md
-drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2024-03-01 10:43:29.874785 python-lsp-ruff-2.2.0/pylsp_ruff/
--rw-r--r--   0 juli      (1000) juli      (1000)        0 2023-11-16 22:00:31.000000 python-lsp-ruff-2.2.0/pylsp_ruff/__init__.py
--rw-r--r--   0 juli      (1000) juli      (1000)    21563 2024-03-01 10:40:40.000000 python-lsp-ruff-2.2.0/pylsp_ruff/plugin.py
--rw-r--r--   0 juli      (1000) juli      (1000)      459 2023-11-16 22:00:31.000000 python-lsp-ruff-2.2.0/pylsp_ruff/ruff.py
--rw-r--r--   0 juli      (1000) juli      (1000)     1816 2024-03-01 10:40:40.000000 python-lsp-ruff-2.2.0/pylsp_ruff/settings.py
--rw-r--r--   0 juli      (1000) juli      (1000)      792 2024-03-01 10:43:03.000000 python-lsp-ruff-2.2.0/pyproject.toml
-drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2024-03-01 10:43:29.874785 python-lsp-ruff-2.2.0/python_lsp_ruff.egg-info/
--rw-r--r--   0 juli      (1000) juli      (1000)     5869 2024-03-01 10:43:29.000000 python-lsp-ruff-2.2.0/python_lsp_ruff.egg-info/PKG-INFO
--rw-r--r--   0 juli      (1000) juli      (1000)      440 2024-03-01 10:43:29.000000 python-lsp-ruff-2.2.0/python_lsp_ruff.egg-info/SOURCES.txt
--rw-r--r--   0 juli      (1000) juli      (1000)        1 2024-03-01 10:43:29.000000 python-lsp-ruff-2.2.0/python_lsp_ruff.egg-info/dependency_links.txt
--rw-r--r--   0 juli      (1000) juli      (1000)       33 2024-03-01 10:43:29.000000 python-lsp-ruff-2.2.0/python_lsp_ruff.egg-info/entry_points.txt
--rw-r--r--   0 juli      (1000) juli      (1000)      132 2024-03-01 10:43:29.000000 python-lsp-ruff-2.2.0/python_lsp_ruff.egg-info/requires.txt
--rw-r--r--   0 juli      (1000) juli      (1000)       11 2024-03-01 10:43:29.000000 python-lsp-ruff-2.2.0/python_lsp_ruff.egg-info/top_level.txt
--rw-r--r--   0 juli      (1000) juli      (1000)       38 2024-03-01 10:43:29.878118 python-lsp-ruff-2.2.0/setup.cfg
--rw-r--r--   0 juli      (1000) juli      (1000)       69 2023-11-16 22:00:31.000000 python-lsp-ruff-2.2.0/setup.py
-drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2024-03-01 10:43:29.874785 python-lsp-ruff-2.2.0/tests/
--rw-r--r--   0 juli      (1000) juli      (1000)     4038 2023-11-25 13:13:27.000000 python-lsp-ruff-2.2.0/tests/test_code_actions.py
--rw-r--r--   0 juli      (1000) juli      (1000)     2830 2024-03-01 10:40:40.000000 python-lsp-ruff-2.2.0/tests/test_ruff_format.py
--rw-r--r--   0 juli      (1000) juli      (1000)     7809 2023-11-26 14:00:02.000000 python-lsp-ruff-2.2.0/tests/test_ruff_lint.py
+drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2024-04-27 13:05:29.470031 python_lsp_ruff-2.2.1/
+-rw-r--r--   0 juli      (1000) juli      (1000)     1138 2023-11-16 22:00:31.000000 python_lsp_ruff-2.2.1/LICENSE
+-rw-r--r--   0 juli      (1000) juli      (1000)     6055 2024-04-27 13:05:29.470031 python_lsp_ruff-2.2.1/PKG-INFO
+-rw-r--r--   0 juli      (1000) juli      (1000)     5376 2024-03-15 08:41:15.000000 python_lsp_ruff-2.2.1/README.md
+drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2024-04-27 13:05:29.466698 python_lsp_ruff-2.2.1/pylsp_ruff/
+-rw-r--r--   0 juli      (1000) juli      (1000)        0 2023-11-16 22:00:31.000000 python_lsp_ruff-2.2.1/pylsp_ruff/__init__.py
+-rw-r--r--   0 juli      (1000) juli      (1000)    21668 2024-04-27 13:00:54.000000 python_lsp_ruff-2.2.1/pylsp_ruff/plugin.py
+-rw-r--r--   0 juli      (1000) juli      (1000)      459 2024-04-27 13:00:54.000000 python_lsp_ruff-2.2.1/pylsp_ruff/ruff.py
+-rw-r--r--   0 juli      (1000) juli      (1000)     1816 2024-03-01 10:40:40.000000 python_lsp_ruff-2.2.1/pylsp_ruff/settings.py
+-rw-r--r--   0 juli      (1000) juli      (1000)      792 2024-04-27 13:01:08.000000 python_lsp_ruff-2.2.1/pyproject.toml
+drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2024-04-27 13:05:29.470031 python_lsp_ruff-2.2.1/python_lsp_ruff.egg-info/
+-rw-r--r--   0 juli      (1000) juli      (1000)     6055 2024-04-27 13:05:29.000000 python_lsp_ruff-2.2.1/python_lsp_ruff.egg-info/PKG-INFO
+-rw-r--r--   0 juli      (1000) juli      (1000)      440 2024-04-27 13:05:29.000000 python_lsp_ruff-2.2.1/python_lsp_ruff.egg-info/SOURCES.txt
+-rw-r--r--   0 juli      (1000) juli      (1000)        1 2024-04-27 13:05:29.000000 python_lsp_ruff-2.2.1/python_lsp_ruff.egg-info/dependency_links.txt
+-rw-r--r--   0 juli      (1000) juli      (1000)       33 2024-04-27 13:05:29.000000 python_lsp_ruff-2.2.1/python_lsp_ruff.egg-info/entry_points.txt
+-rw-r--r--   0 juli      (1000) juli      (1000)      132 2024-04-27 13:05:29.000000 python_lsp_ruff-2.2.1/python_lsp_ruff.egg-info/requires.txt
+-rw-r--r--   0 juli      (1000) juli      (1000)       11 2024-04-27 13:05:29.000000 python_lsp_ruff-2.2.1/python_lsp_ruff.egg-info/top_level.txt
+-rw-r--r--   0 juli      (1000) juli      (1000)       38 2024-04-27 13:05:29.470031 python_lsp_ruff-2.2.1/setup.cfg
+-rw-r--r--   0 juli      (1000) juli      (1000)       69 2023-11-16 22:00:31.000000 python_lsp_ruff-2.2.1/setup.py
+drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2024-04-27 13:05:29.470031 python_lsp_ruff-2.2.1/tests/
+-rw-r--r--   0 juli      (1000) juli      (1000)     4064 2024-04-27 13:00:54.000000 python_lsp_ruff-2.2.1/tests/test_code_actions.py
+-rw-r--r--   0 juli      (1000) juli      (1000)     2830 2024-03-01 10:40:40.000000 python_lsp_ruff-2.2.1/tests/test_ruff_format.py
+-rw-r--r--   0 juli      (1000) juli      (1000)     7809 2023-11-26 14:00:02.000000 python_lsp_ruff-2.2.1/tests/test_ruff_lint.py
```

### Comparing `python-lsp-ruff-2.2.0/LICENSE` & `python_lsp_ruff-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-lsp-ruff-2.2.0/PKG-INFO` & `python_lsp_ruff-2.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lsp-ruff
-Version: 2.2.0
+Version: 2.2.1
 Summary: Ruff linting plugin for pylsp
 Author-email: Julian Hossbach <julian.hossbach@gmx.de>
 License: MIT
 Project-URL: Homepage, https://github.com/python-lsp/python-lsp-ruff
 Project-URL: Bug Tracker, https://github.com/python-lsp/python-lsp-ruff/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -61,14 +61,15 @@
 This example configuration using for `neovim` shows the possible options:
 
 ```lua
 pylsp = {
   plugins = {
     ruff = {
       enabled = true,  -- Enable the plugin
+      formatEnabled = true,  -- Enable formatting using ruffs formatter
       executable = "<path-to-ruff-bin>",  -- Custom path to ruff
       config = "<path_to_custom_ruff_toml>",  -- Custom config for ruff to use
       extendSelect = { "I" },  -- Rules that are additionally used by ruff
       extendIgnore = { "C90" },  -- Rules that are additionally ignored by ruff
       format = { "I" },  -- Rules that are marked as fixable by ruff that should be fixed when running textDocument/formatting
       severities = { ["D212"] = "I" },  -- Optional table of rules where a custom severity is desired
       unsafeFixes = false,  -- Whether or not to offer unsafe fixes as code actions. Ignored with the "Fix All" action
@@ -97,16 +98,17 @@
 [the official LSP reference](https://microsoft.github.io/language-server-protocol/specifications/lsp/3.17/specification/#diagnosticSeverity).
 
 With `v2.0.0` it is also possible to use patterns to match codes. Rules match if the error code starts with the given pattern. If multiple patterns match the error code, `python-lsp-ruff` chooses the one with the most amount of matching characters.
 
 
 ## Code formatting
 
-With `python-lsp-ruff>1.6.0` formatting is done using [ruffs own formatter](https://docs.astral.sh/ruff/formatter/).
-In addition, rules that should be fixed during the `textDocument/formatting` request can be added with the `format` option.
+With `python-lsp-ruff>1.6.0` formatting is done using [ruffs own formatter](https://docs.astral.sh/ruff/formatter/) by default.
+Formatting using ruff can be explicitly disabled by setting `formatEnabled = false` in the LSP settings.
+Additional rules that should be fixed during the `textDocument/formatting` request can be added with the `format` option.
 
 Coming from previous versions the only change is that `isort` rules are **not** applied by default.
 To enable sorting of imports using ruff's isort functionality, add `"I"` to the list of `format` rules. 
 
 
 ## Code actions
```

### Comparing `python-lsp-ruff-2.2.0/README.md` & `python_lsp_ruff-2.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 This example configuration using for `neovim` shows the possible options:
 
 ```lua
 pylsp = {
   plugins = {
     ruff = {
       enabled = true,  -- Enable the plugin
+      formatEnabled = true,  -- Enable formatting using ruffs formatter
       executable = "<path-to-ruff-bin>",  -- Custom path to ruff
       config = "<path_to_custom_ruff_toml>",  -- Custom config for ruff to use
       extendSelect = { "I" },  -- Rules that are additionally used by ruff
       extendIgnore = { "C90" },  -- Rules that are additionally ignored by ruff
       format = { "I" },  -- Rules that are marked as fixable by ruff that should be fixed when running textDocument/formatting
       severities = { ["D212"] = "I" },  -- Optional table of rules where a custom severity is desired
       unsafeFixes = false,  -- Whether or not to offer unsafe fixes as code actions. Ignored with the "Fix All" action
@@ -77,16 +78,17 @@
 [the official LSP reference](https://microsoft.github.io/language-server-protocol/specifications/lsp/3.17/specification/#diagnosticSeverity).
 
 With `v2.0.0` it is also possible to use patterns to match codes. Rules match if the error code starts with the given pattern. If multiple patterns match the error code, `python-lsp-ruff` chooses the one with the most amount of matching characters.
 
 
 ## Code formatting
 
-With `python-lsp-ruff>1.6.0` formatting is done using [ruffs own formatter](https://docs.astral.sh/ruff/formatter/).
-In addition, rules that should be fixed during the `textDocument/formatting` request can be added with the `format` option.
+With `python-lsp-ruff>1.6.0` formatting is done using [ruffs own formatter](https://docs.astral.sh/ruff/formatter/) by default.
+Formatting using ruff can be explicitly disabled by setting `formatEnabled = false` in the LSP settings.
+Additional rules that should be fixed during the `textDocument/formatting` request can be added with the `format` option.
 
 Coming from previous versions the only change is that `isort` rules are **not** applied by default.
 To enable sorting of imports using ruff's isort functionality, add `"I"` to the list of `format` rules. 
 
 
 ## Code actions
```

### Comparing `python-lsp-ruff-2.2.0/pylsp_ruff/plugin.py` & `python_lsp_ruff-2.2.1/pylsp_ruff/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,23 +102,23 @@
         }
     }
     return converter.unstructure(settings)
 
 
 @hookimpl(hookwrapper=True)
 def pylsp_format_document(workspace: Workspace, document: Document) -> Generator:
-    """
-    Provide formatting through ruff.
+    """Provide formatting through ruff.
 
     Parameters
     ----------
     workspace : pylsp.workspace.Workspace
         Current workspace.
     document : pylsp.workspace.Document
         Document to apply ruff on.
+
     """
     log.debug(f"textDocument/formatting: {document}")
     outcome = yield
     result = outcome.get_result()
     if result:
         source = result[0]["newText"]
     else:
@@ -133,15 +133,17 @@
     )
 
     if settings.format:
         # A second pass through the document with `ruff check` and only the rules
         # enabled via the format config property. This allows for things like
         # specifying `format = ["I"]` to get import sorting as part of formatting.
         new_text = run_ruff(
-            settings=PluginSettings(ignore=["ALL"], select=settings.format),
+            settings=PluginSettings(
+                ignore=["ALL"], select=settings.format, executable=settings.executable
+            ),
             document_path=document.path,
             document_source=new_text,
             fix=True,
         )
 
     # Avoid applying empty text edit
     if not new_text or new_text == source:
@@ -154,48 +156,48 @@
     text_edit = TextEdit(range=range, new_text=new_text)
 
     outcome.force_result(converter.unstructure([text_edit]))
 
 
 @hookimpl
 def pylsp_lint(workspace: Workspace, document: Document) -> List[Dict]:
-    """
-    Register ruff as the linter.
+    """Register ruff as the linter.
 
     Parameters
     ----------
     workspace : pylsp.workspace.Workspace
         Current workspace.
     document : pylsp.workspace.Document
         Document to apply ruff on.
 
     Returns
     -------
     List of dicts containing the diagnostics.
+
     """
     settings = load_settings(workspace, document.path)
     checks = run_ruff_check(document=document, settings=settings)
     diagnostics = [create_diagnostic(check=c, settings=settings) for c in checks]
     return converter.unstructure(diagnostics)
 
 
 def create_diagnostic(check: RuffCheck, settings: PluginSettings) -> Diagnostic:
-    """
-    Create a LSP diagnostic based on the given RuffCheck object.
+    """Create a LSP diagnostic based on the given RuffCheck object.
 
     Parameters
     ----------
     check : RuffCheck
         RuffCheck object to convert.
     settings : PluginSettings
         Current settings.
 
     Returns
     -------
     Diagnostic
+
     """
     # Adapt range to LSP specification (zero-based)
     range = Range(
         start=Position(
             line=check.location.row - 1,
             character=check.location.column - 1,
         ),
@@ -244,16 +246,15 @@
 def pylsp_code_actions(
     config: Config,
     workspace: Workspace,
     document: Document,
     range: Dict,
     context: Dict,
 ) -> List[Dict]:
-    """
-    Provide code actions through ruff.
+    """Provide code actions through ruff.
 
     Parameters
     ----------
     config : pylsp.config.config.Config
         Current workspace.
     workspace : pylsp.workspace.Workspace
         Current workspace.
@@ -263,14 +264,15 @@
         Range argument given by pylsp. Not used here.
     context : Dict
         CodeActionContext given as dict.
 
     Returns
     -------
     List of dicts containing the code actions.
+
     """
     log.debug(f"textDocument/codeAction: {document} {range} {context}")
 
     _context = converter.structure(context, CodeActionContext)
     diagnostics = _context.diagnostics
 
     code_actions = []
@@ -318,15 +320,15 @@
                 create_organize_imports_code_action(
                     document=document, diagnostic=diagnostic, fix=fix
                 ),
                 create_disable_code_action(document=document, diagnostic=diagnostic),
             ]
         )
 
-    if checks_with_fixes:
+    if any([c.fix.applicability == "safe" for c in checks_with_fixes]):  # type: ignore
         code_actions.append(
             create_fix_all_code_action(document=document, settings=settings),
         )
 
     return converter.unstructure(code_actions)
 
 
@@ -401,15 +403,15 @@
     )
 
 
 def create_fix_all_code_action(
     document: Document,
     settings: PluginSettings,
 ) -> CodeAction:
-    title = "Ruff: Fix All"
+    title = "Ruff: Fix All (safe fixes)"
     kind = CodeActionKind.SourceFixAll
 
     # No unsafe fixes for 'Fix all', see https://github.com/python-lsp/python-lsp-ruff/issues/55
     settings.unsafe_fixes = False
 
     new_text = run_ruff_fix(document=document, settings=settings)
     range = Range(
@@ -483,16 +485,15 @@
     settings: PluginSettings,
     document_path: str,
     document_source: str,
     subcommand: Subcommand = Subcommand.CHECK,
     fix: bool = False,
     extra_arguments: Optional[List[str]] = None,
 ) -> str:
-    """
-    Run ruff on the given document and the given arguments.
+    """Run ruff on the given document and the given arguments.
 
     Parameters
     ----------
     settings : PluginSettings
         Settings to use.
     document_path : str
         Path to file to run ruff on.
@@ -505,14 +506,15 @@
         Whether to run fix or no-fix.
     extra_arguments : List[str]
         Extra arguments to pass to ruff.
 
     Returns
     -------
     String containing the result in json format.
+
     """
     executable = settings.executable
 
     arguments = subcommand.build_args(document_path, settings, fix, extra_arguments)
 
     p = None
     if executable is not None:
@@ -541,16 +543,15 @@
 
 def build_check_arguments(
     document_path: str,
     settings: PluginSettings,
     fix: bool = False,
     extra_arguments: Optional[List[str]] = None,
 ) -> List[str]:
-    """
-    Build arguments for ruff check.
+    """Build arguments for ruff check.
 
     Parameters
     ----------
     document : pylsp.workspace.Document
         Document to apply ruff on.
     settings : PluginSettings
         Settings to use for arguments to pass to ruff.
@@ -558,14 +559,15 @@
         Whether to execute with --fix.
     extra_arguments : List[str]
         Extra arguments to pass to ruff.
 
     Returns
     -------
     List containing the arguments.
+
     """
     args = []
     # Suppress update announcements
     args.append("--quiet")
     # Suppress exit 1 when violations were found
     args.append("--exit-zero")
     # Use the json formatting for easier evaluation
@@ -627,29 +629,29 @@
 
 
 def build_format_arguments(
     document_path: str,
     settings: PluginSettings,
     extra_arguments: Optional[List[str]] = None,
 ) -> List[str]:
-    """
-    Build arguments for ruff format.
+    """Build arguments for ruff format.
 
     Parameters
     ----------
     document : pylsp.workspace.Document
         Document to apply ruff on.
     settings : PluginSettings
         Settings to use for arguments to pass to ruff.
     extra_arguments : List[str]
         Extra arguments to pass to ruff.
 
     Returns
     -------
     List containing the arguments.
+
     """
     args = []
     # Suppress update announcements
     args.append("--quiet")
 
     # Always force excludes
     args.append("--force-exclude")
@@ -677,27 +679,27 @@
 
     args.extend(["--", "-"])
 
     return args
 
 
 def load_settings(workspace: Workspace, document_path: str) -> PluginSettings:
-    """
-    Load settings from pyproject.toml file in the project path.
+    """Load settings from pyproject.toml file in the project path.
 
     Parameters
     ----------
     workspace : pylsp.workspace.Workspace
         Current workspace.
     document_path : str
         Path to the document to apply ruff on.
 
     Returns
     -------
     PluginSettings read via lsp.
+
     """
     config = workspace._config
     _plugin_settings = config.plugin_settings("ruff", document_path=document_path)
     plugin_settings = converter.structure(_plugin_settings, PluginSettings)
 
     pyproject_file = find_parents(
         workspace.root_path, document_path, ["pyproject.toml"]
```

### Comparing `python-lsp-ruff-2.2.0/pylsp_ruff/settings.py` & `python_lsp_ruff-2.2.1/pylsp_ruff/settings.py`

 * *Files identical despite different names*

### Comparing `python-lsp-ruff-2.2.0/pyproject.toml` & `python_lsp_ruff-2.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-lsp-ruff"
 authors = [
   {name = "Julian Hossbach", email = "julian.hossbach@gmx.de"}
 ]
-version = "2.2.0"
+version = "2.2.1"
 description = "Ruff linting plugin for pylsp"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 dependencies = [
   "ruff>=0.2.0",
   "python-lsp-server",
```

### Comparing `python-lsp-ruff-2.2.0/python_lsp_ruff.egg-info/PKG-INFO` & `python_lsp_ruff-2.2.1/python_lsp_ruff.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lsp-ruff
-Version: 2.2.0
+Version: 2.2.1
 Summary: Ruff linting plugin for pylsp
 Author-email: Julian Hossbach <julian.hossbach@gmx.de>
 License: MIT
 Project-URL: Homepage, https://github.com/python-lsp/python-lsp-ruff
 Project-URL: Bug Tracker, https://github.com/python-lsp/python-lsp-ruff/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -61,14 +61,15 @@
 This example configuration using for `neovim` shows the possible options:
 
 ```lua
 pylsp = {
   plugins = {
     ruff = {
       enabled = true,  -- Enable the plugin
+      formatEnabled = true,  -- Enable formatting using ruffs formatter
       executable = "<path-to-ruff-bin>",  -- Custom path to ruff
       config = "<path_to_custom_ruff_toml>",  -- Custom config for ruff to use
       extendSelect = { "I" },  -- Rules that are additionally used by ruff
       extendIgnore = { "C90" },  -- Rules that are additionally ignored by ruff
       format = { "I" },  -- Rules that are marked as fixable by ruff that should be fixed when running textDocument/formatting
       severities = { ["D212"] = "I" },  -- Optional table of rules where a custom severity is desired
       unsafeFixes = false,  -- Whether or not to offer unsafe fixes as code actions. Ignored with the "Fix All" action
@@ -97,16 +98,17 @@
 [the official LSP reference](https://microsoft.github.io/language-server-protocol/specifications/lsp/3.17/specification/#diagnosticSeverity).
 
 With `v2.0.0` it is also possible to use patterns to match codes. Rules match if the error code starts with the given pattern. If multiple patterns match the error code, `python-lsp-ruff` chooses the one with the most amount of matching characters.
 
 
 ## Code formatting
 
-With `python-lsp-ruff>1.6.0` formatting is done using [ruffs own formatter](https://docs.astral.sh/ruff/formatter/).
-In addition, rules that should be fixed during the `textDocument/formatting` request can be added with the `format` option.
+With `python-lsp-ruff>1.6.0` formatting is done using [ruffs own formatter](https://docs.astral.sh/ruff/formatter/) by default.
+Formatting using ruff can be explicitly disabled by setting `formatEnabled = false` in the LSP settings.
+Additional rules that should be fixed during the `textDocument/formatting` request can be added with the `format` option.
 
 Coming from previous versions the only change is that `isort` rules are **not** applied by default.
 To enable sorting of imports using ruff's isort functionality, add `"I"` to the list of `format` rules. 
 
 
 ## Code actions
```

### Comparing `python-lsp-ruff-2.2.0/tests/test_code_actions.py` & `python_lsp_ruff-2.2.1/tests/test_code_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,20 +43,20 @@
 )
 
 codeactions = [
     "Ruff (F401): Remove unused import: `os`",
     "Ruff (F401): Disable for this line",
     "Ruff (F841): Remove assignment to unused variable `a` (unsafe)",
     "Ruff (F841): Disable for this line",
-    "Ruff: Fix All",
+    "Ruff: Fix All (safe fixes)",
 ]
 
 codeactions_import = [
     "Ruff: Organize imports",
-    "Ruff: Fix All",
+    "Ruff: Fix All (safe fixes)",
     "Ruff (I001): Disable for this line",
 ]
 
 
 def temp_document(doc_text, workspace):
     with tempfile.NamedTemporaryFile(
         mode="w", dir=workspace.root_path, delete=False
```

### Comparing `python-lsp-ruff-2.2.0/tests/test_ruff_format.py` & `python_lsp_ruff-2.2.1/tests/test_ruff_format.py`

 * *Files identical despite different names*

### Comparing `python-lsp-ruff-2.2.0/tests/test_ruff_lint.py` & `python_lsp_ruff-2.2.1/tests/test_ruff_lint.py`

 * *Files identical despite different names*

