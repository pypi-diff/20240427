# Comparing `tmp/bitwarden_import_msecure-1.7.0.tar.gz` & `tmp/bitwarden_import_msecure-1.7.1.tar.gz`

## Comparing `bitwarden_import_msecure-1.7.0.tar` & `bitwarden_import_msecure-1.7.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/.coveragerc
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/.flake8
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/.mypy.ini
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/.pylintrc
--rwxr-xr-x   0        0        0     1340 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/activate.sh
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/invoke.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/pytest.ini
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/requirements.dev.in
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/requirements.dev.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/requirements.in
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/requirements.txt
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/tasks.py
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/.github/workflows/pip_publish.yml
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/.github/workflows/static.yml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/docs/mkdocs.yml
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/docs/src/en/index.md
--rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/docs/src/ru/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/scripts/__init__.py
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/scripts/build-docs.sh
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/scripts/build.sh
--rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/scripts/docs-render-config.sh
--rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/scripts/include_pyproject_requirements.py
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/scripts/upload.sh
--rwxr-xr-x   0        0        0     2525 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/scripts/verup.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/src/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/__about__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/__init__.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/bitwarden_csv.py
--rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/bitwarden_json.py
--rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/main.py
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/msecure.py
--rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/msecure_to_bitwarden.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/tests/conftest.py
--rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/tests/test_bitwarden_import_msecure.py
--rw-r--r--   0        0        0     5666 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/tests/test_e2e.py
--rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/tests/resources/bitwarden_broken_export.json
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/tests/resources/bitwarden_export.csv
--rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/tests/resources/bitwarden_export.json
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/tests/resources/bitwarden_notes_export.csv
--rw-r--r--   0        0        0     5060 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/tests/resources/bitwarden_notes_export.json
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/tests/resources/bitwarden_patched_export.json
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/tests/resources/mSecure Export File.csv
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/LICENSE.txt
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/README.md
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/.coveragerc
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/.flake8
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/.mypy.ini
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/.pylintrc
+-rwxr-xr-x   0        0        0     1340 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/activate.sh
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/invoke.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/pytest.ini
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/requirements.dev.in
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/requirements.dev.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/requirements.in
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/requirements.txt
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/tasks.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/.github/workflows/pip_publish.yml
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/.github/workflows/static.yml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/docs/mkdocs.yml
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/docs/src/en/index.md
+-rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/docs/src/ru/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/scripts/__init__.py
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/scripts/build.sh
+-rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/scripts/docs-render-config.sh
+-rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/scripts/include_pyproject_requirements.py
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/scripts/upload.sh
+-rwxr-xr-x   0        0        0     2525 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/scripts/verup.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/src/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/src/bitwarden_import_msecure/__about__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/src/bitwarden_import_msecure/__init__.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/src/bitwarden_import_msecure/bitwarden_csv.py
+-rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/src/bitwarden_import_msecure/bitwarden_json.py
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/src/bitwarden_import_msecure/main.py
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/src/bitwarden_import_msecure/msecure.py
+-rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/src/bitwarden_import_msecure/msecure_to_bitwarden.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/tests/conftest.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/tests/test_bitwarden_import_msecure.py
+-rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/tests/test_e2e.py
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/tests/resources/bitwarden_broken_export.json
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/tests/resources/bitwarden_export.csv
+-rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/tests/resources/bitwarden_export.json
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/tests/resources/bitwarden_notes_export.csv
+-rw-r--r--   0        0        0     5060 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/tests/resources/bitwarden_notes_export.json
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/tests/resources/bitwarden_patched_export.json
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/tests/resources/mSecure Export File.csv
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/LICENSE.txt
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/README.md
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.1/PKG-INFO
```

### Comparing `bitwarden_import_msecure-1.7.0/.pre-commit-config.yaml` & `bitwarden_import_msecure-1.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/activate.sh` & `bitwarden_import_msecure-1.7.1/activate.sh`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/requirements.dev.txt` & `bitwarden_import_msecure-1.7.1/requirements.dev.txt`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/tasks.py` & `bitwarden_import_msecure-1.7.1/tasks.py`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/.github/workflows/ci.yml` & `bitwarden_import_msecure-1.7.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/.github/workflows/docs.yml` & `bitwarden_import_msecure-1.7.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/.github/workflows/pip_publish.yml` & `bitwarden_import_msecure-1.7.1/.github/workflows/pip_publish.yml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/.github/workflows/static.yml` & `bitwarden_import_msecure-1.7.1/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/docs/mkdocs.yml` & `bitwarden_import_msecure-1.7.1/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/docs/src/en/index.md` & `bitwarden_import_msecure-1.7.1/docs/src/en/index.md`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/docs/src/ru/index.md` & `bitwarden_import_msecure-1.7.1/docs/src/ru/index.md`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/scripts/include_pyproject_requirements.py` & `bitwarden_import_msecure-1.7.1/scripts/include_pyproject_requirements.py`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/scripts/verup.sh` & `bitwarden_import_msecure-1.7.1/scripts/verup.sh`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/bitwarden_csv.py` & `bitwarden_import_msecure-1.7.1/src/bitwarden_import_msecure/bitwarden_csv.py`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/bitwarden_json.py` & `bitwarden_import_msecure-1.7.1/src/bitwarden_import_msecure/bitwarden_json.py`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/main.py` & `bitwarden_import_msecure-1.7.1/src/bitwarden_import_msecure/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,29 +11,33 @@
 click.rich_click.USE_MARKDOWN = True
 
 
 OUTPUT_FILE_DEFAULT = "bitwarden"
 NOTES_MODE = "notes"
 
 
-def error(message: str, abort: bool = True) -> None:
+def error(message: str, show_patch_help: bool = True) -> None:
     """Print error message and exit."""
     console = Console()
     console.print(message, style="bold red")
-    if abort:
-        raise click.Abort()
+    if show_patch_help:
+        msecure_to_bitwarden.patch_help()
+    raise click.Abort()
 
 
 @click.command()
 @click.version_option(version=__version__, prog_name="bitwarden-import-msecure")
 @click.argument("input_file", type=click.Path(exists=True), required=False)
 @click.argument("output_file", type=click.Path(), required=False)
 @click.option("--force", is_flag=True, help="Overwrite the output file if it exists.")
 @click.option(
-    "--patch", is_flag=True, help="Fix old exports, see `--patch-help` for more details."
+    "--patch",
+    is_flag=True,
+    help="Patch Bitwarden export with data from mSecure export that previously was not imported. "
+    "See `--patch-help` for more details.",
 )
 @click.option("--patch-help", is_flag=True, help="Show help for `--patch` option.")
 @click.option(
     "--extra-fields",
     type=click.Choice(["custom-fields", NOTES_MODE]),
     default="custom-fields",
     help=(
@@ -82,21 +86,20 @@
         Path(output_file)
         if output_file
         else input_path.parent / f"{OUTPUT_FILE_DEFAULT}.{output_format}"
     )
 
     if patch:
         if output_format != "json":
-            error("Patching is only supported for JSON format.", abort=False)
-            msecure_to_bitwarden.patch_help()
-            raise click.Abort()
+            error("Patching is only supported for JSON format.", show_patch_help=True)
         if not output_path.exists():
-            error(f"To patch output file `{output_path}` it should exist.", abort=False)
-            msecure_to_bitwarden.patch_help()
-            raise click.Abort()
+            error(
+                f"Output file `{output_path}` does not exist. Cannot patch un-existed file.",
+                show_patch_help=True,
+            )
         msecure_to_bitwarden.patch(input_path, output_path)
     else:
         if output_path.exists() and not force:
             error(f"Output file `{output_path}` already exists. Use --force to overwrite.")
 
         msecure_to_bitwarden.convert(
             input_path,
```

### Comparing `bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/msecure.py` & `bitwarden_import_msecure-1.7.1/src/bitwarden_import_msecure/msecure.py`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/msecure_to_bitwarden.py` & `bitwarden_import_msecure-1.7.1/src/bitwarden_import_msecure/msecure_to_bitwarden.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,77 +1,79 @@
 """Conversion logic."""
 
 import csv
 import json
 from pathlib import Path
+from typing import Dict
 
 from rich.console import Console
 from rich.panel import Panel
 from rich.markdown import Markdown
 from rich.theme import Theme
 
 import rich_click as click
 
 from bitwarden_import_msecure.bitwarden_csv import BitwardenCsv
 from bitwarden_import_msecure.bitwarden_json import BitwardenJson
 from bitwarden_import_msecure.msecure import import_msecure_row
 
 
 def patch(input_path: Path, output_path: Path) -> None:
-    """Fix errors in old exports.
+    """Patch Bitwarden export with data from mSecure export that previously was not imported
 
     Some old versions of `bitwarden-import-msecure` worked incorrectly.
     For example versions before 1.5.0 did not export logins' URLs.
 
     If you migrated to Bitwarden some time ago and cannot just drop all records
     and import them again, use option `--patch`:
 
-    - process the mSecure export `mSecure Export File.csv` with the new `bitwarden-import-msecure`:
-        `bitwarden-import-msecure "mSecure Export File.csv" bitwarden.json`
-    - export json from Bitwarden, let's name the result as `bitwarden_new.json`
-    - patch this export with additional data from the mSecure export:
-        `bitwarden-import-msecure bitwarden.json bitwarden_new.json --patch`
-    - now you have `bitwarden_new.json` with all necessary changes, import it to Bitwarden
+    - export json from Bitwarden, let's name the result as `bitwarden_new.json`.
+    please backup this file in case something goes wrong
+    - patch this export with data from the mSecure export
+        `bitwarden-import-msecure "mSecure Export File.csv" bitwarden_new.json --patch`
+    - now you have `bitwarden_new.json` with additional data
+    - unfortunately Bitwarden does not respect item IDs on import, so to avoid duplicates
+    remove all items from Bitwarden, preferably using web interface.
+    It is save as you have full backup in `bitwarden_new.json`
+    - import bitwarden_new.json to Bitwarden as Bitwarden json file
+    - clean up mSecure export file, `bitwarden_new.json` and it's backup
     """
     if not output_path.exists():
         click.echo(f"Output file `{output_path}` does not exist.")
         raise click.Abort()
 
     try:
-        print(f"Reading input file: {input_path}..")
-        with input_path.open("r") as file:
-            input_data = json.load(file)
-    except json.JSONDecodeError as e:
-        print(f"Error: {input_path} is not a valid JSON file:\n{e}")
-        return
-    except FileNotFoundError as e:
-        print(f"Error: {input_path} not found:\n{e}")
-        return
-
-    try:
         print(f"Reading output file: {output_path}..")
         with output_path.open("r+") as file:
             output_data = json.load(file)
 
-            uri_dict = {}
-            for item in input_data.get("items", []):
-                if item.get("type") == 1:
-                    uris = item.get("login", {}).get("uris", [])
-                    if uris:
-                        if item["name"] in uri_dict:
-                            print(f"Name collision: {item['name']}, skipping..")
-                        else:
-                            uri_dict[item["name"]] = uris
+            uri_dict: Dict[str, str] = {}
+            with input_path.open(newline="", encoding="utf-8") as infile:
+                reader = csv.reader(infile, delimiter=",")
+                for row in reader:
+                    if row and not row[0].startswith("mSecure"):
+                        data = import_msecure_row(row, False)
+                        if data["type"] == "login":
+                            uri = data["login_uri"]
+                            if uri:
+                                if data["name"] in uri_dict:
+                                    print(
+                                        f"Name collision: item `{data['name']}`, "
+                                        f"has different URLs: `{uri_dict[data['name']]}` "
+                                        f"and `{uri}`. Using first one."
+                                    )
+                                else:
+                                    uri_dict[data["name"]] = uri
 
             replaced = 0
             for item in output_data.get("items", []):
                 if item.get("type") == 1 and (
                     item["name"] in uri_dict and not item.get("login", {}).get("uris", [])
                 ):
-                    item["login"]["uris"] = uri_dict[item["name"]]
+                    item["login"]["uris"] = [{"match": None, "uri": uri_dict[item["name"]]}]
                     replaced += 1
             click.echo(f"Added {replaced} URLs.")
 
             file.seek(0)
             json.dump(output_data, file, indent=4)
             file.truncate()
```

### Comparing `bitwarden_import_msecure-1.7.0/tests/conftest.py` & `bitwarden_import_msecure-1.7.1/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     with patch("bitwarden_import_msecure.bitwarden_json.now_string",
                return_value=fixed_now):
         yield
 
 
 @pytest.fixture
 def runner(freeze):
-    return CliRunner()
+    return CliRunner(echo_stdin=True)
 
 
 @pytest.fixture
 def msecure_export():
     with open(RESOURCES / "mSecure Export File.csv") as f:
         yield f.read()
```

### Comparing `bitwarden_import_msecure-1.7.0/tests/test_bitwarden_import_msecure.py` & `bitwarden_import_msecure-1.7.1/tests/test_bitwarden_import_msecure.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     result = runner.invoke(bitwarden_import_msecure, [
         str(dummy_input),
         str(non_existent_output),
         '--patch'
     ])
 
     assert result.exit_code == 1
-    assert f"To patch output file `{non_existent_output}` it should exist." in result.output.replace("\n", "")
+    assert f"Output file `{non_existent_output}` does not exist." in result.output.replace("\n", "")
 
 
 def test_patch_with_incorrect_format(runner, tmp_path):
     dummy_input = tmp_path / "dummy_input.csv"
     dummy_input.touch()  # Create an empty file
 
     incorrect_format_output = tmp_path / "output.csv"
```

### Comparing `bitwarden_import_msecure-1.7.0/tests/test_e2e.py` & `bitwarden_import_msecure-1.7.1/tests/test_e2e.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,17 +104,17 @@
     output_file = tmpdir.join("bitwarden.csv")
 
     if UPDATE_EXPECTED_OUTPUT:
         bitwarden_notes_csv_file.write_text(output_file.read_text(encoding="utf8"))
     assert_files_context_is_equal(output_file, bitwarden_notes_csv_file)
 
 
-def test_bitwarden_patch(runner, tmpdir, msecure_export, bitwarden_file, bitwarden_broken_file, bitwarden_patched_file):
+def test_bitwarden_patch(runner, tmpdir, msecure_export, bitwarden_broken_file, bitwarden_patched_file):
     input_file = tmpdir.join("input.txt")
-    input_file.write(bitwarden_file.read_text(encoding="utf8"))
+    input_file.write(msecure_export)
 
     output_file = tmpdir.join("output.txt")
     output_file.write(bitwarden_broken_file.read_text(encoding="utf8"))
 
     result = runner.invoke(bitwarden_import_msecure, [str(input_file), str(output_file), "--patch"])
     assert result.exit_code == 0
```

### Comparing `bitwarden_import_msecure-1.7.0/tests/resources/bitwarden_broken_export.json` & `bitwarden_import_msecure-1.7.1/tests/resources/bitwarden_broken_export.json`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/tests/resources/bitwarden_export.csv` & `bitwarden_import_msecure-1.7.1/tests/resources/bitwarden_export.csv`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/tests/resources/bitwarden_export.json` & `bitwarden_import_msecure-1.7.1/tests/resources/bitwarden_export.json`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/tests/resources/bitwarden_notes_export.csv` & `bitwarden_import_msecure-1.7.1/tests/resources/bitwarden_notes_export.csv`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/tests/resources/bitwarden_notes_export.json` & `bitwarden_import_msecure-1.7.1/tests/resources/bitwarden_notes_export.json`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/tests/resources/bitwarden_patched_export.json` & `bitwarden_import_msecure-1.7.1/tests/resources/bitwarden_patched_export.json`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/tests/resources/mSecure Export File.csv` & `bitwarden_import_msecure-1.7.1/tests/resources/mSecure Export File.csv`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/LICENSE.txt` & `bitwarden_import_msecure-1.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/README.md` & `bitwarden_import_msecure-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/pyproject.toml` & `bitwarden_import_msecure-1.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.7.0/PKG-INFO` & `bitwarden_import_msecure-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bitwarden-import-msecure
-Version: 1.7.0
+Version: 1.7.1
 Summary: Migration from mSecure to Bitwarden
 Project-URL: Homepage, https://andgineer.github.io/bitwarden-import-msecure/
 Project-URL: Documentation, https://andgineer.github.io/bitwarden-import-msecure/
 Author-email: Andrey Sorokin <andrey@sorokin.engineer>
 License: Copyright (c) 2024 Andrey Sorokin <andrey@sorokin.engineer>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_ydx0oxft_/tmp8taijo9c_TarContainer/0/49", line 74, column 102: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: bitwarden-import-msecure Version: 1.7.0 Summary:
+Metadata-Version: 2.3 Name: bitwarden-import-msecure Version: 1.7.1 Summary:
 Migration from mSecure to Bitwarden Project-URL: Homepage, https://
 andgineer.github.io/bitwarden-import-msecure/ Project-URL: Documentation,
 https://andgineer.github.io/bitwarden-import-msecure/ Author-email: Andrey
 Sorokin
 sorokin.engineer> License: Copyright (c) 2024 Andrey Sorokin
 sorokin.engineer> Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

