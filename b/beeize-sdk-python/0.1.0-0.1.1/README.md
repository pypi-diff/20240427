# Comparing `tmp/beeize-sdk-python-0.1.0.tar.gz` & `tmp/beeize-sdk-python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beeize-sdk-python-0.1.0.tar", last modified: Tue Feb 27 14:27:22 2024, max compression
+gzip compressed data, was "beeize-sdk-python-0.1.1.tar", last modified: Sat Apr 27 11:44:48 2024, max compression
```

## Comparing `beeize-sdk-python-0.1.0.tar` & `beeize-sdk-python-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-02-27 14:27:22.695243 beeize-sdk-python-0.1.0/
--rw-r--r--   0 zhaoyang   (501) staff       (20)       97 2024-02-27 14:27:22.694886 beeize-sdk-python-0.1.0/PKG-INFO
--rw-r--r--   0 zhaoyang   (501) staff       (20)        0 2024-02-27 14:27:18.000000 beeize-sdk-python-0.1.0/README.md
--rw-r--r--   0 zhaoyang   (501) staff       (20)       38 2024-02-27 14:27:22.695344 beeize-sdk-python-0.1.0/setup.cfg
--rw-r--r--   0 zhaoyang   (501) staff       (20)      364 2023-12-28 02:30:23.000000 beeize-sdk-python-0.1.0/setup.py
-drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-02-27 14:27:22.686580 beeize-sdk-python-0.1.0/src/
-drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-02-27 14:27:22.689843 beeize-sdk-python-0.1.0/src/beeize/
--rw-r--r--   0 zhaoyang   (501) staff       (20)        0 2023-11-15 15:29:56.000000 beeize-sdk-python-0.1.0/src/beeize/__init__.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)     1115 2024-01-21 10:11:16.000000 beeize-sdk-python-0.1.0/src/beeize/config.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)      132 2023-12-03 06:12:45.000000 beeize-sdk-python-0.1.0/src/beeize/consts.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)     1556 2024-01-21 10:09:06.000000 beeize-sdk-python-0.1.0/src/beeize/scraper.py
-drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-02-27 14:27:22.693204 beeize-sdk-python-0.1.0/src/beeize/storages/
--rw-r--r--   0 zhaoyang   (501) staff       (20)      161 2023-12-28 06:57:33.000000 beeize-sdk-python-0.1.0/src/beeize/storages/__init__.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)     2726 2024-02-08 15:16:57.000000 beeize-sdk-python-0.1.0/src/beeize/storages/dataset.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)     6227 2024-02-09 07:10:12.000000 beeize-sdk-python-0.1.0/src/beeize/storages/kv_store.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)     5013 2024-02-08 15:16:57.000000 beeize-sdk-python-0.1.0/src/beeize/storages/request_queue.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)        0 2023-11-15 15:27:00.000000 beeize-sdk-python-0.1.0/src/beeize/storages/storage_manager.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)     2159 2023-12-03 11:08:36.000000 beeize-sdk-python-0.1.0/src/beeize/utils.py
-drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-02-27 14:27:22.694504 beeize-sdk-python-0.1.0/src/beeize_sdk_python.egg-info/
--rw-r--r--   0 zhaoyang   (501) staff       (20)       97 2024-02-27 14:27:22.000000 beeize-sdk-python-0.1.0/src/beeize_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 zhaoyang   (501) staff       (20)      476 2024-02-27 14:27:22.000000 beeize-sdk-python-0.1.0/src/beeize_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 zhaoyang   (501) staff       (20)        1 2024-02-27 14:27:22.000000 beeize-sdk-python-0.1.0/src/beeize_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 zhaoyang   (501) staff       (20)        7 2024-02-27 14:27:22.000000 beeize-sdk-python-0.1.0/src/beeize_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-04-27 11:44:48.620743 beeize-sdk-python-0.1.1/
+-rw-r--r--   0 zhaoyang   (501) staff       (20)       97 2024-04-27 11:44:48.620481 beeize-sdk-python-0.1.1/PKG-INFO
+-rw-r--r--   0 zhaoyang   (501) staff       (20)     6405 2024-04-08 15:33:34.000000 beeize-sdk-python-0.1.1/README.md
+-rw-r--r--   0 zhaoyang   (501) staff       (20)       38 2024-04-27 11:44:48.620832 beeize-sdk-python-0.1.1/setup.cfg
+-rw-r--r--   0 zhaoyang   (501) staff       (20)      364 2024-04-27 11:44:46.000000 beeize-sdk-python-0.1.1/setup.py
+drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-04-27 11:44:48.615494 beeize-sdk-python-0.1.1/src/
+drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-04-27 11:44:48.617565 beeize-sdk-python-0.1.1/src/beeize/
+-rw-r--r--   0 zhaoyang   (501) staff       (20)       14 2024-04-27 11:35:18.000000 beeize-sdk-python-0.1.1/src/beeize/__init__.py
+-rw-r--r--   0 zhaoyang   (501) staff       (20)     1130 2024-04-27 11:35:18.000000 beeize-sdk-python-0.1.1/src/beeize/config.py
+-rw-r--r--   0 zhaoyang   (501) staff       (20)      132 2023-12-03 06:12:45.000000 beeize-sdk-python-0.1.1/src/beeize/consts.py
+-rw-r--r--   0 zhaoyang   (501) staff       (20)     1571 2024-04-27 11:35:18.000000 beeize-sdk-python-0.1.1/src/beeize/scraper.py
+drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-04-27 11:44:48.618993 beeize-sdk-python-0.1.1/src/beeize/storages/
+-rw-r--r--   0 zhaoyang   (501) staff       (20)      176 2024-04-27 11:34:11.000000 beeize-sdk-python-0.1.1/src/beeize/storages/__init__.py
+-rw-r--r--   0 zhaoyang   (501) staff       (20)     2846 2024-04-27 11:41:19.000000 beeize-sdk-python-0.1.1/src/beeize/storages/dataset.py
+-rw-r--r--   0 zhaoyang   (501) staff       (20)     6504 2024-04-27 11:41:19.000000 beeize-sdk-python-0.1.1/src/beeize/storages/kv_store.py
+-rw-r--r--   0 zhaoyang   (501) staff       (20)     5203 2024-04-27 11:41:19.000000 beeize-sdk-python-0.1.1/src/beeize/storages/request_queue.py
+-rw-r--r--   0 zhaoyang   (501) staff       (20)        0 2023-11-15 15:27:00.000000 beeize-sdk-python-0.1.1/src/beeize/storages/storage_manager.py
+-rw-r--r--   0 zhaoyang   (501) staff       (20)     2174 2024-04-27 11:35:18.000000 beeize-sdk-python-0.1.1/src/beeize/utils.py
+drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-04-27 11:44:48.620034 beeize-sdk-python-0.1.1/src/beeize_sdk_python.egg-info/
+-rw-r--r--   0 zhaoyang   (501) staff       (20)       97 2024-04-27 11:44:48.000000 beeize-sdk-python-0.1.1/src/beeize_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 zhaoyang   (501) staff       (20)      476 2024-04-27 11:44:48.000000 beeize-sdk-python-0.1.1/src/beeize_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 zhaoyang   (501) staff       (20)        1 2024-04-27 11:44:48.000000 beeize-sdk-python-0.1.1/src/beeize_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 zhaoyang   (501) staff       (20)        7 2024-04-27 11:44:48.000000 beeize-sdk-python-0.1.1/src/beeize_sdk_python.egg-info/top_level.txt
```

### Comparing `beeize-sdk-python-0.1.0/src/beeize/config.py` & `beeize-sdk-python-0.1.1/src/beeize/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# coding=utf-8
 import json
 import os
 import platform
 from typing import Optional, TypeVar, Any
 
 T = TypeVar('T')
```

### Comparing `beeize-sdk-python-0.1.0/src/beeize/scraper.py` & `beeize-sdk-python-0.1.1/src/beeize/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# coding=utf-8
 from typing import Optional, Any
 
 from .config import Configuration
 from .storages import Dataset, RequestQueue, KeyValueStore
 
 
 class Scraper:
```

### Comparing `beeize-sdk-python-0.1.0/src/beeize/storages/dataset.py` & `beeize-sdk-python-0.1.1/src/beeize/storages/dataset.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# coding=utf-8
 import json
 import os
 import threading
 from datetime import datetime, timezone
 from typing import Any, Dict, List, Union, Optional
 
 from ..config import Configuration
@@ -22,41 +23,41 @@
         )
         os.makedirs(self.datasets_path, exist_ok=True)
         self.metadata = self.load_metadata()
 
     def load_metadata(self):
         metadata_path = os.path.join(self.datasets_path, '__metadata__.json')
         if os.path.exists(metadata_path):
-            with open(metadata_path, 'r') as file:
+            with open(metadata_path, 'r', encoding='utf-8', errors='ignore') as file:
                 return json.load(file)
         return {
             'id': self._id,
             'itemCount': 0,
             'accessedAt': None,
             'createdAt': datetime.now(timezone.utc).isoformat(),
             'modifiedAt': None
         }
 
     def update_metadata(self):
         metadata_path = os.path.join(self.datasets_path, '__metadata__.json')
-        with open(metadata_path, 'w') as file:
+        with open(metadata_path, 'w', encoding='utf-8', errors='ignore') as file:
             json.dump(self.metadata, file, indent=4, ensure_ascii=False)
             file.flush()
             os.fsync(file.fileno())
 
     def push_data(self, data: Any) -> None:
         if not isinstance(data, (dict, list, str, int, float, bool, type(None))):
             raise ValueError("Data is not JSON serializable")
 
         with self._lock:
             try:
                 next_file_number = self.get_next_file_number_with_lock()
                 file_name = f"{str(next_file_number).zfill(9)}.json"
                 file_path = os.path.join(self.datasets_path, file_name)
-                with open(file_path, 'w') as file:
+                with open(file_path, 'w', encoding='utf-8', errors='ignore') as file:
                     json.dump(data, file, indent=4, ensure_ascii=False)
                     file.flush()
                     os.fsync(file.fileno())
                 self.metadata['itemCount'] += 1
                 self.metadata['accessedAt'] = datetime.now(timezone.utc).isoformat()
                 self.metadata['modifiedAt'] = datetime.now(timezone.utc).isoformat()
                 self.update_metadata()  # 保存元数据更改
```

### Comparing `beeize-sdk-python-0.1.0/src/beeize/storages/kv_store.py` & `beeize-sdk-python-0.1.1/src/beeize/storages/kv_store.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# coding=utf-8
 import io
 import json
 import os
 import threading
 from datetime import datetime, timezone
 from typing import Optional, Union, TypeVar
 
@@ -23,15 +24,15 @@
         )
         os.makedirs(self.kv_store_path, exist_ok=True)
         self.metadata = self.load_metadata()
 
     def load_metadata(self):
         metadata_path = os.path.join(self.kv_store_path, '__metadata__.json')
         if os.path.exists(metadata_path):
-            with open(metadata_path, 'r') as file:
+            with open(metadata_path, 'r', encoding='utf-8', errors='ignore') as file:
                 return json.load(file)
         return {
             'id': self._id,
             'createdAt': datetime.now(timezone.utc).isoformat(),
             'modifiedAt': datetime.now(timezone.utc).isoformat(),
             'accessedAt': None
         }
@@ -39,15 +40,15 @@
     def update_metadata(self, accessed=False):
         now = datetime.now(timezone.utc).isoformat()
         self.metadata['itemCount'] = self.metadata.get('itemCount', 0) + 1
         if accessed:
             self.metadata['accessedAt'] = now
         else:
             self.metadata['modifiedAt'] = now
-        with open(os.path.join(self.kv_store_path, '__metadata__.json'), 'w') as f:
+        with open(os.path.join(self.kv_store_path, '__metadata__.json'), 'w', encoding='utf-8', errors='ignore') as f:
             json.dump(self.metadata, f, indent=4)
             f.flush()
             os.fsync(f.fileno())
 
     def set_value(self, key: str, value: Union[str, bytes, dict, list], extension: Optional[str] = None) -> None:
         with self._lock:
             extension = extension or self._determine_extension(value)
@@ -61,26 +62,26 @@
                 'key': key,
                 'contentType': content_type,
                 'extension': extension,
                 'filename': filename,
                 'size': os.path.getsize(data_file_path),
             }
             file_path = os.path.join(self.kv_store_path, f'{key}.__metadata__.json')
-            with open(file_path, 'w') as f:
+            with open(file_path, 'w', encoding='utf-8', errors='ignore') as f:
                 json.dump(metadata, f, ensure_ascii=False, indent=4)
                 f.flush()
                 os.fsync(f.fileno())
             self.update_metadata()
 
     def get_value(self, key: str) -> Optional[Union[str, bytes, dict, list]]:
         metadata_file_path = os.path.join(self.kv_store_path, f'{key}.__metadata__.json')
         if not os.path.exists(metadata_file_path):
             return None
 
-        with open(metadata_file_path, 'r') as f:
+        with open(metadata_file_path, 'r', encoding='utf-8', errors='ignore') as f:
             metadata = json.load(f)
 
         data_file_path = os.path.join(self.kv_store_path, metadata['filename'])
         self.update_metadata(accessed=True)
         return self._read_data(data_file_path, metadata['contentType'])
 
     @staticmethod
@@ -131,29 +132,29 @@
             return 'application/octet-stream'
         else:
             raise ValueError("Unsupported data type for KeyValueStore")
 
     @staticmethod
     def _write_data(value, file_path: str, content_type: str) -> None:
         if content_type == 'application/json; charset=utf-8':
-            with open(file_path, 'w') as f:
+            with open(file_path, 'w', encoding='utf-8', errors='ignore') as f:
                 json.dump(value, f, ensure_ascii=False, indent=4)
                 f.flush()
                 os.fsync(f.fileno())
         elif content_type in ['text/plain; charset=utf-8', 'application/octet-stream']:
             mode = 'w' if isinstance(value, str) else 'wb'
-            with open(file_path, mode) as f:
+            with open(file_path, mode, errors='ignore') as f:
                 f.write(value)
                 f.flush()
                 os.fsync(f.fileno())
 
     @staticmethod
     def _read_data(file_path: str, content_type: str) -> Union[str, bytes, dict, list]:
         if content_type == 'application/json; charset=utf-8':
-            with open(file_path, 'r') as f:
+            with open(file_path, 'r', encoding='utf-8', errors='ignore') as f:
                 return json.load(f)
         elif content_type == 'text/plain; charset=utf-8':
-            with open(file_path, 'r') as f:
+            with open(file_path, 'r', encoding='utf-8', errors='ignore') as f:
                 return f.read()
         elif content_type == 'application/octet-stream':
             with open(file_path, 'rb') as f:
                 return f.read()
```

### Comparing `beeize-sdk-python-0.1.0/src/beeize/storages/request_queue.py` & `beeize-sdk-python-0.1.1/src/beeize/storages/request_queue.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# coding=utf-8
 import json
 import os
 import threading
 from datetime import datetime, timezone
 from typing import Dict, Optional
 
 from ..config import Configuration
@@ -25,23 +26,23 @@
         self._total_count = 0
         self._last_activity = None
         self.metadata = self.load_metadata()
 
     def load_metadata(self):
         for filename in os.listdir(self.request_queues_path):
             if filename.endswith('.json') and not filename.startswith('__'):
-                with open(os.path.join(self.request_queues_path, filename), 'r') as f:
+                with open(os.path.join(self.request_queues_path, filename), 'r', encoding='utf-8', errors='ignore') as f:
                     request = json.load(f)
                     if request.get('status', '') != 'handled':
                         self._queue.append(request)
                     self._requests_cache[request['requestId']] = request
 
         metadata_path = os.path.join(self.request_queues_path, '__metadata__.json')
         if os.path.exists(metadata_path):
-            with open(metadata_path, 'r') as file:
+            with open(metadata_path, 'r', encoding='utf-8', errors='ignore') as file:
                 metadata = json.load(file)
                 self._total_count = metadata.get('totalCount', 0)
                 self._handled_count = metadata.get('handledCount', 0)
                 return metadata
         return {
             'id': self._id,
             'handledCount': 0,
@@ -56,15 +57,15 @@
             'id': self._id,
             'handledCount': self._handled_count,
             'totalCount': self._total_count,
             'accessedAt': datetime.now(timezone.utc).isoformat(),
             'createdAt': self._last_activity.isoformat() if self._last_activity else None,
             'modifiedAt': datetime.now(timezone.utc).isoformat()
         }
-        with open(os.path.join(self.request_queues_path, '__metadata__.json'), 'w') as f:
+        with open(os.path.join(self.request_queues_path, '__metadata__.json'), 'w', encoding='utf-8', errors='ignore') as f:
             json.dump(metadata, f, indent=4)
             f.flush()
             os.fsync(f.fileno())
 
     def add_request(self, request: Dict, *, forefront: bool = False) -> Dict:
         with self._lock:
             self._last_activity = datetime.now(timezone.utc)
@@ -78,15 +79,15 @@
 
             if request_id in self._requests_cache:
                 return self._requests_cache[request_id]
 
             self._queue.insert(0, request) if forefront else self._queue.append(request)
             self._requests_cache[request_id] = request
             self._total_count += 1
-            with open(os.path.join(self.request_queues_path, f'{request_id}.json'), 'w') as f:
+            with open(os.path.join(self.request_queues_path, f'{request_id}.json'), 'w', encoding='utf-8', errors='ignore') as f:
                 json.dump(request, f, indent=4)
                 f.flush()
                 os.fsync(f.fileno())
             self.update_metadata()
             return request
 
     def get_request(self, request_id: str) -> Optional[Dict]:
@@ -102,15 +103,15 @@
 
     def mark_request_as_handled(self, request: Dict):
         with self._lock:
             request_id = request.get('requestId')
             if request_id in self._requests_cache:
                 self._requests_cache[request_id]['status'] = 'handled'
                 self._handled_count += 1
-                with open(os.path.join(self.request_queues_path, f'{request_id}.json'), 'w') as f:
+                with open(os.path.join(self.request_queues_path, f'{request_id}.json'), 'w', encoding='utf-8', errors='ignore') as f:
                     json.dump(self._requests_cache[request_id], f, indent=4)
                     f.flush()
                     os.fsync(f.fileno())
                 self.update_metadata()
 
     def reclaim_request(self, request: Dict):
         with self._lock:
```

### Comparing `beeize-sdk-python-0.1.0/src/beeize/utils.py` & `beeize-sdk-python-0.1.1/src/beeize/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# coding=utf-8
 import base64
 import hashlib
 import io
 import json
 import re
 from typing import Any, TypeVar
```

