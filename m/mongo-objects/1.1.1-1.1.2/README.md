# Comparing `tmp/mongo_objects-1.1.1.tar.gz` & `tmp/mongo_objects-1.1.2.tar.gz`

## Comparing `mongo_objects-1.1.1.tar` & `mongo_objects-1.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/.readthedocs.yaml
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/requirements.txt
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/docs/source/MongoDictProxy.rst
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/docs/source/MongoListProxy.rst
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/docs/source/MongoSingleProxy.rst
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/docs/source/MongoUserDict.rst
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/docs/source/conf.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/docs/source/customization.rst
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/docs/source/index.rst
--rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/docs/source/quickstart.rst
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/docs/source/sample.rst
--rw-r--r--   0        0        0    33028 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/src/mongo_objects.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tests/conftest.py
--rw-r--r--   0        0        0    27988 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tests/test_MongoDictProxy.py
--rw-r--r--   0        0        0    31396 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tests/test_MongoListProxy.py
--rw-r--r--   0        0        0    27139 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tests/test_MongoSingleProxy.py
--rw-r--r--   0        0        0    41395 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tests/test_MongoUserDict.py
--rw-r--r--   0        0        0    13920 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tests/test_PolymorphicMongoDictProxy.py
--rw-r--r--   0        0        0    15993 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tests/test_PolymorphicMongoListProxy.py
--rw-r--r--   0        0        0    15550 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tests/test_PolymorphicMongoSingleProxy.py
--rw-r--r--   0        0        0    13745 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tests/test_PolymorphicMongoUserDict.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tests/test_proxy_combo.py
--rwxr-xr-x   0        0        0     1326 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tools/buildProject
--rwxr-xr-x   0        0        0      813 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tools/runTests
--rwxr-xr-x   0        0        0     1960 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tools/setupPythonVenv
--rwxr-xr-x   0        0        0      498 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tools/updateRequirements
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/LICENSE.txt
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/README.rst
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/requirements.txt
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/docs/source/MongoDictProxy.rst
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/docs/source/MongoListProxy.rst
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/docs/source/MongoSingleProxy.rst
+-rw-r--r--   0        0        0     8153 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/docs/source/MongoUserDict.rst
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/docs/source/conf.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/docs/source/customization.rst
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/docs/source/index.rst
+-rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/docs/source/quickstart.rst
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/docs/source/sample.rst
+-rw-r--r--   0        0        0    33427 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/src/mongo_objects.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tests/conftest.py
+-rw-r--r--   0        0        0    27988 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tests/test_MongoDictProxy.py
+-rw-r--r--   0        0        0    31396 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tests/test_MongoListProxy.py
+-rw-r--r--   0        0        0    27139 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tests/test_MongoSingleProxy.py
+-rw-r--r--   0        0        0    41394 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tests/test_MongoUserDict.py
+-rw-r--r--   0        0        0    13920 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tests/test_PolymorphicMongoDictProxy.py
+-rw-r--r--   0        0        0    16023 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tests/test_PolymorphicMongoListProxy.py
+-rw-r--r--   0        0        0    15580 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tests/test_PolymorphicMongoSingleProxy.py
+-rw-r--r--   0        0        0    13775 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tests/test_PolymorphicMongoUserDict.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tests/test_proxy_combo.py
+-rwxr-xr-x   0        0        0     1326 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tools/buildProject
+-rwxr-xr-x   0        0        0      813 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tools/runTests
+-rwxr-xr-x   0        0        0     2399 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tools/setupPythonVenv
+-rwxr-xr-x   0        0        0      498 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tools/updateRequirements
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/README.rst
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/PKG-INFO
```

### Comparing `mongo_objects-1.1.1/.readthedocs.yaml` & `mongo_objects-1.1.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.1.1/requirements.txt` & `mongo_objects-1.1.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.1.1/docs/source/conf.py` & `mongo_objects-1.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.1.1/docs/source/index.rst` & `mongo_objects-1.1.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.1.1/docs/source/quickstart.rst` & `mongo_objects-1.1.2/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.1.1/src/mongo_objects.py` & `mongo_objects-1.1.2/src/mongo_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,24 @@
 
 
 
 ################################################################################
 # Custom exceptions
 ################################################################################
 
-class MongoObjectReadOnly( Exception ):
+class MongoObjectsAuthFailed( Exception ):
     pass
 
-class MongoObjectAuthFailed( Exception ):
+class MongoObjectsDocumentModified( Exception ):
+    pass
+
+class MongoObjectsReadOnly( Exception ):
+    pass
+
+class MongoObjectsSubclassError( Exception ):
     pass
 
 
 ################################################################################
 # MongoDB document wrappers
 ################################################################################
 
@@ -60,21 +66,21 @@
         '''Initialize the custom UserDict object
         Flag readonly objects appropriately'''
         super().__init__( doc )
         self.readonly = readonly
 
         # Authorize creating this object prior to returning to the user
         if not self.authorize_init():
-            raise MongoObjectAuthFailed
+            raise MongoObjectsAuthFailed
 
 
     @classmethod
     def add_object_version_filter( cls, filter, object_version ):
-        '''Implement automatic object version filtering for find() and find_one()
-        The command-line object-version affects if and how to implement
+        '''Implement automatic object version filtering for find() and find_one().
+        The object-version keyword argument affects if and how to implement
         object version filtering.'''
         if cls.object_version is not None:
             # False suppresses automatic object_version filtering
             if object_version is False:
                 pass
             # None (the default) filters the query to the current class object version
             elif object_version is None:
@@ -89,28 +95,31 @@
 
 
     # Authorization hooks()
     # The user may call these hooks to authorize various CRUD operations
     def authorize_init( self ):
         '''Called after the document object is initialized but
         before it is returned to the user.
-        If the return value is not truthy, an exception is raised.'''
+        If the return value is not truthy, a MongoObjectsAuthFailed exception
+        is raised.'''
         return True
 
     def authorize_delete( self ):
         '''Called before the current document is deleted.
-        If the return value is not truthy, an exception is raised.'''
+        If the return value is not truthy, a MongoObjectsAuthFailed
+        exception is raised.'''
         return True
 
     @classmethod
     def authorize_pre_read( cls ):
         '''Called before a read operation is performed.
         This is a class method as no data has been read and no
         document object has been created.
-        If the return value is not truthy, an exception is raised.'''
+        If the return value is not truthy, a MongoObjectsAuthFailed
+        exception is raised.'''
         return True
 
     def authorize_read( self ):
         '''Called after a document has been read but before the
         data is returned to the user.
         If the return value is not truthy, the data will
         not be returned.
@@ -119,15 +128,16 @@
         returned by the underlying MongoDB find_one() call. If the
         document returned does not pass authorization, no attempt is
         made to locate another matching document.'''
         return True
 
     def authorize_save( self ):
         '''Called before the current document is saved.
-        If the return value is not truthy, an exception is raised.'''
+        If the return value is not truthy, a MongoObjectsAuthFailed
+        exception is raised.'''
         return True
 
 
     @classmethod
     def collection( cls ):
         '''Return the collection object from the active database for the named collection'''
         return cls.database.get_collection( cls.collection_name )
@@ -135,30 +145,32 @@
 
     def delete( self ):
         '''Delete the current object
         Remove the id so save() will know this is a new object if we try to re-save.'''
         if '_id' in self:
             # Authorize deleting this object
             if not self.authorize_delete():
-                raise MongoObjectAuthFailed
+                raise MongoObjectsAuthFailed
             self.collection().find_one_and_delete( { '_id' : ObjectId( self['_id'] ) } )
             del self['_id']
 
 
     @classmethod
     def find( cls, filter={}, projection=None, readonly=None, object_version=None, **kwargs ):
         '''Return matching documents as instances of this class'''
         # Authorize reading at all
         if not cls.authorize_pre_read():
-            raise MongoObjectAuthFailed
+            raise MongoObjectsAuthFailed
 
         # if readonly is None, by default force queries with a projection to be read-only
-        # otherwise, accept the (presumably boolean) value provided by the user
+        # otherwise, accept the value provided by the user
         if readonly is None:
             readonly = projection is not None
+        else:
+            readonly = bool( readonly )
 
         # automatically filter by object version if requested
         if cls.object_version is not None:
             filter = cls.add_object_version_filter( filter, object_version )
 
         for doc in cls.collection().find( filter, projection, **kwargs ):
             obj = cls(doc, readonly=readonly)
@@ -168,20 +180,22 @@
 
 
     @classmethod
     def find_one( cls, filter={}, projection=None, readonly=None, object_version=None, no_match=None, **kwargs ):
         '''Return a single matching document as an instance of this class or None'''
         # Authorize reading at all
         if not cls.authorize_pre_read():
-            raise MongoObjectAuthFailed
+            raise MongoObjectsAuthFailed
 
         # if readonly is None, by default force queries with a projection to be read-only
-        # otherwise, accept the (presumably boolean) value provided by the user
+        # otherwise, accept the value provided by the user
         if readonly is None:
             readonly = projection is not None
+        else:
+            readonly = bool( readonly )
 
         # automatically filter by object version if requested
         if cls.object_version is not None:
             filter = cls.add_object_version_filter( filter, object_version )
 
         doc = cls.collection().find_one( filter, projection, **kwargs )
         if doc is not None:
@@ -266,19 +280,19 @@
 
         # internal class to note if a metadata field has added and had no original value
         class NewFieldAdded( object ):
             pass
 
         # authorize saving this document
         if not self.authorize_save():
-            raise MongoObjectAuthFailed
+            raise MongoObjectsAuthFailed
 
         # refuse to save a read-only document
         if self.readonly:
-            raise MongoObjectReadOnly( f"Can't save readonly object {type(self)} at {id(self)}" )
+            raise MongoObjectsReadOnly( f"Can't save readonly object {type(self)} at {id(self)}" )
 
         # Use a dictionary to record original metadata in case they need to be rolled back
         # These metadata values should never be None, so during rollback we remove any values
         # for which get() returned None.
         original_metadata = {}
 
         # set updated timestamp
@@ -309,15 +323,16 @@
             else:
                 result = self.collection().find_one_and_replace(
                     { '_id' : self['_id'], '_updated' : original_metadata['_updated'] },
                     self.data,
                     return_document=ReturnDocument.AFTER )
 
                 # on failure, we assume the document has been updated elsewhere and raise an exception
-                assert result is not None, f"document {self.id()} already updated"
+                if result is None:
+                    raise MongoObjectsDocumentModified( f"document {self.id()} already updated" )
 
         # on any error roll back to the original metadata
         except Exception as e:
             for (k, v) in original_metadata.items():
                 # If the original value is None, assume we added the field and should remove it
                 if v is None:
                     del self[k]
@@ -366,23 +381,23 @@
         '''auto-register every PolymorphicMongoUserDict subclass'''
         super().__init_subclass__(**kwargs)
         try:
             if getattr( cls, 'subclass_key', None ) is not None:
                 assert cls.subclass_key not in cls.subclass_map, f"duplicate subclass_key for {type(cls)}"
                 cls.subclass_map[ cls.subclass_key ] = cls
         except Exception as e:
-            raise Exception( 'PolymorphicMongoUserDict(): unable to register subclass' ) from e
+            raise MongoObjectsSubclassError( 'PolymorphicMongoUserDict(): unable to register subclass' ) from e
 
 
     @classmethod
     def find( cls, filter={}, projection=None, readonly=None, **kwargs ):
         '''Return matching documents as appropriate subclass instances'''
         # Authorize reading at all
         if not cls.authorize_pre_read():
-            raise MongoObjectAuthFailed
+            raise MongoObjectsAuthFailed
 
         # if a projection is provided, force the resulting object to be read-only
         readonly = readonly or projection is not None
 
         for doc in cls.collection().find( filter, projection, **kwargs ):
             obj = cls.instantiate(doc, readonly=readonly)
             # Authorize reading this particular document object before returning it
@@ -391,15 +406,15 @@
 
 
     @classmethod
     def find_one( cls, filter={}, projection=None, readonly=None, no_match=None, **kwargs ):
         '''Return a single matching document as the appropriate subclass or None'''
         # Authorize reading at all
         if not cls.authorize_pre_read():
-            raise MongoObjectAuthFailed
+            raise MongoObjectsAuthFailed
 
         # if a projection is provided, force the resulting object to be read-only
         readonly = readonly or projection is not None
 
         doc = cls.collection().find_one( filter, projection, **kwargs )
         if doc is not None:
             obj = cls.instantiate( doc, readonly=readonly )
@@ -547,15 +562,15 @@
         '''auto-register every PolymorphicMongoBaseProxy subclass'''
         super().__init_subclass__(**kwargs)
         try:
             if getattr( cls, 'proxy_subclass_key', None ) is not None:
                 assert cls.proxy_subclass_key not in cls.proxy_subclass_map, f"duplicate proxy_subclass_key for {type(cls)}"
                 cls.proxy_subclass_map[ cls.proxy_subclass_key ] = cls
         except Exception as e:
-            raise Exception( 'PolymorphicMongoBaseProxy(): unable to register subclass' ) from e
+            raise MongoObjectsSubclassError( 'PolymorphicMongoBaseProxy(): unable to register subclass' ) from e
 
 
     @classmethod
     def create( cls, parent, subdoc={}, autosave=True ):
         '''Add the proxy_subclass_key before passing to the base class create()'''
         if cls.proxy_subclass_key is not None:
             subdoc[ cls.proxy_subclass_key_name ] = cls.proxy_subclass_key
@@ -823,15 +838,15 @@
     '''
 
     @classmethod
     def create( cls, parent, subdoc={}, key=None, autosave=True ):
         '''Add a new single subdocument dictionary to the parent object.
         No new key is auto-assigned as single subdocuments are assigned to fixed keys.
         The key can be defined in the class as "container_name"
-        or overriden on the command line as "key".
+        or overriden in the function call as "key".
         Return the new proxy object.
         '''
         if key is None:
             key = cls.container_name
         parent[ key ] = subdoc
         if autosave:
             parent.save()
```

### Comparing `mongo_objects-1.1.1/tests/test_MongoDictProxy.py` & `mongo_objects-1.1.2/tests/test_MongoDictProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.1.1/tests/test_MongoListProxy.py` & `mongo_objects-1.1.2/tests/test_MongoListProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.1.1/tests/test_MongoSingleProxy.py` & `mongo_objects-1.1.2/tests/test_MongoSingleProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.1.1/tests/test_MongoUserDict.py` & `mongo_objects-1.1.2/tests/test_MongoUserDict.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,15 +212,15 @@
         # verify there is a current object version
         assert MMUD.object_version is not None
 
         # Create an invalid object; BSON dictionary keys must be strings
         obj = MMUD( { 1 : "not valid BSON"} )
         assert '_objver' not in obj
 
-        # saving the object will raise an exceptionsave the object and verify the version was added to the document
+        # saving the object will raise an exception
         with pytest.raises( Exception ):
             obj.save()
 
         # verify that the object version was removed during rollback
         assert '_objver' not in obj
 
 
@@ -422,15 +422,15 @@
         obj.save()
 
         # verify a newer timestamp
         assert obj['_updated'] > obj2['_updated']
 
         # try to save second object; it won't work
         original_updated = obj2.get('_updated')
-        with pytest.raises( Exception ):
+        with pytest.raises( mongo_objects.MongoObjectsDocumentModified ):
             obj2.save()
 
         # verify that obj2 _updated is the original value
         assert obj2.get('_updated') == original_updated
 
         # locate object on disk and verify _updated matches obj (not obj2)
         doc = MMUD.collection().find_one( { '_id' : obj['_id'] } )
@@ -440,29 +440,29 @@
     def test_save_readonly( self, getPopulatedMMUDClass ):
         '''Test attempting to save a readonly object'''
         MMUD = getPopulatedMMUDClass
         result = MMUD.find_one( readonly=True )
         assert result.readonly is True
 
         # saving a readonly document produces an exception
-        with pytest.raises( Exception ):
+        with pytest.raises( mongo_objects.MongoObjectsReadOnly ):
             result.save()
 
 
     def test_save_no_auth( self, getPopulatedMMUDClass ):
         '''Test attempting to save a document without authorization'''
         class LocalMMUD( getPopulatedMMUDClass):
             def authorize_save( self ):
                 return False
 
         obj = LocalMMUD.find_one()
         original = dict( obj )
 
         # verify saving a document without authorization produces an exception
-        with pytest.raises( mongo_objects.MongoObjectAuthFailed ):
+        with pytest.raises( mongo_objects.MongoObjectsAuthFailed ):
             obj.save()
 
         # verify nothing was saved
         assert obj['_updated'] == original['_updated']
 
 
 
@@ -518,15 +518,15 @@
 
         obj = LocalMMUD.find_one()
 
         # note the number of documents in the database
         count = LocalMMUD.collection().count_documents( {} )
 
         # verify deleting a document without authorization produces an exception
-        with pytest.raises( mongo_objects.MongoObjectAuthFailed ):
+        with pytest.raises( mongo_objects.MongoObjectsAuthFailed ):
             obj.delete()
 
         # verify the database document count hasn't changed
         assert count == LocalMMUD.collection().count_documents( {} )
 
 
 
@@ -564,15 +564,15 @@
 
     def test_init_no_auth( self, getMMUDClass, sampleData ):
         class LocalMMUD( getMMUDClass):
             def authorize_init( self ):
                 return False
 
         # verify initializing a document without authorization produces an exception
-        with pytest.raises( mongo_objects.MongoObjectAuthFailed ):
+        with pytest.raises( mongo_objects.MongoObjectsAuthFailed ):
             obj = LocalMMUD( sampleData[0] )
 
 
     def test_add_object_version( self ):
         '''Verify add_object_version adds the correct filter
         The original filter should be left intact.'''
         class LocalClass( mongo_objects.MongoUserDict ):
@@ -800,15 +800,15 @@
         class LocalMMUD( getPopulatedMMUDClass ):
             @classmethod
             def authorize_pre_read( cls ):
                 return False
 
         # verify reading documents without pre-read authorization produces an exception
         # must convert to a list or the generator is never called
-        with pytest.raises( mongo_objects.MongoObjectAuthFailed ):
+        with pytest.raises( mongo_objects.MongoObjectsAuthFailed ):
             list( LocalMMUD.find() )
 
 
     def test_find_no_auth_1( self, getPopulatedMMUDClass ):
         '''Test attempting to read without authorization'''
         class LocalMMUD( getPopulatedMMUDClass):
             def authorize_read( self ):
@@ -999,15 +999,15 @@
         '''Test attempting to read without pre-authorization'''
         class LocalMMUD( getPopulatedMMUDClass ):
             @classmethod
             def authorize_pre_read( cls ):
                 return False
 
         # verify reading a document without pre-read authorization produces an exception
-        with pytest.raises( mongo_objects.MongoObjectAuthFailed ):
+        with pytest.raises( mongo_objects.MongoObjectsAuthFailed ):
             LocalMMUD.find_one()
 
 
     def test_find_one_no_auth( self, getPopulatedMMUDClass ):
         '''Test attempting to read without authorization'''
         class LocalMMUD( getPopulatedMMUDClass):
             def authorize_read( self ):
```

### Comparing `mongo_objects-1.1.1/tests/test_PolymorphicMongoDictProxy.py` & `mongo_objects-1.1.2/tests/test_PolymorphicMongoDictProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.1.1/tests/test_PolymorphicMongoListProxy.py` & `mongo_objects-1.1.2/tests/test_PolymorphicMongoListProxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         }
 
         # verify our local subclass map namespace didn't affect the module base class map
         assert len( mongo_objects.PolymorphicMongoBaseProxy.proxy_subclass_map ) == 0
 
 
     def test_init_subclass_duplicate_key( self ):
-        with pytest.raises( Exception ):
+        with pytest.raises( mongo_objects.MongoObjectsSubclassError ):
 
             class MyTestClassBase( mongo_objects.PolymorphicMongoListProxy ):
                 # create our own local testing namespace
                 proxy_subclass_map = {}
 
             class MyTestSubclassA( MyTestClassBase ):
                 proxy_subclass_key = 'A'
```

### Comparing `mongo_objects-1.1.1/tests/test_PolymorphicMongoSingleProxy.py` & `mongo_objects-1.1.2/tests/test_PolymorphicMongoSingleProxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
         }
 
         # verify our local subclass map namespace didn't affect the module base class map
         assert len( mongo_objects.PolymorphicMongoBaseProxy.proxy_subclass_map ) == 0
 
 
     def test_init_subclass_duplicate_key( self ):
-        with pytest.raises( Exception ):
+        with pytest.raises( mongo_objects.MongoObjectsSubclassError ):
 
             class MyTestClassBase( mongo_objects.PolymorphicMongoSingleProxy ):
                 # create our own local testing namespace
                 proxy_subclass_map = {}
 
             class MyTestSubclassA( MyTestClassBase ):
                 proxy_subclass_key = 'A'
```

### Comparing `mongo_objects-1.1.1/tests/test_PolymorphicMongoUserDict.py` & `mongo_objects-1.1.2/tests/test_PolymorphicMongoUserDict.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         }
 
         # verify our local subclass map namespace didn't affect the module base class map
         assert len( mongo_objects.PolymorphicMongoUserDict.subclass_map ) == 0
 
 
     def test_init_subclass_duplicate_key( self ):
-        with pytest.raises( Exception ):
+        with pytest.raises( mongo_objects.MongoObjectsSubclassError ):
 
             class MyTestClassBase( mongo_objects.PolymorphicMongoUserDict ):
                 # create our own local testing namespace
                 subclass_map = {}
 
             class MyTestSubclassA( MyTestClassBase ):
                 subclass_key = 'A'
```

### Comparing `mongo_objects-1.1.1/tests/test_proxy_combo.py` & `mongo_objects-1.1.2/tests/test_proxy_combo.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.1.1/tools/buildProject` & `mongo_objects-1.1.2/tools/buildProject`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.1.1/tools/runTests` & `mongo_objects-1.1.2/tools/runTests`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.1.1/tools/setupPythonVenv` & `mongo_objects-1.1.2/tools/setupPythonVenv`

 * *Files 12% similar despite different names*

```diff
@@ -8,52 +8,64 @@
 PROJECT_NAME=$(basename ${PROJECT_DIR})
 VENV_DIR=${PROJECT_DIR}/venv
 
 # check the virtual environment version on MacOS
 if [[ "$(uname)" == "Darwin" ]]; then
 
     # Make sure Homebrew Python 3.12 is installed
-    if [[ ! -e /usr/local/bin/python3.12 ]]; then
+    # First check for Apple silicon location
+    if [[ -e /opt/homebrew/bin/python3.12  ]]; then
+        echo "Using Homebrew Python 3.12 on Apple silicon"
+        PYBINDIR=/opt/homebrew/bin
+
+    # Make sure Homebrew Python 3.12 is installed
+    elif [[ -e /usr/local/bin/python3.12  ]]; then
+        echo "Using Homebrew Python 3.12 on Intel"
+        PYBINDIR=/usr/local/bin
+
+    # Make sure Homebrew Python 3.12 is installed
+    else
         echo "Python 3.12 is not installed"
         exit 1
     fi
 
     # If the virtual environment exists, make sure the Python 3.12 version matches
-    if [[ -d ${VENV_DIR} && "$(/usr/local/bin/python3.12 -V)" != "$(${VENV_DIR}/bin/python3 -V)" ]]; then
+    if [[ -d ${VENV_DIR} && "$(${PYBINDIR}/python3.12 -V)" != "$(${VENV_DIR}/bin/python3 -V)" ]]; then
         echo Removing obsolete $(${VENV_DIR}/bin/python3 -V) virtual environment
         rm -rf ${VENV_DIR}
     fi
 fi
 
 
 # create virtual environment if it doesn't exist
 if [[ ! -d ${VENV_DIR} ]]; then
     # only implemented for MacOS
     if [[ "$(uname)" == "Darwin" ]]; then
-        /usr/local/bin/python3.12 -m venv ${VENV_DIR} --prompt "${PROJECT_NAME}-dev"
+        ${PYBINDIR}/python3.12 -m venv ${VENV_DIR} --prompt "${PROJECT_NAME}-dev"
         echo initialized virtual environment ${VENV_DIR}
+
+    else
+        echo "setupPythonVenv does not support OS $(uname)"
+        exit 1
     fi
 fi
 
 # activate virtual environment
-if [[ ! "$(which python)" -ef "${VENV_DIR}/bin/python3" ]]; then
-    source ${VENV_DIR}/bin/activate
-    echo activating virtual environment ${VENV_DIR}
-fi
+source ${VENV_DIR}/bin/activate
+echo activating virtual environment ${VENV_DIR}
 
 # read requirements.txt file and install or upgrade Python modules
 if [[ -f "${PROJECT_DIR}/requirements.txt" ]]; then
     echo updating Python modules
     # If we're using a proxy, download pysocks first as pip requires it
     if [ -n "${ALL_PROXY}" ]
     then
-        ALL_PROXY="" pip install --disable-pip-version-check pysocks
+        ALL_PROXY="" ${VENV_DIR}/bin/pip3 install --disable-pip-version-check pysocks
     fi
 
     # install setuptools and wheel first
-    pip install --disable-pip-version-check setuptools wheel
-
+    ${VENV_DIR}/bin/pip3 install --disable-pip-version-check setuptools wheel
     # now install all packages in the requirements file
-    cat ${PROJECT_DIR}/requirements.txt | xargs pip install --disable-pip-version-check
+    cat ${PROJECT_DIR}/requirements.txt | xargs ${VENV_DIR}/bin/pip3 install --disable-pip-version-check
     echo Python modules installed
 fi
```

### Comparing `mongo_objects-1.1.1/LICENSE.txt` & `mongo_objects-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.1.1/README.rst` & `mongo_objects-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.1.1/pyproject.toml` & `mongo_objects-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.1.1/PKG-INFO` & `mongo_objects-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mongo_objects
-Version: 1.1.1
+Version: 1.1.2
 Summary: Access MongoDB documents and subdocuments through user-defined UserDict and proxy objects.
 Project-URL: Homepage, https://github.com/lindstrom-j/mongo_objects
 Project-URL: Documentation, https://mongo-objects.headwaters.com.sg/en/latest/
 Project-URL: Issues, https://github.com/lindstrom-j/mongo_objects/issues
 Author-email: Jonathan Lindstrom <lindstrom.j@headwaters.com.sg>
 License: MIT License
 License-File: LICENSE.txt
```

