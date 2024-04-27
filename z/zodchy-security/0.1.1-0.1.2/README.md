# Comparing `tmp/zodchy_security-0.1.1.tar.gz` & `tmp/zodchy_security-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodchy_security-0.1.1.tar", max compression
+gzip compressed data, was "zodchy_security-0.1.2.tar", max compression
```

## Comparing `zodchy_security-0.1.1.tar` & `zodchy_security-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       17 2024-04-13 13:40:05.904405 zodchy_security-0.1.1/README.md
--rw-r--r--   0        0        0      468 2024-04-15 11:05:19.578042 zodchy_security-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       90 2024-04-11 13:37:07.017037 zodchy_security-0.1.1/zodchy_security/__init__.py
--rw-r--r--   0        0        0       36 2024-04-11 13:29:06.723696 zodchy_security-0.1.1/zodchy_security/credentials/__init__.py
--rw-r--r--   0        0        0       87 2024-04-11 13:29:06.729526 zodchy_security-0.1.1/zodchy_security/credentials/otp.py
--rw-r--r--   0        0        0        0 2024-04-11 13:14:21.400474 zodchy_security-0.1.1/zodchy_security/tokens/__init__.py
--rw-r--r--   0        0        0     1053 2024-04-11 13:23:33.081141 zodchy_security-0.1.1/zodchy_security/tokens/jwts.py
--rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 zodchy_security-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-04-13 13:40:05.904405 zodchy_security-0.1.2/README.md
+-rw-r--r--   0        0        0      450 2024-04-27 11:29:20.370312 zodchy_security-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       90 2024-04-11 13:37:07.017037 zodchy_security-0.1.2/zodchy_security/__init__.py
+-rw-r--r--   0        0        0       36 2024-04-11 13:29:06.723696 zodchy_security-0.1.2/zodchy_security/credentials/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-11 13:29:06.729526 zodchy_security-0.1.2/zodchy_security/credentials/otp.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:14:21.400474 zodchy_security-0.1.2/zodchy_security/tokens/__init__.py
+-rw-r--r--   0        0        0     1053 2024-04-11 13:23:33.081141 zodchy_security-0.1.2/zodchy_security/tokens/jwts.py
+-rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 zodchy_security-0.1.2/PKG-INFO
```

### Comparing `zodchy_security-0.1.1/zodchy_security/tokens/jwts.py` & `zodchy_security-0.1.2/zodchy_security/tokens/jwts.py`

 * *Files identical despite different names*

### Comparing `zodchy_security-0.1.1/PKG-INFO` & `zodchy_security-0.1.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: zodchy-security
-Version: 0.1.1
+Version: 0.1.2
 Summary: Collection of tools to secure application with zodchy architecture
 Home-page: https://github.com/smairon/zodchy-security
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
-Requires-Dist: zodchy (>=0.1.0,<0.2.0)
 Project-URL: Repository, https://github.com/smairon/zodchy-security
 Description-Content-Type: text/markdown
 
 # Zodchy security
```

