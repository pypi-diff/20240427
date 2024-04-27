# Comparing `tmp/koji_fedoramessaging_messages-1.2.3.tar.gz` & `tmp/koji_fedoramessaging_messages-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koji_fedoramessaging_messages-1.2.3.tar", max compression
+gzip compressed data, was "koji_fedoramessaging_messages-1.2.4.tar", max compression
```

## Comparing `koji_fedoramessaging_messages-1.2.3.tar` & `koji_fedoramessaging_messages-1.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    18092 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/LICENSE
--rw-r--r--   0        0        0      257 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/README.md
--rw-r--r--   0        0        0      676 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/koji_fedoramessaging_messages/__init__.py
--rw-r--r--   0        0        0     4979 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/koji_fedoramessaging_messages/base.py
--rw-r--r--   0        0        0     7251 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/koji_fedoramessaging_messages/build.py
--rw-r--r--   0        0        0     3468 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/koji_fedoramessaging_messages/package.py
--rw-r--r--   0        0        0     2498 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/koji_fedoramessaging_messages/repo.py
--rw-r--r--   0        0        0     9699 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/koji_fedoramessaging_messages/rpm.py
--rw-r--r--   0        0        0     4724 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/koji_fedoramessaging_messages/tag.py
--rw-r--r--   0        0        0     4155 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/koji_fedoramessaging_messages/task.py
--rw-r--r--   0        0        0     1534 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/koji_fedoramessaging_messages/utilities.py
--rwxr-xr-x   0        0        0      333 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/make-spec.sh
--rw-r--r--   0        0        0     2265 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     1302 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/python-koji-fedoramessaging-messages.spec.in
--rw-r--r--   0        0        0        0 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/tests/__init__.py
--rw-r--r--   0        0        0     1061 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/tests/test_base.py
--rw-r--r--   0        0        0     5682 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/tests/test_build.py
--rw-r--r--   0        0        0     1541 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/tests/test_package.py
--rw-r--r--   0        0        0     1036 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/tests/test_repo.py
--rw-r--r--   0        0        0     3510 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/tests/test_rpm.py
--rw-r--r--   0        0        0     2283 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/tests/test_tag.py
--rw-r--r--   0        0        0    14967 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/tests/test_task.py
--rw-r--r--   0        0        0      322 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/tests/test_utilities.py
--rw-r--r--   0        0        0      512 2024-01-05 16:06:15.662890 koji_fedoramessaging_messages-1.2.3/tox.ini
--rw-r--r--   0        0        0     2169 1970-01-01 00:00:00.000000 koji_fedoramessaging_messages-1.2.3/setup.py
--rw-r--r--   0        0        0     1101 1970-01-01 00:00:00.000000 koji_fedoramessaging_messages-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0    18092 2024-04-27 08:13:29.486236 koji_fedoramessaging_messages-1.2.4/LICENSE
+-rw-r--r--   0        0        0      735 2024-04-27 08:13:29.490236 koji_fedoramessaging_messages-1.2.4/README.md
+-rw-r--r--   0        0        0      676 2024-04-27 08:13:29.490236 koji_fedoramessaging_messages-1.2.4/koji_fedoramessaging_messages/__init__.py
+-rw-r--r--   0        0        0     5023 2024-04-27 08:13:29.490236 koji_fedoramessaging_messages-1.2.4/koji_fedoramessaging_messages/base.py
+-rw-r--r--   0        0        0     7251 2024-04-27 08:13:29.490236 koji_fedoramessaging_messages-1.2.4/koji_fedoramessaging_messages/build.py
+-rw-r--r--   0        0        0     3468 2024-04-27 08:13:29.490236 koji_fedoramessaging_messages-1.2.4/koji_fedoramessaging_messages/package.py
+-rw-r--r--   0        0        0     2498 2024-04-27 08:13:29.490236 koji_fedoramessaging_messages-1.2.4/koji_fedoramessaging_messages/repo.py
+-rw-r--r--   0        0        0     9699 2024-04-27 08:13:29.490236 koji_fedoramessaging_messages-1.2.4/koji_fedoramessaging_messages/rpm.py
+-rw-r--r--   0        0        0     4724 2024-04-27 08:13:29.490236 koji_fedoramessaging_messages-1.2.4/koji_fedoramessaging_messages/tag.py
+-rw-r--r--   0        0        0     4155 2024-04-27 08:13:29.490236 koji_fedoramessaging_messages-1.2.4/koji_fedoramessaging_messages/task.py
+-rw-r--r--   0        0        0     1534 2024-04-27 08:13:29.490236 koji_fedoramessaging_messages-1.2.4/koji_fedoramessaging_messages/utilities.py
+-rwxr-xr-x   0        0        0      333 2024-04-27 08:13:29.490236 koji_fedoramessaging_messages-1.2.4/make-spec.sh
+-rw-r--r--   0        0        0     2316 2024-04-27 08:13:29.490236 koji_fedoramessaging_messages-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1302 2024-04-27 08:13:29.490236 koji_fedoramessaging_messages-1.2.4/python-koji-fedoramessaging-messages.spec.in
+-rw-r--r--   0        0        0        0 2024-04-27 08:13:29.490236 koji_fedoramessaging_messages-1.2.4/tests/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-27 08:13:29.490236 koji_fedoramessaging_messages-1.2.4/tests/test_base.py
+-rw-r--r--   0        0        0    13315 2024-04-27 08:13:29.490236 koji_fedoramessaging_messages-1.2.4/tests/test_build.py
+-rw-r--r--   0        0        0     1541 2024-04-27 08:13:29.490236 koji_fedoramessaging_messages-1.2.4/tests/test_package.py
+-rw-r--r--   0        0        0     1036 2024-04-27 08:13:29.490236 koji_fedoramessaging_messages-1.2.4/tests/test_repo.py
+-rw-r--r--   0        0        0     3510 2024-04-27 08:13:29.490236 koji_fedoramessaging_messages-1.2.4/tests/test_rpm.py
+-rw-r--r--   0        0        0     2283 2024-04-27 08:13:29.490236 koji_fedoramessaging_messages-1.2.4/tests/test_tag.py
+-rw-r--r--   0        0        0    14967 2024-04-27 08:13:29.490236 koji_fedoramessaging_messages-1.2.4/tests/test_task.py
+-rw-r--r--   0        0        0      322 2024-04-27 08:13:29.490236 koji_fedoramessaging_messages-1.2.4/tests/test_utilities.py
+-rw-r--r--   0        0        0      512 2024-04-27 08:13:29.490236 koji_fedoramessaging_messages-1.2.4/tox.ini
+-rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 koji_fedoramessaging_messages-1.2.4/setup.py
+-rw-r--r--   0        0        0     1579 1970-01-01 00:00:00.000000 koji_fedoramessaging_messages-1.2.4/PKG-INFO
```

### Comparing `koji_fedoramessaging_messages-1.2.3/LICENSE` & `koji_fedoramessaging_messages-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `koji_fedoramessaging_messages-1.2.3/koji_fedoramessaging_messages/__init__.py` & `koji_fedoramessaging_messages-1.2.4/koji_fedoramessaging_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `koji_fedoramessaging_messages-1.2.3/koji_fedoramessaging_messages/base.py` & `koji_fedoramessaging_messages-1.2.4/koji_fedoramessaging_messages/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 
 from fedora_messaging import message
 
 SCHEMA_URL = "http://fedoraproject.org/message-schema/"
 
 
 TASK_RESULT = {
-    "type": ["null", "object"],
+    # LiveCD results are a string
+    "type": ["null", "object", "string"],
     "description": "the results of a task (files)",
     "properties": {
         "srpm": {
             "type": "string",
         },
         "rpms": {
             "type": "array",
```

### Comparing `koji_fedoramessaging_messages-1.2.3/koji_fedoramessaging_messages/build.py` & `koji_fedoramessaging_messages-1.2.4/koji_fedoramessaging_messages/build.py`

 * *Files identical despite different names*

### Comparing `koji_fedoramessaging_messages-1.2.3/koji_fedoramessaging_messages/package.py` & `koji_fedoramessaging_messages-1.2.4/koji_fedoramessaging_messages/package.py`

 * *Files identical despite different names*

### Comparing `koji_fedoramessaging_messages-1.2.3/koji_fedoramessaging_messages/repo.py` & `koji_fedoramessaging_messages-1.2.4/koji_fedoramessaging_messages/repo.py`

 * *Files identical despite different names*

### Comparing `koji_fedoramessaging_messages-1.2.3/koji_fedoramessaging_messages/rpm.py` & `koji_fedoramessaging_messages-1.2.4/koji_fedoramessaging_messages/rpm.py`

 * *Files identical despite different names*

### Comparing `koji_fedoramessaging_messages-1.2.3/koji_fedoramessaging_messages/tag.py` & `koji_fedoramessaging_messages-1.2.4/koji_fedoramessaging_messages/tag.py`

 * *Files identical despite different names*

### Comparing `koji_fedoramessaging_messages-1.2.3/koji_fedoramessaging_messages/task.py` & `koji_fedoramessaging_messages-1.2.4/koji_fedoramessaging_messages/task.py`

 * *Files identical despite different names*

### Comparing `koji_fedoramessaging_messages-1.2.3/koji_fedoramessaging_messages/utilities.py` & `koji_fedoramessaging_messages-1.2.4/koji_fedoramessaging_messages/utilities.py`

 * *Files identical despite different names*

### Comparing `koji_fedoramessaging_messages-1.2.3/pyproject.toml` & `koji_fedoramessaging_messages-1.2.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "koji-fedoramessaging-messages"
-version = "1.2.3"
+version = "1.2.4"
 description = "A schema package for messages sent by the koji-fedoramessaging plugin"
 
 license = "GPL-3.0-or-later"
 
 authors = [
   "Fedora Infrastructure Team <infrastructure@lists.fedoraproject.org>"
 ]
@@ -35,20 +35,20 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 fedora-messaging = ">=3.0.1"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
+pytest = "^7.1.2 || ^8.0.0"
 pytest-cov = "^3.0.0 || ^4.0.0"
 sphinx = "^3.0 || ^4.0.0 || ^7.0.0"
-black = "^22.6.0 || ^23.0.0"
+black = "^22.6.0 || ^23.0.0 || ^24.0.0"
 poetry = "^1.2.0b2"
-ruff = "^0.0.272 || ^0.0.287 || ^0.0.288 || ^0.0.289 || ^0.0.290 || ^0.0.291 || ^0.0.292 || ^0.1.0"
+ruff = "^0.0.272 || ^0.0.287 || ^0.0.288 || ^0.0.289 || ^0.0.290 || ^0.0.291 || ^0.0.292 || ^0.1.0 || ^0.2.0 || ^0.3.0 || ^0.4.0"
 
 [tool.poetry.build]
 generate-setup-file = true
 
 [tool.black]
 line-length = 100
```

### Comparing `koji_fedoramessaging_messages-1.2.3/python-koji-fedoramessaging-messages.spec.in` & `koji_fedoramessaging_messages-1.2.4/python-koji-fedoramessaging-messages.spec.in`

 * *Files identical despite different names*

### Comparing `koji_fedoramessaging_messages-1.2.3/tests/test_base.py` & `koji_fedoramessaging_messages-1.2.4/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `koji_fedoramessaging_messages-1.2.3/tests/test_package.py` & `koji_fedoramessaging_messages-1.2.4/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `koji_fedoramessaging_messages-1.2.3/tests/test_repo.py` & `koji_fedoramessaging_messages-1.2.4/tests/test_repo.py`

 * *Files identical despite different names*

### Comparing `koji_fedoramessaging_messages-1.2.3/tests/test_rpm.py` & `koji_fedoramessaging_messages-1.2.4/tests/test_rpm.py`

 * *Files identical despite different names*

### Comparing `koji_fedoramessaging_messages-1.2.3/tests/test_tag.py` & `koji_fedoramessaging_messages-1.2.4/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `koji_fedoramessaging_messages-1.2.3/tests/test_task.py` & `koji_fedoramessaging_messages-1.2.4/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `koji_fedoramessaging_messages-1.2.3/tox.ini` & `koji_fedoramessaging_messages-1.2.4/tox.ini`

 * *Files identical despite different names*

### Comparing `koji_fedoramessaging_messages-1.2.3/PKG-INFO` & `koji_fedoramessaging_messages-1.2.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koji-fedoramessaging-messages
-Version: 1.2.3
+Version: 1.2.4
 Summary: A schema package for messages sent by the koji-fedoramessaging plugin
 Home-page: https://github.com/fedora-infra/koji-fedoramessaging-messages
 License: GPL-3.0-or-later
 Keywords: fedora
 Author: Fedora Infrastructure Team
 Author-email: infrastructure@lists.fedoraproject.org
 Requires-Python: >=3.10,<4.0
@@ -19,7 +19,17 @@
 
 # koji-fedoramessaging messages
 
 A schema package for [koji-fedoramessaging](http://github.com/fedora-infra/koji-fedoramessaging).
 
 See the [detailed documentation](https://fedora-messaging.readthedocs.io/en/latest/messages.html) on packaging your schemas.
 
+
+## Rebuilding for Fedora Infra
+
+At the moment this package is not in Fedora. To build a RPM for Fedora Infra, follow the following steps:
+
+- checkout the latest tag: `git co v1.2.4`
+- build the SRPM with Packit: `packit srpm --no-update-release`
+- build the RPM in koji: `koji build f39-infra python-koji-fedoramessaging-messages-1.2.4-1.fc39.src.rpm`
+- move the RPM to the production tag: `koji move f39-infra-stg f39-infra python-koji-fedoramessaging-messages-1.2.4-1.fc39`
+
```

