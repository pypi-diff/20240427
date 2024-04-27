# Comparing `tmp/pycis_cli-0.1.2.tar.gz` & `tmp/pycis_cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycis_cli-0.1.2.tar", max compression
+gzip compressed data, was "pycis_cli-0.1.3.tar", max compression
```

## Comparing `pycis_cli-0.1.2.tar` & `pycis_cli-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1083 2024-01-26 02:55:36.937365 pycis_cli-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0      394 2024-01-26 02:55:36.937511 pycis_cli-0.1.2/README.rst
--rw-r--r--   0        0        0     1102 2024-04-27 20:20:22.776696 pycis_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        1 2024-04-27 16:42:38.282942 pycis_cli-0.1.2/source/packages/pycis/cli/__init__.py
--rw-r--r--   0        0        0      780 2024-04-27 18:46:01.046420 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/__init__.py
--rw-r--r--   0        0        0     1538 2024-04-27 17:02:31.848946 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/__init__.py
--rw-r--r--   0        0        0       43 2024-01-26 02:55:36.939728 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/constants.py
--rw-r--r--   0        0        0     1023 2024-04-27 16:56:49.240929 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/couchdb/__init__.py
--rw-r--r--   0        0        0     3084 2024-04-27 16:54:25.952526 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/couchdb/initialize.py
--rw-r--r--   0        0        0     3423 2024-04-27 18:47:57.999404 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/couchdb/publish.py
--rw-r--r--   0        0        0     1009 2024-04-27 18:47:57.999622 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/mongodb/__init__.py
--rw-r--r--   0        0        0     2967 2024-04-27 16:57:16.723099 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/mongodb/publish.py
--rw-r--r--   0        0        0     1043 2024-04-27 17:09:37.897997 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/__init__.py
--rw-r--r--   0        0        0     1543 2024-04-27 17:04:30.658011 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/__init__.py
--rw-r--r--   0        0        0     2611 2024-01-26 02:55:36.940655 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/addbyproduct.py
--rw-r--r--   0        0        0     2189 2024-01-26 02:55:36.940760 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/addchange.py
--rw-r--r--   0        0        0     2748 2024-01-26 02:55:36.940851 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/initialize.py
--rw-r--r--   0        0        0     2487 2024-01-26 02:55:36.940942 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/setjobdetail.py
--rw-r--r--   0        0        0     2703 2024-01-26 02:55:36.941058 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/update.py
--rw-r--r--   0        0        0     1011 2024-04-27 17:05:16.355144 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/configuration/__init__.py
--rw-r--r--   0        0        0     2168 2024-01-26 02:55:36.941347 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/configuration/decrypt.py
--rw-r--r--   0        0        0     1846 2024-01-26 02:55:36.941437 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/configuration/encrypt.py
--rw-r--r--   0        0        0      743 2024-04-27 17:06:12.311665 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/testrun/__init__.py
--rw-r--r--   0        0        0     1708 2024-01-26 02:55:36.941711 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/testrun/create.py
--rw-r--r--   0        0        0      704 2024-04-27 19:33:19.248701 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/tracking/__init__.py
--rw-r--r--   0        0        0     3189 2024-04-27 20:41:29.486864 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/tracking/jira/__init__.py
--rw-r--r--   0        0        0     3621 2024-04-27 20:40:31.049882 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/tracking/jira/comment.py
--rwxr-xr-x   0        0        0     1144 2024-04-27 16:48:18.298609 pycis_cli-0.1.2/source/packages/pycis/cli/pycis_command.py
--rw-r--r--   0        0        0     1856 1970-01-01 00:00:00.000000 pycis_cli-0.1.2/setup.py
--rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 pycis_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-26 02:55:36.937365 pycis_cli-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0      394 2024-01-26 02:55:36.937511 pycis_cli-0.1.3/README.rst
+-rw-r--r--   0        0        0     1102 2024-04-27 20:58:08.328023 pycis_cli-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-04-27 16:42:38.282942 pycis_cli-0.1.3/source/packages/pycis/cli/__init__.py
+-rw-r--r--   0        0        0      780 2024-04-27 18:46:01.046420 pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/__init__.py
+-rw-r--r--   0        0        0     1538 2024-04-27 17:02:31.848946 pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/datastore/__init__.py
+-rw-r--r--   0        0        0       43 2024-01-26 02:55:36.939728 pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/datastore/constants.py
+-rw-r--r--   0        0        0     1023 2024-04-27 16:56:49.240929 pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/datastore/couchdb/__init__.py
+-rw-r--r--   0        0        0     3084 2024-04-27 16:54:25.952526 pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/datastore/couchdb/initialize.py
+-rw-r--r--   0        0        0     3423 2024-04-27 18:47:57.999404 pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/datastore/couchdb/publish.py
+-rw-r--r--   0        0        0     1009 2024-04-27 18:47:57.999622 pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/datastore/mongodb/__init__.py
+-rw-r--r--   0        0        0     2967 2024-04-27 16:57:16.723099 pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/datastore/mongodb/publish.py
+-rw-r--r--   0        0        0     1043 2024-04-27 17:09:37.897997 pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/__init__.py
+-rw-r--r--   0        0        0     1543 2024-04-27 17:04:30.658011 pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/build/__init__.py
+-rw-r--r--   0        0        0     2611 2024-01-26 02:55:36.940655 pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/build/addbyproduct.py
+-rw-r--r--   0        0        0     2189 2024-01-26 02:55:36.940760 pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/build/addchange.py
+-rw-r--r--   0        0        0     2748 2024-01-26 02:55:36.940851 pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/build/initialize.py
+-rw-r--r--   0        0        0     2487 2024-01-26 02:55:36.940942 pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/build/setjobdetail.py
+-rw-r--r--   0        0        0     2703 2024-01-26 02:55:36.941058 pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/build/update.py
+-rw-r--r--   0        0        0     1011 2024-04-27 17:05:16.355144 pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/configuration/__init__.py
+-rw-r--r--   0        0        0     2168 2024-01-26 02:55:36.941347 pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/configuration/decrypt.py
+-rw-r--r--   0        0        0     1846 2024-01-26 02:55:36.941437 pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/configuration/encrypt.py
+-rw-r--r--   0        0        0      743 2024-04-27 17:06:12.311665 pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/testrun/__init__.py
+-rw-r--r--   0        0        0     1708 2024-01-26 02:55:36.941711 pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/testrun/create.py
+-rw-r--r--   0        0        0      812 2024-04-27 20:58:01.418670 pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/tracking/__init__.py
+-rw-r--r--   0        0        0     3189 2024-04-27 20:41:29.486864 pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/tracking/jira/__init__.py
+-rw-r--r--   0        0        0     3621 2024-04-27 20:40:31.049882 pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/tracking/jira/comment.py
+-rwxr-xr-x   0        0        0     1144 2024-04-27 16:48:18.298609 pycis_cli-0.1.3/source/packages/pycis/cli/pycis_command.py
+-rw-r--r--   0        0        0     1856 1970-01-01 00:00:00.000000 pycis_cli-0.1.3/setup.py
+-rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 pycis_cli-0.1.3/PKG-INFO
```

### Comparing `pycis_cli-0.1.2/LICENSE.txt` & `pycis_cli-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.2/pyproject.toml` & `pycis_cli-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pycis-cli"
 description = "Python Continuous Integration System (PyCIS) - CLI Tools"
-version = "0.1.2"
+version = "0.1.3"
 authors = []
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
```

### Comparing `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/__init__.py` & `pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/__init__.py` & `pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/couchdb/__init__.py` & `pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/datastore/couchdb/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/couchdb/initialize.py` & `pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/datastore/couchdb/initialize.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/couchdb/publish.py` & `pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/datastore/couchdb/publish.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/mongodb/__init__.py` & `pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/datastore/mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/mongodb/publish.py` & `pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/datastore/mongodb/publish.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/__init__.py` & `pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/__init__.py` & `pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/build/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/addbyproduct.py` & `pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/build/addbyproduct.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/addchange.py` & `pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/build/addchange.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/initialize.py` & `pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/build/initialize.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/setjobdetail.py` & `pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/build/setjobdetail.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/update.py` & `pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/build/update.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/configuration/__init__.py` & `pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/configuration/decrypt.py` & `pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/configuration/decrypt.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/configuration/encrypt.py` & `pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/configuration/encrypt.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/testrun/__init__.py` & `pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/testrun/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/testrun/create.py` & `pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/document/testrun/create.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/tracking/__init__.py` & `pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/tracking/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 @click.group("tracking", help="Contains commands for interoperating with tracking software and services.")
 def group_pycis_tracking():
     return
 
 
 def add_groups_and_commands(parent: click.Group):
 
-    from pycis.cli.cmdtree.tracking.jira import add_groups_and_commands as jira_add_groups_and_commands
+    try:
+        from pycis.cli.cmdtree.tracking.jira import add_groups_and_commands as jira_add_groups_and_commands
 
-    jira_add_groups_and_commands(group_pycis_tracking)
+        jira_add_groups_and_commands(group_pycis_tracking)
+    except ImportError:
+        # If jira is not installed, just don't add it
+        pass
 
     parent.add_command(group_pycis_tracking)
 
     return
```

### Comparing `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/tracking/jira/__init__.py` & `pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/tracking/jira/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/tracking/jira/comment.py` & `pycis_cli-0.1.3/source/packages/pycis/cli/cmdtree/tracking/jira/comment.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.2/source/packages/pycis/cli/pycis_command.py` & `pycis_cli-0.1.3/source/packages/pycis/cli/pycis_command.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.2/setup.py` & `pycis_cli-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
  'mongodb': ['pymongo>=4.0.0,<5.0.0']}
 
 entry_points = \
 {'console_scripts': ['pycis = pycis.cli.pycis_command:pycis_root_command']}
 
 setup_kwargs = {
     'name': 'pycis-cli',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Python Continuous Integration System (PyCIS) - CLI Tools',
     'long_description': '========================================================\nPython Continuous Integration System (PyCIS) - CLI Tools\n========================================================\n\nProvides a set of CLI tools for working with the PyCIS continuous integration system.\n\n==========\nReferences\n==========\n\n- `User Guide <userguide/userguide.rst>`\n- `Coding Standards <userguide/10-00-coding-standards.rst>`\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pycis_cli-0.1.2/PKG-INFO` & `pycis_cli-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycis-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Continuous Integration System (PyCIS) - CLI Tools
 License: LICENSE.txt
 Keywords: python
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
```

