# Comparing `tmp/py4web-1.20240420.3.tar.gz` & `tmp/py4web-1.20240427.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4web-1.20240420.3.tar", last modified: Sat Apr 20 19:26:36 2024, max compression
+gzip compressed data, was "py4web-1.20240427.1.tar", last modified: Sat Apr 27 07:48:22 2024, max compression
```

## Comparing `py4web-1.20240420.3.tar` & `py4web-1.20240427.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-20 19:26:36.248291 py4web-1.20240420.3/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20240420.3/LICENSE.md
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7746 2024-04-20 19:26:36.248291 py4web-1.20240420.3/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7174 2024-04-19 07:21:20.000000 py4web-1.20240420.3/README.rst
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-20 19:26:36.214956 py4web-1.20240420.3/py4web/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      752 2024-04-20 19:25:52.000000 py4web-1.20240420.3/py4web/__init__.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-20 19:26:36.234957 py4web-1.20240420.3/py4web/assets/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  2990688 2024-04-20 19:26:28.000000 py4web-1.20240420.3/py4web/assets/py4web.app._dashboard.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   187155 2024-04-20 19:26:28.000000 py4web-1.20240420.3/py4web/assets/py4web.app._default.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  4406167 2024-04-20 19:26:28.000000 py4web-1.20240420.3/py4web/assets/py4web.app._documentation.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5245 2024-04-20 19:26:28.000000 py4web-1.20240420.3/py4web/assets/py4web.app._minimal.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    21723 2024-04-20 19:26:28.000000 py4web-1.20240420.3/py4web/assets/py4web.app._scaffold.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  1392768 2024-04-20 19:26:29.000000 py4web-1.20240420.3/py4web/assets/py4web.app.showcase.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    68412 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/core.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    20383 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/server_adapters.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-20 19:26:36.241624 py4web-1.20240420.3/py4web/utils/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20240420.3/py4web/utils/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    72493 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/auth.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-20 19:26:36.244957 py4web-1.20240420.3/py4web/utils/auth_plugins/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6443 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/auth_plugins/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      797 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/auth_plugins/basic_auth_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1480 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/auth_plugins/email_auth_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35452 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/auth_plugins/ldap_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20240420.3/py4web/utils/auth_plugins/oauth2discord.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      670 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/auth_plugins/oauth2facebook.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      474 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/auth_plugins/oauth2github.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20240420.3/py4web/utils/auth_plugins/oauth2google.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    11958 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/auth_plugins/oauth2google_scoped.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20240420.3/py4web/utils/auth_plugins/oauth2okta.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2079 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/auth_plugins/oauth2server.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6091 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/auth_plugins/oauth2wpminiorange.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5082 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/auth_plugins/pam.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20240420.3/py4web/utils/auth_plugins/pam_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6620 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/auth_plugins/saml2_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2811 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/auth_plugins/x509_auth_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20240420.3/py4web/utils/cors.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1628 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/dbstore.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2102 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/downloader.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3097 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/factories.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35880 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/form.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    69698 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/grid.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1629 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/jsonrpc.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    34797 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/mailer.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9181 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/misc.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20240420.3/py4web/utils/param.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    18284 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/populate.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1602 2024-04-20 18:27:18.000000 py4web-1.20240420.3/py4web/utils/publisher.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2425 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/recaptcha.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3712 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/security.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      124 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/tags.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6578 2024-04-20 18:21:20.000000 py4web-1.20240420.3/py4web/utils/url_signer.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-20 19:26:36.218290 py4web-1.20240420.3/py4web.egg-info/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7746 2024-04-20 19:26:36.000000 py4web-1.20240420.3/py4web.egg-info/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1896 2024-04-20 19:26:36.000000 py4web-1.20240420.3/py4web.egg-info/SOURCES.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-04-20 19:26:36.000000 py4web-1.20240420.3/py4web.egg-info/dependency_links.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       43 2024-04-20 19:26:36.000000 py4web-1.20240420.3/py4web.egg-info/entry_points.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      237 2024-04-20 19:26:36.000000 py4web-1.20240420.3/py4web.egg-info/requires.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        7 2024-04-20 19:26:36.000000 py4web-1.20240420.3/py4web.egg-info/top_level.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      843 2024-04-20 19:26:01.000000 py4web-1.20240420.3/pyproject.toml
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      462 2024-04-20 18:21:20.000000 py4web-1.20240420.3/requirements.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       38 2024-04-20 19:26:36.248291 py4web-1.20240420.3/setup.cfg
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-20 19:26:36.248291 py4web-1.20240420.3/tests/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3462 2023-11-14 06:31:07.000000 py4web-1.20240420.3/tests/test_action.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8508 2023-05-08 00:39:45.000000 py4web-1.20240420.3/tests/test_auth.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2025 2023-05-08 00:39:45.000000 py4web-1.20240420.3/tests/test_cache.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1619 2023-05-08 00:39:45.000000 py4web-1.20240420.3/tests/test_fixture.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20240420.3/tests/test_form.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      634 2023-05-08 00:39:45.000000 py4web-1.20240420.3/tests/test_get_error_snapshot.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1043 2023-05-08 00:39:45.000000 py4web-1.20240420.3/tests/test_json.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      847 2023-05-08 00:39:45.000000 py4web-1.20240420.3/tests/test_main.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4545 2023-05-08 00:39:45.000000 py4web-1.20240420.3/tests/test_session.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      989 2023-05-08 00:39:45.000000 py4web-1.20240420.3/tests/test_tags.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      396 2023-05-08 00:39:45.000000 py4web-1.20240420.3/tests/test_template.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      440 2024-04-07 06:47:57.000000 py4web-1.20240420.3/tests/test_url.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:48:22.785186 py4web-1.20240427.1/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20240427.1/LICENSE.md
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7746 2024-04-27 07:48:22.781853 py4web-1.20240427.1/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7174 2024-04-19 07:21:20.000000 py4web-1.20240427.1/README.rst
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:48:22.745185 py4web-1.20240427.1/py4web/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      752 2024-04-27 07:08:14.000000 py4web-1.20240427.1/py4web/__init__.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:48:22.768519 py4web-1.20240427.1/py4web/assets/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  2990688 2024-04-27 07:48:14.000000 py4web-1.20240427.1/py4web/assets/py4web.app._dashboard.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   187155 2024-04-27 07:48:14.000000 py4web-1.20240427.1/py4web/assets/py4web.app._default.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  4406167 2024-04-27 07:48:15.000000 py4web-1.20240427.1/py4web/assets/py4web.app._documentation.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5245 2024-04-27 07:48:14.000000 py4web-1.20240427.1/py4web/assets/py4web.app._minimal.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    21723 2024-04-27 07:48:14.000000 py4web-1.20240427.1/py4web/assets/py4web.app._scaffold.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  1392768 2024-04-27 07:48:15.000000 py4web-1.20240427.1/py4web/assets/py4web.app.showcase.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    68412 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/core.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    20383 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/server_adapters.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:48:22.775186 py4web-1.20240427.1/py4web/utils/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20240427.1/py4web/utils/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    72606 2024-04-27 07:41:15.000000 py4web-1.20240427.1/py4web/utils/auth.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:48:22.778519 py4web-1.20240427.1/py4web/utils/auth_plugins/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6440 2024-04-22 01:47:37.000000 py4web-1.20240427.1/py4web/utils/auth_plugins/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      797 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/auth_plugins/basic_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1480 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/auth_plugins/email_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35452 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/auth_plugins/ldap_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20240427.1/py4web/utils/auth_plugins/oauth2discord.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      670 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/auth_plugins/oauth2facebook.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      474 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/auth_plugins/oauth2github.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20240427.1/py4web/utils/auth_plugins/oauth2google.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    11958 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/auth_plugins/oauth2google_scoped.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20240427.1/py4web/utils/auth_plugins/oauth2okta.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2079 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/auth_plugins/oauth2server.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6091 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/auth_plugins/oauth2wpminiorange.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5082 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/auth_plugins/pam.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20240427.1/py4web/utils/auth_plugins/pam_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6620 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/auth_plugins/saml2_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2811 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/auth_plugins/x509_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20240427.1/py4web/utils/cors.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1628 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/dbstore.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2102 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/downloader.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3097 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/factories.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35880 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/form.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    69698 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/grid.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1629 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/jsonrpc.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    34797 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/mailer.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9181 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/misc.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20240427.1/py4web/utils/param.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    18284 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/populate.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1602 2024-04-20 18:27:18.000000 py4web-1.20240427.1/py4web/utils/publisher.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2425 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/recaptcha.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3712 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/security.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      124 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/tags.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6578 2024-04-20 18:21:20.000000 py4web-1.20240427.1/py4web/utils/url_signer.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:48:22.748519 py4web-1.20240427.1/py4web.egg-info/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7746 2024-04-27 07:48:22.000000 py4web-1.20240427.1/py4web.egg-info/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1896 2024-04-27 07:48:22.000000 py4web-1.20240427.1/py4web.egg-info/SOURCES.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-04-27 07:48:22.000000 py4web-1.20240427.1/py4web.egg-info/dependency_links.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       43 2024-04-27 07:48:22.000000 py4web-1.20240427.1/py4web.egg-info/entry_points.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      237 2024-04-27 07:48:22.000000 py4web-1.20240427.1/py4web.egg-info/requires.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        7 2024-04-27 07:48:22.000000 py4web-1.20240427.1/py4web.egg-info/top_level.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      843 2024-04-27 07:07:56.000000 py4web-1.20240427.1/pyproject.toml
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      462 2024-04-27 07:19:53.000000 py4web-1.20240427.1/requirements.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       38 2024-04-27 07:48:22.785186 py4web-1.20240427.1/setup.cfg
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:48:22.781853 py4web-1.20240427.1/tests/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3462 2023-11-14 06:31:07.000000 py4web-1.20240427.1/tests/test_action.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8102 2024-04-27 07:45:55.000000 py4web-1.20240427.1/tests/test_auth.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2025 2023-05-08 00:39:45.000000 py4web-1.20240427.1/tests/test_cache.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1619 2023-05-08 00:39:45.000000 py4web-1.20240427.1/tests/test_fixture.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20240427.1/tests/test_form.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      634 2023-05-08 00:39:45.000000 py4web-1.20240427.1/tests/test_get_error_snapshot.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1043 2023-05-08 00:39:45.000000 py4web-1.20240427.1/tests/test_json.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      847 2023-05-08 00:39:45.000000 py4web-1.20240427.1/tests/test_main.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4545 2023-05-08 00:39:45.000000 py4web-1.20240427.1/tests/test_session.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      989 2023-05-08 00:39:45.000000 py4web-1.20240427.1/tests/test_tags.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      396 2023-05-08 00:39:45.000000 py4web-1.20240427.1/tests/test_template.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      440 2024-04-07 06:47:57.000000 py4web-1.20240427.1/tests/test_url.py
```

### Comparing `py4web-1.20240420.3/LICENSE.md` & `py4web-1.20240427.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/PKG-INFO` & `py4web-1.20240427.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20240420.3
+Version: 1.20240427.1
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `py4web-1.20240420.3/README.rst` & `py4web-1.20240427.1/README.rst`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/__init__.py` & `py4web-1.20240427.1/py4web/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 __author__ = "Massimo Di Pierro <massimo.dipierro@gmail.com>"
 __license__ = "BSD-3-Clause"
-__version__ = "1.20240420.3"
+__version__ = "1.20240427.1"
 
 
 def _maybe_gevent():
     for arg in sys.argv[1:]:
         if "gevent" in arg.lower():
             from gevent import monkey
```

### Comparing `py4web-1.20240420.3/py4web/assets/py4web.app._dashboard.zip` & `py4web-1.20240427.1/py4web/assets/py4web.app._dashboard.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/assets/py4web.app._default.zip` & `py4web-1.20240427.1/py4web/assets/py4web.app._default.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/assets/py4web.app._documentation.zip` & `py4web-1.20240427.1/py4web/assets/py4web.app._documentation.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/assets/py4web.app._minimal.zip` & `py4web-1.20240427.1/py4web/assets/py4web.app._minimal.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/assets/py4web.app._scaffold.zip` & `py4web-1.20240427.1/py4web/assets/py4web.app._scaffold.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/assets/py4web.app.showcase.zip` & `py4web-1.20240427.1/py4web/assets/py4web.app.showcase.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/core.py` & `py4web-1.20240427.1/py4web/core.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/server_adapters.py` & `py4web-1.20240427.1/py4web/server_adapters.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/auth.py` & `py4web-1.20240427.1/py4web/utils/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -581,17 +581,18 @@
 
     def register(self, fields, send=True, next="", validate=True, route=None):
         """Registers a new user after the user's parameters are entered
         in the SignUp form"""
         if self.use_username:
             fields["username"] = fields.get("username", "").lower()
         fields["email"] = fields.get("email", "").lower()
-
+        self.db.auth_user.action_token.writable = True
         def store(fields):
             if validate:
+                self.db.auth_user.password.writable = True
                 return self.db.auth_user.validate_and_insert(**fields)
             return dict(id=self.db.auth_user.insert(**fields))
 
         if self.param.registration_requires_confirmation:
             token = str(uuid.uuid4())
             if next:
                 token += "/" + b16e(next)
```

### Comparing `py4web-1.20240420.3/py4web/utils/auth_plugins/__init__.py` & `py4web-1.20240427.1/py4web/utils/auth_plugins/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,26 +58,26 @@
             if isinstance(error, str):
                 code, msg = 401, error
             else:
                 code = error.get("code", 401)
                 msg = error.get("message", "Unknown error")
             raise HTTP(code, msg)
         if auth.db:
+            print(data)
             # map returned fields into auth_user fields
             user = {}
             for key, orig_key in self.maps.items():
                 value = data
                 parts = orig_key.split(".")
-                for part in parts:
-                    try:
+                try:
+                    for part in parts:
                         value = value[int(part) if part.isdigit() else part]
-                    except Exception:
-                        break
-                else:
                     user[key] = value
+                except Exception:
+                    continue
             user["sso_id"] = "%s:%s" % (self.name, user["sso_id"])
             if "username" not in user:
                 user["username"] = user["sso_id"]
             # store or retrieve the user
             data = auth.get_or_register_user(user)
             user_id = data["id"]
         else:
```

### Comparing `py4web-1.20240420.3/py4web/utils/auth_plugins/basic_auth_plugin.py` & `py4web-1.20240427.1/py4web/utils/auth_plugins/basic_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/auth_plugins/email_auth_plugin.py` & `py4web-1.20240427.1/py4web/utils/auth_plugins/email_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/auth_plugins/ldap_plugin.py` & `py4web-1.20240427.1/py4web/utils/auth_plugins/ldap_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/auth_plugins/oauth2discord.py` & `py4web-1.20240427.1/py4web/utils/auth_plugins/oauth2discord.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/auth_plugins/oauth2facebook.py` & `py4web-1.20240427.1/py4web/utils/auth_plugins/oauth2facebook.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/auth_plugins/oauth2google.py` & `py4web-1.20240427.1/py4web/utils/auth_plugins/oauth2google.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/auth_plugins/oauth2google_scoped.py` & `py4web-1.20240427.1/py4web/utils/auth_plugins/oauth2google_scoped.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/auth_plugins/oauth2server.py` & `py4web-1.20240427.1/py4web/utils/auth_plugins/oauth2server.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/auth_plugins/oauth2wpminiorange.py` & `py4web-1.20240427.1/py4web/utils/auth_plugins/oauth2wpminiorange.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/auth_plugins/pam.py` & `py4web-1.20240427.1/py4web/utils/auth_plugins/pam.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/auth_plugins/saml2_plugin.py` & `py4web-1.20240427.1/py4web/utils/auth_plugins/saml2_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/auth_plugins/x509_auth_plugin.py` & `py4web-1.20240427.1/py4web/utils/auth_plugins/x509_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/cors.py` & `py4web-1.20240427.1/py4web/utils/cors.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/dbstore.py` & `py4web-1.20240427.1/py4web/utils/dbstore.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/downloader.py` & `py4web-1.20240427.1/py4web/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/factories.py` & `py4web-1.20240427.1/py4web/utils/factories.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/form.py` & `py4web-1.20240427.1/py4web/utils/form.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/grid.py` & `py4web-1.20240427.1/py4web/utils/grid.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/jsonrpc.py` & `py4web-1.20240427.1/py4web/utils/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/mailer.py` & `py4web-1.20240427.1/py4web/utils/mailer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/misc.py` & `py4web-1.20240427.1/py4web/utils/misc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/populate.py` & `py4web-1.20240427.1/py4web/utils/populate.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/publisher.py` & `py4web-1.20240427.1/py4web/utils/publisher.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/recaptcha.py` & `py4web-1.20240427.1/py4web/utils/recaptcha.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/security.py` & `py4web-1.20240427.1/py4web/utils/security.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web/utils/url_signer.py` & `py4web-1.20240427.1/py4web/utils/url_signer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/py4web.egg-info/PKG-INFO` & `py4web-1.20240427.1/py4web.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20240420.3
+Version: 1.20240427.1
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `py4web-1.20240420.3/py4web.egg-info/SOURCES.txt` & `py4web-1.20240427.1/py4web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/pyproject.toml` & `py4web-1.20240427.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "py4web"
-version = "1.20240420.3"
+version = "1.20240427.1"
 authors = [{ name="Massimo Di Pierro", email="massimo.dipierro@gmail.com" },]
 description = "A fast, stable, comprehensive web framework"
 readme = "README.rst"
 requires-python = ">=3.7"
 classifiers = [
       "Programming Language :: Python :: 3",
       "License :: OSI Approved :: BSD License",
```

### Comparing `py4web-1.20240420.3/tests/test_action.py` & `py4web-1.20240427.1/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/tests/test_auth.py` & `py4web-1.20240427.1/tests/test_auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                 "status": "error",
                 "message": "validation errors",
                 "code": 401,
             },
         )
 
     def test_register(self):
-        self.on_request()
+        self.on_request()        
         body = {
             "username": "ppallino",
             "email": "pinco.pallino@example.com",
             "password": "123456789",
             "first_name": "Pinco",
             "last_name": "Pallino",
         }
@@ -221,26 +221,14 @@
         body = {"password": "432187659", "new_email": "somebody@example.com"}
         self.assertEqual(
             self.auth.action("api/change_email", "POST", {}, body),
             {"updated": 1, "status": "success", "code": 200},
         )
 
         self.on_request(keep_session=True)
-        body = {"first_name": "Max", "last_name": "Powers", "password": "xyz"}
-        self.assertEqual(
-            self.auth.action("api/profile", "POST", {}, body),
-            {
-                "errors": {"password": "invalid"},
-                "status": "error",
-                "message": "validation errors",
-                "code": 401,
-            },
-        )
-
-        self.on_request(keep_session=True)
         body = {"first_name": "Max", "last_name": "Powers"}
         self.assertEqual(
             self.auth.action("api/profile", "POST", {}, body),
             {"updated": 1, "status": "success", "code": 200},
         )
```

### Comparing `py4web-1.20240420.3/tests/test_cache.py` & `py4web-1.20240427.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/tests/test_fixture.py` & `py4web-1.20240427.1/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/tests/test_form.py` & `py4web-1.20240427.1/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/tests/test_get_error_snapshot.py` & `py4web-1.20240427.1/tests/test_get_error_snapshot.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/tests/test_json.py` & `py4web-1.20240427.1/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/tests/test_main.py` & `py4web-1.20240427.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/tests/test_session.py` & `py4web-1.20240427.1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240420.3/tests/test_tags.py` & `py4web-1.20240427.1/tests/test_tags.py`

 * *Files identical despite different names*

