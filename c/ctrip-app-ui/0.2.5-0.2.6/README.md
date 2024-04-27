# Comparing `tmp/ctrip-app-ui-0.2.5.tar.gz` & `tmp/ctrip-app-ui-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.2.5.tar", last modified: Sat Apr 27 01:52:56 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.2.6.tar", last modified: Sat Apr 27 02:03:55 2024, max compression
```

## Comparing `ctrip-app-ui-0.2.5.tar` & `ctrip-app-ui-0.2.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 01:52:56.477672 ctrip-app-ui-0.2.5/
--rw-rw-rw-   0        0        0    11558 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.5/LICENSE
--rw-rw-rw-   0        0        0      474 2024-04-27 01:52:56.477175 ctrip-app-ui-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 01:52:56.474692 ctrip-app-ui-0.2.5/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.5/capp_ui/__init__.py
--rw-rw-rw-   0        0        0     3500 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.5/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1191 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.5/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.5/capp_ui/dir.py
--rw-rw-rw-   0        0        0    58515 2024-04-27 01:52:36.000000 ctrip-app-ui-0.2.5/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.5/capp_ui/fee.py
--rw-rw-rw-   0        0        0     2270 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.5/capp_ui/libs.py
--rw-rw-rw-   0        0        0    23814 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.5/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1799 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.5/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      689 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.5/capp_ui/test.py
--rw-rw-rw-   0        0        0     5563 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.5/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3016 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.5/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-04-27 01:52:56.476678 ctrip-app-ui-0.2.5/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-04-27 01:52:56.000000 ctrip-app-ui-0.2.5/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2024-04-27 01:52:56.000000 ctrip-app-ui-0.2.5/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 01:52:56.000000 ctrip-app-ui-0.2.5/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-27 01:52:56.000000 ctrip-app-ui-0.2.5/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-27 01:52:56.000000 ctrip-app-ui-0.2.5/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 01:52:56.477672 ctrip-app-ui-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-04-27 01:52:46.000000 ctrip-app-ui-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 02:03:55.396058 ctrip-app-ui-0.2.6/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-04-27 02:03:55.395562 ctrip-app-ui-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 02:03:55.392582 ctrip-app-ui-0.2.6/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0     3500 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1191 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    58613 2024-04-27 02:03:35.000000 ctrip-app-ui-0.2.6/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     2270 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    23814 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1799 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      689 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5563 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3016 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-04-27 02:03:55.395065 ctrip-app-ui-0.2.6/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-04-27 02:03:55.000000 ctrip-app-ui-0.2.6/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2024-04-27 02:03:55.000000 ctrip-app-ui-0.2.6/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 02:03:55.000000 ctrip-app-ui-0.2.6/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-27 02:03:55.000000 ctrip-app-ui-0.2.6/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-27 02:03:55.000000 ctrip-app-ui-0.2.6/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 02:03:55.396058 ctrip-app-ui-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-04-27 02:03:48.000000 ctrip-app-ui-0.2.6/setup.py
```

### Comparing `ctrip-app-ui-0.2.5/LICENSE` & `ctrip-app-ui-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.5/capp_ui/date_extend.py` & `ctrip-app-ui-0.2.6/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.5/capp_ui/device.py` & `ctrip-app-ui-0.2.6/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.5/capp_ui/dir.py` & `ctrip-app-ui-0.2.6/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.5/capp_ui/domain_service.py` & `ctrip-app-ui-0.2.6/capp_ui/domain_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,21 +241,23 @@
                 # 提取匹配到的内容
                 if time_match:
                     time_str = time_match.group(1)
                     string = "从订单获取到的过期时间为：{}".format(time_str)
                     is_later = is_later_than_current_time(time_str=time_str, minutes=5)
                     if is_later is False:
                         flag = True
-                        string = remark = "支付时间少于5分钟"
+                        remark = "支付时间少于5分钟"
+                        string = string + "，" + remark
                 elif amount_match:
                     amount_str = amount_match.group(1)
                     string = "从订单获取到的支付金额为：{}".format(amount_str)
                     if Decimal(amount_str) > Decimal(out_total_price):
                         flag = True
-                        string = remark = "航班已变价"
+                        remark = "航班已变价"
+                        string = string + "，" + remark
                 else:
                     string = "从元素的文案<{}>提取时间与金额信息有异常".format(text)
             else:
                 string = "元素定位存在异常，订单详情页没有找到订单支付金额和过期时间"
             print(string)
         except (PocoNoSuchNodeException, PocoTargetTimeout):
             pass
```

### Comparing `ctrip-app-ui-0.2.5/capp_ui/fee.py` & `ctrip-app-ui-0.2.6/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.5/capp_ui/libs.py` & `ctrip-app-ui-0.2.6/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.5/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.2.6/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.5/capp_ui/platforms.py` & `ctrip-app-ui-0.2.6/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.5/capp_ui/test.py` & `ctrip-app-ui-0.2.6/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.5/capp_ui/utils.py` & `ctrip-app-ui-0.2.6/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.5/capp_ui/validators.py` & `ctrip-app-ui-0.2.6/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.5/setup.py` & `ctrip-app-ui-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.2.5',
+    version='0.2.6',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

