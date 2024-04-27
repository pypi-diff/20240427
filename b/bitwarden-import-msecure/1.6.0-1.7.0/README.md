# Comparing `tmp/bitwarden_import_msecure-1.6.0.tar.gz` & `tmp/bitwarden_import_msecure-1.7.0.tar.gz`

## Comparing `bitwarden_import_msecure-1.6.0.tar` & `bitwarden_import_msecure-1.7.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/.coveragerc
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/.flake8
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/.mypy.ini
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/.pylintrc
--rwxr-xr-x   0        0        0     1340 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/activate.sh
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/invoke.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/pytest.ini
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/requirements.dev.in
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/requirements.dev.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/requirements.in
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/requirements.txt
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/tasks.py
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/.github/workflows/pip_publish.yml
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/.github/workflows/static.yml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/docs/mkdocs.yml
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/docs/src/en/index.md
--rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/docs/src/ru/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/scripts/__init__.py
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/scripts/build-docs.sh
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/scripts/build.sh
--rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/scripts/docs-render-config.sh
--rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/scripts/include_pyproject_requirements.py
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/scripts/upload.sh
--rwxr-xr-x   0        0        0     2525 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/scripts/verup.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/src/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/src/bitwarden_import_msecure/__about__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/src/bitwarden_import_msecure/__init__.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/src/bitwarden_import_msecure/bitwarden_csv.py
--rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/src/bitwarden_import_msecure/bitwarden_json.py
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/src/bitwarden_import_msecure/main.py
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/src/bitwarden_import_msecure/msecure.py
--rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/src/bitwarden_import_msecure/patch_export.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/tests/conftest.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/tests/test_bitwarden_import_msecure.py
--rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/tests/test_e2e.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/tests/resources/bitwarden_export.csv
--rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/tests/resources/bitwarden_export.json
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/tests/resources/bitwarden_notes_export.csv
--rw-r--r--   0        0        0     5060 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/tests/resources/bitwarden_notes_export.json
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/tests/resources/mSecure Export File.csv
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/LICENSE.txt
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/README.md
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/.coveragerc
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/.flake8
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/.mypy.ini
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/.pylintrc
+-rwxr-xr-x   0        0        0     1340 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/activate.sh
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/invoke.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/pytest.ini
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/requirements.dev.in
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/requirements.dev.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/requirements.in
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/requirements.txt
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/tasks.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/.github/workflows/pip_publish.yml
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/.github/workflows/static.yml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/docs/mkdocs.yml
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/docs/src/en/index.md
+-rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/docs/src/ru/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/scripts/__init__.py
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/scripts/build.sh
+-rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/scripts/docs-render-config.sh
+-rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/scripts/include_pyproject_requirements.py
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/scripts/upload.sh
+-rwxr-xr-x   0        0        0     2525 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/scripts/verup.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/src/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/__about__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/__init__.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/bitwarden_csv.py
+-rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/bitwarden_json.py
+-rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/main.py
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/msecure.py
+-rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/msecure_to_bitwarden.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/tests/conftest.py
+-rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/tests/test_bitwarden_import_msecure.py
+-rw-r--r--   0        0        0     5666 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/tests/test_e2e.py
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/tests/resources/bitwarden_broken_export.json
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/tests/resources/bitwarden_export.csv
+-rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/tests/resources/bitwarden_export.json
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/tests/resources/bitwarden_notes_export.csv
+-rw-r--r--   0        0        0     5060 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/tests/resources/bitwarden_notes_export.json
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/tests/resources/bitwarden_patched_export.json
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/tests/resources/mSecure Export File.csv
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/README.md
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.7.0/PKG-INFO
```

### Comparing `bitwarden_import_msecure-1.6.0/.pre-commit-config.yaml` & `bitwarden_import_msecure-1.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.6.0/activate.sh` & `bitwarden_import_msecure-1.7.0/activate.sh`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.6.0/requirements.dev.txt` & `bitwarden_import_msecure-1.7.0/requirements.dev.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,161 +1,164 @@
 # This file was autogenerated by uv via the following command:
 #    uv pip compile requirements.dev.in --output-file=requirements.dev.txt
 -e .
 allure-pytest==2.13.5
 allure-python-commons==2.13.5
     # via allure-pytest
-astroid==3.0.2
+astroid==3.1.0
     # via pylint
 attrs==23.2.0
     # via allure-python-commons
 babel==2.14.0
     # via mkdocs-material
 bracex==2.4
     # via wcmatch
-certifi==2023.11.17
+certifi==2024.2.2
     # via requests
 cfgv==3.4.0
     # via pre-commit
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   bitwarden-import-msecure
     #   mkdocs
     #   rich-click
 colorama==0.4.6
     # via mkdocs-material
-coverage==7.3.2
+coverage==7.5.0
     # via pytest-cov
-dill==0.3.7
+dill==0.3.8
     # via pylint
 distlib==0.3.8
     # via virtualenv
-editables==0.5
-    # via hatchling
-filelock==3.13.1
+filelock==3.13.4
     # via virtualenv
 ghp-import==2.1.0
     # via mkdocs
-hatchling==1.20.0
-identify==2.5.33
+hatchling==1.24.2
+identify==2.5.36
     # via pre-commit
-idna==3.6
+idna==3.7
     # via requests
 iniconfig==2.0.0
     # via pytest
 invoke==2.2.0
 isort==5.13.2
     # via pylint
-jinja2==3.1.2
+jinja2==3.1.3
     # via
     #   mkdocs
     #   mkdocs-material
-markdown==3.5.1
+markdown==3.6
     # via
     #   mkdocs
     #   mkdocs-material
     #   pymdown-extensions
 markdown-it-py==3.0.0
     # via rich
-markupsafe==2.1.3
+markupsafe==2.1.5
     # via
     #   jinja2
     #   mkdocs
 mccabe==0.7.0
     # via pylint
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
-    # via mkdocs
-mkdocs==1.5.3
+    # via
+    #   mkdocs
+    #   mkdocs-get-deps
+mkdocs==1.6.0
     # via
     #   mkdocs-awesome-pages-plugin
     #   mkdocs-material
 mkdocs-awesome-pages-plugin==2.9.2
-mkdocs-material==9.5.2
+mkdocs-get-deps==0.2.0
+    # via mkdocs
+mkdocs-material==9.5.19
 mkdocs-material-extensions==1.3.1
     # via mkdocs-material
-mypy==1.7.1
+mypy==1.10.0
 mypy-extensions==1.0.0
     # via mypy
 natsort==8.4.0
     # via mkdocs-awesome-pages-plugin
 nodeenv==1.8.0
     # via pre-commit
-packaging==23.2
+packaging==24.0
     # via
     #   hatchling
     #   mkdocs
     #   pytest
 paginate==0.5.6
     # via mkdocs-material
 pathspec==0.12.1
     # via
     #   hatchling
     #   mkdocs
-platformdirs==4.1.0
+platformdirs==4.2.1
     # via
-    #   mkdocs
+    #   mkdocs-get-deps
     #   pylint
     #   virtualenv
-pluggy==1.3.0
+pluggy==1.5.0
     # via
     #   allure-python-commons
     #   hatchling
     #   pytest
-pre-commit==3.6.0
+pre-commit==3.7.0
 pydocstyle==6.3.0
 pygments==2.17.2
     # via
     #   mkdocs-material
     #   rich
-pylint==3.0.3
-pymdown-extensions==10.5
+pylint==3.1.0
+pymdown-extensions==10.8
     # via mkdocs-material
-pytest==7.4.3
+pytest==8.1.1
     # via
     #   allure-pytest
     #   pytest-cov
-pytest-cov==4.1.0
-python-dateutil==2.8.2
+pytest-cov==5.0.0
+python-dateutil==2.9.0.post0
     # via ghp-import
 pyyaml==6.0.1
     # via
     #   mkdocs
+    #   mkdocs-get-deps
     #   pre-commit
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
-regex==2023.10.3
+regex==2024.4.16
     # via mkdocs-material
 requests==2.31.0
     # via mkdocs-material
 rich==13.7.1
     # via rich-click
 rich-click==1.7.4
     # via bitwarden-import-msecure
-setuptools==69.2.0
+setuptools==69.5.1
     # via nodeenv
 six==1.16.0
     # via python-dateutil
 snowballstemmer==2.2.0
     # via pydocstyle
 toml==0.10.2
-tomlkit==0.12.3
+tomlkit==0.12.4
     # via pylint
-trove-classifiers==2023.11.29
+trove-classifiers==2024.4.10
     # via hatchling
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   mypy
     #   rich-click
-urllib3==2.1.0
+urllib3==2.2.1
     # via requests
-virtualenv==20.25.0
+virtualenv==20.26.0
     # via pre-commit
-watchdog==3.0.0
+watchdog==4.0.0
     # via mkdocs
-wcmatch==8.5
+wcmatch==8.5.1
     # via mkdocs-awesome-pages-plugin
```

### Comparing `bitwarden_import_msecure-1.6.0/tasks.py` & `bitwarden_import_msecure-1.7.0/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,17 +40,17 @@
     return ver
 
 
 @task
 def compile_requirements(c: Context):
     "Convert requirements.in to requirements.txt and requirements.dev.txt."
     start_time = subprocess.check_output(["date", "+%s"]).decode().strip()
-    c.run("uv pip compile requirements.in --output-file=requirements.txt")
+    c.run("uv pip compile requirements.in --output-file=requirements.txt --upgrade")
     reqs_time = subprocess.check_output(["date", "+%s"]).decode().strip()
-    c.run("uv pip compile requirements.dev.in --output-file=requirements.dev.txt")
+    c.run("uv pip compile requirements.dev.in --output-file=requirements.dev.txt --upgrade")
     end_time = subprocess.check_output(["date", "+%s"]).decode().strip()
     print(f"Req's compilation time: {int(reqs_time) - int(start_time)} seconds")
     print(f"Req's dev compilation time: {int(end_time) - int(reqs_time)} seconds")
     print(f"Total execution time: {int(end_time) - int(start_time)} seconds")
 
     c.run("scripts/include_pyproject_requirements.py requirements.in")
```

### Comparing `bitwarden_import_msecure-1.6.0/.github/workflows/ci.yml` & `bitwarden_import_msecure-1.7.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.6.0/.github/workflows/docs.yml` & `bitwarden_import_msecure-1.7.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.6.0/.github/workflows/pip_publish.yml` & `bitwarden_import_msecure-1.7.0/.github/workflows/pip_publish.yml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.6.0/.github/workflows/static.yml` & `bitwarden_import_msecure-1.7.0/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.6.0/docs/mkdocs.yml` & `bitwarden_import_msecure-1.7.0/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.6.0/docs/src/en/index.md` & `bitwarden_import_msecure-1.7.0/docs/src/en/index.md`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.6.0/docs/src/ru/index.md` & `bitwarden_import_msecure-1.7.0/docs/src/ru/index.md`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.6.0/scripts/include_pyproject_requirements.py` & `bitwarden_import_msecure-1.7.0/scripts/include_pyproject_requirements.py`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.6.0/scripts/verup.sh` & `bitwarden_import_msecure-1.7.0/scripts/verup.sh`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.6.0/src/bitwarden_import_msecure/bitwarden_csv.py` & `bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/bitwarden_csv.py`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.6.0/src/bitwarden_import_msecure/bitwarden_json.py` & `bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/bitwarden_json.py`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.6.0/src/bitwarden_import_msecure/main.py` & `bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 """Bitwarden Import mSecure Export."""
 
-import csv
 from pathlib import Path
 
 import rich_click as click
+from rich.console import Console
 
-from bitwarden_import_msecure.bitwarden_csv import BitwardenCsv
-from bitwarden_import_msecure.bitwarden_json import BitwardenJson
-from bitwarden_import_msecure.msecure import import_msecure_row
 from bitwarden_import_msecure.__about__ import __version__
-from bitwarden_import_msecure import patch_export
+from bitwarden_import_msecure import msecure_to_bitwarden
 
 click.rich_click.USE_MARKDOWN = True
 
 
 OUTPUT_FILE_DEFAULT = "bitwarden"
 NOTES_MODE = "notes"
 
 
+def error(message: str, abort: bool = True) -> None:
+    """Print error message and exit."""
+    console = Console()
+    console.print(message, style="bold red")
+    if abort:
+        raise click.Abort()
+
+
 @click.command()
 @click.version_option(version=__version__, prog_name="bitwarden-import-msecure")
 @click.argument("input_file", type=click.Path(exists=True), required=False)
 @click.argument("output_file", type=click.Path(), required=False)
 @click.option("--force", is_flag=True, help="Overwrite the output file if it exists.")
 @click.option(
     "--patch", is_flag=True, help="Fix old exports, see `--patch-help` for more details."
@@ -57,53 +62,50 @@
     to `OUTPUT_FILE`.
 
     - Export CSV from mSecure
     - Run this script on the exported CSV file
     - Import the processed file into Bitwarden
     """
     if patch_help:
-        patch_export.show_help()
+        msecure_to_bitwarden.patch_help()
         return
 
+    if not input_file:
+        error("No input file provided.")
     input_path = Path(input_file)
     if not input_path.exists():
-        click.echo(f"Input file `{input_path}` does not exist.")
-        raise click.Abort()
+        error(f"Input file `{input_path}` does not exist.")
 
     if force and patch:
-        click.echo("--force and --patch cannot be used simultaneously.")
-        raise click.Abort()
+        error("--force and --patch cannot be used simultaneously.")
 
     output_path = (
         Path(output_file)
         if output_file
         else input_path.parent / f"{OUTPUT_FILE_DEFAULT}.{output_format}"
     )
 
     if patch:
+        if output_format != "json":
+            error("Patching is only supported for JSON format.", abort=False)
+            msecure_to_bitwarden.patch_help()
+            raise click.Abort()
         if not output_path.exists():
-            click.echo(f"Cannot patch `{output_path}` - does not exists.")
+            error(f"To patch output file `{output_path}` it should exist.", abort=False)
+            msecure_to_bitwarden.patch_help()
             raise click.Abort()
-        patch_export.patch(input_path, output_path)
+        msecure_to_bitwarden.patch(input_path, output_path)
     else:
         if output_path.exists() and not force:
-            click.echo(f"Output file `{output_path}` already exists. Use --force to overwrite.")
-            raise click.Abort()
-
-        if output_format == "csv":
-            writer = BitwardenCsv(output_path)
-        else:
-            writer = BitwardenJson(output_path)
-
-        with input_path.open(newline="", encoding="utf-8") as infile:
-            reader = csv.reader(infile, delimiter=",")
-            for row in reader:
-                if row and not row[0].startswith("mSecure"):
-                    data = import_msecure_row(row, extra_fields == NOTES_MODE)
-                    writer.write_record(data)
+            error(f"Output file `{output_path}` already exists. Use --force to overwrite.")
 
-        writer.close()
+        msecure_to_bitwarden.convert(
+            input_path,
+            output_path,
+            output_format=output_format,
+            extra_fields_to_notes=extra_fields == NOTES_MODE,
+        )
     click.echo(f"File to import into Bitwarden saved to `{output_path}`")
 
 
 if __name__ == "__main__":  # pragma: no cover
     bitwarden_import_msecure()  # pylint: disable=no-value-for-parameter
```

### Comparing `bitwarden_import_msecure-1.6.0/src/bitwarden_import_msecure/msecure.py` & `bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/msecure.py`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.6.0/src/bitwarden_import_msecure/patch_export.py` & `bitwarden_import_msecure-1.7.0/src/bitwarden_import_msecure/msecure_to_bitwarden.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,38 @@
-"""Fix errors in old exports."""
+"""Conversion logic."""
 
+import csv
 import json
 from pathlib import Path
 
 from rich.console import Console
 from rich.panel import Panel
-from rich.syntax import Syntax
+from rich.markdown import Markdown
 from rich.theme import Theme
 
 import rich_click as click
 
+from bitwarden_import_msecure.bitwarden_csv import BitwardenCsv
+from bitwarden_import_msecure.bitwarden_json import BitwardenJson
+from bitwarden_import_msecure.msecure import import_msecure_row
+
 
 def patch(input_path: Path, output_path: Path) -> None:
     """Fix errors in old exports.
 
     Some old versions of `bitwarden-import-msecure` worked incorrectly.
     For example versions before 1.5.0 did not export logins' URLs.
 
     If you migrated to Bitwarden some time ago and cannot just drop all records
     and import them again, use option `--patch`:
 
-    - process mSecure export `mSecure Export File.csv` with new `bitwarden-import-msecure`:
+    - process the mSecure export `mSecure Export File.csv` with the new `bitwarden-import-msecure`:
         `bitwarden-import-msecure "mSecure Export File.csv" bitwarden.json`
-    - export json from Bitwarden, lets name result as `bitwarden_new.json`
-    - patch this export with additional data from mSecure export:
+    - export json from Bitwarden, let's name the result as `bitwarden_new.json`
+    - patch this export with additional data from the mSecure export:
         `bitwarden-import-msecure bitwarden.json bitwarden_new.json --patch`
     - now you have `bitwarden_new.json` with all necessary changes, import it to Bitwarden
     """
     if not output_path.exists():
         click.echo(f"Output file `{output_path}` does not exist.")
         raise click.Abort()
 
@@ -63,37 +68,57 @@
                     item["name"] in uri_dict and not item.get("login", {}).get("uris", [])
                 ):
                     item["login"]["uris"] = uri_dict[item["name"]]
                     replaced += 1
             click.echo(f"Added {replaced} URLs.")
 
             file.seek(0)
-            json.dump(output_data, file, indent=2)
+            json.dump(output_data, file, indent=4)
             file.truncate()
 
     except json.JSONDecodeError as e:
         print(f"Error: {output_path} is not a valid JSON file:\n{e}")
         return
     except FileNotFoundError as e:
         print(f"Error: {output_path} not found:\n{e}")
         return
 
 
-def show_help() -> None:
+def patch_help() -> None:
     """Show help message for `--patch` option."""
     custom_theme = Theme(
         {
             "markdown.heading": "bold magenta",  # Styling for headings
             "markdown.code": "bold",  # Code blocks often stand out
             "markdown.list": "dim",  # Lists are usually less emphasized
             "markdown.block_quote": "italic",  # Block quotes may be italicized
             "markdown.link": "underline blue",  # Links can be underlined and blue
             "markdown.italic": "italic",  # Explicit style for italic text
             "markdown.bold": "bold",  # Explicit style for bold text
         }
     )
     console = Console(theme=custom_theme)
     assert patch.__doc__
-    doc = "\n".join([line.lstrip() for line in patch.__doc__.split("\n")])
-    syntax = Syntax(doc, "markdown", word_wrap=True, background_color="default")
-    panel = Panel(syntax, border_style="gray46")
+    lines = [line.strip() for line in patch.__doc__.strip().split("\n")]
+    title = lines[0]
+    markdown_content = "\n".join(lines[2:])  # Skip title and empty line
+    markdown = Markdown(markdown_content)
+    panel = Panel(markdown, title=title, border_style="gray46")
+
     console.print(panel)
+
+
+def convert(
+    input_path: Path, output_path: Path, *, output_format: str, extra_fields_to_notes: bool
+) -> None:
+    """Convert mSecure export to Bitwarden format."""
+    if output_format == "csv":
+        writer = BitwardenCsv(output_path)
+    else:
+        writer = BitwardenJson(output_path)
+    with input_path.open(newline="", encoding="utf-8") as infile:
+        reader = csv.reader(infile, delimiter=",")
+        for row in reader:
+            if row and not row[0].startswith("mSecure"):
+                data = import_msecure_row(row, extra_fields_to_notes)
+                writer.write_record(data)
+    writer.close()
```

### Comparing `bitwarden_import_msecure-1.6.0/tests/resources/bitwarden_export.csv` & `bitwarden_import_msecure-1.7.0/tests/resources/bitwarden_export.csv`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.6.0/tests/resources/bitwarden_export.json` & `bitwarden_import_msecure-1.7.0/tests/resources/bitwarden_export.json`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.6.0/tests/resources/bitwarden_notes_export.csv` & `bitwarden_import_msecure-1.7.0/tests/resources/bitwarden_notes_export.csv`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.6.0/tests/resources/bitwarden_notes_export.json` & `bitwarden_import_msecure-1.7.0/tests/resources/bitwarden_notes_export.json`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.6.0/tests/resources/mSecure Export File.csv` & `bitwarden_import_msecure-1.7.0/tests/resources/mSecure Export File.csv`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.6.0/LICENSE.txt` & `bitwarden_import_msecure-1.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.6.0/README.md` & `bitwarden_import_msecure-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.6.0/pyproject.toml` & `bitwarden_import_msecure-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.6.0/PKG-INFO` & `bitwarden_import_msecure-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bitwarden-import-msecure
-Version: 1.6.0
+Version: 1.7.0
 Summary: Migration from mSecure to Bitwarden
 Project-URL: Homepage, https://andgineer.github.io/bitwarden-import-msecure/
 Project-URL: Documentation, https://andgineer.github.io/bitwarden-import-msecure/
 Author-email: Andrey Sorokin <andrey@sorokin.engineer>
 License: Copyright (c) 2024 Andrey Sorokin <andrey@sorokin.engineer>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_0nci1hdm_/tmpsd3hbdu7_TarContainer/0/47", line 74, column 102: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: bitwarden-import-msecure Version: 1.6.0 Summary:
+Metadata-Version: 2.3 Name: bitwarden-import-msecure Version: 1.7.0 Summary:
 Migration from mSecure to Bitwarden Project-URL: Homepage, https://
 andgineer.github.io/bitwarden-import-msecure/ Project-URL: Documentation,
 https://andgineer.github.io/bitwarden-import-msecure/ Author-email: Andrey
 Sorokin
 sorokin.engineer> License: Copyright (c) 2024 Andrey Sorokin
 sorokin.engineer> Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

