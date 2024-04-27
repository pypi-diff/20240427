# Comparing `tmp/ctrip-app-ui-0.3.5.tar.gz` & `tmp/ctrip-app-ui-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.3.5.tar", last modified: Sat Apr 27 09:07:53 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.3.6.tar", last modified: Sat Apr 27 09:56:02 2024, max compression
```

## Comparing `ctrip-app-ui-0.3.5.tar` & `ctrip-app-ui-0.3.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 09:07:53.916950 ctrip-app-ui-0.3.5/
--rw-rw-rw-   0        0        0    11558 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.5/LICENSE
--rw-rw-rw-   0        0        0      474 2024-04-27 09:07:53.916950 ctrip-app-ui-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 09:07:53.913970 ctrip-app-ui-0.3.5/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.5/capp_ui/__init__.py
--rw-rw-rw-   0        0        0     3628 2024-04-27 02:13:31.000000 ctrip-app-ui-0.3.5/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1191 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.5/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.5/capp_ui/dir.py
--rw-rw-rw-   0        0        0    59170 2024-04-27 09:04:48.000000 ctrip-app-ui-0.3.5/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.5/capp_ui/fee.py
--rw-rw-rw-   0        0        0     2270 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.5/capp_ui/libs.py
--rw-rw-rw-   0        0        0    23814 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.5/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1799 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.5/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      689 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.5/capp_ui/test.py
--rw-rw-rw-   0        0        0     5563 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.5/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3016 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.5/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-04-27 09:07:53.916453 ctrip-app-ui-0.3.5/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-04-27 09:07:53.000000 ctrip-app-ui-0.3.5/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2024-04-27 09:07:53.000000 ctrip-app-ui-0.3.5/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 09:07:53.000000 ctrip-app-ui-0.3.5/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-27 09:07:53.000000 ctrip-app-ui-0.3.5/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-27 09:07:53.000000 ctrip-app-ui-0.3.5/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 09:07:53.917446 ctrip-app-ui-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-04-27 09:07:47.000000 ctrip-app-ui-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 09:56:02.010776 ctrip-app-ui-0.3.6/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-04-27 09:56:02.010045 ctrip-app-ui-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 09:56:02.007358 ctrip-app-ui-0.3.6/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0     3628 2024-04-27 02:13:31.000000 ctrip-app-ui-0.3.6/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1191 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    59905 2024-04-27 09:55:14.000000 ctrip-app-ui-0.3.6/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     2270 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    23814 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1799 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      689 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5563 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3016 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.6/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-04-27 09:56:02.009548 ctrip-app-ui-0.3.6/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-04-27 09:56:01.000000 ctrip-app-ui-0.3.6/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2024-04-27 09:56:01.000000 ctrip-app-ui-0.3.6/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 09:56:01.000000 ctrip-app-ui-0.3.6/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-27 09:56:01.000000 ctrip-app-ui-0.3.6/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-27 09:56:01.000000 ctrip-app-ui-0.3.6/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 09:56:02.010776 ctrip-app-ui-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-04-27 09:56:00.000000 ctrip-app-ui-0.3.6/setup.py
```

### Comparing `ctrip-app-ui-0.3.5/LICENSE` & `ctrip-app-ui-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.5/capp_ui/date_extend.py` & `ctrip-app-ui-0.3.6/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.5/capp_ui/device.py` & `ctrip-app-ui-0.3.6/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.5/capp_ui/dir.py` & `ctrip-app-ui-0.3.6/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.5/capp_ui/domain_service.py` & `ctrip-app-ui-0.3.6/capp_ui/domain_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,22 +187,33 @@
                 status = "已取消"
         except (PocoNoSuchNodeException, PocoTargetTimeout):
             pass
         except Exception as e:
             logger.error(e)
         return status
 
-    def is_readme_me(self) -> bool:
+    def is_order_detail_page(self) -> bool:
         """是否在订单详情界面"""
         flag = False
         try:
             order_detail_page_1 = self.device.poco(
                 type="android.widget.TextView", name="浮层标题", text="出行前必读"
             )
-            if order_detail_page_1.exists() is True:
+            order_detail_page_2 = self.device.poco(
+                type="android.widget.TextView", name="header_Text_订单详情", text="订单详情"
+            )
+            order_detail_page_3 = self.device.poco(
+                type="android.widget.TextView", name="operateBtnList_Text_我要退订", text="我要退订"
+            )
+            order_detail_page_4 = self.device.poco(
+                type="android.view.ViewGroup", name="CusHeaderView_TouchableOpacity_leftIconWrap",
+                desc="CusHeaderView_TouchableOpacity_leftIconWrap"
+            )
+            if (order_detail_page_1.exists() is True or order_detail_page_2.exists() is True or
+                    order_detail_page_3.exists() is True or order_detail_page_4.exists() is True):
                 flag = True
         except (PocoNoSuchNodeException, PocoTargetTimeout):
             pass
         except Exception as e:
             logger.error(e)
         return flag
```

### Comparing `ctrip-app-ui-0.3.5/capp_ui/fee.py` & `ctrip-app-ui-0.3.6/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.5/capp_ui/libs.py` & `ctrip-app-ui-0.3.6/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.5/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.3.6/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.5/capp_ui/platforms.py` & `ctrip-app-ui-0.3.6/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.5/capp_ui/test.py` & `ctrip-app-ui-0.3.6/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.5/capp_ui/utils.py` & `ctrip-app-ui-0.3.6/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.5/capp_ui/validators.py` & `ctrip-app-ui-0.3.6/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.5/setup.py` & `ctrip-app-ui-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.3.5',
+    version='0.3.6',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

