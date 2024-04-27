# Comparing `tmp/tcms-api-8.6.0.tar.gz` & `tmp/tcms-api-9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tcms-api-8.6.0.tar", last modified: Wed Oct 28 17:58:22 2020, max compression
+gzip compressed data, was "dist/tcms-api-9.0.tar", last modified: Tue Jan 12 11:55:13 2021, max compression
```

## Comparing `tcms-api-8.6.0.tar` & `tcms-api-9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 senko     (1002) senko     (1002)        0 2020-10-28 17:58:22.000000 tcms-api-8.6.0/
-drwxrwxr-x   0 senko     (1002) senko     (1002)        0 2020-10-28 17:58:22.000000 tcms-api-8.6.0/tcms_api/
--rw-rw-r--   0 senko     (1002) senko     (1002)     4427 2020-10-28 12:12:15.000000 tcms-api-8.6.0/tcms_api/__init__.py
--rw-rw-r--   0 senko     (1002) senko     (1002)    19621 2020-06-25 19:32:51.000000 tcms-api-8.6.0/tcms_api/plugin_helpers.py
--rw-rw-r--   0 senko     (1002) senko     (1002)       22 2020-10-28 17:55:47.000000 tcms-api-8.6.0/tcms_api/version.py
--rw-rw-r--   0 senko     (1002) senko     (1002)     5466 2020-10-28 17:54:53.000000 tcms-api-8.6.0/tcms_api/xmlrpc.py
-drwxrwxr-x   0 senko     (1002) senko     (1002)        0 2020-10-28 17:58:22.000000 tcms-api-8.6.0/tcms_api.egg-info/
--rw-rw-r--   0 senko     (1002) senko     (1002)     8423 2020-10-28 17:58:22.000000 tcms-api-8.6.0/tcms_api.egg-info/PKG-INFO
--rw-rw-r--   0 senko     (1002) senko     (1002)      302 2020-10-28 17:58:22.000000 tcms-api-8.6.0/tcms_api.egg-info/SOURCES.txt
--rw-rw-r--   0 senko     (1002) senko     (1002)        1 2020-10-28 17:58:22.000000 tcms-api-8.6.0/tcms_api.egg-info/dependency_links.txt
--rw-rw-r--   0 senko     (1002) senko     (1002)       26 2020-10-28 17:58:22.000000 tcms-api-8.6.0/tcms_api.egg-info/requires.txt
--rw-rw-r--   0 senko     (1002) senko     (1002)        9 2020-10-28 17:58:22.000000 tcms-api-8.6.0/tcms_api.egg-info/top_level.txt
--rw-rw-r--   0 senko     (1002) senko     (1002)    24484 2020-03-22 00:18:50.000000 tcms-api-8.6.0/LICENSE
--rw-rw-r--   0 senko     (1002) senko     (1002)       44 2020-04-10 10:48:58.000000 tcms-api-8.6.0/MANIFEST.in
--rw-rw-r--   0 senko     (1002) senko     (1002)     5993 2020-10-28 17:57:07.000000 tcms-api-8.6.0/README.rst
--rw-rw-r--   0 senko     (1002) senko     (1002)        9 2020-10-28 17:54:53.000000 tcms-api-8.6.0/requirements.txt
--rw-rw-r--   0 senko     (1002) senko     (1002)     1800 2020-10-28 17:54:53.000000 tcms-api-8.6.0/setup.py
--rw-rw-r--   0 senko     (1002) senko     (1002)     8423 2020-10-28 17:58:22.000000 tcms-api-8.6.0/PKG-INFO
--rw-rw-r--   0 senko     (1002) senko     (1002)       38 2020-10-28 17:58:22.000000 tcms-api-8.6.0/setup.cfg
+drwxrwxr-x   0 senko     (1002) senko     (1002)        0 2021-01-12 11:55:13.000000 tcms-api-9.0/
+drwxrwxr-x   0 senko     (1002) senko     (1002)        0 2021-01-12 11:55:13.000000 tcms-api-9.0/tcms_api/
+-rw-rw-r--   0 senko     (1002) senko     (1002)     4427 2020-10-28 12:12:15.000000 tcms-api-9.0/tcms_api/__init__.py
+-rw-rw-r--   0 senko     (1002) senko     (1002)    19318 2021-01-12 11:54:56.000000 tcms-api-9.0/tcms_api/plugin_helpers.py
+-rw-rw-r--   0 senko     (1002) senko     (1002)       20 2021-01-12 11:54:56.000000 tcms-api-9.0/tcms_api/version.py
+-rw-rw-r--   0 senko     (1002) senko     (1002)     5466 2020-10-28 17:54:53.000000 tcms-api-9.0/tcms_api/xmlrpc.py
+drwxrwxr-x   0 senko     (1002) senko     (1002)        0 2021-01-12 11:55:13.000000 tcms-api-9.0/tcms_api.egg-info/
+-rw-rw-r--   0 senko     (1002) senko     (1002)     8773 2021-01-12 11:55:13.000000 tcms-api-9.0/tcms_api.egg-info/PKG-INFO
+-rw-rw-r--   0 senko     (1002) senko     (1002)      302 2021-01-12 11:55:13.000000 tcms-api-9.0/tcms_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 senko     (1002) senko     (1002)        1 2021-01-12 11:55:13.000000 tcms-api-9.0/tcms_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 senko     (1002) senko     (1002)       26 2021-01-12 11:55:13.000000 tcms-api-9.0/tcms_api.egg-info/requires.txt
+-rw-rw-r--   0 senko     (1002) senko     (1002)        9 2021-01-12 11:55:13.000000 tcms-api-9.0/tcms_api.egg-info/top_level.txt
+-rw-rw-r--   0 senko     (1002) senko     (1002)    24484 2020-03-22 00:18:50.000000 tcms-api-9.0/LICENSE
+-rw-rw-r--   0 senko     (1002) senko     (1002)       44 2020-04-10 10:48:58.000000 tcms-api-9.0/MANIFEST.in
+-rw-rw-r--   0 senko     (1002) senko     (1002)     6317 2021-01-12 11:54:56.000000 tcms-api-9.0/README.rst
+-rw-rw-r--   0 senko     (1002) senko     (1002)        9 2020-10-28 17:54:53.000000 tcms-api-9.0/requirements.txt
+-rw-rw-r--   0 senko     (1002) senko     (1002)     1800 2020-10-28 17:54:53.000000 tcms-api-9.0/setup.py
+-rw-rw-r--   0 senko     (1002) senko     (1002)     8773 2021-01-12 11:55:13.000000 tcms-api-9.0/PKG-INFO
+-rw-rw-r--   0 senko     (1002) senko     (1002)       59 2021-01-12 11:55:13.000000 tcms-api-9.0/setup.cfg
```

### Comparing `tcms-api-8.6.0/tcms_api/__init__.py` & `tcms-api-9.0/tcms_api/__init__.py`

 * *Files identical despite different names*

### Comparing `tcms-api-8.6.0/tcms_api/plugin_helpers.py` & `tcms-api-9.0/tcms_api/plugin_helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2019 Alexander Todorov <atodorov@MrSenko.com>
+# Copyright (c) 2019-2021 Alexander Todorov <atodorov@MrSenko.com>
 
 import os
 from datetime import datetime
 
 from . import TCMS
 
 
@@ -226,59 +226,51 @@
                                            'value': version_val})
         if not version:
             version = [self.rpc.Version.create({'product': product_id,
                                                 'value': version_val})]
 
         return version[0]['id'], version_val
 
-    def get_build_id(self, product_id, _version_id):
+    def get_build_id(self, version_id):
         """
             Return a ``tcms.management.models.Build`` (PK, name).
 
             .. warning::
 
                 For internal use by `.configure()`!
 
-            :param product_id: ``tcms.management.models.Product`` PK
-                               for which to look for Build
-            :type product_id: int
             :param version_id: ``tcms.management.models.Version`` PK
                                for which to look for Build
             :type version_id: int
             :return: (build_id, build_name)
             :rtype: tuple(int, str)
 
             Order of precedence:
 
             - use `$TCMS_BUILD` as Build.name if specified, otherwise
             - use `$TRAVIS_BUILD_NUMBER` as Build.name if specified, otherwise
             - use `$BUILD_NUMBER` as Build.name if specified
 
             If Build doesn't exist in the database it will be created with the
-            specified `product_id`!
-
-            .. note::
-
-                For `version_id` see
-                https://github.com/kiwitcms/Kiwi/issues/246
+            specified `version_id`!
         """
         build_number = os.environ.get('TCMS_BUILD',
                                       os.environ.get('TRAVIS_BUILD_NUMBER',
                                                      os.environ.get(
                                                          'BUILD_NUMBER')))
         if not build_number:
             raise Exception('Build number not defined, '
                             'missing one of TCMS_BUILD, '
                             'TRAVIS_BUILD_NUMBER or BUILD_NUMBER')
 
         build = self.rpc.Build.filter({'name': build_number,
-                                       'product': product_id})
+                                       'version': version_id})
         if not build:
             build = [self.rpc.Build.create({'name': build_number,
-                                            'product': product_id})]
+                                            'version': version_id})]
 
         return build[0]['id'], build_number
 
     def get_plan_type_id(self):
         """
             Return an **Integration** PlanType.
 
@@ -384,15 +376,15 @@
             :rtype: int
         """
         run_id = os.environ.get('TCMS_RUN_ID')
 
         if not run_id:
             product_id, product_name = self.get_product_id(0)
             version_id, version_val = self.get_version_id(product_id)
-            build_id, build_number = self.get_build_id(product_id, version_id)
+            build_id, build_number = self.get_build_id(version_id)
             plan_id = self.get_plan_id(0)
             # TR.manager is always the author of the TP, which is either
             # another existing user (existing TP) or self.default_tester_id()
             # in case of newly created TP
             manager_id = self.rpc.TestPlan.filter({
                 'pk': plan_id
             })[0]['author_id']
```

### Comparing `tcms-api-8.6.0/tcms_api/xmlrpc.py` & `tcms-api-9.0/tcms_api/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `tcms-api-8.6.0/tcms_api.egg-info/PKG-INFO` & `tcms-api-9.0/tcms_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: tcms-api
-Version: 8.6.0
+Version: 9.0
 Summary: Python API for Kiwi
 Home-page: https://github.com/kiwitcms/tcms-api
-Maintainer: Kiwi TCMS
-Maintainer-email: info@kiwitcms.org
+Author: Kiwi TCMS
+Author-email: info@kiwitcms.org
 License: LGPLv2+
 Description: Python API for Kiwi TCMS
         ========================
         
         .. image:: https://travis-ci.org/kiwitcms/tcms-api.svg?branch=master
             :target: https://travis-ci.org/kiwitcms/tcms-api
         
@@ -63,19 +63,31 @@
         ``dnf install gcc krb5-devel python3-devel`` (Red Hat/Fedora) or
         ``apt-get install gcc libkrb5-dev libpython3-dev`` (Debian/Ubuntu).
         
         
         CHANGELOG
         ---------
         
+        v9.0 (12 January 2021)
+        ~~~~~~~~~~~~~~~~~~~~~~
+        
+        **WARNING:** contains backwards incompatible changes!
+        
+        - Compatible with Kiwi TCMS v9.0 or later
+        - Method ``Backend.build_id()`` doesn't receive ``product_id`` as firsts
+          parameter anymore! Related to Kiwi TCMS
+          `Issue #246 <https://github.com/kiwitcms/Kiwi/issues/246>`_
+        
+        
         v8.6.0 (28 October 2020)
         ~~~~~~~~~~~~~~~~~~~~~~~~
         
         - Use a sub-package to install gssapi, see installation instructions
         
+        
         v8.5.0 (04 August 2020)
         ~~~~~~~~~~~~~~~~~~~~~~~
         
         - Fix ``super()`` call in ``CookieTransport`` class to make this package
           compatible with Python 3.8 (Václav Klikar)
         
         
@@ -200,9 +212,7 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-Provides-Extra: gssapi
```

### Comparing `tcms-api-8.6.0/LICENSE` & `tcms-api-9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tcms-api-8.6.0/README.rst` & `tcms-api-9.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -55,19 +55,31 @@
 ``dnf install gcc krb5-devel python3-devel`` (Red Hat/Fedora) or
 ``apt-get install gcc libkrb5-dev libpython3-dev`` (Debian/Ubuntu).
 
 
 CHANGELOG
 ---------
 
+v9.0 (12 January 2021)
+~~~~~~~~~~~~~~~~~~~~~~
+
+**WARNING:** contains backwards incompatible changes!
+
+- Compatible with Kiwi TCMS v9.0 or later
+- Method ``Backend.build_id()`` doesn't receive ``product_id`` as firsts
+  parameter anymore! Related to Kiwi TCMS
+  `Issue #246 <https://github.com/kiwitcms/Kiwi/issues/246>`_
+
+
 v8.6.0 (28 October 2020)
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
 - Use a sub-package to install gssapi, see installation instructions
 
+
 v8.5.0 (04 August 2020)
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 - Fix ``super()`` call in ``CookieTransport`` class to make this package
   compatible with Python 3.8 (Václav Klikar)
```

### Comparing `tcms-api-8.6.0/setup.py` & `tcms-api-9.0/setup.py`

 * *Files identical despite different names*

### Comparing `tcms-api-8.6.0/PKG-INFO` & `tcms-api-9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: tcms-api
-Version: 8.6.0
+Version: 9.0
 Summary: Python API for Kiwi
 Home-page: https://github.com/kiwitcms/tcms-api
-Maintainer: Kiwi TCMS
-Maintainer-email: info@kiwitcms.org
+Author: Kiwi TCMS
+Author-email: info@kiwitcms.org
 License: LGPLv2+
 Description: Python API for Kiwi TCMS
         ========================
         
         .. image:: https://travis-ci.org/kiwitcms/tcms-api.svg?branch=master
             :target: https://travis-ci.org/kiwitcms/tcms-api
         
@@ -63,19 +63,31 @@
         ``dnf install gcc krb5-devel python3-devel`` (Red Hat/Fedora) or
         ``apt-get install gcc libkrb5-dev libpython3-dev`` (Debian/Ubuntu).
         
         
         CHANGELOG
         ---------
         
+        v9.0 (12 January 2021)
+        ~~~~~~~~~~~~~~~~~~~~~~
+        
+        **WARNING:** contains backwards incompatible changes!
+        
+        - Compatible with Kiwi TCMS v9.0 or later
+        - Method ``Backend.build_id()`` doesn't receive ``product_id`` as firsts
+          parameter anymore! Related to Kiwi TCMS
+          `Issue #246 <https://github.com/kiwitcms/Kiwi/issues/246>`_
+        
+        
         v8.6.0 (28 October 2020)
         ~~~~~~~~~~~~~~~~~~~~~~~~
         
         - Use a sub-package to install gssapi, see installation instructions
         
+        
         v8.5.0 (04 August 2020)
         ~~~~~~~~~~~~~~~~~~~~~~~
         
         - Fix ``super()`` call in ``CookieTransport`` class to make this package
           compatible with Python 3.8 (Václav Klikar)
         
         
@@ -200,9 +212,7 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-Provides-Extra: gssapi
```

