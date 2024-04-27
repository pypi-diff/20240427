# Comparing `tmp/cmdict-0.1.7.tar.gz` & `tmp/cmdict-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdict-0.1.7.tar", max compression
+gzip compressed data, was "cmdict-0.1.9.tar", max compression
```

## Comparing `cmdict-0.1.7.tar` & `cmdict-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2023-06-25 09:02:28.422962 cmdict-0.1.7/LICENSE
--rw-r--r--   0        0        0     2717 2023-06-25 09:02:28.422962 cmdict-0.1.7/README.md
--rw-r--r--   0        0        0     1298 2023-06-25 09:02:28.422962 cmdict-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       93 2023-06-25 09:02:28.422962 cmdict-0.1.7/src/cmdict/__init__.py
--rw-r--r--   0        0        0      112 2023-06-25 09:02:28.422962 cmdict-0.1.7/src/cmdict/__main__.py
--rw-r--r--   0        0        0     2558 2023-06-25 09:02:28.422962 cmdict-0.1.7/src/cmdict/ecdict_connector.py
--rw-r--r--   0        0        0     1423 2023-06-25 09:02:28.422962 cmdict-0.1.7/src/cmdict/history.py
--rw-r--r--   0        0        0     4685 2023-06-25 09:02:28.422962 cmdict-0.1.7/src/cmdict/pdf_tools.py
--rw-r--r--   0        0        0     6901 2023-06-25 09:02:28.422962 cmdict-0.1.7/src/cmdict/run_script.py
--rw-r--r--   0        0        0      463 2023-06-25 09:02:28.422962 cmdict-0.1.7/src/cmdict/txt_tools.py
--rw-r--r--   0        0        0      384 2023-06-25 09:02:28.422962 cmdict-0.1.7/src/cmdict/utils.py
--rw-r--r--   0        0        0     3623 1970-01-01 00:00:00.000000 cmdict-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-01-31 20:01:50.838208 cmdict-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3208 2024-01-31 20:01:50.838208 cmdict-0.1.9/README.md
+-rw-r--r--   0        0        0     1329 2024-01-31 20:01:50.838208 cmdict-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       93 2024-01-31 20:01:50.838208 cmdict-0.1.9/src/cmdict/__init__.py
+-rw-r--r--   0        0        0      112 2024-01-31 20:01:50.838208 cmdict-0.1.9/src/cmdict/__main__.py
+-rw-r--r--   0        0        0     2558 2024-01-31 20:01:50.838208 cmdict-0.1.9/src/cmdict/ecdict_connector.py
+-rw-r--r--   0        0        0     1423 2024-01-31 20:01:50.838208 cmdict-0.1.9/src/cmdict/history.py
+-rw-r--r--   0        0        0     4699 2024-01-31 20:01:50.838208 cmdict-0.1.9/src/cmdict/pdf_tools.py
+-rw-r--r--   0        0        0     6931 2024-01-31 20:01:50.838208 cmdict-0.1.9/src/cmdict/run_script.py
+-rw-r--r--   0        0        0      463 2024-01-31 20:01:50.838208 cmdict-0.1.9/src/cmdict/txt_tools.py
+-rw-r--r--   0        0        0      384 2024-01-31 20:01:50.838208 cmdict-0.1.9/src/cmdict/utils.py
+-rw-r--r--   0        0        0     4158 1970-01-01 00:00:00.000000 cmdict-0.1.9/PKG-INFO
```

### Comparing `cmdict-0.1.7/LICENSE` & `cmdict-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cmdict-0.1.7/README.md` & `cmdict-0.1.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # cmdict &middot; [![pypi](https://badge.fury.io/py/cmdict.svg)](https://pypi.org/project/cmdict/) [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/zequnyu/cmdict/blob/master/LICENSE) [![CI](https://github.com/pasty-dev/cmdict/actions/workflows/ci.yml/badge.svg)](https://github.com/pasty-dev/cmdict/actions/workflows/ci.yml) [![codecov](https://codecov.io/gh/zequnyu/cmdict/branch/master/graph/badge.svg)](https://codecov.io/gh/zequnyu/cmdict) [![poetry](https://img.shields.io/badge/PyPM-poetry-5975aa)](https://python-poetry.org) [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-`cmdict` is a command-line dictionary toolset.
+`cmdict` not only is an English-to-Chinese dictionary application with a command-line interface, but also provide out-of-box features like extracting highlighted words from a PDF file. It runs on Linux, macOS, and Windows. Additionally, it can be used as a Python package.
 
-## Installation
+## How to install
 
-Use [`homebrew`](https://brew.sh/):
+The easiest way is to use [Homebrew](https://brew.sh/):
 
 ```sh
-brew install pasty-dev/cmdict/cmdict
+brew install pastydev/cmdict/cmdict
 ```
 
-or [`pip`](https://pypi.org/project/cmdict/):
+To install it from [PyPI](https://pypi.org/project/cmdict/):
 
 ```sh
 pip install cmdict
 ```
 
-## How to Use
+## How to use
 
 ```console
 $ cmdict --help
 Usage: cmdict [OPTIONS] COMMAND [ARGS]...
 
   Command line interface.
 
@@ -74,19 +74,23 @@
         - [医] 苹果
     collins: 3
     oxford: 1
     bnc: 2446
     frq: 2695
 ```
 
-## Support
+## Data support
 
 - [`skywind3000/ECDICT`](https://github.com/skywind3000/ECDICT/releases): a free English to Chinese dictionary database (英中双解词典数据库).
 
 ```console
 $ cmdict download
 --------
 Downloading the dictionary...
 100%|████████████████████████| 217M/217M [00:29<00:00, 666MiB/s]
 
 cmdict is ready to use!
 ```
+
+## How to contribute
+
+[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?hide_repo_select=true&ref=master&repo=266903250&machine=largePremiumLinux&location=WestEurope)
```

### Comparing `cmdict-0.1.7/pyproject.toml` & `cmdict-0.1.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 [tool.poetry]
 name = "cmdict"
-version = "0.1.7"
+version = "0.1.9"
 description = "A command line dictionary toolset."
 authors = ["zequnyu <zequnyu11@gmail.com>", "edxu96 <edxu96@outlook.com>"]
 license = "GPL-3.0"
 exclude = ["src/cmdict/data/*"]
 readme = "README.md"
 repository = "https://github.com/pastydev/cmdict"
 
 [tool.poetry.scripts]
 cmdict = 'cmdict:run_script.cli'
 cmdicts = 'cmdict:run_script.search'
 
 [tool.poetry.dependencies]
-python = ">=3.7.0"
+python = ">=3.7.0,<4.0"
 loguru = ">=0.5.1"
 click = ">=7.1.2"
 colorama = ">=0.4.3"
 requests = ">=2.24.0"
 tqdm = ">=4.48.0"
 pyyaml = ">=5.3.1"
+trogon = "~0.5.0"
 
 [tool.poetry.group.pdf]
 optional = true
 
 [tool.poetry.group.pdf.dependencies]
-PyMuPDF = "1.22.3"
+PyMuPDF = "1.22.5"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0.0"
-pytest-cov = "^2.9.0"
-pytest-xdist = "^1.32.0"
+pytest-cov = ">=2.9,<5.0"
+pytest-xdist = ">=1.32,<4.0"
 
 [tool.poetry.group.check]
 optional = true
 
 [tool.poetry.group.check.dependencies]
 pre-commit = "2.21.0"
```

### Comparing `cmdict-0.1.7/src/cmdict/ecdict_connector.py` & `cmdict-0.1.9/src/cmdict/ecdict_connector.py`

 * *Files identical despite different names*

### Comparing `cmdict-0.1.7/src/cmdict/history.py` & `cmdict-0.1.9/src/cmdict/history.py`

 * *Files identical despite different names*

### Comparing `cmdict-0.1.7/src/cmdict/pdf_tools.py` & `cmdict-0.1.9/src/cmdict/pdf_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from cmdict.utils import remove_punctuation
 
 PDF_FEATURES: bool
 """If the features for PDF are enabled."""
 try:
     # ``import fitz`` still works, if the directory where it comes from
     # is empty, so the following command must be used.
-    from fitz import open
+    from fitz import open  # noqa: A004
 except (ImportError, ModuleNotFoundError):
     PDF_FEATURES = False
 else:
     PDF_FEATURES = True
 
 PREVIEW_COLORS = {
     "yellow": [250, 205, 90],
```

### Comparing `cmdict-0.1.7/src/cmdict/run_script.py` & `cmdict-0.1.9/src/cmdict/run_script.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import zipfile
 
 import click
 from colorama import Fore, Style
 from colorama import init as _init_colorama
 import requests
 from tqdm import tqdm
+from trogon import tui
 import yaml
 
 from cmdict.ecdict_connector import ECDICTConnector
 from cmdict.pdf_tools import extract_words, PDF_FEATURES
 from cmdict.txt_tools import scan_words
 
 DB_URL = "https://github.com/skywind3000/ECDICT/releases/download/1.0.28/ecdict-sqlite-28.zip"  # noqa: E501
@@ -44,14 +45,15 @@
         """
         if active:
             return super(ActiveFlagCommand, self).command(*args, **kwargs)
         else:
             return lambda f: f
 
 
+@tui()
 @click.group(cls=ActiveFlagCommand)
 def cli():
     """Command line interface."""
 
 
 @cli.command()
 def download():
```

### Comparing `cmdict-0.1.7/PKG-INFO` & `cmdict-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 Metadata-Version: 2.1
 Name: cmdict
-Version: 0.1.7
+Version: 0.1.9
 Summary: A command line dictionary toolset.
 Home-page: https://github.com/pastydev/cmdict
 License: GPL-3.0
 Author: zequnyu
 Author-email: zequnyu11@gmail.com
-Requires-Python: >=3.7.0
+Requires-Python: >=3.7.0,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=7.1.2)
 Requires-Dist: colorama (>=0.4.3)
 Requires-Dist: loguru (>=0.5.1)
 Requires-Dist: pyyaml (>=5.3.1)
 Requires-Dist: requests (>=2.24.0)
 Requires-Dist: tqdm (>=4.48.0)
+Requires-Dist: trogon (>=0.5.0,<0.6.0)
 Project-URL: Repository, https://github.com/pastydev/cmdict
 Description-Content-Type: text/markdown
 
 # cmdict &middot; [![pypi](https://badge.fury.io/py/cmdict.svg)](https://pypi.org/project/cmdict/) [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/zequnyu/cmdict/blob/master/LICENSE) [![CI](https://github.com/pasty-dev/cmdict/actions/workflows/ci.yml/badge.svg)](https://github.com/pasty-dev/cmdict/actions/workflows/ci.yml) [![codecov](https://codecov.io/gh/zequnyu/cmdict/branch/master/graph/badge.svg)](https://codecov.io/gh/zequnyu/cmdict) [![poetry](https://img.shields.io/badge/PyPM-poetry-5975aa)](https://python-poetry.org) [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-`cmdict` is a command-line dictionary toolset.
+`cmdict` not only is an English-to-Chinese dictionary application with a command-line interface, but also provide out-of-box features like extracting highlighted words from a PDF file. It runs on Linux, macOS, and Windows. Additionally, it can be used as a Python package.
 
-## Installation
+## How to install
 
-Use [`homebrew`](https://brew.sh/):
+The easiest way is to use [Homebrew](https://brew.sh/):
 
 ```sh
-brew install pasty-dev/cmdict/cmdict
+brew install pastydev/cmdict/cmdict
 ```
 
-or [`pip`](https://pypi.org/project/cmdict/):
+To install it from [PyPI](https://pypi.org/project/cmdict/):
 
 ```sh
 pip install cmdict
 ```
 
-## How to Use
+## How to use
 
 ```console
 $ cmdict --help
 Usage: cmdict [OPTIONS] COMMAND [ARGS]...
 
   Command line interface.
 
@@ -99,20 +100,24 @@
         - [医] 苹果
     collins: 3
     oxford: 1
     bnc: 2446
     frq: 2695
 ```
 
-## Support
+## Data support
 
 - [`skywind3000/ECDICT`](https://github.com/skywind3000/ECDICT/releases): a free English to Chinese dictionary database (英中双解词典数据库).
 
 ```console
 $ cmdict download
 --------
 Downloading the dictionary...
 100%|████████████████████████| 217M/217M [00:29<00:00, 666MiB/s]
 
 cmdict is ready to use!
 ```
 
+## How to contribute
+
+[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?hide_repo_select=true&ref=master&repo=266903250&machine=largePremiumLinux&location=WestEurope)
+
```

