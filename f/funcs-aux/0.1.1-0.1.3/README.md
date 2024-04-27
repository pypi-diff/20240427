# Comparing `tmp/funcs_aux-0.1.1.tar.gz` & `tmp/funcs_aux-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcs_aux-0.1.1.tar", last modified: Thu Mar 28 14:45:15 2024, max compression
+gzip compressed data, was "funcs_aux-0.1.3.tar", last modified: Sat Apr 27 13:32:10 2024, max compression
```

## Comparing `funcs_aux-0.1.1.tar` & `funcs_aux-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 14:45:15.371121 funcs_aux-0.1.1/
--rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 funcs_aux-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1883 2024-03-28 14:45:15.370123 funcs_aux-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      990 2024-03-28 14:44:47.000000 funcs_aux-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-28 14:45:15.360552 funcs_aux-0.1.1/funcs_aux/
--rw-rw-rw-   0        0        0      282 2024-03-28 09:55:47.000000 funcs_aux-0.1.1/funcs_aux/__init__.py
--rw-rw-rw-   0        0        0     1894 2024-03-01 08:49:51.000000 funcs_aux-0.1.1/funcs_aux/arrays.py
--rw-rw-rw-   0        0        0     6005 2024-03-28 14:40:09.000000 funcs_aux-0.1.1/funcs_aux/collects.py
--rw-rw-rw-   0        0        0     5211 2024-03-22 14:19:18.000000 funcs_aux-0.1.1/funcs_aux/iterables.py
--rw-rw-rw-   0        0        0     8973 2024-03-22 14:19:18.000000 funcs_aux-0.1.1/funcs_aux/results.py
--rw-rw-rw-   0        0        0     1920 2024-03-01 08:45:13.000000 funcs_aux-0.1.1/funcs_aux/strings.py
-drwxrwxrwx   0        0        0        0 2024-03-28 14:45:15.369171 funcs_aux-0.1.1/funcs_aux.egg-info/
--rw-rw-rw-   0        0        0     1883 2024-03-28 14:45:15.000000 funcs_aux-0.1.1/funcs_aux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2024-03-28 14:45:15.000000 funcs_aux-0.1.1/funcs_aux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 14:45:15.000000 funcs_aux-0.1.1/funcs_aux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-03-28 14:45:15.000000 funcs_aux-0.1.1/funcs_aux.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-28 14:45:15.371238 funcs_aux-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 funcs_aux-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 13:32:10.201542 funcs_aux-0.1.3/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 funcs_aux-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1883 2024-04-27 13:32:10.200541 funcs_aux-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2024-04-27 13:31:41.000000 funcs_aux-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 13:32:10.190369 funcs_aux-0.1.3/funcs_aux/
+-rw-rw-rw-   0        0        0      282 2024-03-28 09:55:47.000000 funcs_aux-0.1.3/funcs_aux/__init__.py
+-rw-rw-rw-   0        0        0     1894 2024-03-01 08:49:51.000000 funcs_aux-0.1.3/funcs_aux/arrays.py
+-rw-rw-rw-   0        0        0     6005 2024-03-28 14:40:09.000000 funcs_aux-0.1.3/funcs_aux/collects.py
+-rw-rw-rw-   0        0        0     5211 2024-03-22 14:19:18.000000 funcs_aux-0.1.3/funcs_aux/iterables.py
+-rw-rw-rw-   0        0        0     9110 2024-04-27 13:29:45.000000 funcs_aux-0.1.3/funcs_aux/results.py
+-rw-rw-rw-   0        0        0     1920 2024-03-01 08:45:13.000000 funcs_aux-0.1.3/funcs_aux/strings.py
+drwxrwxrwx   0        0        0        0 2024-04-27 13:32:10.200541 funcs_aux-0.1.3/funcs_aux.egg-info/
+-rw-rw-rw-   0        0        0     1883 2024-04-27 13:32:10.000000 funcs_aux-0.1.3/funcs_aux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2024-04-27 13:32:10.000000 funcs_aux-0.1.3/funcs_aux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 13:32:10.000000 funcs_aux-0.1.3/funcs_aux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-27 13:32:10.000000 funcs_aux-0.1.3/funcs_aux.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 13:32:10.202542 funcs_aux-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 funcs_aux-0.1.3/setup.py
```

### Comparing `funcs_aux-0.1.1/LICENSE` & `funcs_aux-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.1/PKG-INFO` & `funcs_aux-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs_aux
-Version: 0.1.1
+Version: 0.1.3
 Summary: useful funcs in one place
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/funcs_aux
 Keywords: functions,auxiliary,auxiliary funcs,np funcs,collections funcs,strings funcs,result object
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# funcs_aux (v0.1.1)
+# funcs_aux (v0.1.3)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.1.1/README.md` & `funcs_aux-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# funcs_aux (v0.1.1)
+# funcs_aux (v0.1.3)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.1.1/funcs_aux/arrays.py` & `funcs_aux-0.1.3/funcs_aux/arrays.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.1/funcs_aux/collects.py` & `funcs_aux-0.1.3/funcs_aux/collects.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.1/funcs_aux/iterables.py` & `funcs_aux-0.1.3/funcs_aux/iterables.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.1/funcs_aux/results.py` & `funcs_aux-0.1.3/funcs_aux/results.py`

 * *Files 5% similar despite different names*

```diff
@@ -165,14 +165,16 @@
     CHAIN__USE_RESULT: bool = True
     CHAIN__STOP_ON_FAIL: bool = True
 
     # RESULT ----------------------------------
     STEP__RESULT: Optional[bool] = None
     STEP__EXX: Optional[bool] = None
 
+    STEP__INDEX: int = None
+
     def __init__(
             self,
             # _ResultExpect_Base ---------------------
             title: Optional[str] = None,
 
             args: TYPE__ARGS = None,
             kwargs: TYPE__KWARGS = None,
@@ -190,15 +192,15 @@
         self.CHAIN__STOP_ON_FAIL = chain__stop_on_fail
 
     def __call__(self, *args, **kwargs) -> Self:
         return self.run(*args, **kwargs)
 
     @property
     def MSG(self) -> str:
-        result = f"[result={self.STEP__RESULT}]{self.TITLE or ''}"
+        result = f"ResultExpect[result={self.STEP__RESULT}/title={self.TITLE or ''}/index={self.STEP__INDEX}]"
         return result
 
     def _result__clear(self) -> None:
         self.STEP__RESULT = False
         self.STEP__EXX = None
 
     def run(self, *args, **kwargs) -> bool:
@@ -210,15 +212,15 @@
             self.KWARGS = kwargs
 
         # WORK -----------------------
         try:
             self.STEP__RESULT = self._run__wrapped()
         except Exception as exx:
             self.STEP__EXX = exx
-
+        #
         print(self.MSG)
         return self.STEP__RESULT
 
     def _run__wrapped(self) -> Union[bool, NoReturn]:
         pass
 
 
@@ -281,14 +283,15 @@
 
     def _run__wrapped(self) -> bool:
         self.STEP__INDEX = -1
         result = True
         for step in self.CHAINS:
             self.STEP__INDEX += 1
             if isinstance(step, _ResultExpect_Base):
+                step.STEP__INDEX = self.STEP__INDEX
                 step.run(*self.ARGS, **self.KWARGS)
 
                 if step.CHAIN__USE_RESULT:
                     result &= bool(step.STEP__RESULT)
 
                 if not step.STEP__RESULT and step.CHAIN__STOP_ON_FAIL:
                     break
```

### Comparing `funcs_aux-0.1.1/funcs_aux/strings.py` & `funcs_aux-0.1.3/funcs_aux/strings.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.1/funcs_aux.egg-info/PKG-INFO` & `funcs_aux-0.1.3/funcs_aux.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs_aux
-Version: 0.1.1
+Version: 0.1.3
 Summary: useful funcs in one place
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/funcs_aux
 Keywords: functions,auxiliary,auxiliary funcs,np funcs,collections funcs,strings funcs,result object
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# funcs_aux (v0.1.1)
+# funcs_aux (v0.1.3)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.1.1/setup.py` & `funcs_aux-0.1.3/setup.py`

 * *Files identical despite different names*

