# Comparing `tmp/ctrip-app-ui-0.2.6.tar.gz` & `tmp/ctrip-app-ui-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.2.6.tar", last modified: Sat Apr 27 02:03:55 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.2.7.tar", last modified: Sat Apr 27 02:14:13 2024, max compression
```

## Comparing `ctrip-app-ui-0.2.6.tar` & `ctrip-app-ui-0.2.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 02:03:55.396058 ctrip-app-ui-0.2.6/
--rw-rw-rw-   0        0        0    11558 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/LICENSE
--rw-rw-rw-   0        0        0      474 2024-04-27 02:03:55.395562 ctrip-app-ui-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 02:03:55.392582 ctrip-app-ui-0.2.6/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/capp_ui/__init__.py
--rw-rw-rw-   0        0        0     3500 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1191 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/capp_ui/dir.py
--rw-rw-rw-   0        0        0    58613 2024-04-27 02:03:35.000000 ctrip-app-ui-0.2.6/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/capp_ui/fee.py
--rw-rw-rw-   0        0        0     2270 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/capp_ui/libs.py
--rw-rw-rw-   0        0        0    23814 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1799 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      689 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/capp_ui/test.py
--rw-rw-rw-   0        0        0     5563 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3016 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.6/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-04-27 02:03:55.395065 ctrip-app-ui-0.2.6/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-04-27 02:03:55.000000 ctrip-app-ui-0.2.6/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2024-04-27 02:03:55.000000 ctrip-app-ui-0.2.6/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 02:03:55.000000 ctrip-app-ui-0.2.6/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-27 02:03:55.000000 ctrip-app-ui-0.2.6/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-27 02:03:55.000000 ctrip-app-ui-0.2.6/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 02:03:55.396058 ctrip-app-ui-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-04-27 02:03:48.000000 ctrip-app-ui-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 02:14:13.550710 ctrip-app-ui-0.2.7/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-04-27 02:14:13.550213 ctrip-app-ui-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 02:14:13.547233 ctrip-app-ui-0.2.7/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.7/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0     3628 2024-04-27 02:13:31.000000 ctrip-app-ui-0.2.7/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1191 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.7/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.7/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    58613 2024-04-27 02:03:35.000000 ctrip-app-ui-0.2.7/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.7/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     2270 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.7/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    23814 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.7/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1799 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.7/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      689 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.7/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5563 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.7/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3016 2024-04-27 01:24:22.000000 ctrip-app-ui-0.2.7/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-04-27 02:14:13.549717 ctrip-app-ui-0.2.7/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-04-27 02:14:13.000000 ctrip-app-ui-0.2.7/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2024-04-27 02:14:13.000000 ctrip-app-ui-0.2.7/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 02:14:13.000000 ctrip-app-ui-0.2.7/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-27 02:14:13.000000 ctrip-app-ui-0.2.7/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-27 02:14:13.000000 ctrip-app-ui-0.2.7/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 02:14:13.550710 ctrip-app-ui-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-04-27 02:14:05.000000 ctrip-app-ui-0.2.7/setup.py
```

### Comparing `ctrip-app-ui-0.2.6/LICENSE` & `ctrip-app-ui-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.6/capp_ui/date_extend.py` & `ctrip-app-ui-0.2.7/capp_ui/date_extend.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,12 +91,14 @@
     return datetime.now().strftime(standard_date_format)
 
 
 def is_later_than_current_time(time_str: str, minutes: int = 5):
     # 将给定时间字符串转换为 datetime 对象
     given_time = datetime.strptime(time_str, '%H:%M')
     # 获取当前时间
-    current_time = datetime.now()
+    current_datatime = datetime.now()
+    current_time_str = current_datatime.strftime("%H:%M")
+    current_time = datetime.strptime(current_time_str, '%H:%M')
     # 计算当前时间之后5分钟的时间
     five_minutes_later = current_time + timedelta(minutes=minutes)
     # 比较给定时间是否晚于当前时间5分钟后的时间
     return given_time > five_minutes_later
```

### Comparing `ctrip-app-ui-0.2.6/capp_ui/device.py` & `ctrip-app-ui-0.2.7/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.6/capp_ui/dir.py` & `ctrip-app-ui-0.2.7/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.6/capp_ui/domain_service.py` & `ctrip-app-ui-0.2.7/capp_ui/domain_service.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.6/capp_ui/fee.py` & `ctrip-app-ui-0.2.7/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.6/capp_ui/libs.py` & `ctrip-app-ui-0.2.7/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.6/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.2.7/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.6/capp_ui/platforms.py` & `ctrip-app-ui-0.2.7/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.6/capp_ui/test.py` & `ctrip-app-ui-0.2.7/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.6/capp_ui/utils.py` & `ctrip-app-ui-0.2.7/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.6/capp_ui/validators.py` & `ctrip-app-ui-0.2.7/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.6/setup.py` & `ctrip-app-ui-0.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.2.6',
+    version='0.2.7',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

