# Comparing `tmp/midsummer-0.1.0.tar.gz` & `tmp/midsummer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midsummer-0.1.0.tar", max compression
+gzip compressed data, was "midsummer-0.1.1.tar", max compression
```

## Comparing `midsummer-0.1.0.tar` & `midsummer-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1481 2024-04-27 17:43:00.332605 midsummer-0.1.0/README.md
--rw-r--r--   0        0        0       58 2024-04-27 17:43:00.332605 midsummer-0.1.0/midsummer/__init__.py
--rw-r--r--   0        0        0     1202 2024-04-27 17:43:00.332605 midsummer-0.1.0/midsummer/midsummer.py
--rw-r--r--   0        0        0     1262 2024-04-27 17:43:00.332605 midsummer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1765 1970-01-01 00:00:00.000000 midsummer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1243 2024-04-27 20:26:09.820341 midsummer-0.1.1/README.md
+-rw-r--r--   0        0        0       58 2024-04-27 20:26:09.820341 midsummer-0.1.1/midsummer/__init__.py
+-rw-r--r--   0        0        0     1202 2024-04-27 20:26:09.820341 midsummer-0.1.1/midsummer/midsummer.py
+-rw-r--r--   0        0        0     1276 2024-04-27 20:26:09.820341 midsummer-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1541 1970-01-01 00:00:00.000000 midsummer-0.1.1/PKG-INFO
```

### Comparing `midsummer-0.1.0/README.md` & `midsummer-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: midsummer
+Version: 0.1.1
+Summary: Midsummer Date
+Author: fredrik
+Author-email: nfredrik@hotmail.com
+Requires-Python: >=3.12,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+
 # Midsummer Date Calculator
 
 This Python module calculates the date of Midsummer's Day for a given year. Midsummer's Day typically falls on a Friday between June 20th and June 26th.
 
 ## Features
 
 - **Custom Exception**: Includes a `MidsummerException` for handling errors specific to the Midsummer date calculation.
@@ -23,14 +34,10 @@
 ## Functionality
 The midsummer_date function calculates the date of Midsummer’s Day for the specified year. If the calculated date does not fall on a Friday, a ValueError is raised.
 
 ## Exceptions
 MidsummerException: Raised if the input year is not an integer or if the date falls outside the expected range.
 ValueError: Raised if the calculated Midsummer’s Day does not fall on a Friday, as per tradition.
 
-## Constants
-FIRST_POSSIBLE_DAY: The earliest possible day in June that Midsummer’s Day can fall on.
-MIDSUMMER_MONTH: The month of June.
-DAYS_IN_A_WEEK_ZERO_CNT: The number of days to check from the first possible day to find a Friday.
-
 ## License
-This project is licensed under the MIT License - see the LICENSE.md file for details.
+This project is licensed under the MIT License - see the LICENSE.md file for details.
+
```

### Comparing `midsummer-0.1.0/midsummer/midsummer.py` & `midsummer-0.1.1/midsummer/midsummer.py`

 * *Files identical despite different names*

### Comparing `midsummer-0.1.0/pyproject.toml` & `midsummer-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "midsummer"
-version = "0.1.0"
-description = ""
+version = "0.1.1"
+description = "Midsummer Date"
 authors = ["fredrik <nfredrik@hotmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 
 [[tool.poetry.source]]
```

