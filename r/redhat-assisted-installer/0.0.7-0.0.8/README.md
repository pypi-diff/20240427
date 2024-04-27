# Comparing `tmp/redhat_assisted_installer-0.0.7.tar.gz` & `tmp/redhat_assisted_installer-0.0.8.tar.gz`

## Comparing `redhat_assisted_installer-0.0.7.tar` & `redhat_assisted_installer-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.7/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.7/src/redhat_assisted_installer/__init__.py
--rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.7/src/redhat_assisted_installer/assistedinstaller.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.7/src/redhat_assisted_installer/lib/logging.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.7/src/redhat_assisted_installer/lib/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.7/src/redhat_assisted_installer/lib/schema/__init__.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.7/src/redhat_assisted_installer/lib/schema/createParams.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.7/tests/clusters/createanddelete.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.7/tests/clusters/createcluster.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.7/tests/clusters/deleteclusters.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.7/tests/clusters/getcluster.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.7/tests/infra-envs/createInfraEnvs.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.7/tests/infra-envs/deleteInfraEnvs.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.7/tests/infra-envs/getInfraEnv.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.7/README.md
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/src/redhat_assisted_installer/__init__.py
+-rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/src/redhat_assisted_installer/assistedinstaller.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/src/redhat_assisted_installer/lib/logging.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/src/redhat_assisted_installer/lib/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/src/redhat_assisted_installer/lib/schema/__init__.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/src/redhat_assisted_installer/lib/schema/createParams.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/tests/clusters/createanddelete.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/tests/clusters/createcluster.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/tests/clusters/deleteclusters.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/tests/clusters/getcluster.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/tests/infra-envs/createInfraEnvs.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/tests/infra-envs/deleteInfraEnvs.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/tests/infra-envs/getInfraEnv.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/README.md
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.8/PKG-INFO
```

### Comparing `redhat_assisted_installer-0.0.7/src/redhat_assisted_installer/assistedinstaller.py` & `redhat_assisted_installer-0.0.8/src/redhat_assisted_installer/assistedinstaller.py`

 * *Files identical despite different names*

### Comparing `redhat_assisted_installer-0.0.7/src/redhat_assisted_installer/lib/tools.py` & `redhat_assisted_installer-0.0.8/src/redhat_assisted_installer/lib/tools.py`

 * *Files identical despite different names*

### Comparing `redhat_assisted_installer-0.0.7/src/redhat_assisted_installer/lib/schema/createParams.py` & `redhat_assisted_installer-0.0.8/src/redhat_assisted_installer/lib/schema/createParams.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 
 class infraEnvCreateParams:
     def __init__(self, name, pullsecret, cpuarchitecture="x86_64", version=None, clusterid=None):
         self.params = {}
-        self.params['name'] = name + "infra-env"
+        self.params['name'] = name + "-infra-env"
         self.params['pull_secret'] = pullsecret
         self.params['cpu_architecture'] = cpuarchitecture
         if version is not None:
             self.params['openshift_version'] = version
         if clusterid is not None:
             self.params['cluster_id'] = clusterid
```

### Comparing `redhat_assisted_installer-0.0.7/pyproject.toml` & `redhat_assisted_installer-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "redhat-assisted-installer"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Justin Batchelor", email="justinrossbatchelor@gmail.com" },
 ]
 description = "Python module to implement the RedHat Assisted Installer API"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `redhat_assisted_installer-0.0.7/PKG-INFO` & `redhat_assisted_installer-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: redhat-assisted-installer
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python module to implement the RedHat Assisted Installer API
 Project-URL: Homepage, https://github.com/JustinBatchelor/red-hat-assisted-installer
 Project-URL: Issues, https://github.com/JustinBatchelor/red-hat-assisted-installer/issues
 Author-email: Justin Batchelor <justinrossbatchelor@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

