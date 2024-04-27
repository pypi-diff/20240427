# Comparing `tmp/passwork-0.1.2.tar.gz` & `tmp/passwork-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passwork-0.1.2.tar", last modified: Tue Apr 23 15:29:02 2024, max compression
+gzip compressed data, was "passwork-0.1.3.tar", last modified: Sat Apr 27 14:05:13 2024, max compression
```

## Comparing `passwork-0.1.2.tar` & `passwork-0.1.3.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-23 15:29:02.056072 passwork-0.1.2/
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1065 2024-04-23 15:05:31.000000 passwork-0.1.2/LICENSE
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     6227 2024-04-23 15:29:02.056017 passwork-0.1.2/PKG-INFO
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     5814 2024-04-23 15:05:31.000000 passwork-0.1.2/README.md
-drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-23 15:29:02.052696 passwork-0.1.2/passwork/
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-23 15:05:31.000000 passwork-0.1.2/passwork/__init__.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)       42 2024-04-23 15:05:31.000000 passwork-0.1.2/passwork/main.py
-drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-23 15:29:02.054069 passwork-0.1.2/passwork/password_crud/
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      168 2024-04-23 15:05:31.000000 passwork-0.1.2/passwork/password_crud/__init__.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     2908 2024-04-23 15:05:31.000000 passwork-0.1.2/passwork/password_crud/add_password.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      799 2024-04-23 15:05:31.000000 passwork-0.1.2/passwork/password_crud/delete_password.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     2247 2024-04-23 15:05:31.000000 passwork-0.1.2/passwork/password_crud/get_password.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1658 2024-04-23 15:05:31.000000 passwork-0.1.2/passwork/password_crud/search_password.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     6816 2024-04-23 15:20:34.000000 passwork-0.1.2/passwork/passwork_api.py
-drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-23 15:29:02.054974 passwork-0.1.2/passwork/rest_modules/
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1056 2024-04-23 15:05:31.000000 passwork-0.1.2/passwork/rest_modules/__init__.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     3843 2024-04-23 15:05:31.000000 passwork-0.1.2/passwork/rest_modules/passwords.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1462 2024-04-23 15:05:31.000000 passwork-0.1.2/passwork/rest_modules/users.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      431 2024-04-23 15:05:31.000000 passwork-0.1.2/passwork/rest_modules/vaults.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1223 2024-04-23 15:05:31.000000 passwork-0.1.2/passwork/session_options.py
-drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-23 15:29:02.055642 passwork-0.1.2/passwork/utils/
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      116 2024-04-23 15:05:31.000000 passwork-0.1.2/passwork/utils/__init__.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     3954 2024-04-23 15:05:31.000000 passwork-0.1.2/passwork/utils/base32.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     3200 2024-04-23 15:05:31.000000 passwork-0.1.2/passwork/utils/crypto_file.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     4269 2024-04-23 15:05:31.000000 passwork-0.1.2/passwork/utils/crypto_interface.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     3060 2024-04-23 15:05:31.000000 passwork-0.1.2/passwork/utils/passwork_utils.py
-drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-23 15:29:02.055817 passwork-0.1.2/passwork.egg-info/
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     6227 2024-04-23 15:29:02.000000 passwork-0.1.2/passwork.egg-info/PKG-INFO
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      765 2024-04-23 15:29:02.000000 passwork-0.1.2/passwork.egg-info/SOURCES.txt
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)        1 2024-04-23 15:29:02.000000 passwork-0.1.2/passwork.egg-info/dependency_links.txt
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)       52 2024-04-23 15:29:02.000000 passwork-0.1.2/passwork.egg-info/requires.txt
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)        9 2024-04-23 15:29:02.000000 passwork-0.1.2/passwork.egg-info/top_level.txt
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)       38 2024-04-23 15:29:02.056278 passwork-0.1.2/setup.cfg
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      638 2024-04-23 15:29:00.000000 passwork-0.1.2/setup.py
+drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-27 14:05:13.734683 passwork-0.1.3/
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1065 2024-04-23 15:05:31.000000 passwork-0.1.3/LICENSE
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     6227 2024-04-27 14:05:13.734626 passwork-0.1.3/PKG-INFO
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     5814 2024-04-23 15:05:31.000000 passwork-0.1.3/README.md
+drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-27 14:05:13.730125 passwork-0.1.3/passwork/
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-23 15:05:31.000000 passwork-0.1.3/passwork/__init__.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)       42 2024-04-23 15:05:31.000000 passwork-0.1.3/passwork/main.py
+drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-27 14:05:13.732142 passwork-0.1.3/passwork/password_crud/
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      168 2024-04-23 15:05:31.000000 passwork-0.1.3/passwork/password_crud/__init__.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     2908 2024-04-23 15:05:31.000000 passwork-0.1.3/passwork/password_crud/add_password.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      799 2024-04-23 15:05:31.000000 passwork-0.1.3/passwork/password_crud/delete_password.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     2121 2024-04-27 14:02:55.000000 passwork-0.1.3/passwork/password_crud/get_inbox_password.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     2248 2024-04-27 12:13:16.000000 passwork-0.1.3/passwork/password_crud/get_password.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1658 2024-04-23 15:05:31.000000 passwork-0.1.3/passwork/password_crud/search_password.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     8159 2024-04-27 13:34:55.000000 passwork-0.1.3/passwork/passwork_api.py
+drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-27 14:05:13.732944 passwork-0.1.3/passwork/rest_modules/
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1056 2024-04-23 15:05:31.000000 passwork-0.1.3/passwork/rest_modules/__init__.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     4646 2024-04-27 12:34:52.000000 passwork-0.1.3/passwork/rest_modules/passwords.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1808 2024-04-27 13:02:05.000000 passwork-0.1.3/passwork/rest_modules/users.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      431 2024-04-23 15:05:31.000000 passwork-0.1.3/passwork/rest_modules/vaults.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1362 2024-04-27 13:22:16.000000 passwork-0.1.3/passwork/session_options.py
+drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-27 14:05:13.734119 passwork-0.1.3/passwork/utils/
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      116 2024-04-23 15:05:31.000000 passwork-0.1.3/passwork/utils/__init__.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     3954 2024-04-23 15:05:31.000000 passwork-0.1.3/passwork/utils/base32.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     3200 2024-04-23 15:05:31.000000 passwork-0.1.3/passwork/utils/crypto_file.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     4679 2024-04-27 13:36:30.000000 passwork-0.1.3/passwork/utils/crypto_interface.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     3552 2024-04-27 12:57:05.000000 passwork-0.1.3/passwork/utils/passwork_utils.py
+drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-27 14:05:13.734374 passwork-0.1.3/passwork.egg-info/
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     6227 2024-04-27 14:05:13.000000 passwork-0.1.3/passwork.egg-info/PKG-INFO
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      810 2024-04-27 14:05:13.000000 passwork-0.1.3/passwork.egg-info/SOURCES.txt
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)        1 2024-04-27 14:05:13.000000 passwork-0.1.3/passwork.egg-info/dependency_links.txt
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)       52 2024-04-27 14:05:13.000000 passwork-0.1.3/passwork.egg-info/requires.txt
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)        9 2024-04-27 14:05:13.000000 passwork-0.1.3/passwork.egg-info/top_level.txt
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)       38 2024-04-27 14:05:13.734910 passwork-0.1.3/setup.cfg
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      638 2024-04-27 14:05:07.000000 passwork-0.1.3/setup.py
```

### Comparing `passwork-0.1.2/LICENSE` & `passwork-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `passwork-0.1.2/PKG-INFO` & `passwork-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passwork
-Version: 0.1.2
+Version: 0.1.3
 Summary: Passwork connector
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `passwork-0.1.2/README.md` & `passwork-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `passwork-0.1.2/passwork/password_crud/add_password.py` & `passwork-0.1.3/passwork/password_crud/add_password.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.2/passwork/password_crud/delete_password.py` & `passwork-0.1.3/passwork/password_crud/delete_password.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.2/passwork/password_crud/get_password.py` & `passwork-0.1.3/passwork/password_crud/get_password.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 from loguru import logger
 from passwork.passwork_api import PassworkAPI
 
+
 def get_password(api: PassworkAPI, password_id: str, log_pretty_data: bool = True) -> dict:
 
     """
     Retrieve password information from Passwork API.
 
     Args:
         api (PassworkAPI): An instance of PassworkAPI class initialized with appropriate credentials.
```

### Comparing `passwork-0.1.2/passwork/password_crud/search_password.py` & `passwork-0.1.3/passwork/password_crud/search_password.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.2/passwork/passwork_api.py` & `passwork-0.1.3/passwork/passwork_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from .session_options import SessionOptions
 from .rest_modules.passwords import get_password, get_attachments, search_passwords, add_password, \
-    delete_password
+    delete_password, get_inbox_passwords, get_inbox_password
 from .rest_modules.vaults import get_vault
 from .utils import (
     get_vault_password,
     get_encryption_key,
     get_customs,
     decrypt_and_save_password_attachment,
     decrypt_string,
+    get_inbox_encryption_key,
 )
 
 
 class PassworkAPI:
     """Interface for interacting with a methods from rest-modules."""
     def __init__(
             self,
@@ -32,14 +33,20 @@
 
     def logout(self):
         """Closes an API session.
         REST Endpoint: POST /auth/logout
         """
         self.session_options.logout()
 
+    def get_user_info(self):
+        """Get user info (RSA and etc.).
+        REST Endpoint: GET /user/info
+        """
+        self.session_options.get_user_info()
+
     def get_password(self, password_id: str) -> dict:
         """Retrieves a password by its identifier.
         REST Endpoint: GET /passwords/{password_id}
         Args:
             password_id (str): The identifier of the password to retrieve
 
         Returns:
@@ -194,7 +201,41 @@
 
         return add_password(
             password_adding_fields,
             vault_item,
             vault_password,
             options=self.session_options,
         )
+
+    def get_inbox_passwords(self) -> list[dict]:
+        """Retrieves a inbox password by its identifier.
+        REST Endpoint: GET /sharing/inbox/list
+
+        Returns:
+            The retrieved inbox passwords list
+        """
+
+        return get_inbox_passwords(self.session_options)
+
+    def get_inbox_password(self, inbox_password_id) -> dict:
+        """Retrieves a inbox password by its identifier.
+        REST Endpoint: POST /sharing/inbox/{inbox_password_id}
+
+        Args:
+            inbox_password_id (str): The identifier of the inbox password to retrieve
+
+        Returns:
+            The retrieved inbox password object dict
+        """
+        return get_inbox_password(inbox_password_id, self.session_options)
+
+    def get_inbox_encryption_key(self, inbox_password) -> str:
+        """Decrypts the encryption key for a password item.
+
+        Args:
+            inbox_password: The inbox password encrypted key
+
+        Returns:
+            Decrypted encryption key for inbox password decryption
+        """
+        return get_inbox_encryption_key(inbox_password, self.session_options)
+
```

### Comparing `passwork-0.1.2/passwork/rest_modules/__init__.py` & `passwork-0.1.3/passwork/rest_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.2/passwork/rest_modules/passwords.py` & `passwork-0.1.3/passwork/rest_modules/passwords.py`

 * *Files 23% similar despite different names*

```diff
@@ -124,7 +124,36 @@
     if is_failed_status_code(
         status_code=response.status_code,
         prefix=f"Error when deleting password with id {password_id}",
     ):
         raise Exception
 
     logger.success(f"Deletion of password with id {password_id} completed successfully")
+
+
+def get_inbox_passwords(options):
+    response = requests.get(
+        url=f"{options.host}/sharing/inbox/list", headers=options.request_headers
+    )
+
+    if is_failed_status_code(
+        status_code=response.status_code,
+        prefix=f"Error when getting list of inbox passwords",
+    ):
+        raise Exception
+
+    return response.json().get("data")
+
+
+def get_inbox_password(inbox_password_id, options):
+    response = requests.post(
+        url=f"{options.host}/sharing/inbox/{inbox_password_id}", headers=options.request_headers
+    )
+
+    if is_failed_status_code(
+        status_code=response.status_code,
+        prefix=f"Error when getting inbox password id: {inbox_password_id}",
+    ):
+        raise Exception
+
+    inbox_password = response.json().get("data")
+    return inbox_password
```

### Comparing `passwork-0.1.2/passwork/rest_modules/users.py` & `passwork-0.1.3/passwork/rest_modules/users.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,7 +37,16 @@
         response = requests.post(
             url=f"{self.options.host}/auth/logout",
             headers={"Passwork-Auth": self.options.token},
         )
         if is_failed_status_code(prefix="Failed to log out", status_code=response.status_code):
             raise Exception
         return response.json().get("data")
+
+    def get_user_info(self):
+        response = requests.get(
+            url=f"{self.options.host}/user/info",
+            headers=self.options.request_headers,
+        )
+        if is_failed_status_code(prefix="Failed to get user info", status_code=response.status_code):
+            raise Exception
+        return response.json().get("data")
```

### Comparing `passwork-0.1.2/passwork/utils/base32.py` & `passwork-0.1.3/passwork/utils/base32.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.2/passwork/utils/crypto_file.py` & `passwork-0.1.3/passwork/utils/crypto_file.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.2/passwork/utils/crypto_interface.py` & `passwork-0.1.3/passwork/utils/crypto_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import os
 import re
 import hashlib
 import secrets
 import binascii
 from base64 import b64encode, b64decode
+from cryptography.hazmat.primitives import padding, serialization
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
-from cryptography.hazmat.primitives import padding
+from cryptography.hazmat.primitives.asymmetric import padding as padding_rsa
 from cryptography.hazmat.backends import default_backend
 
+
 from ..utils.base32 import base32
 
 
 __all__ = [
     "encrypt_aes",
     "decrypt_aes",
     "generate_password",
     "get_master_key",
     "get_request_headers",
     "generate_string",
+    "rsa_decrypt"
 ]
 
 
 def evp_bytes_to_key(password: str, salt: bytes, key_len: int, iv_len: int):
     """
     OpenSSL key and IV generation
     """
@@ -121,7 +124,19 @@
     headers = {"Passwork-Auth": token}
 
     if use_master_password:
         # calculate hash
         master_key_hash = hashlib.sha256(master_key.encode()).hexdigest()
         headers["Passwork-MasterHash"] = master_key_hash
     return headers
+
+
+def rsa_decrypt(data, private_key):
+    private_key = serialization.load_pem_private_key(
+        private_key.encode(),  # Convert to bytes
+        password=None
+    )
+    decrypted_data = private_key.decrypt(
+        b64decode(data),
+        padding_rsa.PKCS1v15()
+    )
+    return decrypted_data
```

### Comparing `passwork-0.1.2/passwork/utils/passwork_utils.py` & `passwork-0.1.3/passwork/utils/passwork_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     "get_customs",
     "is_valid_totp",
     "use_key_encryption",
     "validate_customs",
     "encrypt_string",
     "encrypt_customs",
     "decrypt_string",
+    "get_inbox_encryption_key"
 ]
 
 
 def get_encryption_key(password: dict, vault_password: str, use_master_password: bool = False):
     if not use_master_password:
         return ""
 
@@ -84,7 +85,18 @@
         for field, value in custom.items():
             if field not in ["name", "value", "type"]:
                 encrypted_custom[field] = value  # Preserve these fields without encryption
             else:
                 encrypted_custom[field] = encrypt_string(value, encryption_key, options)
         encrypted_fields.append(encrypted_custom)
     return encrypted_fields
+
+
+def get_inbox_encryption_key(inbox_password, options):
+    user_info = options.user_info
+    if options.use_master_password:
+        if not user_info.get("keys"):
+            raise Exception({"code": "Can't fetch user private keys"})
+        privat_key = decrypt_string(user_info["keys"]["privateCrypted"], options.master_key, options)
+        return crypto_interface.rsa_decrypt(inbox_password["cryptedKey"], privat_key).decode()
+    else:
+        return ""
```

### Comparing `passwork-0.1.2/passwork.egg-info/PKG-INFO` & `passwork-0.1.3/passwork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passwork
-Version: 0.1.2
+Version: 0.1.3
 Summary: Passwork connector
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `passwork-0.1.2/passwork.egg-info/SOURCES.txt` & `passwork-0.1.3/passwork.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 passwork.egg-info/SOURCES.txt
 passwork.egg-info/dependency_links.txt
 passwork.egg-info/requires.txt
 passwork.egg-info/top_level.txt
 passwork/password_crud/__init__.py
 passwork/password_crud/add_password.py
 passwork/password_crud/delete_password.py
+passwork/password_crud/get_inbox_password.py
 passwork/password_crud/get_password.py
 passwork/password_crud/search_password.py
 passwork/rest_modules/__init__.py
 passwork/rest_modules/passwords.py
 passwork/rest_modules/users.py
 passwork/rest_modules/vaults.py
 passwork/utils/__init__.py
```

### Comparing `passwork-0.1.2/setup.py` & `passwork-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='passwork',
-    version='0.1.2',
+    version='0.1.3',
     description='Passwork connector',
     long_description=readme(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'requests>=2.31.0',
         'cryptography>=42.0.5',
```

