# Comparing `tmp/pypomes_core-0.8.9.tar.gz` & `tmp/pypomes_core-0.9.0.tar.gz`

## Comparing `pypomes_core-0.8.9.tar` & `pypomes_core-0.9.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/Makefile
--rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/make.bat
--rw-r--r--   0        0        0    18730 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/doctrees/environment.pickle
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/doctrees/index.doctree
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/.buildinfo
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/genindex.html
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/index.html
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/objects.inv
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/search.html
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/searchindex.js
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/alabaster.css
--rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/basic.css
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/custom.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/doctools.js
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/file.png
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/plus.png
--rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/pygments.css
--rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/source/conf.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/source/index.rst
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    23887 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/Makefile
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/make.bat
+-rw-r--r--   0        0        0    18730 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/doctrees/index.doctree
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/.buildinfo
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/genindex.html
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/index.html
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/objects.inv
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/search.html
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/alabaster.css
+-rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/source/conf.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/source/index.rst
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    23887 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/PKG-INFO
```

### Comparing `pypomes_core-0.8.9/docs/Makefile` & `pypomes_core-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/docs/make.bat` & `pypomes_core-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/docs/build/doctrees/environment.pickle` & `pypomes_core-0.9.0/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/docs/build/doctrees/index.doctree` & `pypomes_core-0.9.0/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/docs/build/html/genindex.html` & `pypomes_core-0.9.0/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/docs/build/html/index.html` & `pypomes_core-0.9.0/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/docs/build/html/search.html` & `pypomes_core-0.9.0/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/docs/build/html/searchindex.js` & `pypomes_core-0.9.0/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/docs/build/html/_static/alabaster.css` & `pypomes_core-0.9.0/docs/build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/docs/build/html/_static/basic.css` & `pypomes_core-0.9.0/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/docs/build/html/_static/doctools.js` & `pypomes_core-0.9.0/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/docs/build/html/_static/language_data.js` & `pypomes_core-0.9.0/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/docs/build/html/_static/pygments.css` & `pypomes_core-0.9.0/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/docs/build/html/_static/searchtools.js` & `pypomes_core-0.9.0/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/docs/build/html/_static/sphinx_highlight.js` & `pypomes_core-0.9.0/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/docs/source/conf.py` & `pypomes_core-0.9.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/src/pypomes_core/.ruff.toml` & `pypomes_core-0.9.0/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/src/pypomes_core/__init__.py` & `pypomes_core-0.9.0/src/pypomes_core/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,16 @@
     json_normalize_dict, json_normalize_iterable,
 )
 from .list_pomes import (
     list_compare, list_flatten, list_unflatten,
     list_find_coupled, list_elem_starting_with, list_transform,
 )
 from .str_pomes import (
-    str_sanitize, str_split_on_mark, str_find_whitespace, str_get_between, str_get_positional,
+    str_as_list, str_sanitize, str_split_on_mark,
+    str_find_whitespace, str_get_between, str_get_positional,
 )
 from .validation_msgs import (
     validate_add_msgs, validate_set_msgs
 )
 from .validation_pomes import (
     VALIDATE_MSG_LANGUAGE, VALIDATE_MSG_PREFIX,
     validate_value, validate_bool, validate_int, validate_float, validate_str,
@@ -77,15 +78,16 @@
     "file_from_request", "file_get_data",
     # json_pomes
     "json_normalize_dict", "json_normalize_iterable",
     # list_pomes
     "list_compare", "list_flatten", "list_unflatten",
     "list_find_coupled", "list_elem_starting_with", "list_transform",
     # str_pomes
-    "str_sanitize", "str_split_on_mark", "str_find_whitespace", "str_get_between", "str_get_positional",
+    "str_as_list", "str_sanitize", "str_split_on_mark",
+    "str_find_whitespace", "str_get_between", "str_get_positional",
     # validation_msgs
     "validate_add_msgs", "validate_set_msgs",
     # validation_pomes
     "VALIDATE_MSG_LANGUAGE", "VALIDATE_MSG_PREFIX",
     "validate_value", "validate_bool", "validate_int", "validate_float", "validate_str",
     "validate_date", "validate_datetime", "validate_ints", "validate_strs",
     "validate_format_error", "validate_format_errors", "validate_unformat_errors",
```

### Comparing `pypomes_core-0.8.9/src/pypomes_core/datetime_pomes.py` & `pypomes_core-0.9.0/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/src/pypomes_core/dict_pomes.py` & `pypomes_core-0.9.0/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/src/pypomes_core/email_pomes.py` & `pypomes_core-0.9.0/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/src/pypomes_core/encoding_pomes.py` & `pypomes_core-0.9.0/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/src/pypomes_core/env_pomes.py` & `pypomes_core-0.9.0/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/src/pypomes_core/exception_pomes.py` & `pypomes_core-0.9.0/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/src/pypomes_core/file_pomes.py` & `pypomes_core-0.9.0/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/src/pypomes_core/json_pomes.py` & `pypomes_core-0.9.0/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/src/pypomes_core/list_pomes.py` & `pypomes_core-0.9.0/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/src/pypomes_core/str_pomes.py` & `pypomes_core-0.9.0/src/pypomes_core/str_pomes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+from typing import Any
+
+
+def str_as_list(source: str | Any,
+                separator: str = ",") -> list[any]:
+    """
+    Return *source* as a *list*, by splitting its comma-separated contents.
+
+    If *source* is not a *str*, then it is itself returned.
+
+    :param source: the source value to be worked on
+    :param separator: the separator (defaults to ",")
+    :return: a list built from the contents of the source parameter, or that parameter itself, if is not string
+    """
+    result: str | list[Any]
+    if isinstance(source, str):
+        result = str.split(separator)
+    else:
+        result = source
+
+    return result
+
+
 def str_sanitize(target_str: str) -> str:
     """
     Clean the given *target_str* string.
 
     The sanitization is carried out by:
         - removing backslashes
         - replacing double quotes with single quotes
```

### Comparing `pypomes_core-0.8.9/src/pypomes_core/validation_msgs.py` & `pypomes_core-0.9.0/src/pypomes_core/validation_msgs.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/src/pypomes_core/validation_pomes.py` & `pypomes_core-0.9.0/src/pypomes_core/validation_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/src/pypomes_core/xml_pomes.py` & `pypomes_core-0.9.0/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/LICENSE` & `pypomes_core-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.9/pyproject.toml` & `pypomes_core-0.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.8.9"
+version = "0.9.0"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-0.8.9/PKG-INFO` & `pypomes_core-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 0.8.9
+Version: 0.9.0
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

