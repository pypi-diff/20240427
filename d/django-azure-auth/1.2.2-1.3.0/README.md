# Comparing `tmp/django_azure_auth-1.2.2.tar.gz` & `tmp/django_azure_auth-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_azure_auth-1.2.2.tar", max compression
+gzip compressed data, was "django_azure_auth-1.3.0.tar", max compression
```

## Comparing `django_azure_auth-1.2.2.tar` & `django_azure_auth-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1064 2024-04-23 08:03:57.407501 django_azure_auth-1.2.2/LICENSE
--rw-r--r--   0        0        0     5327 2024-04-23 08:03:57.407501 django_azure_auth-1.2.2/README.md
--rw-r--r--   0        0        0        0 2024-04-23 08:03:57.407501 django_azure_auth-1.2.2/azure_auth/__init__.py
--rw-r--r--   0        0        0      151 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/apps.py
--rw-r--r--   0        0        0      415 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/backends.py
--rw-r--r--   0        0        0      529 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/decorators.py
--rw-r--r--   0        0        0      333 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/exceptions.py
--rw-r--r--   0        0        0     6575 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/handlers.py
--rw-r--r--   0        0        0     1148 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/middleware.py
--rw-r--r--   0        0        0        0 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/tests/__init__.py
--rw-r--r--   0        0        0     2029 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/tests/conftest.py
--rw-r--r--   0        0        0     3943 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/tests/settings.py
--rw-r--r--   0        0        0     1409 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/tests/test_decorators.py
--rw-r--r--   0        0        0     1885 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/tests/test_middleware.py
--rw-r--r--   0        0        0    11498 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/tests/test_views.py
--rw-r--r--   0        0        0     1017 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/tests/urls.py
--rw-r--r--   0        0        0      324 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/urls.py
--rw-r--r--   0        0        0      732 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/views.py
--rw-r--r--   0        0        0     1464 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     6308 1970-01-01 00:00:00.000000 django_azure_auth-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-27 16:50:15.543754 django_azure_auth-1.3.0/LICENSE
+-rw-r--r--   0        0        0     5957 2024-04-27 16:50:15.543754 django_azure_auth-1.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-27 16:50:15.543754 django_azure_auth-1.3.0/azure_auth/__init__.py
+-rw-r--r--   0        0        0      151 2024-04-27 16:50:15.543754 django_azure_auth-1.3.0/azure_auth/apps.py
+-rw-r--r--   0        0        0      415 2024-04-27 16:50:15.543754 django_azure_auth-1.3.0/azure_auth/backends.py
+-rw-r--r--   0        0        0      529 2024-04-27 16:50:15.543754 django_azure_auth-1.3.0/azure_auth/decorators.py
+-rw-r--r--   0        0        0      333 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/exceptions.py
+-rw-r--r--   0        0        0     6773 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/handlers.py
+-rw-r--r--   0        0        0     1148 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/middleware.py
+-rw-r--r--   0        0        0        0 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/tests/__init__.py
+-rw-r--r--   0        0        0     2091 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/tests/conftest.py
+-rw-r--r--   0        0        0     3943 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/tests/settings.py
+-rw-r--r--   0        0        0     1409 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/tests/test_decorators.py
+-rw-r--r--   0        0        0     1885 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/tests/test_middleware.py
+-rw-r--r--   0        0        0    11869 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/tests/test_views.py
+-rw-r--r--   0        0        0     1017 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/tests/urls.py
+-rw-r--r--   0        0        0      324 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/urls.py
+-rw-r--r--   0        0        0      869 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/views.py
+-rw-r--r--   0        0        0     1464 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6938 1970-01-01 00:00:00.000000 django_azure_auth-1.3.0/PKG-INFO
```

### Comparing `django_azure_auth-1.2.2/LICENSE` & `django_azure_auth-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.2.2/README.md` & `django_azure_auth-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ![Build](https://github.com/Weird-Sheep-Labs/django-azure-auth/actions/workflows/ci.yml/badge.svg)
 ![Coverage Status](./reports/coverage/coverage-badge.svg?dummy=8484744)
 
-# Django Azure Auth
+# django-azure-auth
 
 ### A simple Django app for user authentication with Azure Active Directory/Entra ID.
 
-by Weird Sheep Labs
+by [Weird Sheep Labs](https://weirdsheeplabs.com)
 
-<a target="_blank" href="https://weirdsheeplabs.com"><img src="https://weirdsheeplabs.com/android-chrome-192x192.png" height="50" width="50" /></a>
+<a target="_blank" href="https://weirdsheeplabs.com"><img src="https://weirdsheeplabs.com/android-chrome-192x192.png" height="40" width="40" /></a>
 
 #### Naming update
 
 In March 2024, [Microsoft renamed Azure Active Directory (Azure AD) to Microsoft Entra ID](https://learn.microsoft.com/en-us/entra/fundamentals/new-name).
 
 ## Description
 
@@ -150,17 +150,25 @@
 ```
 
 If a user is assigned to one or more of this groups listed in the configuration, the user will be added
 automatically to the respective Django group. The group will be created if it does not exist.
 If a user is not part of a group (revoke permissions case), but is still in the Django group, the user
 will be removed from the Django group.
 
+## Bypass logout account selection
+
+During logout, if the ID token includes only the default claims, Active Directory will present the user with a page prompting them to select the account to log out. To disable this, simply enable the `login_hint` optional claim in your client application in Azure, as described in https://learn.microsoft.com/en-us/entra/identity-platform/v2-protocols-oidc#send-a-sign-out-request.
+
 ## Credits
 
 This app is heavily inspired by and builds on functionality in
 https://github.com/shubhamdipt/django-microsoft-authentication, with both feature
 improvements and code assurance through testing.
 
 Credit also to:
 
 - https://github.com/Azure-Samples/ms-identity-python-webapp
 - https://github.com/AzMoo/django-okta-auth
+
+<div align="center">
+    <a target="_blank" href="https://weirdsheeplabs.com"><img src="https://weirdsheeplabs.com/android-chrome-192x192.png" height="50" width="50" /></a>
+</div>
```

### Comparing `django_azure_auth-1.2.2/azure_auth/decorators.py` & `django_azure_auth-1.3.0/azure_auth/decorators.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.2.2/azure_auth/handlers.py` & `django_azure_auth-1.3.0/azure_auth/handlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from http import HTTPStatus
 from typing import cast
+from urllib import parse
 
 import msal
 import requests
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import AbstractBaseUser, Group
 from django.http import HttpRequest
@@ -25,14 +26,17 @@
         """
         self.request = request
         self.graph_user_endpoint = "https://graph.microsoft.com/v1.0/me"
         self.auth_flow_session_key = "auth_flow"
         self._cache = msal.SerializableTokenCache()
         self._msal_app = None
 
+        # Eagerly load the claims from the session
+        self.claims = self.request.session.get("id_token_claims", {})
+
     def get_auth_uri(self) -> str:
         """
         Requests the auth flow dictionary and stores it on the session to be
         queried later in the auth process.
 
         :return: Authentication redirect URI
         """
@@ -115,29 +119,28 @@
                 else:
                     # No permission so check if user is in group and remove
                     if user.groups.filter(name=group_name).exists():
                         user.groups.remove(django_group)
 
         return user
 
-    @staticmethod
-    def get_logout_uri() -> str:
+    def get_logout_uri(self) -> str:
         """
         Forms the URI to log the user out in the Active Directory app and
         redirect to the webapp logout page.
 
         :return: Active Directory app logout URI
         """
         authority = settings.AZURE_AUTH["AUTHORITY"]
-        logout_uri = settings.AZURE_AUTH.get("LOGOUT_URI", "")
-        if logout_uri:
-            return (
-                f"{authority}/oauth2/v2.0/logout?post_logout_redirect_uri={logout_uri}"
-            )
-        return f"{authority}/oauth2/v2.0/logout"
+        _query_params = {
+            "post_logout_redirect_uri": settings.AZURE_AUTH.get("LOGOUT_URI"),
+            "logout_hint": self.claims.get("login_hint"),
+        }
+        query_params = {k: v for k, v in _query_params.items() if v}
+        return f"{authority}/oauth2/v2.0/logout?{parse.urlencode(query_params)}"
 
     @property
     def msal_app(self):
         if self._msal_app is None:
             self._msal_app = msal.ConfidentialClientApplication(
                 client_id=settings.AZURE_AUTH["CLIENT_ID"],
                 client_credential=settings.AZURE_AUTH["CLIENT_SECRET"],
```

### Comparing `django_azure_auth-1.2.2/azure_auth/middleware.py` & `django_azure_auth-1.3.0/azure_auth/middleware.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.2.2/azure_auth/tests/conftest.py` & `django_azure_auth-1.3.0/azure_auth/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,13 +56,14 @@
             "preferred_username": "dummy_id_token_claims_preferred_username",
             "rh": "dummy_id_token_claims_rh",
             "sub": "dummy_id_token_claims_sub",
             "tid": "dummy_id_token_claims_tid",
             "uti": "dummy_id_token_claims_uti",
             "ver": "2.0",
             "roles": ["95170e67-2bbf-4e3e-a4d7-e7e5829fe7a7"],
+            "login_hint": "dummy_id_token_claims_login_hint",
         },
     }
 
     if request.cls:
         request.cls.token = _token
     return _token
```

### Comparing `django_azure_auth-1.2.2/azure_auth/tests/settings.py` & `django_azure_auth-1.3.0/azure_auth/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.2.2/azure_auth/tests/test_decorators.py` & `django_azure_auth-1.3.0/azure_auth/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.2.2/azure_auth/tests/test_middleware.py` & `django_azure_auth-1.3.0/azure_auth/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.2.2/azure_auth/tests/test_views.py` & `django_azure_auth-1.3.0/azure_auth/tests/test_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,46 +236,58 @@
         self.user.is_active = False  # type: ignore
         self.user.save()  # type: ignore
         resp = self.client.get(reverse("azure_auth:callback"))
         assert resp.status_code == HTTPStatus.FORBIDDEN
         assert resp.content.decode() == "Invalid email for this app."
 
 
-@patch.object(msal, "ConfidentialClientApplication")
+@pytest.mark.usefixtures("token")
 class TestLogoutView(TestCase):
     # No redirect logout
-    no_redirect_logout_settings = copy.deepcopy(settings.AZURE_AUTH)
-    del no_redirect_logout_settings["LOGOUT_URI"]
+    no_logout_query_params_settings = copy.deepcopy(settings.AZURE_AUTH)
+    del no_logout_query_params_settings["LOGOUT_URI"]
 
     def setUp(self):
         super().setUp()
         self.client.force_login(self.user)  # type: ignore
 
-    def test_logout_with_redirect(self, *args):
+        # Token will be on the session
+        session = self.client.session
+        session["id_token_claims"] = self.token["id_token_claims"]  # type: ignore
+        session.save()
+
+    def test_logout_with_query_params(self):
         # Check user has been correctly logged in
         assert all(
             [
                 key in self.client.session
-                for key in ["_auth_user_id", "_auth_user_backend", "_auth_user_hash"]
+                for key in [
+                    "_auth_user_id",
+                    "_auth_user_backend",
+                    "_auth_user_hash",
+                ]
             ]
         )
         resp = self.client.get(reverse("azure_auth:logout"))
         assert resp.status_code == HTTPStatus.FOUND
         assert (
             resp.url == f"{settings.AZURE_AUTH['AUTHORITY']}/oauth2/v2.0/logout"  # type: ignore
-            f"?post_logout_redirect_uri={settings.AZURE_AUTH['LOGOUT_URI']}"
+            f"?post_logout_redirect_uri=http%3A%2F%2Fmydomain%2Flogout&logout_hint=dummy_id_token_claims_login_hint"
         )
         assert not self.client.session.keys()
 
-    @override_settings(AZURE_AUTH=no_redirect_logout_settings)
-    def test_logout_without_redirect(self, *args):
+    @override_settings(AZURE_AUTH=no_logout_query_params_settings)
+    def test_logout_without_query_params(self):
         # Check user has been correctly logged in
         assert all(
             [
                 key in self.client.session
                 for key in ["_auth_user_id", "_auth_user_backend", "_auth_user_hash"]
             ]
         )
         resp = self.client.get(reverse("azure_auth:logout"))
         assert resp.status_code == HTTPStatus.FOUND
-        assert resp.url == f"{settings.AZURE_AUTH['AUTHORITY']}/oauth2/v2.0/logout"  # type: ignore
+        assert (
+            resp.url  # type: ignore
+            == f"{settings.AZURE_AUTH['AUTHORITY']}/oauth2/v2.0/logout?logout_hint=dummy_id_token_claims_login_hint"
+        )
         assert not self.client.session.keys()
```

### Comparing `django_azure_auth-1.2.2/azure_auth/tests/urls.py` & `django_azure_auth-1.3.0/azure_auth/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.2.2/pyproject.toml` & `django_azure_auth-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-azure-auth"
-version = "1.2.2"
+version = "1.3.0"
 description = "A simple Django app for user authentication with Azure Active Directory/Entra ID."
 authors = ["Weird Sheep Labs <info@weirdsheeplabs.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Weird-Sheep-Labs/django-azure-auth"
 keywords = ['django', 'azure', 'authentication', 'microsoft', 'entra']
 classifiers = [
```

### Comparing `django_azure_auth-1.2.2/PKG-INFO` & `django_azure_auth-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-azure-auth
-Version: 1.2.2
+Version: 1.3.0
 Summary: A simple Django app for user authentication with Azure Active Directory/Entra ID.
 Home-page: https://github.com/Weird-Sheep-Labs/django-azure-auth
 License: MIT
 Keywords: django,azure,authentication,microsoft,entra
 Author: Weird Sheep Labs
 Author-email: info@weirdsheeplabs.com
 Requires-Python: >=3.8,<4.0
@@ -21,21 +21,21 @@
 Requires-Dist: Django (>=3.2)
 Requires-Dist: msal (>=1.18.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 ![Build](https://github.com/Weird-Sheep-Labs/django-azure-auth/actions/workflows/ci.yml/badge.svg)
 ![Coverage Status](./reports/coverage/coverage-badge.svg?dummy=8484744)
 
-# Django Azure Auth
+# django-azure-auth
 
 ### A simple Django app for user authentication with Azure Active Directory/Entra ID.
 
-by Weird Sheep Labs
+by [Weird Sheep Labs](https://weirdsheeplabs.com)
 
-<a target="_blank" href="https://weirdsheeplabs.com"><img src="https://weirdsheeplabs.com/android-chrome-192x192.png" height="50" width="50" /></a>
+<a target="_blank" href="https://weirdsheeplabs.com"><img src="https://weirdsheeplabs.com/android-chrome-192x192.png" height="40" width="40" /></a>
 
 #### Naming update
 
 In March 2024, [Microsoft renamed Azure Active Directory (Azure AD) to Microsoft Entra ID](https://learn.microsoft.com/en-us/entra/fundamentals/new-name).
 
 ## Description
 
@@ -174,18 +174,26 @@
 ```
 
 If a user is assigned to one or more of this groups listed in the configuration, the user will be added
 automatically to the respective Django group. The group will be created if it does not exist.
 If a user is not part of a group (revoke permissions case), but is still in the Django group, the user
 will be removed from the Django group.
 
+## Bypass logout account selection
+
+During logout, if the ID token includes only the default claims, Active Directory will present the user with a page prompting them to select the account to log out. To disable this, simply enable the `login_hint` optional claim in your client application in Azure, as described in https://learn.microsoft.com/en-us/entra/identity-platform/v2-protocols-oidc#send-a-sign-out-request.
+
 ## Credits
 
 This app is heavily inspired by and builds on functionality in
 https://github.com/shubhamdipt/django-microsoft-authentication, with both feature
 improvements and code assurance through testing.
 
 Credit also to:
 
 - https://github.com/Azure-Samples/ms-identity-python-webapp
 - https://github.com/AzMoo/django-okta-auth
 
+<div align="center">
+    <a target="_blank" href="https://weirdsheeplabs.com"><img src="https://weirdsheeplabs.com/android-chrome-192x192.png" height="50" width="50" /></a>
+</div>
+
```

