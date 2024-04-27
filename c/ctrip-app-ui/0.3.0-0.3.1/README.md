# Comparing `tmp/ctrip-app-ui-0.3.0.tar.gz` & `tmp/ctrip-app-ui-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.3.0.tar", last modified: Sat Apr 27 08:15:19 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.3.1.tar", last modified: Sat Apr 27 08:28:47 2024, max compression
```

## Comparing `ctrip-app-ui-0.3.0.tar` & `ctrip-app-ui-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 08:15:19.806386 ctrip-app-ui-0.3.0/
--rw-rw-rw-   0        0        0    11558 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/LICENSE
--rw-rw-rw-   0        0        0      474 2024-04-27 08:15:19.805890 ctrip-app-ui-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 08:15:19.803327 ctrip-app-ui-0.3.0/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/capp_ui/__init__.py
--rw-rw-rw-   0        0        0     3628 2024-04-27 02:13:31.000000 ctrip-app-ui-0.3.0/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1191 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/capp_ui/dir.py
--rw-rw-rw-   0        0        0    59708 2024-04-27 08:15:00.000000 ctrip-app-ui-0.3.0/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/capp_ui/fee.py
--rw-rw-rw-   0        0        0     2270 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/capp_ui/libs.py
--rw-rw-rw-   0        0        0    23814 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1799 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      689 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/capp_ui/test.py
--rw-rw-rw-   0        0        0     5563 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3016 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-04-27 08:15:19.805391 ctrip-app-ui-0.3.0/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-04-27 08:15:19.000000 ctrip-app-ui-0.3.0/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2024-04-27 08:15:19.000000 ctrip-app-ui-0.3.0/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 08:15:19.000000 ctrip-app-ui-0.3.0/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-27 08:15:19.000000 ctrip-app-ui-0.3.0/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-27 08:15:19.000000 ctrip-app-ui-0.3.0/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 08:15:19.806386 ctrip-app-ui-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-04-27 08:15:10.000000 ctrip-app-ui-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 08:28:47.400774 ctrip-app-ui-0.3.1/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-04-27 08:28:47.400774 ctrip-app-ui-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 08:28:47.398210 ctrip-app-ui-0.3.1/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.1/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0     3628 2024-04-27 02:13:31.000000 ctrip-app-ui-0.3.1/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1191 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.1/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.1/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    59704 2024-04-27 08:28:27.000000 ctrip-app-ui-0.3.1/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.1/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     2270 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.1/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    23814 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.1/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1799 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.1/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      689 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.1/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5563 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.1/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3016 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.1/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-04-27 08:28:47.400276 ctrip-app-ui-0.3.1/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-04-27 08:28:47.000000 ctrip-app-ui-0.3.1/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2024-04-27 08:28:47.000000 ctrip-app-ui-0.3.1/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 08:28:47.000000 ctrip-app-ui-0.3.1/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-27 08:28:47.000000 ctrip-app-ui-0.3.1/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-27 08:28:47.000000 ctrip-app-ui-0.3.1/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 08:28:47.401270 ctrip-app-ui-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-04-27 08:28:41.000000 ctrip-app-ui-0.3.1/setup.py
```

### Comparing `ctrip-app-ui-0.3.0/LICENSE` & `ctrip-app-ui-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.0/capp_ui/date_extend.py` & `ctrip-app-ui-0.3.1/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.0/capp_ui/device.py` & `ctrip-app-ui-0.3.1/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.0/capp_ui/dir.py` & `ctrip-app-ui-0.3.1/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.0/capp_ui/domain_service.py` & `ctrip-app-ui-0.3.1/capp_ui/domain_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
                 type="android.widget.TextView", name="ctrip.android.view:id/a", text="确定"
             )
             if logout_user.exists() is True:
                 logout_user.click()
         except (PocoNoSuchNodeException,):
             pass
 
-    @SleepWait(wait_time=2)
+    @SleepWait(wait_time=1)
     def touch_unpaid(self) -> None:
         """进入my主页后，点击【待付款】"""
         try:
             # 登录后的待付款元素定位
             login_unpaid_button = self.device.poco(
                 type="android.widget.TextView", name="ctrip.android.view:id/a", text="待付款"
             )
@@ -1266,30 +1266,30 @@
             touchable=False,
         )[0]
         deduction_amount = tickect_deduction_amount.get_text()
         deduction_amount = Decimal(deduction_amount[2:]) if isinstance(deduction_amount,
                                                                        str) else -9999999999.9999999999
         return deduction_amount
 
-    @SleepWait(wait_time=10)
+    @SleepWait(wait_time=5)
     def enter_payment_pass(self, payment_pass: str) -> None:
         """
         请输入支付密码
         """
         device = PlatformService.minicap_device()
         payment_pass = payment_pass if isinstance(payment_pass, str) else str(payment_pass)
         for char in payment_pass:
             file_name = join_path([get_images_dir(), "支付_{}.png".format(char)])
             if is_exists(file_name):
                 temp = device.get_cv_template(file_name=file_name)
                 device.touch(v=temp)
             else:
                 raise ValueError("文件<{}>缺失...", format(file_name))
 
-    @SleepWait(wait_time=10)
+    @SleepWait(wait_time=1)
     def is_balance(self, payment_card: str) -> bool:
         """
         判断是否出现余额不足的小弹框
         """
         flag = False
         try:
             balance_poco = self.device.get_po(
@@ -1301,15 +1301,15 @@
                 logger.warning("银行卡【{}】余额不足，请更换其他银行卡或使用其他支付方式.".format(payment_card))
                 balance_poco.click()
                 flag = True
         except (PocoNoSuchNodeException, Exception):
             logger.warning("没有找到余额不足小弹框，接下来更换支付方式，继续支付.")
         return flag
 
-    @SleepWait(wait_time=10)
+    @SleepWait(wait_time=1)
     def is_payment_complete(self) -> bool:
         """
         判断是否限额，余额不足或其他异常，没有异常的话，输入密码后，会出现【完成】小弹框界面
         """
         flag = False
         try:
             limit_quotas = self.device.get_po_extend(
@@ -1343,15 +1343,15 @@
             payment_amount = payment_amount.get_text()
             logger.info("从支付成功界面获取到的实际支付金额是: {}".format(payment_amount))
             payment_amount = Decimal(payment_amount) if isinstance(payment_amount, str) else payment_amount
         except Exception as e:
             logger.error(str(e))
         return payment_amount
 
-    @SleepWait(wait_time=20)
+    @SleepWait(wait_time=5)
     def touch_payment_complete(self) -> None:
         """在支付成功界面，点击【完成】"""
         try:
             payment_complete_button = self.device.get_po_extend(
                 type="android.widget.TextView",
                 name="android.widget.TextView",
                 text="完成",
```

### Comparing `ctrip-app-ui-0.3.0/capp_ui/fee.py` & `ctrip-app-ui-0.3.1/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.0/capp_ui/libs.py` & `ctrip-app-ui-0.3.1/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.0/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.3.1/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.0/capp_ui/platforms.py` & `ctrip-app-ui-0.3.1/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.0/capp_ui/test.py` & `ctrip-app-ui-0.3.1/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.0/capp_ui/utils.py` & `ctrip-app-ui-0.3.1/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.0/capp_ui/validators.py` & `ctrip-app-ui-0.3.1/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.0/setup.py` & `ctrip-app-ui-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.3.0',
+    version='0.3.1',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

