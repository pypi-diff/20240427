# Comparing `tmp/hcp_vault_secrets-0.0.3.tar.gz` & `tmp/hcp_vault_secrets-0.0.4.tar.gz`

## Comparing `hcp_vault_secrets-0.0.3.tar` & `hcp_vault_secrets-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    74591 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.3/docs/pics/hcp-topo.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.3/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.3/src/hcp_vault_secrets/__init__.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.3/src/hcp_vault_secrets/vaultsecrets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.3/src/hcp_vault_secrets/lib/__init__.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.3/src/hcp_vault_secrets/lib/logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.3/tests/getSecrets.py
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.3/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    74591 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.4/docs/pics/hcp-topo.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.4/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.4/src/hcp_vault_secrets/__init__.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.4/src/hcp_vault_secrets/vaultsecrets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.4/src/hcp_vault_secrets/lib/__init__.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.4/src/hcp_vault_secrets/lib/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.4/tests/getSecrets.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.4/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.4/PKG-INFO
```

### Comparing `hcp_vault_secrets-0.0.3/docs/pics/hcp-topo.png` & `hcp_vault_secrets-0.0.4/docs/pics/hcp-topo.png`

 * *Files identical despite different names*

### Comparing `hcp_vault_secrets-0.0.3/src/hcp_vault_secrets/vaultsecrets.py` & `hcp_vault_secrets-0.0.4/src/hcp_vault_secrets/vaultsecrets.py`

 * *Files identical despite different names*

### Comparing `hcp_vault_secrets-0.0.3/README.md` & `hcp_vault_secrets-0.0.4/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 
 ### Hashicorp Cloud Platform (HCP)
 
 **HCP Topology**
 
 - Organization -> Project(s) -> Service(s) [e.g Vault Secrets] -> Application -> Key/Value (secret)
 
+![](https://github.com/JustinBatchelor/hcp-vault-secrets/blob/37ad8ca3c33e52dc256d3c187a05169665283192/docs/pics/hcp-topo.png?raw=true)
+
+
 ## How to use
 
 ### Create Hashicorp Cloud Platform Instance
 
     # import hcp_vault_secrets package
     import hcp_vault_secrets.vaultsecrets as vaultsecrets
 
@@ -54,17 +57,14 @@
 Path Parameters
 
 | name | type | description | required |
 | ---- | ---- | ----------- | -------- |
 | appName | string | The name of the vault secrets application where the key is stored | True |
 | secretName | string | The name of the secrets' key you want to retrieve | True |
 
-![](https://github.com/JustinBatchelor/hcp-vault-secrets/blob/37ad8ca3c33e52dc256d3c187a05169665283192/docs/pics/hcp-topo.png?raw=true)
-
-
 **EXAMPLES**
 
     import hcp_vault_secrets.vaultsecrets as vaultsecrets
 
     # create hcp instance
     hcp = vaultsecrets.vaultsecrets()
```

### Comparing `hcp_vault_secrets-0.0.3/pyproject.toml` & `hcp_vault_secrets-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hcp-vault-secrets"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Justin Batchelor", email="justinrossbatchelor@gmail.com" },
 ]
 description = "Python module to implement the the Hashicorp Cloud Platform vault secrets API"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `hcp_vault_secrets-0.0.3/PKG-INFO` & `hcp_vault_secrets-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hcp-vault-secrets
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python module to implement the the Hashicorp Cloud Platform vault secrets API
 Project-URL: Homepage, https://github.com/JustinBatchelor/red-hat-assisted-installer
 Project-URL: Issues, https://github.com/JustinBatchelor/red-hat-assisted-installer/issues
 Author-email: Justin Batchelor <justinrossbatchelor@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -44,14 +44,17 @@
 
 ### Hashicorp Cloud Platform (HCP)
 
 **HCP Topology**
 
 - Organization -> Project(s) -> Service(s) [e.g Vault Secrets] -> Application -> Key/Value (secret)
 
+![](https://github.com/JustinBatchelor/hcp-vault-secrets/blob/37ad8ca3c33e52dc256d3c187a05169665283192/docs/pics/hcp-topo.png?raw=true)
+
+
 ## How to use
 
 ### Create Hashicorp Cloud Platform Instance
 
     # import hcp_vault_secrets package
     import hcp_vault_secrets.vaultsecrets as vaultsecrets
 
@@ -67,17 +70,14 @@
 Path Parameters
 
 | name | type | description | required |
 | ---- | ---- | ----------- | -------- |
 | appName | string | The name of the vault secrets application where the key is stored | True |
 | secretName | string | The name of the secrets' key you want to retrieve | True |
 
-![](https://github.com/JustinBatchelor/hcp-vault-secrets/blob/37ad8ca3c33e52dc256d3c187a05169665283192/docs/pics/hcp-topo.png?raw=true)
-
-
 **EXAMPLES**
 
     import hcp_vault_secrets.vaultsecrets as vaultsecrets
 
     # create hcp instance
     hcp = vaultsecrets.vaultsecrets()
```

