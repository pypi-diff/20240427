# Comparing `tmp/jaraco_home-3.8.1.tar.gz` & `tmp/jaraco_home-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco_home-3.8.1.tar", last modified: Tue Apr 16 02:05:14 2024, max compression
+gzip compressed data, was "jaraco_home-3.9.0.tar", last modified: Sat Apr 27 14:08:05 2024, max compression
```

## Comparing `jaraco_home-3.8.1.tar` & `jaraco_home-3.9.0.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:05:14.024095 jaraco_home-3.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:05:14.020095 jaraco_home-3.8.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:05:14.020095 jaraco_home-3.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-16 02:05:14.024095 jaraco_home-3.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:05:14.020095 jaraco_home-3.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:05:14.016095 jaraco_home-3.8.1/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:05:14.020095 jaraco_home-3.8.1/jaraco/home/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/jaraco/home/Gather HDHomeRun Stats.plist
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/jaraco/home/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/jaraco/home/check-traps.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/jaraco/home/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/jaraco/home/hdhomerun.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/jaraco/home/mock hdhomerun.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/jaraco/home/relay.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/jaraco/home/report-spam-call.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/jaraco/home/thermostat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:05:14.024095 jaraco_home-3.8.1/jaraco.home.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-16 02:05:13.000000 jaraco_home-3.8.1/jaraco.home.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-16 02:05:14.000000 jaraco_home-3.8.1/jaraco.home.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 02:05:13.000000 jaraco_home-3.8.1/jaraco.home.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-16 02:05:13.000000 jaraco_home-3.8.1/jaraco.home.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 02:05:13.000000 jaraco_home-3.8.1/jaraco.home.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-16 02:05:14.024095 jaraco_home-3.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:08:05.313402 jaraco_home-3.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:08:05.305402 jaraco_home-3.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:08:05.305402 jaraco_home-3.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-27 14:08:05.313402 jaraco_home-3.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:08:05.305402 jaraco_home-3.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:08:05.301402 jaraco_home-3.9.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:08:05.309402 jaraco_home-3.9.0/jaraco/home/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/jaraco/home/Gather HDHomeRun Stats.plist
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/jaraco/home/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/jaraco/home/check-traps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:08:05.309402 jaraco_home-3.9.0/jaraco/home/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/jaraco/home/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/jaraco/home/compat/py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/jaraco/home/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/jaraco/home/hdhomerun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/jaraco/home/mock hdhomerun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/jaraco/home/relay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/jaraco/home/report-spam-call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/jaraco/home/thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:08:05.309402 jaraco_home-3.9.0/jaraco.home.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-27 14:08:05.000000 jaraco_home-3.9.0/jaraco.home.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-27 14:08:05.000000 jaraco_home-3.9.0/jaraco.home.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 14:08:05.000000 jaraco_home-3.9.0/jaraco.home.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-27 14:08:05.000000 jaraco_home-3.9.0/jaraco.home.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-27 14:08:05.000000 jaraco_home-3.9.0/jaraco.home.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 14:08:05.313402 jaraco_home-3.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-27 14:07:44.000000 jaraco_home-3.9.0/tox.ini
```

### Comparing `jaraco_home-3.8.1/.github/workflows/main.yml` & `jaraco_home-3.9.0/.github/workflows/main.yml`

 * *Files 4% similar despite different names*

```diff
@@ -27,17 +27,18 @@
   TOX_OVERRIDE: >-
     testenv.pass_env+=GITHUB_*,FORCE_COLOR
 
 
 jobs:
   test:
     strategy:
+      # https://blog.jaraco.com/efficient-use-of-ci-resources/
       matrix:
         python:
-        - "3.9"
+        - "3.8"
         - "3.12"
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
         - python: "3.9"
@@ -50,15 +51,15 @@
           platform: ubuntu-latest
         exclude:
         # lxml fails to build on Windows
         # https://bugs.launchpad.net/lxml/+bug/1977998
         - platform: windows-latest
           python: '3.11'
     runs-on: ${{ matrix.platform }}
-    continue-on-error: ${{ matrix.python == '3.13' }}
+    continue-on-error: ${{ matrix.python == '3.13' || (matrix.python == '3.8' || matrix.python == '3.9') && matrix.platform == 'macos-latest' }}
     steps:
       - uses: actions/checkout@v4
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
           allow-prereleases: true
```

### Comparing `jaraco_home-3.8.1/LICENSE` & `jaraco_home-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco_home-3.8.1/NEWS.rst` & `jaraco_home-3.9.0/NEWS.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v3.9.0
+======
+
+Features
+--------
+
+- Restored Python 3.8 compatibility.
+
+
 v3.8.1
 ======
 
 Bugfixes
 --------
 
 - Fix check-traps to actually reflect status.
```

### Comparing `jaraco_home-3.8.1/PKG-INFO` & `jaraco_home-3.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: jaraco.home
-Version: 3.8.1
+Version: 3.9.0
 Summary: Some functions supporting the devices in jaraco's home
-Home-page: https://github.com/jaraco/jaraco.home
-Author: Jason R. Coombs
-Author-email: jaraco@jaraco.com
+Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
+Project-URL: Homepage, https://github.com/jaraco/jaraco.home
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.9
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: lxml>=4.2.6
 Requires-Dist: pymongo
 Requires-Dist: jaraco.functools
 Requires-Dist: jaraco.mongodb
 Requires-Dist: dnspython
 Requires-Dist: keyring
 Requires-Dist: jaraco.collections
 Requires-Dist: splinter[selenium]
 Requires-Dist: autocommand
 Requires-Dist: python-dateutil
 Requires-Dist: victor-smart-kill
+Requires-Dist: importlib_resources; python_version < "3.9"
+Requires-Dist: lxml<5; python_version < "3.9" and platform_system == "Darwin"
 Provides-Extra: testing
-Requires-Dist: pytest!=8.1.1,>=6; extra == "testing"
+Requires-Dist: pytest!=8.1.*,>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-mypy; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
 Requires-Dist: types-requests; extra == "testing"
 Requires-Dist: mockproc; extra == "testing"
```

### Comparing `jaraco_home-3.8.1/README.rst` & `jaraco_home-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `jaraco_home-3.8.1/conftest.py` & `jaraco_home-3.9.0/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import platform
-from importlib.resources import files
 
 import pytest
 from mockproc import mockprocess
 
 win_ignore = [
     'jaraco/home/hdhomerun.py',
 ] * (platform.system() == 'Windows')
@@ -12,16 +11,19 @@
     'jaraco/home/relay.py',
 ] + win_ignore
 
 
 @pytest.fixture(scope='session', autouse=True)
 def hdhomerun_config_mocked():
     import jaraco.home.hdhomerun as hd
+    from jaraco.home.compat.py38 import resources
 
     hd.hdhomerun_config = 'hdhomerun_config'
     scripts = mockprocess.MockProc()
     script = (
-        files('jaraco.home').joinpath('mock hdhomerun.py').read_text(encoding='utf-8')
+        resources.files('jaraco.home')
+        .joinpath('mock hdhomerun.py')
+        .read_text(encoding='utf-8')
     )
     scripts.append('hdhomerun_config', returncode=0, script=script)
     with scripts:
         yield
```

### Comparing `jaraco_home-3.8.1/docs/conf.py` & `jaraco_home-3.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco_home-3.8.1/jaraco/home/Gather HDHomeRun Stats.plist` & `jaraco_home-3.9.0/jaraco/home/Gather HDHomeRun Stats.plist`

 * *Files identical despite different names*

### Comparing `jaraco_home-3.8.1/jaraco/home/check-traps.py` & `jaraco_home-3.9.0/jaraco/home/check-traps.py`

 * *Files identical despite different names*

### Comparing `jaraco_home-3.8.1/jaraco/home/hdhomerun.py` & `jaraco_home-3.9.0/jaraco/home/hdhomerun.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import functools
 import pathlib
 import random
 import re
 import subprocess
 import sys
 import time
-from importlib.resources import files
 
 import keyring
 
+from .compat.py38 import resources
+
 from jaraco.collections import DictStack
 from jaraco.functools import retry
 from jaraco.mongodb.helper import connect_db
 
 
 def parse_field(item):
     key, value = item.split('=')
@@ -108,15 +109,15 @@
     set_channel(tuner, None)
 
 
 def install():
     name = 'Gather HDHomeRun Stats.plist'
     agents = pathlib.Path('~/Library/LaunchAgents').expanduser()
     target = agents / name
-    tmpl_name = files(__package__) / name
+    tmpl_name = resources.files(__package__) / name
     tmpl = tmpl_name.read_text()
     logs = pathlib.Path(sys.executable).parent.parent / 'logs'
     source = tmpl.format(sys=sys, logs=logs)
     target.write_text(source)
     subprocess.check_output(['launchctl', 'load', target])
```

### Comparing `jaraco_home-3.8.1/jaraco/home/relay.py` & `jaraco_home-3.9.0/jaraco/home/relay.py`

 * *Files identical despite different names*

### Comparing `jaraco_home-3.8.1/jaraco/home/report-spam-call.py` & `jaraco_home-3.9.0/jaraco/home/report-spam-call.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 import re
 
 import autocommand
 import dateutil.parser
 from splinter import Browser
 
 from . import contact as contact_info
+from .compat.py38 import removeprefix
+
 
 DROPPED_CALL = '2'
 
 
 def clean_phone(number):
     """
     >>> clean_phone("+1 202 555 1212")
     '2025551212'
     """
-    return re.sub(r'[-. ]', '', number.removeprefix('+1'))
+    return re.sub(r'[-. ]', '', removeprefix(number, '+1'))
 
 
 @autocommand.autocommand(__name__)
 def report_spam_call(
     number,
     comment='',
     close=False,
```

### Comparing `jaraco_home-3.8.1/jaraco/home/thermostat.py` & `jaraco_home-3.9.0/jaraco/home/thermostat.py`

 * *Files identical despite different names*

### Comparing `jaraco_home-3.8.1/jaraco.home.egg-info/PKG-INFO` & `jaraco_home-3.9.0/jaraco.home.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: jaraco.home
-Version: 3.8.1
+Version: 3.9.0
 Summary: Some functions supporting the devices in jaraco's home
-Home-page: https://github.com/jaraco/jaraco.home
-Author: Jason R. Coombs
-Author-email: jaraco@jaraco.com
+Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
+Project-URL: Homepage, https://github.com/jaraco/jaraco.home
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.9
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: lxml>=4.2.6
 Requires-Dist: pymongo
 Requires-Dist: jaraco.functools
 Requires-Dist: jaraco.mongodb
 Requires-Dist: dnspython
 Requires-Dist: keyring
 Requires-Dist: jaraco.collections
 Requires-Dist: splinter[selenium]
 Requires-Dist: autocommand
 Requires-Dist: python-dateutil
 Requires-Dist: victor-smart-kill
+Requires-Dist: importlib_resources; python_version < "3.9"
+Requires-Dist: lxml<5; python_version < "3.9" and platform_system == "Darwin"
 Provides-Extra: testing
-Requires-Dist: pytest!=8.1.1,>=6; extra == "testing"
+Requires-Dist: pytest!=8.1.*,>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-mypy; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
 Requires-Dist: types-requests; extra == "testing"
 Requires-Dist: mockproc; extra == "testing"
```

### Comparing `jaraco_home-3.8.1/jaraco.home.egg-info/SOURCES.txt` & `jaraco_home-3.9.0/jaraco.home.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 NEWS.rst
 README.rst
 conftest.py
 mypy.ini
 pyproject.toml
 pytest.ini
 ruff.toml
-setup.cfg
 towncrier.toml
 tox.ini
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
 docs/history.rst
 docs/index.rst
@@ -27,8 +26,10 @@
 jaraco/home/__init__.py
 jaraco/home/check-traps.py
 jaraco/home/contact.py
 jaraco/home/hdhomerun.py
 jaraco/home/mock hdhomerun.py
 jaraco/home/relay.py
 jaraco/home/report-spam-call.py
-jaraco/home/thermostat.py
+jaraco/home/thermostat.py
+jaraco/home/compat/__init__.py
+jaraco/home/compat/py38.py
```

### Comparing `jaraco_home-3.8.1/pytest.ini` & `jaraco_home-3.9.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco_home-3.8.1/tox.ini` & `jaraco_home-3.9.0/tox.ini`

 * *Files identical despite different names*

