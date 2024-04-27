# Comparing `tmp/cookieplone-0.4.1.tar.gz` & `tmp/cookieplone-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookieplone-0.4.1.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `cookieplone-0.4.1.tar` & `cookieplone-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,43 @@
--rw-r--r--   0        0        0     1142 2024-04-19 01:23:35.441045 cookieplone-0.4.1/README.md
--rw-r--r--   0        0        0       22 2024-04-19 18:08:42.551908 cookieplone-0.4.1/cookieplone/__init__.py
--rw-r--r--   0        0        0      191 2024-04-16 22:18:14.202809 cookieplone-0.4.1/cookieplone/__main__.py
--rw-r--r--   0        0        0     5548 2024-04-19 16:42:39.978057 cookieplone-0.4.1/cookieplone/cli.py
--rw-r--r--   0        0        0     1203 2024-04-17 19:41:55.848797 cookieplone-0.4.1/cookieplone/data.py
--rw-r--r--   0        0        0      452 2024-04-18 19:29:44.648761 cookieplone-0.4.1/cookieplone/exceptions.py
--rw-r--r--   0        0        0     2401 2024-04-18 17:59:28.841529 cookieplone-0.4.1/cookieplone/filters/__init__.py
--rw-r--r--   0        0        0     4122 2024-04-19 18:08:06.052237 cookieplone-0.4.1/cookieplone/generator.py
--rw-r--r--   0        0        0     1347 2024-04-18 23:57:11.861636 cookieplone-0.4.1/cookieplone/repository.py
--rw-r--r--   0        0        0      394 2024-04-18 19:18:47.072810 cookieplone-0.4.1/cookieplone/settings.py
--rw-r--r--   0        0        0       60 2024-04-17 16:17:54.105869 cookieplone-0.4.1/cookieplone/utils/__init__.py
--rw-r--r--   0        0        0     2696 2024-04-18 17:54:31.026810 cookieplone-0.4.1/cookieplone/utils/commands/__init__.py
--rw-r--r--   0        0        0     3710 2024-04-19 00:07:35.659983 cookieplone-0.4.1/cookieplone/utils/console.py
--rw-r--r--   0        0        0      243 2024-04-18 17:23:34.273811 cookieplone-0.4.1/cookieplone/utils/containers.py
--rw-r--r--   0        0        0      486 2024-04-18 22:26:25.935421 cookieplone-0.4.1/cookieplone/utils/files.py
--rw-r--r--   0        0        0      887 2024-04-16 23:39:28.137531 cookieplone-0.4.1/cookieplone/utils/sanity.py
--rw-r--r--   0        0        0     4516 2024-04-18 22:47:44.003042 cookieplone-0.4.1/cookieplone/utils/validators.py
--rw-r--r--   0        0        0     2780 2024-04-18 17:23:34.273620 cookieplone-0.4.1/cookieplone/utils/versions.py
--rw-r--r--   0        0        0     2196 2024-04-19 01:26:29.201409 cookieplone-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2128 1970-01-01 00:00:00.000000 cookieplone-0.4.1/setup.py
--rw-r--r--   0        0        0     2568 1970-01-01 00:00:00.000000 cookieplone-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 cookieplone-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 cookieplone-0.5.0/CHANGES.md
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 cookieplone-0.5.0/Makefile
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cookieplone-0.5.0/tox.ini
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cookieplone-0.5.0/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.5.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cookieplone-0.5.0/cookieplone/__init__.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cookieplone-0.5.0/cookieplone/__main__.py
+-rw-r--r--   0        0        0     5387 2020-02-02 00:00:00.000000 cookieplone-0.5.0/cookieplone/cli.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 cookieplone-0.5.0/cookieplone/data.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 cookieplone-0.5.0/cookieplone/exceptions.py
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 cookieplone-0.5.0/cookieplone/generator.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cookieplone-0.5.0/cookieplone/repository.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 cookieplone-0.5.0/cookieplone/settings.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 cookieplone-0.5.0/cookieplone/filters/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 cookieplone-0.5.0/cookieplone/utils/__init__.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 cookieplone-0.5.0/cookieplone/utils/console.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 cookieplone-0.5.0/cookieplone/utils/containers.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 cookieplone-0.5.0/cookieplone/utils/files.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 cookieplone-0.5.0/cookieplone/utils/git.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 cookieplone-0.5.0/cookieplone/utils/internal.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 cookieplone-0.5.0/cookieplone/utils/sanity.py
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 cookieplone-0.5.0/cookieplone/utils/validators.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 cookieplone-0.5.0/cookieplone/utils/versions.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 cookieplone-0.5.0/cookieplone/utils/commands/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 cookieplone-0.5.0/news/.changelog_template.jinja
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookieplone-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 cookieplone-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 cookieplone-0.5.0/tests/test_filters.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 cookieplone-0.5.0/tests/utils/test_commands.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 cookieplone-0.5.0/tests/utils/test_console.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 cookieplone-0.5.0/tests/utils/test_containers.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 cookieplone-0.5.0/tests/utils/test_files.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 cookieplone-0.5.0/tests/utils/test_git.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 cookieplone-0.5.0/tests/utils/test_internal.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 cookieplone-0.5.0/tests/utils/test_sanity.py
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 cookieplone-0.5.0/tests/utils/test_validators.py
+-rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 cookieplone-0.5.0/tests/utils/test_versions.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cookieplone-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 cookieplone-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5749 2020-02-02 00:00:00.000000 cookieplone-0.5.0/README.md
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 cookieplone-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7111 2020-02-02 00:00:00.000000 cookieplone-0.5.0/PKG-INFO
```

### Comparing `cookieplone-0.4.1/cookieplone/cli.py` & `cookieplone-0.5.0/cookieplone/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
+# SPDX-FileCopyrightText: 2024-present Plone Foundation <board@plone.org>
+#
+# SPDX-License-Identifier: MIT
 """Main `cookieplone` CLI."""
 
 import os
-import sys
 from pathlib import Path
 from typing import Annotated
 
 import typer
-from cookiecutter import __version__ as __cookiecutter_version__
 from cookiecutter.log import configure_logger
 from rich import print
 from rich.prompt import Prompt
 
-from cookieplone import __version__, data
+from cookieplone import data, settings
 from cookieplone.exceptions import GeneratorException
 from cookieplone.generator import generate
 from cookieplone.repository import get_base_repository, get_template_options
-from cookieplone.utils import console
+from cookieplone.utils import console, internal
 
 
 def validate_extra_context(value: list[str] | None = None):
     """Validate extra content follows the correct pattern."""
     if not value:
         return {}
     for string in value:
@@ -38,25 +39,14 @@
     templates = get_template_options(base_path)
     choices = {i[0]: i[1] for i in templates}
     console.welcome_screen(templates)
     answer = Prompt.ask("Select a template", choices=list(choices.keys()), default="1")
     return choices[answer]
 
 
-def version_info() -> str:
-    """Return the Cookieplone version, location and Python powering it."""
-    python_version = sys.version
-    location = Path(__file__).parent
-    return (
-        f"Cookieplone {__version__} from {location} "
-        f"(Cookiecutter {__cookiecutter_version__}, "
-        f"Python {python_version})"
-    )
-
-
 def cli(
     template: Annotated[str, typer.Argument(help="Template to be used.")] = "",
     extra_context: Annotated[
         data.OptionalListStr,
         typer.Argument(callback=validate_extra_context, help="Extra context."),
     ] = None,
     output_dir: Annotated[
@@ -116,36 +106,38 @@
             "--debug-file", help="File to be used as a stream for DEBUG logging"
         ),
     ] = None,
     verbose: Annotated[bool, typer.Option("--verbose", "-v")] = False,
 ):
     """Generate a new Plone codebase."""
     if version:
-        info = version_info
-        print(info)
+        print(internal.version_info)
         raise typer.Exit()
-    repository = os.environ.get("COOKIEPLONE_REPOSITORY")
+    repository = os.environ.get(settings.REPO_LOCATION)
     if not repository:
         repository = "gh:plone/cookiecutter-plone"
 
+    repo_path = get_base_repository(repository)
     if not template:
         # Display template options
-        repo_path = get_base_repository(repository)
-        template = prompt_for_template(Path(repo_path))
+        template = prompt_for_template(repo_path)
     else:
         console.welcome_screen()
 
     if replay_file:
         replay = replay_file
     passwd = os.environ.get(
-        "COOKIECUTTER_REPO_PASSWORD", os.environ.get("COOKIEPLONE_REPO_PASSWORD")
+        settings.REPO_PASSWORD, os.environ.get("COOKIECUTTER_REPO_PASSWORD")
     )
     if not output_dir:
         output_dir = Path().cwd()
     configure_logger(stream_level="DEBUG" if verbose else "INFO", debug_file=debug_file)
+    # Annotate extra_context
+    extra_context = extra_context if extra_context else {}
+    extra_context["__generator_signature"] = internal.signature_md(repo_path)
     # Run generator
     try:
         generate(
             repository,
             tag,
             no_input,
             extra_context,
```

### Comparing `cookieplone-0.4.1/cookieplone/data.py` & `cookieplone-0.5.0/cookieplone/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# SPDX-FileCopyrightText: 2024-present Plone Foundation <board@plone.org>
+#
+# SPDX-License-Identifier: MIT
 from collections.abc import Callable
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Literal, Optional, TypeAlias
 
 OptionalPath: TypeAlias = Optional[Path]  # noQA:UP007
 OptionalListStr: TypeAlias = Optional[list[str]]  # noQA:UP007
```

### Comparing `cookieplone-0.4.1/cookieplone/filters/__init__.py` & `cookieplone-0.5.0/cookieplone/filters/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# SPDX-FileCopyrightText: 2024-present Plone Foundation <board@plone.org>
+#
+# SPDX-License-Identifier: MIT
 import os
 
 from cookiecutter.utils import simple_filter
 
 from cookieplone.utils import containers, versions
```

### Comparing `cookieplone-0.4.1/cookieplone/generator.py` & `cookieplone-0.5.0/cookieplone/generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# SPDX-FileCopyrightText: 2024-present Plone Foundation <board@plone.org>
+#
+# SPDX-License-Identifier: MIT
 import json
 from collections import OrderedDict
 from pathlib import Path
 
 from cookiecutter import exceptions as exc
 from cookiecutter.main import cookiecutter
```

### Comparing `cookieplone-0.4.1/cookieplone/repository.py` & `cookieplone-0.5.0/cookieplone/repository.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# SPDX-FileCopyrightText: 2024-present Plone Foundation <board@plone.org>
+#
+# SPDX-License-Identifier: MIT
 import json
 from pathlib import Path
 
 from cookiecutter.config import get_user_config
 from cookiecutter.repository import determine_repo_dir
 
 from cookieplone import data
@@ -9,28 +12,29 @@
 
 def get_base_repository(
     repository: str,
     tag: str | None = None,
     password: str = "",
     config_file: data.OptionalPath = None,
     default_config: bool = False,
-):
+) -> Path:
     config_dict = get_user_config(
         config_file=config_file,
         default_config=default_config,
     )
     base_repo_dir, _ = determine_repo_dir(
         template=repository,
         abbreviations=config_dict["abbreviations"],
         clone_to_dir=config_dict["cookiecutters_dir"],
         checkout=tag,
         no_input=True,  # Force download
         password=password,
         directory="",
     )
+    base_repo_dir = Path(base_repo_dir).resolve()
     return base_repo_dir
 
 
 def get_template_options(base_path: Path) -> list[list[str]]:
     """Parse cookiecutter.json and return a list of template options."""
     config = json.loads((base_path / "cookiecutter.json").read_text())
     available_templates = config.get("templates", {})
```

### Comparing `cookieplone-0.4.1/cookieplone/utils/commands/__init__.py` & `cookieplone-0.5.0/cookieplone/utils/commands/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# SPDX-FileCopyrightText: 2024-present Plone Foundation <board@plone.org>
+#
+# SPDX-License-Identifier: MIT
 import re
 import subprocess
 import sys
 
 from cookieplone import settings
 
 
@@ -70,16 +73,16 @@
     raw_version = _get_command_version("docker")
     if not raw_version:
         return "Docker not found."
     else:
         version = _parse_docker_version(raw_version)
         return (
             ""
-            if version >= settings.MIN_DOCKER_VERSION
-            else f"Docker version is not supported: Got {raw_version}"
+            if version >= min_version
+            else f"Docker version is not supported: Got {version}"
         )
 
 
 def check_command_is_available(command: str) -> str:
     """Check if a command line utility is available."""
     raw_version = _get_command_version(command)
     return "" if raw_version else f"Command {command} is not available."
```

### Comparing `cookieplone-0.4.1/cookieplone/utils/console.py` & `cookieplone-0.5.0/cookieplone/utils/console.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,16 @@
+# SPDX-FileCopyrightText: 2024-present Plone Foundation <board@plone.org>
+#
+# SPDX-License-Identifier: MIT
 import os
 from textwrap import dedent
 
 from rich import print as base_print
+from rich.align import Align
+from rich.console import Group
 from rich.markup import escape
 from rich.panel import Panel
 from rich.table import Table
 
 from cookieplone.settings import QUIET_MODE_VAR
 
 BANNER = """
@@ -114,18 +119,24 @@
     for idx, _, title, description in rows:
         table.add_row(idx, title, description)
 
     return table
 
 
 def welcome_screen(templates: list[list[str]] | None = None):
-    print_plone_banner()
+    items = [
+        Align.center(f"[bold blue]{BANNER}[/bold blue]"),
+    ]
     if templates:
-        table = table_available_templates("Templates", templates)
-        _print(table)
+        items.append(Panel(table_available_templates("Templates", templates)))
+    panel = Panel(
+        Group(*items),
+        title="cookieplone",
+    )
+    base_print(panel)
 
 
 def enable_quiet_mode():
     """Enable quiet mode."""
     os.environ[QUIET_MODE_VAR] = "1"
```

### Comparing `cookieplone-0.4.1/cookieplone/utils/sanity.py` & `cookieplone-0.5.0/cookieplone/utils/sanity.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,29 @@
+# SPDX-FileCopyrightText: 2024-present Plone Foundation <board@plone.org>
+#
+# SPDX-License-Identifier: MIT
 from cookieplone import data
 
 
 def run_sanity_checks(checks: list[data.SanityCheck]) -> data.SanityCheckResults:
     """Run sanity checks."""
     global_status = True
     results = []
     for check in checks:
+        status = False
         name = check.name
         func = check.func
         args = check.args
         level = check.level
         message = func(*args)
         if not message:
             status = True
             message = "✓"
         elif level == "warning":
             status = True
-        elif level == "error":
-            status = False
         global_status = global_status and status
         results.append(data.SanityCheckResult(name, status, message))
     global_message = (
         f"Ran {len(checks)} checks and they {'passed' if global_status else 'failed'}."
     )
     return data.SanityCheckResults(
         status=global_status, message=global_message, checks=results
```

### Comparing `cookieplone-0.4.1/cookieplone/utils/validators.py` & `cookieplone-0.5.0/cookieplone/utils/validators.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# SPDX-FileCopyrightText: 2024-present Plone Foundation <board@plone.org>
+#
+# SPDX-License-Identifier: MIT
 import re
 from typing import Any
 from urllib.parse import urlparse
 
 from packaging.version import InvalidVersion, Version
 
 from cookieplone import data, settings
@@ -77,27 +80,27 @@
     """Validate the npm package name is valid."""
     pattern = r"^(@[a-z0-9-~][a-z0-9-._~]*\/)?[a-z0-9-~][a-z0-9-._~]*$"
     return "" if re.match(pattern, value) else f"'{value}' is not a valid package name."
 
 
 def validate_plone_version(value: str) -> str:
     """Validate Plone Version."""
-    status = False
     version = _version_from_str(value)
-    if version:
-        status = version >= _version_from_str(settings.PLONE_MIN_VERSION)
+    status = bool(version) and (
+        version >= _version_from_str(settings.PLONE_MIN_VERSION)
+    )
     return "" if status else f"{value} is not a valid Plone version."
 
 
 def validate_volto_version(value: str) -> str:
     """Validate Volto Version."""
-    status = False
     version = _version_from_str(value)
-    if version:
-        status = version >= _version_from_str(settings.VOLTO_MIN_VERSION)
+    status = bool(version) and (
+        version >= _version_from_str(settings.VOLTO_MIN_VERSION)
+    )
     return "" if status else f"{value} is not a valid Volto version."
 
 
 def run_context_validations(
     context: dict, validations: list[data.ItemValidator], allow_empty: bool = False
 ) -> data.ContextValidatorResult:
     """Run validations for context."""
@@ -107,26 +110,25 @@
         func = validate_not_empty
         for key in context:
             if key.startswith("_"):
                 # Ignore computed values
                 continue
             validations.append(data.ItemValidator(key, func, "error"))
     for validation in validations:
+        status = False
         key = validation.key
         func = validation.func
         value = context.get(key, "")
         level = validation.level
         message = func(value, key) if func == validate_not_empty else func(value)
         if not message:
             status = True
             message = "✓"
         elif level == "warning":
             status = True
-        elif level == "error":
-            status = False
         global_status = global_status and status
         results.append(data.ItemValidatorResult(key, status, message))
     global_message = (
         f"Ran {len(results)} validations and "
         f"they {'passed' if global_status else 'failed'}."
     )
     return data.ContextValidatorResult(
```

### Comparing `cookieplone-0.4.1/cookieplone/utils/versions.py` & `cookieplone-0.5.0/cookieplone/utils/versions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# SPDX-FileCopyrightText: 2024-present Plone Foundation <board@plone.org>
+#
+# SPDX-License-Identifier: MIT
 import requests
 from packaging.version import Version
 
 from cookieplone import settings
 
 
 def get_npm_package_versions(package: str) -> list[str]:
```

