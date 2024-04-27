# Comparing `tmp/caped-ai-tabulour-0.1.2.tar.gz` & `tmp/caped_ai_tabulour-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caped-ai-tabulour-0.1.2.tar", last modified: Mon Oct 16 10:01:53 2023, max compression
+gzip compressed data, was "caped_ai_tabulour-0.1.3.tar", last modified: Sat Apr 27 17:06:04 2024, max compression
```

## Comparing `caped-ai-tabulour-0.1.2.tar` & `caped_ai_tabulour-0.1.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-10-16 10:01:53.593853 caped-ai-tabulour-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-10-16 10:01:53.448986 caped-ai-tabulour-0.1.2/.github/
-drwxrwxrwx   0        0        0        0 2023-10-16 10:01:53.494796 caped-ai-tabulour-0.1.2/.github/workflows/
--rw-rw-rw-   0        0        0     1078 2023-10-14 13:12:23.000000 caped-ai-tabulour-0.1.2/.github/workflows/deploy.yml
--rw-rw-rw-   0        0        0      591 2023-09-09 15:49:23.000000 caped-ai-tabulour-0.1.2/.github/workflows/napari-hub-preview.yml
--rw-rw-rw-   0        0        0     1973 2023-10-14 13:12:32.000000 caped-ai-tabulour-0.1.2/.github/workflows/test_and_deploy.yml
--rw-rw-rw-   0        0        0      991 2023-10-14 12:21:34.000000 caped-ai-tabulour-0.1.2/.gitignore
--rw-rw-rw-   0        0        0     1008 2023-09-09 15:49:23.000000 caped-ai-tabulour-0.1.2/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0     1487 2023-10-14 12:21:34.000000 caped-ai-tabulour-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       96 2023-10-14 12:21:34.000000 caped-ai-tabulour-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3970 2023-10-16 10:01:53.592711 caped-ai-tabulour-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2389 2023-10-14 12:21:34.000000 caped-ai-tabulour-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-10-16 10:01:53.545346 caped-ai-tabulour-0.1.2/licenses/
--rw-rw-rw-   0        0        0    11358 2023-10-14 12:21:34.000000 caped-ai-tabulour-0.1.2/licenses/Apache-2
--rw-rw-rw-   0        0        0     1487 2023-10-14 12:21:34.000000 caped-ai-tabulour-0.1.2/licenses/BSD-3
--rw-rw-rw-   0        0        0    35148 2023-10-14 12:21:34.000000 caped-ai-tabulour-0.1.2/licenses/GPL-3
--rw-rw-rw-   0        0        0     7653 2023-10-14 12:21:34.000000 caped-ai-tabulour-0.1.2/licenses/LGPL-3
--rw-rw-rw-   0        0        0     1080 2023-10-14 12:21:34.000000 caped-ai-tabulour-0.1.2/licenses/MIT
--rw-rw-rw-   0        0        0    16726 2023-10-14 12:21:34.000000 caped-ai-tabulour-0.1.2/licenses/MPL-2
--rw-rw-rw-   0        0        0       91 2023-10-14 13:43:24.000000 caped-ai-tabulour-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0     1787 2023-10-16 10:01:53.595018 caped-ai-tabulour-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-10-16 10:01:53.449986 caped-ai-tabulour-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-10-16 10:01:53.554891 caped-ai-tabulour-0.1.2/src/caped_ai_tabulour/
--rw-rw-rw-   0        0        0      107 2023-10-14 13:36:32.000000 caped-ai-tabulour-0.1.2/src/caped_ai_tabulour/__init__.py
--rw-rw-rw-   0        0        0     3929 2023-10-14 13:02:31.000000 caped-ai-tabulour-0.1.2/src/caped_ai_tabulour/_data_model.py
--rw-rw-rw-   0        0        0     8564 2023-10-14 12:21:34.000000 caped-ai-tabulour-0.1.2/src/caped_ai_tabulour/_tabulour.py
-drwxrwxrwx   0        0        0        0 2023-10-16 10:01:53.590405 caped-ai-tabulour-0.1.2/src/caped_ai_tabulour/_tests/
--rw-rw-rw-   0        0        0        0 2023-10-14 12:21:34.000000 caped-ai-tabulour-0.1.2/src/caped_ai_tabulour/_tests/__init__.py
--rw-rw-rw-   0        0        0     2073 2023-10-14 12:21:34.000000 caped-ai-tabulour-0.1.2/src/caped_ai_tabulour/_tests/test_tabulour.py
--rw-rw-rw-   0        0        0       80 2023-10-16 09:59:31.000000 caped-ai-tabulour-0.1.2/src/caped_ai_tabulour/_version.py
--rw-rw-rw-   0        0        0       69 2023-10-14 12:21:34.000000 caped-ai-tabulour-0.1.2/src/caped_ai_tabulour/caped.yaml
-drwxrwxrwx   0        0        0        0 2023-10-16 10:01:53.589406 caped-ai-tabulour-0.1.2/src/caped_ai_tabulour.egg-info/
--rw-rw-rw-   0        0        0     3970 2023-10-16 10:01:53.000000 caped-ai-tabulour-0.1.2/src/caped_ai_tabulour.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      847 2023-10-16 10:01:53.000000 caped-ai-tabulour-0.1.2/src/caped_ai_tabulour.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-16 10:01:53.000000 caped-ai-tabulour-0.1.2/src/caped_ai_tabulour.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-10-16 10:01:53.000000 caped-ai-tabulour-0.1.2/src/caped_ai_tabulour.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-10-16 10:01:53.000000 caped-ai-tabulour-0.1.2/src/caped_ai_tabulour.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-10-16 10:01:53.000000 caped-ai-tabulour-0.1.2/src/caped_ai_tabulour.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      612 2023-10-14 12:21:34.000000 caped-ai-tabulour-0.1.2/tox.ini
--rw-rw-rw-   0        0        0      620 2023-10-14 13:03:59.000000 caped-ai-tabulour-0.1.2/update_version.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-04-27 17:06:04.874544 caped_ai_tabulour-0.1.3/
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-04-27 17:06:04.862544 caped_ai_tabulour-0.1.3/.github/
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-04-27 17:06:04.866544 caped_ai_tabulour-0.1.3/.github/workflows/
+-rw-r--r--   0 debian    (1000) debian    (1000)     1078 2024-04-27 16:28:13.000000 caped_ai_tabulour-0.1.3/.github/workflows/deploy.yml
+-rw-r--r--   0 debian    (1000) debian    (1000)      591 2024-04-27 16:28:13.000000 caped_ai_tabulour-0.1.3/.github/workflows/napari-hub-preview.yml
+-rw-r--r--   0 debian    (1000) debian    (1000)     1973 2024-04-27 16:28:13.000000 caped_ai_tabulour-0.1.3/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 debian    (1000) debian    (1000)      947 2024-04-27 16:48:54.000000 caped_ai_tabulour-0.1.3/.gitignore
+-rw-r--r--   0 debian    (1000) debian    (1000)     1008 2024-04-27 16:28:13.000000 caped_ai_tabulour-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-04-27 16:28:13.000000 caped_ai_tabulour-0.1.3/LICENSE
+-rw-r--r--   0 debian    (1000) debian    (1000)       96 2024-04-27 16:28:13.000000 caped_ai_tabulour-0.1.3/MANIFEST.in
+-rw-r--r--   0 debian    (1000) debian    (1000)     3873 2024-04-27 17:06:04.874544 caped_ai_tabulour-0.1.3/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)     2389 2024-04-27 16:28:13.000000 caped_ai_tabulour-0.1.3/README.md
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-04-27 17:06:04.870544 caped_ai_tabulour-0.1.3/licenses/
+-rw-r--r--   0 debian    (1000) debian    (1000)    11358 2024-04-27 16:28:13.000000 caped_ai_tabulour-0.1.3/licenses/Apache-2
+-rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-04-27 16:28:13.000000 caped_ai_tabulour-0.1.3/licenses/BSD-3
+-rw-r--r--   0 debian    (1000) debian    (1000)    35148 2024-04-27 16:28:13.000000 caped_ai_tabulour-0.1.3/licenses/GPL-3
+-rw-r--r--   0 debian    (1000) debian    (1000)     7653 2024-04-27 16:28:13.000000 caped_ai_tabulour-0.1.3/licenses/LGPL-3
+-rw-r--r--   0 debian    (1000) debian    (1000)     1080 2024-04-27 16:28:13.000000 caped_ai_tabulour-0.1.3/licenses/MIT
+-rw-r--r--   0 debian    (1000) debian    (1000)    16726 2024-04-27 16:28:13.000000 caped_ai_tabulour-0.1.3/licenses/MPL-2
+-rw-r--r--   0 debian    (1000) debian    (1000)      116 2024-04-27 17:05:12.000000 caped_ai_tabulour-0.1.3/pyproject.toml
+-rw-r--r--   0 debian    (1000) debian    (1000)     1726 2024-04-27 17:06:04.874544 caped_ai_tabulour-0.1.3/setup.cfg
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-04-27 17:06:04.862544 caped_ai_tabulour-0.1.3/src/
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-04-27 17:06:04.870544 caped_ai_tabulour-0.1.3/src/caped_ai_tabulour/
+-rw-r--r--   0 debian    (1000) debian    (1000)      107 2024-04-27 16:28:13.000000 caped_ai_tabulour-0.1.3/src/caped_ai_tabulour/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     3220 2024-04-27 16:48:55.000000 caped_ai_tabulour-0.1.3/src/caped_ai_tabulour/_data_model.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     8564 2024-04-27 16:28:13.000000 caped_ai_tabulour-0.1.3/src/caped_ai_tabulour/_tabulour.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-04-27 17:06:04.870544 caped_ai_tabulour-0.1.3/src/caped_ai_tabulour/_tests/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2024-04-27 16:28:13.000000 caped_ai_tabulour-0.1.3/src/caped_ai_tabulour/_tests/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     2073 2024-04-27 16:28:13.000000 caped_ai_tabulour-0.1.3/src/caped_ai_tabulour/_tests/test_tabulour.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       78 2024-04-27 16:49:01.000000 caped_ai_tabulour-0.1.3/src/caped_ai_tabulour/_version.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       69 2024-04-27 16:28:13.000000 caped_ai_tabulour-0.1.3/src/caped_ai_tabulour/caped.yaml
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-04-27 17:06:04.870544 caped_ai_tabulour-0.1.3/src/caped_ai_tabulour.egg-info/
+-rw-r--r--   0 debian    (1000) debian    (1000)     3873 2024-04-27 17:06:04.000000 caped_ai_tabulour-0.1.3/src/caped_ai_tabulour.egg-info/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)      847 2024-04-27 17:06:04.000000 caped_ai_tabulour-0.1.3/src/caped_ai_tabulour.egg-info/SOURCES.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)        1 2024-04-27 17:06:04.000000 caped_ai_tabulour-0.1.3/src/caped_ai_tabulour.egg-info/dependency_links.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       66 2024-04-27 17:06:04.000000 caped_ai_tabulour-0.1.3/src/caped_ai_tabulour.egg-info/entry_points.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       53 2024-04-27 17:06:04.000000 caped_ai_tabulour-0.1.3/src/caped_ai_tabulour.egg-info/requires.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       18 2024-04-27 17:06:04.000000 caped_ai_tabulour-0.1.3/src/caped_ai_tabulour.egg-info/top_level.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)      612 2024-04-27 16:28:13.000000 caped_ai_tabulour-0.1.3/tox.ini
+-rw-r--r--   0 debian    (1000) debian    (1000)      620 2024-04-27 16:28:13.000000 caped_ai_tabulour-0.1.3/update_version.py
```

### Comparing `caped-ai-tabulour-0.1.2/.github/workflows/deploy.yml` & `caped_ai_tabulour-0.1.3/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `caped-ai-tabulour-0.1.2/.github/workflows/napari-hub-preview.yml` & `caped_ai_tabulour-0.1.3/.github/workflows/napari-hub-preview.yml`

 * *Files identical despite different names*

### Comparing `caped-ai-tabulour-0.1.2/.github/workflows/test_and_deploy.yml` & `caped_ai_tabulour-0.1.3/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `caped-ai-tabulour-0.1.2/.gitignore` & `caped_ai_tabulour-0.1.3/.gitignore`

 * *Files 11% similar despite different names*

```diff
@@ -75,10 +75,7 @@
 .ipynb_checkpoints
 
 # pyenv
 .python-version
 
 # OS
 .DS_Store
-
-# written by setuptools_scm
-**/_version.py
```

### Comparing `caped-ai-tabulour-0.1.2/.pre-commit-config.yaml` & `caped_ai_tabulour-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `caped-ai-tabulour-0.1.2/LICENSE` & `caped_ai_tabulour-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `caped-ai-tabulour-0.1.2/PKG-INFO` & `caped_ai_tabulour-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-Metadata-Version: 2.1
-Name: caped-ai-tabulour
-Version: 0.1.2
-Summary: A base table widget for KapoorLabs Napari plugins
-Home-page: https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour
-Author: Varun Kapoor
-Author-email: randomaccessiblekapoor@gmail.com
-License: BSD-3-Clause
-Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/issues
-Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour#README.md
-Project-URL: Source Code, https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour
-Project-URL: User Support, https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/issues
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: napari
-Requires-Dist: pandas
-Requires-Dist: numpy
-Provides-Extra: testing
-Requires-Dist: tox; extra == "testing"
-Requires-Dist: pytest; extra == "testing"
-Requires-Dist: pytest-cov; extra == "testing"
-
-# caped-ai-tabulour
-
-[![License BSD-3](https://img.shields.io/pypi/l/caped-ai-tabulour.svg?color=green)](https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/raw/main/LICENSE)
-[![PyPI](https://img.shields.io/pypi/v/caped-ai-tabulour.svg?color=green)](https://pypi.org/project/caped-ai-tabulour)
-[![Python Version](https://img.shields.io/pypi/pyversions/caped-ai-tabulour.svg?color=green)](https://python.org)
-[![tests](https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/workflows/tests/badge.svg)](https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/actions)
-[![codecov](https://codecov.io/gh/Kapoorlabs-CAPED/caped-ai-tabulour/branch/main/graph/badge.svg)](https://codecov.io/gh/Kapoorlabs-CAPED/caped-ai-tabulour)
-
-
-A base table widget for KapoorLabs Napari plugins
-
-----------------------------------
-
-This [caped] package was generated with [Cookiecutter] using [@caped]'s [cookiecutter-template] template.
-
-
-
-## Installation
-
-You can install `caped-ai-tabulour` via [pip]:
-
-    pip install caped-ai-tabulour
-
-
-
-To install latest development version :
-
-    pip install git+https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour.git
-
-
-## Contributing
-
-Contributions are very welcome. Tests can be run with [tox], please ensure
-the coverage at least stays the same before you submit a pull request.
-
-## License
-
-Distributed under the terms of the [BSD-3] license,
-"caped-ai-tabulour" is free and open source software
-
-## Issues
-
-If you encounter any problems, please [file an issue] along with a detailed description.
-
-
-[pip]: https://pypi.org/project/pip/
-[caped]: https://github.com/Kapoorlabs-CAPED
-[Cookiecutter]: https://github.com/audreyr/cookiecutter
-[@caped]: https://github.com/Kapoorlabs-CAPED
-[MIT]: http://opensource.org/licenses/MIT
-[BSD-3]: http://opensource.org/licenses/BSD-3-Clause
-[GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
-[GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
-[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
-[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
-[cookiecutter-template]: https://github.com/Kapoorlabs-CAPED/cookiecutter-template
-
-[file an issue]: https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/issues
-
-[caped]: https://github.com/Kapoorlabs-CAPED/
-[tox]: https://tox.readthedocs.io/en/latest/
-[pip]: https://pypi.org/project/pip/
-[PyPI]: https://pypi.org/
+Metadata-Version: 2.1
+Name: caped-ai-tabulour
+Version: 0.1.3
+Summary: A base table widget for KapoorLabs Napari plugins
+Home-page: https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour
+Author: Varun Kapoor
+Author-email: randomaccessiblekapoor@gmail.com
+License: BSD-3-Clause
+Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/issues
+Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour#README.md
+Project-URL: Source Code, https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour
+Project-URL: User Support, https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/issues
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: napari
+Requires-Dist: pandas
+Requires-Dist: numpy
+Provides-Extra: testing
+Requires-Dist: tox; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+
+# caped-ai-tabulour
+
+[![License BSD-3](https://img.shields.io/pypi/l/caped-ai-tabulour.svg?color=green)](https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/raw/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/caped-ai-tabulour.svg?color=green)](https://pypi.org/project/caped-ai-tabulour)
+[![Python Version](https://img.shields.io/pypi/pyversions/caped-ai-tabulour.svg?color=green)](https://python.org)
+[![tests](https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/workflows/tests/badge.svg)](https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/actions)
+[![codecov](https://codecov.io/gh/Kapoorlabs-CAPED/caped-ai-tabulour/branch/main/graph/badge.svg)](https://codecov.io/gh/Kapoorlabs-CAPED/caped-ai-tabulour)
+
+
+A base table widget for KapoorLabs Napari plugins
+
+----------------------------------
+
+This [caped] package was generated with [Cookiecutter] using [@caped]'s [cookiecutter-template] template.
+
+
+
+## Installation
+
+You can install `caped-ai-tabulour` via [pip]:
+
+    pip install caped-ai-tabulour
+
+
+
+To install latest development version :
+
+    pip install git+https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour.git
+
+
+## Contributing
+
+Contributions are very welcome. Tests can be run with [tox], please ensure
+the coverage at least stays the same before you submit a pull request.
+
+## License
+
+Distributed under the terms of the [BSD-3] license,
+"caped-ai-tabulour" is free and open source software
+
+## Issues
+
+If you encounter any problems, please [file an issue] along with a detailed description.
+
+
+[pip]: https://pypi.org/project/pip/
+[caped]: https://github.com/Kapoorlabs-CAPED
+[Cookiecutter]: https://github.com/audreyr/cookiecutter
+[@caped]: https://github.com/Kapoorlabs-CAPED
+[MIT]: http://opensource.org/licenses/MIT
+[BSD-3]: http://opensource.org/licenses/BSD-3-Clause
+[GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
+[GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
+[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
+[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
+[cookiecutter-template]: https://github.com/Kapoorlabs-CAPED/cookiecutter-template
+
+[file an issue]: https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/issues
+
+[caped]: https://github.com/Kapoorlabs-CAPED/
+[tox]: https://tox.readthedocs.io/en/latest/
+[pip]: https://pypi.org/project/pip/
+[PyPI]: https://pypi.org/
```

### Comparing `caped-ai-tabulour-0.1.2/README.md` & `caped_ai_tabulour-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `caped-ai-tabulour-0.1.2/licenses/Apache-2` & `caped_ai_tabulour-0.1.3/licenses/Apache-2`

 * *Files identical despite different names*

### Comparing `caped-ai-tabulour-0.1.2/licenses/BSD-3` & `caped_ai_tabulour-0.1.3/licenses/BSD-3`

 * *Files identical despite different names*

### Comparing `caped-ai-tabulour-0.1.2/licenses/GPL-3` & `caped_ai_tabulour-0.1.3/licenses/GPL-3`

 * *Files identical despite different names*

### Comparing `caped-ai-tabulour-0.1.2/licenses/LGPL-3` & `caped_ai_tabulour-0.1.3/licenses/LGPL-3`

 * *Files identical despite different names*

### Comparing `caped-ai-tabulour-0.1.2/licenses/MIT` & `caped_ai_tabulour-0.1.3/licenses/MIT`

 * *Files identical despite different names*

### Comparing `caped-ai-tabulour-0.1.2/licenses/MPL-2` & `caped_ai_tabulour-0.1.3/licenses/MPL-2`

 * *Files identical despite different names*

### Comparing `caped-ai-tabulour-0.1.2/setup.cfg` & `caped_ai_tabulour-0.1.3/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,112 +1,108 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2063 6170 6564 2d61 692d 7461 6275   = caped-ai-tabu
-00000020: 6c6f 7572 0d0a 7665 7273 696f 6e20 3d20  lour..version = 
-00000030: 6174 7472 3a20 6361 7065 645f 6169 5f74  attr: caped_ai_t
-00000040: 6162 756c 6f75 722e 5f76 6572 7369 6f6e  abulour._version
-00000050: 2e5f 5f76 6572 7369 6f6e 5f5f 0d0a 6465  .__version__..de
-00000060: 7363 7269 7074 696f 6e20 3d20 4120 6261  scription = A ba
-00000070: 7365 2074 6162 6c65 2077 6964 6765 7420  se table widget 
-00000080: 666f 7220 4b61 706f 6f72 4c61 6273 204e  for KapoorLabs N
-00000090: 6170 6172 6920 706c 7567 696e 730d 0a6c  apari plugins..l
-000000a0: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
-000000b0: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
-000000c0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
-000000d0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-000000e0: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
-000000f0: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
-00000100: 6769 7468 7562 2e63 6f6d 2f4b 6170 6f6f  github.com/Kapoo
-00000110: 726c 6162 732d 4341 5045 442f 6361 7065  rlabs-CAPED/cape
-00000120: 642d 6169 2d74 6162 756c 6f75 720d 0a61  d-ai-tabulour..a
-00000130: 7574 686f 7220 3d20 5661 7275 6e20 4b61  uthor = Varun Ka
-00000140: 706f 6f72 0d0a 6175 7468 6f72 5f65 6d61  poor..author_ema
-00000150: 696c 203d 2072 616e 646f 6d61 6363 6573  il = randomacces
-00000160: 7369 626c 656b 6170 6f6f 7240 676d 6169  siblekapoor@gmai
-00000170: 6c2e 636f 6d0d 0a6c 6963 656e 7365 203d  l.com..license =
-00000180: 2042 5344 2d33 2d43 6c61 7573 650d 0a6c   BSD-3-Clause..l
-00000190: 6963 656e 7365 5f66 696c 6573 203d 204c  icense_files = L
-000001a0: 4943 454e 5345 0d0a 636c 6173 7369 6669  ICENSE..classifi
-000001b0: 6572 7320 3d20 0d0a 0944 6576 656c 6f70  ers = ...Develop
-000001c0: 6d65 6e74 2053 7461 7475 7320 3a3a 2035  ment Status :: 5
-000001d0: 202d 2050 726f 6475 6374 696f 6e2f 5374   - Production/St
-000001e0: 6162 6c65 0d0a 0949 6e74 656e 6465 6420  able...Intended 
-000001f0: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
-00000200: 6c6f 7065 7273 0d0a 094c 6963 656e 7365  lopers...License
-00000210: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-00000220: 203a 3a20 4253 4420 4c69 6365 6e73 650d   :: BSD License.
-00000230: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
-00000240: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
-00000250: 6465 6e74 0d0a 0950 726f 6772 616d 6d69  dent...Programmi
-00000260: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000270: 7974 686f 6e0d 0a09 5072 6f67 7261 6d6d  ython...Programm
-00000280: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000290: 5079 7468 6f6e 203a 3a20 330d 0a09 5072  Python :: 3...Pr
-000002a0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000002b0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000002c0: 3320 3a3a 204f 6e6c 790d 0a09 5072 6f67  3 :: Only...Prog
-000002d0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000002e0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-000002f0: 380d 0a09 5072 6f67 7261 6d6d 696e 6720  8...Programming 
-00000300: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000310: 6f6e 203a 3a20 332e 390d 0a09 5072 6f67  on :: 3.9...Prog
-00000320: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000330: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000340: 3130 0d0a 0954 6f70 6963 203a 3a20 5363  10...Topic :: Sc
-00000350: 6965 6e74 6966 6963 2f45 6e67 696e 6565  ientific/Enginee
-00000360: 7269 6e67 203a 3a20 496d 6167 6520 5072  ring :: Image Pr
-00000370: 6f63 6573 7369 6e67 0d0a 7072 6f6a 6563  ocessing..projec
-00000380: 745f 7572 6c73 203d 200d 0a09 4275 6720  t_urls = ...Bug 
-00000390: 5472 6163 6b65 7220 3d20 6874 7470 733a  Tracker = https:
-000003a0: 2f2f 6769 7468 7562 2e63 6f6d 2f4b 6170  //github.com/Kap
-000003b0: 6f6f 726c 6162 732d 4341 5045 442f 6361  oorlabs-CAPED/ca
-000003c0: 7065 642d 6169 2d74 6162 756c 6f75 722f  ped-ai-tabulour/
-000003d0: 6973 7375 6573 0d0a 0944 6f63 756d 656e  issues...Documen
-000003e0: 7461 7469 6f6e 203d 2068 7474 7073 3a2f  tation = https:/
-000003f0: 2f67 6974 6875 622e 636f 6d2f 4b61 706f  /github.com/Kapo
-00000400: 6f72 6c61 6273 2d43 4150 4544 2f63 6170  orlabs-CAPED/cap
-00000410: 6564 2d61 692d 7461 6275 6c6f 7572 2352  ed-ai-tabulour#R
-00000420: 4541 444d 452e 6d64 0d0a 0953 6f75 7263  EADME.md...Sourc
-00000430: 6520 436f 6465 203d 2068 7474 7073 3a2f  e Code = https:/
-00000440: 2f67 6974 6875 622e 636f 6d2f 4b61 706f  /github.com/Kapo
-00000450: 6f72 6c61 6273 2d43 4150 4544 2f63 6170  orlabs-CAPED/cap
-00000460: 6564 2d61 692d 7461 6275 6c6f 7572 0d0a  ed-ai-tabulour..
-00000470: 0955 7365 7220 5375 7070 6f72 7420 3d20  .User Support = 
-00000480: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000490: 6f6d 2f4b 6170 6f6f 726c 6162 732d 4341  om/Kapoorlabs-CA
-000004a0: 5045 442f 6361 7065 642d 6169 2d74 6162  PED/caped-ai-tab
-000004b0: 756c 6f75 722f 6973 7375 6573 0d0a 0d0a  ulour/issues....
-000004c0: 5b6f 7074 696f 6e73 5d0d 0a70 6163 6b61  [options]..packa
-000004d0: 6765 7320 3d20 6669 6e64 3a0d 0a69 6e73  ges = find:..ins
-000004e0: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
-000004f0: 0d0a 096e 6170 6172 690d 0a09 7061 6e64  ...napari...pand
-00000500: 6173 0d0a 096e 756d 7079 0d0a 7079 7468  as...numpy..pyth
-00000510: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-00000520: 332e 380d 0a69 6e63 6c75 6465 5f70 6163  3.8..include_pac
-00000530: 6b61 6765 5f64 6174 6120 3d20 5472 7565  kage_data = True
-00000540: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
-00000550: 0d0a 093d 7372 630d 0a73 6574 7570 5f72  ...=src..setup_r
-00000560: 6571 7569 7265 7320 3d20 7365 7475 7074  equires = setupt
-00000570: 6f6f 6c73 5f73 636d 0d0a 0d0a 5b6f 7074  ools_scm....[opt
-00000580: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
-00000590: 6e64 5d0d 0a77 6865 7265 203d 2073 7263  nd]..where = src
-000005a0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 6e74  ....[options.ent
-000005b0: 7279 5f70 6f69 6e74 735d 0d0a 6361 7065  ry_points]..cape
-000005c0: 642e 6d61 6e69 6665 7374 203d 200d 0a09  d.manifest = ...
-000005d0: 6361 7065 642d 6169 2d74 6162 756c 6f75  caped-ai-tabulou
-000005e0: 7220 3d20 6361 7065 645f 6169 5f74 6162  r = caped_ai_tab
-000005f0: 756c 6f75 723a 6361 7065 642e 7961 6d6c  ulour:caped.yaml
-00000600: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 7874  ....[options.ext
-00000610: 7261 735f 7265 7175 6972 655d 0d0a 7465  ras_require]..te
-00000620: 7374 696e 6720 3d20 0d0a 0974 6f78 0d0a  sting = ...tox..
-00000630: 0970 7974 6573 7420 2023 2068 7474 7073  .pytest  # https
-00000640: 3a2f 2f64 6f63 732e 7079 7465 7374 2e6f  ://docs.pytest.o
-00000650: 7267 2f65 6e2f 6c61 7465 7374 2f63 6f6e  rg/en/latest/con
-00000660: 7465 6e74 732e 6874 6d6c 0d0a 0970 7974  tents.html...pyt
-00000670: 6573 742d 636f 7620 2023 2068 7474 7073  est-cov  # https
-00000680: 3a2f 2f70 7974 6573 742d 636f 762e 7265  ://pytest-cov.re
-00000690: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-000006a0: 6c61 7465 7374 2f0d 0a0d 0a5b 6f70 7469  latest/....[opti
-000006b0: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
-000006c0: 5d0d 0a2a 203d 202a 2e79 616d 6c0d 0a0d  ]..* = *.yaml...
-000006d0: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-000006e0: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-000006f0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6361 7065 642d 6169 2d74 6162 756c  = caped-ai-tabul
+00000020: 6f75 720a 7665 7273 696f 6e20 3d20 6174  our.version = at
+00000030: 7472 3a20 6361 7065 645f 6169 5f74 6162  tr: caped_ai_tab
+00000040: 756c 6f75 722e 5f76 6572 7369 6f6e 2e5f  ulour._version._
+00000050: 5f76 6572 7369 6f6e 5f5f 0a64 6573 6372  _version__.descr
+00000060: 6970 7469 6f6e 203d 2041 2062 6173 6520  iption = A base 
+00000070: 7461 626c 6520 7769 6467 6574 2066 6f72  table widget for
+00000080: 204b 6170 6f6f 724c 6162 7320 4e61 7061   KapoorLabs Napa
+00000090: 7269 2070 6c75 6769 6e73 0a6c 6f6e 675f  ri plugins.long_
+000000a0: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
+000000b0: 6c65 3a20 5245 4144 4d45 2e6d 640a 6c6f  le: README.md.lo
+000000c0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
+000000d0: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
+000000e0: 7874 2f6d 6172 6b64 6f77 6e0a 7572 6c20  xt/markdown.url 
+000000f0: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+00000100: 2e63 6f6d 2f4b 6170 6f6f 726c 6162 732d  .com/Kapoorlabs-
+00000110: 4341 5045 442f 6361 7065 642d 6169 2d74  CAPED/caped-ai-t
+00000120: 6162 756c 6f75 720a 6175 7468 6f72 203d  abulour.author =
+00000130: 2056 6172 756e 204b 6170 6f6f 720a 6175   Varun Kapoor.au
+00000140: 7468 6f72 5f65 6d61 696c 203d 2072 616e  thor_email = ran
+00000150: 646f 6d61 6363 6573 7369 626c 656b 6170  domaccessiblekap
+00000160: 6f6f 7240 676d 6169 6c2e 636f 6d0a 6c69  oor@gmail.com.li
+00000170: 6365 6e73 6520 3d20 4253 442d 332d 436c  cense = BSD-3-Cl
+00000180: 6175 7365 0a6c 6963 656e 7365 5f66 696c  ause.license_fil
+00000190: 6573 203d 204c 4943 454e 5345 0a63 6c61  es = LICENSE.cla
+000001a0: 7373 6966 6965 7273 203d 200a 0944 6576  ssifiers = ..Dev
+000001b0: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
+000001c0: 3a3a 2035 202d 2050 726f 6475 6374 696f  :: 5 - Productio
+000001d0: 6e2f 5374 6162 6c65 0a09 496e 7465 6e64  n/Stable..Intend
+000001e0: 6564 2041 7564 6965 6e63 6520 3a3a 2044  ed Audience :: D
+000001f0: 6576 656c 6f70 6572 730a 094c 6963 656e  evelopers..Licen
+00000200: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+00000210: 6564 203a 3a20 4253 4420 4c69 6365 6e73  ed :: BSD Licens
+00000220: 650a 094f 7065 7261 7469 6e67 2053 7973  e..Operating Sys
+00000230: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+00000240: 6e64 656e 740a 0950 726f 6772 616d 6d69  ndent..Programmi
+00000250: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000260: 7974 686f 6e0a 0950 726f 6772 616d 6d69  ython..Programmi
+00000270: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000280: 7974 686f 6e20 3a3a 2033 0a09 5072 6f67  ython :: 3..Prog
+00000290: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000002a0: 203a 3a20 5079 7468 6f6e 203a 3a20 3320   :: Python :: 3 
+000002b0: 3a3a 204f 6e6c 790a 0950 726f 6772 616d  :: Only..Program
+000002c0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000002d0: 2050 7974 686f 6e20 3a3a 2033 2e38 0a09   Python :: 3.8..
+000002e0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000002f0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000300: 3a20 332e 390a 0950 726f 6772 616d 6d69  : 3.9..Programmi
+00000310: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000320: 7974 686f 6e20 3a3a 2033 2e31 300a 0954  ython :: 3.10..T
+00000330: 6f70 6963 203a 3a20 5363 6965 6e74 6966  opic :: Scientif
+00000340: 6963 2f45 6e67 696e 6565 7269 6e67 203a  ic/Engineering :
+00000350: 3a20 496d 6167 6520 5072 6f63 6573 7369  : Image Processi
+00000360: 6e67 0a70 726f 6a65 6374 5f75 726c 7320  ng.project_urls 
+00000370: 3d20 0a09 4275 6720 5472 6163 6b65 7220  = ..Bug Tracker 
+00000380: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+00000390: 2e63 6f6d 2f4b 6170 6f6f 726c 6162 732d  .com/Kapoorlabs-
+000003a0: 4341 5045 442f 6361 7065 642d 6169 2d74  CAPED/caped-ai-t
+000003b0: 6162 756c 6f75 722f 6973 7375 6573 0a09  abulour/issues..
+000003c0: 446f 6375 6d65 6e74 6174 696f 6e20 3d20  Documentation = 
+000003d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000003e0: 6f6d 2f4b 6170 6f6f 726c 6162 732d 4341  om/Kapoorlabs-CA
+000003f0: 5045 442f 6361 7065 642d 6169 2d74 6162  PED/caped-ai-tab
+00000400: 756c 6f75 7223 5245 4144 4d45 2e6d 640a  ulour#README.md.
+00000410: 0953 6f75 7263 6520 436f 6465 203d 2068  .Source Code = h
+00000420: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000430: 6d2f 4b61 706f 6f72 6c61 6273 2d43 4150  m/Kapoorlabs-CAP
+00000440: 4544 2f63 6170 6564 2d61 692d 7461 6275  ED/caped-ai-tabu
+00000450: 6c6f 7572 0a09 5573 6572 2053 7570 706f  lour..User Suppo
+00000460: 7274 203d 2068 7474 7073 3a2f 2f67 6974  rt = https://git
+00000470: 6875 622e 636f 6d2f 4b61 706f 6f72 6c61  hub.com/Kapoorla
+00000480: 6273 2d43 4150 4544 2f63 6170 6564 2d61  bs-CAPED/caped-a
+00000490: 692d 7461 6275 6c6f 7572 2f69 7373 7565  i-tabulour/issue
+000004a0: 730a 0a5b 6f70 7469 6f6e 735d 0a70 6163  s..[options].pac
+000004b0: 6b61 6765 7320 3d20 6669 6e64 3a0a 696e  kages = find:.in
+000004c0: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
+000004d0: 200a 096e 6170 6172 690a 0970 616e 6461   ..napari..panda
+000004e0: 730a 096e 756d 7079 0a70 7974 686f 6e5f  s..numpy.python_
+000004f0: 7265 7175 6972 6573 203d 203e 3d33 2e38  requires = >=3.8
+00000500: 0a69 6e63 6c75 6465 5f70 6163 6b61 6765  .include_package
+00000510: 5f64 6174 6120 3d20 5472 7565 0a70 6163  _data = True.pac
+00000520: 6b61 6765 5f64 6972 203d 200a 093d 7372  kage_dir = ..=sr
+00000530: 630a 7365 7475 705f 7265 7175 6972 6573  c.setup_requires
+00000540: 203d 2073 6574 7570 746f 6f6c 735f 7363   = setuptools_sc
+00000550: 6d0a 0a5b 6f70 7469 6f6e 732e 7061 636b  m..[options.pack
+00000560: 6167 6573 2e66 696e 645d 0a77 6865 7265  ages.find].where
+00000570: 203d 2073 7263 0a0a 5b6f 7074 696f 6e73   = src..[options
+00000580: 2e65 6e74 7279 5f70 6f69 6e74 735d 0a63  .entry_points].c
+00000590: 6170 6564 2e6d 616e 6966 6573 7420 3d20  aped.manifest = 
+000005a0: 0a09 6361 7065 642d 6169 2d74 6162 756c  ..caped-ai-tabul
+000005b0: 6f75 7220 3d20 6361 7065 645f 6169 5f74  our = caped_ai_t
+000005c0: 6162 756c 6f75 723a 6361 7065 642e 7961  abulour:caped.ya
+000005d0: 6d6c 0a0a 5b6f 7074 696f 6e73 2e65 7874  ml..[options.ext
+000005e0: 7261 735f 7265 7175 6972 655d 0a74 6573  ras_require].tes
+000005f0: 7469 6e67 203d 200a 0974 6f78 0a09 7079  ting = ..tox..py
+00000600: 7465 7374 2020 2320 6874 7470 733a 2f2f  test  # https://
+00000610: 646f 6373 2e70 7974 6573 742e 6f72 672f  docs.pytest.org/
+00000620: 656e 2f6c 6174 6573 742f 636f 6e74 656e  en/latest/conten
+00000630: 7473 2e68 746d 6c0a 0970 7974 6573 742d  ts.html..pytest-
+00000640: 636f 7620 2023 2068 7474 7073 3a2f 2f70  cov  # https://p
+00000650: 7974 6573 742d 636f 762e 7265 6164 7468  ytest-cov.readth
+00000660: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+00000670: 7374 2f0a 0a5b 6f70 7469 6f6e 732e 7061  st/..[options.pa
+00000680: 636b 6167 655f 6461 7461 5d0a 2a20 3d20  ckage_data].* = 
+00000690: 2a2e 7961 6d6c 0a0a 5b65 6767 5f69 6e66  *.yaml..[egg_inf
+000006a0: 6f5d 0a74 6167 5f62 7569 6c64 203d 200a  o].tag_build = .
+000006b0: 7461 675f 6461 7465 203d 2030 0a0a       tag_date = 0..
```

### Comparing `caped-ai-tabulour-0.1.2/src/caped_ai_tabulour/_data_model.py` & `caped_ai_tabulour-0.1.3/src/caped_ai_tabulour/_data_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,26 @@
-import math
-
-import numpy as np
-import pandas as pd
 from qtpy import QtCore, QtGui
+import pandas as pd
+import numpy as np
+import math
 
 
 class pandasModel(QtCore.QAbstractTableModel):
-
-    # signalMyDataChanged = QtCore.pyqtSignal(object, object, object)
     signalMyDataChanged = QtCore.Signal(object, object, object)
-    """Emit on user editing a cell."""
 
     def __init__(self, data: pd.DataFrame):
-        """Data model for a pandas dataframe.
-
-        Args:
-            data (pd.dataframe): pandas dataframe
-        """
         QtCore.QAbstractTableModel.__init__(self)
-
         self._data = data
 
     def get_data(self):
-
         return self._data
 
     def data(self, index, role=QtCore.Qt.DisplayRole):
         if index.isValid():
             if role == QtCore.Qt.ToolTipRole:
-                # no tooltips here
                 return QtGui.QBrush(QtCore.Qt.magenta)
             elif role in [QtCore.Qt.DisplayRole, QtCore.Qt.EditRole]:
                 columnName = self._data.columns[index.column()]
                 realRow = index.row()
                 retVal = self._data.loc[realRow, columnName]
                 if isinstance(retVal, np.float64):
                     retVal = float(retVal)
@@ -40,65 +28,53 @@
                     retVal = int(retVal)
                 elif isinstance(retVal, np.bool_):
                     retVal = str(retVal)
                 elif isinstance(retVal, list):
                     retVal = str(retVal)
                 elif isinstance(retVal, str) and retVal == "nan":
                     retVal = ""
-
                 if isinstance(retVal, float) and math.isnan(retVal):
-                    # don't show 'nan' in table
                     retVal = ""
                 return retVal
-
             elif role == QtCore.Qt.FontRole:
-                # realRow = self._data.index[index.row()]
-                realRow = index.row()
                 columnName = self._data.columns[index.column()]
                 if columnName == "Symbol":
-                    # make symbols larger
-                    return QtCore.QVariant(QtGui.QFont("Arial", pointSize=16))
-                return QtCore.QVariant()
-
+                    font = QtGui.QFont("Arial")
+                    font.setPointSize(16)
+                    return font
             elif role == QtCore.Qt.ForegroundRole:
-
-                return QtCore.QVariant()
-
+                return None  # No specific foreground role
             elif role == QtCore.Qt.BackgroundRole:
                 columnName = self._data.columns[index.column()]
                 if columnName == "Face Color":
                     realRow = self._data.index[index.row()]
-                    face_color = self._data.loc[realRow, "Face Color"]  # rgba
-                    face_color = (
-                        face_color[0] + face_color[7:9] + face_color[1:7]
-                    )
-                    theColor = QtCore.QVariant(QtGui.QColor(face_color))
-                    return theColor
+                    face_color = self._data.loc[realRow, "Face Color"]
+                    face_color = face_color[0] + face_color[7:9] + face_color[1:7]
+                    return QtGui.QColor(face_color)
                 elif index.row() % 2 == 0:
-                    return QtCore.QVariant(QtGui.QColor("#444444"))
+                    return QtGui.QColor("#444444")
                 else:
-                    return QtCore.QVariant(QtGui.QColor("#666666"))
-        #
-        return QtCore.QVariant()
+                    return QtGui.QColor("#666666")
+        return None
 
     def headerData(self, col, orientation, role):
         if role == QtCore.Qt.DisplayRole:
             if orientation == QtCore.Qt.Horizontal:
                 try:
                     return self._data.columns[col]
-                except (IndexError):
+                except IndexError:
                     print(
                         f"IndexError for col:{col} len:{len(self._data.columns)}, shape:{self._data.shape}"
                     )
-                    # raise
-            elif orientation == QtCore.Qt.Vertical:
-                # this is to show pandas 'index' column
-                return col
-        return QtCore.QVariant()
+        elif orientation == QtCore.Qt.Vertical:
+            return col
+        return None
 
     def rowCount(self, parent=None):
         if self._data is not None:
             return self._data.shape[0]
+        return 0
 
-    def columnCount(self, parnet=None):
+    def columnCount(self, parent=None):
         if self._data is not None:
             return self._data.shape[1]
+        return 0
```

### Comparing `caped-ai-tabulour-0.1.2/src/caped_ai_tabulour/_tabulour.py` & `caped_ai_tabulour-0.1.3/src/caped_ai_tabulour/_tabulour.py`

 * *Files identical despite different names*

### Comparing `caped-ai-tabulour-0.1.2/src/caped_ai_tabulour/_tests/test_tabulour.py` & `caped_ai_tabulour-0.1.3/src/caped_ai_tabulour/_tests/test_tabulour.py`

 * *Files identical despite different names*

### Comparing `caped-ai-tabulour-0.1.2/src/caped_ai_tabulour.egg-info/PKG-INFO` & `caped_ai_tabulour-0.1.3/src/caped_ai_tabulour.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-Metadata-Version: 2.1
-Name: caped-ai-tabulour
-Version: 0.1.2
-Summary: A base table widget for KapoorLabs Napari plugins
-Home-page: https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour
-Author: Varun Kapoor
-Author-email: randomaccessiblekapoor@gmail.com
-License: BSD-3-Clause
-Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/issues
-Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour#README.md
-Project-URL: Source Code, https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour
-Project-URL: User Support, https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/issues
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: napari
-Requires-Dist: pandas
-Requires-Dist: numpy
-Provides-Extra: testing
-Requires-Dist: tox; extra == "testing"
-Requires-Dist: pytest; extra == "testing"
-Requires-Dist: pytest-cov; extra == "testing"
-
-# caped-ai-tabulour
-
-[![License BSD-3](https://img.shields.io/pypi/l/caped-ai-tabulour.svg?color=green)](https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/raw/main/LICENSE)
-[![PyPI](https://img.shields.io/pypi/v/caped-ai-tabulour.svg?color=green)](https://pypi.org/project/caped-ai-tabulour)
-[![Python Version](https://img.shields.io/pypi/pyversions/caped-ai-tabulour.svg?color=green)](https://python.org)
-[![tests](https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/workflows/tests/badge.svg)](https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/actions)
-[![codecov](https://codecov.io/gh/Kapoorlabs-CAPED/caped-ai-tabulour/branch/main/graph/badge.svg)](https://codecov.io/gh/Kapoorlabs-CAPED/caped-ai-tabulour)
-
-
-A base table widget for KapoorLabs Napari plugins
-
-----------------------------------
-
-This [caped] package was generated with [Cookiecutter] using [@caped]'s [cookiecutter-template] template.
-
-
-
-## Installation
-
-You can install `caped-ai-tabulour` via [pip]:
-
-    pip install caped-ai-tabulour
-
-
-
-To install latest development version :
-
-    pip install git+https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour.git
-
-
-## Contributing
-
-Contributions are very welcome. Tests can be run with [tox], please ensure
-the coverage at least stays the same before you submit a pull request.
-
-## License
-
-Distributed under the terms of the [BSD-3] license,
-"caped-ai-tabulour" is free and open source software
-
-## Issues
-
-If you encounter any problems, please [file an issue] along with a detailed description.
-
-
-[pip]: https://pypi.org/project/pip/
-[caped]: https://github.com/Kapoorlabs-CAPED
-[Cookiecutter]: https://github.com/audreyr/cookiecutter
-[@caped]: https://github.com/Kapoorlabs-CAPED
-[MIT]: http://opensource.org/licenses/MIT
-[BSD-3]: http://opensource.org/licenses/BSD-3-Clause
-[GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
-[GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
-[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
-[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
-[cookiecutter-template]: https://github.com/Kapoorlabs-CAPED/cookiecutter-template
-
-[file an issue]: https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/issues
-
-[caped]: https://github.com/Kapoorlabs-CAPED/
-[tox]: https://tox.readthedocs.io/en/latest/
-[pip]: https://pypi.org/project/pip/
-[PyPI]: https://pypi.org/
+Metadata-Version: 2.1
+Name: caped-ai-tabulour
+Version: 0.1.3
+Summary: A base table widget for KapoorLabs Napari plugins
+Home-page: https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour
+Author: Varun Kapoor
+Author-email: randomaccessiblekapoor@gmail.com
+License: BSD-3-Clause
+Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/issues
+Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour#README.md
+Project-URL: Source Code, https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour
+Project-URL: User Support, https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/issues
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: napari
+Requires-Dist: pandas
+Requires-Dist: numpy
+Provides-Extra: testing
+Requires-Dist: tox; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+
+# caped-ai-tabulour
+
+[![License BSD-3](https://img.shields.io/pypi/l/caped-ai-tabulour.svg?color=green)](https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/raw/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/caped-ai-tabulour.svg?color=green)](https://pypi.org/project/caped-ai-tabulour)
+[![Python Version](https://img.shields.io/pypi/pyversions/caped-ai-tabulour.svg?color=green)](https://python.org)
+[![tests](https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/workflows/tests/badge.svg)](https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/actions)
+[![codecov](https://codecov.io/gh/Kapoorlabs-CAPED/caped-ai-tabulour/branch/main/graph/badge.svg)](https://codecov.io/gh/Kapoorlabs-CAPED/caped-ai-tabulour)
+
+
+A base table widget for KapoorLabs Napari plugins
+
+----------------------------------
+
+This [caped] package was generated with [Cookiecutter] using [@caped]'s [cookiecutter-template] template.
+
+
+
+## Installation
+
+You can install `caped-ai-tabulour` via [pip]:
+
+    pip install caped-ai-tabulour
+
+
+
+To install latest development version :
+
+    pip install git+https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour.git
+
+
+## Contributing
+
+Contributions are very welcome. Tests can be run with [tox], please ensure
+the coverage at least stays the same before you submit a pull request.
+
+## License
+
+Distributed under the terms of the [BSD-3] license,
+"caped-ai-tabulour" is free and open source software
+
+## Issues
+
+If you encounter any problems, please [file an issue] along with a detailed description.
+
+
+[pip]: https://pypi.org/project/pip/
+[caped]: https://github.com/Kapoorlabs-CAPED
+[Cookiecutter]: https://github.com/audreyr/cookiecutter
+[@caped]: https://github.com/Kapoorlabs-CAPED
+[MIT]: http://opensource.org/licenses/MIT
+[BSD-3]: http://opensource.org/licenses/BSD-3-Clause
+[GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
+[GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
+[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
+[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
+[cookiecutter-template]: https://github.com/Kapoorlabs-CAPED/cookiecutter-template
+
+[file an issue]: https://github.com/Kapoorlabs-CAPED/caped-ai-tabulour/issues
+
+[caped]: https://github.com/Kapoorlabs-CAPED/
+[tox]: https://tox.readthedocs.io/en/latest/
+[pip]: https://pypi.org/project/pip/
+[PyPI]: https://pypi.org/
```

### Comparing `caped-ai-tabulour-0.1.2/src/caped_ai_tabulour.egg-info/SOURCES.txt` & `caped_ai_tabulour-0.1.3/src/caped_ai_tabulour.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caped-ai-tabulour-0.1.2/tox.ini` & `caped_ai_tabulour-0.1.3/tox.ini`

 * *Files identical despite different names*

### Comparing `caped-ai-tabulour-0.1.2/update_version.py` & `caped_ai_tabulour-0.1.3/update_version.py`

 * *Files identical despite different names*

