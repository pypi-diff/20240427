# Comparing `tmp/hcp_vault_secrets-0.0.1.tar.gz` & `tmp/hcp_vault_secrets-0.0.2.tar.gz`

## Comparing `hcp_vault_secrets-0.0.1.tar` & `hcp_vault_secrets-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.1/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.1/src/hcp_vault_secrets/__init__.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.1/src/hcp_vault_secrets/vaultsecrets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.1/src/hcp_vault_secrets/lib/__init__.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.1/src/hcp_vault_secrets/lib/logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.1/tests/getSecrets.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.1/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.2/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.2/src/hcp_vault_secrets/__init__.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.2/src/hcp_vault_secrets/vaultsecrets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.2/src/hcp_vault_secrets/lib/__init__.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.2/src/hcp_vault_secrets/lib/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.2/tests/getSecrets.py
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.2/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 hcp_vault_secrets-0.0.2/PKG-INFO
```

### Comparing `hcp_vault_secrets-0.0.1/src/hcp_vault_secrets/vaultsecrets.py` & `hcp_vault_secrets-0.0.2/src/hcp_vault_secrets/vaultsecrets.py`

 * *Files identical despite different names*

### Comparing `hcp_vault_secrets-0.0.1/pyproject.toml` & `hcp_vault_secrets-0.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hcp-vault-secrets"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Justin Batchelor", email="justinrossbatchelor@gmail.com" },
 ]
 description = "Python module to implement the the Hashicorp Cloud Platform vault secrets API"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

