# Comparing `tmp/capmonster_python-3.1.0.tar.gz` & `tmp/capmonster_python-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capmonster_python-3.1.0.tar", last modified: Wed Apr 17 18:55:46 2024, max compression
+gzip compressed data, was "capmonster_python-3.2.0.tar", last modified: Sat Apr 27 13:03:32 2024, max compression
```

## Comparing `capmonster_python-3.1.0.tar` & `capmonster_python-3.2.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:55:46.220413 capmonster_python-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-17 18:55:39.000000 capmonster_python-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-17 18:55:46.220413 capmonster_python-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-17 18:55:39.000000 capmonster_python-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:55:46.216413 capmonster_python-3.1.0/capmonster_python/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-17 18:55:39.000000 capmonster_python-3.1.0/capmonster_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-04-17 18:55:39.000000 capmonster_python-3.1.0/capmonster_python/capmonster.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-17 18:55:39.000000 capmonster_python-3.1.0/capmonster_python/compleximage.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-17 18:55:39.000000 capmonster_python-3.1.0/capmonster_python/datadome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-17 18:55:39.000000 capmonster_python-3.1.0/capmonster_python/fun_captcha.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-17 18:55:39.000000 capmonster_python-3.1.0/capmonster_python/geetest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-17 18:55:39.000000 capmonster_python-3.1.0/capmonster_python/hcaptcha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-17 18:55:39.000000 capmonster_python-3.1.0/capmonster_python/image_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-17 18:55:39.000000 capmonster_python-3.1.0/capmonster_python/recaptcha_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-17 18:55:39.000000 capmonster_python-3.1.0/capmonster_python/recaptcha_v2_enterprise.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-17 18:55:39.000000 capmonster_python-3.1.0/capmonster_python/recaptcha_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-17 18:55:39.000000 capmonster_python-3.1.0/capmonster_python/tendi.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-17 18:55:39.000000 capmonster_python-3.1.0/capmonster_python/turnstile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-17 18:55:39.000000 capmonster_python-3.1.0/capmonster_python/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:55:46.220413 capmonster_python-3.1.0/capmonster_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-17 18:55:46.000000 capmonster_python-3.1.0/capmonster_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-17 18:55:46.000000 capmonster_python-3.1.0/capmonster_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 18:55:46.000000 capmonster_python-3.1.0/capmonster_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 18:55:46.000000 capmonster_python-3.1.0/capmonster_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-17 18:55:46.000000 capmonster_python-3.1.0/capmonster_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 18:55:46.220413 capmonster_python-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-17 18:55:39.000000 capmonster_python-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:03:32.984691 capmonster_python-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-27 13:03:22.000000 capmonster_python-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-27 13:03:32.984691 capmonster_python-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-27 13:03:22.000000 capmonster_python-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:03:32.984691 capmonster_python-3.2.0/capmonster_python/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-27 13:03:22.000000 capmonster_python-3.2.0/capmonster_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-27 13:03:22.000000 capmonster_python-3.2.0/capmonster_python/aws_waf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-04-27 13:03:22.000000 capmonster_python-3.2.0/capmonster_python/capmonster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-27 13:03:22.000000 capmonster_python-3.2.0/capmonster_python/compleximage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-27 13:03:22.000000 capmonster_python-3.2.0/capmonster_python/datadome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-27 13:03:22.000000 capmonster_python-3.2.0/capmonster_python/fun_captcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-27 13:03:22.000000 capmonster_python-3.2.0/capmonster_python/geetest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-27 13:03:22.000000 capmonster_python-3.2.0/capmonster_python/hcaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-27 13:03:22.000000 capmonster_python-3.2.0/capmonster_python/image_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-27 13:03:22.000000 capmonster_python-3.2.0/capmonster_python/recaptcha_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-27 13:03:22.000000 capmonster_python-3.2.0/capmonster_python/recaptcha_v2_enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-27 13:03:22.000000 capmonster_python-3.2.0/capmonster_python/recaptcha_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-27 13:03:22.000000 capmonster_python-3.2.0/capmonster_python/tendi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-27 13:03:22.000000 capmonster_python-3.2.0/capmonster_python/turnstile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-27 13:03:22.000000 capmonster_python-3.2.0/capmonster_python/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:03:32.984691 capmonster_python-3.2.0/capmonster_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-27 13:03:32.000000 capmonster_python-3.2.0/capmonster_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-27 13:03:32.000000 capmonster_python-3.2.0/capmonster_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 13:03:32.000000 capmonster_python-3.2.0/capmonster_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-27 13:03:32.000000 capmonster_python-3.2.0/capmonster_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 13:03:32.000000 capmonster_python-3.2.0/capmonster_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-27 13:03:32.984691 capmonster_python-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-27 13:03:23.000000 capmonster_python-3.2.0/setup.py
```

### Comparing `capmonster_python-3.1.0/LICENSE` & `capmonster_python-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `capmonster_python-3.1.0/PKG-INFO` & `capmonster_python-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capmonster_python
-Version: 3.1.0
+Version: 3.2.0
 Summary: capmonster.cloud library for Python
 Home-page: https://github.com/alperensert/capmonster_python
 Author: Alperen Sert
 Author-email: business@alperen.io
 License: MIT
 Project-URL: Documentation, https://alperensert.github.io/capmonster_python/
 Project-URL: Source, https://github.com/alperensert/capmonster_python/
```

### Comparing `capmonster_python-3.1.0/README.md` & `capmonster_python-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `capmonster_python-3.1.0/capmonster_python/capmonster.py` & `capmonster_python-3.2.0/capmonster_python/capmonster.py`

 * *Files identical despite different names*

### Comparing `capmonster_python-3.1.0/capmonster_python/compleximage.py` & `capmonster_python-3.2.0/capmonster_python/compleximage.py`

 * *Files identical despite different names*

### Comparing `capmonster_python-3.1.0/capmonster_python/datadome.py` & `capmonster_python-3.2.0/capmonster_python/datadome.py`

 * *Files identical despite different names*

### Comparing `capmonster_python-3.1.0/capmonster_python/fun_captcha.py` & `capmonster_python-3.2.0/capmonster_python/fun_captcha.py`

 * *Files identical despite different names*

### Comparing `capmonster_python-3.1.0/capmonster_python/geetest.py` & `capmonster_python-3.2.0/capmonster_python/geetest.py`

 * *Files identical despite different names*

### Comparing `capmonster_python-3.1.0/capmonster_python/hcaptcha.py` & `capmonster_python-3.2.0/capmonster_python/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `capmonster_python-3.1.0/capmonster_python/image_to_text.py` & `capmonster_python-3.2.0/capmonster_python/image_to_text.py`

 * *Files identical despite different names*

### Comparing `capmonster_python-3.1.0/capmonster_python/recaptcha_v2.py` & `capmonster_python-3.2.0/capmonster_python/recaptcha_v2.py`

 * *Files identical despite different names*

### Comparing `capmonster_python-3.1.0/capmonster_python/recaptcha_v2_enterprise.py` & `capmonster_python-3.2.0/capmonster_python/recaptcha_v2_enterprise.py`

 * *Files identical despite different names*

### Comparing `capmonster_python-3.1.0/capmonster_python/recaptcha_v3.py` & `capmonster_python-3.2.0/capmonster_python/recaptcha_v3.py`

 * *Files identical despite different names*

### Comparing `capmonster_python-3.1.0/capmonster_python/tendi.py` & `capmonster_python-3.2.0/capmonster_python/tendi.py`

 * *Files identical despite different names*

### Comparing `capmonster_python-3.1.0/capmonster_python/turnstile.py` & `capmonster_python-3.2.0/capmonster_python/turnstile.py`

 * *Files identical despite different names*

### Comparing `capmonster_python-3.1.0/capmonster_python/utils.py` & `capmonster_python-3.2.0/capmonster_python/utils.py`

 * *Files identical despite different names*

### Comparing `capmonster_python-3.1.0/capmonster_python.egg-info/PKG-INFO` & `capmonster_python-3.2.0/capmonster_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capmonster_python
-Version: 3.1.0
+Version: 3.2.0
 Summary: capmonster.cloud library for Python
 Home-page: https://github.com/alperensert/capmonster_python
 Author: Alperen Sert
 Author-email: business@alperen.io
 License: MIT
 Project-URL: Documentation, https://alperensert.github.io/capmonster_python/
 Project-URL: Source, https://github.com/alperensert/capmonster_python/
```

### Comparing `capmonster_python-3.1.0/capmonster_python.egg-info/SOURCES.txt` & `capmonster_python-3.2.0/capmonster_python.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 capmonster_python/__init__.py
+capmonster_python/aws_waf.py
 capmonster_python/capmonster.py
 capmonster_python/compleximage.py
 capmonster_python/datadome.py
 capmonster_python/fun_captcha.py
 capmonster_python/geetest.py
 capmonster_python/hcaptcha.py
 capmonster_python/image_to_text.py
```

### Comparing `capmonster_python-3.1.0/setup.py` & `capmonster_python-3.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="capmonster_python",
-    version="3.1.0",
+    version="3.2.0",
     packages=["capmonster_python"],
     url="https://github.com/alperensert/capmonster_python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     author="Alperen Sert",
     author_email="business@alperen.io",
```

