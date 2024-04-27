# Comparing `tmp/signal_export-2.2.2.tar.gz` & `tmp/signal_export-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signal_export-2.2.2.tar", last modified: Wed Mar 27 09:17:46 2024, max compression
+gzip compressed data, was "signal_export-2.3.0.tar", last modified: Sat Apr 27 16:27:44 2024, max compression
```

## Comparing `signal_export-2.2.2.tar` & `signal_export-2.3.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1170 2024-03-27 09:17:37.523158 signal_export-2.2.2/LICENSE
--rw-r--r--   0        0        0     8271 2024-03-27 09:17:37.523158 signal_export-2.2.2/README.md
--rw-r--r--   0        0        0     2015 2024-03-27 09:17:45.995147 signal_export-2.2.2/pyproject.toml
--rw-r--r--   0        0        0       79 2024-03-27 09:17:37.523158 signal_export-2.2.2/sigexport/__init__.py
--rw-r--r--   0        0        0     3157 2024-03-27 09:17:37.523158 signal_export-2.2.2/sigexport/create.py
--rw-r--r--   0        0        0     2956 2024-03-27 09:17:37.523158 signal_export-2.2.2/sigexport/data.py
--rw-r--r--   0        0        0     3209 2024-03-27 09:17:37.523158 signal_export-2.2.2/sigexport/files.py
--rw-r--r--   0        0        0     3451 2024-03-27 09:17:37.523158 signal_export-2.2.2/sigexport/html.py
--rw-r--r--   0        0        0      144 2024-03-27 09:17:37.523158 signal_export-2.2.2/sigexport/logging.py
--rwxr-xr-x   0        0        0     8367 2024-03-27 09:17:37.523158 signal_export-2.2.2/sigexport/main.py
--rw-r--r--   0        0        0     2722 2024-03-27 09:17:37.523158 signal_export-2.2.2/sigexport/merge.py
--rw-r--r--   0        0        0     4310 2024-03-27 09:17:37.523158 signal_export-2.2.2/sigexport/models.py
--rw-r--r--   0        0        0     1846 2024-03-27 09:17:37.523158 signal_export-2.2.2/sigexport/style.css
--rw-r--r--   0        0        0     1271 2024-03-27 09:17:37.527158 signal_export-2.2.2/sigexport/templates.py
--rw-r--r--   0        0        0     2409 2024-03-27 09:17:37.527158 signal_export-2.2.2/sigexport/utils.py
--rw-r--r--   0        0        0     2546 2024-03-27 09:17:37.527158 signal_export-2.2.2/tests/data/attachments.noindex/image.jpeg
--rw-r--r--   0        0        0    17641 2024-03-27 09:17:37.527158 signal_export-2.2.2/tests/data/attachments.noindex/voicenote.m4a
--rw-r--r--   0        0        0       22 2024-03-27 09:17:37.527158 signal_export-2.2.2/tests/data/config.json
--rw-r--r--   0        0        0    16384 2024-03-27 09:17:37.527158 signal_export-2.2.2/tests/data/sql/db.sqlite
--rw-r--r--   0        0        0     5125 2024-03-27 09:17:37.527158 signal_export-2.2.2/tests/test_integration.py
--rw-r--r--   0        0        0       86 2024-03-27 09:17:37.527158 signal_export-2.2.2/tests/test_utils.py
--rw-r--r--   0        0        0     9205 1970-01-01 00:00:00.000000 signal_export-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1170 2024-04-27 16:27:41.496862 signal_export-2.3.0/LICENSE
+-rw-r--r--   0        0        0     6921 2024-04-27 16:27:41.496862 signal_export-2.3.0/README.md
+-rw-r--r--   0        0        0     2006 2024-04-27 16:27:44.832870 signal_export-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-04-27 16:27:41.496862 signal_export-2.3.0/sigexport/__init__.py
+-rw-r--r--   0        0        0       69 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/__main__.py
+-rw-r--r--   0        0        0     3157 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/create.py
+-rw-r--r--   0        0        0     2956 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/data.py
+-rw-r--r--   0        0        0     3209 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/files.py
+-rw-r--r--   0        0        0     3451 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/html.py
+-rw-r--r--   0        0        0      144 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/logging.py
+-rwxr-xr-x   0        0        0     8356 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/main.py
+-rw-r--r--   0        0        0     2722 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/merge.py
+-rw-r--r--   0        0        0     4310 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/models.py
+-rw-r--r--   0        0        0     1846 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/style.css
+-rw-r--r--   0        0        0     1271 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/templates.py
+-rw-r--r--   0        0        0     2467 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/utils.py
+-rw-r--r--   0        0        0     2546 2024-04-27 16:27:41.500862 signal_export-2.3.0/tests/data/attachments.noindex/image.jpeg
+-rw-r--r--   0        0        0    17641 2024-04-27 16:27:41.500862 signal_export-2.3.0/tests/data/attachments.noindex/voicenote.m4a
+-rw-r--r--   0        0        0       22 2024-04-27 16:27:41.500862 signal_export-2.3.0/tests/data/config.json
+-rw-r--r--   0        0        0    16384 2024-04-27 16:27:41.500862 signal_export-2.3.0/tests/data/sql/db.sqlite
+-rw-r--r--   0        0        0     5125 2024-04-27 16:27:41.500862 signal_export-2.3.0/tests/test_integration.py
+-rw-r--r--   0        0        0       86 2024-04-27 16:27:41.500862 signal_export-2.3.0/tests/test_utils.py
+-rw-r--r--   0        0        0     7846 1970-01-01 00:00:00.000000 signal_export-2.3.0/PKG-INFO
```

### Comparing `signal_export-2.2.2/LICENSE` & `signal_export-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `signal_export-2.2.2/README.md` & `signal_export-2.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: signal-export
+Version: 2.3.0
+Summary: Export Signal conversations to Markdown and HTML
+Keywords: backup,chat,export
+Home-page: https://github.com/carderne/signal-export
+Author-Email: Chris Arderne <chris@rdrn.me>
+License: MIT License
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python
+Project-URL: Homepage, https://github.com/carderne/signal-export
+Project-URL: Repository, https://github.com/carderne/signal-export
+Requires-Python: >=3.9
+Requires-Dist: beautifulsoup4~=4.11
+Requires-Dist: emoji~=2.0
+Requires-Dist: Markdown~=3.4
+Requires-Dist: typer[all]~=0.7
+Requires-Dist: pysqlcipher3==1.1.0; python_version < "3.11" and extra == "sql"
+Requires-Dist: pysqlcipher3>=1.2.0; python_version >= "3.11" and extra == "sql"
+Provides-Extra: sql
+Description-Content-Type: text/markdown
+
 # signal-export
 [![cicd](https://github.com/carderne/signal-export/actions/workflows/cicd.yml/badge.svg)](https://github.com/carderne/signal-export/actions/workflows/cicd.yml)
 [![PyPI version](https://badge.fury.io/py/signal-export.svg)](https://pypi.org/project/signal-export/)
 
 Export chats from the [Signal](https://www.signal.org/) [Desktop app](https://www.signal.org/download/) to Markdown and HTML files with attachments. Each chat is exported as an individual .md/.html file and the attachments for each are stored in a separate folder. Attachments are linked from the Markdown files and displayed in the HTML (pictures, videos, voice notes).
 
 Currently this seems to be the only way to get chat history out of Signal!
@@ -16,40 +40,96 @@
 [2019-05-29, 15:20] Jim: I'm not.
 ```
 
 Images are attached inline with `![name](path)` while other attachments (voice notes, videos, documents) are included as links like `[name](path)` so a click will take you to the file.
 
 This is converted to HTML at the end so it can be opened with any web browser. The stylesheet `.css` is still very basic but I'll get to it sooner or later.
 
-## 🚀 Installation with Docker
-This tool has some pretty difficult dependencies, so it's easier to get some help from Docker.
-For most people this will probably be the easiest way.
-It requires installing Docker and then pulling a [200MB image](https://hub.docker.com/r/carderne/sigexport), so avoid this if data use is a concern.
+## 🪟 Installation: Windows
+If you need step-by-step instructions on things like enabling WSL2, please see the dedicated [Windows Installation](./INSTALLATION.md) instructions.
 
-First off, [install Docker](https://docs.docker.com/get-docker/) (including following the [post-installation steps](https://docs.docker.com/engine/install/linux-postinstall/) for managing Docker as a non-root user).  
-And make sure you have Python installed.
+In order to use this tool, you'll need to install WSL2, Docker and Python.
+The steps to do this are below.
+(**NB:** Improvements to these instructions are welcome.)
+
+1. Enable Windows WSL2 feature
+2. Install [Docker Desktop](https://docs.docker.com/get-docker/) with the WSL2 backend
+3. Install Python 3.12 via Windows Store
+4. In a PowerShell terminal, run
+```bash
+pip install signal-export
+```
+5. Run the script like this (you can enter any directory, it will be created)
+```bash
+sigexport C:\Temp\SignalExport
+```
+Run it without any arguments to get instructions about other options
+```bash
+sigexport
+```
 
-Then install this package:
+**NB** You may get an error like `term 'sigexport' is not recognized`, in which case you can use the following:
+```bash
+python -m sigexport.main ~/signal-chats
+```
+
+## 🐧 Installation: Linux
+1. [Install Docker](https://docs.docker.com/get-docker/) (including following the [post-installation steps](https://docs.docker.com/engine/install/linux-postinstall/) for managing Docker as a non-root user).  
+2. Make sure you have Python installed.
+
+3. Install this package:
 ```bash
 pip install signal-export
 ```
 
-Then run the script!
-It will do some Docker stuff under the hood to get your data out of the encrypted database.
+4. Then run the script! It will do some Docker stuff under the hood to get your data out of the encrypted database.
 ```bash
 sigexport ~/signal-chats
 # output will be saved to the supplied directory
 ```
 
-**NB** On Windows/PowerShell, you may get an error like `term 'sigexport' is not recognized`, in which case you can use the following:
+### Linux without Docker
+1. Install the required libraries.
 ```bash
-python -m sigexport.main ~/signal-chats
+sudo apt install libsqlite3-dev tclsh libssl-dev
+```
+
+2. Then clone [sqlcipher](https://github.com/sqlcipher/sqlcipher) and install it:
+```bash
+git clone https://github.com/sqlcipher/sqlcipher.git
+cd sqlcipher
+./configure --enable-tempstore=yes CFLAGS="-DSQLITE_HAS_CODEC" LDFLAGS="-lcrypto -lsqlite3"
+make && sudo make install
+```
+
+3. Then you can install and run signal-export without Docker:
+```bash
+pip install 'signal-export[sql]'
+sigexport --no-use-docker ...
+```
+
+## 🍏 Installation: macOS
+To use it with Docker, just follow the standard Linux instructions above.
+
+### macOS without Docker
+1. Install [Homebrew](https://brew.sh).
+2. Run `brew install openssl sqlcipher`
+3. Export some needed env vars:
+```bash
+export C_INCLUDE_PATH="$(brew --prefix sqlcipher)/include"
+export LIBRARY_PATH="${brew --prefix sqlcipher)/lib"
+```
+
+4. Then you can install and run signal-export without Docker:
+```bash
+pip install 'signal-export[sql]'
+sigexport --no-use-docker ...
 ```
 
-## Usage
+## 🚀 Usage
 Please fully exit your Signal app before proceeding, otherwise you will likely encounter an `I/O disk` error, due to the message database being made read-only, as it was being accessed by the app.
 
 See the full help info:
 ```bash
 sigexport --help
 ```
 
@@ -105,88 +185,16 @@
   -v "$SIGNAL_INPUT:/Signal:ro" \
   -v "$SIGNAL_OUTPUT:/output" \
     carderne/sigexport:latest \
     --overwrite /output \         # this line is obligatory!
     --chats Jim                   # this line isn't
 ```
 
-## 🗻 BYOD (Build-Your-Own-Docker) image
-Running this script using the methods above requires you to trust that I haven't snuck anything into the Docker image.
-You can inspect the code in this repo, and after `pip install`ing, you can confirm that the code installed on your computer matches this repo.
-But the methods above rely on the [Docker image](https://hub.docker.com/r/carderne/sigexport), which is a bit more complex.
-
-You can check the [Dockerfile](./Dockerfile) in this repo, and the [GitHub Actions workflow](./.github/workflows/cicd.yaml).
-You can check that the last [Actions run](https://github.com/carderne/signal-export/actions) matches the time on the last push to the DockerHub registry.
-But you can't guarantee that I didn't sneak something in, so the next thing is to check the image itself.
-
-So you can run `docker inspect carderne/sigexport` and check the `Entrypoint` and `Cmd` values.
-Then you can run `docker run --rm -it --entrypoint='' carderne/sigexport bash` and check what Entrypoint/Cmd values correspond to inside the container, and check that _that_ matches the repo!
-
-You can also just build your own Docker image from this repo:
-```bash
-git clone https://github.com/carderne/signal-export.git
-cd signal-export
-docker build -t yourname/sigexport .
-```
-
-And _then_ run the Python script, but tell it to use the image you just created:
-```bash
-sigexport --docker-image yourname/sigexport outputdir/
-```
-
-## 🌋 No-Docker install
-This is hard mode, and involves installing more stuff.
-Probably easy on macOS, slightly involved on Linux, and impossible on Windows.
-
-Before you can install `signal-export`, you need to get `sqlcipher` working.
-Follow the instructions for your OS:
-
-### Ubuntu (other distros can adapt to their package manager)
-Install the required libraries.
-```bash
-sudo apt install libsqlite3-dev tclsh libssl-dev
-```
-
-Then clone [sqlcipher](https://github.com/sqlcipher/sqlcipher) and install it:
-```bash
-git clone https://github.com/sqlcipher/sqlcipher.git
-cd sqlcipher
-./configure --enable-tempstore=yes CFLAGS="-DSQLITE_HAS_CODEC" LDFLAGS="-lcrypto -lsqlite3"
-make && sudo make install
-```
-
-### macOS
-1. Install [Homebrew](https://brew.sh).
-2. Run `brew install openssl sqlcipher`
-3. Export some needed env vars:
-```bash
-export C_INCLUDE_PATH="$(brew --prefix sqlcipher)/include"
-export LIBRARy_PATH="${brew --prefix sqlcipher)/lib"
-```
-
-### Windows
-Ubuntu on WSL2 should work!
-That is, install WSL2 and Ubuntu on Windows, and then follow the **For Linux** instructions and feel your way forward.
-But probably just give up here and use the Docker method instead.
-
-### Install signal-export
-Then you're ready to install signal-export:
-(Note the `[sql]` that has been added!)
-```bash
-pip install 'signal-export[sql]'
-```
-
 Then you should be able to use the [Usage instructions](#usage) as above.
 
-## Uninstall
-```bash
-docker system prune
-pip uninstall signal-export
-```
-
 ## Development
 ```bash
 git clone https://github.com/carderne/signal-export.git
 cd signal-export
 rye sync --no-lock
 ```
```

### Comparing `signal_export-2.2.2/pyproject.toml` & `signal_export-2.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -89,18 +89,18 @@
 ]
 dependencies = [
     "beautifulsoup4 ~= 4.11",
     "emoji ~= 2.0",
     "Markdown ~= 3.4",
     "typer[all] ~= 0.7",
 ]
-version = "2.2.2"
+version = "2.3.0"
 
 [project.license]
-text = "BSD 3-Clause License"
+text = "MIT License"
 
 [project.optional-dependencies]
 sql = [
     "pysqlcipher3 == 1.1.0; python_version <  \"3.11\"",
     "pysqlcipher3 >= 1.2.0; python_version >= \"3.11\"",
 ]
```

### Comparing `signal_export-2.2.2/sigexport/create.py` & `signal_export-2.3.0/sigexport/create.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.2.2/sigexport/data.py` & `signal_export-2.3.0/sigexport/data.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.2.2/sigexport/files.py` & `signal_export-2.3.0/sigexport/files.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.2.2/sigexport/html.py` & `signal_export-2.3.0/sigexport/html.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.2.2/sigexport/main.py` & `signal_export-2.3.0/sigexport/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sys
 from dataclasses import asdict
 from pathlib import Path
 from typing import Optional
 
 from typer import Argument, Exit, Option, colors, run, secho
 
-from sigexport import __version__, create, files, html, logging, merge, models, utils
+from sigexport import create, files, html, logging, merge, models, utils
 from sigexport.logging import log
 
 DATA_DELIM = "-----DATA-----"
 
 
 # these are here because tiangolo/typer doesn't like Foo | None syntax
 OptionalPath = Optional[Path]
@@ -75,15 +75,15 @@
         secho(f"Error: {source} not found in directory {src}")
         raise Exit(code=1)
 
     log(f"Fetching data from {db_file}\n")
 
     if use_docker:
         if not docker_image:
-            docker_version = __version__.split(".dev")[0]
+            docker_version = utils.VERSION.split(".dev")[0]
             docker_image = f"carderne/sigexport:v{docker_version}"
         secho(
             "Using Docker to extract data, this may take a while the first time!",
             fg=colors.BLUE,
         )
         cmd = [
             "docker",
```

### Comparing `signal_export-2.2.2/sigexport/merge.py` & `signal_export-2.3.0/sigexport/merge.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.2.2/sigexport/models.py` & `signal_export-2.3.0/sigexport/models.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.2.2/sigexport/style.css` & `signal_export-2.3.0/sigexport/style.css`

 * *Files identical despite different names*

### Comparing `signal_export-2.2.2/sigexport/templates.py` & `signal_export-2.3.0/sigexport/templates.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.2.2/sigexport/utils.py` & `signal_export-2.3.0/sigexport/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import sys
 from datetime import datetime
+from importlib.metadata import version
 from pathlib import Path
 from typing import cast
 
 import emoji
 from typer import Exit, secho
 
-from sigexport import __version__, models
+from sigexport import models
+
+VERSION = version("signal-export")
 
 
 def dt_from_ts(ts: float) -> datetime:
     return datetime.fromtimestamp(ts / 1000.0)
 
 
 def parse_datetime(input_str: str) -> datetime:
@@ -28,15 +31,15 @@
     exception = cast(ValueError, last_exception)
     raise (exception)
 
 
 def version_callback(value: bool) -> None:
     """Get sigexport version."""
     if value:
-        print(f"v{__version__}")
+        print(f"v{VERSION}")
         raise Exit()
 
 
 def source_location() -> Path:
     """Get OS-dependent source location."""
     home = Path.home()
     paths = {
```

### Comparing `signal_export-2.2.2/tests/data/attachments.noindex/image.jpeg` & `signal_export-2.3.0/tests/data/attachments.noindex/image.jpeg`

 * *Files identical despite different names*

### Comparing `signal_export-2.2.2/tests/data/attachments.noindex/voicenote.m4a` & `signal_export-2.3.0/tests/data/attachments.noindex/voicenote.m4a`

 * *Files identical despite different names*

### Comparing `signal_export-2.2.2/tests/data/sql/db.sqlite` & `signal_export-2.3.0/tests/data/sql/db.sqlite`

 * *Files identical despite different names*

### Comparing `signal_export-2.2.2/tests/test_integration.py` & `signal_export-2.3.0/tests/test_integration.py`

 * *Files identical despite different names*

