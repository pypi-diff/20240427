# Comparing `tmp/redhat_assisted_installer-0.0.9.tar.gz` & `tmp/redhat_assisted_installer-0.1.0.tar.gz`

## Comparing `redhat_assisted_installer-0.0.9.tar` & `redhat_assisted_installer-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/requirements.txt
--rw-r--r--   0        0        0   129638 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/docs/downloads_console.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/src/redhat_assisted_installer/__init__.py
--rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/src/redhat_assisted_installer/assistedinstaller.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/src/redhat_assisted_installer/lib/logging.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/src/redhat_assisted_installer/lib/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/src/redhat_assisted_installer/lib/schema/__init__.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/src/redhat_assisted_installer/lib/schema/createParams.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/tests/clusters/createanddelete.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/tests/clusters/createcluster.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/tests/clusters/deleteclusters.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/tests/clusters/getcluster.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/tests/infra-envs/createInfraEnvs.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/tests/infra-envs/deleteInfraEnvs.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/tests/infra-envs/getInfraEnv.py
--rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/README.md
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     7497 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0   129638 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.1.0/downloads_console.png
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.1.0/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.1.0/src/redhat_assisted_installer/__init__.py
+-rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.1.0/src/redhat_assisted_installer/assistedinstaller.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.1.0/src/redhat_assisted_installer/lib/logging.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.1.0/src/redhat_assisted_installer/lib/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.1.0/src/redhat_assisted_installer/lib/schema/__init__.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.1.0/src/redhat_assisted_installer/lib/schema/createParams.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.1.0/tests/clusters/createanddelete.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.1.0/tests/clusters/createcluster.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.1.0/tests/clusters/deleteclusters.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.1.0/tests/clusters/getcluster.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.1.0/tests/infra-envs/createInfraEnvs.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.1.0/tests/infra-envs/deleteInfraEnvs.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.1.0/tests/infra-envs/getInfraEnv.py
+-rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.1.0/README.md
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7490 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.1.0/PKG-INFO
```

### Comparing `redhat_assisted_installer-0.0.9/docs/downloads_console.png` & `redhat_assisted_installer-0.1.0/downloads_console.png`

 * *Files identical despite different names*

### Comparing `redhat_assisted_installer-0.0.9/src/redhat_assisted_installer/assistedinstaller.py` & `redhat_assisted_installer-0.1.0/src/redhat_assisted_installer/assistedinstaller.py`

 * *Files identical despite different names*

### Comparing `redhat_assisted_installer-0.0.9/src/redhat_assisted_installer/lib/tools.py` & `redhat_assisted_installer-0.1.0/src/redhat_assisted_installer/lib/tools.py`

 * *Files identical despite different names*

### Comparing `redhat_assisted_installer-0.0.9/src/redhat_assisted_installer/lib/schema/createParams.py` & `redhat_assisted_installer-0.1.0/src/redhat_assisted_installer/lib/schema/createParams.py`

 * *Files identical despite different names*

### Comparing `redhat_assisted_installer-0.0.9/README.md` & `redhat_assisted_installer-0.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 - `REDHAT_PULL_SECRET`: The pull secret associated with your RedHat Hybrid Cloud account
 
 - `REDHAT_OFFLINE_TOKEN`: The offline token associated with your RedHat Hybrid Cloud account
 
 
 **_You can find these credentials by navigating to https://console.redhat.com/openshift/overview. In the side panel navigate to `Downloads`, and at the bottom of the page you should see the pull secret and token_**
 
-![alt text](./docs/downloads_console.png)
+![alt text](downloads_console.png)
 
 
 ## How to use
 
 ### Create AssistedInstaller instance
 
     # import package
```

### Comparing `redhat_assisted_installer-0.0.9/pyproject.toml` & `redhat_assisted_installer-0.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "redhat-assisted-installer"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Justin Batchelor", email="justinrossbatchelor@gmail.com" },
 ]
 description = "Python module to implement the RedHat Assisted Installer API"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `redhat_assisted_installer-0.0.9/PKG-INFO` & `redhat_assisted_installer-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: redhat-assisted-installer
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python module to implement the RedHat Assisted Installer API
 Project-URL: Homepage, https://github.com/JustinBatchelor/red-hat-assisted-installer
 Project-URL: Issues, https://github.com/JustinBatchelor/red-hat-assisted-installer/issues
 Author-email: Justin Batchelor <justinrossbatchelor@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -32,15 +32,15 @@
 - `REDHAT_PULL_SECRET`: The pull secret associated with your RedHat Hybrid Cloud account
 
 - `REDHAT_OFFLINE_TOKEN`: The offline token associated with your RedHat Hybrid Cloud account
 
 
 **_You can find these credentials by navigating to https://console.redhat.com/openshift/overview. In the side panel navigate to `Downloads`, and at the bottom of the page you should see the pull secret and token_**
 
-![alt text](./docs/downloads_console.png)
+![alt text](downloads_console.png)
 
 
 ## How to use
 
 ### Create AssistedInstaller instance
 
     # import package
```

