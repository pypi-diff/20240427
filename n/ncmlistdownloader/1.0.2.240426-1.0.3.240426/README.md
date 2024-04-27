# Comparing `tmp/ncmlistdownloader-1.0.2.240426.tar.gz` & `tmp/ncmlistdownloader-1.0.3.240426.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncmlistdownloader-1.0.2.240426.tar", last modified: Fri Apr 26 07:24:08 2024, max compression
+gzip compressed data, was "ncmlistdownloader-1.0.3.240426.tar", last modified: Fri Apr 26 09:45:20 2024, max compression
```

## Comparing `ncmlistdownloader-1.0.2.240426.tar` & `ncmlistdownloader-1.0.3.240426.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 07:24:08.812514 ncmlistdownloader-1.0.2.240426/
--rw-rw-rw-   0        0        0    35181 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.2.240426/LICENSE
--rw-rw-rw-   0        0        0     1409 2024-04-26 07:24:08.812514 ncmlistdownloader-1.0.2.240426/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-26 07:24:08.780915 ncmlistdownloader-1.0.2.240426/cmd/
--rw-rw-rw-   0        0        0     1736 2024-04-25 10:28:31.000000 ncmlistdownloader-1.0.2.240426/cmd/__init__.py
--rw-rw-rw-   0        0        0      653 2024-04-25 14:23:37.000000 ncmlistdownloader-1.0.2.240426/cmd/common.py
--rw-rw-rw-   0        0        0     1661 2024-04-25 14:30:46.000000 ncmlistdownloader-1.0.2.240426/cmd/download.py
--rw-rw-rw-   0        0        0     2501 2024-04-22 14:56:53.000000 ncmlistdownloader-1.0.2.240426/cmd/find_from_id.py
--rw-rw-rw-   0        0        0     1664 2024-04-25 10:31:47.000000 ncmlistdownloader-1.0.2.240426/cmd/json_io.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:24:08.782515 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/
--rw-rw-rw-   0        0        0     1232 2024-04-26 07:19:53.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:24:08.802026 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/common/
--rw-rw-rw-   0        0        0     2866 2024-04-26 07:14:57.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/common/__init__.py
--rw-rw-rw-   0        0        0     2325 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/common/encode_sec_key.py
--rw-rw-rw-   0        0        0     2258 2024-04-26 07:22:12.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/common/global_args.py
--rw-rw-rw-   0        0        0     1784 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/common/thread_test.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:24:08.803346 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/downloader/
--rw-rw-rw-   0        0        0     6526 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:24:08.805342 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/editer/
--rw-rw-rw-   0        0        0     3929 2024-04-26 07:14:43.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/editer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:24:08.806321 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/playlist/
--rw-rw-rw-   0        0        0     2323 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/playlist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:24:08.807339 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/song/
--rw-rw-rw-   0        0        0     8428 2024-04-26 07:14:17.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/song/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:24:08.810311 ncmlistdownloader-1.0.2.240426/ncmlistdownloader.egg-info/
--rw-rw-rw-   0        0        0     1409 2024-04-26 07:24:08.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      687 2024-04-26 07:24:08.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 07:24:08.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-26 07:24:08.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-04-26 07:24:08.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-04-26 07:24:08.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 07:24:08.812514 ncmlistdownloader-1.0.2.240426/setup.cfg
--rw-rw-rw-   0        0        0     1756 2024-04-26 07:23:52.000000 ncmlistdownloader-1.0.2.240426/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:45:20.323953 ncmlistdownloader-1.0.3.240426/
+-rw-rw-rw-   0        0        0    35181 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.3.240426/LICENSE
+-rw-rw-rw-   0        0        0     1409 2024-04-26 09:45:20.321254 ncmlistdownloader-1.0.3.240426/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-26 09:45:20.270537 ncmlistdownloader-1.0.3.240426/ncmlistdownloader/
+-rw-rw-rw-   0        0        0     1313 2024-04-26 09:40:50.000000 ncmlistdownloader-1.0.3.240426/ncmlistdownloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:45:20.296833 ncmlistdownloader-1.0.3.240426/ncmlistdownloader/cmd/
+-rw-rw-rw-   0        0        0     1736 2024-04-25 10:28:31.000000 ncmlistdownloader-1.0.3.240426/ncmlistdownloader/cmd/__init__.py
+-rw-rw-rw-   0        0        0      653 2024-04-25 14:23:37.000000 ncmlistdownloader-1.0.3.240426/ncmlistdownloader/cmd/common.py
+-rw-rw-rw-   0        0        0     1661 2024-04-25 14:30:46.000000 ncmlistdownloader-1.0.3.240426/ncmlistdownloader/cmd/download.py
+-rw-rw-rw-   0        0        0     2501 2024-04-22 14:56:53.000000 ncmlistdownloader-1.0.3.240426/ncmlistdownloader/cmd/find_from_id.py
+-rw-rw-rw-   0        0        0     1664 2024-04-25 10:31:47.000000 ncmlistdownloader-1.0.3.240426/ncmlistdownloader/cmd/json_io.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:45:20.305178 ncmlistdownloader-1.0.3.240426/ncmlistdownloader/common/
+-rw-rw-rw-   0        0        0     2866 2024-04-26 07:14:57.000000 ncmlistdownloader-1.0.3.240426/ncmlistdownloader/common/__init__.py
+-rw-rw-rw-   0        0        0     2325 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.3.240426/ncmlistdownloader/common/encode_sec_key.py
+-rw-rw-rw-   0        0        0     2300 2024-04-26 09:37:52.000000 ncmlistdownloader-1.0.3.240426/ncmlistdownloader/common/global_args.py
+-rw-rw-rw-   0        0        0     1784 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.3.240426/ncmlistdownloader/common/thread_test.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:45:20.307477 ncmlistdownloader-1.0.3.240426/ncmlistdownloader/downloader/
+-rw-rw-rw-   0        0        0     6526 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.3.240426/ncmlistdownloader/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:45:20.313459 ncmlistdownloader-1.0.3.240426/ncmlistdownloader/editer/
+-rw-rw-rw-   0        0        0     3929 2024-04-26 07:14:43.000000 ncmlistdownloader-1.0.3.240426/ncmlistdownloader/editer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:45:20.315455 ncmlistdownloader-1.0.3.240426/ncmlistdownloader/playlist/
+-rw-rw-rw-   0        0        0     2388 2024-04-26 09:44:03.000000 ncmlistdownloader-1.0.3.240426/ncmlistdownloader/playlist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:45:20.316451 ncmlistdownloader-1.0.3.240426/ncmlistdownloader/song/
+-rw-rw-rw-   0        0        0     8428 2024-04-26 07:14:17.000000 ncmlistdownloader-1.0.3.240426/ncmlistdownloader/song/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:45:20.320272 ncmlistdownloader-1.0.3.240426/ncmlistdownloader.egg-info/
+-rw-rw-rw-   0        0        0     1409 2024-04-26 09:45:20.000000 ncmlistdownloader-1.0.3.240426/ncmlistdownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      777 2024-04-26 09:45:20.000000 ncmlistdownloader-1.0.3.240426/ncmlistdownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 09:45:20.000000 ncmlistdownloader-1.0.3.240426/ncmlistdownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-26 09:45:20.000000 ncmlistdownloader-1.0.3.240426/ncmlistdownloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-04-26 09:45:20.000000 ncmlistdownloader-1.0.3.240426/ncmlistdownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-26 09:45:20.000000 ncmlistdownloader-1.0.3.240426/ncmlistdownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 09:45:20.323953 ncmlistdownloader-1.0.3.240426/setup.cfg
+-rw-rw-rw-   0        0        0     1827 2024-04-26 09:45:12.000000 ncmlistdownloader-1.0.3.240426/setup.py
```

### Comparing `ncmlistdownloader-1.0.2.240426/LICENSE` & `ncmlistdownloader-1.0.3.240426/LICENSE`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.2.240426/PKG-INFO` & `ncmlistdownloader-1.0.3.240426/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.2.240426
+Version: 1.0.3.240426
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncmlistdownloader-1.0.2.240426/cmd/__init__.py` & `ncmlistdownloader-1.0.3.240426/ncmlistdownloader/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.2.240426/cmd/common.py` & `ncmlistdownloader-1.0.3.240426/ncmlistdownloader/cmd/common.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.2.240426/cmd/download.py` & `ncmlistdownloader-1.0.3.240426/ncmlistdownloader/cmd/download.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.2.240426/cmd/find_from_id.py` & `ncmlistdownloader-1.0.3.240426/ncmlistdownloader/cmd/find_from_id.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.2.240426/cmd/json_io.py` & `ncmlistdownloader-1.0.3.240426/ncmlistdownloader/cmd/json_io.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.2.240426/ncmlistdownloader/__init__.py` & `ncmlistdownloader-1.0.3.240426/ncmlistdownloader/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 '''
 ncmlistdownloader/__init__.py
-Core.Ver.1.0.2.240426
+Core.Ver.1.0.3.240426
 Author: CooooldWind_
 '''
 from pathlib import Path
+import time
 from ncmlistdownloader.playlist import *
 from ncmlistdownloader.common import *
 from ncmlistdownloader.common.global_args import *
 
 def main():
     for i in CMD_START_WORDS:
         print(i)
@@ -24,15 +25,17 @@
         fnf = '$title$ - $artist$'
     if d[-1] != '/' and d[-1] != '\\':
         d += '/'
     d = d.replace('\\', '/')
     auto_mkdir(d)
     for i in p.track:
         i.filename_format = d + fnf
-    p.get_detail_info()
+    p.multiprocessing_get_detail()
+    while p.mp_succeed == False:
+        time.sleep(1)
     for i in p.track:
         music_filename = i.song_download()
         if music_filename == -1:
             print(i.title + ' cannot download.')
             continue
         i.cover_download()
         i.lyric_get()
```

### Comparing `ncmlistdownloader-1.0.2.240426/ncmlistdownloader/common/__init__.py` & `ncmlistdownloader-1.0.3.240426/ncmlistdownloader/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.2.240426/ncmlistdownloader/common/encode_sec_key.py` & `ncmlistdownloader-1.0.3.240426/ncmlistdownloader/common/encode_sec_key.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.2.240426/ncmlistdownloader/common/global_args.py` & `ncmlistdownloader-1.0.3.240426/ncmlistdownloader/common/global_args.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 list_downloader/global_args.py
-Core.Ver.1.0.0.240410a1
+Core.Ver.1.0.3.240426
 Author: CooooldWind_, 是青旨啊
 '''
 FUNC_F_PART = [
   "00e0b509f6259df8642dbc35662901477df22677ec152b5ff68ace615bb7",
   "b725152b3ab17a876aea8a5aa76d2e417629ec4ee341f56135fccf695280",
   "104e0312ecbda92557c93870114af6c9d05c4f7f0c3685b7a46bee255932",
   "575cce10b424d813cfe4875d3e82047b97ddef52741d546b8e289dc6935b",
@@ -37,16 +37,17 @@
 SEC_KEY = json_file['SEC_KEY']
 PLAYLIST_API = json_file['PLAYLIST_API']
 SONG_INFO_API = json_file['SONG_INFO_API']
 SONG_FILE_API = json_file['SONG_FILE_API']
 SONG_FILE_API_2 = json_file['SONG_FILE_API_2']
 SEARCH_API = "https://music.163.com/weapi/cloudsearch/get/web?csrf_token="
 LYRIC_API = json_file['LYRIC_API']
-CMD_VERSION = 'Ver.1.0.2.24042601'
-CORE_VERSION = 'Core.Ver.1.0.2.240426'
+CMD_VERSION = 'Ver.1.0.3.240426'
+CORE_VERSION_SETUP = '1.0.3.240426'
+CORE_VERSION = 'Core.Ver.' + CORE_VERSION_SETUP
 CMD_START_WORDS = [
     f"163ListDownloader CMD Ver - {CMD_VERSION}",
     "Made by CooooldWind_",
     "Here's the Gitee/GitHub Page, click a star if you like it~",
     "Gitee: https://gitee.com/CooooldWind/163ListDownloader_NexT/issues",
     "GitHub: https://github.com/CooooldWind/163ListDownloader_NexT/issues",
 ]
```

### Comparing `ncmlistdownloader-1.0.2.240426/ncmlistdownloader/common/thread_test.py` & `ncmlistdownloader-1.0.3.240426/ncmlistdownloader/common/thread_test.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.2.240426/ncmlistdownloader/downloader/__init__.py` & `ncmlistdownloader-1.0.3.240426/ncmlistdownloader/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.2.240426/ncmlistdownloader/editer/__init__.py` & `ncmlistdownloader-1.0.3.240426/ncmlistdownloader/editer/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.2.240426/ncmlistdownloader/playlist/__init__.py` & `ncmlistdownloader-1.0.3.240426/ncmlistdownloader/playlist/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 ncmlistdownloader/playlist/__init__.py
-Core.Ver.1.0.1.240419a1
+Core.Ver.1.0.3.240426
 Author: CooooldWind_
 '''
 from ncmlistdownloader.common import *
 from ncmlistdownloader.common.encode_sec_key import *
 from ncmlistdownloader.common.global_args import *
 from ncmlistdownloader.song import *
 import threading
@@ -17,14 +17,15 @@
         self.track: list[Song] = []
         self.creator_id = ""
         self.raw_info = {}
         self.track_count = int(0)
         self.creator = ""
         self.track_id = []
         self.title = ""
+        self.mp_succeed = False
 
     def get_info(self, cookies = None):
         self.raw_info = NeteaseParams(url = PLAYLIST_API,
                                       encode_data = {
                                           'csrf_token': '',
                                           'id': self.id,
                                       }).get_resource(cookies = cookies)
@@ -44,14 +45,15 @@
         threads: list[threading.Thread] = []
         for i in self.track:
             thread = threading.Thread(target = i.multi_get_info)
             thread.start()
             threads.append(thread)
         for i in threads:
             i.join()
+        self.mp_succeed = True
 
     def auto_get_info(self, cookies = dict()):
         if self.get_info(cookies = cookies) != -1:
             self.get_detail_info()
         else: return -1
 
     def done_sum(self):
@@ -59,8 +61,8 @@
         for i in self.track:
             if i.is_get == True:
                 count += 1
         return count
     
     def multiprocessing_get_detail(self):
         p = threading.Thread(target = self.get_detail_info)
-        p.start()
+        p.start()
```

### Comparing `ncmlistdownloader-1.0.2.240426/ncmlistdownloader/song/__init__.py` & `ncmlistdownloader-1.0.3.240426/ncmlistdownloader/song/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.2.240426/ncmlistdownloader.egg-info/PKG-INFO` & `ncmlistdownloader-1.0.3.240426/ncmlistdownloader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.2.240426
+Version: 1.0.3.240426
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncmlistdownloader-1.0.2.240426/ncmlistdownloader.egg-info/SOURCES.txt` & `ncmlistdownloader-1.0.3.240426/ncmlistdownloader.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 LICENSE
 setup.py
-cmd/__init__.py
-cmd/common.py
-cmd/download.py
-cmd/find_from_id.py
-cmd/json_io.py
 ncmlistdownloader/__init__.py
 ncmlistdownloader.egg-info/PKG-INFO
 ncmlistdownloader.egg-info/SOURCES.txt
 ncmlistdownloader.egg-info/dependency_links.txt
 ncmlistdownloader.egg-info/entry_points.txt
 ncmlistdownloader.egg-info/requires.txt
 ncmlistdownloader.egg-info/top_level.txt
+ncmlistdownloader/cmd/__init__.py
+ncmlistdownloader/cmd/common.py
+ncmlistdownloader/cmd/download.py
+ncmlistdownloader/cmd/find_from_id.py
+ncmlistdownloader/cmd/json_io.py
 ncmlistdownloader/common/__init__.py
 ncmlistdownloader/common/encode_sec_key.py
 ncmlistdownloader/common/global_args.py
 ncmlistdownloader/common/thread_test.py
 ncmlistdownloader/downloader/__init__.py
 ncmlistdownloader/editer/__init__.py
 ncmlistdownloader/playlist/__init__.py
```

### Comparing `ncmlistdownloader-1.0.2.240426/setup.py` & `ncmlistdownloader-1.0.3.240426/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from setuptools import setup, find_packages
+# from ncmlistdownloader.common.global_args import CORE_VERSION_SETUP
 setup(
     classifiers = [
         # 发展时期
         # 'Development Status :: 3 - Alpha',
         # 'Development Status :: 4 - Beta',
         'Development Status :: 5 - Production/Stable',
         # 开发的目标用户
@@ -26,15 +27,15 @@
 		'Programming Language :: Python :: 3.8',
 		'Programming Language :: Python :: 3.9',
 		'Programming Language :: Python :: 3.10',
 		'Programming Language :: Python :: 3.11',
 		'Programming Language :: Python :: 3.12',
     ],
     name = 'ncmlistdownloader',
-    version = "1.0.2.240426",
+    version = "1.0.3.240426",
     description = '获取网易云音乐歌单数据，下载音乐，主动添加元信息。',
     author = 'CooooldWind_',
     url = 'https://gitee.com/Cooooldwind/163ListDownloader_NexT',
     packages = find_packages(),
     install_requires = ['pycryptodome','pillow','mutagen','requests',],
     entry_points = {'console_scripts': ['ncmlistdownloader = ncmlistdownloader.__init__:main']},
 )
```

