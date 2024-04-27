# Comparing `tmp/streamlit-ldap-authenticator-0.2.4.tar.gz` & `tmp/streamlit-ldap-authenticator-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-ldap-authenticator-0.2.4.tar", last modified: Mon Apr  8 11:32:28 2024, max compression
+gzip compressed data, was "streamlit-ldap-authenticator-0.2.5.tar", last modified: Sat Apr 27 03:20:18 2024, max compression
```

## Comparing `streamlit-ldap-authenticator-0.2.4.tar` & `streamlit-ldap-authenticator-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 11:32:28.746775 streamlit-ldap-authenticator-0.2.4/
--rw-rw-rw-   0        0        0     1089 2024-02-22 23:54:56.000000 streamlit-ldap-authenticator-0.2.4/LICENSE
--rw-rw-rw-   0        0        0    23668 2024-04-08 11:32:28.742824 streamlit-ldap-authenticator-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    22653 2024-04-08 11:31:49.000000 streamlit-ldap-authenticator-0.2.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-08 11:32:28.746775 streamlit-ldap-authenticator-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1505 2024-04-08 11:31:58.000000 streamlit-ldap-authenticator-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 11:32:28.716378 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator/
--rw-rw-rw-   0        0        0      308 2024-03-23 04:43:04.000000 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator/__init__.py
--rw-rw-rw-   0        0        0    18464 2024-04-08 10:58:49.000000 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator/authenticate.py
--rw-rw-rw-   0        0        0    10523 2024-03-23 04:42:56.000000 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator/configs.py
--rw-rw-rw-   0        0        0      971 2024-02-22 10:48:27.000000 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator/exceptions.py
--rw-rw-rw-   0        0        0     7428 2024-04-04 00:17:59.000000 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator/ldap_authenticate.py
-drwxrwxrwx   0        0        0        0 2024-04-08 11:32:28.737010 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator.egg-info/
--rw-rw-rw-   0        0        0    23668 2024-04-08 11:32:28.000000 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2024-04-08 11:32:28.000000 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 11:32:28.000000 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      231 2024-04-08 11:32:28.000000 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-04-08 11:32:28.000000 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 03:20:18.297975 streamlit-ldap-authenticator-0.2.5/
+-rw-rw-rw-   0        0        0     1089 2024-02-29 23:36:46.000000 streamlit-ldap-authenticator-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0    23758 2024-04-27 03:20:18.297086 streamlit-ldap-authenticator-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0    22743 2024-04-27 03:20:04.000000 streamlit-ldap-authenticator-0.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 03:20:18.298976 streamlit-ldap-authenticator-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1505 2024-04-27 03:18:41.000000 streamlit-ldap-authenticator-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:20:18.284974 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator/
+-rw-rw-rw-   0        0        0      308 2024-03-27 14:06:56.000000 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator/__init__.py
+-rw-rw-rw-   0        0        0    18526 2024-04-27 03:17:12.000000 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator/authenticate.py
+-rw-rw-rw-   0        0        0    10671 2024-04-27 03:17:16.000000 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator/configs.py
+-rw-rw-rw-   0        0        0      971 2024-02-29 23:36:46.000000 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator/exceptions.py
+-rw-rw-rw-   0        0        0     7428 2024-04-27 03:07:29.000000 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator/ldap_authenticate.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:20:18.293974 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator.egg-info/
+-rw-rw-rw-   0        0        0    23758 2024-04-27 03:20:18.000000 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2024-04-27 03:20:18.000000 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 03:20:18.000000 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      231 2024-04-27 03:20:18.000000 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-04-27 03:20:18.000000 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator.egg-info/top_level.txt
```

### Comparing `streamlit-ldap-authenticator-0.2.4/LICENSE` & `streamlit-ldap-authenticator-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-ldap-authenticator-0.2.4/PKG-INFO` & `streamlit-ldap-authenticator-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-ldap-authenticator
-Version: 0.2.4
+Version: 0.2.5
 Summary: Authenticate using ldap
 Home-page: https://github.com/NathanChen198/streamlit-ldap-authenticator
 Author: Nathan Chen
 Author-email: nathan.chen.198@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -518,14 +518,18 @@
 
 - Enhance security by clearing password from Connection object after bind.
 
 ### Version 0.2.4
 
 - Fix 'no attribute in signinevent' when cookie option is disabled.
 
+### Version 0.2.5
+
+- Add Optional delay_sec in cookie config for set and del cookie.
+
 [pypi_badge]: https://img.shields.io/pypi/v/streamlit-ldap-authenticator.svg
 [pypi_link]: https://pypi.org/project/streamlit-ldap-authenticator
 [pypi_download_badge]: https://static.pepy.tech/badge/streamlit-ldap-authenticator
 [github_badge]: https://badgen.net/badge/icon/GitHub?icon=github&color=black&label
 [github_link]: https://github.com/NathanChen198/streamlit-ldap-authenticator
 [license_badge]: https://img.shields.io/badge/Licence-MIT-gr.svg
 [license_link]: https://github.com/NathanChen198/streamlit-ldap-authenticator/blob/main/LICENSE
```

### Comparing `streamlit-ldap-authenticator-0.2.4/README.md` & `streamlit-ldap-authenticator-0.2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -492,14 +492,18 @@
 
 - Enhance security by clearing password from Connection object after bind.
 
 ### Version 0.2.4
 
 - Fix 'no attribute in signinevent' when cookie option is disabled.
 
+### Version 0.2.5
+
+- Add Optional delay_sec in cookie config for set and del cookie.
+
 [pypi_badge]: https://img.shields.io/pypi/v/streamlit-ldap-authenticator.svg
 [pypi_link]: https://pypi.org/project/streamlit-ldap-authenticator
 [pypi_download_badge]: https://static.pepy.tech/badge/streamlit-ldap-authenticator
 [github_badge]: https://badgen.net/badge/icon/GitHub?icon=github&color=black&label
 [github_link]: https://github.com/NathanChen198/streamlit-ldap-authenticator
 [license_badge]: https://img.shields.io/badge/Licence-MIT-gr.svg
 [license_link]: https://github.com/NathanChen198/streamlit-ldap-authenticator/blob/main/LICENSE
```

### Comparing `streamlit-ldap-authenticator-0.2.4/setup.py` & `streamlit-ldap-authenticator-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Author   : Nathan Chen
-# Date     : 08-Apr-2024
+# Date     : 27-Apr-2024
 
 
 from pathlib import Path
 from setuptools import setup, find_packages
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding='UTF-8')
 
 setup(
     name='streamlit-ldap-authenticator',
-    version='0.2.4',
+    version='0.2.5',
     author='Nathan Chen',
     author_email='nathan.chen.198@gmail.com',
     description='Authenticate using ldap',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/NathanChen198/streamlit-ldap-authenticator',
     packages=find_packages(),
```

### Comparing `streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator/authenticate.py` & `streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator/authenticate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Author    : Nathan Chen
-# Date      : 04-Apr-2024
+# Date      : 27-Apr-2024
+
 
 
 import time
 import jwt
 import re
 import streamlit as st
 from streamlit_cookies_controller import CookieController
@@ -36,19 +37,20 @@
         Reauthorization using cookie in the client's browser feature will be disabled when `None`.
     """
     
     session_configs: SessionStateConfig
     cookie_configs: Optional[CookieConfig]
 
 
-    def __init__(self,
-                 ldap_configs: Union[LdapConfig, AttrDict],
-                 session_configs: Union[SessionStateConfig, AttrDict, None] = None,
-                 cookie_configs: Union[CookieConfig, AttrDict, None] = None,
-                 encryptor_configs: Union[EncryptorConfig, AttrDict, None] = None):
+    def __init__(
+            self,
+            ldap_configs: Union[LdapConfig, AttrDict],
+            session_configs: Union[SessionStateConfig, AttrDict, None] = None,
+            cookie_configs: Union[CookieConfig, AttrDict, None] = None,
+            encryptor_configs: Union[EncryptorConfig, AttrDict, None] = None):
         """ Create a new instance of `Authenticate`
 
         ## Arguments
         ldap_config: LdapConfig | dict | streamlit.runtime.secrets.AttrDict
             Config for Ldap authentication
 
         session_configs: SessionStateConfig | dict | streamlit.runtime.secrets.AttrDict | None
@@ -184,30 +186,30 @@
 
         remember_me = self.__getRememberMe()
         if not remember_me: return
 
         token = self.__tokenEncode(self.cookie_configs, user)
         exp_date = datetime.now() + timedelta(days=self.cookie_configs.expiry_days)
         self.cookie_manager.set(self.cookie_configs.name, token, expires=exp_date)
-        time.sleep(0.1)
+        time.sleep(self.cookie_configs.delay_sec)
 
     def __deleteCookie(self):
         """ Delete the cookie in the client's browser
             if reauthorization using cookie in the client's browser is enabled
         """
         if self.cookie_configs is None: return
 
         cookies = self.cookie_manager.getAll()
         if self.cookie_configs.name in cookies:
             self.cookie_manager.remove(self.cookie_configs.name)
+            time.sleep(self.cookie_configs.delay_sec)
 
     def __getLoginConfig(self, config: Union[Object, LoginConfig, None] = None):
         config = config if type(config) is dict else \
-            config.toDict() if isinstance(config, LoginConfig) else \
-            {}
+            config.toDict() if isinstance(config, LoginConfig) else {}
         
         if self.cookie_configs is not None and 'remember' not in config:
             config['remember'] = {}
         
         busy_message = config.get("busy_message")
         config.pop('busy_message', "")
         if type(busy_message) is not str: busy_message = "Logging in..."
```

### Comparing `streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator/configs.py` & `streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # Author    : Nathan Chen
-# Date      : 23-Mar-2024
-
-
+# Date      : 27-Apr-2024
 
 
 
 from streamlit.runtime.secrets import AttrDict as _AttrDict
 from streamlit_rsa_auth_ui import SigninFormConfig, SignoutFormConfig, FormType, HorizontalAlign, Object
 from typing import Type, Optional, Union, TypeVar, List, Dict, Any
 
@@ -196,31 +194,36 @@
         name of the cookie to save in the client's browser
     expiry_days: float
         The number of days before the reauthentication cookie automatically expires on the client's browser.
     """
     __default_name__: str = "login_cookie"
     __default_expiry_days__: float = 1.0
     __default_auto_renewal__: bool = True
+    __default_delay_sec__: float = 0.1
 
     
     key: str
     name: str
     expiry_days: float
     auto_renewal: bool
+    delay_sec: float
 
-    def __init__(self, key: str,
-                 name: str = __default_name__,
-                 expiry_days: float = __default_expiry_days__,
-                 auto_renewal: bool = __default_auto_renewal__):
+    def __init__(
+            self, key: str,
+            name: str = __default_name__,
+            expiry_days: float = __default_expiry_days__,
+            auto_renewal: bool = __default_auto_renewal__,
+            delay_sec: float = __default_delay_sec__):
         """ Create an instance of `CookieConfig` object
         """
         self.key = key
         self.name = name
         self.expiry_days = expiry_days
         self.auto_renewal = auto_renewal
+        self.delay_sec = delay_sec
 
     @classmethod
     def from_dict(cls, dict: AttrDict) -> 'CookieConfig':
         key = cls._getAttr(dict, 'key', str)
         name = cls._getAttrWithDefault(dict, 'name', str, cls.__default_name__)
         expiry_days = cls._getAttrWithDefault(dict, 'expiry_days', float, cls.__default_expiry_days__)
         auto_renewal = cls._getAttrWithDefault(dict, 'auto_renewal', bool, cls.__default_auto_renewal__)
```

### Comparing `streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator/exceptions.py` & `streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator/exceptions.py`

 * *Files identical despite different names*

### Comparing `streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator/ldap_authenticate.py` & `streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator/ldap_authenticate.py`

 * *Files identical despite different names*

### Comparing `streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator.egg-info/PKG-INFO` & `streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-ldap-authenticator
-Version: 0.2.4
+Version: 0.2.5
 Summary: Authenticate using ldap
 Home-page: https://github.com/NathanChen198/streamlit-ldap-authenticator
 Author: Nathan Chen
 Author-email: nathan.chen.198@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -518,14 +518,18 @@
 
 - Enhance security by clearing password from Connection object after bind.
 
 ### Version 0.2.4
 
 - Fix 'no attribute in signinevent' when cookie option is disabled.
 
+### Version 0.2.5
+
+- Add Optional delay_sec in cookie config for set and del cookie.
+
 [pypi_badge]: https://img.shields.io/pypi/v/streamlit-ldap-authenticator.svg
 [pypi_link]: https://pypi.org/project/streamlit-ldap-authenticator
 [pypi_download_badge]: https://static.pepy.tech/badge/streamlit-ldap-authenticator
 [github_badge]: https://badgen.net/badge/icon/GitHub?icon=github&color=black&label
 [github_link]: https://github.com/NathanChen198/streamlit-ldap-authenticator
 [license_badge]: https://img.shields.io/badge/Licence-MIT-gr.svg
 [license_link]: https://github.com/NathanChen198/streamlit-ldap-authenticator/blob/main/LICENSE
```

