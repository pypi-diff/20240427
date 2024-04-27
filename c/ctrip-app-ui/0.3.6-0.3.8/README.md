# Comparing `tmp/ctrip-app-ui-0.3.6.tar.gz` & `tmp/ctrip-app-ui-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.3.6.tar", last modified: Sat Apr 27 09:56:02 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.3.8.tar", last modified: Sat Apr 27 10:16:28 2024, max compression
```

## Comparing `ctrip-app-ui-0.3.6.tar` & `ctrip-app-ui-0.3.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 09:56:02.010776 ctrip-app-ui-0.3.6/
--rw-rw-rw-   0        0        0    11558 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/LICENSE
--rw-rw-rw-   0        0        0      474 2024-04-27 09:56:02.010045 ctrip-app-ui-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 09:56:02.007358 ctrip-app-ui-0.3.6/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/capp_ui/__init__.py
--rw-rw-rw-   0        0        0     3628 2024-04-27 02:13:31.000000 ctrip-app-ui-0.3.6/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1191 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/capp_ui/dir.py
--rw-rw-rw-   0        0        0    59905 2024-04-27 09:55:14.000000 ctrip-app-ui-0.3.6/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/capp_ui/fee.py
--rw-rw-rw-   0        0        0     2270 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/capp_ui/libs.py
--rw-rw-rw-   0        0        0    23814 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1799 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      689 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/capp_ui/test.py
--rw-rw-rw-   0        0        0     5563 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3016 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-04-27 09:56:02.009548 ctrip-app-ui-0.3.6/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-04-27 09:56:01.000000 ctrip-app-ui-0.3.6/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2024-04-27 09:56:01.000000 ctrip-app-ui-0.3.6/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 09:56:01.000000 ctrip-app-ui-0.3.6/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-27 09:56:01.000000 ctrip-app-ui-0.3.6/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-27 09:56:01.000000 ctrip-app-ui-0.3.6/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 09:56:02.010776 ctrip-app-ui-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-04-27 09:56:00.000000 ctrip-app-ui-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:16:28.734110 ctrip-app-ui-0.3.8/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.8/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-04-27 10:16:28.733614 ctrip-app-ui-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 10:16:28.731130 ctrip-app-ui-0.3.8/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.8/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0     3628 2024-04-27 02:13:31.000000 ctrip-app-ui-0.3.8/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1191 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.8/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.8/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    59905 2024-04-27 10:15:52.000000 ctrip-app-ui-0.3.8/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.8/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     2270 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.8/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    23814 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.8/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1799 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.8/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      689 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.8/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5563 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.8/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3016 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.8/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:16:28.733614 ctrip-app-ui-0.3.8/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-04-27 10:16:28.000000 ctrip-app-ui-0.3.8/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2024-04-27 10:16:28.000000 ctrip-app-ui-0.3.8/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 10:16:28.000000 ctrip-app-ui-0.3.8/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-27 10:16:28.000000 ctrip-app-ui-0.3.8/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-27 10:16:28.000000 ctrip-app-ui-0.3.8/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 10:16:28.734110 ctrip-app-ui-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-04-27 10:16:25.000000 ctrip-app-ui-0.3.8/setup.py
```

### Comparing `ctrip-app-ui-0.3.6/LICENSE` & `ctrip-app-ui-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.6/capp_ui/date_extend.py` & `ctrip-app-ui-0.3.8/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.6/capp_ui/device.py` & `ctrip-app-ui-0.3.8/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.6/capp_ui/dir.py` & `ctrip-app-ui-0.3.8/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.6/capp_ui/domain_service.py` & `ctrip-app-ui-0.3.8/capp_ui/domain_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1346,15 +1346,15 @@
             payment_amount = payment_amount.get_text()
             logger.info("从支付成功界面获取到的实际支付金额是: {}".format(payment_amount))
             payment_amount = Decimal(payment_amount) if isinstance(payment_amount, str) else payment_amount
         except Exception as e:
             logger.error(str(e))
         return payment_amount
 
-    @SleepWait(wait_time=5)
+    @SleepWait(wait_time=3)
     def touch_payment_complete(self) -> None:
         """在支付成功界面，点击【完成】"""
         try:
             payment_complete_button = self.device.get_po_extend(
                 type="android.widget.TextView",
                 name="android.widget.TextView",
                 text="完成",
```

### Comparing `ctrip-app-ui-0.3.6/capp_ui/fee.py` & `ctrip-app-ui-0.3.8/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.6/capp_ui/libs.py` & `ctrip-app-ui-0.3.8/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.6/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.3.8/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.6/capp_ui/platforms.py` & `ctrip-app-ui-0.3.8/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.6/capp_ui/test.py` & `ctrip-app-ui-0.3.8/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.6/capp_ui/utils.py` & `ctrip-app-ui-0.3.8/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.6/capp_ui/validators.py` & `ctrip-app-ui-0.3.8/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.6/setup.py` & `ctrip-app-ui-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.3.6',
+    version='0.3.8',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

