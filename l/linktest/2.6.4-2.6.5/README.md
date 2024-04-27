# Comparing `tmp/linktest-2.6.4.tar.gz` & `tmp/linktest-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.6.4.tar", last modified: Thu Apr 25 08:22:31 2024, max compression
+gzip compressed data, was "linktest-2.6.5.tar", last modified: Fri Apr 26 09:02:17 2024, max compression
```

## Comparing `linktest-2.6.4.tar` & `linktest-2.6.5.tar`

### file list

```diff
@@ -1,51 +1,56 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-25 08:22:31.246190 linktest-2.6.4/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-25 08:22:31.245913 linktest-2.6.4/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-25 08:22:31.244258 linktest-2.6.4/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-25 08:20:06.000000 linktest-2.6.4/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    15760 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    34827 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   106703 2024-04-25 08:16:26.000000 linktest-2.6.4/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8022 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-25 08:20:16.000000 linktest-2.6.4/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-04-25 08:19:58.000000 linktest-2.6.4/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-25 08:06:42.000000 linktest-2.6.4/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-25 08:22:31.245629 linktest-2.6.4/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-25 08:22:31.000000 linktest-2.6.4/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1271 2024-04-25 08:22:31.000000 linktest-2.6.4/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-25 08:22:31.000000 linktest-2.6.4/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-25 08:22:31.000000 linktest-2.6.4/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-25 08:22:31.000000 linktest-2.6.4/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-25 08:22:31.246239 linktest-2.6.4/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-25 08:22:27.000000 linktest-2.6.4/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-26 09:02:17.445931 linktest-2.6.5/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-26 09:02:17.445636 linktest-2.6.5/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-26 09:02:17.442960 linktest-2.6.5/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-26 03:09:15.000000 linktest-2.6.5/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    15893 2024-04-26 08:38:14.000000 linktest-2.6.5/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    34827 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   106703 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9047 2024-04-26 08:34:28.000000 linktest-2.6.5/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-26 03:09:22.000000 linktest-2.6.5/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-04-25 08:19:58.000000 linktest-2.6.5/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14254 2024-04-26 08:06:07.000000 linktest-2.6.5/linktest/webdriver_wrapper_chrome.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13822 2024-04-26 07:00:42.000000 linktest-2.6.5/linktest/webdriver_wrapper_edge.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13840 2024-04-26 06:55:27.000000 linktest-2.6.5/linktest/webdriver_wrapper_firefox.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13810 2024-04-26 08:08:43.000000 linktest-2.6.5/linktest/webdriver_wrapper_ie.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14254 2024-04-26 08:05:52.000000 linktest-2.6.5/linktest/webdriver_wrapper_safari.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-26 03:06:06.000000 linktest-2.6.5/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-26 09:02:17.445209 linktest-2.6.5/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-26 09:02:17.000000 linktest-2.6.5/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1451 2024-04-26 09:02:17.000000 linktest-2.6.5/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-26 09:02:17.000000 linktest-2.6.5/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-26 09:02:17.000000 linktest-2.6.5/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-26 09:02:17.000000 linktest-2.6.5/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-26 09:02:17.445991 linktest-2.6.5/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-26 09:02:11.000000 linktest-2.6.5/setup.py
```

### Comparing `linktest-2.6.4/linktest/appium_utils.py` & `linktest-2.6.5/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/auto_generate_testcase_list.py` & `linktest-2.6.5/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.6.5/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/base_testcase.py` & `linktest-2.6.5/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/clean_data.py` & `linktest-2.6.5/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/conver_xml_into_db.py` & `linktest-2.6.5/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/database_helper.py` & `linktest-2.6.5/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/date_utilities.py` & `linktest-2.6.5/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/doctor.py` & `linktest-2.6.5/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/framework_log.py` & `linktest-2.6.5/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/generate_html_log.py` & `linktest-2.6.5/linktest/generate_html_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,19 @@
 
 
 def generate_html_log(executing_testcase):
     # executing_testcase.logfile_full_name 是日志文件的完整路径
     # executing_testcase.full_tc_folder 是存放生成的HTML文件的目录
 
     case_type = "API"
+    browser_type = "chrome"
     if getattr(executing_testcase, "browser", None):
         case_type = "UI"
+        browser_type = executing_testcase.browser_name
+
 
     # 读取日志文件内容
     with open(executing_testcase.logfile_full_name, "r") as logfile:
         execution_log = logfile.readlines()
 
     parts = [part for part in executing_testcase.packages.split(',') if part]
     last_part = parts[-1] if parts else ''
@@ -153,18 +156,18 @@
                 font-size: 14px;
             }
         </style>
     </head>
     <body>
         <div class="header">
             <h2 style='padding-left: 25px;'>Execution Log for TestCase: %s</h2> 
-            <h3 style='padding-left: 22px;'>%s &nbsp; | &nbsp;&nbsp; CaseType: %s</h3>
+            <h3 style='padding-left: 22px;'>%s &nbsp; | &nbsp;&nbsp; CaseType: %s &nbsp; | &nbsp; &nbsp; Browser: %s</h3>
         </div>
         <div class="container">
-    """ % (testcase_name_with_package, testcase_status_info, case_type)
+    """ % (testcase_name_with_package, testcase_status_info, case_type, browser_type)
 
     lines = ""
     single_line_flag = False
     traceback_flag = False
 
     # 将日志行转换为HTML元素
     for line in execution_log:
```

### Comparing `linktest-2.6.4/linktest/get_adb_devices.py` & `linktest-2.6.5/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/get_ios_devices_list.py` & `linktest-2.6.5/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/get_platform_info.py` & `linktest-2.6.5/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/get_project_info.py` & `linktest-2.6.5/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/html_report.py` & `linktest-2.6.5/linktest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/logged_requests.py` & `linktest-2.6.5/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/main.py` & `linktest-2.6.5/linktest/main.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/memory_usage.py` & `linktest-2.6.5/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/re_func.py` & `linktest-2.6.5/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/run.py` & `linktest-2.6.5/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/run_testcase_thread.py` & `linktest-2.6.5/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/scp_report_to_specified_path.py` & `linktest-2.6.5/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/selenium_helper.py` & `linktest-2.6.5/linktest/selenium_helper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 import os
 import platform
 import traceback
 import subprocess
 from selenium import webdriver
-from .webdriver_wrapper import WebDriverWrapper
 
+from .webdriver_wrapper_firefox import WebDriverWrapperFireFox
+from .webdriver_wrapper_edge import WebDriverWrapperEdge
+from .webdriver_wrapper_chrome import WebDriverWrapperChrome
+from .webdriver_wrapper_safari import WebDriverWrapperSafari
+from .webdriver_wrapper_ie import WebDriverWrapperIE
 
 try:
     import settings
 except ImportError:
     traceback.print_exc()
 
 try:
     if hasattr(settings, "run_by_github_action") and settings.run_by_github_action is True:
         pass
     else:
-        # Check if the current version of chromedriver exists
-        # and if it doesn't exist, download it automatically,
-        # then add chromedriver to path
-
         try:
             from settings import auto_download_chromedriver
         except ImportError:
             auto_download_chromedriver = False
 
         if auto_download_chromedriver is True:
             import chromedriver_autoinstaller
+
             chromedriver_autoinstaller.install()
 except BaseException:
     traceback.print_exc()
 
 
-from . import get_project_info
-
-
-
 class SeleniumHelper(object):
     set_implicitly_wait_flag = False
 
     @staticmethod
     def open_browser(ui_testcase=None, browser_name=None):
         if browser_name is None:
             if hasattr(settings, "DefaultBrowserName"):
@@ -46,14 +43,16 @@
             elif hasattr(ui_testcase, "DefaultBrowserName"):
                 browser_name = ui_testcase.DefaultBrowserName
             else:
                 browser_name = "chrome"
 
         browser_name = browser_name.lower()
 
+        ui_testcase.browser_name = browser_name
+
         if hasattr(settings, "token") and settings.token:
             # todo: 1. 如果settings.token 存在，则所有UI case 都使用此 token ?  2.  此处先实现功能为主，暂时只支持 Chrome
             if browser_name == 'chrome':
                 from seleniumwire import webdriver  # Import from seleniumwire
                 browser = webdriver.Chrome()
 
                 def interceptor(request):
@@ -75,60 +74,78 @@
 
                 return browser
 
         else:
             from selenium import webdriver
 
             if browser_name == 'ie':
-                browser = webdriver.Ie()
+                    browser = WebDriverWrapperIE(ui_testcase)
+            elif browser_name == 'edge':
+                if hasattr(settings, "HEAD_LESS") and settings.HEAD_LESS:
+                    edge_options = webdriver.EdgeOptions()
+                    edge_options.add_argument("--headless")
+
+                    # 使用 WebDriverWrapperEdge 替换原来的 webdriver 实例
+                    browser = WebDriverWrapperEdge(ui_testcase, options=edge_options)
+                else:
+                    browser = WebDriverWrapperEdge(ui_testcase)
+
             elif browser_name == 'safari':
-                browser = webdriver.Safari()
+                    browser = WebDriverWrapperSafari(ui_testcase)
+
             elif browser_name == 'chrome':
                 chrome_options = webdriver.ChromeOptions()
                 chrome_options.add_argument("--disable-infobars")
 
                 if hasattr(settings, "BROWSER_OPTION"):
                     for opt in settings.BROWSER_OPTION:
                         if type(opt) is str:
                             chrome_options.add_argument(opt)
                         else:
                             raise Exception("settings.BROWSER_OPTION must be a string list!")
 
                 if ui_testcase is None:
-                    browser = webdriver.Chrome(chrome_options=chrome_options)
+                    # read setting.HEAD_LESS 如存在并且值为True 则使用无头模式 否则使用有头模式
+                    if hasattr(settings, "HEAD_LESS") and settings.HEAD_LESS:
+                        # from selenium.webdriver.chrome.options import Options
+                        chrome_options.add_argument("--headless")
+                        chrome_options.add_argument("--disable-gpu")
+                        chrome_options.add_argument("--no-sandbox")
+                        chrome_options.add_argument("--disable-dev-shm-usage")
+                        browser = webdriver.Chrome(chrome_options=chrome_options)
+                    else:
+                        browser = webdriver.Chrome(chrome_options=chrome_options)
                 else:
-                    # TODO: remove below hardcode ".webrtc.", instead of providing the BROWSER_OPTION in setting/__init__.py
-                    if ui_testcase.__module__.find(".webrtc.") == -1:
+                    if hasattr(settings, "HEAD_LESS") and settings.HEAD_LESS:
+                        # from selenium.webdriver.chrome.options import Options
+                        chrome_options.add_argument("--headless")
+                        chrome_options.add_argument("--disable-gpu")
+                        chrome_options.add_argument("--no-sandbox")
+                        chrome_options.add_argument("--disable-dev-shm-usage")
+                        # 使用 WebDriverWrapperChrome 替换原来的 webdriver 实例
+                        browser = WebDriverWrapperChrome(ui_testcase, options=chrome_options)
+                    else:
                         # browser = webdriver.Chrome()
+                        # 使用 WebDriverWrapperChrome 替换原来的 webdriver 实例
+                        browser = WebDriverWrapperChrome(ui_testcase)
+
+            elif browser_name in ('firefox', 'ff'):
+                if hasattr(settings, "HEAD_LESS") and settings.HEAD_LESS:
+                    firefox_options = webdriver.FirefoxOptions()
+                    firefox_options.add_argument("--headless")
+
+                    # 使用 WebDriverWrapperFireFox 替换原来的 webdriver 实例
+                    browser = WebDriverWrapperFireFox(ui_testcase, options=firefox_options)
+                else:
+                    browser = WebDriverWrapperFireFox(ui_testcase)
+
 
-                        # 使用 WebDriverWrapper 替换原来的 webdriver 实例
-                        browser = WebDriverWrapper(ui_testcase)
-                    else:
-                        chrome_options.add_argument("--use-fake-device-for-media-stream")
-                        chrome_options.add_argument("--use-fake-ui-for-media-stream")
-                        chrome_options.add_argument("--incognito")
-
-                        if platform.system() == "Darwin":
-                            pass
-                            # chrome_options.add_argument("--kiosk")
 
-                        if platform.system() == "Windows":
-                            chrome_options.add_argument("--start-fullscreen")
 
-                        browser = webdriver.Chrome(chrome_options=chrome_options)
 
-            elif browser_name in ('firefox', 'ff'):
-                profile = webdriver.FirefoxProfile(settings.FIREFOX_PROFILE)
-                profile.set_preference("startup.homepage_welcome_url.additional", "about:blank")
-                if ui_testcase.__module__.find("tests.webrtc.") == -1:
-                    browser = webdriver.Firefox()
-                else:
-                    profile.set_preference("media.navigator.permission.disabled", "true")
-                    profile.set_preference("browser.dom.window.dump.enabled", "true")
-                    browser = webdriver.Firefox(firefox_profile=profile)
             elif browser_name == 'device':
                 from appium import webdriver as mobiledriver
                 browser = mobiledriver.Remote(
                     command_executor='http://' + ui_testcase.appium_server_ip + ':' + ui_testcase.appium_server_port
                                      + '/wd/hub', desired_capabilities=ui_testcase.capability)
 
         try:
```

### Comparing `linktest-2.6.4/linktest/timeout_thread.py` & `linktest-2.6.5/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/ui_testcase.py` & `linktest-2.6.5/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/update_config.py` & `linktest-2.6.5/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/webdriver_wrapper.py` & `linktest-2.6.5/linktest/webdriver_wrapper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest/xml_report.py` & `linktest-2.6.5/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.4/linktest.egg-info/SOURCES.txt` & `linktest-2.6.5/linktest.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -33,14 +33,19 @@
 linktest/setup.py
 linktest/testcase_order.py
 linktest/testcase_timeout_exception.py
 linktest/timeout_thread.py
 linktest/ui_testcase.py
 linktest/update_config.py
 linktest/webdriver_wrapper.py
+linktest/webdriver_wrapper_chrome.py
+linktest/webdriver_wrapper_edge.py
+linktest/webdriver_wrapper_firefox.py
+linktest/webdriver_wrapper_ie.py
+linktest/webdriver_wrapper_safari.py
 linktest/windows_helper.py
 linktest/xml_report.py
 linktest.egg-info/PKG-INFO
 linktest.egg-info/SOURCES.txt
 linktest.egg-info/dependency_links.txt
 linktest.egg-info/requires.txt
 linktest.egg-info/top_level.txt
```

