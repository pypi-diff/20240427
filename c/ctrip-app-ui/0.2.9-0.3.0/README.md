# Comparing `tmp/ctrip-app-ui-0.2.9.tar.gz` & `tmp/ctrip-app-ui-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.2.9.tar", last modified: Sat Apr 27 03:04:25 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.3.0.tar", last modified: Sat Apr 27 08:15:19 2024, max compression
```

## Comparing `ctrip-app-ui-0.2.9.tar` & `ctrip-app-ui-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 03:04:25.681097 ctrip-app-ui-0.2.9/
--rw-rw-rw-   0        0        0    11558 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.9/LICENSE
--rw-rw-rw-   0        0        0      474 2024-04-27 03:04:25.681097 ctrip-app-ui-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 03:04:25.678117 ctrip-app-ui-0.2.9/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.9/capp_ui/__init__.py
--rw-rw-rw-   0        0        0     3628 2024-04-27 02:13:31.000000 ctrip-app-ui-0.2.9/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1191 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.9/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.9/capp_ui/dir.py
--rw-rw-rw-   0        0        0    58650 2024-04-27 03:04:03.000000 ctrip-app-ui-0.2.9/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.9/capp_ui/fee.py
--rw-rw-rw-   0        0        0     2270 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.9/capp_ui/libs.py
--rw-rw-rw-   0        0        0    23814 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.9/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1799 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.9/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      689 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.9/capp_ui/test.py
--rw-rw-rw-   0        0        0     5563 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.9/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3016 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.9/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-04-27 03:04:25.680601 ctrip-app-ui-0.2.9/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-04-27 03:04:25.000000 ctrip-app-ui-0.2.9/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2024-04-27 03:04:25.000000 ctrip-app-ui-0.2.9/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 03:04:25.000000 ctrip-app-ui-0.2.9/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-27 03:04:25.000000 ctrip-app-ui-0.2.9/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-27 03:04:25.000000 ctrip-app-ui-0.2.9/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 03:04:25.681097 ctrip-app-ui-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-04-27 03:04:23.000000 ctrip-app-ui-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 08:15:19.806386 ctrip-app-ui-0.3.0/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-04-27 08:15:19.805890 ctrip-app-ui-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 08:15:19.803327 ctrip-app-ui-0.3.0/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0     3628 2024-04-27 02:13:31.000000 ctrip-app-ui-0.3.0/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1191 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    59708 2024-04-27 08:15:00.000000 ctrip-app-ui-0.3.0/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     2270 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    23814 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1799 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      689 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5563 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3016 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.0/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-04-27 08:15:19.805391 ctrip-app-ui-0.3.0/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-04-27 08:15:19.000000 ctrip-app-ui-0.3.0/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2024-04-27 08:15:19.000000 ctrip-app-ui-0.3.0/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 08:15:19.000000 ctrip-app-ui-0.3.0/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-27 08:15:19.000000 ctrip-app-ui-0.3.0/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-27 08:15:19.000000 ctrip-app-ui-0.3.0/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 08:15:19.806386 ctrip-app-ui-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-04-27 08:15:10.000000 ctrip-app-ui-0.3.0/setup.py
```

### Comparing `ctrip-app-ui-0.2.9/LICENSE` & `ctrip-app-ui-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.9/capp_ui/date_extend.py` & `ctrip-app-ui-0.3.0/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.9/capp_ui/device.py` & `ctrip-app-ui-0.3.0/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.9/capp_ui/dir.py` & `ctrip-app-ui-0.3.0/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.9/capp_ui/domain_service.py` & `ctrip-app-ui-0.3.0/capp_ui/domain_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,37 @@
                 status = "已取消"
         except (PocoNoSuchNodeException, PocoTargetTimeout):
             pass
         except Exception as e:
             logger.error(e)
         return status
 
+    def is_order_detail_page(self) -> bool:
+        """是否在订单详情界面"""
+        flag = False
+        try:
+            order_detail_page_1 = self.device.poco(
+                type="android.widget.TextView", name="header_Text_订单详情", text="订单详情"
+            )
+            order_detail_page_2 = self.device.poco(
+                type="android.widget.TextView", name="operateBtnList_Text_我要退订", text="我要退订"
+            )
+            order_detail_page_3 = self.device.poco(
+                type="android.view.ViewGroup", name="CusHeaderView_TouchableOpacity_leftIconWrap",
+                desc="CusHeaderView_TouchableOpacity_leftIconWrap"
+            )
+            if (order_detail_page_1.exists() is True or order_detail_page_2.exists() is True or
+                    order_detail_page_3.exists() is True):
+                flag = True
+        except (PocoNoSuchNodeException, PocoTargetTimeout):
+            pass
+        except Exception as e:
+            logger.error(e)
+        return flag
+
     @SleepWait(wait_time=1)
     def touch_go_back_to_unpaid_list_page_by_search_page(self) -> None:
         """从搜索界面退回到【待支付】列表页"""
         try:
             go_back = self.device.poco(type="android.widget.TextView", name="icon_back")
             if go_back.exists() is True:
                 go_back.click()
```

### Comparing `ctrip-app-ui-0.2.9/capp_ui/fee.py` & `ctrip-app-ui-0.3.0/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.9/capp_ui/libs.py` & `ctrip-app-ui-0.3.0/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.9/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.3.0/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.9/capp_ui/platforms.py` & `ctrip-app-ui-0.3.0/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.9/capp_ui/test.py` & `ctrip-app-ui-0.3.0/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.9/capp_ui/utils.py` & `ctrip-app-ui-0.3.0/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.9/capp_ui/validators.py` & `ctrip-app-ui-0.3.0/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.9/setup.py` & `ctrip-app-ui-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.2.9',
+    version='0.3.0',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

