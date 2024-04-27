# Comparing `tmp/avro_py-2024.4.27.tar.gz` & `tmp/avro.py-2024.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avro_py-2024.4.27.tar", last modified: Sat Apr 27 05:51:22 2024, max compression
+gzip compressed data, was "avro.py-2024.4.7.tar", last modified: Sun Apr  7 06:59:50 2024, max compression
```

## Comparing `avro_py-2024.4.27.tar` & `avro.py-2024.4.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 05:51:22.742331 avro_py-2024.4.27/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-27 05:51:18.000000 avro_py-2024.4.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-27 05:51:18.000000 avro_py-2024.4.27/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-04-27 05:51:22.742331 avro_py-2024.4.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-04-27 05:51:18.000000 avro_py-2024.4.27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 05:51:22.742331 avro_py-2024.4.27/avro/
--rwxr-xr-x   0 runner    (1001) docker     (127)      275 2024-04-27 05:51:18.000000 avro_py-2024.4.27/avro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-27 05:51:18.000000 avro_py-2024.4.27/avro/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      799 2024-04-27 05:51:18.000000 avro_py-2024.4.27/avro/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12937 2024-04-27 05:51:18.000000 avro_py-2024.4.27/avro/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 05:51:22.742331 avro_py-2024.4.27/avro/resources/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-27 05:51:18.000000 avro_py-2024.4.27/avro/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39017 2024-04-27 05:51:18.000000 avro_py-2024.4.27/avro/resources/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 05:51:22.742331 avro_py-2024.4.27/avro/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-27 05:51:18.000000 avro_py-2024.4.27/avro/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      576 2024-04-27 05:51:18.000000 avro_py-2024.4.27/avro/utils/count.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2389 2024-04-27 05:51:18.000000 avro_py-2024.4.27/avro/utils/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 05:51:22.742331 avro_py-2024.4.27/avro.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-04-27 05:51:22.000000 avro_py-2024.4.27/avro.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-27 05:51:22.000000 avro_py-2024.4.27/avro.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 05:51:22.000000 avro_py-2024.4.27/avro.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-27 05:51:22.000000 avro_py-2024.4.27/avro.py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-27 05:51:22.000000 avro_py-2024.4.27/avro.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-27 05:51:22.000000 avro_py-2024.4.27/avro.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-27 05:51:18.000000 avro_py-2024.4.27/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 05:51:22.742331 avro_py-2024.4.27/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1820 2024-04-27 05:51:18.000000 avro_py-2024.4.27/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 05:51:22.742331 avro_py-2024.4.27/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5589 2024-04-27 05:51:18.000000 avro_py-2024.4.27/tests/test_main.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1051 2024-04-27 05:51:18.000000 avro_py-2024.4.27/tests/test_utils_count.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3923 2024-04-27 05:51:18.000000 avro_py-2024.4.27/tests/test_utils_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:59:50.337261 avro.py-2024.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-07 06:59:46.000000 avro.py-2024.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-07 06:59:46.000000 avro.py-2024.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-07 06:59:50.337261 avro.py-2024.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-04-07 06:59:46.000000 avro.py-2024.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:59:50.337261 avro.py-2024.4.7/avro/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      274 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      799 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12937 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:59:50.337261 avro.py-2024.4.7/avro/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39017 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/resources/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:59:50.337261 avro.py-2024.4.7/avro/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      576 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/utils/count.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2389 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/utils/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:59:50.337261 avro.py-2024.4.7/avro.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-07 06:59:50.000000 avro.py-2024.4.7/avro.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-07 06:59:50.000000 avro.py-2024.4.7/avro.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 06:59:50.000000 avro.py-2024.4.7/avro.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-07 06:59:50.000000 avro.py-2024.4.7/avro.py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-07 06:59:50.000000 avro.py-2024.4.7/avro.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-07 06:59:50.000000 avro.py-2024.4.7/avro.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-07 06:59:46.000000 avro.py-2024.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 06:59:50.337261 avro.py-2024.4.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1804 2024-04-07 06:59:46.000000 avro.py-2024.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:59:50.337261 avro.py-2024.4.7/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5589 2024-04-07 06:59:46.000000 avro.py-2024.4.7/tests/test_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1051 2024-04-07 06:59:46.000000 avro.py-2024.4.7/tests/test_utils_count.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3923 2024-04-07 06:59:46.000000 avro.py-2024.4.7/tests/test_utils_validate.py
```

### Comparing `avro_py-2024.4.27/LICENSE` & `avro.py-2024.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `avro_py-2024.4.27/PKG-INFO` & `avro.py-2024.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avro.py
-Version: 2024.4.27
+Version: 2024.4.7
 Summary: A modern Pythonic implementation of Avro Phonetic.
 Home-page: https://github.com/hitblast/avro.py
 Author: HitBlast
 Author-email: hitblastlive@gmail.com
 License: MIT
 Keywords: python,phonetics,avro,avro phonetic,bangla,bengali,bengali phonetics,transliteration
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,14 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: cli
 Requires-Dist: click>=8.0.0; extra == "cli"
 Requires-Dist: pyclip>=0.7.0; extra == "cli"
-Requires-Dist: rich>=13.0.0; extra == "cli"
 
 
 <!-- SPDX-License-Identifier: MIT -->
 
 <div align="center">
 
 # <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/python/python.png" height="40px"/> avro.py
```

### Comparing `avro_py-2024.4.27/README.md` & `avro.py-2024.4.7/README.md`

 * *Files identical despite different names*

### Comparing `avro_py-2024.4.27/avro/cli.py` & `avro.py-2024.4.7/avro/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 
 import avro
 
 # Try to import the required modules.
 try:
     import click
     import pyclip
-    from rich.console import Console
-
 except ImportError:
     print('In order to enable CLI, please install avro.py using: pip install avro.py[cli]')
     exit()
 
 
 # Create a new group for putting the CLI commands.
 @click.group(help=avro.__description__)
@@ -23,53 +21,39 @@
     package_name='avro.py',
     message='Package: %(prog)s, version %(version)s\nCore: version {0}'.format(avro.__version__),
 )
 def cli() -> None:
     pass
 
 
-# Initialize Console object for rich-based output.
-console = Console()
-
-
-# Helper functions for CLI commands.
-def _print_err(text: str) -> None:
-    console.print(text, style='red')
-    return click.echo(err=True)
-
-
 # Helper function for CLI actions.
 def _cli_action(
     text: str,
     *,
     bijoy: bool = False,
     from_clipboard: bool = False,
     copy_on_success: bool = False,
     reverse: bool = False,
 ) -> Optional[str]:
     if not text:
         if not from_clipboard:
-            return _print_err('No text provided.')
+            return click.echo('No text provided.')
         else:
             if not (text := pyclip.paste(text=True).strip()):
-                return _print_err('No text found in the clipboard.')
+                return click.echo('No text found in the clipboard.')
 
     if reverse:
-        output = avro.reverse(text)
+        text = avro.reverse(text)
     else:
-        output = avro.parse(text) if not bijoy else avro.parse(text, bijoy=True)
-
-    if output == text:
-        return _print_err('No changes in output.')
-
-    console.print(f'\n[bold green]Output[/bold green]\n {text}\n')
+        text = avro.parse(text) if not bijoy else avro.parse(text, bijoy=True)
 
     if copy_on_success:
         pyclip.copy(text)
-        console.print('[bold yellow](copied to clipboard)[/bold yellow]\n')
+
+    click.echo(text)
 
 
 # usage: avro parse <text> [--bijoy] [--from-clip] [--copy]
 @cli.command('parse', help='Parse a given text to Bangla / Bengali.')
 @click.argument('text', required=False)
 @click.option('--bijoy', is_flag=True, help='Use Bijoy Keyboard format for parsing.')
 @click.option('--from-clip', is_flag=True, help='Parse text from clipboard.')
```

### Comparing `avro_py-2024.4.27/avro/config.py` & `avro.py-2024.4.7/avro/config.py`

 * *Files identical despite different names*

### Comparing `avro_py-2024.4.27/avro/main.py` & `avro.py-2024.4.7/avro/main.py`

 * *Files identical despite different names*

### Comparing `avro_py-2024.4.27/avro/resources/dictionary.py` & `avro.py-2024.4.7/avro/resources/dictionary.py`

 * *Files identical despite different names*

### Comparing `avro_py-2024.4.27/avro/utils/count.py` & `avro.py-2024.4.7/avro/utils/count.py`

 * *Files identical despite different names*

### Comparing `avro_py-2024.4.27/avro/utils/validate.py` & `avro.py-2024.4.7/avro/utils/validate.py`

 * *Files identical despite different names*

### Comparing `avro_py-2024.4.27/avro.py.egg-info/PKG-INFO` & `avro.py-2024.4.7/avro.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avro.py
-Version: 2024.4.27
+Version: 2024.4.7
 Summary: A modern Pythonic implementation of Avro Phonetic.
 Home-page: https://github.com/hitblast/avro.py
 Author: HitBlast
 Author-email: hitblastlive@gmail.com
 License: MIT
 Keywords: python,phonetics,avro,avro phonetic,bangla,bengali,bengali phonetics,transliteration
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,14 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: cli
 Requires-Dist: click>=8.0.0; extra == "cli"
 Requires-Dist: pyclip>=0.7.0; extra == "cli"
-Requires-Dist: rich>=13.0.0; extra == "cli"
 
 
 <!-- SPDX-License-Identifier: MIT -->
 
 <div align="center">
 
 # <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/python/python.png" height="40px"/> avro.py
```

### Comparing `avro_py-2024.4.27/setup.py` & `avro.py-2024.4.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     extras_require={
-        'cli': ['click>=8.0.0', 'pyclip >= 0.7.0', 'rich>=13.0.0'],
+        'cli': ['click>=8.0.0', 'pyclip >= 0.7.0'],
     },
     entry_points={
         'console_scripts': [
             'avro=avro.cli:main',
         ],
     },
 )
```

### Comparing `avro_py-2024.4.27/tests/test_main.py` & `avro.py-2024.4.7/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `avro_py-2024.4.27/tests/test_utils_count.py` & `avro.py-2024.4.7/tests/test_utils_count.py`

 * *Files identical despite different names*

### Comparing `avro_py-2024.4.27/tests/test_utils_validate.py` & `avro.py-2024.4.7/tests/test_utils_validate.py`

 * *Files identical despite different names*

