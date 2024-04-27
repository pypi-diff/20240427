# Comparing `tmp/enhancedwebdriver-0.1.5.tar.gz` & `tmp/enhancedwebdriver-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhancedwebdriver-0.1.5.tar", last modified: Thu Apr 25 09:05:43 2024, max compression
+gzip compressed data, was "enhancedwebdriver-0.1.6.tar", last modified: Sat Apr 27 13:53:07 2024, max compression
```

## Comparing `enhancedwebdriver-0.1.5.tar` & `enhancedwebdriver-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-25 09:05:43.070170 enhancedwebdriver-0.1.5/
--rw-rw-r--   0 tesla     (1000) tesla     (1000)     1070 2024-04-12 20:08:24.000000 enhancedwebdriver-0.1.5/LICENSE
--rw-r--r--   0 tesla     (1000) tesla     (1000)     1106 2024-04-25 09:05:43.070170 enhancedwebdriver-0.1.5/PKG-INFO
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      465 2024-04-13 15:12:35.000000 enhancedwebdriver-0.1.5/README.md
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      106 2024-04-12 19:44:41.000000 enhancedwebdriver-0.1.5/pyproject.toml
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      743 2024-04-25 09:05:43.070170 enhancedwebdriver-0.1.5/setup.cfg
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-25 09:05:43.066170 enhancedwebdriver-0.1.5/src/
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-25 09:05:43.070170 enhancedwebdriver-0.1.5/src/EnhancedWebdriver.egg-info/
--rw-r--r--   0 tesla     (1000) tesla     (1000)     1106 2024-04-25 09:05:43.000000 enhancedwebdriver-0.1.5/src/EnhancedWebdriver.egg-info/PKG-INFO
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      345 2024-04-25 09:05:43.000000 enhancedwebdriver-0.1.5/src/EnhancedWebdriver.egg-info/SOURCES.txt
--rw-rw-r--   0 tesla     (1000) tesla     (1000)        1 2024-04-25 09:05:43.000000 enhancedwebdriver-0.1.5/src/EnhancedWebdriver.egg-info/dependency_links.txt
--rw-rw-r--   0 tesla     (1000) tesla     (1000)       64 2024-04-25 09:05:43.000000 enhancedwebdriver-0.1.5/src/EnhancedWebdriver.egg-info/requires.txt
--rw-rw-r--   0 tesla     (1000) tesla     (1000)       19 2024-04-25 09:05:43.000000 enhancedwebdriver-0.1.5/src/EnhancedWebdriver.egg-info/top_level.txt
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-25 09:05:43.070170 enhancedwebdriver-0.1.5/src/enhanced_webdriver/
--rw-rw-r--   0 tesla     (1000) tesla     (1000)    10303 2024-04-25 09:01:33.000000 enhancedwebdriver-0.1.5/src/enhanced_webdriver/EnhancedWebdriver.py
--rw-rw-r--   0 tesla     (1000) tesla     (1000)       82 2024-04-12 20:08:24.000000 enhancedwebdriver-0.1.5/src/enhanced_webdriver/__init__.py
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-27 13:53:07.633942 enhancedwebdriver-0.1.6/
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)     1070 2024-04-12 20:08:24.000000 enhancedwebdriver-0.1.6/LICENSE
+-rw-r--r--   0 tesla     (1000) tesla     (1000)     1106 2024-04-27 13:53:07.633942 enhancedwebdriver-0.1.6/PKG-INFO
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)      465 2024-04-13 15:12:35.000000 enhancedwebdriver-0.1.6/README.md
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)      106 2024-04-12 19:44:41.000000 enhancedwebdriver-0.1.6/pyproject.toml
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)      743 2024-04-27 13:53:07.633942 enhancedwebdriver-0.1.6/setup.cfg
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-27 13:53:07.625942 enhancedwebdriver-0.1.6/src/
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-27 13:53:07.629942 enhancedwebdriver-0.1.6/src/EnhancedWebdriver.egg-info/
+-rw-r--r--   0 tesla     (1000) tesla     (1000)     1106 2024-04-27 13:53:07.000000 enhancedwebdriver-0.1.6/src/EnhancedWebdriver.egg-info/PKG-INFO
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)      345 2024-04-27 13:53:07.000000 enhancedwebdriver-0.1.6/src/EnhancedWebdriver.egg-info/SOURCES.txt
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)        1 2024-04-27 13:53:07.000000 enhancedwebdriver-0.1.6/src/EnhancedWebdriver.egg-info/dependency_links.txt
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)       64 2024-04-27 13:53:07.000000 enhancedwebdriver-0.1.6/src/EnhancedWebdriver.egg-info/requires.txt
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)       19 2024-04-27 13:53:07.000000 enhancedwebdriver-0.1.6/src/EnhancedWebdriver.egg-info/top_level.txt
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-27 13:53:07.629942 enhancedwebdriver-0.1.6/src/enhanced_webdriver/
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)    10376 2024-04-27 13:10:00.000000 enhancedwebdriver-0.1.6/src/enhanced_webdriver/EnhancedWebdriver.py
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)       82 2024-04-12 20:08:24.000000 enhancedwebdriver-0.1.6/src/enhanced_webdriver/__init__.py
```

### Comparing `enhancedwebdriver-0.1.5/LICENSE` & `enhancedwebdriver-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `enhancedwebdriver-0.1.5/PKG-INFO` & `enhancedwebdriver-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnhancedWebdriver
-Version: 0.1.5
+Version: 0.1.6
 Summary: Extension of webdriver with less boilerplate
 Home-page: https://github.com/Tesla2000/EnhancedWebdriver
 Author: Tesla2000
 Author-email: fratajczak124@gmail.com
 Project-URL: Homepage, https://github.com/Tesla2000/EnhancedWebdriver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enhancedwebdriver-0.1.5/setup.cfg` & `enhancedwebdriver-0.1.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = EnhancedWebdriver
-version = 0.1.5
+version = 0.1.6
 author = Tesla2000
 author_email = fratajczak124@gmail.com
 description = Extension of webdriver with less boilerplate
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Tesla2000/EnhancedWebdriver
 project_urls =
```

### Comparing `enhancedwebdriver-0.1.5/src/EnhancedWebdriver.egg-info/PKG-INFO` & `enhancedwebdriver-0.1.6/src/EnhancedWebdriver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnhancedWebdriver
-Version: 0.1.5
+Version: 0.1.6
 Summary: Extension of webdriver with less boilerplate
 Home-page: https://github.com/Tesla2000/EnhancedWebdriver
 Author: Tesla2000
 Author-email: fratajczak124@gmail.com
 Project-URL: Homepage, https://github.com/Tesla2000/EnhancedWebdriver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enhancedwebdriver-0.1.5/src/enhanced_webdriver/EnhancedWebdriver.py` & `enhancedwebdriver-0.1.6/src/enhanced_webdriver/EnhancedWebdriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             if not undetected:
                 web_driver = webdriver.Chrome(
                     options=options, service=service, keep_alive=keep_alive
                 )
             else:
                 import undetected_chromedriver as uc
 
-                web_driver = uc.Chrome(chrome_options=options, service_args=service)
+                web_driver = uc.Chrome(options=options, service_args=service, keep_alive=keep_alive)
         instance.__dict__ = web_driver.__dict__
         return instance
 
     def __enter__(self):
         """
         Enter the context.
 
@@ -96,15 +96,16 @@
 
         :param value: Locator value of the element.
         :param by: Locator strategy, defaults to By.XPATH.
         :param seconds: Maximum time to wait for the element, defaults to 1.
         :return: The innerText of the element.
 
         """
-        return self._wait(value, seconds, by).text
+        elem = self._wait(value, seconds, by)
+        return elem.text or elem.get_attribute("textContent")
 
     @retry(tries=5, delay=1)
     def is_element_present(
         self, value: str, seconds: float = 1, by: By = By.XPATH
     ) -> bool:
         """
         Check if an element is present in the DOM.
```

