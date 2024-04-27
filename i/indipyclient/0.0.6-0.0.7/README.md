# Comparing `tmp/indipyclient-0.0.6.tar.gz` & `tmp/indipyclient-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipyclient-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "indipyclient-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `indipyclient-0.0.6.tar` & `indipyclient-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.0.6/LICENSE
--rw-r--r--   0        0        0     2646 2024-04-13 20:38:26.000000 indipyclient-0.0.6/README.md
--rw-r--r--   0        0        0      291 2024-04-25 16:27:19.000000 indipyclient-0.0.6/indipyclient/__init__.py
--rw-r--r--   0        0        0     3089 2024-04-03 21:43:04.000000 indipyclient-0.0.6/indipyclient/__main__.py
--rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.0.6/indipyclient/console/__init__.py
--rw-r--r--   0        0        0    19759 2024-04-04 21:35:51.000000 indipyclient-0.0.6/indipyclient/console/consoleclient.py
--rw-r--r--   0        0        0    48364 2024-04-05 12:12:41.000000 indipyclient-0.0.6/indipyclient/console/widgets.py
--rw-r--r--   0        0        0   144085 2024-04-25 16:29:53.000000 indipyclient-0.0.6/indipyclient/console/windows.py
--rw-r--r--   0        0        0      192 2023-09-20 21:15:05.000000 indipyclient-0.0.6/indipyclient/error.py
--rw-r--r--   0        0        0    25044 2024-04-13 18:46:37.000000 indipyclient-0.0.6/indipyclient/events.py
--rw-r--r--   0        0        0    34740 2024-04-12 08:47:00.000000 indipyclient-0.0.6/indipyclient/ipyclient.py
--rw-r--r--   0        0        0    15584 2024-04-11 11:19:29.000000 indipyclient-0.0.6/indipyclient/propertymembers.py
--rw-r--r--   0        0        0    27590 2024-04-13 18:00:12.000000 indipyclient-0.0.6/indipyclient/propertyvectors.py
--rw-r--r--   0        0        0      935 2024-04-25 16:27:34.000000 indipyclient-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3417 1970-01-01 00:00:00.000000 indipyclient-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2646 2024-04-13 20:38:26.000000 indipyclient-0.0.7/README.md
+-rw-r--r--   0        0        0      291 2024-04-26 20:02:42.000000 indipyclient-0.0.7/indipyclient/__init__.py
+-rw-r--r--   0        0        0     3089 2024-04-03 21:43:04.000000 indipyclient-0.0.7/indipyclient/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.0.7/indipyclient/console/__init__.py
+-rw-r--r--   0        0        0    19759 2024-04-04 21:35:51.000000 indipyclient-0.0.7/indipyclient/console/consoleclient.py
+-rw-r--r--   0        0        0    48364 2024-04-05 12:12:41.000000 indipyclient-0.0.7/indipyclient/console/widgets.py
+-rw-r--r--   0        0        0   144085 2024-04-25 16:29:53.000000 indipyclient-0.0.7/indipyclient/console/windows.py
+-rw-r--r--   0        0        0      192 2023-09-20 21:15:05.000000 indipyclient-0.0.7/indipyclient/error.py
+-rw-r--r--   0        0        0    25043 2024-04-26 19:21:44.000000 indipyclient-0.0.7/indipyclient/events.py
+-rw-r--r--   0        0        0    34740 2024-04-12 08:47:00.000000 indipyclient-0.0.7/indipyclient/ipyclient.py
+-rw-r--r--   0        0        0    15822 2024-04-26 20:12:26.000000 indipyclient-0.0.7/indipyclient/propertymembers.py
+-rw-r--r--   0        0        0    27590 2024-04-13 18:00:12.000000 indipyclient-0.0.7/indipyclient/propertyvectors.py
+-rw-r--r--   0        0        0      935 2024-04-26 20:02:28.000000 indipyclient-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3417 1970-01-01 00:00:00.000000 indipyclient-0.0.7/PKG-INFO
```

### Comparing `indipyclient-0.0.6/LICENSE` & `indipyclient-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.6/README.md` & `indipyclient-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.6/indipyclient/__main__.py` & `indipyclient-0.0.7/indipyclient/__main__.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.6/indipyclient/console/consoleclient.py` & `indipyclient-0.0.7/indipyclient/console/consoleclient.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.6/indipyclient/console/widgets.py` & `indipyclient-0.0.7/indipyclient/console/widgets.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.6/indipyclient/console/windows.py` & `indipyclient-0.0.7/indipyclient/console/windows.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.6/indipyclient/events.py` & `indipyclient-0.0.7/indipyclient/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,15 +325,14 @@
         properties = device.data
 
         # does this vector already exist
         if self.vectorname in properties:
             self.vector = properties[self.vectorname]
             # set changed values into self.vector
             self.vector._defvector(self)
-
         else:
             # create a new NumberVector
             self.vector = propertyvectors.NumberVector(self)
             # add it to properties
             properties[self.vectorname] = self.vector
```

### Comparing `indipyclient-0.0.6/indipyclient/ipyclient.py` & `indipyclient-0.0.7/indipyclient/ipyclient.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.6/indipyclient/propertymembers.py` & `indipyclient-0.0.7/indipyclient/propertymembers.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,32 +32,32 @@
 
 class SwitchMember(Member):
     """A SwitchMember can only have one of 'On' or 'Off' values"""
 
     def __init__(self, name, label=None, membervalue="Off"):
         super().__init__(name, label, membervalue)
         if membervalue not in ('On', 'Off'):
-            raise ParseException(f"Error: Invalid value {membervalue}, should be On or Off")
+            raise ParseException(f"Invalid value {membervalue}, should be On or Off")
 
     @property
     def membervalue(self):
         return self._membervalue
 
     @membervalue.setter
     def membervalue(self, value):
         if not value:
-            raise ParseException("Error: No value given, should be On or Off")
+            raise ParseException("No value given, should be On or Off")
         newvalue = self.checkvalue(value, ['On', 'Off'])
         if self._membervalue != newvalue:
             self._membervalue = newvalue
 
     def checkvalue(self, value, allowed):
         "allowed is a list of values, checks if value is in it"
         if value not in allowed:
-            raise ParseException(f"Error: Invalid value:{value}")
+            raise ParseException(f"Invalid value:{value}")
         return value
 
     def _snapshot(self):
         snapmember = Member(self.name, self.label, self._membervalue)
         return snapmember
 
     def oneswitch(self, newvalue):
@@ -70,55 +70,55 @@
 
 class LightMember(Member):
     """A LightMember can only have one of 'Idle', 'Ok', 'Busy' or 'Alert' values"""
 
     def __init__(self, name, label=None, membervalue="Idle"):
         super().__init__(name, label, membervalue)
         if membervalue not in ('Idle','Ok','Busy','Alert'):
-            raise ParseException(f"Error: Invalid light value {membervalue}")
+            raise ParseException(f"Invalid light value {membervalue}")
 
     @property
     def membervalue(self):
         return self._membervalue
 
     @membervalue.setter
     def membervalue(self, value):
         if not value:
-            raise ParseException("Error: No light value given")
+            raise ParseException("No light value given")
         newvalue = self.checkvalue(value, ['Idle','Ok','Busy','Alert'])
         if self._membervalue != newvalue:
             self._membervalue = newvalue
 
     def checkvalue(self, value, allowed):
         "allowed is a list of values, checks if value is in it"
         if value not in allowed:
-            raise ParseException(f"Error: Invalid value:{value}")
+            raise ParseException(f"Invalid value:{value}")
         return value
 
     def _snapshot(self):
         snapmember = Member(self.name, self.label, self._membervalue)
         return snapmember
 
 
 class TextMember(Member):
     """Contains a text string"""
 
     def __init__(self, name, label=None, membervalue=""):
         super().__init__(name, label, membervalue)
         if not isinstance(membervalue, str):
-            raise ParseException("Error: The text value should be a string")
+            raise ParseException("The text value should be a string")
 
     @property
     def membervalue(self):
         return self._membervalue
 
     @membervalue.setter
     def membervalue(self, value):
         if not isinstance(value, str):
-            raise ParseException("Error: The text value should be a string")
+            raise ParseException("The text value should be a string")
         if self._membervalue != value:
             self._membervalue = value
 
     def _snapshot(self):
         snapmember = Member(self.name, self.label, self._membervalue)
         return snapmember
 
@@ -190,15 +190,15 @@
             assert len(parts) == 3
             # a part could be empty string, ie if 2:5: is given
             numbers = list(float(x) if x else 0.0 for x in parts)
             floatvalue = numbers[0] + (numbers[1]/60) + (numbers[2]/3600)
             if negative:
                 floatvalue = -1 * floatvalue
         except:
-            raise TypeError("Error: Unable to parse number value")
+            raise TypeError("Unable to parse number value")
         return floatvalue
 
 
     def getformattedvalue(self):
         """This method returns this members value as a formatted string."""
         return self.getformattedstring(self._membervalue)
 
@@ -289,52 +289,62 @@
                         degrees = degrees + 1
                 valstring = f"{'-' if negative else ''}{degrees}:{integerminutes:02d}:{seconds:0{fn-4}.{fn-7}f}"
                 if w:
                     return valstring.rjust(int(w), ' ')
                 return valstring
 
         except:
-            raise TypeError("Error: Unable to parse number value")
+            raise TypeError("Unable to parse number value")
 
         # no other options accepted
-        raise TypeError("Error: Unable to process number format")
+        raise TypeError("Unable to process number format")
 
 
 class NumberMember(ParentNumberMember):
     """Contains a number, the attributes inform the client how the number should be
        displayed.
     """
 
     def __init__(self, name, label=None, format='', min='0', max='0', step='0', membervalue='0'):
         super().__init__(name, label, format, min, max, step, membervalue)
         self.format = format
         if not isinstance(min, str):
-            raise ParseException("Error: minimum value must be given as a string")
+            raise ParseException("Number minimum value must be given as a string")
         self.min = min
         if not isinstance(max, str):
-            raise ParseException("Error: maximum value must be given as a string")
+            raise ParseException("Number maximum value must be given as a string")
         self.max = max
         if not isinstance(step, str):
-            raise ParseException("Error: step value must be given as a string")
+            raise ParseException("Number step value must be given as a string")
         self.step = step
         if not isinstance(membervalue, str):
-            raise ParseException("Error: number value must be given as a string")
+            raise ParseException("Number value must be given as a string")
+        try:
+            # test a float can be created from this membervalue
+            floatvalue = self.getfloat(membervalue)
+        except:
+            raise ParseException("Cannot parse the number")
 
     @property
     def membervalue(self):
         return self._membervalue
 
     @membervalue.setter
     def membervalue(self, value):
+        if self._membervalue == value:
+            return
         if not isinstance(value, str):
-            raise ParseException("Error: number value must be given as a string")
+            raise ParseException("Number value must be given as a string")
         if not value:
-            raise ParseException("Error: no number value given")
-        if self._membervalue != value:
-            self._membervalue = value
+            raise ParseException("No number value given")
+        try:
+            # test a float can be created from this membervalue
+            floatvalue = self.getfloat(value)
+        except:
+            raise ParseException("Cannot parse the number")
 
 
     def onenumber(self, newvalue):
         """Returns xml of a oneNumber"""
         xmldata = ET.Element('oneNumber')
         xmldata.set("name", self.name)
         xmldata.text = newvalue
@@ -360,27 +370,27 @@
 
 class BLOBMember(ParentBLOBMember):
     """Contains a 'binary large object' such as an image."""
 
     def __init__(self, name, label=None, blobsize=0, blobformat='', membervalue=None):
         super().__init__(name, label, membervalue)
         if not isinstance(blobsize, int):
-            raise ParseException("Error: blobsize must be given as an integer")
+            raise ParseException("Blobsize must be given as an integer")
         # membervalue can be a byte string, path, string path or file like object
         self.blobsize = blobsize
         self.blobformat = blobformat
 
     @property
     def membervalue(self):
         return self._membervalue
 
     @membervalue.setter
     def membervalue(self, value):
         if not value:
-            raise ParseException("Error: No BLOB value given")
+            raise ParseException("No BLOB value given")
         self._membervalue = value
 
 
     def oneblob(self, newvalue, newsize, newformat):
         """Returns xml of a oneBLOB"""
         xmldata = ET.Element('oneBLOB')
         xmldata.set("name", self.name)
@@ -389,35 +399,35 @@
         # the value set in the xmldata object should be a bytes object
         if isinstance(newvalue, bytes):
             xmldata.text = newvalue
         elif isinstance(newvalue, pathlib.Path):
             try:
                 xmldata.text = newvalue.read_bytes()
             except:
-                raise ParseException("Error: Unable to read the given file")
+                raise ParseException("Unable to read the given file")
         elif hasattr(newvalue, "seek") and hasattr(newvalue, "read") and callable(newvalue.read):
             # a file-like object
             # set seek(0) so is read from start of file
             newvalue.seek(0)
             bytescontent = newvalue.read()
             newvalue.close()
             if not isinstance(bytescontent, bytes):
-                raise ParseException("Error: The read BLOB is not a bytes object")
+                raise ParseException("The read BLOB is not a bytes object")
             if bytescontent == b"":
-                raise ParseException("Error: The read BLOB value is empty")
+                raise ParseException("The read BLOB value is empty")
             xmldata.text = bytescontent
         else:
             # could be a path to a file
             try:
                 with open(newvalue, "rb") as fp:
                     bytescontent = fp.read()
             except:
-                raise ParseException("Error: Unable to read the given file")
+                raise ParseException("Unable to read the given file")
             if bytescontent == b"":
-                raise ParseException("Error: The read BLOB value is empty")
+                raise ParseException("The read BLOB value is empty")
             xmldata.text = bytescontent
         return xmldata
 
 
     def _snapshot(self):
         snapmember = ParentBLOBMember(self.name, self.label, self.blobsize, self.blobformat, self._membervalue)
         return snapmember
```

### Comparing `indipyclient-0.0.6/indipyclient/propertyvectors.py` & `indipyclient-0.0.7/indipyclient/propertyvectors.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.6/pyproject.toml` & `indipyclient-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipyclient"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "0.0.6"
+version = "0.0.7"
 description="Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'client', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipyclient.readthedocs.io"
```

### Comparing `indipyclient-0.0.6/PKG-INFO` & `indipyclient-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indipyclient
-Version: 0.0.6
+Version: 0.0.7
 Summary: Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol.
 Keywords: indi,client,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

