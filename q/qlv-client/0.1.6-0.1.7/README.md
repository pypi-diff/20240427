# Comparing `tmp/qlv-client-0.1.6.tar.gz` & `tmp/qlv-client-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlv-client-0.1.6.tar", last modified: Fri Apr 26 01:48:20 2024, max compression
+gzip compressed data, was "qlv-client-0.1.7.tar", last modified: Sat Apr 27 02:38:32 2024, max compression
```

## Comparing `qlv-client-0.1.6.tar` & `qlv-client-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 01:48:20.192404 qlv-client-0.1.6/
--rw-rw-rw-   0        0        0    11558 2024-04-17 06:55:59.000000 qlv-client-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      456 2024-04-26 01:48:20.191907 qlv-client-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 06:55:59.000000 qlv-client-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 01:48:20.188686 qlv-client-0.1.6/qlv_client/
--rw-rw-rw-   0        0        0      463 2024-04-17 08:02:13.000000 qlv-client-0.1.6/qlv_client/__init__.py
--rw-rw-rw-   0        0        0     9543 2024-04-17 08:27:22.000000 qlv-client-0.1.6/qlv_client/api.py
--rw-rw-rw-   0        0        0     1224 2024-04-17 07:59:59.000000 qlv-client-0.1.6/qlv_client/config.py
--rw-rw-rw-   0        0        0     1303 2024-04-17 07:30:16.000000 qlv-client-0.1.6/qlv_client/converter.py
--rw-rw-rw-   0        0        0     4115 2024-04-17 08:27:22.000000 qlv-client-0.1.6/qlv_client/http_client.py
--rw-rw-rw-   0        0        0     6737 2024-04-26 01:48:00.000000 qlv-client-0.1.6/qlv_client/proxy.py
--rw-rw-rw-   0        0        0     3187 2024-04-17 08:27:22.000000 qlv-client-0.1.6/qlv_client/repository.py
--rw-rw-rw-   0        0        0     2235 2024-04-17 08:27:22.000000 qlv-client-0.1.6/qlv_client/test.py
--rw-rw-rw-   0        0        0     1995 2024-04-17 07:29:50.000000 qlv-client-0.1.6/qlv_client/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-26 01:48:20.191907 qlv-client-0.1.6/qlv_client.egg-info/
--rw-rw-rw-   0        0        0      456 2024-04-26 01:48:20.000000 qlv-client-0.1.6/qlv_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2024-04-26 01:48:20.000000 qlv-client-0.1.6/qlv_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 01:48:20.000000 qlv-client-0.1.6/qlv_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-26 01:48:20.000000 qlv-client-0.1.6/qlv_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-26 01:48:20.000000 qlv-client-0.1.6/qlv_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 01:48:20.192404 qlv-client-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1066 2024-04-26 01:48:09.000000 qlv-client-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 02:38:32.094154 qlv-client-0.1.7/
+-rw-rw-rw-   0        0        0    11558 2024-04-17 06:55:59.000000 qlv-client-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      456 2024-04-27 02:38:32.094154 qlv-client-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 06:55:59.000000 qlv-client-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 02:38:32.091175 qlv-client-0.1.7/qlv_client/
+-rw-rw-rw-   0        0        0      463 2024-04-17 08:02:13.000000 qlv-client-0.1.7/qlv_client/__init__.py
+-rw-rw-rw-   0        0        0     9543 2024-04-17 08:27:22.000000 qlv-client-0.1.7/qlv_client/api.py
+-rw-rw-rw-   0        0        0     1224 2024-04-17 07:59:59.000000 qlv-client-0.1.7/qlv_client/config.py
+-rw-rw-rw-   0        0        0     1303 2024-04-17 07:30:16.000000 qlv-client-0.1.7/qlv_client/converter.py
+-rw-rw-rw-   0        0        0     4115 2024-04-17 08:27:22.000000 qlv-client-0.1.7/qlv_client/http_client.py
+-rw-rw-rw-   0        0        0     6834 2024-04-27 02:37:27.000000 qlv-client-0.1.7/qlv_client/proxy.py
+-rw-rw-rw-   0        0        0     3187 2024-04-17 08:27:22.000000 qlv-client-0.1.7/qlv_client/repository.py
+-rw-rw-rw-   0        0        0     2235 2024-04-17 08:27:22.000000 qlv-client-0.1.7/qlv_client/test.py
+-rw-rw-rw-   0        0        0     1995 2024-04-17 07:29:50.000000 qlv-client-0.1.7/qlv_client/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-27 02:38:32.093658 qlv-client-0.1.7/qlv_client.egg-info/
+-rw-rw-rw-   0        0        0      456 2024-04-27 02:38:32.000000 qlv-client-0.1.7/qlv_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2024-04-27 02:38:32.000000 qlv-client-0.1.7/qlv_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 02:38:32.000000 qlv-client-0.1.7/qlv_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-27 02:38:32.000000 qlv-client-0.1.7/qlv_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-27 02:38:32.000000 qlv-client-0.1.7/qlv_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 02:38:32.094154 qlv-client-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2024-04-27 02:35:45.000000 qlv-client-0.1.7/setup.py
```

### Comparing `qlv-client-0.1.6/LICENSE` & `qlv-client-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.6/qlv_client/api.py` & `qlv-client-0.1.7/qlv_client/api.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.6/qlv_client/config.py` & `qlv-client-0.1.7/qlv_client/config.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.6/qlv_client/converter.py` & `qlv-client-0.1.7/qlv_client/converter.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.6/qlv_client/http_client.py` & `qlv-client-0.1.7/qlv_client/http_client.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.6/qlv_client/proxy.py` & `qlv-client-0.1.7/qlv_client/proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         kwargs.update(unlock_order_params)
         order_ser = OrderService(**QlvConfigRepository.get_host_params())
         result = order_ser.unlock_order(**kwargs)
         if result.get("code") == 1:
             logger.info("劲旅平台订单<{}>解锁成功.".format(order_id))
             return True
         else:
-            logger.error("劲旅平台订单<{}>解锁失败...".format(order_id))
+            logger.error("劲旅平台订单<{}>解锁失败，返回：{}".format(order_id, result))
             return False
 
     @classmethod
     def unlock_reason_with_flag(cls, flag: bool, order_id: int, oper: str, remark: str) -> bool:
         unlock_reason_params = QlvConfigRepository.get_unlock_reason_params(
             flag=flag, order_id=order_id, oper=oper, remark=remark
         )
@@ -66,30 +66,30 @@
         logger.info("开始向劲旅系统回填采购信息...")
         args = QlvConfigRepository.get_request_base_params(inter_name="save_order_pay_info")
         order_pay_info = QlvConfigRepository.get_order_pay_info(**kwargs)
         args.update(order_pay_info)
         order_ser = OrderService(**QlvConfigRepository.get_host_params())
         result = order_ser.save_order_pay_info(**args)
         if result.get("code") == 0:
-            logger.error("向劲旅系统回填采购信息失败...")
+            logger.error("向劲旅系统回填采购信息失败，返回：{}".format(result))
             return False
         else:
             logger.error("向劲旅系统回填采购信息成功.")
             return True
 
     @classmethod
     def save_itinerary_info(cls, **kwargs) -> bool:
         logger.info("开始向劲旅系统回填乘客票单信息...")
         args = QlvConfigRepository.get_request_base_params(inter_name="fill_order_itinerary_info")
         order_itinerary_info = QlvConfigRepository.get_order_itinerary_info(**kwargs)
         args.update(order_itinerary_info)
         order_ser = OrderService(**QlvConfigRepository.get_host_params())
         result = order_ser.fill_order_itinerary_info(**args)
         if result.get("code") == 0:
-            logger.error("向劲旅系统回填乘客票单信息失败...")
+            logger.error("向劲旅系统回填乘客票单信息失败，返回：{}".format(result))
             return False
         else:
             logger.error("向劲旅系统回填乘客票单信息成功.")
             return True
 
     @classmethod
     def save_itinerary_info_by_batch_itinerary(cls, pre_order_id: int, oper: str, itinerary_info: list) -> bool:
@@ -111,15 +111,15 @@
                 "oper": oper,
                 "ticket_infos": ";".join(ticket_infos)
             }
             args.update(order_itinerary_info)
             order_ser = OrderService(**QlvConfigRepository.get_host_params())
             result = order_ser.fill_order_itinerary_info(**args)
             if result.get("code") == 0:
-                logger.error("向劲旅系统回填乘客票单信息失败...")
+                logger.error("向劲旅系统回填乘客票单信息失败，返回：{}".format(result))
                 return False
             else:
                 logger.info("向劲旅系统回填乘客票单信息成功.")
                 return True
         else:
             return False
```

### Comparing `qlv-client-0.1.6/qlv_client/repository.py` & `qlv-client-0.1.7/qlv_client/repository.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.6/qlv_client/test.py` & `qlv-client-0.1.7/qlv_client/test.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.6/qlv_client/utils.py` & `qlv-client-0.1.7/qlv_client/utils.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.6/setup.py` & `qlv-client-0.1.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qlv-client',
-    version='0.1.6',
+    version='0.1.7',
     description='This is my qlv proxy qlv_client package',
     long_description='This is my qlv proxy qlv_client package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/qlvClient',
     packages=find_packages(),
     install_requires=[
```

