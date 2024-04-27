# Comparing `tmp/espy_contact-0.1.tar.gz` & `tmp/espy_contact-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espy_contact-0.1.tar", last modified: Fri Apr 26 16:29:49 2024, max compression
+gzip compressed data, was "espy_contact-0.2.tar", last modified: Sat Apr 27 02:59:59 2024, max compression
```

## Comparing `espy_contact-0.1.tar` & `espy_contact-0.2.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:29:49.765822 espy_contact-0.1/
--rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-04-26 01:29:16.000000 espy_contact-0.1/LICENSE
--rw-r--r--   0 philipadigun   (501) staff       (20)      348 2024-04-26 16:29:49.765678 espy_contact-0.1/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      109 2024-04-26 04:34:47.000000 espy_contact-0.1/README.md
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:29:49.764335 espy_contact-0.1/espy_contact/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.1/espy_contact/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2723 2024-04-26 04:04:33.000000 espy_contact-0.1/espy_contact/schema.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1396 2024-04-26 16:25:18.000000 espy_contact-0.1/espy_contact/service.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:29:49.765056 espy_contact-0.1/espy_contact.egg-info/
--rw-r--r--   0 philipadigun   (501) staff       (20)      348 2024-04-26 16:29:49.000000 espy_contact-0.1/espy_contact.egg-info/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      341 2024-04-26 16:29:49.000000 espy_contact-0.1/espy_contact.egg-info/SOURCES.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-04-26 16:29:49.000000 espy_contact-0.1/espy_contact.egg-info/dependency_links.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       63 2024-04-26 16:29:49.000000 espy_contact-0.1/espy_contact.egg-info/requires.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       19 2024-04-26 16:29:49.000000 espy_contact-0.1/espy_contact.egg-info/top_level.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-04-26 16:29:49.765870 espy_contact-0.1/setup.cfg
--rw-r--r--   0 philipadigun   (501) staff       (20)      631 2024-04-26 16:29:05.000000 espy_contact-0.1/setup.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:29:49.765513 espy_contact-0.1/tests/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.1/tests/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1621 2024-04-26 01:31:37.000000 espy_contact-0.1/tests/test_copyright.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.1/tests/test_service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 02:59:59.376239 espy_contact-0.2/
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-04-26 01:29:16.000000 espy_contact-0.2/LICENSE
+-rw-r--r--   0 philipadigun   (501) staff       (20)      348 2024-04-27 02:59:59.376114 espy_contact-0.2/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      109 2024-04-26 04:34:47.000000 espy_contact-0.2/README.md
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 02:59:59.373762 espy_contact-0.2/espy_contact/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.2/espy_contact/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 02:59:59.374722 espy_contact-0.2/espy_contact/model/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:34:03.000000 espy_contact-0.2/espy_contact/model/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1091 2024-04-26 04:22:51.000000 espy_contact-0.2/espy_contact/model/models.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2723 2024-04-26 04:04:33.000000 espy_contact-0.2/espy_contact/schema.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1574 2024-04-27 02:59:30.000000 espy_contact-0.2/espy_contact/service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 02:59:59.375289 espy_contact-0.2/espy_contact/util/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      959 2024-04-26 03:59:10.000000 espy_contact-0.2/espy_contact/util/CONSTANTS.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:33:54.000000 espy_contact-0.2/espy_contact/util/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3777 2024-04-26 01:33:55.000000 espy_contact-0.2/espy_contact/util/enums.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 02:59:59.374490 espy_contact-0.2/espy_contact.egg-info/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      348 2024-04-27 02:59:59.000000 espy_contact-0.2/espy_contact.egg-info/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      489 2024-04-27 02:59:59.000000 espy_contact-0.2/espy_contact.egg-info/SOURCES.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-04-27 02:59:59.000000 espy_contact-0.2/espy_contact.egg-info/dependency_links.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       63 2024-04-27 02:59:59.000000 espy_contact-0.2/espy_contact.egg-info/requires.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       19 2024-04-27 02:59:59.000000 espy_contact-0.2/espy_contact.egg-info/top_level.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-04-27 02:59:59.376293 espy_contact-0.2/setup.cfg
+-rw-r--r--   0 philipadigun   (501) staff       (20)      631 2024-04-27 02:59:43.000000 espy_contact-0.2/setup.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 02:59:59.375943 espy_contact-0.2/tests/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.2/tests/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1621 2024-04-26 01:31:37.000000 espy_contact-0.2/tests/test_copyright.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.2/tests/test_service.py
```

### Comparing `espy_contact-0.1/LICENSE` & `espy_contact-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `espy_contact-0.1/espy_contact/schema.py` & `espy_contact-0.2/espy_contact/schema.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.1/espy_contact/service.py` & `espy_contact-0.2/espy_contact/service.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 
 def verify_password(plain_password: str, hashed_password: str) -> bool:
     """
     Verify a plain password against the hashed version.
     """
     # Ensure both plain_password and hashed_password are bytes
     return bcrypt.checkpw(plain_password.encode(), hashed_password.encode())
+def encrypt_pass(plain_password: str) -> str:
+    """Hash a password for storing."""
+    salt = bcrypt.gensalt()
+    return bcrypt.hashpw(plain_password.encode(), salt).decode()
 
 def user_login():
     pass
 
 def user_register():
     pass
```

### Comparing `espy_contact-0.1/setup.py` & `espy_contact-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 VERSION = '0.0.2'
 DESCRIPTION = 'ESSL users management'
 LONG_DESCRIPTION = 'Internal helper package for ESSL users management'
 setup(
     name='espy_contact',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     install_requires=[
         'bcrypt==4.1.2',
         'pytest==8.1.1',
         'pydantic==2.7.1',
         'sqlalchemy==2.0.29'
         ],
```

### Comparing `espy_contact-0.1/tests/test_copyright.py` & `espy_contact-0.2/tests/test_copyright.py`

 * *Files identical despite different names*

