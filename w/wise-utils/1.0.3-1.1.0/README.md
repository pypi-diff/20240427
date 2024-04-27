# Comparing `tmp/wise-utils-1.0.3.tar.gz` & `tmp/wise_utils-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wise-utils-1.0.3.tar", last modified: Fri Sep 15 07:02:28 2023, max compression
+gzip compressed data, was "wise_utils-1.1.0.tar", last modified: Sat Apr 27 06:23:36 2024, max compression
```

## Comparing `wise-utils-1.0.3.tar` & `wise_utils-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-09-15 07:02:28.466137 wise-utils-1.0.3/
--rw-rw-rw-   0        0        0     1091 2022-08-01 11:04:29.000000 wise-utils-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       44 2022-08-01 11:04:29.000000 wise-utils-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1756 2023-09-15 07:02:28.465136 wise-utils-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      857 2022-08-24 03:51:54.000000 wise-utils-1.0.3/README.md
--rw-rw-rw-   0        0        0      108 2022-08-01 11:04:29.000000 wise-utils-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-09-15 07:02:28.473136 wise-utils-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1256 2023-09-15 06:47:57.000000 wise-utils-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-15 07:02:28.405120 wise-utils-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-09-15 07:02:28.420509 wise-utils-1.0.3/src/wise_utils/
--rw-rw-rw-   0        0        0       58 2022-08-01 11:04:29.000000 wise-utils-1.0.3/src/wise_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-15 07:02:28.450134 wise-utils-1.0.3/src/wise_utils/common/
--rw-rw-rw-   0        0        0      412 2023-09-15 06:46:49.000000 wise-utils-1.0.3/src/wise_utils/common/__init__.py
--rw-rw-rw-   0        0        0      119 2022-08-01 11:04:29.000000 wise-utils-1.0.3/src/wise_utils/common/exceptions.py
--rw-rw-rw-   0        0        0     4476 2022-08-01 11:04:29.000000 wise-utils-1.0.3/src/wise_utils/common/ftp.py
--rw-rw-rw-   0        0        0     7684 2022-08-01 11:04:29.000000 wise-utils-1.0.3/src/wise_utils/common/log.py
--rw-rw-rw-   0        0        0      411 2022-08-01 11:04:29.000000 wise-utils-1.0.3/src/wise_utils/common/mail.py
--rw-rw-rw-   0        0        0     2425 2022-09-05 09:02:51.000000 wise-utils-1.0.3/src/wise_utils/common/retry_decorator.py
-drwxrwxrwx   0        0        0        0 2023-09-15 07:02:28.456132 wise-utils-1.0.3/src/wise_utils/db/
--rw-rw-rw-   0        0        0      185 2022-08-01 11:04:29.000000 wise-utils-1.0.3/src/wise_utils/db/__init__.py
--rw-rw-rw-   0        0        0    12291 2022-08-01 11:04:29.000000 wise-utils-1.0.3/src/wise_utils/db/db_mysql.py
--rw-rw-rw-   0        0        0      238 2022-08-01 11:04:29.000000 wise-utils-1.0.3/src/wise_utils/db/db_redis.py
-drwxrwxrwx   0        0        0        0 2023-09-15 07:02:28.463136 wise-utils-1.0.3/src/wise_utils/spider/
--rw-rw-rw-   0        0        0      194 2022-08-01 11:04:29.000000 wise-utils-1.0.3/src/wise_utils/spider/__init__.py
--rw-rw-rw-   0        0        0      473 2022-08-01 11:04:29.000000 wise-utils-1.0.3/src/wise_utils/spider/basespider.py
--rw-rw-rw-   0        0        0    25503 2022-08-24 03:51:54.000000 wise-utils-1.0.3/src/wise_utils/spider/selenium_spider.py
--rw-rw-rw-   0        0        0   162046 2022-08-01 11:04:29.000000 wise-utils-1.0.3/src/wise_utils/spider/stealth.js
-drwxrwxrwx   0        0        0        0 2023-09-15 07:02:28.438477 wise-utils-1.0.3/src/wise_utils.egg-info/
--rw-rw-rw-   0        0        0     1756 2023-09-15 07:02:28.000000 wise-utils-1.0.3/src/wise_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      712 2023-09-15 07:02:28.000000 wise-utils-1.0.3/src/wise_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-15 07:02:28.000000 wise-utils-1.0.3/src/wise_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      229 2023-09-15 07:02:28.000000 wise-utils-1.0.3/src/wise_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-09-15 07:02:28.000000 wise-utils-1.0.3/src/wise_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 06:23:36.175974 wise_utils-1.1.0/
+-rw-rw-rw-   0        0        0     1091 2022-09-17 11:47:05.000000 wise_utils-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       44 2022-09-17 11:47:05.000000 wise_utils-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1678 2024-04-27 06:23:36.174397 wise_utils-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      857 2022-09-17 11:47:05.000000 wise_utils-1.1.0/README.md
+-rw-rw-rw-   0        0        0      108 2022-09-17 11:47:05.000000 wise_utils-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-27 06:23:36.175974 wise_utils-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1186 2024-04-27 06:22:24.000000 wise_utils-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 06:23:36.100612 wise_utils-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-27 06:23:36.116827 wise_utils-1.1.0/src/wise_utils/
+-rw-rw-rw-   0        0        0       58 2023-08-01 06:36:46.000000 wise_utils-1.1.0/src/wise_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 06:23:36.144280 wise_utils-1.1.0/src/wise_utils/common/
+-rw-rw-rw-   0        0        0      478 2022-10-08 02:17:40.000000 wise_utils-1.1.0/src/wise_utils/common/__init__.py
+-rw-rw-rw-   0        0        0      119 2022-10-08 02:17:40.000000 wise_utils-1.1.0/src/wise_utils/common/exceptions.py
+-rw-rw-rw-   0        0        0     4488 2024-04-27 06:14:49.000000 wise_utils-1.1.0/src/wise_utils/common/ftp.py
+-rw-rw-rw-   0        0        0     7684 2022-10-08 02:17:40.000000 wise_utils-1.1.0/src/wise_utils/common/log.py
+-rw-rw-rw-   0        0        0     2425 2022-10-08 02:17:40.000000 wise_utils-1.1.0/src/wise_utils/common/retry_decorator.py
+drwxrwxrwx   0        0        0        0 2024-04-27 06:23:36.153273 wise_utils-1.1.0/src/wise_utils/db/
+-rw-rw-rw-   0        0        0      185 2022-10-08 02:17:40.000000 wise_utils-1.1.0/src/wise_utils/db/__init__.py
+-rw-rw-rw-   0        0        0    12291 2022-10-08 02:17:40.000000 wise_utils-1.1.0/src/wise_utils/db/db_mysql.py
+-rw-rw-rw-   0        0        0      238 2022-10-08 02:17:40.000000 wise_utils-1.1.0/src/wise_utils/db/db_redis.py
+drwxrwxrwx   0        0        0        0 2024-04-27 06:23:36.171478 wise_utils-1.1.0/src/wise_utils/spider/
+-rw-rw-rw-   0        0        0      194 2022-10-08 02:17:40.000000 wise_utils-1.1.0/src/wise_utils/spider/__init__.py
+-rw-rw-rw-   0        0        0      475 2024-02-28 09:03:38.000000 wise_utils-1.1.0/src/wise_utils/spider/basespider.py
+-rw-rw-rw-   0        0        0        2 2024-02-28 08:59:12.000000 wise_utils-1.1.0/src/wise_utils/spider/demo.py
+-rw-rw-rw-   0        0        0    11814 2024-02-28 13:02:43.000000 wise_utils-1.1.0/src/wise_utils/spider/selenium_base_spider.py
+-rw-rw-rw-   0        0        0    24625 2024-04-27 06:19:50.000000 wise_utils-1.1.0/src/wise_utils/spider/selenium_spider.py
+-rw-rw-rw-   0        0        0   162046 2022-10-08 02:17:40.000000 wise_utils-1.1.0/src/wise_utils/spider/stealth.js
+drwxrwxrwx   0        0        0        0 2024-04-27 06:23:36.173424 wise_utils-1.1.0/src/wise_utils.egg-info/
+-rw-rw-rw-   0        0        0     1678 2024-04-27 06:23:35.000000 wise_utils-1.1.0/src/wise_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      748 2024-04-27 06:23:36.000000 wise_utils-1.1.0/src/wise_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 06:23:35.000000 wise_utils-1.1.0/src/wise_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      180 2024-04-27 06:23:35.000000 wise_utils-1.1.0/src/wise_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-27 06:23:35.000000 wise_utils-1.1.0/src/wise_utils.egg-info/top_level.txt
```

### Comparing `wise-utils-1.0.3/LICENSE` & `wise_utils-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wise-utils-1.0.3/PKG-INFO` & `wise_utils-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: wise-utils
-Version: 1.0.3
-Home-page: https://gitee.com/duquan1995/wise-utils.git
+Version: 1.1.0
+Home-page: http://code.wise-inc.com/spider/wise-utils.git
 Author: wise-python
 Author-email: duke.du@uifox.com.cn
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: yagmail>=0.15.277
 Requires-Dist: requests>=2.25.1
 Requires-Dist: urllib3>=1.26.7
 Requires-Dist: selenium>=4.1.0
 Requires-Dist: redis
 Requires-Dist: PyMySQL>=1.0.2
 Requires-Dist: nacos-sdk-python>=0.1.6
 Requires-Dist: better-exceptions>=0.3.3
 Requires-Dist: loguru>=0.6.0
 Requires-Dist: PyVirtualDisplay>=2.2
-Requires-Dist: undetected_chromedriver~=3.1.5
 Requires-Dist: webdriver_manager~=3.5.4
 
 # 小工具
 
 - common
     - exceptions: 异常处理
     - ftp: FTP上传下载
```

### Comparing `wise-utils-1.0.3/README.md` & `wise_utils-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `wise-utils-1.0.3/setup.py` & `wise_utils-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-VERSION = "1.0.3"
+VERSION = "1.1.0"
 
 setuptools.setup(
     name="wise-utils",
     version=VERSION,
     author="wise-python",
     author_email="duke.du@uifox.com.cn",
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://gitee.com/duquan1995/wise-utils.git",
+    url="http://code.wise-inc.com/spider/wise-utils.git",
     project_urls={
         "Bug Tracker": "https://github.com/pypa/sampleproject/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     include_package_data=True,
     python_requires=">3",
     install_requires=[
-        "yagmail>=0.15.277",
         "requests>=2.25.1",
         "urllib3>=1.26.7",
         "selenium>=4.1.0",
         "redis",
         "PyMySQL>=1.0.2",
         "nacos-sdk-python>=0.1.6",
         "better-exceptions>=0.3.3",
         "loguru>=0.6.0",
         "PyVirtualDisplay>=2.2",
-        "undetected_chromedriver~=3.1.5",
         "webdriver_manager~=3.5.4"
     ]
 )
```

### Comparing `wise-utils-1.0.3/src/wise_utils/common/ftp.py` & `wise_utils-1.1.0/src/wise_utils/common/ftp.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.password = password  # 登陆密码
         self.ftp = self.ftp_connect()
 
     def ftp_connect(self):
         """ftp连接"""
         ftp = ftplib.FTP()
         try:
-            ftp.connect(self.ftp_server, self.port)
+            ftp.connect(self.ftp_server, self.port, timeout=20)
             ftp.login(self.username, self.password)
         except:
             raise IOError('FTP login failed!!!')
         else:
             print(ftp.getwelcome())
             return ftp
```

### Comparing `wise-utils-1.0.3/src/wise_utils/common/log.py` & `wise_utils-1.1.0/src/wise_utils/common/log.py`

 * *Files identical despite different names*

### Comparing `wise-utils-1.0.3/src/wise_utils/common/retry_decorator.py` & `wise_utils-1.1.0/src/wise_utils/common/retry_decorator.py`

 * *Files identical despite different names*

### Comparing `wise-utils-1.0.3/src/wise_utils/db/db_mysql.py` & `wise_utils-1.1.0/src/wise_utils/db/db_mysql.py`

 * *Files identical despite different names*

### Comparing `wise-utils-1.0.3/src/wise_utils/spider/selenium_spider.py` & `wise_utils-1.1.0/src/wise_utils/spider/selenium_spider.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 import os
 import sys
 import time
 import string
 import zipfile
 import logging
-import undetected_chromedriver as uc
 
 from selenium import webdriver
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.select import Select
 from selenium.webdriver.support.wait import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
@@ -60,27 +59,36 @@
                              no_pop_ups: bool = False,
                              page_load_strategy: str = "none",
                              no_extensions: bool = False,
                              use_proxy: bool = False,
                              userdata_file_path: str = "",
                              executable_path: str = "",
                              chrome_options: webdriver.ChromeOptions = None,
-                             execute_cdp_cmd: bool = False
+                             execute_cdp_cmd: bool = False,
+                             browser = None
                              ):
         """
         创建本地浏览器
         :params headless: 无头模式
         :params incognito: 无痕模式
         :params no_picture: 禁止加载图片元素
         :params no_pop_ups: 禁止弹窗
         :params page_load_strategy: 页面加载策略 可设置为三种  1 eager selenium会等待整个界面加载完成（指对html和子资源的下载与解析，不包括ajax）  2 normal 要等待整个dom树加载完成，即DOMContentLoaded这个事件完成，仅对html的内容进行下载解析 3 none 当html下载完成之后，不等待解析完成，selenium会直接返回
         :params no_extensions: 禁止使用插件
         :params use_proxy: 使用代理
         :params userdata_file_path: 保存历史和缓存（多爬虫同时使用不行）
         """
+
+        if browser:
+            try:
+                print(browser.title)
+                return browser
+            except:
+                pass
+
         self.__browser_model = "local"
         if sys.platform == "linux":
             # 打开虚拟窗口
             from pyvirtualdisplay import Display
             self.__display = Display(visible=False, size=(1792, 1120))
             self.__display.start()
 
@@ -158,46 +166,61 @@
             "se:screenResolution": "1920x1080"
         }
         browser = webdriver.Remote(command_executor=remote_url, desired_capabilities=desired_capabilities, options=chrome_options)
         browser.set_page_load_timeout(self.PAGE_LOAD_TIMEOUT)
         browser.maximize_window()
         return browser
 
-    def create_undetected_browser(self,
-                                  chrome_version,
-                                  headless: bool = True,
-                                  incognito: bool = True,
-                                  no_pop_ups: bool = False,
-                                  page_load_strategy: str = "none",
-                                  no_extensions: bool = False,
-                                  userdata_file_path: str = "",
-                                  chrome_options: uc.ChromeOptions = None,
-
-                                  ):
-        """通过undetected_chromedriver创建chrome，需要指定浏览器版本。可过五秒盾"""
-        self.__browser_model = "undetected"
-
-        if sys.platform == "linux":
-            # 打开虚拟窗口
-            from pyvirtualdisplay import Display
-            self.__display = Display(visible=False, size=(1792, 1120))
-            self.__display.start()
+    def create_remote_browser_for_specific_chrome_node(self, remote_url,
+                              node_name,
+                              desired_capabilities: dict = {},
+                              headless: bool = True,
+                              incognito: bool = True,
+                              no_picture: bool = False,
+                              no_pop_ups: bool = False,
+                              page_load_strategy: str = "none",
+                              no_extensions: bool = False,
+                              use_proxy: bool = False,
+                              userdata_file_path: str = "",
+                              chrome_options: webdriver.ChromeOptions = None,
+                              ):
+        """
+        创建远程浏览器: selenium grid
+        :params headless: 无头模式
+        :params incognito: 无痕模式
+        :params no_picture: 禁止加载图片元素
+        :params no_pop_ups: 禁止弹窗
+        :params page_load_strategy: 页面加载策略 可设置为三种  1 eager selenium会等待整个界面加载完成（指对html和子资源的下载与解析，不包括ajax）  2 normal 要等待整个dom树加载完成，即DOMContentLoaded这个事件完成，仅对html的内容进行下载解析 3 none 当html下载完成之后，不等待解析完成，selenium会直接返回
+        :params no_extensions: 禁止使用插件
+        :params use_proxy: 使用代理
+        :params userdata_file_path: 保存历史和缓存（多爬虫同时使用不行）
+        """
 
-        from multiprocessing import freeze_support
-        freeze_support()
+        self.__browser_model = "remote"
 
-        chrome_options = chrome_options if chrome_options else self.get_undetected_chrome_options(
+        chrome_options= self.get_chrome_options(
             headless=headless,
             incognito=incognito,
+            no_picture=no_picture,
             no_pop_ups=no_pop_ups,
             page_load_strategy=page_load_strategy,
             no_extensions=no_extensions,
-            userdata_file_path=userdata_file_path
+            use_proxy=use_proxy,
+            userdata_file_path=userdata_file_path,
         )
-        browser = uc.Chrome(options=chrome_options, version_main=chrome_version)
+
+
+
+        chrome_options.set_capability("nodename:applicationName",node_name)
+        chrome_options.set_capability("platformName", "LINUX")
+        chrome_options.set_capability("browserName", "chrome")
+        chrome_options.set_capability("browserVersion","105.0.5195.52")
+
+        browser = webdriver.Remote(command_executor=remote_url,
+                                   options=chrome_options)
 
         browser.set_page_load_timeout(self.PAGE_LOAD_TIMEOUT)
         browser.maximize_window()
         return browser
 
     @staticmethod
     def reconnect_existed_browser(executor_url, session_id):
@@ -272,62 +295,14 @@
 
         if incognito:
             # 无痕
             chrome_options.add_argument("--incognito")
 
         if headless:
             # 无头
-            chrome_options.add_argument("--headless")
-
-        if userdata_file_path:
-            chrome_options.add_argument(f"--user-data-dir={userdata_file_path}")
-        return chrome_options
-
-    @staticmethod
-    def get_undetected_chrome_options(
-            headless: bool = True,
-            incognito: bool = True,
-            no_pop_ups: bool = False,
-            page_load_strategy: str = "none",
-            no_extensions: bool = False,
-            userdata_file_path: str = "",
-    ):
-        """获取undetected_chrome_options"""
-        chrome_options = uc.ChromeOptions()
-        chrome_options.add_argument("--disable-gpu")  # 谷歌文档提到需要加上这个属性来规避bug
-        chrome_options.add_argument("--hide-scrollbars")  # 隐藏滚动条, 应对一些特殊页面
-        chrome_options.add_argument("--disable-infobars")  # 关闭提示
-        chrome_options.add_argument("--disable-dev-shm-usage")  # 修复选项卡崩溃
-        chrome_options.add_argument("--ignore-certificate-errors")  # 忽略验证：您的连接不是私密连接
-
-        if no_extensions:
-            chrome_options.add_argument("--disable-extensions")
-            chrome_options.add_experimental_option("useAutomationExtension", False)
-
-        if no_pop_ups:
-            # 禁止弹窗加入
-            prefs = {
-                "profile.default_content_setting_values":
-                    {
-                        "notifications": 2
-                    }
-            }
-        else:
-            prefs = dict()
-        prefs["credentials_enable_service"] = False
-        prefs["profile.password_manager_enabled"] = False
-        chrome_options.add_experimental_option("prefs", prefs)
-        chrome_options.set_capability("PageloadStrategy", page_load_strategy)
-
-        if incognito:
-            # 无痕
-            chrome_options.add_argument("--incognito")
-
-        if headless:
-            # 无头
             chrome_options.add_argument("--headless")
 
         if userdata_file_path:
             chrome_options.add_argument(f"--user-data-dir={userdata_file_path}")
         return chrome_options
 
     def clear_and_send_keys(self, browser, by: str, value: str, msg):
```

### Comparing `wise-utils-1.0.3/src/wise_utils/spider/stealth.js` & `wise_utils-1.1.0/src/wise_utils/spider/stealth.js`

 * *Files identical despite different names*

### Comparing `wise-utils-1.0.3/src/wise_utils.egg-info/PKG-INFO` & `wise_utils-1.1.0/src/wise_utils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: wise-utils
-Version: 1.0.3
-Home-page: https://gitee.com/duquan1995/wise-utils.git
+Version: 1.1.0
+Home-page: http://code.wise-inc.com/spider/wise-utils.git
 Author: wise-python
 Author-email: duke.du@uifox.com.cn
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: yagmail>=0.15.277
 Requires-Dist: requests>=2.25.1
 Requires-Dist: urllib3>=1.26.7
 Requires-Dist: selenium>=4.1.0
 Requires-Dist: redis
 Requires-Dist: PyMySQL>=1.0.2
 Requires-Dist: nacos-sdk-python>=0.1.6
 Requires-Dist: better-exceptions>=0.3.3
 Requires-Dist: loguru>=0.6.0
 Requires-Dist: PyVirtualDisplay>=2.2
-Requires-Dist: undetected_chromedriver~=3.1.5
 Requires-Dist: webdriver_manager~=3.5.4
 
 # 小工具
 
 - common
     - exceptions: 异常处理
     - ftp: FTP上传下载
```

### Comparing `wise-utils-1.0.3/src/wise_utils.egg-info/SOURCES.txt` & `wise_utils-1.1.0/src/wise_utils.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
 setup.py
 src/wise_utils/__init__.py
 src/wise_utils.egg-info/PKG-INFO
 src/wise_utils.egg-info/SOURCES.txt
 src/wise_utils.egg-info/dependency_links.txt
 src/wise_utils.egg-info/requires.txt
 src/wise_utils.egg-info/top_level.txt
 src/wise_utils/common/__init__.py
 src/wise_utils/common/exceptions.py
 src/wise_utils/common/ftp.py
 src/wise_utils/common/log.py
-src/wise_utils/common/mail.py
 src/wise_utils/common/retry_decorator.py
 src/wise_utils/db/__init__.py
 src/wise_utils/db/db_mysql.py
 src/wise_utils/db/db_redis.py
 src/wise_utils/spider/__init__.py
 src/wise_utils/spider/basespider.py
+src/wise_utils/spider/demo.py
+src/wise_utils/spider/selenium_base_spider.py
 src/wise_utils/spider/selenium_spider.py
 src/wise_utils/spider/stealth.js
```

