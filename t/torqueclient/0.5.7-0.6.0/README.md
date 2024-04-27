# Comparing `tmp/torqueclient-0.5.7.tar.gz` & `tmp/torqueclient-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torqueclient-0.5.7.tar", last modified: Fri Jan 26 23:05:57 2024, max compression
+gzip compressed data, was "torqueclient-0.6.0.tar", last modified: Sat Apr 27 17:49:28 2024, max compression
```

## Comparing `torqueclient-0.5.7.tar` & `torqueclient-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-01-26 23:05:57.345542 torqueclient-0.5.7/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    34523 2023-02-19 01:57:21.000000 torqueclient-0.5.7/LICENSE
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1031 2024-01-26 23:05:57.345542 torqueclient-0.5.7/PKG-INFO
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      502 2023-02-19 01:57:21.000000 torqueclient-0.5.7/README.md
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      107 2023-02-19 01:57:21.000000 torqueclient-0.5.7/pyproject.toml
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       38 2024-01-26 23:05:57.345542 torqueclient-0.5.7/setup.cfg
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      973 2023-02-19 01:57:21.000000 torqueclient-0.5.7/setup.py
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-01-26 23:05:57.341542 torqueclient-0.5.7/torqueclient/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       85 2024-01-26 22:57:36.000000 torqueclient-0.5.7/torqueclient/__init__.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    14658 2024-01-26 22:57:36.000000 torqueclient-0.5.7/torqueclient/api.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     6851 2024-01-26 22:57:36.000000 torqueclient-0.5.7/torqueclient/cache.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       22 2024-01-26 22:04:36.000000 torqueclient-0.5.7/torqueclient/version.py
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-01-26 23:05:57.345542 torqueclient-0.5.7/torqueclient.egg-info/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1031 2024-01-26 23:05:57.000000 torqueclient-0.5.7/torqueclient.egg-info/PKG-INFO
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      319 2024-01-26 23:05:57.000000 torqueclient-0.5.7/torqueclient.egg-info/SOURCES.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        1 2024-01-26 23:05:57.000000 torqueclient-0.5.7/torqueclient.egg-info/dependency_links.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       25 2024-01-26 23:05:57.000000 torqueclient-0.5.7/torqueclient.egg-info/requires.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       13 2024-01-26 23:05:57.000000 torqueclient-0.5.7/torqueclient.egg-info/top_level.txt
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-04-27 17:49:28.562573 torqueclient-0.6.0/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    34523 2024-04-27 17:48:33.000000 torqueclient-0.6.0/LICENSE
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1031 2024-04-27 17:49:28.562573 torqueclient-0.6.0/PKG-INFO
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      502 2023-02-19 01:57:21.000000 torqueclient-0.6.0/README.md
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      107 2023-02-19 01:57:21.000000 torqueclient-0.6.0/pyproject.toml
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       38 2024-04-27 17:49:28.562573 torqueclient-0.6.0/setup.cfg
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      973 2023-02-19 01:57:21.000000 torqueclient-0.6.0/setup.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-04-27 17:49:28.562573 torqueclient-0.6.0/torqueclient/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       85 2024-01-26 22:57:36.000000 torqueclient-0.6.0/torqueclient/__init__.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    18992 2024-04-27 17:39:34.000000 torqueclient-0.6.0/torqueclient/api.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     6876 2024-04-27 17:39:34.000000 torqueclient-0.6.0/torqueclient/cache.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       22 2024-04-27 17:44:12.000000 torqueclient-0.6.0/torqueclient/version.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-04-27 17:49:28.562573 torqueclient-0.6.0/torqueclient.egg-info/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1031 2024-04-27 17:49:28.000000 torqueclient-0.6.0/torqueclient.egg-info/PKG-INFO
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      319 2024-04-27 17:49:28.000000 torqueclient-0.6.0/torqueclient.egg-info/SOURCES.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        1 2024-04-27 17:49:28.000000 torqueclient-0.6.0/torqueclient.egg-info/dependency_links.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       25 2024-04-27 17:49:28.000000 torqueclient-0.6.0/torqueclient.egg-info/requires.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       13 2024-04-27 17:49:28.000000 torqueclient-0.6.0/torqueclient.egg-info/top_level.txt
```

### Comparing `torqueclient-0.5.7/LICENSE` & `torqueclient-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torqueclient-0.5.7/PKG-INFO` & `torqueclient-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torqueclient
-Version: 0.5.7
+Version: 0.6.0
 Summary: Python client for mediawiki/torque
 Home-page: https://code.librehq.com/ots/mediawiki/torque
 Author: Open Tech Strategies, LLC
 Author-email: frankduncan@opentechstrategies.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `torqueclient-0.5.7/setup.py` & `torqueclient-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `torqueclient-0.5.7/torqueclient/api.py` & `torqueclient-0.6.0/torqueclient/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,37 +30,39 @@
     is then set as a synonym alias for collections.  For example, if the
     COLLECTIONS_ALIAS on the server is set to "competitions", then there's
     an additional attribute as follows:
 
     competition : Collections
         All the competitions available from the server
 
-
     Methods
     -------
     search(search_term, collection_name=None)
         searches for documents
     bulk_fetch(documents, num_threads=10)
         eager loads the documents
     """
 
-    def __init__(self, url, username, password, cache=DiskCache()):
+    def __init__(self, url, username, password, cache=None):
         """Initializes to a running torque system available from
         a mediawiki instance at URL that is accessed using USERNAME
         and PASSWORD.
 
         URL must be fully qualified with the protocol, ie
         http://your.domain.tld/
 
         CACHE is an optional cache that implements cache.Cache,
         defaulting to the DiskCache"""
         (scheme, host) = url.split("://")
+        self.url = url
         self.site = mwclient.Site(host, path="/", scheme=scheme, reqs={"timeout": 300})
         self.site.login(username, password)
         self.cache = cache
+        if not self.cache:
+            self.cache = DiskCache()
 
         self.collections = Collections(self)
 
         information = self._get_data("/system")
         self.documents_alias = None
         if "collections_alias" in information:
             self.documents_alias = information["documents_alias"]
@@ -365,14 +367,18 @@
     data : dict
         initially set to None (until lazy loaded), a dictionary of names to values
 
     Methods
     -------
     keys()
         all the field keys
+    upload_attachment(name, column, stream)
+        upload an attachment
+    attachments()
+        the attachments for this document
     uri()
         the uri of the document, which is a useful index when creating a cache
     original()
         the original form of the document, as uploaded in the collection
     latest()
         the most recent form of the document, which is the default
     """
@@ -412,20 +418,47 @@
         return d
 
     def uri(self):
         """Returns the uri of the doucment on the server."""
         version_string = ""
         if self.version != "latest":
             version_string = "/version/" + self.version
-        return "/collections/%s/documents/%s%s" % (self.collection.name, self.key, version_string)
+        return "/collections/%s/documents/%s%s" % (
+            self.collection.name,
+            self.key,
+            version_string,
+        )
 
     def keys(self):
         """Returns the list of all the field keys available on the server."""
         return self._get_data().keys()
 
+    def upload_attachment(self, name, column, stream):
+        """Uploads an attachment named via NAME, permissioned to column
+        COLUMN, and provided by the file stream STREAM.  This attachment
+        will get attached to the current document.
+
+        The user must have torque-admin permissions to upload."""
+        self.torque.site.raw_call(
+            "api",
+            {
+                "action": "torqueuploadattachment",
+                "format": "json",
+                "collection_name": self.collection.name,
+                "object_id": self.key,
+                "permissions_field": column,
+                "attachment_name": name,
+            },
+            {"attachment": stream.read()},
+        )
+
+    def attachments(self):
+        """Returns the list of all attachments for this document."""
+        return Attachments(self.torque, self)
+
     def _get_data(self):
         """Gets the data for the document from the server.
 
         There's logic here as well that will refresh data if new, as well
         as pull from cache as appropriate."""
         if self.data is None:
             if self.torque.cache is not None:
@@ -443,7 +476,115 @@
                 and not self.torque.cache.contains_document_data(
                     self, self.collection.last_updated
                 )
             ):
                 self.torque.cache.persist_document(self, self.collection.last_updated)
 
         return self.data
+
+
+class Attachments:
+    """
+    A container object for all the attachments on given Document.
+
+    This is a list/dict like class that represents the attachments on the server.
+
+    It can indexed like a dict, but also iterated over like a list.  So the
+    following work:
+
+        Torque(...).collections["XYZ"].documents["123"].attachments["attachment_1.pdf"]
+
+    and
+
+        for collection in Torque(...).collections:
+            for document in collection.documents:
+                for attachment in document.attachments:
+                    ...
+
+    It stores the list of attachments in memory, so getting the list of attachments
+    requires calling into document.attachments again.  However, each time `.get()` is
+    called, it will fetch the most recent version of the attachment from the server.
+
+    Attributes
+    ----------
+    torque : Torque
+        The parent torque object
+    document: Collection
+        The parent Collection object
+    names: list
+        The names of the available attachments
+    """
+
+    def __init__(self, torque, document):
+        self.torque = torque
+        self.document = document
+        self.attachments = {
+            a["name"]: Attachment(torque, document, a["name"], a["size"])
+            for a in self.torque._get_data(
+                "/collections/%s/documents/%s/attachments"
+                % (document.collection.name, document.key)
+            )
+        }
+        self.names = self.attachments.keys()
+
+    def __iter__(self):
+        self.idx = 0
+        return self
+
+    def __next__(self):
+        if self.idx < len(self.names):
+            name = self.names[self.idx]
+            self.idx += 1
+            return self.attachments[name]
+        else:
+            raise StopIteration()
+
+    def __getitem__(self, name):
+        return self.attachments[name]
+
+
+class Attachment:
+    """An Attachment
+
+    A lazy loaded instance of an attachment on the torque server.  This does
+    not load any data from the server until accessed (via get())
+
+    Attributes
+    ----------
+    torque : Torque
+        the parent torque object
+    collection : Torque
+        the parent collection object
+    name : str
+        the name of the attachment
+    size : int
+        the size of the attachment
+
+    Methods
+    -------
+    download(destination=None)
+        retrieves the attachment from the server and writes it to destination if provided,
+        otherwise returns it
+    """
+
+    def __init__(self, torque, document, name, size):
+        self.torque = torque
+        self.document = document
+        self.name = name
+        self.size = size
+
+    def download(self, destination=None):
+        url = (
+            "%s/index.php/Special:TorqueAttachment?collection_name=%s&id=%s&attachment=%s"
+            % (
+                self.torque.url,
+                self.document.collection.name,
+                self.document.key,
+                self.name,
+            )
+        )
+        if destination is not None:
+            res = self.torque.site.connection.get(url, stream=True)
+            for chunk in res.iter_content(1024):
+                destination.write(chunk)
+        else:
+            return self.torque.site.connection.get(url).content
```

### Comparing `torqueclient-0.5.7/torqueclient/cache.py` & `torqueclient-0.6.0/torqueclient/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,17 @@
 
     def _document_path(self, document):
         """Internal function to get the disk cache path for DOCUMENT"""
         version_string = ""
         if document.version != "latest":
             version_string = "_" + document.version
         return os.path.join(
-            self.location, document.collection.name, "%s%s.json" % (document.key, version_string)
+            self.location,
+            document.collection.name,
+            "%s%s.json" % (document.key, version_string),
         )
 
     def contains_document_data(self, document, last_updated_time):
         """Implements the Cache interface on disk."""
         if not os.path.exists(self._document_path(document)):
             return False
         with open(self._document_path(document), "r") as f:
```

### Comparing `torqueclient-0.5.7/torqueclient.egg-info/PKG-INFO` & `torqueclient-0.6.0/torqueclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torqueclient
-Version: 0.5.7
+Version: 0.6.0
 Summary: Python client for mediawiki/torque
 Home-page: https://code.librehq.com/ots/mediawiki/torque
 Author: Open Tech Strategies, LLC
 Author-email: frankduncan@opentechstrategies.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

