# Comparing `tmp/tormail-0.0.2.tar.gz` & `tmp/tormail-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tormail-0.0.2.tar", last modified: Sat Apr 27 15:50:20 2024, max compression
+gzip compressed data, was "tormail-0.0.3.tar", last modified: Sat Apr 27 15:56:12 2024, max compression
```

## Comparing `tormail-0.0.2.tar` & `tormail-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 15:50:20.557896 tormail-0.0.2/
--rw-rw-rw-   0        0        0       86 2024-04-27 15:50:20.555896 tormail-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-27 13:44:27.000000 tormail-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 15:50:20.557896 tormail-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      190 2024-04-27 15:49:16.000000 tormail-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 15:50:20.541896 tormail-0.0.2/tormail/
--rw-rw-rw-   0        0        0       58 2024-04-27 15:46:08.000000 tormail-0.0.2/tormail/__init__.py
--rw-rw-rw-   0        0        0     1727 2024-04-27 15:35:57.000000 tormail-0.0.2/tormail/listen.py
--rw-rw-rw-   0        0        0     3373 2024-04-27 15:45:49.000000 tormail-0.0.2/tormail/mail.py
-drwxrwxrwx   0        0        0        0 2024-04-27 15:50:20.553897 tormail-0.0.2/tormail.egg-info/
--rw-rw-rw-   0        0        0       86 2024-04-27 15:50:20.000000 tormail-0.0.2/tormail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2024-04-27 15:50:20.000000 tormail-0.0.2/tormail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 15:50:20.000000 tormail-0.0.2/tormail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-27 15:50:20.000000 tormail-0.0.2/tormail.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-27 15:50:20.000000 tormail-0.0.2/tormail.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 15:56:12.464341 tormail-0.0.3/
+-rw-rw-rw-   0        0        0       86 2024-04-27 15:56:12.462341 tormail-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-27 13:44:27.000000 tormail-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 15:56:12.464341 tormail-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      190 2024-04-27 15:55:53.000000 tormail-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 15:56:12.439343 tormail-0.0.3/tormail/
+-rw-rw-rw-   0        0        0       58 2024-04-27 15:46:08.000000 tormail-0.0.3/tormail/__init__.py
+-rw-rw-rw-   0        0        0     1727 2024-04-27 15:35:57.000000 tormail-0.0.3/tormail/listen.py
+-rw-rw-rw-   0        0        0     3374 2024-04-27 15:55:46.000000 tormail-0.0.3/tormail/mail.py
+drwxrwxrwx   0        0        0        0 2024-04-27 15:56:12.460342 tormail-0.0.3/tormail.egg-info/
+-rw-rw-rw-   0        0        0       86 2024-04-27 15:56:12.000000 tormail-0.0.3/tormail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2024-04-27 15:56:12.000000 tormail-0.0.3/tormail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 15:56:12.000000 tormail-0.0.3/tormail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-27 15:56:12.000000 tormail-0.0.3/tormail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-27 15:56:12.000000 tormail-0.0.3/tormail.egg-info/top_level.txt
```

### Comparing `tormail-0.0.2/tormail/listen.py` & `tormail-0.0.3/tormail/listen.py`

 * *Files identical despite different names*

### Comparing `tormail-0.0.2/tormail/mail.py` & `tormail-0.0.3/tormail/mail.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import string
 import random
 import requests
-from listen import Listener
+from .listen import Listener
 
 class MailClient(Listener):
     def __init__(self):
         super().__init__()  # Call the constructor of the superclass
         self.account_url = "https://api.mail.tm/accounts"
         self.token_url = "https://api.mail.tm/token"
         self.token = None  # Initialize token attribute
```

