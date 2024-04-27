# Comparing `tmp/reasoner_validator-4.0.2.tar.gz` & `tmp/reasoner_validator-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-4.0.2.tar", max compression
+gzip compressed data, was "reasoner_validator-4.0.3.tar", max compression
```

## Comparing `reasoner_validator-4.0.2.tar` & `reasoner_validator-4.0.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1153 2024-04-23 02:28:42.039440 reasoner_validator-4.0.2/LICENSE
--rw-r--r--   0        0        0    13645 2024-04-23 02:28:42.039440 reasoner_validator-4.0.2/README.md
--rw-r--r--   0        0        0      131 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/.nojekyll
--rw-r--r--   0        0        0      634 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/Makefile
--rw-r--r--   0        0        0     2291 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/conf.py
--rw-r--r--   0        0        0    20365 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/index.rst
--rw-r--r--   0        0        0      795 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/make.bat
--rw-r--r--   0        0        0      136 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      152 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    39468 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2963 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    85875 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    43025 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0     1761 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/github.py
--rw-r--r--   0        0        0     3973 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/message.py
--rw-r--r--   0        0        0    46755 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4754 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0    14288 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1120 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    14745 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    35564 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/validator.py
--rw-r--r--   0        0        0    11943 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      838 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/versions.yaml
--rw-r--r--   0        0        0     2407 2024-04-23 02:28:42.047441 reasoner_validator-4.0.2/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 02:28:42.047441 reasoner_validator-4.0.2/tests/conftest.py
--rw-r--r--   0        0        0   138310 2024-04-23 02:28:42.047441 reasoner_validator-4.0.2/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62107 2024-04-23 02:28:42.047441 reasoner_validator-4.0.2/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
--rw-r--r--   0        0        0    41247 2024-04-23 02:28:42.047441 reasoner_validator-4.0.2/tests/test_response_validator.py
--rw-r--r--   0        0        0     6157 2024-04-23 02:28:42.047441 reasoner_validator-4.0.2/tests/test_semver.py
--rw-r--r--   0        0        0     2248 2024-04-23 02:28:42.047441 reasoner_validator-4.0.2/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    27195 2024-04-23 02:28:42.047441 reasoner_validator-4.0.2/tests/test_validate.py
--rw-r--r--   0        0        0    30223 2024-04-23 02:28:42.047441 reasoner_validator-4.0.2/tests/test_validation_report.py
--rw-r--r--   0        0        0     2734 2024-04-23 02:28:42.047441 reasoner_validator-4.0.2/tests/test_workflows.py
--rw-r--r--   0        0        0    15948 1970-01-01 00:00:00.000000 reasoner_validator-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1153 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/LICENSE
+-rw-r--r--   0        0        0    13727 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/README.md
+-rw-r--r--   0        0        0      131 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/Makefile
+-rw-r--r--   0        0        0     2291 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/conf.py
+-rw-r--r--   0        0        0    20365 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/index.rst
+-rw-r--r--   0        0        0      795 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/make.bat
+-rw-r--r--   0        0        0      136 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      152 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    39468 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2299 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    85875 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    43025 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0     1761 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/github.py
+-rw-r--r--   0        0        0     3973 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/message.py
+-rw-r--r--   0        0        0    46755 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4754 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0    14288 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1120 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    14745 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    35564 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/validator.py
+-rw-r--r--   0        0        0    11943 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0      838 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/versions.yaml
+-rw-r--r--   0        0        0     2407 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/tests/conftest.py
+-rw-r--r--   0        0        0   138310 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62107 2024-04-27 21:11:06.982750 reasoner_validator-4.0.3/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
+-rw-r--r--   0        0        0    41247 2024-04-27 21:11:06.982750 reasoner_validator-4.0.3/tests/test_response_validator.py
+-rw-r--r--   0        0        0     6157 2024-04-27 21:11:06.982750 reasoner_validator-4.0.3/tests/test_semver.py
+-rw-r--r--   0        0        0     2248 2024-04-27 21:11:06.982750 reasoner_validator-4.0.3/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    27195 2024-04-27 21:11:06.982750 reasoner_validator-4.0.3/tests/test_validate.py
+-rw-r--r--   0        0        0    30223 2024-04-27 21:11:06.982750 reasoner_validator-4.0.3/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2734 2024-04-27 21:11:06.982750 reasoner_validator-4.0.3/tests/test_workflows.py
+-rw-r--r--   0        0        0    15266 1970-01-01 00:00:00.000000 reasoner_validator-4.0.3/PKG-INFO
```

### Comparing `reasoner_validator-4.0.2/LICENSE` & `reasoner_validator-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/README.md` & `reasoner_validator-4.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,36 +21,40 @@
 
 The module may be installed directly from pypi.org using (Python 3) `pip` or `pip3`, namely:
 
 ```bash
 pip install reasoner-validator
 ```
 
-If you want to install it with the extra dependencies for using it as a web service, you can use:
-
-```bash
-pip install "reasoner-validator[web]"
-```
-
 ## Installing and working with the module locally from source
 
 As of release 3.1.6, this project uses the [poetry dependency management](https://python-poetry.org) tool to orchestrate its installation and dependencies.
 
-After [installing poetry](https://python-poetry.org/docs/#installation) and cloning the project, the poetry installation may be run:
+After [installing poetry](https://python-poetry.org/docs/#installation) and cloning the project, the poetry installation may be run (within the available poetry shell):
 
 ```bash
 git clone https://github.com/NCATSTranslator/reasoner-validator.git
 cd reasoner-validator
+poetry use 3.10
+poetry shell
 poetry install
 ```
 
-To develop this package, install with all extras dependencies using:
+Note that the **`poetry env`** can be set to either Python 3.10 or 3.11 at the present time.
+
+This installation also installs testing dependencies (in the poetry 'dev' group in the pyproject.toml) and documentation dependencies (in the corresponding poetry 'docs' group). If you don't want the overhead of these dependencies, then the installation of these poetry group dependencies may be excluded:
+
+```bash
+poetry install --without dev,docs
+```
+
+If you plan to run the web service API,  then install it with the optional web group:
 
 ```bash
-poetry install --all-extras
+poetry install reasoner-validator --with web
 ```
 
 ## Running Validation against an ARS UUID Result(*) or using a Local TRAPI Request Query
 
 A local script **`trapi_validator.py`** is available to run TRAPI Response validation against either a PK (UUID)
 indexed query result of the Biomedical Knowledge Translator "Autonomous Relay System" (ARS), a local JSON Response
 text file or a locally triggered _ad hoc_ query Request against a directly specified TRAPI endpoint.
@@ -63,21 +67,15 @@
 ./trapi_validator.py --help
 ```
 
 (*) Thank you Eric Deutsch for the prototype code for this script
 
 ## Running tests
 
-To run the test locally install with the `dev` dependencies, if not already done (e.g. by **`--all-extras`** above):
-
-```bash
-poetry install --extras dev
-```
-
-Run the tests with coverage report:
+Run the available unit tests with coverage report:
 
 ```bash
 poetry run pytest --cov
 ```
 
 Note that [poetry automatically uses any existing virtual environment](https://python-poetry.org/docs/basic-usage/#using-your-virtual-environment), but you can otherwise also enter the one that is created by poetry by default:
 
@@ -104,23 +102,15 @@
 
 ```bash
 python -m http.server 3000 --directory ./htmlcov
 ```
 
 ## Building the Documentation Locally
 
-All paths here are relative to the root project directory.
-
-First install the documentation-specific dependencies, if not already done (e.g. by **`--all-extras`** above):
-
-```bash
-poetry install --extras docs  # or poetry install --all-extras
-```
-
-The validation codes MarkDown file should first be regenerated if needed (i.e. if it was revised):
+All paths here are relative to the root project directory. The validation codes MarkDown file should first be regenerated if needed (i.e. if the **`codes.yaml`** was revised):
 
 ```bash
 cd reasoner_validator
 python ./validation_codes.py
 ```
 
 Then build the documentation locally:
```

### Comparing `reasoner_validator-4.0.2/docs/Makefile` & `reasoner_validator-4.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/docs/conf.py` & `reasoner_validator-4.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/docs/index.rst` & `reasoner_validator-4.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/docs/make.bat` & `reasoner_validator-4.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/docs/validation_codes_dictionary.md` & `reasoner_validator-4.0.3/docs/validation_codes_dictionary.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/reasoner_validator/biolink/__init__.py` & `reasoner_validator-4.0.3/reasoner_validator/biolink/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/reasoner_validator/codes.yaml` & `reasoner_validator-4.0.3/reasoner_validator/codes.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/reasoner_validator/github.py` & `reasoner_validator-4.0.3/reasoner_validator/github.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/reasoner_validator/message.py` & `reasoner_validator-4.0.3/reasoner_validator/message.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/reasoner_validator/report.py` & `reasoner_validator-4.0.3/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/reasoner_validator/sri/util.py` & `reasoner_validator-4.0.3/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/reasoner_validator/trapi/__init__.py` & `reasoner_validator-4.0.3/reasoner_validator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/reasoner_validator/trapi/mapping.py` & `reasoner_validator-4.0.3/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/reasoner_validator/validation_codes.py` & `reasoner_validator-4.0.3/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/reasoner_validator/validator.py` & `reasoner_validator-4.0.3/reasoner_validator/validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/reasoner_validator/versioning.py` & `reasoner_validator-4.0.3/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/reasoner_validator/versions.yaml` & `reasoner_validator-4.0.3/reasoner_validator/versions.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/tests/__init__.py` & `reasoner_validator-4.0.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/tests/test_biolink_compliance_validation.py` & `reasoner_validator-4.0.3/tests/test_biolink_compliance_validation.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml` & `reasoner_validator-4.0.3/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/tests/test_response_validator.py` & `reasoner_validator-4.0.3/tests/test_response_validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/tests/test_semver.py` & `reasoner_validator-4.0.3/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/tests/test_trapi_versioning.py` & `reasoner_validator-4.0.3/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/tests/test_validate.py` & `reasoner_validator-4.0.3/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/tests/test_validation_report.py` & `reasoner_validator-4.0.3/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/tests/test_workflows.py` & `reasoner_validator-4.0.3/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.2/PKG-INFO` & `reasoner_validator-4.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,34 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 4.0.2
+Version: 4.0.3
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
 Maintainer-email: richard.bruskiewich@delphinai.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<3.12
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Provides-Extra: docs
-Provides-Extra: web
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: bioregistry (>=0.11.1,<0.12.0)
 Requires-Dist: bmt (>=1.4.0,<2.0.0)
 Requires-Dist: dictdiffer (>=0.9.0,<0.10.0)
-Requires-Dist: fastapi ; extra == "web"
-Requires-Dist: httpx (>=0.18.2,<0.19.0) ; extra == "web"
 Requires-Dist: jsonschema (>=4.17.3,<4.18.0)
-Requires-Dist: myst-parser (>=2.0.0,<3.0.0) ; extra == "docs"
-Requires-Dist: numpydoc (>=1.5.0,<2.0.0) ; extra == "docs"
-Requires-Dist: opentelemetry-exporter-otlp-proto-http ; extra == "web"
-Requires-Dist: opentelemetry-instrumentation-fastapi ; extra == "web"
-Requires-Dist: opentelemetry-instrumentation-httpx ; extra == "web"
 Requires-Dist: pydantic (>=2,<3)
-Requires-Dist: pytest (>=7.2.2,<8.0.0)
-Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: sphinx (>=6.2.1,<7.0.0) ; extra == "docs"
-Requires-Dist: sphinx-rtd-theme (>=1.2.2,<2.0.0) ; extra == "docs"
 Requires-Dist: urllib3 (>=1.26.15,<2.0.0)
-Requires-Dist: uvicorn ; extra == "web"
 Project-URL: Bug Tracker, https://github.com/NCATSTranslator/reasoner-validator/issues
 Project-URL: Change Log, https://github.com/NCATSTranslator/reasoner-validator/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://translator-reasoner-validator.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/NCATSTranslator/reasoner-validator
 Description-Content-Type: text/markdown
 
 # Reasoner Validator
@@ -69,36 +54,40 @@
 
 The module may be installed directly from pypi.org using (Python 3) `pip` or `pip3`, namely:
 
 ```bash
 pip install reasoner-validator
 ```
 
-If you want to install it with the extra dependencies for using it as a web service, you can use:
-
-```bash
-pip install "reasoner-validator[web]"
-```
-
 ## Installing and working with the module locally from source
 
 As of release 3.1.6, this project uses the [poetry dependency management](https://python-poetry.org) tool to orchestrate its installation and dependencies.
 
-After [installing poetry](https://python-poetry.org/docs/#installation) and cloning the project, the poetry installation may be run:
+After [installing poetry](https://python-poetry.org/docs/#installation) and cloning the project, the poetry installation may be run (within the available poetry shell):
 
 ```bash
 git clone https://github.com/NCATSTranslator/reasoner-validator.git
 cd reasoner-validator
+poetry use 3.10
+poetry shell
 poetry install
 ```
 
-To develop this package, install with all extras dependencies using:
+Note that the **`poetry env`** can be set to either Python 3.10 or 3.11 at the present time.
+
+This installation also installs testing dependencies (in the poetry 'dev' group in the pyproject.toml) and documentation dependencies (in the corresponding poetry 'docs' group). If you don't want the overhead of these dependencies, then the installation of these poetry group dependencies may be excluded:
+
+```bash
+poetry install --without dev,docs
+```
+
+If you plan to run the web service API,  then install it with the optional web group:
 
 ```bash
-poetry install --all-extras
+poetry install reasoner-validator --with web
 ```
 
 ## Running Validation against an ARS UUID Result(*) or using a Local TRAPI Request Query
 
 A local script **`trapi_validator.py`** is available to run TRAPI Response validation against either a PK (UUID)
 indexed query result of the Biomedical Knowledge Translator "Autonomous Relay System" (ARS), a local JSON Response
 text file or a locally triggered _ad hoc_ query Request against a directly specified TRAPI endpoint.
@@ -111,21 +100,15 @@
 ./trapi_validator.py --help
 ```
 
 (*) Thank you Eric Deutsch for the prototype code for this script
 
 ## Running tests
 
-To run the test locally install with the `dev` dependencies, if not already done (e.g. by **`--all-extras`** above):
-
-```bash
-poetry install --extras dev
-```
-
-Run the tests with coverage report:
+Run the available unit tests with coverage report:
 
 ```bash
 poetry run pytest --cov
 ```
 
 Note that [poetry automatically uses any existing virtual environment](https://python-poetry.org/docs/basic-usage/#using-your-virtual-environment), but you can otherwise also enter the one that is created by poetry by default:
 
@@ -152,23 +135,15 @@
 
 ```bash
 python -m http.server 3000 --directory ./htmlcov
 ```
 
 ## Building the Documentation Locally
 
-All paths here are relative to the root project directory.
-
-First install the documentation-specific dependencies, if not already done (e.g. by **`--all-extras`** above):
-
-```bash
-poetry install --extras docs  # or poetry install --all-extras
-```
-
-The validation codes MarkDown file should first be regenerated if needed (i.e. if it was revised):
+All paths here are relative to the root project directory. The validation codes MarkDown file should first be regenerated if needed (i.e. if the **`codes.yaml`** was revised):
 
 ```bash
 cd reasoner_validator
 python ./validation_codes.py
 ```
 
 Then build the documentation locally:
```

