# Comparing `tmp/botastico-0.1.5.tar.gz` & `tmp/botastico-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botastico-0.1.5.tar", max compression
+gzip compressed data, was "botastico-0.1.7.tar", max compression
```

## Comparing `botastico-0.1.5.tar` & `botastico-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1077 2023-07-14 16:59:15.508276 botastico-0.1.5/LICENSE
--rw-r--r--   0        0        0     2298 2023-07-19 10:57:57.497617 botastico-0.1.5/README.md
--rw-r--r--   0        0        0       32 2023-07-19 17:41:18.512739 botastico-0.1.5/botastico/__init__.py
--rw-r--r--   0        0        0     6933 2023-07-22 11:14:24.115479 botastico-0.1.5/botastico/botastico.py
--rw-r--r--   0        0        0     5686 2023-10-16 06:50:28.483520 botastico-0.1.5/botastico/langchain.py
--rw-r--r--   0        0        0      844 2023-10-16 09:46:24.613510 botastico-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2835 1970-01-01 00:00:00.000000 botastico-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-14 16:59:15.508276 botastico-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2298 2023-07-19 10:57:57.497617 botastico-0.1.7/README.md
+-rw-r--r--   0        0        0       32 2023-07-19 17:41:18.512739 botastico-0.1.7/botastico/__init__.py
+-rw-r--r--   0        0        0     8874 2024-04-12 14:14:45.610215 botastico-0.1.7/botastico/botastico.py
+-rw-r--r--   0        0        0     5686 2023-10-16 06:50:28.483520 botastico-0.1.7/botastico/langchain.py
+-rw-r--r--   0        0        0      844 2024-04-12 10:27:39.533849 botastico-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2835 1970-01-01 00:00:00.000000 botastico-0.1.7/PKG-INFO
```

### Comparing `botastico-0.1.5/LICENSE` & `botastico-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `botastico-0.1.5/README.md` & `botastico-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `botastico-0.1.5/botastico/botastico.py` & `botastico-0.1.7/botastico/botastico.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import requests
 import os
 import mimetypes
 import logging
 import httpx
 import asyncio
+import shutil
 
 class Botastico:
     def __init__(self, api_key, base_url, agent_id):
         self.api_key = api_key
         self.base_url = base_url
         self.headers = {'Authorization': f'Bearer {api_key}'}
         self.agent_id = agent_id
@@ -46,15 +47,15 @@
                 else:
                     logging.error(f"File upload failed after {MAX_RETRIES} attempts. Moving on to next file. Error: {error_message}")
                 return {'status_code': None, 'file_name': file_name, 'kbdoc_id': None, 'message': error_message}
             except Exception as e:
                 logging.error(f'Error occurred while uploading file: {file_name}. Error: {str(e)}')
                 return {'status_code': None, 'file_name': file_name, 'kbdoc_id': None, 'message': str(e)}
 
-    async def upload_folder(self, folder_path, max_concurrent_tasks=100):
+    async def upload_folder(self, folder_path, max_concurrent_tasks=6):
         if not os.path.exists(folder_path):
             logging.error(f'Folder path: {folder_path} does not exist.')
             return
 
         semaphore = asyncio.Semaphore(max_concurrent_tasks)  # Change this to the maximum number of concurrent tasks you want to allow
 
         async def upload_with_semaphore(file_path, file_name, file_type):
@@ -77,14 +78,40 @@
 
         responses = await asyncio.gather(*tasks)
 
         for response in responses:
             if response is not None:
                 results.append(response) 
         return results
+    
+    async def upload_filenames(self, folder_path, filenames, max_concurrent_tasks=6):
+        if not os.path.exists(folder_path):
+            logging.error(f'Folder path: {folder_path} does not exist.')
+            return
+
+        # Filter out the files that are not in the filenames list
+        filtered_files = []
+        for root, dirs, files in os.walk(folder_path):
+            for file in files:
+                if file in filenames:
+                    filtered_files.append(os.path.join(root, file))
+
+        # Create a temporary folder and copy the filtered files into it
+        temp_folder = os.path.join(folder_path, 'temp_upload')
+        os.makedirs(temp_folder, exist_ok=True)
+        for file_path in filtered_files:
+            shutil.copy(file_path, temp_folder)
+
+        # Upload the entire temp folder
+        results = await self.upload_folder(temp_folder, max_concurrent_tasks=max_concurrent_tasks)
+
+        # Clean up the temporary folder after uploading
+        shutil.rmtree(temp_folder)
+
+        return results
 
     def count_uploadable_files(self, folder_path):
         if not os.path.exists(folder_path):
             logging.error(f'Folder path: {folder_path} does not exist.')
             return 0  # Return 0 if the folder doesn't exist
 
         uploadable_file_count = 0
@@ -108,20 +135,38 @@
                     continue  # Skip .DS_Store files
                 file_path = os.path.join(root, file)
                 file_name = os.path.basename(file_path)
                 uploadable_files_dict[file_path] = file_name
 
         return uploadable_files_dict
 
+    # def extract_kbdoc_ids(self):
+    #     list_response = requests.get(f'{self.base_url}/v1/agents?agent_ids={self.agent_id}', headers=self.headers)
+    #     agent = list_response.json()
+    #     kbdoc_ids = [file['kbdoc_id'] for dictionary in agent for file in dictionary['files'] if 'kbdoc_id' in file]
+    #     return kbdoc_ids
+
+    # def extract_kbdoc_filenames(self):
+    #     list_response = requests.get(f'{self.base_url}/v1/agents?agent_ids={self.agent_id}', headers=self.headers)
+    #     agent = list_response.json()
+    #     filenames = [file['filename'] for dictionary in agent for file in dictionary['files'] if 'filename' in file]
+    #     return filenames
+
     def extract_kbdoc_ids(self):
-        list_response = requests.get(f'{self.base_url}/v1/agents?agent_ids={self.agent_id}', headers=self.headers)
+        list_response = requests.get(f'{self.base_url}/v1/agents/{self.agent_id}/kb', headers=self.headers)
         agent = list_response.json()
-        kbdoc_ids = [file['kbdoc_id'] for dictionary in agent for file in dictionary['files'] if 'kbdoc_id' in file]
+        kbdoc_ids = [kbdoc['kbdoc_id'] for kbdoc in agent]
         return kbdoc_ids
 
+    def extract_kbdoc_filenames(self):
+        list_response = requests.get(f'{self.base_url}/v1/agents/{self.agent_id}/kb', headers=self.headers)
+        agent = list_response.json()
+        filenames = [kbdoc['filename'] for kbdoc in agent]
+        return filenames
+
     async def delete_agent_kbdocs(self):
         kbdoc_ids = self.extract_kbdoc_ids()
         MAX_RETRIES = 3
         async with httpx.AsyncClient() as client:
             for kbdoc_id in kbdoc_ids:
                 for attempt in range(MAX_RETRIES):
                     try:
```

### Comparing `botastico-0.1.5/botastico/langchain.py` & `botastico-0.1.7/botastico/langchain.py`

 * *Files identical despite different names*

### Comparing `botastico-0.1.5/pyproject.toml` & `botastico-0.1.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "botastico"
-version = "0.1.5"
+version = "0.1.7"
 homepage = "https://github.com/botastico/botastico-python"
 description = "Python SDK for using the botasti.co chat API"
 authors = ["Andres Kull", "Bartol Karuza"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `botastico-0.1.5/PKG-INFO` & `botastico-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botastico
-Version: 0.1.5
+Version: 0.1.7
 Summary: Python SDK for using the botasti.co chat API
 Home-page: https://github.com/botastico/botastico-python
 Author: Andres Kull
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
```

