# Comparing `tmp/ownlib-0.0.1b4.tar.gz` & `tmp/ownlib-0.0.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ownlib-0.0.1b4.tar", max compression
+gzip compressed data, was "ownlib-0.0.1b5.tar", max compression
```

## Comparing `ownlib-0.0.1b4.tar` & `ownlib-0.0.1b5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2022-10-30 19:22:48.704414 ownlib-0.0.1b4/LICENSE
--rw-r--r--   0        0        0      140 2024-03-03 12:27:11.775267 ownlib-0.0.1b4/README.md
--rw-r--r--   0        0        0      638 2024-04-13 19:28:55.405393 ownlib-0.0.1b4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-03 12:27:11.775267 ownlib-0.0.1b4/src/ownlib/__init__.py
--rw-r--r--   0        0        0     2213 2024-04-12 17:12:32.850420 ownlib-0.0.1b4/src/ownlib/class_person.py
--rw-r--r--   0        0        0     4503 2024-04-12 17:12:32.850420 ownlib-0.0.1b4/src/ownlib/class_whatsapp_message.py
--rw-r--r--   0        0        0    13461 2024-04-12 17:12:32.850420 ownlib-0.0.1b4/src/ownlib/functions_whatsapp_refueling.py
--rw-r--r--   0        0        0     2074 2024-04-12 17:12:32.850420 ownlib-0.0.1b4/src/ownlib/months.py
--rw-r--r--   0        0        0     9806 2024-04-12 17:12:32.850420 ownlib-0.0.1b4/src/ownlib/my_datalib.py
--rw-r--r--   0        0        0      390 2024-04-12 17:12:32.850420 ownlib-0.0.1b4/src/ownlib/my_fileio.py
--rw-r--r--   0        0        0     9512 2024-04-12 17:12:32.850420 ownlib-0.0.1b4/src/ownlib/mytinylib.py
--rw-r--r--   0        0        0     1708 2024-03-03 12:27:11.779267 ownlib-0.0.1b4/src/ownlib/one_s_uat_lib.py
--rw-r--r--   0        0        0      164 2024-03-03 12:27:11.779267 ownlib-0.0.1b4/src/ownlib/platon_settings.py
--rw-r--r--   0        0        0     5257 2024-04-12 17:12:32.850420 ownlib-0.0.1b4/src/ownlib/txt_lib.py
--rw-r--r--   0        0        0     2138 2024-04-12 17:12:32.850420 ownlib-0.0.1b4/src/ownlib/whapp_funcs.py
--rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 ownlib-0.0.1b4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-10-30 19:22:48.704414 ownlib-0.0.1b5/LICENSE
+-rw-r--r--   0        0        0      140 2024-03-03 12:27:11.775267 ownlib-0.0.1b5/README.md
+-rw-r--r--   0        0        0      638 2024-04-27 20:27:31.889044 ownlib-0.0.1b5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-03 12:27:11.775267 ownlib-0.0.1b5/src/ownlib/__init__.py
+-rw-r--r--   0        0        0     2213 2024-04-12 17:12:32.850420 ownlib-0.0.1b5/src/ownlib/class_person.py
+-rw-r--r--   0        0        0     4503 2024-04-12 17:12:32.850420 ownlib-0.0.1b5/src/ownlib/class_whatsapp_message.py
+-rw-r--r--   0        0        0    13461 2024-04-12 17:12:32.850420 ownlib-0.0.1b5/src/ownlib/functions_whatsapp_refueling.py
+-rw-r--r--   0        0        0     2074 2024-04-12 17:12:32.850420 ownlib-0.0.1b5/src/ownlib/months.py
+-rw-r--r--   0        0        0     9806 2024-04-12 17:12:32.850420 ownlib-0.0.1b5/src/ownlib/my_datalib.py
+-rw-r--r--   0        0        0      390 2024-04-12 17:12:32.850420 ownlib-0.0.1b5/src/ownlib/my_fileio.py
+-rw-r--r--   0        0        0     9496 2024-04-27 20:19:48.292053 ownlib-0.0.1b5/src/ownlib/mytinylib.py
+-rw-r--r--   0        0        0     1708 2024-03-03 12:27:11.779267 ownlib-0.0.1b5/src/ownlib/one_s_uat_lib.py
+-rw-r--r--   0        0        0      164 2024-03-03 12:27:11.779267 ownlib-0.0.1b5/src/ownlib/platon_settings.py
+-rw-r--r--   0        0        0     5512 2024-04-26 05:53:41.129855 ownlib-0.0.1b5/src/ownlib/txt_lib.py
+-rw-r--r--   0        0        0     2138 2024-04-12 17:12:32.850420 ownlib-0.0.1b5/src/ownlib/whapp_funcs.py
+-rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 ownlib-0.0.1b5/PKG-INFO
```

### Comparing `ownlib-0.0.1b4/LICENSE` & `ownlib-0.0.1b5/LICENSE`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1b4/pyproject.toml` & `ownlib-0.0.1b5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ownlib"
-version = "0.0.1b4"
+version = "0.0.1b5"
 description = "Sample pypi project"
 authors = ["Андрей Мартынов <real.cloudhunter@gmail.com>"]
 license = "GNU"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `ownlib-0.0.1b4/src/ownlib/class_person.py` & `ownlib-0.0.1b5/src/ownlib/class_person.py`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1b4/src/ownlib/class_whatsapp_message.py` & `ownlib-0.0.1b5/src/ownlib/class_whatsapp_message.py`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1b4/src/ownlib/functions_whatsapp_refueling.py` & `ownlib-0.0.1b5/src/ownlib/functions_whatsapp_refueling.py`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1b4/src/ownlib/months.py` & `ownlib-0.0.1b5/src/ownlib/months.py`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1b4/src/ownlib/my_datalib.py` & `ownlib-0.0.1b5/src/ownlib/my_datalib.py`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1b4/src/ownlib/mytinylib.py` & `ownlib-0.0.1b5/src/ownlib/mytinylib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Short useful functions library
 """
 from typing import (Any,
-                    Union
+                    Sequence,
                     )
 import os
 from glob import glob
 import pathlib
 from hashlib import md5
 
 from datetime import datetime
@@ -73,16 +73,16 @@
 
 
 def show_choices(choices: list, axe: str = 'v'):
     """
         TODO add some description
     """
     if axe == 'v':
-        max_chars_in_item = max(choices, key=len, default=0)
-        max_chars_in_idx = len(str(len(choices)))
+        max_chars_in_item = len(max(choices, key=len, default=0))
+        max_chars_in_idx = len(choices) % 10
         max_line_length = max_chars_in_idx + 2 + max_chars_in_item
         div_line = repeated_string(max_line_length)
 
         print(div_line)
         for i, item in enumerate(choices):
             print(f"{i}: {item}")
         print(div_line)
@@ -103,15 +103,15 @@
     Show warning message
     :param message:
     :return: None
     """
     print(f"[!] Wrong input value: {message}")
 
 
-def last_index(sequence: Union[str, list, tuple, set]) -> int:
+def last_index(sequence: Sequence) -> int:
     """
     Return last iterator index\n
     :param sequence: - data sequence for example
     :return: last index in iterator
     """
     return len(sequence) - 1
```

### Comparing `ownlib-0.0.1b4/src/ownlib/one_s_uat_lib.py` & `ownlib-0.0.1b5/src/ownlib/one_s_uat_lib.py`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1b4/src/ownlib/txt_lib.py` & `ownlib-0.0.1b5/src/ownlib/txt_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,21 +125,24 @@
 
 
 def string_transform(manipulated_string: str,
                      rules: dict[str, str] | None = None) -> str | None:
     """Change change_rules.key => change_rules.value in manipulated_string
 
     :param manipulated_string: str - source string on which we could change a symbols
+    # TODO Have change to ordered dict type
     :param rules: dict - {symbol_from_change : symbol_to_change}
     :return: result string: str
-    Example rules: rules = {'\xa0' : EMPTY_STR\n' : ' '}
+    Example rules: rules = {'\xa0' : EMPTY_STR, '\n' : ' '}
     """
     result_string = ''
+    # Leave here default value setting else catch default mutable warning in func arg line
     rules = rules if rules else {'\xa0': EMPTY_STR}
 
+    # TODO use str.replace() here, but with type(rules) == OrderedDict
     for char in manipulated_string:
         result_string += rules[char] \
             if char in rules else char
     return result_string
 
 
 def list_transform(manipulated_list: list[str],
@@ -177,14 +180,15 @@
     return float_arg
 
 
 def items_in_string(analysing_string: str,
                     parent_list: list[str]) -> list[str]:
     """
     Return the ordered list of words from analysing string,
+    # TODO Rename variables Idea - 'patterns'
     which have equals in the predefined list
 
     :param analysing_string: str - Analysing string
     :param parent_list: list[str] - Predefined list
     :return: list[str] - An ordered list of words equals the same
     ones in parent_list
     """
```

### Comparing `ownlib-0.0.1b4/src/ownlib/whapp_funcs.py` & `ownlib-0.0.1b5/src/ownlib/whapp_funcs.py`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1b4/PKG-INFO` & `ownlib-0.0.1b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ownlib
-Version: 0.0.1b4
+Version: 0.0.1b5
 Summary: Sample pypi project
 License: GNU
 Author: Андрей Мартынов
 Author-email: real.cloudhunter@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

