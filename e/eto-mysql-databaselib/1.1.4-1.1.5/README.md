# Comparing `tmp/eto-mysql-databaselib-1.1.4.tar.gz` & `tmp/eto_mysql_databaselib-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eto-mysql-databaselib-1.1.4.tar", last modified: Tue Feb 27 10:40:01 2024, max compression
+gzip compressed data, was "eto_mysql_databaselib-1.1.5.tar", last modified: Sat Apr 27 13:07:21 2024, max compression
```

## Comparing `eto-mysql-databaselib-1.1.4.tar` & `eto_mysql_databaselib-1.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-02-27 10:40:01.687621 eto-mysql-databaselib-1.1.4/
--rw-rw-rw-   0        0        0     1090 2024-02-20 10:00:19.000000 eto-mysql-databaselib-1.1.4/LICENSE
--rw-rw-rw-   0        0        0     6926 2024-02-27 10:40:01.683948 eto-mysql-databaselib-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     5032 2024-02-23 08:52:52.000000 eto-mysql-databaselib-1.1.4/README.md
--rw-rw-rw-   0        0        0      771 2024-02-27 10:37:00.000000 eto-mysql-databaselib-1.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-27 10:40:01.687621 eto-mysql-databaselib-1.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-27 10:40:01.587494 eto-mysql-databaselib-1.1.4/src/
-drwxrwxrwx   0        0        0        0 2024-02-27 10:40:01.655401 eto-mysql-databaselib-1.1.4/src/databaselib/
--rw-rw-rw-   0        0        0      180 2024-02-27 10:36:57.000000 eto-mysql-databaselib-1.1.4/src/databaselib/__init__.py
--rw-rw-rw-   0        0        0     6229 2024-02-27 10:36:43.000000 eto-mysql-databaselib-1.1.4/src/databaselib/databaseDevFriendlyAbstraction.py
--rw-rw-rw-   0        0        0     9821 2024-02-21 16:54:56.000000 eto-mysql-databaselib-1.1.4/src/databaselib/etodatabaselib.py
--rw-rw-rw-   0        0        0      693 2024-02-20 10:00:19.000000 eto-mysql-databaselib-1.1.4/src/databaselib/etohashlib.py
--rw-rw-rw-   0        0        0      266 2024-02-20 10:00:19.000000 eto-mysql-databaselib-1.1.4/src/databaselib/helper.py
-drwxrwxrwx   0        0        0        0 2024-02-27 10:40:01.682040 eto-mysql-databaselib-1.1.4/src/eto_mysql_databaselib.egg-info/
--rw-rw-rw-   0        0        0     6926 2024-02-27 10:40:01.000000 eto-mysql-databaselib-1.1.4/src/eto_mysql_databaselib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      444 2024-02-27 10:40:01.000000 eto-mysql-databaselib-1.1.4/src/eto_mysql_databaselib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-27 10:40:01.000000 eto-mysql-databaselib-1.1.4/src/eto_mysql_databaselib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-02-27 10:40:01.000000 eto-mysql-databaselib-1.1.4/src/eto_mysql_databaselib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-02-27 10:40:01.000000 eto-mysql-databaselib-1.1.4/src/eto_mysql_databaselib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 13:07:21.841908 eto_mysql_databaselib-1.1.5/
+-rw-rw-rw-   0        0        0     1090 2024-02-20 10:00:19.000000 eto_mysql_databaselib-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0     6926 2024-04-27 13:07:21.839399 eto_mysql_databaselib-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5032 2024-02-23 08:52:52.000000 eto_mysql_databaselib-1.1.5/README.md
+-rw-rw-rw-   0        0        0      771 2024-04-27 12:28:45.000000 eto_mysql_databaselib-1.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-27 13:07:21.841908 eto_mysql_databaselib-1.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-27 13:07:21.731033 eto_mysql_databaselib-1.1.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-27 13:07:21.783870 eto_mysql_databaselib-1.1.5/src/databaselib/
+-rw-rw-rw-   0        0        0      180 2024-04-27 12:28:39.000000 eto_mysql_databaselib-1.1.5/src/databaselib/__init__.py
+-rw-rw-rw-   0        0        0     8866 2024-04-27 12:47:20.000000 eto_mysql_databaselib-1.1.5/src/databaselib/databaseDevFriendlyAbstraction.py
+-rw-rw-rw-   0        0        0     9821 2024-02-21 16:54:56.000000 eto_mysql_databaselib-1.1.5/src/databaselib/etodatabaselib.py
+-rw-rw-rw-   0        0        0      693 2024-02-20 10:00:19.000000 eto_mysql_databaselib-1.1.5/src/databaselib/etohashlib.py
+-rw-rw-rw-   0        0        0      266 2024-02-20 10:00:19.000000 eto_mysql_databaselib-1.1.5/src/databaselib/helper.py
+drwxrwxrwx   0        0        0        0 2024-04-27 13:07:21.835052 eto_mysql_databaselib-1.1.5/src/eto_mysql_databaselib.egg-info/
+-rw-rw-rw-   0        0        0     6926 2024-04-27 13:07:21.000000 eto_mysql_databaselib-1.1.5/src/eto_mysql_databaselib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2024-04-27 13:07:21.000000 eto_mysql_databaselib-1.1.5/src/eto_mysql_databaselib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 13:07:21.000000 eto_mysql_databaselib-1.1.5/src/eto_mysql_databaselib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-27 13:07:21.000000 eto_mysql_databaselib-1.1.5/src/eto_mysql_databaselib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-27 13:07:21.000000 eto_mysql_databaselib-1.1.5/src/eto_mysql_databaselib.egg-info/top_level.txt
```

### Comparing `eto-mysql-databaselib-1.1.4/LICENSE` & `eto_mysql_databaselib-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eto-mysql-databaselib-1.1.4/PKG-INFO` & `eto_mysql_databaselib-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eto-mysql-databaselib
-Version: 1.1.4
+Version: 1.1.5
 Summary: A library with the sole purpose of making connections to mysql databases easier
 Author-email: Eto_chan <etochandev@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Etozinhachan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `eto-mysql-databaselib-1.1.4/README.md` & `eto_mysql_databaselib-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `eto-mysql-databaselib-1.1.4/pyproject.toml` & `eto_mysql_databaselib-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eto-mysql-databaselib"
-version = "1.1.4"
+version = "1.1.5"
 description = "A library with the sole purpose of making connections to mysql databases easier"
 readme = "README.md"
 authors = [{name = "Eto_chan", email = "etochandev@gmail.com"}]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `eto-mysql-databaselib-1.1.4/src/databaselib/databaseDevFriendlyAbstraction.py` & `eto_mysql_databaselib-1.1.5/src/databaselib/databaseDevFriendlyAbstraction.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,63 @@
 import databaselib.etodatabaselib as mycooldatabase
 import databaselib.etohashlib as mycoolhashlib
 
 idColumnName = "id"
 usernameColumnName = "username"
 passwordColumnName = "password"
+emailColumnName = "email"
 saltColumnName = "salt"
 usersTableName = "users"
 
 class User():
-    def __init__(self, id:int, username:str, password_hashed:str):
+    def __init__(self, id:int, username:str, email:str, password_hashed:str):
         
         self._id = id
         self._username = username
+        self._email = email
         self._password = password_hashed
 
     def __repr__(self):
 
-        return f"\nUser Info:\n{"":->20}\nId: {self.id}\nUsername: {self.username}\nPassword: {self.password}\n{"":->20}"
+        return f"\nUser Info:\n{"":->20}\nId: {self.id}\nUsername: {self.username}\nEmail: {self.email}\nPassword: {self.password}\n{"":->20}"
 
     # Getters
 
     @property
     def id(self):
         return self._id
     
     @property
     def username(self):
         return self._username
     
     @property
+    def email(self):
+        return self._email
+        
+    @property
     def password(self):
         return self._password
     
     # Setters
 
     @username.setter
     def username(self, new_username):
         
         editionSucceeded:bool = mycooldatabase.edit_rows(usersTableName, {f"{usernameColumnName}": f"{new_username}"}, f"{idColumnName} = {self.id}", [f"{usernameColumnName}"])
         if editionSucceeded:
             self._username = new_username
 
+    @email.setter
+    def email(self, new_email):
+
+        editionSucceeded:bool = mycooldatabase.edit_rows(usersTableName, {f"{emailColumnName}": f"{new_email}"}, f"{idColumnName} = {self.id}", [f"{emailColumnName}"])
+        if editionSucceeded:
+            self._email = new_email
+
     @password.setter
     def password(self, new_password):
         (hashed_password, salt) = mycoolhashlib.generateSaltHash(new_password)
         editionSucceeded:bool = mycooldatabase.edit_rows(usersTableName, {f"{passwordColumnName}": f"{hashed_password}", f"{saltColumnName}": f"{salt}"}, f"{idColumnName} = {self.id}")
         #print(editionSucceeded)
         if editionSucceeded:
             self._password = hashed_password
@@ -58,29 +71,39 @@
     dictionaryToCompare = {f"{usernameColumnName}": f"{username}"}
     if usernameColumnResults == None:
         return False
     if not dictionaryToCompare in usernameColumnResults:
         return False
     return True
 
-def registerUser(username:str, password:str) -> User:
+def userExistsByEmail(email: str) -> bool:
+    emailColumnResults = mycooldatabase.get_rows(usersTableName, [f"{emailColumnName}"])
+    dictionaryToCompare = {f"{emailColumnName}": f"{email}"}
+    if emailColumnResults == None:
+        return False
+    if not dictionaryToCompare in emailColumnResults:
+        return False
+    return True
+
+def registerUser(username:str, email:str, password:str) -> User:
     try:
         global usernameColumnName
         global passwordColumnName
+        global emailColumnName
         global usersTableName
         global saltColumnName
         (hashed_password, salt) = mycoolhashlib.generateSaltHash(password)
-        mycooldatabase.createTable(usersTableName, {f"{idColumnName}": "INT PRIMARY KEY NOT NULL AUTO_INCREMENT", f"{usernameColumnName}": "VARCHAR(100) NOT NULL", f"{passwordColumnName}": "VARCHAR(150) NOT NULL", f"{saltColumnName}": "VARCHAR(150) NOT NULL"}, True)
+        mycooldatabase.createTable(usersTableName, {f"{idColumnName}": "INT PRIMARY KEY NOT NULL AUTO_INCREMENT", f"{usernameColumnName}": "VARCHAR(100) NOT NULL", f"{emailColumnName}": "VARCHAR(100) NOT NULL", f"{passwordColumnName}": "VARCHAR(150) NOT NULL", f"{saltColumnName}": "VARCHAR(150) NOT NULL"}, True)
 
-        rows_inserted:bool = mycooldatabase.insert_rows(usersTableName, {f"{usernameColumnName}": f"{username}", f"{passwordColumnName}": f"{hashed_password}", f"{saltColumnName}": f"{salt}"}, [f"{usernameColumnName}"])
+        rows_inserted:bool = mycooldatabase.insert_rows(usersTableName, {f"{usernameColumnName}": f"{username}", f"{emailColumnName}": f"{email}", f"{passwordColumnName}": f"{hashed_password}", f"{saltColumnName}": f"{salt}"}, [f"{usernameColumnName}", f"{emailColumnName}"])
         if rows_inserted:
-            notStructuredUser = mycooldatabase.get_rows(usersTableName, [f"{idColumnName}", f"{usernameColumnName}", f"{passwordColumnName}"], f"{usernameColumnName} = '{username}'")  
+            notStructuredUser = mycooldatabase.get_rows(usersTableName, [f"{idColumnName}", f"{usernameColumnName}", f"{emailColumnName}", f"{passwordColumnName}"], f"{usernameColumnName} = '{username}' AND {emailColumnName} = '{email}'")  
             notStructuredUser = notStructuredUser[0]
 
-            return User(notStructuredUser.get(f'{idColumnName}'), notStructuredUser.get(f'{usernameColumnName}'), notStructuredUser.get(f'{passwordColumnName}'))
+            return User(notStructuredUser.get(f'{idColumnName}'), notStructuredUser.get(f'{usernameColumnName}'), notStructuredUser.get(f'{emailColumnName}'), notStructuredUser.get(f'{passwordColumnName}'))
         return None
     except ValueError:
         #print('rawr')
         pass
 
 def loginUser(username:str, password:str) -> User:
     try:
@@ -102,35 +125,65 @@
 
             return User(notStructuredUser.get(f'{idColumnName}'), notStructuredUser.get(f'{usernameColumnName}'), notStructuredUser.get(f'{passwordColumnName}'))
         return None
     except ValueError:
         #print('login rawr :c')
         pass
 
-def editUser(user_to_update:User, new_username:str = None, new_password:str = None) -> User:
+
+def loginUserByEmail(email:str, password:str) -> User:
+    try:
+        global emailColumnName
+        global passwordColumnName
+        global usersTableName
+        global saltColumnName
+        if not userExistsByEmail(email):
+            return None
+        passwordSalt = mycooldatabase.get_rows(usersTableName, [f"{passwordColumnName}", f"{saltColumnName}"], f"{emailColumnName} = '{email}'")
+        if passwordSalt == None:
+            return None
+        usablePasswordSalt = passwordSalt[0]
+
+        if mycoolhashlib.checkPassword(usablePasswordSalt.get(f'{passwordColumnName}'), password, usablePasswordSalt.get(f'{saltColumnName}')):
+            notStructuredUser = mycooldatabase.get_rows(usersTableName, [f"{idColumnName}", f"{usernameColumnName}", f"{emailColumnName}", f"{passwordColumnName}"], f"{emailColumnName} = '{email}'")
+            
+            notStructuredUser = notStructuredUser[0]
+
+            return User(notStructuredUser.get(f'{idColumnName}'), notStructuredUser.get(f'{usernameColumnName}'), notStructuredUser.get(f'{emailColumnName}'), notStructuredUser.get(f'{passwordColumnName}'))
+        return None
+    except ValueError:
+        #print('login rawr :c')
+        pass
+
+
+def editUser(user_to_update:User, new_username:str = None, new_email=None, new_password:str = None) -> User:
     try:
         if not userExists(user_to_update.username):
             return None
-        if new_username == None and new_password == None:
+        if new_username == None and new_email and new_password == None:
             return user_to_update
         
         username_column_update_string = None if new_username == None else usernameColumnName
         username_value_update_string = None if new_username == None else new_username
 
+        email_column_update_string = None if new_email == None else emailColumnName
+        email_value_update_string = None if new_email == None else new_email
+
         password_column_update_string = None if new_password == None else passwordColumnName
         password_value_update_string = None if new_password == None else new_password
+        
         (hashed_password, salt) = (None, None)
         salt_column_update_string = None
         if not password_column_update_string == None:
             (hashed_password, salt) = mycoolhashlib.generateSaltHash(password_value_update_string)
             salt_column_update_string = saltColumnName
 
-        edition_suceedeed = mycooldatabase.edit_rows(usersTableName, {username_column_update_string: username_value_update_string, password_column_update_string: hashed_password, salt_column_update_string: salt}, f"{idColumnName} = {user_to_update.id}", [f"{usernameColumnName}"])
+        edition_suceedeed = mycooldatabase.edit_rows(usersTableName, {username_column_update_string: username_value_update_string, email_column_update_string: email_value_update_string, password_column_update_string: hashed_password, salt_column_update_string: salt}, f"{idColumnName} = {user_to_update.id}", [f"{usernameColumnName}", f"{emailColumnName}"])
         if edition_suceedeed:
-            notStructuredUser = mycooldatabase.get_rows(usersTableName, [f"{idColumnName}", f"{usernameColumnName}", f"{passwordColumnName}"], f"{idColumnName} = '{user_to_update.id}'")  
+            notStructuredUser = mycooldatabase.get_rows(usersTableName, [f"{idColumnName}", f"{usernameColumnName}", f"{emailColumnName}" ,f"{passwordColumnName}"], f"{idColumnName} = '{user_to_update.id}'")  
             notStructuredUser = notStructuredUser[0]
 
-            return User(notStructuredUser.get(f'{idColumnName}'), notStructuredUser.get(f'{usernameColumnName}'), notStructuredUser.get(f'{passwordColumnName}'))
+            return User(notStructuredUser.get(f'{idColumnName}'), notStructuredUser.get(f'{usernameColumnName}'), notStructuredUser.get(f'{emailColumnName}'), notStructuredUser.get(f'{passwordColumnName}'))
         return None
     except ValueError:
         #print('edit rawr :c')
         pass
```

### Comparing `eto-mysql-databaselib-1.1.4/src/databaselib/etodatabaselib.py` & `eto_mysql_databaselib-1.1.5/src/databaselib/etodatabaselib.py`

 * *Files identical despite different names*

### Comparing `eto-mysql-databaselib-1.1.4/src/databaselib/etohashlib.py` & `eto_mysql_databaselib-1.1.5/src/databaselib/etohashlib.py`

 * *Files identical despite different names*

### Comparing `eto-mysql-databaselib-1.1.4/src/eto_mysql_databaselib.egg-info/PKG-INFO` & `eto_mysql_databaselib-1.1.5/src/eto_mysql_databaselib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eto-mysql-databaselib
-Version: 1.1.4
+Version: 1.1.5
 Summary: A library with the sole purpose of making connections to mysql databases easier
 Author-email: Eto_chan <etochandev@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Etozinhachan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

