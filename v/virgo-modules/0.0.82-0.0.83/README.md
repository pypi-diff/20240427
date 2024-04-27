# Comparing `tmp/virgo_modules-0.0.82.tar.gz` & `tmp/virgo_modules-0.0.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virgo_modules-0.0.82.tar", last modified: Sat Apr 20 13:56:40 2024, max compression
+gzip compressed data, was "virgo_modules-0.0.83.tar", last modified: Sat Apr 27 12:42:06 2024, max compression
```

## Comparing `virgo_modules-0.0.82.tar` & `virgo_modules-0.0.83.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 13:56:40.289166 virgo_modules-0.0.82/
--rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.82/LICENSE
--rw-rw-rw-   0        0        0     1411 2024-04-20 13:56:40.286166 virgo_modules-0.0.82/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.82/README.md
--rw-rw-rw-   0        0        0       42 2024-04-20 13:56:40.289166 virgo_modules-0.0.82/setup.cfg
--rw-rw-rw-   0        0        0     1230 2024-04-20 13:56:03.000000 virgo_modules-0.0.82/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 13:56:40.203163 virgo_modules-0.0.82/virgo_app/
-drwxrwxrwx   0        0        0        0 2024-04-20 13:56:40.238168 virgo_modules-0.0.82/virgo_app/virgo_modules/
--rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.82/virgo_app/virgo_modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 13:56:40.283165 virgo_modules-0.0.82/virgo_app/virgo_modules/src/
--rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.82/virgo_app/virgo_modules/src/__init__.py
--rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.82/virgo_app/virgo_modules/src/aws_utils.py
--rw-rw-rw-   0        0        0    13268 2024-04-05 06:56:27.000000 virgo_modules-0.0.82/virgo_app/virgo_modules/src/edge_utils.py
--rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.82/virgo_app/virgo_modules/src/pull_artifacts.py
--rw-rw-rw-   0        0        0    71590 2024-04-19 12:55:21.000000 virgo_modules-0.0.82/virgo_app/virgo_modules/src/re_utils.py
--rw-rw-rw-   0        0        0   144162 2024-04-20 13:56:03.000000 virgo_modules-0.0.82/virgo_app/virgo_modules/src/ticketer_source.py
-drwxrwxrwx   0        0        0        0 2024-04-20 13:56:40.259163 virgo_modules-0.0.82/virgo_app/virgo_modules.egg-info/
--rw-rw-rw-   0        0        0     1411 2024-04-20 13:56:39.000000 virgo_modules-0.0.82/virgo_app/virgo_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2024-04-20 13:56:39.000000 virgo_modules-0.0.82/virgo_app/virgo_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 13:56:39.000000 virgo_modules-0.0.82/virgo_app/virgo_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      276 2024-04-20 13:56:39.000000 virgo_modules-0.0.82/virgo_app/virgo_modules.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-20 13:56:39.000000 virgo_modules-0.0.82/virgo_app/virgo_modules.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 12:42:06.508839 virgo_modules-0.0.83/
+-rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.83/LICENSE
+-rw-rw-rw-   0        0        0     1411 2024-04-27 12:42:06.506838 virgo_modules-0.0.83/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.83/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 12:42:06.509840 virgo_modules-0.0.83/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2024-04-27 12:41:59.000000 virgo_modules-0.0.83/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 12:42:06.390043 virgo_modules-0.0.83/virgo_app/
+drwxrwxrwx   0        0        0        0 2024-04-27 12:42:06.420221 virgo_modules-0.0.83/virgo_app/virgo_modules/
+-rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.83/virgo_app/virgo_modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 12:42:06.493450 virgo_modules-0.0.83/virgo_app/virgo_modules/src/
+-rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.83/virgo_app/virgo_modules/src/__init__.py
+-rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.83/virgo_app/virgo_modules/src/aws_utils.py
+-rw-rw-rw-   0        0        0    13268 2024-04-05 06:56:27.000000 virgo_modules-0.0.83/virgo_app/virgo_modules/src/edge_utils.py
+-rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.83/virgo_app/virgo_modules/src/pull_artifacts.py
+-rw-rw-rw-   0        0        0    71652 2024-04-27 12:41:59.000000 virgo_modules-0.0.83/virgo_app/virgo_modules/src/re_utils.py
+-rw-rw-rw-   0        0        0   144162 2024-04-20 13:56:03.000000 virgo_modules-0.0.83/virgo_app/virgo_modules/src/ticketer_source.py
+drwxrwxrwx   0        0        0        0 2024-04-27 12:42:06.468445 virgo_modules-0.0.83/virgo_app/virgo_modules.egg-info/
+-rw-rw-rw-   0        0        0     1411 2024-04-27 12:42:05.000000 virgo_modules-0.0.83/virgo_app/virgo_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2024-04-27 12:42:05.000000 virgo_modules-0.0.83/virgo_app/virgo_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 12:42:05.000000 virgo_modules-0.0.83/virgo_app/virgo_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      276 2024-04-27 12:42:05.000000 virgo_modules-0.0.83/virgo_app/virgo_modules.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-27 12:42:05.000000 virgo_modules-0.0.83/virgo_app/virgo_modules.egg-info/top_level.txt
```

### Comparing `virgo_modules-0.0.82/LICENSE` & `virgo_modules-0.0.83/LICENSE`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.82/PKG-INFO` & `virgo_modules-0.0.83/virgo_app/virgo_modules.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: virgo_modules
-Version: 0.0.82
+Name: virgo-modules
+Version: 0.0.83
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.82/setup.py` & `virgo_modules-0.0.83/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("virgo_app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="virgo_modules",
-    version="0.0.82",
+    version="0.0.83",
     description="data processing and statistical modeling using stock market data",
     package_dir={"": "virgo_app"},
     packages=find_packages(where="virgo_app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelmayhem92/virgo_module",
     author="Miguel Mayhuire",
```

### Comparing `virgo_modules-0.0.82/virgo_app/virgo_modules/src/aws_utils.py` & `virgo_modules-0.0.83/virgo_app/virgo_modules/src/aws_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.82/virgo_app/virgo_modules/src/edge_utils.py` & `virgo_modules-0.0.83/virgo_app/virgo_modules/src/edge_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.82/virgo_app/virgo_modules/src/pull_artifacts.py` & `virgo_modules-0.0.83/virgo_app/virgo_modules/src/pull_artifacts.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.82/virgo_app/virgo_modules/src/re_utils.py` & `virgo_modules-0.0.83/virgo_app/virgo_modules/src/re_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1274,15 +1274,17 @@
         if self.save_path:
             fig.write_json(self.save_path+result_json_name)
         if self.show_plot:
             fig.show()
         if self.save_path and self.save_aws:
             # upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = f'market_plots/{self.ticket_name}/'+result_json_name ,input_path = self.save_path+result_json_name)
             upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = self.save_aws + result_json_name, input_path = self.save_path + result_json_name, aws_credentials = self.aws_credentials)
-
+        if self.return_figs:
+            return fig
+        
 def plot_hmm_analysis_logger(data_frame,test_data_size, save_path = False, show_plot = True):
     '''
     display box plots train and test of hmm state returns
 
             Parameters:
                     data_frame (pd.DataFrame): asset data
                     test_data_size (int): test data size, the remaining is training data
```

### Comparing `virgo_modules-0.0.82/virgo_app/virgo_modules/src/ticketer_source.py` & `virgo_modules-0.0.83/virgo_app/virgo_modules/src/ticketer_source.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.82/virgo_app/virgo_modules.egg-info/PKG-INFO` & `virgo_modules-0.0.83/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: virgo-modules
-Version: 0.0.82
+Name: virgo_modules
+Version: 0.0.83
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.82/virgo_app/virgo_modules.egg-info/SOURCES.txt` & `virgo_modules-0.0.83/virgo_app/virgo_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

