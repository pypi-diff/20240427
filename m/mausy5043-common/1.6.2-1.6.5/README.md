# Comparing `tmp/mausy5043_common-1.6.2.tar.gz` & `tmp/mausy5043_common-1.6.5.tar.gz`

## Comparing `mausy5043_common-1.6.2.tar` & `mausy5043_common-1.6.5.tar`

### file list

```diff
@@ -1,24 +1,20 @@
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/.editorconfig
--rw-r--r--   0        0        0    21857 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/.pylintrc
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/BUILDING.md
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/environment.yml
--rwxr-xr-x   0        0        0     2166 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/mkbld
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/requirements.txt
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/tox.ini
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/.github/dependabot.yml
--rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/src/mausy5043_common/__init__.py
--rwxr-xr-x   0        0        0     1089 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/src/mausy5043_common/funfile.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/src/mausy5043_common/funfile.pyi
--rwxr-xr-x   0        0        0     1419 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/src/mausy5043_common/funmeteo.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/src/mausy5043_common/funmeteo.pyi
--rwxr-xr-x   0        0        0      700 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/src/mausy5043_common/libsignals.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/src/mausy5043_common/libsignals.pyi
--rwxr-xr-x   0        0        0     9000 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/src/mausy5043_common/libsqlite3.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/src/mausy5043_common/libsqlite3.pyi
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/src/mausy5043_common/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/tests/.placeholder
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/LICENSE
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/README.md
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/pyproject.toml
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 mausy5043_common-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/.editorconfig
+-rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/.pylintrc
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/BUILDING.md
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/environment.yml
+-rwxr-xr-x   0        0        0     2292 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/mkbld
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/requirements.txt
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/tox.ini
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/.github/dependabot.yml
+-rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/src/mausy5043_common/__init__.py
+-rwxr-xr-x   0        0        0     1089 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/src/mausy5043_common/funfile.py
+-rwxr-xr-x   0        0        0     1419 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/src/mausy5043_common/funmeteo.py
+-rwxr-xr-x   0        0        0      700 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/src/mausy5043_common/libsignals.py
+-rwxr-xr-x   0        0        0     9000 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/src/mausy5043_common/libsqlite3.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/src/mausy5043_common/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/tests/.placeholder
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/LICENSE
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/README.md
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/pyproject.toml
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/PKG-INFO
```

### Comparing `mausy5043_common-1.6.2/.pylintrc` & `mausy5043_common-1.6.5/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -445,15 +445,15 @@
         use-symbolic-message-instead,
         use-implicit-booleaness-not-comparison-to-string,
         use-implicit-booleaness-not-comparison-to-zero,
         too-many-arguments,
         too-many-locals,
         too-many-branches,
         too-many-statements,
-        logging-fstring-interpolation,
+                logging-fstring-interpolation,
         import-error,
         invalid-name,
         missing-function-docstring,
         missing-module-docstring
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
```

### Comparing `mausy5043_common-1.6.2/BUILDING.md` & `mausy5043_common-1.6.5/BUILDING.md`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.6.2/mkbld` & `mausy5043_common-1.6.5/mkbld`

 * *Files 13% similar despite different names*

```diff
@@ -17,25 +17,26 @@
     echo
     echo "Checking build-system installation..."
     python3 -m pip install --upgrade build | grep -v "already satisfied"
     python3 -m pip install --upgrade twine | grep -v "already satisfied"
     ### build package
     echo
     echo "Building..."
-    rm dist/*
-    python3 -m build
+    rm -r dist/*
+    rm -r ./*.egg-info
+    python3 -m build --outdir ./dist # not needed by default: --sdist --wheel
 }
 
 test_app() {
     LOCATION=$1
     echo "Upload package to TestPyPi from $LOCATION"
     python3 -m twine upload --repository testpypi dist/*
     echo ""
     echo "To test installing this package use:"
-    echo "python3 -m pip install --index-url https://test.pypi.org/simple/ --no-deps --upgrade ${PACKAGE_NAME}"
+    echo "python3 -m pip install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple/ --no-deps --upgrade ${PACKAGE_NAME}"
 }
 
 dist_app() {
     LOCATION=$1
     echo "Upload distribution package to PyPi from $LOCATION"
     python3 -m twine upload --repository pypi dist/*
     echo ""
```

### Comparing `mausy5043_common-1.6.2/tox.ini` & `mausy5043_common-1.6.5/tox.ini`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.6.2/src/mausy5043_common/funfile.py` & `mausy5043_common-1.6.5/src/mausy5043_common/funfile.py`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.6.2/src/mausy5043_common/funmeteo.py` & `mausy5043_common-1.6.5/src/mausy5043_common/funmeteo.py`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.6.2/src/mausy5043_common/libsignals.py` & `mausy5043_common-1.6.5/src/mausy5043_common/libsignals.py`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.6.2/src/mausy5043_common/libsqlite3.py` & `mausy5043_common-1.6.5/src/mausy5043_common/libsqlite3.py`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.6.2/.gitignore` & `mausy5043_common-1.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.6.2/LICENSE` & `mausy5043_common-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.6.2/README.md` & `mausy5043_common-1.6.5/README.md`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.6.2/pyproject.toml` & `mausy5043_common-1.6.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,46 @@
+# pyproject.toml
+
 # Hatchling  https://packaging.python.org/en/latest/key_projects/#hatch
+
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mausy5043-common"
-description = "Common python functions"
-version = "1.6.2"  # latest production version
+version = "1.6.5"  # latest production version
 # version = "1.5.4" # latest test version
-dependencies = [
-    "numpy",
-    "pandas",
-]
+description = "Common python functions"
+readme = "README.md"
+requires-python = ">=3.8"
+license = "MIT"
 authors = [
   { name="Mausy5043" },
 ]
-license = "MIT"
-readme = "README.md"
-requires-python = ">=3.8"
+keywords = [
+    "private",
+    "Raspberry Pi",
+]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "numpy",
+    "pandas",
+]
+
+[tool.hatch.build.targets.wheel.force-include]
+"./pyproject.toml" = "mausy5043_common/pyproject.toml"
 
 [project.urls]
 "Homepage" = "https://github.com/Mausy5043/mausy5043-common"
 "Bug Tracker" = "https://github.com/Mausy5043/mausy5043-common/issues"
 
-[tool.setuptools.package-data]
-"mausy5043-common" = ["py.typed"]
+# [tool.setuptools.package-data]
+# "mausy5043-common" = ["py.typed"]
```

### Comparing `mausy5043_common-1.6.2/PKG-INFO` & `mausy5043_common-1.6.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: mausy5043-common
-Version: 1.6.2
+Version: 1.6.5
 Summary: Common python functions
 Project-URL: Homepage, https://github.com/Mausy5043/mausy5043-common
 Project-URL: Bug Tracker, https://github.com/Mausy5043/mausy5043-common/issues
 Author: Mausy5043
 License-Expression: MIT
 License-File: LICENSE
+Keywords: Raspberry Pi,private
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

