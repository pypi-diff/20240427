# Comparing `tmp/sharepoint_utils-1.0.tar.gz` & `tmp/sharepoint_utils-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharepoint_utils-1.0.tar", last modified: Sun Apr 21 08:23:35 2024, max compression
+gzip compressed data, was "sharepoint_utils-1.1.tar", last modified: Sat Apr 27 10:28:25 2024, max compression
```

## Comparing `sharepoint_utils-1.0.tar` & `sharepoint_utils-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 08:23:35.421550 sharepoint_utils-1.0/
--rw-rw-rw-   0        0        0     1083 2024-04-16 16:34:38.000000 sharepoint_utils-1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1916 2024-04-21 08:23:35.407400 sharepoint_utils-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-21 08:23:35.421572 sharepoint_utils-1.0/setup.cfg
--rw-rw-rw-   0        0        0      791 2024-04-21 07:53:38.000000 sharepoint_utils-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 08:23:35.359104 sharepoint_utils-1.0/sharepoint_utils/
--rw-rw-rw-   0        0        0     6128 2024-04-21 08:21:04.000000 sharepoint_utils-1.0/sharepoint_utils/ModuleRead.py
--rw-rw-rw-   0        0        0      373 2024-04-21 07:52:09.000000 sharepoint_utils-1.0/sharepoint_utils/__init__.py
--rw-rw-rw-   0        0        0     3003 2024-04-21 07:52:35.000000 sharepoint_utils-1.0/sharepoint_utils/main.py
-drwxrwxrwx   0        0        0        0 2024-04-21 08:23:35.405802 sharepoint_utils-1.0/sharepoint_utils.egg-info/
--rw-rw-rw-   0        0        0     1916 2024-04-21 08:23:34.000000 sharepoint_utils-1.0/sharepoint_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2024-04-21 08:23:35.000000 sharepoint_utils-1.0/sharepoint_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 08:23:34.000000 sharepoint_utils-1.0/sharepoint_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-21 08:23:34.000000 sharepoint_utils-1.0/sharepoint_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-21 08:23:34.000000 sharepoint_utils-1.0/sharepoint_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 10:28:25.104755 sharepoint_utils-1.1/
+-rw-rw-rw-   0        0        0     1083 2024-04-16 16:34:38.000000 sharepoint_utils-1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2104 2024-04-27 10:28:25.102964 sharepoint_utils-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-27 10:28:25.104755 sharepoint_utils-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      791 2024-04-27 10:24:50.000000 sharepoint_utils-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:28:25.074841 sharepoint_utils-1.1/sharepoint_utils/
+-rw-rw-rw-   0        0        0     6128 2024-04-21 08:21:04.000000 sharepoint_utils-1.1/sharepoint_utils/ModuleRead.py
+-rw-rw-rw-   0        0        0      416 2024-04-27 10:24:37.000000 sharepoint_utils-1.1/sharepoint_utils/__init__.py
+-rw-rw-rw-   0        0        0     4333 2024-04-27 10:24:08.000000 sharepoint_utils-1.1/sharepoint_utils/main.py
+drwxrwxrwx   0        0        0        0 2024-04-27 10:28:25.101981 sharepoint_utils-1.1/sharepoint_utils.egg-info/
+-rw-rw-rw-   0        0        0     2104 2024-04-27 10:28:24.000000 sharepoint_utils-1.1/sharepoint_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2024-04-27 10:28:24.000000 sharepoint_utils-1.1/sharepoint_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 10:28:24.000000 sharepoint_utils-1.1/sharepoint_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-27 10:28:24.000000 sharepoint_utils-1.1/sharepoint_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-27 10:28:24.000000 sharepoint_utils-1.1/sharepoint_utils.egg-info/top_level.txt
```

### Comparing `sharepoint_utils-1.0/LICENSE.txt` & `sharepoint_utils-1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sharepoint_utils-1.0/PKG-INFO` & `sharepoint_utils-1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharepoint_utils
-Version: 1.0
+Version: 1.1
 Summary: Utility functions for working with SharePoint files
 Author: Omkar Sutar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -27,14 +27,15 @@
 from sharepoint_utils import  upload_dataframe_to_sharepoint
 from sharepoint_utils import  read_file_from_sharepoint
 
 # functions for reading files and folders.
 from sharepoint_utils import  combine_files_into_dataframe
 from sharepoint_utils import  get_folder_urls
 from sharepoint_utils import  get_file_paths
+from sharepoint_utils import  copy_files_within_folders
 ```
 ### Usage Examples
 
 ```python
 # Create connection to sharepoint
 sharepoint_ctx = connect_to_sharepoint('your_username', 'your_password', 'https://your_sharepoint_site_url')
 
@@ -49,13 +50,16 @@
 # get sharepoint folder url as a list
 folder_urls  =  get_folder_urls(sharepoint_ctx, document_library_relative_url)
 print(folder_urls)
 
 # get sharepoint file path as a list
 file_paths  =  get_file_paths(sharepoint_ctx, subfolder_urls_files)
 print(file_paths)
+
+# copy files from one folder to another within sharepoint site
+copy_files_within_folders(ctx, filepath , files_upload_to_path)
 ``` 
 ### Contributing
 
   
 
 Contributions are welcome! If you have any suggestions or find any issues, please feel free to contact me.
```

### Comparing `sharepoint_utils-1.0/setup.py` & `sharepoint_utils-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of README.md
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='sharepoint_utils',
-    version='1.0',
+    version='1.1',
     author='Omkar Sutar',
     description='Utility functions for working with SharePoint files',
     long_description=long_description,
     long_description_content_type='text/markdown',  # This tells setuptools that the long description is in Markdown format
     packages=find_packages(),
     install_requires=[
         'pandas',
```

### Comparing `sharepoint_utils-1.0/sharepoint_utils/ModuleRead.py` & `sharepoint_utils-1.1/sharepoint_utils/ModuleRead.py`

 * *Files identical despite different names*

### Comparing `sharepoint_utils-1.0/sharepoint_utils.egg-info/PKG-INFO` & `sharepoint_utils-1.1/sharepoint_utils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharepoint-utils
-Version: 1.0
+Version: 1.1
 Summary: Utility functions for working with SharePoint files
 Author: Omkar Sutar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -27,14 +27,15 @@
 from sharepoint_utils import  upload_dataframe_to_sharepoint
 from sharepoint_utils import  read_file_from_sharepoint
 
 # functions for reading files and folders.
 from sharepoint_utils import  combine_files_into_dataframe
 from sharepoint_utils import  get_folder_urls
 from sharepoint_utils import  get_file_paths
+from sharepoint_utils import  copy_files_within_folders
 ```
 ### Usage Examples
 
 ```python
 # Create connection to sharepoint
 sharepoint_ctx = connect_to_sharepoint('your_username', 'your_password', 'https://your_sharepoint_site_url')
 
@@ -49,13 +50,16 @@
 # get sharepoint folder url as a list
 folder_urls  =  get_folder_urls(sharepoint_ctx, document_library_relative_url)
 print(folder_urls)
 
 # get sharepoint file path as a list
 file_paths  =  get_file_paths(sharepoint_ctx, subfolder_urls_files)
 print(file_paths)
+
+# copy files from one folder to another within sharepoint site
+copy_files_within_folders(ctx, filepath , files_upload_to_path)
 ``` 
 ### Contributing
 
   
 
 Contributions are welcome! If you have any suggestions or find any issues, please feel free to contact me.
```

