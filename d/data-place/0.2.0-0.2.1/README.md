# Comparing `tmp/data-place-0.2.0.tar.gz` & `tmp/data-place-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-place-0.2.0.tar", last modified: Thu Apr 25 06:17:15 2024, max compression
+gzip compressed data, was "data-place-0.2.1.tar", last modified: Sat Apr 27 12:41:23 2024, max compression
```

## Comparing `data-place-0.2.0.tar` & `data-place-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 06:17:15.660901 data-place-0.2.0/
--rw-rw-rw-   0        0        0       44 2024-04-25 06:17:15.000000 data-place-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6073 2024-04-25 06:17:15.660901 data-place-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     5156 2024-01-27 16:23:24.000000 data-place-0.2.0/README.md
--rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 data-place-0.2.0/build.py
-drwxrwxrwx   0        0        0        0 2024-04-25 06:17:15.659900 data-place-0.2.0/data_place.egg-info/
--rw-rw-rw-   0        0        0     6073 2024-04-25 06:17:15.000000 data-place-0.2.0/data_place.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2024-04-25 06:17:15.000000 data-place-0.2.0/data_place.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 06:17:15.000000 data-place-0.2.0/data_place.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-25 06:17:15.000000 data-place-0.2.0/data_place.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-25 06:17:15.000000 data-place-0.2.0/data_place.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-25 06:17:15.658901 data-place-0.2.0/dataplace/
--rw-rw-rw-   0        0        0      269 2024-01-20 13:15:44.000000 data-place-0.2.0/dataplace/__init__.py
--rw-rw-rw-   0        0        0     1611 2024-01-24 19:26:19.000000 data-place-0.2.0/dataplace/base.py
--rw-rw-rw-   0        0        0     2304 2024-01-27 08:30:20.000000 data-place-0.2.0/dataplace/callback.py
--rw-rw-rw-   0        0        0     2251 2024-01-27 16:19:43.000000 data-place-0.2.0/dataplace/control.py
--rw-rw-rw-   0        0        0     3556 2024-02-11 17:10:37.000000 data-place-0.2.0/dataplace/handler.py
--rw-rw-rw-   0        0        0     2771 2024-01-25 20:35:44.000000 data-place-0.2.0/dataplace/io.py
--rw-rw-rw-   0        0        0     8302 2024-01-26 07:10:39.000000 data-place-0.2.0/dataplace/receive.py
--rw-rw-rw-   0        0        0    10585 2024-01-26 07:23:18.000000 data-place-0.2.0/dataplace/send.py
--rw-rw-rw-   0        0        0     7533 2024-04-25 06:14:46.000000 data-place-0.2.0/dataplace/store.py
--rw-rw-rw-   0        0        0       10 2024-01-20 13:15:44.000000 data-place-0.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 06:17:15.660901 data-place-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1615 2024-04-25 06:17:12.000000 data-place-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 12:41:23.158195 data-place-0.2.1/
+-rw-rw-rw-   0        0        0       44 2024-04-27 12:41:23.000000 data-place-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6073 2024-04-27 12:41:23.157158 data-place-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5156 2024-01-27 16:23:24.000000 data-place-0.2.1/README.md
+-rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 data-place-0.2.1/build.py
+drwxrwxrwx   0        0        0        0 2024-04-27 12:41:23.157158 data-place-0.2.1/data_place.egg-info/
+-rw-rw-rw-   0        0        0     6073 2024-04-27 12:41:23.000000 data-place-0.2.1/data_place.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2024-04-27 12:41:23.000000 data-place-0.2.1/data_place.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 12:41:23.000000 data-place-0.2.1/data_place.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-27 12:41:23.000000 data-place-0.2.1/data_place.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-27 12:41:23.000000 data-place-0.2.1/data_place.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 12:41:23.155830 data-place-0.2.1/dataplace/
+-rw-rw-rw-   0        0        0      269 2024-01-20 13:15:44.000000 data-place-0.2.1/dataplace/__init__.py
+-rw-rw-rw-   0        0        0     1611 2024-01-24 19:26:19.000000 data-place-0.2.1/dataplace/base.py
+-rw-rw-rw-   0        0        0     2304 2024-01-27 08:30:20.000000 data-place-0.2.1/dataplace/callback.py
+-rw-rw-rw-   0        0        0     2251 2024-01-27 16:19:43.000000 data-place-0.2.1/dataplace/control.py
+-rw-rw-rw-   0        0        0     3556 2024-02-11 17:10:37.000000 data-place-0.2.1/dataplace/handler.py
+-rw-rw-rw-   0        0        0     2771 2024-01-25 20:35:44.000000 data-place-0.2.1/dataplace/io.py
+-rw-rw-rw-   0        0        0     8302 2024-01-26 07:10:39.000000 data-place-0.2.1/dataplace/receive.py
+-rw-rw-rw-   0        0        0    10585 2024-01-26 07:23:18.000000 data-place-0.2.1/dataplace/send.py
+-rw-rw-rw-   0        0        0     7260 2024-04-27 12:38:35.000000 data-place-0.2.1/dataplace/store.py
+-rw-rw-rw-   0        0        0       10 2024-01-20 13:15:44.000000 data-place-0.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 12:41:23.158195 data-place-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1615 2024-04-27 12:41:20.000000 data-place-0.2.1/setup.py
```

### Comparing `data-place-0.2.0/PKG-INFO` & `data-place-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-place
-Version: 0.2.0
+Version: 0.2.1
 Summary: A powerfull and flexible framework for designing async socket based data streaming and distribution systems, with automated parsing, dynamic data store and high-level control hooks.
 Home-page: https://github.com/Shahaf-F-S/data-place
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `data-place-0.2.0/README.md` & `data-place-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `data-place-0.2.0/build.py` & `data-place-0.2.1/build.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.0/data_place.egg-info/PKG-INFO` & `data-place-0.2.1/data_place.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-place
-Version: 0.2.0
+Version: 0.2.1
 Summary: A powerfull and flexible framework for designing async socket based data streaming and distribution systems, with automated parsing, dynamic data store and high-level control hooks.
 Home-page: https://github.com/Shahaf-F-S/data-place
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `data-place-0.2.0/dataplace/base.py` & `data-place-0.2.1/dataplace/base.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.0/dataplace/callback.py` & `data-place-0.2.1/dataplace/callback.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.0/dataplace/control.py` & `data-place-0.2.1/dataplace/control.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.0/dataplace/handler.py` & `data-place-0.2.1/dataplace/handler.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.0/dataplace/io.py` & `data-place-0.2.1/dataplace/io.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.0/dataplace/receive.py` & `data-place-0.2.1/dataplace/receive.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.0/dataplace/send.py` & `data-place-0.2.1/dataplace/send.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.0/dataplace/store.py` & `data-place-0.2.1/dataplace/store.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,30 +56,21 @@
 
     def __iter__(self) -> Generator[S, ..., ...]:
 
         yield from self.keys()
 
     def __contains__(self, item: S | D) -> bool:
 
-        if (
-            isinstance(item, Hashable) and
-            not isinstance(item, collections.abc.Iterable)
-        ):
+        if not isinstance(item, collections.abc.Iterable):
             item = (item,)
 
-        if (
-            not isinstance(item, Hashable) and
-            isinstance(item, collections.abc.Iterable)
-        ):
+        else:
             item = tuple(item)
 
-        return (
-            (item in self.store) and
-            (item is None or item in self.store[item])
-        )
+        return item in self.store
 
     def __add__(self, other: ...) -> Self:
 
         if not isinstance(other, type(self)):
             raise TypeError(
                 f"both objects must be {type(self)} "
                 f"instances for addition, received: {type(other)}"
```

### Comparing `data-place-0.2.0/setup.py` & `data-place-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='data-place',
-        version='0.2.0',
+        version='0.2.1',
         description=(
             "A powerfull and flexible framework for designing async "
             "socket based data streaming and distribution systems, "
             "with automated parsing, dynamic data store and "
             "high-level control hooks."
         ),
         license='MIT',
```

