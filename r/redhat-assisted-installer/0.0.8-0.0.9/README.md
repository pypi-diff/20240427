# Comparing `tmp/redhat_assisted_installer-0.0.8.tar.gz` & `tmp/redhat_assisted_installer-0.0.9.tar.gz`

## Comparing `redhat_assisted_installer-0.0.8.tar` & `redhat_assisted_installer-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/src/redhat_assisted_installer/__init__.py
--rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/src/redhat_assisted_installer/assistedinstaller.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/src/redhat_assisted_installer/lib/logging.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/src/redhat_assisted_installer/lib/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/src/redhat_assisted_installer/lib/schema/__init__.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/src/redhat_assisted_installer/lib/schema/createParams.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/tests/clusters/createanddelete.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/tests/clusters/createcluster.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/tests/clusters/deleteclusters.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/tests/clusters/getcluster.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/tests/infra-envs/createInfraEnvs.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/tests/infra-envs/deleteInfraEnvs.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/tests/infra-envs/getInfraEnv.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/README.md
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/requirements.txt
+-rw-r--r--   0        0        0   129638 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/docs/downloads_console.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/src/redhat_assisted_installer/__init__.py
+-rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/src/redhat_assisted_installer/assistedinstaller.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/src/redhat_assisted_installer/lib/logging.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/src/redhat_assisted_installer/lib/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/src/redhat_assisted_installer/lib/schema/__init__.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/src/redhat_assisted_installer/lib/schema/createParams.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/tests/clusters/createanddelete.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/tests/clusters/createcluster.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/tests/clusters/deleteclusters.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/tests/clusters/getcluster.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/tests/infra-envs/createInfraEnvs.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/tests/infra-envs/deleteInfraEnvs.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/tests/infra-envs/getInfraEnv.py
+-rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/README.md
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     7497 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/PKG-INFO
```

### Comparing `redhat_assisted_installer-0.0.8/src/redhat_assisted_installer/assistedinstaller.py` & `redhat_assisted_installer-0.0.9/src/redhat_assisted_installer/assistedinstaller.py`

 * *Files identical despite different names*

### Comparing `redhat_assisted_installer-0.0.8/src/redhat_assisted_installer/lib/tools.py` & `redhat_assisted_installer-0.0.9/src/redhat_assisted_installer/lib/tools.py`

 * *Files identical despite different names*

### Comparing `redhat_assisted_installer-0.0.8/src/redhat_assisted_installer/lib/schema/createParams.py` & `redhat_assisted_installer-0.0.9/src/redhat_assisted_installer/lib/schema/createParams.py`

 * *Files identical despite different names*

### Comparing `redhat_assisted_installer-0.0.8/pyproject.toml` & `redhat_assisted_installer-0.0.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "redhat-assisted-installer"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Justin Batchelor", email="justinrossbatchelor@gmail.com" },
 ]
 description = "Python module to implement the RedHat Assisted Installer API"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

