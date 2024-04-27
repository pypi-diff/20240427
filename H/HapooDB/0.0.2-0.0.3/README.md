# Comparing `tmp/HapooDB-0.0.2.tar.gz` & `tmp/HapooDB-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HapooDB-0.0.2.tar", last modified: Sat Apr 13 18:09:32 2024, max compression
+gzip compressed data, was "HapooDB-0.0.3.tar", last modified: Sat Apr 27 09:31:52 2024, max compression
```

## Comparing `HapooDB-0.0.2.tar` & `HapooDB-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 18:09:32.482910 HapooDB-0.0.2/
-drwxrwxrwx   0        0        0        0 2024-04-13 18:09:32.463960 HapooDB-0.0.2/HapooDB/
--rw-rw-rw-   0        0        0     3778 2024-04-13 17:02:36.000000 HapooDB-0.0.2/HapooDB/HapooDB.py
--rw-rw-rw-   0        0        0       28 2024-04-13 18:08:23.000000 HapooDB-0.0.2/HapooDB/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 18:09:32.478919 HapooDB-0.0.2/HapooDB.egg-info/
--rw-rw-rw-   0        0        0      451 2024-04-13 18:09:32.000000 HapooDB-0.0.2/HapooDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      171 2024-04-13 18:09:32.000000 HapooDB-0.0.2/HapooDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 18:09:32.000000 HapooDB-0.0.2/HapooDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-13 18:09:32.000000 HapooDB-0.0.2/HapooDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      451 2024-04-13 18:09:32.480914 HapooDB-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-13 18:09:32.482910 HapooDB-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      699 2024-04-13 18:06:25.000000 HapooDB-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 09:31:52.760864 HapooDB-0.0.3/
+drwxrwxrwx   0        0        0        0 2024-04-27 09:31:52.756874 HapooDB-0.0.3/HapooDB.egg-info/
+-rw-rw-rw-   0        0        0      478 2024-04-27 09:31:52.000000 HapooDB-0.0.3/HapooDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2024-04-27 09:31:52.000000 HapooDB-0.0.3/HapooDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 09:31:52.000000 HapooDB-0.0.3/HapooDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-27 09:31:52.000000 HapooDB-0.0.3/HapooDB.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 09:31:52.754880 HapooDB-0.0.3/HapooDBfolder/
+-rw-rw-rw-   0        0        0     4460 2024-04-27 09:16:01.000000 HapooDB-0.0.3/HapooDBfolder/HapooDB.py
+-rw-rw-rw-   0        0        0       28 2024-04-27 08:41:15.000000 HapooDB-0.0.3/HapooDBfolder/__init__.py
+-rw-rw-rw-   0        0        0     1299 2024-04-27 09:31:12.000000 HapooDB-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      478 2024-04-27 09:31:52.758869 HapooDB-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      493 2024-04-27 09:31:38.000000 HapooDB-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 09:31:52.760864 HapooDB-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      699 2024-04-27 09:27:45.000000 HapooDB-0.0.3/setup.py
```

### Comparing `HapooDB-0.0.2/HapooDB/HapooDB.py` & `HapooDB-0.0.3/HapooDBfolder/HapooDB.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,79 +5,108 @@
         self.variables = []
         if title:
             self.filename = f"{title[0]}.txt"
         else:
             self.filename = f"HapooDB.txt"
         try:
             try:
-                self.file = open(self.filename,"xt")
+                with open(self.filename,"xt") as file:
+                    pass
+
             except IndexError:
-                self.file = open(self.filename,"xt")
-            self.file.close() 
+                with open(self.filename,"xt") as file:
+                    pass
         except FileExistsError: 
             pass
+
     def destroyfile(self) -> None:
         if os.path.exists(self.filename):
             os.remove(self.filename)
         else:
             print("!The file, {} does not exist".format(self.filename))
-    def declare(self,key,val) -> None:
-        self.file = open(self.filename,"at")
-        self.file.write(f"{key}={val}\n")
-    def closeFile(self) -> None:
-        self.file.close()
-    def access(self) -> list:
-        self.file = open(self.filename,"rt")
-        lines = [line.strip("\n") for line in self.file.readlines()]
-        variables = {}
-        for line in lines:
-            line = [element for element in line.split("=")]
-            variables[line[0]] = line[1]
-        return variables    
+
+
+    def declare(self, key, val):
+        with open(self.filename, "at") as self.file:
+            self.file.write(f"{key}={val}\n")
+
+    def access(self) -> dict:
+        with  open(self.filename,"rt") as self.file:
+            lines = [line.strip("\n") for line in self.file.readlines()]
+            variables = {}
+            for line in lines:
+                line = [element for element in line.split("=")]
+                variables[line[0]] = line[1]
+            return variables  
+      
     def accessSingle(self,key) -> str:
-        self.file = open(self.filename,"rt")
-        lines = [line.strip("\n") for line in self.file.readlines()]
-        val = None
-        for line in lines:
-            if key in line:
-                val = line.split("=")[1]
-            else:
-                continue
-        try:
-            return val.strip("\n")            
-        except AttributeError:
-            print("!There is no such of key in the DB.")
+        with open(self.filename,"rt") as self.file:
+            lines = [line.strip("\n") for line in self.file.readlines()]
+            val = None
+            for line in lines:
+                if key in line:
+                    val = line.split("=")[1]
+                    break
+                else:
+                    continue
+            try:
+                return val.strip("\n")         
+           
+            except AttributeError:
+                print("!There is no such of key in the DB.")
+
+
     def declareCluster(self,keyValPair:dict) -> None:
-        self.file = open(self.filename,"at")
-        content = list(keyValPair.items())
-        for branchlist in content:
-            self.file.write(f"{branchlist[0]}={branchlist[1]}\n")      
+        with open(self.filename,"at") as self.file:
+            content = list(keyValPair.items())
+            for branchlist in content:
+                self.file.write(f"{branchlist[0]}={branchlist[1]}\n")   
+
+
+
     def clearFile(self) -> None:
-        self.file = open(self.filename,"wt")
-        self.file.write('')
+        with open(self.filename,"wt") as self.file:
+            self.file.write('')
+
+
     def declareEncryption(self,key,value) -> None: 
         key = self.__private_Encrypt(key)
         value = self.__private_Encrypt(value)
 
-        self.file = open(self.filename,"at")
-        self.file.write(f"{key}={value}\n")
+        with  open(self.filename,"at") as self.file:
+            self.file.write(f"{key}={value}\n")
+
+
     def accessEncryption(self,key):
-        self.file = open(self.filename,"rt")
-        lines = [line.strip("\n") for line in self.file.readlines()]
-        val = None
-        for line in lines:
-            if self.__private_Encrypt(key) in line:
-                val = line.split("=")[1]
-                print(val)
-            else:
-                continue
-        try:
-            return self.__private_Decrypt(val.strip("\n"))
-        except AttributeError:
-            print("!There is no such of key in the DB.")
+        with open(self.filename,"rt") as self.file:
+            lines = [line.strip("\n") for line in self.file.readlines()]
+            val = None
+            for line in lines:
+                if self.__private_Encrypt(key) in line:
+                    val = line.split("=")[1]
+                else:
+                    continue
+            try:
+                return self.__private_Decrypt(val.strip("\n"))
+            except AttributeError:
+                print("!There is no such of key in the DB.")
+        ##todo
+    def changeValue(self,key,changingValue):
+        with open(self.filename,"rt") as self.file:
+            lines = [line for line in self.file.readlines()]
+        print(lines)
+        for index,line in enumerate(lines):
+            if key in line:
+                indexOfLine = index
+                break
+        lines[indexOfLine] = f"{key}={changingValue}\n"
+        with open(self.filename, "w") as file: 
+            file.write("".join(lines))  
+            
+
     def __private_Encrypt(self,val):
         alphabets = [letter for letter in "QWERTYUIOPASDFGHJKLZXCVBNMqwertyuiopasdfghjklzxcvbnm1234567890"]
         EncodedMsg = []
         for letter in val:
             if letter in val:
                 index = alphabets.index(letter)
                 newPosition = (index + 3) % 62
```

### Comparing `HapooDB-0.0.2/setup.py` & `HapooDB-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Hapoo DB'
 
 
 # Setting up
 setup(
     name="HapooDB",
     version=VERSION,
```

