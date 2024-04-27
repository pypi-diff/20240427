# Comparing `tmp/python-iso639-2024.2.7.tar.gz` & `tmp/python_iso639-2024.4.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-iso639-2024.2.7.tar", last modified: Thu Feb  8 04:17:52 2024, max compression
+gzip compressed data, was "python_iso639-2024.4.27.tar", last modified: Sat Apr 27 19:21:37 2024, max compression
```

## Comparing `python-iso639-2024.2.7.tar` & `python_iso639-2024.4.27.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2024-02-08 04:17:52.872998 python-iso639-2024.2.7/
--rw-r--r--   0 jacksonlee   (501) staff       (20)    10759 2022-08-28 17:23:57.000000 python-iso639-2024.2.7/LICENSE.txt
--rw-r--r--   0 jacksonlee   (501) staff       (20)    13724 2024-02-08 04:17:52.872655 python-iso639-2024.2.7/PKG-INFO
--rw-r--r--   0 jacksonlee   (501) staff       (20)    12175 2024-02-08 04:16:42.000000 python-iso639-2024.2.7/README.md
--rw-r--r--   0 jacksonlee   (501) staff       (20)     1765 2024-02-08 04:16:42.000000 python-iso639-2024.2.7/pyproject.toml
--rw-r--r--   0 jacksonlee   (501) staff       (20)       38 2024-02-08 04:17:52.873069 python-iso639-2024.2.7/setup.cfg
-drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2024-02-08 04:17:52.868639 python-iso639-2024.2.7/src/
-drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2024-02-08 04:17:52.870195 python-iso639-2024.2.7/src/iso639/
--rw-r--r--   0 jacksonlee   (501) staff       (20)      525 2024-02-08 04:16:42.000000 python-iso639-2024.2.7/src/iso639/__init__.py
--rw-r--r--   0 jacksonlee   (501) staff       (20)     7897 2023-12-12 14:11:20.000000 python-iso639-2024.2.7/src/iso639/language.py
--rw-r--r--   0 jacksonlee   (501) staff       (20)   540672 2024-02-08 04:16:42.000000 python-iso639-2024.2.7/src/iso639/languages.db
-drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2024-02-08 04:17:52.871973 python-iso639-2024.2.7/src/python_iso639.egg-info/
--rw-r--r--   0 jacksonlee   (501) staff       (20)    13724 2024-02-08 04:17:52.000000 python-iso639-2024.2.7/src/python_iso639.egg-info/PKG-INFO
--rw-r--r--   0 jacksonlee   (501) staff       (20)      402 2024-02-08 04:17:52.000000 python-iso639-2024.2.7/src/python_iso639.egg-info/SOURCES.txt
--rw-r--r--   0 jacksonlee   (501) staff       (20)        1 2024-02-08 04:17:52.000000 python-iso639-2024.2.7/src/python_iso639.egg-info/dependency_links.txt
--rw-r--r--   0 jacksonlee   (501) staff       (20)        1 2022-08-28 17:28:05.000000 python-iso639-2024.2.7/src/python_iso639.egg-info/not-zip-safe
--rw-r--r--   0 jacksonlee   (501) staff       (20)       75 2024-02-08 04:17:52.000000 python-iso639-2024.2.7/src/python_iso639.egg-info/requires.txt
--rw-r--r--   0 jacksonlee   (501) staff       (20)        7 2024-02-08 04:17:52.000000 python-iso639-2024.2.7/src/python_iso639.egg-info/top_level.txt
-drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2024-02-08 04:17:52.871617 python-iso639-2024.2.7/tests/
--rw-r--r--   0 jacksonlee   (501) staff       (20)     3046 2024-02-08 04:16:42.000000 python-iso639-2024.2.7/tests/test_language.py
--rw-r--r--   0 jacksonlee   (501) staff       (20)     1295 2022-08-28 17:23:57.000000 python-iso639-2024.2.7/tests/test_version_number.py
+drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2024-04-27 19:21:37.405793 python_iso639-2024.4.27/
+-rw-r--r--   0 jacksonlee   (501) staff       (20)    10759 2022-08-28 17:23:57.000000 python_iso639-2024.4.27/LICENSE.txt
+-rw-r--r--   0 jacksonlee   (501) staff       (20)    13774 2024-04-27 19:21:37.405441 python_iso639-2024.4.27/PKG-INFO
+-rw-r--r--   0 jacksonlee   (501) staff       (20)    12167 2024-04-27 19:20:36.000000 python_iso639-2024.4.27/README.md
+-rw-r--r--   0 jacksonlee   (501) staff       (20)     1801 2024-04-27 19:20:36.000000 python_iso639-2024.4.27/pyproject.toml
+-rw-r--r--   0 jacksonlee   (501) staff       (20)       38 2024-04-27 19:21:37.405845 python_iso639-2024.4.27/setup.cfg
+drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2024-04-27 19:21:37.399842 python_iso639-2024.4.27/src/
+drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2024-04-27 19:21:37.401735 python_iso639-2024.4.27/src/iso639/
+-rw-r--r--   0 jacksonlee   (501) staff       (20)      525 2024-04-27 19:20:36.000000 python_iso639-2024.4.27/src/iso639/__init__.py
+-rw-r--r--   0 jacksonlee   (501) staff       (20)     7897 2023-12-12 14:11:20.000000 python_iso639-2024.4.27/src/iso639/language.py
+-rw-r--r--   0 jacksonlee   (501) staff       (20)   540672 2024-04-27 19:20:36.000000 python_iso639-2024.4.27/src/iso639/languages.db
+drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2024-04-27 19:21:37.404671 python_iso639-2024.4.27/src/python_iso639.egg-info/
+-rw-r--r--   0 jacksonlee   (501) staff       (20)    13774 2024-04-27 19:21:37.000000 python_iso639-2024.4.27/src/python_iso639.egg-info/PKG-INFO
+-rw-r--r--   0 jacksonlee   (501) staff       (20)      402 2024-04-27 19:21:37.000000 python_iso639-2024.4.27/src/python_iso639.egg-info/SOURCES.txt
+-rw-r--r--   0 jacksonlee   (501) staff       (20)        1 2024-04-27 19:21:37.000000 python_iso639-2024.4.27/src/python_iso639.egg-info/dependency_links.txt
+-rw-r--r--   0 jacksonlee   (501) staff       (20)        1 2022-08-28 17:28:05.000000 python_iso639-2024.4.27/src/python_iso639.egg-info/not-zip-safe
+-rw-r--r--   0 jacksonlee   (501) staff       (20)       92 2024-04-27 19:21:37.000000 python_iso639-2024.4.27/src/python_iso639.egg-info/requires.txt
+-rw-r--r--   0 jacksonlee   (501) staff       (20)        7 2024-04-27 19:21:37.000000 python_iso639-2024.4.27/src/python_iso639.egg-info/top_level.txt
+drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2024-04-27 19:21:37.404418 python_iso639-2024.4.27/tests/
+-rw-r--r--   0 jacksonlee   (501) staff       (20)     3046 2024-04-27 19:20:36.000000 python_iso639-2024.4.27/tests/test_language.py
+-rw-r--r--   0 jacksonlee   (501) staff       (20)     1295 2022-08-28 17:23:57.000000 python_iso639-2024.4.27/tests/test_version_number.py
```

### Comparing `python-iso639-2024.2.7/LICENSE.txt` & `python_iso639-2024.4.27/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-iso639-2024.2.7/PKG-INFO` & `python_iso639-2024.4.27/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: python-iso639
-Version: 2024.2.7
-Summary: Look-up utilities for ISO 639 language codes and names
+Version: 2024.4.27
+Summary: ISO 639 language codes, names, and other associated information
 Author-email: "Jackson L. Lee" <jacksonlunlee@gmail.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/jacksonllee/iso639
 Keywords: ISO 639,language codes,languages,linguistics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -24,28 +24,29 @@
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Indexing
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Provides-Extra: dev
-Requires-Dist: black==24.1.1; extra == "dev"
-Requires-Dist: build==1.0.3; extra == "dev"
+Requires-Dist: black==24.4.2; extra == "dev"
+Requires-Dist: build==1.2.1; extra == "dev"
 Requires-Dist: flake8==7.0.0; extra == "dev"
-Requires-Dist: pytest==8.0.0; extra == "dev"
-Requires-Dist: twine==4.0.2; extra == "dev"
+Requires-Dist: pytest==8.1.2; extra == "dev"
+Requires-Dist: requests==2.31.0; extra == "dev"
+Requires-Dist: twine==5.0.0; extra == "dev"
 
 # python-iso639
 
 [![PyPI version](https://badge.fury.io/py/python-iso639.svg)](https://pypi.org/project/python-iso639/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/python-iso639.svg)](https://pypi.org/project/python-iso639/)
 [![PyPI downloads last month](https://img.shields.io/pypi/dm/python-iso639)](https://pypi.org/project/python-iso639/)
 [![CircleCI Builds](https://circleci.com/gh/jacksonllee/iso639.svg?style=shield)](https://circleci.com/gh/jacksonllee/iso639)
 
-`python-iso639` is a Python package for accessing ISO 639 language codes, names, and
+`python-iso639` is a Python package for ISO 639 language codes, names, and
 other associated information.
 
 Current features:
 
 * A representation of languages mapped across ISO 639-1, 639-2, and 639-3.
 * Functionality to "guess" what a language is for a given
   unknown language code or name.
@@ -253,15 +254,15 @@
 As soon as a match is found, `Language.match` returns a `Language` instance.
 If there isn't a match, a `LanguageNotFoundError` is raised.
 
 ### `Language` is a dataclass
 
 The `Language` class is a dataclass.
 All functionality of
-[dataclases](https://docs.python.org/3/library/dataclasses.html)
+[dataclasses](https://docs.python.org/3/library/dataclasses.html)
 applies to `Language` and its instances,
 e.g., [`dataclasses.asdict`](https://docs.python.org/3/library/dataclasses.html#dataclasses.asdict):
 
 ```python
 >>> import dataclasses, iso639
 >>> language = iso639.Language.match('fra')
 >>> dataclasses.asdict(language)
@@ -271,25 +272,25 @@
 ### Constants
 
 * `DATA_LAST_UPDATED`: The release date of the included language code data from SIL
 
     ```python
     >>> import iso639
     >>> iso639.DATA_LAST_UPDATED
-    datetime.date(2024, 2, 7)
+    datetime.date(2024, 4, 15)
     ```
 
 * `ALL_LANGUAGES`: The list of all `Language` objects based on the included language code data
 
     ```python
     >>> import iso639
     >>> type(iso639.ALL_LANGUAGES)
     <class 'list'>
     >>> len(iso639.ALL_LANGUAGES)
-    7919
+    7920
     >>> iso639.ALL_LANGUAGES[0]
     Language(part3='aaa', scope='I', type='L', status='A', name='Ghotuo', ...)
     ```
 
 ## Links
 
 * Author: [Jackson L. Lee](https://jacksonllee.com)
```

### Comparing `python-iso639-2024.2.7/README.md` & `python_iso639-2024.4.27/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # python-iso639
 
 [![PyPI version](https://badge.fury.io/py/python-iso639.svg)](https://pypi.org/project/python-iso639/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/python-iso639.svg)](https://pypi.org/project/python-iso639/)
 [![PyPI downloads last month](https://img.shields.io/pypi/dm/python-iso639)](https://pypi.org/project/python-iso639/)
 [![CircleCI Builds](https://circleci.com/gh/jacksonllee/iso639.svg?style=shield)](https://circleci.com/gh/jacksonllee/iso639)
 
-`python-iso639` is a Python package for accessing ISO 639 language codes, names, and
+`python-iso639` is a Python package for ISO 639 language codes, names, and
 other associated information.
 
 Current features:
 
 * A representation of languages mapped across ISO 639-1, 639-2, and 639-3.
 * Functionality to "guess" what a language is for a given
   unknown language code or name.
@@ -217,15 +217,15 @@
 As soon as a match is found, `Language.match` returns a `Language` instance.
 If there isn't a match, a `LanguageNotFoundError` is raised.
 
 ### `Language` is a dataclass
 
 The `Language` class is a dataclass.
 All functionality of
-[dataclases](https://docs.python.org/3/library/dataclasses.html)
+[dataclasses](https://docs.python.org/3/library/dataclasses.html)
 applies to `Language` and its instances,
 e.g., [`dataclasses.asdict`](https://docs.python.org/3/library/dataclasses.html#dataclasses.asdict):
 
 ```python
 >>> import dataclasses, iso639
 >>> language = iso639.Language.match('fra')
 >>> dataclasses.asdict(language)
@@ -235,25 +235,25 @@
 ### Constants
 
 * `DATA_LAST_UPDATED`: The release date of the included language code data from SIL
 
     ```python
     >>> import iso639
     >>> iso639.DATA_LAST_UPDATED
-    datetime.date(2024, 2, 7)
+    datetime.date(2024, 4, 15)
     ```
 
 * `ALL_LANGUAGES`: The list of all `Language` objects based on the included language code data
 
     ```python
     >>> import iso639
     >>> type(iso639.ALL_LANGUAGES)
     <class 'list'>
     >>> len(iso639.ALL_LANGUAGES)
-    7919
+    7920
     >>> iso639.ALL_LANGUAGES[0]
     Language(part3='aaa', scope='I', type='L', status='A', name='Ghotuo', ...)
     ```
 
 ## Links
 
 * Author: [Jackson L. Lee](https://jacksonllee.com)
```

### Comparing `python-iso639-2024.2.7/pyproject.toml` & `python_iso639-2024.4.27/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 65.3.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-iso639"
-version = "2024.2.7"
-description = "Look-up utilities for ISO 639 language codes and names"
+version = "2024.4.27"
+description = "ISO 639 language codes, names, and other associated information"
 readme = "README.md"
 requires-python = ">= 3.8"
 license = { text = "Apache 2.0" }
 authors = [ { name = "Jackson L. Lee", email = "jacksonlunlee@gmail.com" } ]
 keywords = ["ISO 639", "language codes", "languages", "linguistics"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -30,19 +30,20 @@
     "Topic :: Text Processing :: General",
     "Topic :: Text Processing :: Indexing",
     "Topic :: Text Processing :: Linguistic",
 ]
 
 [project.optional-dependencies]
 dev = [
-    "black == 24.1.1",
-    "build == 1.0.3",
+    "black == 24.4.2",
+    "build == 1.2.1",
     "flake8 == 7.0.0",
-    "pytest == 8.0.0",
-    "twine == 4.0.2",
+    "pytest == 8.1.2",
+    "requests == 2.31.0",
+    "twine == 5.0.0",
 ]
 
 [project.urls]
 Source = "https://github.com/jacksonllee/iso639"
 
 [tool.setuptools.packages.find]
 where = [ "src" ]
```

### Comparing `python-iso639-2024.2.7/src/iso639/__init__.py` & `python_iso639-2024.4.27/src/iso639/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "__version__",
     "ALL_LANGUAGES",
     "DATA_LAST_UPDATED",
     "Language",
     "LanguageNotFoundError",
 ]
 
-DATA_LAST_UPDATED = datetime.date(2024, 1, 10)
+DATA_LAST_UPDATED = datetime.date(2024, 4, 15)
 
 
 def __getattr__(name):
     if name == "ALL_LANGUAGES":
         return _get_all_languages()
     else:
         raise AttributeError(f"module {__name__!r} has no attribute {name!r}")
```

### Comparing `python-iso639-2024.2.7/src/iso639/language.py` & `python_iso639-2024.4.27/src/iso639/language.py`

 * *Files identical despite different names*

### Comparing `python-iso639-2024.2.7/src/iso639/languages.db` & `python_iso639-2024.4.27/src/iso639/languages.db`

 * *Files 1% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -1562,15 +1562,15 @@
 INSERT INTO codes VALUES('dgg',NULL,NULL,NULL,'I','L','Doga',NULL);
 INSERT INTO codes VALUES('dgh',NULL,NULL,NULL,'I','L','Dghwede',NULL);
 INSERT INTO codes VALUES('dgi',NULL,NULL,NULL,'I','L','Northern Dagara',NULL);
 INSERT INTO codes VALUES('dgk',NULL,NULL,NULL,'I','L','Dagba',NULL);
 INSERT INTO codes VALUES('dgl',NULL,NULL,NULL,'I','L','Andaandi',NULL);
 INSERT INTO codes VALUES('dgn',NULL,NULL,NULL,'I','E','Dagoman',NULL);
 INSERT INTO codes VALUES('dgo',NULL,NULL,NULL,'I','L','Dogri (individual language)',NULL);
-INSERT INTO codes VALUES('dgr','dgr','dgr',NULL,'I','L','Dogrib',NULL);
+INSERT INTO codes VALUES('dgr','dgr','dgr',NULL,'I','L','Tlicho',NULL);
 INSERT INTO codes VALUES('dgs',NULL,NULL,NULL,'I','L','Dogoso',NULL);
 INSERT INTO codes VALUES('dgt',NULL,NULL,NULL,'I','E','Ndra''ngith',NULL);
 INSERT INTO codes VALUES('dgw',NULL,NULL,NULL,'I','E','Daungwurrung',NULL);
 INSERT INTO codes VALUES('dgx',NULL,NULL,NULL,'I','L','Doghoro',NULL);
 INSERT INTO codes VALUES('dgz',NULL,NULL,NULL,'I','L','Daga',NULL);
 INSERT INTO codes VALUES('dhd',NULL,NULL,NULL,'I','L','Dhundari',NULL);
 INSERT INTO codes VALUES('dhg',NULL,NULL,NULL,'I','L','Dhangu-Djangu',NULL);
@@ -2671,14 +2671,15 @@
 INSERT INTO codes VALUES('isl','ice','isl','is','I','L','Icelandic',NULL);
 INSERT INTO codes VALUES('ism',NULL,NULL,NULL,'I','L','Masimasi',NULL);
 INSERT INTO codes VALUES('isn',NULL,NULL,NULL,'I','L','Isanzu',NULL);
 INSERT INTO codes VALUES('iso',NULL,NULL,NULL,'I','L','Isoko',NULL);
 INSERT INTO codes VALUES('isr',NULL,NULL,NULL,'I','L','Israeli Sign Language',NULL);
 INSERT INTO codes VALUES('ist',NULL,NULL,NULL,'I','L','Istriot',NULL);
 INSERT INTO codes VALUES('isu',NULL,NULL,NULL,'I','L','Isu (Menchum Division)',NULL);
+INSERT INTO codes VALUES('isv',NULL,NULL,NULL,'I','C','Interslavic',NULL);
 INSERT INTO codes VALUES('ita','ita','ita','it','I','L','Italian',NULL);
 INSERT INTO codes VALUES('itb',NULL,NULL,NULL,'I','L','Binongan Itneg',NULL);
 INSERT INTO codes VALUES('itd',NULL,NULL,NULL,'I','L','Southern Tidung',NULL);
 INSERT INTO codes VALUES('ite',NULL,NULL,NULL,'I','E','Itene',NULL);
 INSERT INTO codes VALUES('iti',NULL,NULL,NULL,'I','L','Inlaod Itneg',NULL);
 INSERT INTO codes VALUES('itk',NULL,NULL,NULL,'I','L','Judeo-Italian',NULL);
 INSERT INTO codes VALUES('itl',NULL,NULL,NULL,'I','L','Itelmen',NULL);
@@ -9548,15 +9549,15 @@
 INSERT INTO name_index VALUES('dgi','Northern Dagara','Dagara, Northern');
 INSERT INTO name_index VALUES('dgk','Dagba','Dagba');
 INSERT INTO name_index VALUES('dgl','Andaandi','Andaandi');
 INSERT INTO name_index VALUES('dgl','Dongolawi','Dongolawi');
 INSERT INTO name_index VALUES('dgn','Dagoman','Dagoman');
 INSERT INTO name_index VALUES('dgo','Dogri (individual language)','Dogri (individual language)');
 INSERT INTO name_index VALUES('dgr','Dogrib','Dogrib');
-INSERT INTO name_index VALUES('dgr','Tłı̨chǫ','Tłı̨chǫ');
+INSERT INTO name_index VALUES('dgr','Tlicho','Tlicho');
 INSERT INTO name_index VALUES('dgs','Dogoso','Dogoso');
 INSERT INTO name_index VALUES('dgt','Ndra''ngith','Ndra''ngith');
 INSERT INTO name_index VALUES('dgw','Daungwurrung','Daungwurrung');
 INSERT INTO name_index VALUES('dgx','Doghoro','Doghoro');
 INSERT INTO name_index VALUES('dgz','Daga','Daga');
 INSERT INTO name_index VALUES('dhd','Dhundari','Dhundari');
 INSERT INTO name_index VALUES('dhg','Dhangu','Dhangu');
@@ -10732,14 +10733,15 @@
 INSERT INTO name_index VALUES('isl','Icelandic','Icelandic');
 INSERT INTO name_index VALUES('ism','Masimasi','Masimasi');
 INSERT INTO name_index VALUES('isn','Isanzu','Isanzu');
 INSERT INTO name_index VALUES('iso','Isoko','Isoko');
 INSERT INTO name_index VALUES('isr','Israeli Sign Language','Israeli Sign Language');
 INSERT INTO name_index VALUES('ist','Istriot','Istriot');
 INSERT INTO name_index VALUES('isu','Isu (Menchum Division)','Isu (Menchum Division)');
+INSERT INTO name_index VALUES('isv','Interslavic','Interslavic');
 INSERT INTO name_index VALUES('ita','Italian','Italian');
 INSERT INTO name_index VALUES('itb','Binongan Itneg','Itneg, Binongan');
 INSERT INTO name_index VALUES('itd','Southern Tidung','Tidung, Southern');
 INSERT INTO name_index VALUES('ite','Itene','Itene');
 INSERT INTO name_index VALUES('iti','Inlaod Itneg','Itneg, Inlaod');
 INSERT INTO name_index VALUES('itk','Judeo-Italian','Judeo-Italian');
 INSERT INTO name_index VALUES('itl','Itelmen','Itelmen');
```

### Comparing `python-iso639-2024.2.7/src/python_iso639.egg-info/PKG-INFO` & `python_iso639-2024.4.27/src/python_iso639.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: python-iso639
-Version: 2024.2.7
-Summary: Look-up utilities for ISO 639 language codes and names
+Version: 2024.4.27
+Summary: ISO 639 language codes, names, and other associated information
 Author-email: "Jackson L. Lee" <jacksonlunlee@gmail.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/jacksonllee/iso639
 Keywords: ISO 639,language codes,languages,linguistics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -24,28 +24,29 @@
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Indexing
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Provides-Extra: dev
-Requires-Dist: black==24.1.1; extra == "dev"
-Requires-Dist: build==1.0.3; extra == "dev"
+Requires-Dist: black==24.4.2; extra == "dev"
+Requires-Dist: build==1.2.1; extra == "dev"
 Requires-Dist: flake8==7.0.0; extra == "dev"
-Requires-Dist: pytest==8.0.0; extra == "dev"
-Requires-Dist: twine==4.0.2; extra == "dev"
+Requires-Dist: pytest==8.1.2; extra == "dev"
+Requires-Dist: requests==2.31.0; extra == "dev"
+Requires-Dist: twine==5.0.0; extra == "dev"
 
 # python-iso639
 
 [![PyPI version](https://badge.fury.io/py/python-iso639.svg)](https://pypi.org/project/python-iso639/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/python-iso639.svg)](https://pypi.org/project/python-iso639/)
 [![PyPI downloads last month](https://img.shields.io/pypi/dm/python-iso639)](https://pypi.org/project/python-iso639/)
 [![CircleCI Builds](https://circleci.com/gh/jacksonllee/iso639.svg?style=shield)](https://circleci.com/gh/jacksonllee/iso639)
 
-`python-iso639` is a Python package for accessing ISO 639 language codes, names, and
+`python-iso639` is a Python package for ISO 639 language codes, names, and
 other associated information.
 
 Current features:
 
 * A representation of languages mapped across ISO 639-1, 639-2, and 639-3.
 * Functionality to "guess" what a language is for a given
   unknown language code or name.
@@ -253,15 +254,15 @@
 As soon as a match is found, `Language.match` returns a `Language` instance.
 If there isn't a match, a `LanguageNotFoundError` is raised.
 
 ### `Language` is a dataclass
 
 The `Language` class is a dataclass.
 All functionality of
-[dataclases](https://docs.python.org/3/library/dataclasses.html)
+[dataclasses](https://docs.python.org/3/library/dataclasses.html)
 applies to `Language` and its instances,
 e.g., [`dataclasses.asdict`](https://docs.python.org/3/library/dataclasses.html#dataclasses.asdict):
 
 ```python
 >>> import dataclasses, iso639
 >>> language = iso639.Language.match('fra')
 >>> dataclasses.asdict(language)
@@ -271,25 +272,25 @@
 ### Constants
 
 * `DATA_LAST_UPDATED`: The release date of the included language code data from SIL
 
     ```python
     >>> import iso639
     >>> iso639.DATA_LAST_UPDATED
-    datetime.date(2024, 2, 7)
+    datetime.date(2024, 4, 15)
     ```
 
 * `ALL_LANGUAGES`: The list of all `Language` objects based on the included language code data
 
     ```python
     >>> import iso639
     >>> type(iso639.ALL_LANGUAGES)
     <class 'list'>
     >>> len(iso639.ALL_LANGUAGES)
-    7919
+    7920
     >>> iso639.ALL_LANGUAGES[0]
     Language(part3='aaa', scope='I', type='L', status='A', name='Ghotuo', ...)
     ```
 
 ## Links
 
 * Author: [Jackson L. Lee](https://jacksonllee.com)
```

### Comparing `python-iso639-2024.2.7/tests/test_language.py` & `python_iso639-2024.4.27/tests/test_language.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,21 +64,21 @@
     with pytest.raises(LanguageNotFoundError):
         Language.from_part3("Fra")  # case-sensitive!
     with pytest.raises(LanguageNotFoundError):
         Language.from_part3("unknown code")
 
 
 def test_data_last_updated():
-    assert DATA_LAST_UPDATED == datetime.date(2024, 1, 10), "Need to update README.md"
+    assert DATA_LAST_UPDATED == datetime.date(2024, 4, 15), "Need to update README.md"
 
 
 def test_all_languages():
     assert type(ALL_LANGUAGES) is list
     assert type(ALL_LANGUAGES[0]) is Language
-    assert len(ALL_LANGUAGES) == 7919, "Need to update README.md"
+    assert len(ALL_LANGUAGES) == 7920, "Need to update README.md"
 
     lang = ALL_LANGUAGES[0]
     assert lang.part3 == "aaa", "Need to update README.md"
     assert lang.name == "Ghotuo", "Need to update README.md"
 
 
 def test_eq():
```

### Comparing `python-iso639-2024.2.7/tests/test_version_number.py` & `python_iso639-2024.4.27/tests/test_version_number.py`

 * *Files identical despite different names*

