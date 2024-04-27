# Comparing `tmp/pycis_cli-0.1.1.tar.gz` & `tmp/pycis_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycis_cli-0.1.1.tar", max compression
+gzip compressed data, was "pycis_cli-0.1.2.tar", max compression
```

## Comparing `pycis_cli-0.1.1.tar` & `pycis_cli-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,30 @@
--rw-r--r--   0        0        0     1083 2024-01-26 02:55:36.937365 pycis_cli-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0      394 2024-01-26 02:55:36.937511 pycis_cli-0.1.1/README.rst
--rw-r--r--   0        0        0     1024 2024-04-17 20:07:57.988900 pycis_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-26 02:55:36.939407 pycis_cli-0.1.1/source/packages/pycis/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 02:55:36.939494 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/__init__.py
--rw-r--r--   0        0        0      768 2024-01-26 02:55:36.939649 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/__init__.py
--rw-r--r--   0        0        0       43 2024-01-26 02:55:36.939728 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/constants.py
--rw-r--r--   0        0        0      802 2024-01-26 02:55:36.939873 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/couchdb/__init__.py
--rw-r--r--   0        0        0     2948 2024-01-26 02:55:36.940023 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/couchdb/initialize.py
--rw-r--r--   0        0        0     3290 2024-04-17 20:07:28.153563 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/couchdb/publish.py
--rw-r--r--   0        0        0      602 2024-01-26 02:55:36.940225 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/mongodb/__init__.py
--rw-r--r--   0        0        0     2835 2024-01-26 02:55:36.940304 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/mongodb/publish.py
--rw-r--r--   0        0        0      882 2024-01-26 02:55:36.940432 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/__init__.py
--rw-r--r--   0        0        0     1367 2024-01-26 02:55:36.940557 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/__init__.py
--rw-r--r--   0        0        0     2611 2024-01-26 02:55:36.940655 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/addbyproduct.py
--rw-r--r--   0        0        0     2189 2024-01-26 02:55:36.940760 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/addchange.py
--rw-r--r--   0        0        0     2748 2024-01-26 02:55:36.940851 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/initialize.py
--rw-r--r--   0        0        0     2487 2024-01-26 02:55:36.940942 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/setjobdetail.py
--rw-r--r--   0        0        0     2703 2024-01-26 02:55:36.941058 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/update.py
--rw-r--r--   0        0        0      859 2024-01-26 02:55:36.941225 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/configuration/__init__.py
--rw-r--r--   0        0        0     2168 2024-01-26 02:55:36.941347 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/configuration/decrypt.py
--rw-r--r--   0        0        0     1846 2024-01-26 02:55:36.941437 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/configuration/encrypt.py
--rw-r--r--   0        0        0      612 2024-01-26 02:55:36.941583 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/testrun/__init__.py
--rw-r--r--   0        0        0     1708 2024-01-26 02:55:36.941711 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/testrun/create.py
--rw-r--r--   0        0        0     1273 2024-01-26 02:55:36.941794 pycis_cli-0.1.1/source/packages/pycis/cli/pycis_command.py
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 pycis_cli-0.1.1/setup.py
--rw-r--r--   0        0        0     1353 1970-01-01 00:00:00.000000 pycis_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-26 02:55:36.937365 pycis_cli-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0      394 2024-01-26 02:55:36.937511 pycis_cli-0.1.2/README.rst
+-rw-r--r--   0        0        0     1102 2024-04-27 20:20:22.776696 pycis_cli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-04-27 16:42:38.282942 pycis_cli-0.1.2/source/packages/pycis/cli/__init__.py
+-rw-r--r--   0        0        0      780 2024-04-27 18:46:01.046420 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/__init__.py
+-rw-r--r--   0        0        0     1538 2024-04-27 17:02:31.848946 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/__init__.py
+-rw-r--r--   0        0        0       43 2024-01-26 02:55:36.939728 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/constants.py
+-rw-r--r--   0        0        0     1023 2024-04-27 16:56:49.240929 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/couchdb/__init__.py
+-rw-r--r--   0        0        0     3084 2024-04-27 16:54:25.952526 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/couchdb/initialize.py
+-rw-r--r--   0        0        0     3423 2024-04-27 18:47:57.999404 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/couchdb/publish.py
+-rw-r--r--   0        0        0     1009 2024-04-27 18:47:57.999622 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/mongodb/__init__.py
+-rw-r--r--   0        0        0     2967 2024-04-27 16:57:16.723099 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/mongodb/publish.py
+-rw-r--r--   0        0        0     1043 2024-04-27 17:09:37.897997 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/__init__.py
+-rw-r--r--   0        0        0     1543 2024-04-27 17:04:30.658011 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/__init__.py
+-rw-r--r--   0        0        0     2611 2024-01-26 02:55:36.940655 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/addbyproduct.py
+-rw-r--r--   0        0        0     2189 2024-01-26 02:55:36.940760 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/addchange.py
+-rw-r--r--   0        0        0     2748 2024-01-26 02:55:36.940851 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/initialize.py
+-rw-r--r--   0        0        0     2487 2024-01-26 02:55:36.940942 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/setjobdetail.py
+-rw-r--r--   0        0        0     2703 2024-01-26 02:55:36.941058 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/update.py
+-rw-r--r--   0        0        0     1011 2024-04-27 17:05:16.355144 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/configuration/__init__.py
+-rw-r--r--   0        0        0     2168 2024-01-26 02:55:36.941347 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/configuration/decrypt.py
+-rw-r--r--   0        0        0     1846 2024-01-26 02:55:36.941437 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/configuration/encrypt.py
+-rw-r--r--   0        0        0      743 2024-04-27 17:06:12.311665 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/testrun/__init__.py
+-rw-r--r--   0        0        0     1708 2024-01-26 02:55:36.941711 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/testrun/create.py
+-rw-r--r--   0        0        0      704 2024-04-27 19:33:19.248701 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/tracking/__init__.py
+-rw-r--r--   0        0        0     3189 2024-04-27 20:41:29.486864 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/tracking/jira/__init__.py
+-rw-r--r--   0        0        0     3621 2024-04-27 20:40:31.049882 pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/tracking/jira/comment.py
+-rwxr-xr-x   0        0        0     1144 2024-04-27 16:48:18.298609 pycis_cli-0.1.2/source/packages/pycis/cli/pycis_command.py
+-rw-r--r--   0        0        0     1856 1970-01-01 00:00:00.000000 pycis_cli-0.1.2/setup.py
+-rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 pycis_cli-0.1.2/PKG-INFO
```

### Comparing `pycis_cli-0.1.1/LICENSE.txt` & `pycis_cli-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.1/pyproject.toml` & `pycis_cli-0.1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 [tool.poetry]
 name = "pycis-cli"
 description = "Python Continuous Integration System (PyCIS) - CLI Tools"
-version = "0.1.1"
+version = "0.1.2"
 authors = []
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
 ]
 keywords = [
     "python"
 ]
 packages = [{include="pycis", from="source/packages"}]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.9 <4.0"
 click = "^8.1.4"
-pymongo = {extras = ["srv"], version = "^4.0.0", optional = true}
+pymongo = {version = "^4.0.0", optional = true}
 couchdb = {version = "^1.2", optional = true}
 mojo-xmodules = ">=1.3.0 <1.4.0"
+mojo-credentials = ">=1.3.10 <1.4.0"
 mojo-config = ">=1.3.0 <1.4.0"
+jira = {version="^3.8.0", optional = true}
 
 [tool.poetry.scripts]
 pycis = "pycis.cli.pycis_command:pycis_root_command"
 
 [tool.poetry.extras]
 mongodb = ["pymongo"]
 couchdb = ["couchdb"]
+jira = ["jira"]
 
 [tool.poetry.group.dev.dependencies]
 myst-parser = "^0.18.1"
 sphinx = ">=1.6,<6"
 sphinx-rtd-theme = "^1.1.1"
 
 [tool.poetry.group.dbio.dependencies]
```

### Comparing `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/__init__.py` & `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/mongodb/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,33 @@
+
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
 __version__ = "1.0.0"
 __maintainer__ = "Myron Walker"
 __email__ = "myron.walker@gmail.com"
 __status__ = "Development" # Prototype, Development or Production
 __license__ = "MIT"
 
 import click
 
-from pycis.cli.cmdtree.datastore.couchdb import group_pycis_datastore_couchdb
-from pycis.cli.cmdtree.datastore.mongodb import group_pycis_datastore_mongodb
+from pycis.cli.cmdtree.datastore.mongodb.publish import command_pycis_datastore_mongodb_publish
 
-datastore_HELP = "Contains commands groups for datastore test results to different types of data stores."
 
-@click.group("datastore", help=datastore_HELP)
-def group_pycis_datastore():
+@click.group("mongodb", help="Contains commands datastore test results to MongoDB.")
+def group_pycis_datastore_mongodb():
     return
 
-group_pycis_datastore.add_command(group_pycis_datastore_couchdb)
-group_pycis_datastore.add_command(group_pycis_datastore_mongodb)
+group_pycis_datastore_mongodb.add_command(command_pycis_datastore_mongodb_publish)
+
+def add_groups_and_commands(parent: click.Group):
+    
+    from pycis.cli.cmdtree.datastore.mongodb.publish import add_groups_and_commands as publish_add_groups_and_commands
+
+    # Call to child groups to add themselfs to this group
+    publish_add_groups_and_commands(group_pycis_datastore_mongodb)
+
+    # Add this group to its parent
+    parent.add_command(group_pycis_datastore_mongodb)
+
+    
+    return
```

### Comparing `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/couchdb/__init__.py` & `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/couchdb/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,19 +6,26 @@
 __maintainer__ = "Myron Walker"
 __email__ = "myron.walker@gmail.com"
 __status__ = "Development" # Prototype, Development or Production
 __license__ = "MIT"
 
 import click
 
-from pycis.cli.cmdtree.datastore.couchdb.initialize \
-    import command_pycis_datastore_couchdb_initialize
-from pycis.cli.cmdtree.datastore.couchdb.publish \
-    import command_pycis_datastore_couchdb_publish
-
 
 @click.group("couchdb", help="Contains commands datastore test results to CouchDB.")
 def group_pycis_datastore_couchdb():
     return
 
-group_pycis_datastore_couchdb.add_command(command_pycis_datastore_couchdb_initialize)
-group_pycis_datastore_couchdb.add_command(command_pycis_datastore_couchdb_publish)
+def add_groups_and_commands(parent: click.Group):
+    
+    from pycis.cli.cmdtree.datastore.couchdb.initialize import add_groups_and_commands as initialize_add_groups_and_commands
+    from pycis.cli.cmdtree.datastore.couchdb.publish import add_groups_and_commands as publish_add_groups_and_commands
+
+    # Call to child groups to add themselfs to this group
+    initialize_add_groups_and_commands(group_pycis_datastore_couchdb)
+    publish_add_groups_and_commands(group_pycis_datastore_couchdb)
+
+    # Add this group to its parent
+    parent.add_command(group_pycis_datastore_couchdb)
+
+    
+    return
```

### Comparing `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/couchdb/initialize.py` & `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/couchdb/initialize.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,8 +92,15 @@
             },
             "language": "javascript",
             "options": {"partitioned": False }
         }
 
         database.save( data )
 
+    return
+
+
+def add_groups_and_commands(parent: click.Group):
+    
+    parent.add_command(command_pycis_datastore_couchdb_initialize)
+
     return
```

### Comparing `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/couchdb/publish.py` & `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/couchdb/publish.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,8 +85,14 @@
     docobj["expiry_date"] = expiry_date.isoformat()
 
     dbsvr = couchdb.Server(connection)
 
     pycis = dbsvr[PYCIS_DB_BYPRODUCTS]
     pycis.save(docobj)
 
-    return
+    return
+
+def add_groups_and_commands(parent: click.Group):
+    
+    parent.add_command(command_pycis_datastore_couchdb_publish)
+
+    return
```

### Comparing `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/mongodb/publish.py` & `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/datastore/mongodb/publish.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,8 +76,14 @@
     client = MongoClient(host, port)
     
     pycisdb = client[PYCIS_DB_BYPRODUCTS]
 
     testruns = pycisdb[category]
     testruns.insert_one(docobj)
 
+    return
+
+def add_groups_and_commands(parent: click.Group):
+    
+    parent.add_command(command_pycis_datastore_mongodb_publish)
+
     return
```

### Comparing `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/__init__.py` & `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/configuration/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,28 +6,32 @@
 __maintainer__ = "Myron Walker"
 __email__ = "myron.walker@gmail.com"
 __status__ = "Development" # Prototype, Development or Production
 __license__ = "MIT"
 
 import click
 
-from pycis.cli.cmdtree.document.build \
-    import group_pycis_document_build
-from pycis.cli.cmdtree.document.configuration \
-    import group_pycis_document_configuration
-from pycis.cli.cmdtree.document.testrun \
-    import group_pycis_document_testrun
 
+from pycis.cli.cmdtree.document.configuration.decrypt \
+    import command_pycis_document_configuration_decrypt
+from pycis.cli.cmdtree.document.configuration.encrypt \
+    import command_pycis_document_configuration_encrypt
 
-@click.group("document", help="Contains commands for writing data to a pycis document.")
-def group_pycis_document():
+
+@click.group("configuration", help="Contains commands for working configuration documents.")
+def group_pycis_document_configuration():
     return
 
-group_pycis_document.add_command(
-    group_pycis_document_build
-)
-group_pycis_document.add_command(
-    group_pycis_document_configuration
-)
-group_pycis_document.add_command(
-    group_pycis_document_testrun
-)
+
+def add_groups_and_commands(parent: click.Group):
+    
+    group_pycis_document_configuration.add_command(
+        command_pycis_document_configuration_decrypt
+    )
+    group_pycis_document_configuration.add_command(
+        command_pycis_document_configuration_encrypt
+    )
+
+
+    parent.add_command(group_pycis_document_configuration)
+
+    return
```

### Comparing `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/__init__.py` & `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,22 +23,29 @@
 
 
 
 @click.group("build", help="Contains commands for writing data to a pycis 'build' document.")
 def group_pycis_document_build():
     return
 
-group_pycis_document_build.add_command(
-    command_pycis_document_build_addbyproduct
-)
-group_pycis_document_build.add_command(
-    command_pycis_document_build_addchange
-)
-group_pycis_document_build.add_command(
-    command_pycis_document_build_initialize
-)
-group_pycis_document_build.add_command(
-    command_pycis_document_build_setjobdetail
-)
-group_pycis_document_build.add_command(
-    command_pycis_document_build_update
-)
+def add_groups_and_commands(parent: click.Group):
+
+    group_pycis_document_build.add_command(
+        command_pycis_document_build_addbyproduct
+    )
+    group_pycis_document_build.add_command(
+        command_pycis_document_build_addchange
+    )
+    group_pycis_document_build.add_command(
+        command_pycis_document_build_initialize
+    )
+    group_pycis_document_build.add_command(
+        command_pycis_document_build_setjobdetail
+    )
+    group_pycis_document_build.add_command(
+        command_pycis_document_build_update
+    )
+
+    parent.add_command(group_pycis_document_build)
+
+    return
+
```

### Comparing `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/addbyproduct.py` & `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/addbyproduct.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/addchange.py` & `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/addchange.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/initialize.py` & `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/initialize.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/setjobdetail.py` & `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/setjobdetail.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/update.py` & `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/build/update.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/configuration/decrypt.py` & `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/configuration/decrypt.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/configuration/encrypt.py` & `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/configuration/encrypt.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/testrun/__init__.py` & `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/testrun/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,10 +15,17 @@
     import command_pycis_document_testrun_create
 
 
 @click.group("testrun", help="Contains commands for creating a pycis 'testrun' document.")
 def group_pycis_document_testrun():
     return
 
-group_pycis_document_testrun.add_command(
-    command_pycis_document_testrun_create
-)
+
+def add_groups_and_commands(parent: click.Group):
+
+    group_pycis_document_testrun.add_command(
+        command_pycis_document_testrun_create
+    )
+
+    parent.add_command(group_pycis_document_testrun)
+
+    return
```

### Comparing `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/testrun/create.py` & `pycis_cli-0.1.2/source/packages/pycis/cli/cmdtree/document/testrun/create.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.1/source/packages/pycis/cli/pycis_command.py` & `pycis_cli-0.1.2/source/packages/pycis/cli/pycis_command.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,17 +14,14 @@
 __maintainer__ = "Myron Walker"
 __email__ = "myron.walker@gmail.com"
 __status__ = "Development" # Prototype, Development or Production
 __license__ = "MIT"
 
 import click
 
-from pycis.cli.cmdtree.datastore import group_pycis_datastore
-from pycis.cli.cmdtree.document import group_pycis_document
-
 
 @click.group("pycis")
 @click.option('-v', '--verbose', count=True)
 @click.pass_context
 def pycis_root_command(ctx, verbose):
 
     if verbose == 0:
@@ -38,12 +35,15 @@
         elif verbose == 2:
             ctx.log_level_console = "DEBUG"
         elif verbose > 2:
             ctx.log_level_console = "NOTSET"
 
     return
 
-pycis_root_command.add_command(group_pycis_datastore)
-pycis_root_command.add_command(group_pycis_document)
+
+from pycis.cli.cmdtree import add_groups_and_commands
+
+add_groups_and_commands(pycis_root_command)
+
 
 if __name__ == '__main__':
     pycis_root_command()
```

### Comparing `pycis_cli-0.1.1/setup.py` & `pycis_cli-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,44 +10,49 @@
  'pycis.cli.cmdtree',
  'pycis.cli.cmdtree.datastore',
  'pycis.cli.cmdtree.datastore.couchdb',
  'pycis.cli.cmdtree.datastore.mongodb',
  'pycis.cli.cmdtree.document',
  'pycis.cli.cmdtree.document.build',
  'pycis.cli.cmdtree.document.configuration',
- 'pycis.cli.cmdtree.document.testrun']
+ 'pycis.cli.cmdtree.document.testrun',
+ 'pycis.cli.cmdtree.tracking',
+ 'pycis.cli.cmdtree.tracking.jira']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['click>=8.1.4,<9.0.0',
  'mojo-config>=1.3.0,<1.4.0',
+ 'mojo-credentials>=1.3.10,<1.4.0',
  'mojo-xmodules>=1.3.0,<1.4.0']
 
 extras_require = \
-{'couchdb': ['couchdb>=1.2,<2.0'], 'mongodb': ['pymongo[srv]>=4.0.0,<5.0.0']}
+{'couchdb': ['couchdb>=1.2,<2.0'],
+ 'jira': ['jira>=3.8.0,<4.0.0'],
+ 'mongodb': ['pymongo>=4.0.0,<5.0.0']}
 
 entry_points = \
 {'console_scripts': ['pycis = pycis.cli.pycis_command:pycis_root_command']}
 
 setup_kwargs = {
     'name': 'pycis-cli',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Python Continuous Integration System (PyCIS) - CLI Tools',
     'long_description': '========================================================\nPython Continuous Integration System (PyCIS) - CLI Tools\n========================================================\n\nProvides a set of CLI tools for working with the PyCIS continuous integration system.\n\n==========\nReferences\n==========\n\n- `User Guide <userguide/userguide.rst>`\n- `Coding Standards <userguide/10-00-coding-standards.rst>`\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pycis_cli-0.1.1/PKG-INFO` & `pycis_cli-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: pycis-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Continuous Integration System (PyCIS) - CLI Tools
 License: LICENSE.txt
 Keywords: python
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: couchdb
+Provides-Extra: jira
 Provides-Extra: mongodb
 Requires-Dist: click (>=8.1.4,<9.0.0)
 Requires-Dist: couchdb (>=1.2,<2.0) ; extra == "couchdb"
+Requires-Dist: jira (>=3.8.0,<4.0.0) ; extra == "jira"
 Requires-Dist: mojo-config (>=1.3.0,<1.4.0)
+Requires-Dist: mojo-credentials (>=1.3.10,<1.4.0)
 Requires-Dist: mojo-xmodules (>=1.3.0,<1.4.0)
-Requires-Dist: pymongo[srv] (>=4.0.0,<5.0.0) ; extra == "mongodb"
+Requires-Dist: pymongo (>=4.0.0,<5.0.0) ; extra == "mongodb"
 Description-Content-Type: text/x-rst
 
 ========================================================
 Python Continuous Integration System (PyCIS) - CLI Tools
 ========================================================
 
 Provides a set of CLI tools for working with the PyCIS continuous integration system.
```

