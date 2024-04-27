# Comparing `tmp/pylic-3.5.0.tar.gz` & `tmp/pylic-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylic-3.5.0.tar", max compression
+gzip compressed data, was "pylic-3.6.0.tar", max compression
```

## Comparing `pylic-3.5.0.tar` & `pylic-3.6.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1069 2023-01-22 22:16:02.674940 pylic-3.5.0/LICENSE
--rw-r--r--   0        0        0     4491 2023-01-22 22:16:02.674940 pylic-3.5.0/README.md
--rw-r--r--   0        0        0       39 2023-01-22 22:16:02.674940 pylic-3.5.0/pylic/__main__.py
--rw-r--r--   0        0        0       18 2023-01-22 22:16:02.674940 pylic-3.5.0/pylic/__version__.py
--rw-r--r--   0        0        0      625 2023-01-22 22:16:02.674940 pylic-3.5.0/pylic/cli/app.py
--rw-r--r--   0        0        0     6777 2023-01-22 22:16:02.674940 pylic-3.5.0/pylic/cli/commands/check.py
--rw-r--r--   0        0        0      347 2023-01-22 22:16:02.674940 pylic-3.5.0/pylic/cli/commands/command.py
--rw-r--r--   0        0        0     1400 2023-01-22 22:16:02.674940 pylic-3.5.0/pylic/cli/commands/help.py
--rw-r--r--   0        0        0     1527 2023-01-22 22:16:02.674940 pylic-3.5.0/pylic/cli/commands/list.py
--rw-r--r--   0        0        0      454 2023-01-22 22:16:02.674940 pylic-3.5.0/pylic/cli/commands/version.py
--rw-r--r--   0        0        0     2645 2023-01-22 22:16:02.674940 pylic-3.5.0/pylic/cli/console_reader.py
--rw-r--r--   0        0        0     1303 2023-01-22 22:16:02.674940 pylic-3.5.0/pylic/cli/console_writer.py
--rw-r--r--   0        0        0     4006 2023-01-22 22:16:02.674940 pylic-3.5.0/pylic/license_checker.py
--rw-r--r--   0        0        0     1551 2023-01-22 22:16:02.674940 pylic-3.5.0/pylic/licenses.py
--rw-r--r--   0        0        0     1292 2023-01-22 22:16:02.674940 pylic-3.5.0/pylic/toml.py
--rw-r--r--   0        0        0     2383 2023-01-22 22:16:02.674940 pylic-3.5.0/pyproject.toml
--rw-r--r--   0        0        0     5438 1970-01-01 00:00:00.000000 pylic-3.5.0/setup.py
--rw-r--r--   0        0        0     5331 1970-01-01 00:00:00.000000 pylic-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-27 12:13:48.198938 pylic-3.6.0/LICENSE
+-rw-r--r--   0        0        0     4843 2024-04-27 12:13:48.198938 pylic-3.6.0/README.md
+-rw-r--r--   0        0        0       39 2024-04-27 12:13:48.198938 pylic-3.6.0/pylic/__main__.py
+-rw-r--r--   0        0        0       18 2024-04-27 12:13:48.198938 pylic-3.6.0/pylic/__version__.py
+-rw-r--r--   0        0        0      552 2024-04-27 12:13:48.198938 pylic-3.6.0/pylic/cli/app.py
+-rw-r--r--   0        0        0     6663 2024-04-27 12:13:48.198938 pylic-3.6.0/pylic/cli/commands/check.py
+-rw-r--r--   0        0        0      347 2024-04-27 12:13:48.198938 pylic-3.6.0/pylic/cli/commands/command.py
+-rw-r--r--   0        0        0     1400 2024-04-27 12:13:48.202938 pylic-3.6.0/pylic/cli/commands/help.py
+-rw-r--r--   0        0        0     1527 2024-04-27 12:13:48.202938 pylic-3.6.0/pylic/cli/commands/list.py
+-rw-r--r--   0        0        0      454 2024-04-27 12:13:48.202938 pylic-3.6.0/pylic/cli/commands/version.py
+-rw-r--r--   0        0        0     2624 2024-04-27 12:13:48.202938 pylic-3.6.0/pylic/cli/console_reader.py
+-rw-r--r--   0        0        0     1303 2024-04-27 12:13:48.202938 pylic-3.6.0/pylic/cli/console_writer.py
+-rw-r--r--   0        0        0     3975 2024-04-27 12:13:48.202938 pylic-3.6.0/pylic/license_checker.py
+-rw-r--r--   0        0        0     1488 2024-04-27 12:13:48.202938 pylic-3.6.0/pylic/licenses.py
+-rw-r--r--   0        0        0     1256 2024-04-27 12:13:48.202938 pylic-3.6.0/pylic/toml.py
+-rw-r--r--   0        0        0     2780 2024-04-27 12:13:48.202938 pylic-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5688 1970-01-01 00:00:00.000000 pylic-3.6.0/PKG-INFO
```

### Comparing `pylic-3.5.0/LICENSE` & `pylic-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylic-3.5.0/README.md` & `pylic-3.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # pylic - Python license checker [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/sandrochuber/pylic/blob/main/LICENSE) [![PyPI version](https://badge.fury.io/py/pylic.svg)](https://badge.fury.io/py/pylic/) [![Codecov](https://codecov.io/gh/ubersan/pylic//branch/main/graph/badge.svg)](https://codecov.io/gh/ubersan/pylic/)
 
 Reads pylic configuration in `pyproject.toml` and checks licenses of installed packages recursively.
 
 Principles:
+
 - Every license has to be allowed explicitly (case-insensitive comparison).
 - All installed packages without a license are considered unsafe and have to be listed as such.
 
 > Only installed packages are checked for licenses. Packages/dependencies listed in `pyproject.toml` are ignored.
 
 ## Installation
 
 ```sh
 pip install pylic
 ```
 
 ## Configuration
 
 `pylic` needs be run in the directory where your `pyproject.toml` file is located. You can configure
+
 - `safe_licenses`: All licenses you consider safe for usage. The string comparison is case-insensitive.
 - `unsafe_packages`: If you rely on a package that does not come with a license you have to explicitly list it as such.
 - `ignore_packages`: Packages that will not be reported as unsafe even if they use a license not listed as safe. This is useful in case an existing projects want to start integrating `pylic`, but are still using unsafe licenses. This enables first to ignore these packages temporarely, while they're being replaced, second to already validate newly added or updated packages against the safe license set and third to integrate `pylic` frictionless into CI/CD from the get go.
 
 ```toml
 [tool.pylic]
 safe_licenses = [
@@ -37,14 +39,15 @@
     "ignoredPackage",
 ]
 ```
 
 ## Commands
 
 `pylic` provides the following commands (also see `pylic help`):
+
 - `check`: Checks all installed licenses.
 - `list`: Lists all installed packages and their corresponding license.
 
 ## Usage Example
 
 Create a venv to start with a clean ground and activate it
 
@@ -117,17 +120,32 @@
 
 Use `pylic list` to list all installed packages and their corresponding licenses.
 
 ## Advanced Usage
 
 In cases where the safe licenses or unsafe packages are centrally managed keeping the configuration in perfect sync to the installed packages might be too cumbersome or even impossible. To support these use cases the `check` command provides the two options (see also `check --help`) `--allow-extra-safe-licenses` and `--allow-extra-unused-packages`. These options only affect the returned status code and will keep all corresponding printed warnings unchanged.
 
+## Pre-commit
+
+`pylic` provides a [pre-commit](https://pre-commit.com/) integration. Follow the [instructions](https://pre-commit.com/#quick-start) and enable automatic license checking on commits by adding
+
+```sh
+-  repo: https://github.com/ubersan/pylic
+   rev: v<version>
+   hooks:
+   -  id: pylic
+```
+
+to your `.pre-commit-config.yaml` file.
+
 ## Development
 
 Required tools:
+
 - Poetry (https://python-poetry.org/)
 
 Run `poetry install` to install all necessary dependencies. Checkout the `[tool.taskipy.tasks]` (see [taskipy](https://github.com/illBeRoy/taskipy)) section in the `pyproject.toml` file for utility tasks. You can run these with `poetry run task <task>`.
 
 Creating a new release is as simple as:
+
 - Update `version` in the pyproject.toml and the `__version__.py` file.
 - `poetry run task release`.
```

### Comparing `pylic-3.5.0/pylic/cli/app.py` & `pylic-3.6.0/pylic/cli/app.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,22 +6,15 @@
 from pylic.cli.commands.version import VersionCommand
 from pylic.cli.console_reader import ConsoleReader
 
 
 def main() -> None:
     sys.argv.pop(0)
 
-    program = ConsoleReader(
-        commands=[
-            CheckCommand(),
-            ListCommand(),
-            HelpCommand(),
-            VersionCommand(),
-        ]
-    ).get_program(sys.argv)
+    program = ConsoleReader(commands=[CheckCommand(), ListCommand(), HelpCommand(), VersionCommand()]).get_program(sys.argv)
 
     status_code = program.command.handle(program.options)
     exit(status_code)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pylic-3.5.0/pylic/cli/commands/check.py` & `pylic-3.6.0/pylic/cli/commands/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 
 class CheckCommand(Command):
     targets_to_token = TargetsToToken(targets=["check"], token="check")
     option_targets_to_token = [
         TargetsToToken(targets=["--allow-extra-unused-packages", "-p"], token="allow_extra_packages"),
         TargetsToToken(targets=["--allow-extra-safe-licenses", "-l"], token="allow_extra_licenses"),
+        TargetsToToken(targets=["--quiet", "-q"], token="quiet"),
         TargetsToToken(targets=["--help", "-h"], token="help"),
     ]
 
     def handle(self, options: List[str]) -> int:
         if "help" in options:
             self._show_help()
             return 1
@@ -56,38 +57,32 @@
                 for unnecessary_ignore_package in unnecessary_ignore_packages:
                     console_writer.line(f"  {WARNING}{unnecessary_ignore_package}{END_STYLE}")
 
             if len(bad_unsafe_packages) > 0:
                 console_writer.line("Found unsafe packages with a known license. Instead allow these licenses explicitly:")
                 for bad_package in bad_unsafe_packages:
                     console_writer.line(
-                        (
-                            f"  {WARNING}{bad_package['package']}{END_STYLE} {LABEL}({bad_package['version']}{END_STYLE}): "
-                            f"{BLUE}{bad_package['license']}{END_STYLE}"
-                        )
+                        f"  {WARNING}{bad_package['package']}{END_STYLE} {LABEL}({bad_package['version']}{END_STYLE}): "
+                        f"{BLUE}{bad_package['license']}{END_STYLE}"
                     )
 
             if len(missing_unsafe_packages) > 0:
                 console_writer.line("Found unsafe packages:")
                 for missing_unsafe_package in missing_unsafe_packages:
                     console_writer.line(
-                        (
-                            f"  {WARNING}{missing_unsafe_package['package']}{END_STYLE} "
-                            f"{LABEL}({missing_unsafe_package['version']}){END_STYLE}"
-                        )
+                        f"  {WARNING}{missing_unsafe_package['package']}{END_STYLE} "
+                        f"{LABEL}({missing_unsafe_package['version']}){END_STYLE}"
                     )
 
             if len(unsafe_licenses.found) > 0:
                 console_writer.line("Found unsafe licenses:")
                 for bad_license in unsafe_licenses.found:
                     console_writer.line(
-                        (
-                            f"  {BLUE}{bad_license['package']}{END_STYLE} {LABEL}({bad_license['version']}){END_STYLE}: "
-                            f"{WARNING}{bad_license['license']}{END_STYLE}"
-                        )
+                        f"  {BLUE}{bad_license['package']}{END_STYLE} {LABEL}({bad_license['version']}){END_STYLE}: "
+                        f"{WARNING}{bad_license['license']}{END_STYLE}"
                     )
 
             if not all([unnecessary_ignore_packages, bad_unsafe_packages, missing_unsafe_packages, unsafe_licenses.found]):
                 extra_packages_declared_and_allowed = len(unnecessary_unsafe_packages) > 0 and "allow_extra_packages" in options
                 extra_licenses_declared_and_allowed = len(unnecessary_safe_licenses) > 0 and "allow_extra_licenses" in options
                 if (
                     (not unnecessary_safe_licenses and extra_packages_declared_and_allowed)
@@ -99,21 +94,21 @@
 
             return 1
 
         if len(unsafe_licenses.ignored) > 0:
             console_writer.line("Ignored packages with unsafe licenses:")
             for bad_license in unsafe_licenses.ignored:
                 console_writer.line(
-                    (
-                        f"  {BLUE}{bad_license['package']}{END_STYLE} {LABEL}({bad_license['version']}){END_STYLE}: "
-                        f"{WARNING}{bad_license['license']}{END_STYLE}"
-                    )
+                    f"  {BLUE}{bad_license['package']}{END_STYLE} {LABEL}({bad_license['version']}){END_STYLE}: "
+                    f"{WARNING}{bad_license['license']}{END_STYLE}"
                 )
 
-        console_writer.write_all_licenses_ok()
+        if 'quiet' not in options:
+            console_writer.write_all_licenses_ok()
+            
         return 0
 
     def _show_help(self) -> None:
         console_writer.line(f"{BOLD}USAGE{END_STYLE}")
         console_writer.line(f"  {UNDERLINE}pylic{END_STYLE} {UNDERLINE}check{END_STYLE} [-h] [-l] [-p]\n")
         console_writer.line(f"{BOLD}OPTIONS{END_STYLE}")
         console_writer.line(f"  {LABEL}-h{END_STYLE} (--help)\t\t\t\tDisplay this help message")
```

### Comparing `pylic-3.5.0/pylic/cli/commands/help.py` & `pylic-3.6.0/pylic/cli/commands/help.py`

 * *Files identical despite different names*

### Comparing `pylic-3.5.0/pylic/cli/commands/list.py` & `pylic-3.6.0/pylic/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `pylic-3.5.0/pylic/cli/console_reader.py` & `pylic-3.6.0/pylic/cli/console_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,16 +43,15 @@
             )
             exit(1)
         tokens.append(command.targets_to_token.token)
 
         if len(sanitized_inputs) > 0 and command.option_targets_to_token is not None:
             for option_target in sanitized_inputs[1:]:
                 option_targets_to_token = next(
-                    filter(lambda targets_to_token: option_target in targets_to_token.targets, command.option_targets_to_token),
-                    None,
+                    filter(lambda targets_to_token: option_target in targets_to_token.targets, command.option_targets_to_token), None
                 )
                 if option_targets_to_token is None:
                     console_writer.write_no_such_option_for_command(option_target, command.targets_to_token.token)
                     exit(1)
                 tokens.append(option_targets_to_token.token)
 
         return tokens
```

### Comparing `pylic-3.5.0/pylic/cli/console_writer.py` & `pylic-3.6.0/pylic/cli/console_writer.py`

 * *Files identical despite different names*

### Comparing `pylic-3.5.0/pylic/license_checker.py` & `pylic-3.6.0/pylic/license_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,19 +7,15 @@
 @dataclass
 class UnsafeLicenses:
     found: List[Dict]
     ignored: List[Dict]
 
 
 class LicenseChecker:
-    def __init__(
-        self,
-        config: Optional[AppConfig] = None,
-        installed_licenses: Optional[List[Dict]] = None,
-    ) -> None:
+    def __init__(self, config: Optional[AppConfig] = None, installed_licenses: Optional[List[Dict]] = None) -> None:
         self.config = config or AppConfig()
         self.installed_licenses = installed_licenses or []
 
     def get_unnecessary_safe_licenses(self) -> List[str]:
         installed_license_names = [license_info["license"].lower() for license_info in self.installed_licenses]
 
         unnecessary_safe_licenses = []
```

### Comparing `pylic-3.5.0/pylic/licenses.py` & `pylic-3.6.0/pylic/licenses.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,15 @@
         license_string = _read_license_from_classifier(distribution)
         if license_string == "unknown":
             license_string = _read_license_from_metadata(distribution)
         if license_string == "OSI Approved":
             license_string = _read_license_from_metadata(distribution, fallback="OSI Approved")
 
         installed_licenses.append(
-            {
-                "license": license_string,
-                "package": distribution.metadata["Name"],
-                "version": distribution.metadata["Version"],
-            }
+            {"license": license_string, "package": distribution.metadata["Name"], "version": distribution.metadata["Version"]}
         )
 
     return installed_licenses
 
 
 def _read_license_from_classifier(distribution: Distribution) -> str:
     for key, content in distribution.metadata.items():  # type:ignore
```

### Comparing `pylic-3.5.0/pylic/toml.py` & `pylic-3.6.0/pylic/toml.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,20 +18,16 @@
 
     if "unknown" in [safe_license.lower() for safe_license in safe_licenses]:
         raise ValueError("'unknown' can't be an safe license. Whitelist the corresponding packages instead.")
 
     unsafe_packages: List[str] = pylic_config.get("unsafe_packages", [])
     ignore_packages: List[str] = pylic_config.get("ignore_packages", [])
 
-    return AppConfig(
-        safe_licenses=safe_licenses,
-        unsafe_packages=unsafe_packages,
-        ignore_packages=ignore_packages,
-    )
+    return AppConfig(safe_licenses=safe_licenses, unsafe_packages=unsafe_packages, ignore_packages=ignore_packages)
 
 
 def _read_pyproject_file(filename: str) -> MutableMapping[str, Any]:
-    with open(filename, "r") as pyproject_file:
+    with open(filename) as pyproject_file:
         try:
             return toml.load(pyproject_file)
         except Exception as exception:
             raise exception
```

### Comparing `pylic-3.5.0/pyproject.toml` & `pylic-3.6.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -4,61 +4,66 @@
 description = "A Python license checker"
 homepage = "https://github.com/ubersan/pylic"
 keywords = ["cli", "license", "checker"]
 license = "MIT License"
 name = "pylic"
 readme = "README.md"
 repository = "https://github.com/ubersan/pylic"
-version = "3.5.0"
+version = "3.6.0"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.7.2"
 importlib-metadata = "^6.0.0"
 toml = "^0.10.2"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.10.0"
-flake8 = "^3.9.2"
-isort = "^5.10.1"
 mypy = "^0.991"
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 taskipy = "^1.10.3"
 types-toml = "^0.10.8.1"
+ruff = "^0.4.2"
+pytest-only = "^2.1.1"
 
 [tool.poetry.scripts]
 pylic = 'pylic.cli.app:main'
 
 [tool.taskipy.tasks]
-check_licenses = "python -m pylic check"
-get_current_version = "echo -n v$(sed '11q;d' pyproject.toml | awk '{print $3}' | tail -c +2 | head -c -2)"
-quality = "black . && flake8 --max-line-length 140 --count . && isort . && mypy ."
-release = " git tag $(task get_current_version) && git push origin $(task get_current_version)"
+check-format = "echo 'Checking formatting ...' && ruff fomrat --diff --quiet ."
+fix-format = "echo 'Fixing formatting ...' && ruff format ."
+check-lint = "echo 'Checking linting ...' && ruff check --quiet ."
+fix-lint = "echo 'Fixing linting ...' && ruff check --fix ."
+check-types = "echo 'Checking types ...' && mypy --pretty --no-error-summary ."
+check-licenses = "echo 'Checking licenses ...' && python -m pylic check --quiet"
+check-all = "task check-format && task check-lint && task check-types && task check-licenses && echo ✅"
+fix-all = "task fix-format ; task fix-lint"
+get-current-version = "echo -n v$(sed '11q;d' pyproject.toml | awk '{print $3}' | tail -c +2 | head -c -2)"
+release = " git tag $(task get-current-version) && git push origin $(task get-current-version)"
 test = "pytest --cov=./ --cov-report=xml"
 
 [tool.pylic]
 safe_licenses = [
   "BSD License",
   "Apache Software License",
   "MIT License",
-  "Python Software Foundation License",
-  "Mozilla Public License 2.0 (MPL 2.0)",
+  "Python Software Foundation License"
 ]
 
-[tool.black]
-line_length = 140
+[tool.ruff]
+line-length = 140
 
-[tool.isort]
-ensure_newline_before_comments = "True"
-force_grid_wrap = 0
-include_trailing_comma = "True"
-line_length = 140
-multi_line_output = 3
-use_parentheses = "True"
+[tool.ruff.format]
+skip-magic-trailing-comma = true
+
+[tool.ruff.lint]
+select = ["E", "F", "UP", "B", "SIM", "I"]
+
+[tool.ruff.lint.isort]
+split-on-trailing-comma = false
 
 [tool.coverage.report]
 exclude_lines = [
   "if __name__ == .__main__.:",
   "from importlib_metadata import Distribution, distributions", # tested by integration tests
   "app.run()", # tested by integration tests
   "pragma: no cover",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pylic-3.5.0/setup.py` & `pylic-3.6.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,175 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pylic
+Version: 3.6.0
+Summary: A Python license checker
+Home-page: https://github.com/ubersan/pylic
+License: MIT
+Keywords: cli,license,checker
+Author: Sandro Huber
+Author-email: sandrochuber@gmail.com
+Requires-Python: >=3.7.2,<4.0.0
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: importlib-metadata (>=6.0.0,<7.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Project-URL: Repository, https://github.com/ubersan/pylic
+Description-Content-Type: text/markdown
 
-packages = \
-['pylic', 'pylic.cli', 'pylic.cli.commands']
+# pylic - Python license checker [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/sandrochuber/pylic/blob/main/LICENSE) [![PyPI version](https://badge.fury.io/py/pylic.svg)](https://badge.fury.io/py/pylic/) [![Codecov](https://codecov.io/gh/ubersan/pylic//branch/main/graph/badge.svg)](https://codecov.io/gh/ubersan/pylic/)
 
-package_data = \
-{'': ['*']}
+Reads pylic configuration in `pyproject.toml` and checks licenses of installed packages recursively.
 
-install_requires = \
-['importlib-metadata>=6.0.0,<7.0.0', 'toml>=0.10.2,<0.11.0']
-
-entry_points = \
-{'console_scripts': ['pylic = pylic.cli.app:main']}
-
-setup_kwargs = {
-    'name': 'pylic',
-    'version': '3.5.0',
-    'description': 'A Python license checker',
-    'long_description': '# pylic - Python license checker [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/sandrochuber/pylic/blob/main/LICENSE) [![PyPI version](https://badge.fury.io/py/pylic.svg)](https://badge.fury.io/py/pylic/) [![Codecov](https://codecov.io/gh/ubersan/pylic//branch/main/graph/badge.svg)](https://codecov.io/gh/ubersan/pylic/)\n\nReads pylic configuration in `pyproject.toml` and checks licenses of installed packages recursively.\n\nPrinciples:\n- Every license has to be allowed explicitly (case-insensitive comparison).\n- All installed packages without a license are considered unsafe and have to be listed as such.\n\n> Only installed packages are checked for licenses. Packages/dependencies listed in `pyproject.toml` are ignored.\n\n## Installation\n\n```sh\npip install pylic\n```\n\n## Configuration\n\n`pylic` needs be run in the directory where your `pyproject.toml` file is located. You can configure\n- `safe_licenses`: All licenses you consider safe for usage. The string comparison is case-insensitive.\n- `unsafe_packages`: If you rely on a package that does not come with a license you have to explicitly list it as such.\n- `ignore_packages`: Packages that will not be reported as unsafe even if they use a license not listed as safe. This is useful in case an existing projects want to start integrating `pylic`, but are still using unsafe licenses. This enables first to ignore these packages temporarely, while they\'re being replaced, second to already validate newly added or updated packages against the safe license set and third to integrate `pylic` frictionless into CI/CD from the get go.\n\n```toml\n[tool.pylic]\nsafe_licenses = [\n    "Apache Software License",\n    "Apache License 2.0",\n    "MIT License",\n    "Python Software Foundation License",\n    "Mozilla Public License 2.0 (MPL 2.0)",\n]\nunsafe_packages = [\n    "unlicensedPackage",\n]\nignore_packages = [\n    "ignoredPackage",\n]\n```\n\n## Commands\n\n`pylic` provides the following commands (also see `pylic help`):\n- `check`: Checks all installed licenses.\n- `list`: Lists all installed packages and their corresponding license.\n\n## Usage Example\n\nCreate a venv to start with a clean ground and activate it\n\n```sh\npython -m venv .venv\nsource .venv/bin/activate\n```\n\nInstall `pylic` and create an empty `pyproject.toml`\n\n```sh\npip install pylic\ntouch pyproject.toml\n```\n\nInstall all your dependencies\n\n```sh\npip install <packageA> <packageB>\n```\n\nRun pylic\n\n```sh\npylic check\n```\n\nThe output will be similar to\n\n```sh\nFound unsafe packages:\n  pkg_resources (0.0.0)\nFound unsafe licenses:\n  pip (18.1): MIT License\n  zipp (3.4.1): MIT License\n  toml (0.10.2): MIT License\n  pylic (1.2.0): MIT License\n  setuptools (40.8.0): MIT License\n  typing-extensions (3.7.4.3): Python Software Foundation License\n  importlib-metadata (3.9.0): Apache Software License\n```\n\nThe return code of `pylic` is in this case non-zero due to unsafe licenses. This allows usage of pylic in CI.\n\n```sh\necho $? # prints 1\n```\n\nAs these licenses and packages are all ok we can configure `pylic` accordingly\n\n```sh\ncat <<EOT >> pyproject.toml\n[tool.pylic]\nsafe_licenses = ["Apache Software License", "MIT License", "Python Software Foundation License"]\nunsafe_packages = ["pkg_resources"]\nEOT\n```\n\nAfter rerunning `pylic check` the output now reveals a successful validation\n\n```sh\n✨ All licenses ok ✨\n```\n\nAlso the return code now signals that all is good\n\n```sh\necho $? # prints 0\n```\n\nUse `pylic list` to list all installed packages and their corresponding licenses.\n\n## Advanced Usage\n\nIn cases where the safe licenses or unsafe packages are centrally managed keeping the configuration in perfect sync to the installed packages might be too cumbersome or even impossible. To support these use cases the `check` command provides the two options (see also `check --help`) `--allow-extra-safe-licenses` and `--allow-extra-unused-packages`. These options only affect the returned status code and will keep all corresponding printed warnings unchanged.\n\n## Development\n\nRequired tools:\n- Poetry (https://python-poetry.org/)\n\nRun `poetry install` to install all necessary dependencies. Checkout the `[tool.taskipy.tasks]` (see [taskipy](https://github.com/illBeRoy/taskipy)) section in the `pyproject.toml` file for utility tasks. You can run these with `poetry run task <task>`.\n\nCreating a new release is as simple as:\n- Update `version` in the pyproject.toml and the `__version__.py` file.\n- `poetry run task release`.\n',
-    'author': 'Sandro Huber',
-    'author_email': 'sandrochuber@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/ubersan/pylic',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+Principles:
 
+- Every license has to be allowed explicitly (case-insensitive comparison).
+- All installed packages without a license are considered unsafe and have to be listed as such.
+
+> Only installed packages are checked for licenses. Packages/dependencies listed in `pyproject.toml` are ignored.
+
+## Installation
+
+```sh
+pip install pylic
+```
+
+## Configuration
+
+`pylic` needs be run in the directory where your `pyproject.toml` file is located. You can configure
+
+- `safe_licenses`: All licenses you consider safe for usage. The string comparison is case-insensitive.
+- `unsafe_packages`: If you rely on a package that does not come with a license you have to explicitly list it as such.
+- `ignore_packages`: Packages that will not be reported as unsafe even if they use a license not listed as safe. This is useful in case an existing projects want to start integrating `pylic`, but are still using unsafe licenses. This enables first to ignore these packages temporarely, while they're being replaced, second to already validate newly added or updated packages against the safe license set and third to integrate `pylic` frictionless into CI/CD from the get go.
+
+```toml
+[tool.pylic]
+safe_licenses = [
+    "Apache Software License",
+    "Apache License 2.0",
+    "MIT License",
+    "Python Software Foundation License",
+    "Mozilla Public License 2.0 (MPL 2.0)",
+]
+unsafe_packages = [
+    "unlicensedPackage",
+]
+ignore_packages = [
+    "ignoredPackage",
+]
+```
+
+## Commands
+
+`pylic` provides the following commands (also see `pylic help`):
+
+- `check`: Checks all installed licenses.
+- `list`: Lists all installed packages and their corresponding license.
+
+## Usage Example
+
+Create a venv to start with a clean ground and activate it
+
+```sh
+python -m venv .venv
+source .venv/bin/activate
+```
+
+Install `pylic` and create an empty `pyproject.toml`
+
+```sh
+pip install pylic
+touch pyproject.toml
+```
+
+Install all your dependencies
+
+```sh
+pip install <packageA> <packageB>
+```
+
+Run pylic
+
+```sh
+pylic check
+```
+
+The output will be similar to
+
+```sh
+Found unsafe packages:
+  pkg_resources (0.0.0)
+Found unsafe licenses:
+  pip (18.1): MIT License
+  zipp (3.4.1): MIT License
+  toml (0.10.2): MIT License
+  pylic (1.2.0): MIT License
+  setuptools (40.8.0): MIT License
+  typing-extensions (3.7.4.3): Python Software Foundation License
+  importlib-metadata (3.9.0): Apache Software License
+```
+
+The return code of `pylic` is in this case non-zero due to unsafe licenses. This allows usage of pylic in CI.
+
+```sh
+echo $? # prints 1
+```
+
+As these licenses and packages are all ok we can configure `pylic` accordingly
+
+```sh
+cat <<EOT >> pyproject.toml
+[tool.pylic]
+safe_licenses = ["Apache Software License", "MIT License", "Python Software Foundation License"]
+unsafe_packages = ["pkg_resources"]
+EOT
+```
+
+After rerunning `pylic check` the output now reveals a successful validation
+
+```sh
+✨ All licenses ok ✨
+```
+
+Also the return code now signals that all is good
+
+```sh
+echo $? # prints 0
+```
+
+Use `pylic list` to list all installed packages and their corresponding licenses.
+
+## Advanced Usage
+
+In cases where the safe licenses or unsafe packages are centrally managed keeping the configuration in perfect sync to the installed packages might be too cumbersome or even impossible. To support these use cases the `check` command provides the two options (see also `check --help`) `--allow-extra-safe-licenses` and `--allow-extra-unused-packages`. These options only affect the returned status code and will keep all corresponding printed warnings unchanged.
+
+## Pre-commit
+
+`pylic` provides a [pre-commit](https://pre-commit.com/) integration. Follow the [instructions](https://pre-commit.com/#quick-start) and enable automatic license checking on commits by adding
+
+```sh
+-  repo: https://github.com/ubersan/pylic
+   rev: v<version>
+   hooks:
+   -  id: pylic
+```
+
+to your `.pre-commit-config.yaml` file.
+
+## Development
+
+Required tools:
+
+- Poetry (https://python-poetry.org/)
+
+Run `poetry install` to install all necessary dependencies. Checkout the `[tool.taskipy.tasks]` (see [taskipy](https://github.com/illBeRoy/taskipy)) section in the `pyproject.toml` file for utility tasks. You can run these with `poetry run task <task>`.
+
+Creating a new release is as simple as:
+
+- Update `version` in the pyproject.toml and the `__version__.py` file.
+- `poetry run task release`.
 
-setup(**setup_kwargs)
```

