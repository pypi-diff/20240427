# Comparing `tmp/webdriver_browser-0.1.5.tar.gz` & `tmp/webdriver_browser-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webdriver_browser-0.1.5.tar", max compression
+gzip compressed data, was "webdriver_browser-0.1.6.tar", max compression
```

## Comparing `webdriver_browser-0.1.5.tar` & `webdriver_browser-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1089 2024-01-19 15:17:22.905063 webdriver_browser-0.1.5/LICENSE
--rw-r--r--   0        0        0      794 2024-04-23 03:11:54.935918 webdriver_browser-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       86 2024-01-19 15:17:22.905063 webdriver_browser-0.1.5/README.md
--rw-r--r--   0        0        0    15628 2024-04-23 03:08:56.474090 webdriver_browser-0.1.5/webdriver_browser/__init__.py
--rw-r--r--   0        0        0     3962 2024-04-07 14:36:12.703346 webdriver_browser-0.1.5/webdriver_browser/chrome.py
--rw-r--r--   0        0        0     1133 2024-01-19 15:17:22.915062 webdriver_browser-0.1.5/webdriver_browser/edge.py
--rw-r--r--   0        0        0     3086 2024-01-19 15:17:22.915062 webdriver_browser-0.1.5/webdriver_browser/firefox.py
--rw-r--r--   0        0        0     5484 2024-01-19 15:17:22.915062 webdriver_browser-0.1.5/webdriver_browser/patch.py
--rw-r--r--   0        0        0     6191 2024-01-19 15:17:22.917572 webdriver_browser-0.1.5/webdriver_browser/rsync.py
--rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 webdriver_browser-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-01-19 15:17:22.905063 webdriver_browser-0.1.6/LICENSE
+-rw-r--r--   0        0        0      817 2024-04-26 14:33:45.538128 webdriver_browser-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      603 2024-04-26 13:47:48.636884 webdriver_browser-0.1.6/README.md
+-rw-r--r--   0        0        0    15859 2024-04-27 16:06:17.768675 webdriver_browser-0.1.6/webdriver_browser/__init__.py
+-rw-r--r--   0        0        0     4121 2024-04-26 13:38:52.072068 webdriver_browser-0.1.6/webdriver_browser/chrome.py
+-rw-r--r--   0        0        0     1142 2024-04-26 13:35:59.627517 webdriver_browser-0.1.6/webdriver_browser/edge.py
+-rw-r--r--   0        0        0     3095 2024-04-26 13:35:45.583395 webdriver_browser-0.1.6/webdriver_browser/firefox.py
+-rw-r--r--   0        0        0     5484 2024-01-19 15:17:22.915062 webdriver_browser-0.1.6/webdriver_browser/patch.py
+-rw-r--r--   0        0        0     6191 2024-01-19 15:17:22.917572 webdriver_browser-0.1.6/webdriver_browser/rsync.py
+-rw-r--r--   0        0        0     1560 1970-01-01 00:00:00.000000 webdriver_browser-0.1.6/PKG-INFO
```

### Comparing `webdriver_browser-0.1.5/LICENSE` & `webdriver_browser-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `webdriver_browser-0.1.5/pyproject.toml` & `webdriver_browser-0.1.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [tool.poetry]
 name = "webdriver-browser"
-version = "0.1.5"
+version = "0.1.6"
 description = "More convenient methods for creating multiple selenium browsers."
 authors = ["Invoker Bot <invoker-bot@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 urllib3 = "^1.26.18"
 selenium = "^4.16.0"
 selenium-wire = "^5.1.0"
 webdriver-manager = "^4.0.1"
-undetected-chromedriver = "^3.5.4"
+undetected-chromedriver = "^3.5.5"
 pyee = "^11.1.0"
 tenacity = "^8.2.3"
 psutil = "^5.9.8"
+requestium = "^0.4.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 flake8 = "^6.1.0"
 pylint = "^3.0.3"
 mock = "^5.1.0"
 freezegun = "^1.4.0"
```

### Comparing `webdriver_browser-0.1.5/webdriver_browser/__init__.py` & `webdriver_browser-0.1.6/webdriver_browser/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from urllib.parse import urlparse, ParseResult
 from abc import ABC, abstractmethod
 from typing import Callable, Optional, Union, TypeVar
 from dataclasses import dataclass
 from functools import partial
 import psutil
 from pyee import EventEmitter
+import requestium
 from tenacity import Retrying, stop_after_attempt, wait_random_exponential, after_log, before_log, retry_if_exception_type, retry_if_not_result
 from requests.exceptions import RequestException
 from selenium.common.exceptions import WebDriverException
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.support import expected_conditions as EC
@@ -39,14 +40,15 @@
     proxy_server: str = None
     extensions_dirs: list[str] = None
     headless: bool = False
     force_selenium_wire: bool = False
     wait_timeout: float = 15.0
     compressed: bool = False
     singleton: bool = False
+    undetected_chrome_driver: bool = None
 
 
 class RemoteBrowser(ABC):  # pylint: disable=too-many-public-methods
     """Remote browser"""
 
     def __init__(self, options: BrowserOptions = None, driver_manager: DriverManager = None):
         if options is None:
@@ -58,37 +60,42 @@
             driver_manager = self.default_driver_manager()
         if options.data_dir is not None:  # pylint: disable=too-many-nested-blocks
             self.make_root_data_dir()
             if options.compressed:
                 if not os.path.isdir(self.get_data_dir('default')):
                     default_options = BrowserOptions(data_dir='default', headless=True, compressed=False)
                     default_driver = self.new_driver(default_options, self.driver_options(
-                        default_options), self.driver_service(driver_manager))
+                        default_options), self.driver_service(options, driver_manager))
                     default_driver.quit()
                 if not os.path.isdir(self.get_data_dir('default')):
                     options.compressed = False
                     logger.warning("Reference dir '%s' not created, using uncompressed data dir", options.data_dir)
                 else:
                     compressed_file = self.get_data_dir(options.data_dir + ".patch")
                     if not os.path.exists(self.data_dir):
                         if os.path.exists(compressed_file):
                             try:
                                 unpack_dir_with_ref(self.get_data_dir('default'), compressed_file, self.data_dir)
                             except ValueError:
                                 logger.warning("Reference dir '%s' changed, using uncompressed data",
                                                self.get_data_dir('default'))
-        self.driver = self.new_driver(options, self.driver_options(options), self.driver_service(driver_manager))
+        self.driver = self.new_driver(options, self.driver_options(options), self.driver_service(options, driver_manager))
         self.config_driver()
+        self.session = requestium.Session(driver=self.driver)
         self.wait = WebDriverWait(self.driver, options.wait_timeout)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        self.driver.__exit__(exc_type, exc_val, exc_tb)
+        # self.driver.__exit__(exc_type, exc_val, exc_tb)
+        self.quit()
+
+    def __del__(self):
+        pass
 
     def is_locked(self):
         """Check if the browser is locked"""
         data_dir = self.data_dir
         if data_dir is not None:
             for filename in ('lockfile', 'SingletonCookie', 'SingletonLock', 'parent.lock'):
                 if os.path.exists(os.path.join(data_dir, filename)):
@@ -116,15 +123,15 @@
     @classmethod
     @abstractmethod
     def driver_options(cls, options: BrowserOptions) -> DriverOptions:
         """Driver options"""
 
     @classmethod
     @abstractmethod
-    def driver_service(cls, driver_manager) -> DriverService:
+    def driver_service(cls, options: BrowserOptions, driver_manager) -> DriverService:
         """Driver service"""
 
     @classmethod
     @abstractmethod
     def new_driver(cls, options: BrowserOptions, driver_options: DriverOptions, service: DriverService) -> WebDriver:
         """Default driver"""
```

### Comparing `webdriver_browser-0.1.5/webdriver_browser/chrome.py` & `webdriver_browser-0.1.6/webdriver_browser/chrome.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,30 +45,32 @@
     @classmethod
     def driver_options(cls, options):
         """Driver options"""
         driver_options = webdriver.ChromeOptions()
         return cls.config_driver_options(options, driver_options)
 
     @classmethod
-    def driver_service(cls, driver_manager):
+    def driver_service(cls, options, driver_manager):
         """Driver service"""
-        return None if cls.use_undetected_driver() else webdriver.ChromeService(driver_manager.install())
+        return None if cls.use_undetected_driver(options) else webdriver.ChromeService(driver_manager.install())
 
     @classmethod
-    def use_undetected_driver(cls):
+    def use_undetected_driver(cls, options: BrowserOptions):
         """Undetected driver"""
+        if options.undetected_chrome_driver is not None:
+            return options.undetected_chrome_driver
         return os.getenv('UNDETECTED_CHROME_DRIVER', 'true').lower() not in ('false', '0', 'off', 'no', '')
 
     @classmethod
     def new_driver(cls, options, driver_options, service):
         """Default driver
         set UNDETECTED_CHROME_DRIVER=false will not use undetected_chromedriver
         """
         user_data_dir = None
-        if cls.use_undetected_driver():
+        if cls.use_undetected_driver(options):
             if options.data_dir is None:  # should set tmp
                 options.data_dir = user_data_dir = cls.get_data_dir('.tmp')
                 shutil.rmtree(user_data_dir, ignore_errors=True)
             if cls.use_seleniumwire(options):
                 return wire_uc.Chrome(options=driver_options, user_data_dir=user_data_dir,
                                       seleniumwire_options=cls.default_seleniumwire_config(options))
             return uc.Chrome(options=driver_options, user_data_dir=user_data_dir)
```

### Comparing `webdriver_browser-0.1.5/webdriver_browser/edge.py` & `webdriver_browser-0.1.6/webdriver_browser/edge.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     @classmethod
     def driver_options(cls, options):
         driver_options = webdriver.EdgeOptions()
         return cls.config_driver_options(options, driver_options)
 
     @classmethod
-    def driver_service(cls, driver_manager):
+    def driver_service(cls, options, driver_manager):
         """Driver service"""
         return webdriver.EdgeService(driver_manager.install())
 
     @classmethod
     def default_driver_manager(cls):
         """Default driver manager"""
         return EdgeChromiumDriverManager()
```

### Comparing `webdriver_browser-0.1.5/webdriver_browser/firefox.py` & `webdriver_browser-0.1.6/webdriver_browser/firefox.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             else:
                 raise ValueError(f"unsupported proxy server scheme: '{result.scheme}'")
             driver_options.set_preference("network.proxy.type", 1)
             driver_options.set_preference("network.proxy.no_proxies_on", "localhost, 127.0.0.1")
         return driver_options
 
     @classmethod
-    def driver_service(cls, driver_manager):
+    def driver_service(cls, options, driver_manager):
         """Driver service"""
         return webdriver.FirefoxService(driver_manager.install())
 
     @classmethod
     def new_driver(cls, options, driver_options, service):
         """Default driver"""
         if cls.use_seleniumwire(options):
```

### Comparing `webdriver_browser-0.1.5/webdriver_browser/patch.py` & `webdriver_browser-0.1.6/webdriver_browser/patch.py`

 * *Files identical despite different names*

### Comparing `webdriver_browser-0.1.5/webdriver_browser/rsync.py` & `webdriver_browser-0.1.6/webdriver_browser/rsync.py`

 * *Files identical despite different names*

