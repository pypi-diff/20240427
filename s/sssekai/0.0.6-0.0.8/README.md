# Comparing `tmp/sssekai-0.0.6.tar.gz` & `tmp/sssekai-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sssekai-0.0.6.tar", last modified: Sat Feb 17 12:38:42 2024, max compression
+gzip compressed data, was "sssekai-0.0.8.tar", last modified: Sat Apr 27 08:13:05 2024, max compression
```

## Comparing `sssekai-0.0.6.tar` & `sssekai-0.0.8.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 12:38:42.957343 sssekai-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-02-17 12:38:42.957343 sssekai-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-02-17 12:38:30.000000 sssekai-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-17 12:38:42.957343 sssekai-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-17 12:38:30.000000 sssekai-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 12:38:42.953343 sssekai-0.0.6/sssekai/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-17 12:38:30.000000 sssekai-0.0.6/sssekai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-02-17 12:38:30.000000 sssekai-0.0.6/sssekai/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 12:38:42.953343 sssekai-0.0.6/sssekai/abcache/
--rw-r--r--   0 runner    (1001) docker     (127)    12889 2024-02-17 12:38:30.000000 sssekai-0.0.6/sssekai/abcache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 12:38:42.953343 sssekai-0.0.6/sssekai/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-02-17 12:38:30.000000 sssekai-0.0.6/sssekai/crypto/APIManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-17 12:38:30.000000 sssekai-0.0.6/sssekai/crypto/AssetBundle.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-17 12:38:30.000000 sssekai-0.0.6/sssekai/crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 12:38:42.957343 sssekai-0.0.6/sssekai/entrypoint/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-17 12:38:30.000000 sssekai-0.0.6/sssekai/entrypoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-02-17 12:38:30.000000 sssekai-0.0.6/sssekai/entrypoint/abcache.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-17 12:38:30.000000 sssekai-0.0.6/sssekai/entrypoint/abdecrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-02-17 12:38:30.000000 sssekai-0.0.6/sssekai/entrypoint/apidecrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-02-17 12:38:30.000000 sssekai-0.0.6/sssekai/entrypoint/live2dextract.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-02-17 12:38:30.000000 sssekai-0.0.6/sssekai/entrypoint/mitm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-02-17 12:38:30.000000 sssekai-0.0.6/sssekai/entrypoint/spineextract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-02-17 12:38:30.000000 sssekai-0.0.6/sssekai/entrypoint/usmdemux.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 12:38:42.957343 sssekai-0.0.6/sssekai/fmt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-17 12:38:30.000000 sssekai-0.0.6/sssekai/fmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-02-17 12:38:30.000000 sssekai-0.0.6/sssekai/fmt/moc3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 12:38:42.957343 sssekai-0.0.6/sssekai/unity/
--rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-02-17 12:38:30.000000 sssekai-0.0.6/sssekai/unity/AnimationClip.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-02-17 12:38:30.000000 sssekai-0.0.6/sssekai/unity/AssetBundle.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-17 12:38:30.000000 sssekai-0.0.6/sssekai/unity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 12:38:42.957343 sssekai-0.0.6/sssekai/unity/constant/
--rw-r--r--   0 runner    (1001) docker     (127)    47730 2024-02-17 12:38:30.000000 sssekai-0.0.6/sssekai/unity/constant/SekaiLive2DPathNames.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-17 12:38:30.000000 sssekai-0.0.6/sssekai/unity/constant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 12:38:42.957343 sssekai-0.0.6/sssekai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-02-17 12:38:42.000000 sssekai-0.0.6/sssekai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-02-17 12:38:42.000000 sssekai-0.0.6/sssekai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-17 12:38:42.000000 sssekai-0.0.6/sssekai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-17 12:38:42.000000 sssekai-0.0.6/sssekai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-17 12:38:42.000000 sssekai-0.0.6/sssekai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-17 12:38:42.000000 sssekai-0.0.6/sssekai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:05.016878 sssekai-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-27 08:13:05.016878 sssekai-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-27 08:13:00.000000 sssekai-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 08:13:05.016878 sssekai-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-27 08:13:00.000000 sssekai-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:05.012878 sssekai-0.0.8/sssekai/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:05.012878 sssekai-0.0.8/sssekai/abcache/
+-rw-r--r--   0 runner    (1001) docker     (127)    14490 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/abcache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:05.012878 sssekai-0.0.8/sssekai/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/crypto/APIManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/crypto/AssetBundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:05.012878 sssekai-0.0.8/sssekai/entrypoint/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/entrypoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/entrypoint/abcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/entrypoint/abdecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/entrypoint/apidecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/entrypoint/live2dextract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/entrypoint/mitm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/entrypoint/mvdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/entrypoint/spineextract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/entrypoint/usmdemux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:05.012878 sssekai-0.0.8/sssekai/fmt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/fmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/fmt/moc3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:05.016878 sssekai-0.0.8/sssekai/unity/
+-rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/unity/AnimationClip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/unity/AssetBundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/unity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:05.016878 sssekai-0.0.8/sssekai/unity/constant/
+-rw-r--r--   0 runner    (1001) docker     (127)    60945 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/unity/constant/SekaiLive2DPathNames.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/unity/constant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:05.016878 sssekai-0.0.8/sssekai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-27 08:13:05.000000 sssekai-0.0.8/sssekai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-27 08:13:05.000000 sssekai-0.0.8/sssekai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 08:13:05.000000 sssekai-0.0.8/sssekai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-27 08:13:05.000000 sssekai-0.0.8/sssekai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 08:13:05.000000 sssekai-0.0.8/sssekai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-27 08:13:05.000000 sssekai-0.0.8/sssekai.egg-info/top_level.txt
```

### Comparing `sssekai-0.0.6/PKG-INFO` & `sssekai-0.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sssekai
-Version: 0.0.6
+Version: 0.0.8
 Home-page: https://github.com/mos9527/sssekai
 Author: greats3an
 Author-email: greats3an@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -40,15 +40,16 @@
                             These can be found at /sdcard/Android/data/com.hermes.mk.asia/files/data/
         usmdemux            Demux Sekai USM Video in a AssetBundle
         abcache             Sekai AssetBundle local cache
                             Downloads/Updates *ALL* PJSK JP assets to local devices.
                             NOTE: The assets can take quite a lot of space (est. 42.5GB for app version 3.3.1) so be prepared
                             NOTE: The AssetBundles *cached* are NOT OBFUSCATED. They can be used as is by various Unity ripping tools (and sssekai by extension)
                                   that supports stripped Unity version (should be 2020.3.21f1. the version is ripped).
-        live2dextract       Extract Sekai Live2D Models in a AssetBundle
+        spineextract        Extract Sekai Spine (Esoteric Spine2D) Models in a AssetBundle
+        mvdata              Query Sekai MV data from AssetBundle
         mitm                Run Sekai API MITM proxy (WIP)
 
 # Usage
 Refer to the Wiki!
 https://github.com/mos9527/sssekai/wiki （附带简中）
 
 # See Also
```

### Comparing `sssekai-0.0.6/README.md` & `sssekai-0.0.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -24,15 +24,16 @@
                             These can be found at /sdcard/Android/data/com.hermes.mk.asia/files/data/
         usmdemux            Demux Sekai USM Video in a AssetBundle
         abcache             Sekai AssetBundle local cache
                             Downloads/Updates *ALL* PJSK JP assets to local devices.
                             NOTE: The assets can take quite a lot of space (est. 42.5GB for app version 3.3.1) so be prepared
                             NOTE: The AssetBundles *cached* are NOT OBFUSCATED. They can be used as is by various Unity ripping tools (and sssekai by extension)
                                   that supports stripped Unity version (should be 2020.3.21f1. the version is ripped).
-        live2dextract       Extract Sekai Live2D Models in a AssetBundle
+        spineextract        Extract Sekai Spine (Esoteric Spine2D) Models in a AssetBundle
+        mvdata              Query Sekai MV data from AssetBundle
         mitm                Run Sekai API MITM proxy (WIP)
 
 # Usage
 Refer to the Wiki!
 https://github.com/mos9527/sssekai/wiki （附带简中）
 
 # See Also
```

### Comparing `sssekai-0.0.6/setup.py` & `sssekai-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.0.6/sssekai/__main__.py` & `sssekai-0.0.8/sssekai/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,35 @@
 import codecs
 import sys, os
 import argparse
 from sssekai.entrypoint.apidecrypt import main_apidecrypt
 from sssekai.entrypoint.abdecrypt import main_abdecrypt
 from sssekai.entrypoint.mitm import main_mitm
+from sssekai.entrypoint.mvdata import main_mvdata
 from sssekai.entrypoint.usmdemux import main_usmdemux
 from sssekai.entrypoint.abcache import main_abcache
 from sssekai.entrypoint.live2dextract import main_live2dextract
 from sssekai.entrypoint.spineextract import main_spineextract
 from sssekai.unity import SEKAI_UNITY_VERSION
-from sssekai.abcache import DEFAULT_CACHE_DIR, DEFAULT_SEKAI_VERSION, DEFAULT_SEKAI_PLATFORM
+from sssekai.abcache import DEFAULT_CACHE_DIR, DEFAULT_SEKAI_LATEST_VERSION, DEFAULT_SEKAI_PLATFORM
 def __main__():
     from tqdm.std import tqdm as tqdm_c
     class SemaphoreStdout:
         @staticmethod
         def write(__s):
             # Blocks tqdm's output until write on this stream is done
             # Solves cases where progress bars gets re-rendered when logs
             # spews out too fast
             with tqdm_c.external_write_mode(file=sys.stdout, nolock=False):
                 return sys.stdout.write(__s)
-    import coloredlogs
-    from logging import basicConfig
-    coloredlogs.install(
-            level='INFO',
-            fmt="%(asctime)s %(name)s [%(levelname).4s] %(message)s",
-            isatty=True,
-            stream=SemaphoreStdout
-        )
-    basicConfig(
-        level='INFO', format="[%(levelname).4s] %(name)s %(message)s", stream=SemaphoreStdout
-    )
     parser = argparse.ArgumentParser(description='''SSSekai Proejct SEKAI feat. Hatsune Miku (Android) Modding Tools
 Installation:
     pip install git+https://github.com/mos9527/sssekai                                    
 ''', formatter_class=argparse.RawTextHelpFormatter)
+    parser.add_argument('--log-level', type=str, help='logging level (default: %(default)s)', default='INFO', choices=['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'])
     subparsers = parser.add_subparsers(title='subcommands', description='valid subcommands', help='additional help')
     # apidecrypt
     apidecrypt_parser = subparsers.add_parser('apidecrypt', help='''API crypto dumper
 This crypto applies to:
     - API request/response body dumped by packet sniffer (mitmproxy, wireshark, etc.)
     - AssetBundleInfo (can be found at /sdcard/Android/data/com.hermes.mk.asia/files/data/AssetBundleInfo,or see sssekai.abcache)''')
     apidecrypt_parser.add_argument('infile', type=str, help='input dump file')
@@ -60,34 +51,51 @@
     abcache_parser = subparsers.add_parser('abcache', help='''Sekai AssetBundle local cache
 Downloads/Updates *ALL* PJSK JP assets to local devices.
 NOTE: The assets can take quite a lot of space (est. 42.5GB for app version 3.3.1) so be prepared
 NOTE: The AssetBundles *cached* are NOT OBFUSCATED. They can be used as is by various Unity ripping tools (and sssekai by extension)
       that supports stripped Unity version (should be %s. the version is ripped).''' % SEKAI_UNITY_VERSION)
     abcache_parser.add_argument('--cache-dir', type=str, help='cache directory (default: %(default)s)',default=DEFAULT_CACHE_DIR)
     abcache_parser.add_argument('--skip-update',action='store_true',help='skip all updates and use cached assets as is.')
-    abcache_parser.add_argument('--version', type=str, help='PJSK app version (default: %(default)s)', default=DEFAULT_SEKAI_VERSION)
+    abcache_parser.add_argument('--version', type=str, help='PJSK app version (default: %(default)s)', default=DEFAULT_SEKAI_LATEST_VERSION)
     abcache_parser.add_argument('--platform', type=str, help='PJSK app platform (default: %(default)s)', default=DEFAULT_SEKAI_PLATFORM)
     abcache_parser.add_argument('--open', action='store_true',help='open cache directory. this will skip all updates.')
     abcache_parser.set_defaults(func=main_abcache)
     # live2dextract
     live2dextract_parser = subparsers.add_parser('live2dextract', help='''Extract Sekai Live2D Models in a AssetBundle''')
     live2dextract_parser.add_argument('infile', type=str, help='input file')
     live2dextract_parser.add_argument('outdir', type=str, help='output directory')
     live2dextract_parser.add_argument('--no-anim',action='store_true',help='don\'t extract animation clips')
     live2dextract_parser.set_defaults(func=main_live2dextract)
     # spineextract
     spineextract_parser = subparsers.add_parser('spineextract', help='''Extract Sekai Spine (Esoteric Spine2D) Models in a AssetBundle''')
     spineextract_parser.add_argument('infile', type=str, help='input file')
     spineextract_parser.add_argument('outdir', type=str, help='output directory')    
     spineextract_parser.set_defaults(func=main_spineextract)    
+    # mvdata
+    mvdata_parser = subparsers.add_parser('mvdata', help='''Query Sekai MV data from AssetBundle''')
+    mvdata_parser.add_argument('--cache-dir', type=str, help='abcache cache directory (default: %(default)s)',default=DEFAULT_CACHE_DIR)
+    mvdata_parser.add_argument('query', type=str, help='query string. Either MV ID or MV (full) name')
+    mvdata_parser.set_defaults(func=main_mvdata)
     # mitm
     mitm_parser = subparsers.add_parser('mitm', help='Run Sekai API MITM proxy (WIP)')
     mitm_parser.set_defaults(func=main_mitm)
     # parse args
     args = parser.parse_args()
+    # set logging level
+    import coloredlogs
+    from logging import basicConfig
+    coloredlogs.install(
+            level=args.log_level,
+            fmt="%(asctime)s %(name)s [%(levelname).4s] %(message)s",
+            isatty=True,
+            stream=SemaphoreStdout
+        )
+    basicConfig(
+        level=args.log_level, format="[%(levelname).4s] %(name)s %(message)s", stream=SemaphoreStdout
+    )
     if 'func' in args:
         args.func(args)
     else:
         parser.print_help()
 
 
 if __name__ == "__main__":
```

### Comparing `sssekai-0.0.6/sssekai/abcache/__init__.py` & `sssekai-0.0.8/sssekai/abcache/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 from os import path, remove, makedirs, stat
 from typing import List, Mapping
 from dataclasses import dataclass, asdict
 from requests import Session
 from logging import getLogger
-from json import dump, load
 from pathlib import Path
 from concurrent.futures import ThreadPoolExecutor
 logger = getLogger('sssekai.abcache')
 
 from sssekai.crypto.APIManager import decrypt
 from sssekai.crypto.AssetBundle import decrypt_headaer_inplace, SEKAI_AB_MAGIC
-from msgpack import unpackb
+from msgpack import unpackb, dump, load
 from tqdm import tqdm
 DEFAULT_CACHE_DIR = '~/.sssekai/abcache'
-DEFAULT_SEKAI_VERSION = '3.3.1'
+DEFAULT_SEKAI_LATEST_VERSION = 'latest'
 DEFAULT_SEKAI_PLATFORM = 'android'
-
 DOWNLOADER_WORKER_COUNT = 8
-class ThreadpoolDownloader(ThreadPoolExecutor):
+# TODO: These seems to be in pairs?
+DEFAULT_SEKAI_FALLBACK_VERSION = '3.4.1'
+DEFAULT_SEKAI_FALLBACK_APP_HASH = 'a3015fe8-785f-27e1-fb8b-546a23c82c1f'
+
+DEFAULT_FILESIZE_MATCH_RATIO = 1.5
+class SekaiAssetBundleThreadpoolDownloader(ThreadPoolExecutor):
     session : Session
     progress : tqdm
 
     def download(self, url, fname, length):
         RETRIES = 1
         for _ in range(0,RETRIES):
             try:
                 resp = self.session.get(url,stream=True)
                 resp.raise_for_status()
                 makedirs(path.dirname(fname),exist_ok=True)
                 with open(fname, 'wb') as f:
                     magic = next(resp.iter_content(4))
+                    self.progress.update(4)
                     if magic == SEKAI_AB_MAGIC:
                         header = next(resp.iter_content(128))            
                         self.progress.update(128)
                         f.write(decrypt_headaer_inplace(bytearray(header)))
                     else:
                         f.write(magic)                
                     for chunk in resp.iter_content(65536):
@@ -53,38 +57,44 @@
         super().__init__(max_workers=DOWNLOADER_WORKER_COUNT)
 
 class AbCacheConfig:
     app_version : str
     app_platform : str
 
     cache_dir : str # absolute path to cache directory
-    downloader : ThreadpoolDownloader
-    def __init__(self, downloader : ThreadpoolDownloader, cache_dir: str = DEFAULT_CACHE_DIR, version: str = DEFAULT_SEKAI_VERSION, platform : str = DEFAULT_SEKAI_PLATFORM) -> None:
+    downloader : SekaiAssetBundleThreadpoolDownloader
+
+    def __init__(self, downloader : SekaiAssetBundleThreadpoolDownloader, cache_dir: str = DEFAULT_CACHE_DIR, version: str = DEFAULT_SEKAI_LATEST_VERSION, platform : str = DEFAULT_SEKAI_PLATFORM) -> None:
         self.cache_dir = path.expanduser(cache_dir)
         self.cache_dir = path.abspath(self.cache_dir)
         self.downloader = downloader
         self.app_version = version
         self.app_platform = platform
+
 @dataclass
 class AbCacheEntry(dict):
     bundleName: str
     cacheFileName: str
     cacheDirectoryName: str
     hash: str
     category: str
     crc: int
     fileSize:int
     dependencies : List[str]
     paths : List[str]
     isBuiltin : bool
 
     def up_to_date(self, config: AbCacheConfig, other) -> bool:
-        return self.hash == other.hash and self.get_file_exists(config)
-        # HACK: we don't have proper hash checking yet. so we just check if the file exists.
-        # The file size isn't a useful predicate, also. Some files will have incorrect file size (compared to the ab cache report)
+        return (
+            self.hash == other.hash and 
+            self.get_file_exists(config) and 
+            (other.fileSize / max(1,self.get_file_size(config)) < DEFAULT_FILESIZE_MATCH_RATIO)
+        )
+        # HACK: we don't have proper hash checking yet. so we just check if the file exists and
+        # the file size roughly matches
 
     def get_file_size(self, config: AbCacheConfig):
         if self.get_file_exists(config):
             return stat(self.get_file_path(config)).st_size
         else:
             return 0
 
@@ -119,37 +129,45 @@
 class SekaiSystemData:
     serverDate : int
     timezone : str
     profile : str
     maintenanceStatus : str
     appVersions : List[SekaiAppVersion]    
 
-    def get_app_version_by_app(self, app: str) -> SekaiAppVersion | None:
+    def get_app_version_by_app(self, app: str) -> SekaiAppVersion | None:        
         for av in self.appVersions:
             if app in av.appVersion:
                 return av
         return None
     
+    def get_app_version_latest(self):
+        return self.appVersions[-1]
+    
     def list_app_versions(self) -> List[str]:
         return [av.appVersion for av in self.appVersions]
 @dataclass
 class SekaiGameVersionData:
     profile : str
     assetbundleHostHash : str
     domain : str
 class AbCache(Session):    
     config : AbCacheConfig
-    index : AbCacheIndex
     
-    sekai_system_data : SekaiSystemData
-    sekai_gameversion_data : SekaiGameVersionData
+    local_abcache_index : AbCacheIndex  = None
+
+    sekai_abcache_index  : AbCacheIndex = None
+    sekai_system_data : SekaiSystemData  = None
+    sekai_gameversion_data : SekaiGameVersionData  = None
 
     @property
     def SEKAI_APP_VERSION(self): 
-        version = self.sekai_system_data.get_app_version_by_app(self.config.app_version)
+        if self.config.app_version == DEFAULT_SEKAI_LATEST_VERSION:
+            version = self.sekai_system_data.get_app_version_latest()
+        else:
+            version = self.sekai_system_data.get_app_version_by_app(self.config.app_version)
         assert version, "Incorrect app version %s. Please choose from: %s" % (self.config.app_version, ', '.join(self.sekai_system_data.list_app_versions()))
         return version
     @property
     def SEKAI_ASSET_VERSION(self): return self.SEKAI_APP_VERSION.assetVersion
     @property
     def SEKAI_AB_HASH(self): return self.SEKAI_APP_VERSION.assetHash
     @property
@@ -195,101 +213,111 @@
         logger.info('Updating game version data')
         resp = self.get(self.SEKAI_API_GAMEVERSION_ENDPOINT + '/' + self.SEKAI_APP_VERSION.appVersion + '/' + self.SEKAI_APP_VERSION.appHash)
         resp.raise_for_status()
         data = decrypt(resp.content)
         data = unpackb(data)
         self.sekai_gameversion_data = SekaiGameVersionData(**data)
     
-    def download_cache_index(self) -> AbCacheIndex:
-        logger.info('Downloading Asset Bundle Index')
+    def update_abcache_index(self) -> AbCacheIndex:
+        logger.info('Updating Assetbundle index')
         resp = self.get(
             url=self.SEKAI_AB_INFO_ENDPOINT + self.SEKAI_AB_INDEX_PATH
         )
         resp.raise_for_status()
         data = decrypt(resp.content)
         data = unpackb(data)
-        cache = AbCacheIndex(**data)
+        self.sekai_abcache_index = cache = AbCacheIndex(**data)
         for k,v in cache.bundles.items():
-            cache.bundles[k] = AbCacheEntry(**v)
-        return cache
+            cache.bundles[k] = AbCacheEntry(**v)         
 
-    def update_cahce_entry(self, entry : AbCacheEntry, new_entry : AbCacheEntry = None):
+    def list_entry_keys(self) -> List[str]:
+        return self.local_abcache_index.bundles.keys()
+
+    def query_entry(self, bundleName : str) -> AbCacheEntry | None:
+        return self.local_abcache_index.bundles.get(bundleName, None)
+
+    def queue_update_cache_entry(self, entry : AbCacheEntry, new_entry : AbCacheEntry = None):
         if new_entry:
             entry = new_entry
         return self.config.downloader.add_link(
             self.SEKAI_AB_ENDPOINT + self.SEKAI_AB_BASE_PATH + entry.bundleName,
             entry.get_file_path(self.config),
             entry.fileSize
         )
-                
-    def update_cahce_index(self):
-        logger.info('Updating Asset Bundle Index')
-        dl = self.download_cache_index()
-        all_keys = sorted(list({k for k in dl.bundles.keys()}.union({k for k in self.index.bundles.keys()})))
+
+    def queue_update_cache_entry_full(self):        
+        all_keys = sorted(list({k for k in self.sekai_abcache_index.bundles.keys()}.union({k for k in self.local_abcache_index.bundles.keys()})))
         update_count = 0
         for k in all_keys:
-            if k in dl.bundles and k in self.index.bundles:
+            if k in self.sekai_abcache_index.bundles and k in self.local_abcache_index.bundles:
                 # update
-                if not dl.bundles[k].up_to_date(self.config, self.index.bundles[k]):
-                    logger.info('Updating bundle %s. (size on disk=%d, reported=%d)' % (k, self.index.bundles[k].get_file_size(self.config), self.index.bundles[k].fileSize))
-                    self.update_cahce_entry(self.index.bundles[k], dl.bundles[k])
+                if not self.sekai_abcache_index.bundles[k].up_to_date(self.config,self.local_abcache_index.bundles[k]):
+                    logger.debug('Updating bundle %s. (size on disk=%d, reported=%d)' % (k, self.local_abcache_index.bundles[k].get_file_size(self.config), self.local_abcache_index.bundles[k].fileSize))
+                    self.queue_update_cache_entry(self.local_abcache_index.bundles[k], self.sekai_abcache_index.bundles[k])
                     update_count+=1
-                else:
-                    logger.debug('Bundle %s is up to date' % k)
+                else:                    
                     pass
-            elif k in dl.bundles: 
+            elif k in self.sekai_abcache_index.bundles: 
                 # append
                 logger.debug('Adding bundle %s', k)
-                self.index.bundles[k] = dl.bundles[k]
-                self.update_cahce_entry(self.index.bundles[k])
+                self.local_abcache_index.bundles[k] = self.sekai_abcache_index.bundles[k]
+                self.queue_update_cache_entry(self.local_abcache_index.bundles[k])
                 update_count+=1
             else: 
                 # removal
-                logger.info('Removing bundle %s', k)
-                if path.exists(self.index.bundles[k].get_file_path(self.config)):
-                    remove(self.index.bundles[k].get_file_path(self.config))
-                del self.index.bundles[k]
-        logger.info('Saving AssetBundle index')
+                logger.debug('Removing bundle %s', k)
+                if path.exists(self.local_abcache_index.bundles[k].get_file_path(self.config)):
+                    remove(self.local_abcache_index.bundles[k].get_file_path(self.config))
+                del self.local_abcache_index.bundles[k]
+        logger.debug('Saving AssetBundle index')
         self.save()
-        logger.info('...Saved. Need %d updates' % update_count)
-        self.config.downloader.shutdown(wait=True)
-        logger.info('AssetBundles are now up-to-date')
+        logger.debug('Queued %d updates' % update_count)
     
+    def update_metadata(self):
+        logger.info('Updating metadata')
+        logger.debug('Cache directory: %s' % self.config.cache_dir)
+        logger.debug('Set App version: %s (%s)' % (self.config.app_version,self.config.app_platform))
+        self.update_signatures()
+        self.update_system_data()
+        self.update_gameversion_data()               
+        self.update_abcache_index()
+        # Update to the actually usable set version
+        self.config.app_version = self.SEKAI_APP_VERSION.appVersion
+        self.headers['X-App-Version'] = self.SEKAI_APP_VERSION.appVersion
+        self.headers['X-App-Hash'] = self.SEKAI_APP_VERSION.appHash
+        logger.debug('Actual App version: %s (%s), hash=%s' % (self.config.app_version,self.config.app_platform, self.SEKAI_APP_VERSION.appHash))
+        logger.debug('Sekai AssetBundle version: %s' % self.SEKAI_ASSET_VERSION)
+        logger.debug('Sekai AssetBundle host hash: %s' % self.SEKAI_AB_HOST_HASH)
+
     def __init__(self, config : AbCacheConfig) -> None:
         super().__init__()
         self.config = config
         self.headers.update({
             'Accept': 'application/octet-stream',
             'Content-Type': 'application/octet-stream',
             'Accept-Encoding': 'deflate, gzip',
             'User-Agent': 'UnityPlayer/2020.3.32f1 (UnityWebRequest/1.0, libcurl/7.80.0-DEV)',
             'X-Platform': self.config.app_platform,
             'X-Unity-Version': '2020.3.32f1',
-            'X-App-Version': self.config.app_version,
-            'X-Platform': self.config.app_platform
+            'X-App-Version': DEFAULT_SEKAI_FALLBACK_VERSION, # These will be updated later
+            'X-App-Hash': DEFAULT_SEKAI_FALLBACK_APP_HASH
         })
-        logger.info('Cache directory: %s' % self.config.cache_dir)
-        logger.info('App version: %s (%s)' % (self.config.app_version,self.config.app_platform))
-        self.update_signatures()
-        self.update_system_data()
-        self.update_gameversion_data()
-        logger.info('Sekai AssetBundle version: %s' % self.SEKAI_ASSET_VERSION)
-        logger.info('Sekai AssetBundle host hash: %s' % self.SEKAI_AB_HOST_HASH)
         makedirs(self.config.cache_dir,exist_ok=True)
         try:
             self.load()
         except Exception as e:
-            logger.warning('Failed to load cache index. Creating new one. (%s)' % e)
-            self.index = AbCacheIndex(bundles=dict())
+            logger.warning('Failed to load cache index. Creating a new one. (%s)' % e)
+            self.local_abcache_index = AbCacheIndex(bundles=dict())
             self.save()
+        
     
     def save(self):
-        with open(path.join(self.config.cache_dir, 'abindex.json'),'w',encoding='utf-8') as f:
-            dump(asdict(self.index), f, indent=4, ensure_ascii=False)
-            logger.info("Saved %d entries to cache index" % len(self.index.bundles))
+        with open(path.join(self.config.cache_dir, 'abindex'),'wb') as f:
+            dump(asdict(self.local_abcache_index), f)
+            logger.info("Saved %d entries to cache index" % len(self.local_abcache_index.bundles))
 
     def load(self):
-        with open(path.join(self.config.cache_dir, 'abindex.json'),'r',encoding='utf-8') as f:
-            self.index = AbCacheIndex(**load(f))
-            for k,v in self.index.bundles.items():
-                self.index.bundles[k] = AbCacheEntry(**v)
-            logger.info("Loaded %d entries from cache index" % len(self.index.bundles))
+        with open(path.join(self.config.cache_dir, 'abindex'), 'rb') as f:
+            self.local_abcache_index = AbCacheIndex(**load(f, raw=False))
+            for k,v in self.local_abcache_index.bundles.items():
+                self.local_abcache_index.bundles[k] = AbCacheEntry(**v)
+            logger.info("Loaded %d entries from cache index" % len(self.local_abcache_index.bundles))
```

### Comparing `sssekai-0.0.6/sssekai/crypto/APIManager.py` & `sssekai-0.0.8/sssekai/crypto/APIManager.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.0.6/sssekai/crypto/AssetBundle.py` & `sssekai-0.0.8/sssekai/crypto/AssetBundle.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.0.6/sssekai/entrypoint/live2dextract.py` & `sssekai-0.0.8/sssekai/entrypoint/live2dextract.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.0.6/sssekai/entrypoint/spineextract.py` & `sssekai-0.0.8/sssekai/entrypoint/spineextract.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.0.6/sssekai/entrypoint/usmdemux.py` & `sssekai-0.0.8/sssekai/entrypoint/usmdemux.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from sssekai.crypto.AssetBundle import SEKAI_AB_MAGIC
 from sssekai.unity.AssetBundle import load_assetbundle
 
 from os import path,remove,makedirs
 def main_usmdemux(args):
     from UnityPy.enums import ClassIDType
     from wannacri.usm import Usm
```

### Comparing `sssekai-0.0.6/sssekai/fmt/moc3.py` & `sssekai-0.0.8/sssekai/fmt/moc3.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.0.6/sssekai/unity/AnimationClip.py` & `sssekai-0.0.8/sssekai/unity/AnimationClip.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.0.6/sssekai/unity/constant/SekaiLive2DPathNames.py` & `sssekai-0.0.8/sssekai/unity/constant/SekaiLive2DPathNames.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 NAMES_CRC_TBL = {
+    4021652092:"Parts/ArtMesh159_Skinning",
     1133065872:"Parts/ArtMesh159_Skinning2",
+    1702931593:"Parts/ArtMesh161_Skinning",
     2396259621:"Parts/ArtMesh161_Skinning2",
+    2394363786:"Parts/ArtMesh162_Skinning",
     389440292:"Parts/ArtMesh162_Skinning2",
     300985368:"Parts/ArtMesh163Skinning",
     1972486609:"Parts/ArtMesh164Skinning",
     3950300558:"Parts/ArtMesh164Skinning2",
     2208917453:"Parts/ArtMesh164_Skinning",
     1659557266:"Parts/ArtMesh165Skinning",
     938903439:"Parts/ArtMesh181_Skinning",
     1743115835:"Parts/ArtMesh181_Skinning2",
+    3499729872:"Parts/ArtMesh21_Skinning",
     2631333242:"Parts/ArtMesh21_Skinning2",
     814342638:"Parts/ArtMesh325_Skinning",
     880554451:"Parts/ArtMesh327_Skinning",
     716505440:"Parts/ArtMesh329_Skinning",
     4176256596:"Parts/ArtMesh331_Skinning",
     2820643001:"Parts/PARTS",
     2831198909:"Parts/PARTS2",
@@ -29,15 +33,20 @@
     1898224287:"Parts/PARTS_ARM_L",
     2334894076:"Parts/PARTS_ARM_R",
     2290070841:"Parts/PARTS_BALLOON",
     2761942943:"Parts/PARTS_BODY",
     3851622095:"Parts/PARTS_BODY_1",
     2090485621:"Parts/PARTS_BODY_2",
     347760994:"Parts/PARTS_CORE",
+    3126818741:"Parts/PARTS_EAR_CAT",
     798560733:"Parts/PARTS_EYE",
+    2173469883:"Parts/PARTS_EYE_EFFECT_L1",
+    411424001:"Parts/PARTS_EYE_EFFECT_L2",
+    1439546212:"Parts/PARTS_EYE_EFFECT_R1",
+    3435457246:"Parts/PARTS_EYE_EFFECT_R2",
     1572268774:"Parts/PARTS_EYE_L",
     1407274922:"Parts/PARTS_EYE_L2",
     619085628:"Parts/PARTS_EYE_L3",
     2813974405:"Parts/PARTS_EYE_R",
     2275438709:"Parts/PARTS_EYE_R2",
     4037492963:"Parts/PARTS_EYE_R3",
     2049152842:"Parts/PARTS_FACE",
@@ -45,14 +54,16 @@
     4221633922:"Parts/PARTS_FACE3",
     2836404823:"Parts/PARTS_HAIR_BACK",
     4017318464:"Parts/PARTS_HAIR_BACK2",
     2557762262:"Parts/PARTS_HAIR_BACK3",
     2296643005:"Parts/PARTS_HAIR_FRONT",
     2945290945:"Parts/PARTS_HAIR_FRONT2",
     3632964183:"Parts/PARTS_HAIR_FRONT3",
+    1689995882:"Parts/PARTS_HAIR_SIDE_L",
+    2662627081:"Parts/PARTS_HAIR_SIDE_R",
     3636730545:"Parts/PARTS_HEAD",
     2792093965:"Parts/PARTS_HEAD2",
     1687227251:"Parts/PARTS_HEAD_EFFECT",
     3552382848:"Parts/PARTS_HEAD_EFFECT2",
     2763669270:"Parts/PARTS_HEAD_EFFECT3",
     3758823366:"Parts/PARTS_MOUTH",
     1748161183:"Parts/PARTS_MOUTH2",
@@ -108,22 +119,25 @@
     3269042246:"Parts/Part52",
     3051262160:"Parts/Part53",
     733611379:"Parts/Part54",
     2554118162:"Parts/Part6",
     4013682820:"Parts/Part7",
     2139417877:"Parts/Part8",
     142859651:"Parts/Part9",
+    2634930170:"Parts/PartAccessory",
     3724361956:"Parts/PartArm",
     181549335:"Parts/PartArmL",
     2567760371:"Parts/PartArmL2",
     4041016436:"Parts/PartArmR",
     1296946732:"Parts/PartArmR2",
     977987258:"Parts/PartArmR3",
     3536744278:"Parts/PartArmRibbon",
+    2725054883:"Parts/PartBalloon",
     2393564822:"Parts/PartBlazer",
+    2347293104:"Parts/PartBody",
     1211544802:"Parts/PartBody1",
     2371943827:"Parts/PartBody1_1",
     342469673:"Parts/PartBody1_2",
     1668193471:"Parts/PartBody1_3",
     3510625624:"Parts/PartBody2",
     2788742606:"Parts/PartBody3",
     945569901:"Parts/PartBody4",
@@ -155,17 +169,23 @@
     1348423653:"Parts/PartFace3",
     896714094:"Parts/PartFrill",
     3434591003:"Parts/PartHair",
     3031058490:"Parts/PartHairBack",
     3698183671:"Parts/PartHairBack2",
     1808830924:"Parts/PartHairBackL",
     2447355055:"Parts/PartHairBackR",
+    1986500206:"Parts/PartHairBackSkinning1",
+    4017014740:"Parts/PartHairBackSkinning2",
+    2557081410:"Parts/PartHairBackSkinning3",
+    101540577:"Parts/PartHairBackSkinning4",
+    1896501879:"Parts/PartHairBackSkinning5",
     2443541283:"Parts/PartHairDeco",
     2157148866:"Parts/PartHairFront",
     1866436331:"Parts/PartHairFront2",
+    4209349304:"Parts/PartHairSide",
     3751108641:"Parts/PartHairSide2",
     1747467290:"Parts/PartHairSideL",
     2452029817:"Parts/PartHairSideR",
     1524055430:"Parts/PartHairside",
     1041645371:"Parts/PartHandL",
     2883600662:"Parts/PartHandL2",
     3706155392:"Parts/PartHandL3",
@@ -182,35 +202,46 @@
     227914602:"Parts/PartHead2",
     1159802403:"Parts/PartHeadAccessory",
     1712963455:"Parts/PartHeadDeco",
     497937938:"Parts/PartHeadEffect",
     3916522155:"Parts/PartHeadEffect2",
     1222988053:"Parts/PartHeadPhones",
     1523874884:"Parts/PartHeadRibbon",
+    3309336036:"Parts/PartHighlightL",
+    1062160519:"Parts/PartHighlightR",
     1688702150:"Parts/PartHood",
     2210588766:"Parts/PartKatyusha",
     3239288476:"Parts/PartLowerBody",
+    3014432234:"Parts/PartMoon",
     1889238377:"Parts/PartMouth",
     785120396:"Parts/PartMouth2",
     3819404183:"Parts/PartNeckRibbon",
     3502030545:"Parts/PartNose",
     1735176321:"Parts/PartParker",
     3718539789:"Parts/PartPonL",
     665540462:"Parts/PartPonR",
     2884797086:"Parts/PartRibbon",
     2407603119:"Parts/PartRibon_L",
     1972250316:"Parts/PartRibon_R",
     1711001070:"Parts/PartShirt",
     3670282009:"Parts/PartSketch",
+    430471656:"Parts/PartTear",
+    60825605:"Parts/PartTearL",
+    4189003110:"Parts/PartTearR",
     1527994312:"Parts/PartTemp",
     1627218647:"Parts/PartTie",
+    2203288786:"Parts/PartTwintailL",
+    2036119985:"Parts/PartTwintailR",
     2706143167:"Parts/PartUpperBody",
     51296898:"Parts/PartWork",
     799151642:"Parts/Part_CORE",
     1138891839:"Parts/PartlowerBody",
+    309063465:"Parts/Partvehicle",
+    1087288124:"Parameters/PARAMCloudExtendX",
+    2063567466:"Parameters/PARAMRainbowExtend",
     2426468873:"Parameters/PARAM_ANGLE_X",
     3886533279:"Parameters/PARAM_ANGLE_Y",
     2125372197:"Parameters/PARAM_ANGLE_Z",
     1469304612:"Parameters/PARAM_ARM_L",
     3608623690:"Parameters/PARAM_ARM_L_1",
     1310616560:"Parameters/PARAM_ARM_L_2",
     957963110:"Parameters/PARAM_ARM_L_3",
@@ -348,14 +379,16 @@
     1795978481:"Parameters/PARAM_SWING_RIBBON_3",
     1488605431:"Parameters/PARAM_TEAR",
     1494750122:"Parameters/PARAM_TEAR_FROM",
     3638031514:"Parameters/PARAM_TEETH",
     2190374941:"Parameters/PARAM_TIE_SWING",
     3181879606:"Parameters/PARAM_UPPER_BODY",
     3750319138:"Parameters/PARAM_UPPER_BODY_Z",
+    172220796:"Parameters/ParaBalloonFuwa",
+    3410241356:"Parameters/ParaBalloonSwing",
     528322740:"Parameters/Param",
     3522937444:"Parameters/Param10",
     2801595122:"Parameters/Param11",
     1073062728:"Parameters/Param12",
     1223857118:"Parameters/Param13",
     3600156285:"Parameters/Param14",
     2710648555:"Parameters/Param15",
@@ -376,14 +409,15 @@
     1161247105:"Parameters/Param3ParamArmL8",
     1067782461:"Parameters/Param4",
     1218585003:"Parameters/Param5",
     3517673489:"Parameters/Param6",
     2796306567:"Parameters/Param7",
     907238678:"Parameters/Param8",
     1091857792:"Parameters/Param9",
+    2463981908:"Parameters/ParamAdjust",
     549326005:"Parameters/ParamAngleRotation24",
     1471757347:"Parameters/ParamAngleRotation25",
     3467668889:"Parameters/ParamAngleRotation26",
     3115801871:"Parameters/ParamAngleRotation27",
     688406686:"Parameters/ParamAngleRotation28",
     1578070024:"Parameters/ParamAngleRotation29",
     1053358573:"Parameters/ParamAngleRotation30",
@@ -400,82 +434,142 @@
     4025350793:"Parameters/ParamAngleRotation47",
     2136139544:"Parameters/ParamAngleRotation48",
     139843470:"Parameters/ParamAngleRotation49",
     1754422891:"Parameters/ParamAngleRotation50",
     397467875:"Parameters/ParamAngleX",
     1622659189:"Parameters/ParamAngleY",
     4190011855:"Parameters/ParamAngleZ",
+    1035069756:"Parameters/ParamArm",
+    3683193423:"Parameters/ParamArm0",
+    1085069303:"Parameters/ParamArm01L1",
+    3651503693:"Parameters/ParamArm01L2",
+    2929899227:"Parameters/ParamArm01L3",
+    2498619432:"Parameters/ParamArm01R1",
+    233093522:"Parameters/ParamArm01R2",
+    2061732100:"Parameters/ParamArm01R3",
+    1122658734:"Parameters/ParamArm02L1",
+    3689101332:"Parameters/ParamArm02L2",
+    2900625538:"Parameters/ParamArm02L3",
+    2527811185:"Parameters/ParamArm02R1",
+    262277067:"Parameters/ParamArm02R2",
+    2024093533:"Parameters/ParamArm02R3",
+    1271936805:"Parameters/ParamArm0L",
+    2984184390:"Parameters/ParamArm0R",
+    2894996185:"Parameters/ParamArm1",
+    1389037156:"Parameters/ParamArm1L",
+    2831432455:"Parameters/ParamArm1R",
+    898069347:"Parameters/ParamArm2",
+    2045138343:"Parameters/ParamArm2L",
+    2213112004:"Parameters/ParamArm2R",
+    1115702261:"Parameters/ParamArm3",
+    1627219174:"Parameters/ParamArm3L",
     564466456:"Parameters/ParamArmARSwitch",
     3951770818:"Parameters/ParamArmBMove",
     2938770683:"Parameters/ParamArmBRSwitch",
     1592314462:"Parameters/ParamArmFront",
+    384977929:"Parameters/ParamArmL01",
+    2415599027:"Parameters/ParamArmL02",
     3874360414:"Parameters/ParamArmL1",
     2028883422:"Parameters/ParamArmL10",
     2145869284:"Parameters/ParamArmL2",
     148925810:"Parameters/ParamArmL3",
     2525296849:"Parameters/ParamArmL4",
     3783510087:"Parameters/ParamArmL5",
     2022349309:"Parameters/ParamArmL6",
     260942187:"Parameters/ParamArmL7",
     2670900474:"Parameters/ParamArmL8",
     3895821420:"Parameters/ParamArmL9",
     1397086757:"Parameters/ParamArmLRibbonSwing1",
     3394014111:"Parameters/ParamArmLRibbonSwing2",
+    3531658658:"Parameters/ParamArmLX",
+    2777146676:"Parameters/ParamArmLY",
+    4899443:"Parameters/ParamArmR01",
+    2571342793:"Parameters/ParamArmR02",
     850342785:"Parameters/ParamArmR1",
     1851179940:"Parameters/ParamArmR10",
     2879808059:"Parameters/ParamArmR2",
     3701559981:"Parameters/ParamArmR3",
     1120257806:"Parameters/ParamArmR4",
     901969816:"Parameters/ParamArmR5",
     2899027490:"Parameters/ParamArmR6",
     3687618228:"Parameters/ParamArmR7",
     1265863461:"Parameters/ParamArmR8",
     1014283187:"Parameters/ParamArmR9",
     497315919:"Parameters/ParamArmRRibbonSwing1",
     2225938933:"Parameters/ParamArmRRibbonSwing2",
+    113371773:"Parameters/ParamArmRX",
+    1908857579:"Parameters/ParamArmRY",
     2280925350:"Parameters/ParamArmRise",
+    775526053:"Parameters/ParamArmarillSwing",
+    3158823164:"Parameters/ParamArmarillSwing2",
+    4024589799:"Parameters/ParamBagSwingA",
+    1995115613:"Parameters/ParamBagSwingB",
+    32259275:"Parameters/ParamBagSwingC",
+    763945921:"Parameters/ParamBalloonRibbonFuwa",
+    2125669247:"Parameters/ParamBalloonRibbonSwing",
+    3102943170:"Parameters/ParamBalloonSize",
+    1862790838:"Parameters/ParamBalloonSize2",
+    1456950351:"Parameters/ParamBalloonX",
+    59120950:"Parameters/ParamBalloonYPosX",
     1063149258:"Parameters/ParamBeard",
     4203107101:"Parameters/ParamBeltFuwa",
     4043420464:"Parameters/ParamBeltSwing",
     1023250194:"Parameters/ParamBeltSwing2",
     2846399352:"Parameters/ParamBloodVessel",
+    1257546180:"Parameters/ParamBoadUpDown",
+    2257996805:"Parameters/ParamBoadUpDown2",
+    369372051:"Parameters/ParamBoadUpDown2Body",
+    3168167613:"Parameters/ParamBoadUpDownBody",
+    2367297234:"Parameters/ParamBoadZ",
+    1921325027:"Parameters/ParamBoadZ2",
+    1590068145:"Parameters/ParamBoadZ2Body",
+    3427274522:"Parameters/ParamBoadZBody",
+    2933719285:"Parameters/ParamBody1",
+    936661327:"Parameters/ParamBody2",
     2112179668:"Parameters/ParamBody2HangZ",
     1141202947:"Parameters/ParamBodyAngleX",
     855789717:"Parameters/ParamBodyAngleY",
     2852847919:"Parameters/ParamBodyAngleZ",
     2720197501:"Parameters/ParamBodyFrillHuwa",
     64735409:"Parameters/ParamBodyFrillSwing",
     1245006479:"Parameters/ParamBodyFuwa",
     2928948592:"Parameters/ParamBodyFuwaA",
     933061834:"Parameters/ParamBodyFuwaB",
     18333004:"Parameters/ParamBodyHangZ",
     2867477948:"Parameters/ParamBodyHuwa",
     295996177:"Parameters/ParamBodyHuwaA",
     2293095083:"Parameters/ParamBodyHuwaB",
     4289391165:"Parameters/ParamBodyHuwaC",
+    1533977428:"Parameters/ParamBodyLegY",
+    3261592302:"Parameters/ParamBodyLegZ",
+    2899942910:"Parameters/ParamBodyLine",
     589872730:"Parameters/ParamBodyRibbonFuwa1",
     1994466024:"Parameters/ParamBodyRibbonSwing1",
     4024988498:"Parameters/ParamBodyRibbonSwing2",
     2565817284:"Parameters/ParamBodyRibbonSwing3",
     3538771839:"Parameters/ParamBodySwingA",
     1273237189:"Parameters/ParamBodySwingB",
     3099187545:"Parameters/ParamBodySwingB_01",
     565217507:"Parameters/ParamBodySwingB_02",
     1021525587:"Parameters/ParamBodySwingC",
+    3901447549:"Parameters/ParamBodySwingC2",
     1597374790:"Parameters/ParamBodySwingCL",
     2771991589:"Parameters/ParamBodySwingCR",
     1399288064:"Parameters/ParamBodySwingC_L",
     2842184803:"Parameters/ParamBodySwingC_R",
     2726800368:"Parameters/ParamBodySwingD",
     276273025:"Parameters/ParamBodySwingDL",
     3933776610:"Parameters/ParamBodySwingDR",
     1445488517:"Parameters/ParamBodySwingD_L",
     2888260326:"Parameters/ParamBodySwingD_R",
     3581975398:"Parameters/ParamBodySwingE",
     1284098780:"Parameters/ParamBodySwingF",
+    2516363576:"Parameters/ParamBodySwingF2",
+    3808139694:"Parameters/ParamBodySwingF3",
+    2090798093:"Parameters/ParamBodySwingF4",
     3595699470:"Parameters/ParamBodySwingFuwa",
     999225930:"Parameters/ParamBodySwingG",
     995804226:"Parameters/ParamBodySwingGL",
     3243637025:"Parameters/ParamBodySwingGR",
     2872174555:"Parameters/ParamBodySwingH",
     3694581581:"Parameters/ParamBodySwingI",
     1161791223:"Parameters/ParamBodySwingJ",
@@ -494,14 +588,15 @@
     2876944824:"Parameters/ParamBracelet1Fuwa",
     1475090613:"Parameters/ParamBracelet1Swing",
     3973761896:"Parameters/ParamBracelet2Fuwa",
     3514329627:"Parameters/ParamBracelet2Swing",
     1671053000:"Parameters/ParamBracelet4Fuwa",
     1732271208:"Parameters/ParamBraceletSwing",
     3823476906:"Parameters/ParamBreath",
+    3120995542:"Parameters/ParamBroachSwing",
     321347094:"Parameters/ParamBrowLAngle",
     2550903895:"Parameters/ParamBrowLForm",
     1254050164:"Parameters/ParamBrowLWrinkle",
     2333223759:"Parameters/ParamBrowLWrinkle01",
     303790837:"Parameters/ParamBrowLWrinkle02",
     4199213146:"Parameters/ParamBrowLWrinkleL",
     2780107611:"Parameters/ParamBrowLX",
@@ -518,86 +613,143 @@
     1817757842:"Parameters/ParamBustFuriruSwing",
     3288276072:"Parameters/ParamBustRibbonFuwa",
     164668746:"Parameters/ParamBustX",
     2128057820:"Parameters/ParamBustY",
     4080828015:"Parameters/ParamCaneSwitch",
     1390522448:"Parameters/ParamCardiganFuwa",
     4190431742:"Parameters/ParamCardiganSwing",
+    730756834:"Parameters/ParamChainHuwaB",
+    3712910823:"Parameters/ParamChainSwingA",
+    610699091:"Parameters/ParamChainSwingA2",
     1650564732:"Parameters/ParamCheek",
     3262488404:"Parameters/ParamCheek02",
     3044192194:"Parameters/ParamCheek03",
     722877025:"Parameters/ParamCheek04",
     1124393604:"Parameters/ParamCheek2",
     872665618:"Parameters/ParamCheek3",
     2120432374:"Parameters/ParamCheekAngry",
+    4190688805:"Parameters/ParamCheekAngryL",
+    63433542:"Parameters/ParamCheekAngryR",
+    570935191:"Parameters/ParamCherryPosX",
+    1426126593:"Parameters/ParamCherryPosY",
+    3423184571:"Parameters/ParamCherryPosZ",
+    2425361543:"Parameters/ParamCherryX",
     796091174:"Parameters/ParamChuckFuwa",
     1088401188:"Parameters/ParamChuckSwing",
     2521177425:"Parameters/ParamChuckSwingH",
     3779145159:"Parameters/ParamChuckSwingI",
+    13298184:"Parameters/ParamCloakHuwaB",
+    2646264349:"Parameters/ParamCloakSwingA",
     3313808680:"Parameters/ParamClothFuwa1",
     1552802962:"Parameters/ParamClothFuwa2",
     2508309524:"Parameters/ParamClothFuwaA",
     210277806:"Parameters/ParamClothFuwaB",
     2073011512:"Parameters/ParamClothFuwaC",
     3857395867:"Parameters/ParamClothFuwaD",
     39001500:"Parameters/ParamClothFuwaJ",
     716274293:"Parameters/ParamClothHuwaA",
     3015191503:"Parameters/ParamClothHuwaB",
     3300858713:"Parameters/ParamClothHuwaC",
     1524338426:"Parameters/ParamClothHuwaD",
     639921375:"Parameters/ParamClothesFuwa",
     2226631315:"Parameters/ParamClothesSwing",
+    1173588212:"Parameters/ParamCloudUpDown",
+    2565317455:"Parameters/ParamCloudY",
+    1921022208:"Parameters/ParamClowdFuwa",
+    3287315499:"Parameters/ParamCollarFuwa",
+    1048727694:"Parameters/ParamCollarSwing",
+    4282613642:"Parameters/ParamCollarswing",
     1857891283:"Parameters/ParamCollorSwing",
     610714875:"Parameters/ParamCorsetSwing1",
     3178206529:"Parameters/ParamCorsetSwing2",
     2182970360:"Parameters/ParamCostumeFuwa",
     555302639:"Parameters/ParamCostumeSwing",
+    955573577:"Parameters/ParamCreamPosX",
+    1341380063:"Parameters/ParamCreamPosY",
+    3606742117:"Parameters/ParamCreamPosZ",
+    2506156731:"Parameters/ParamCreamX",
     619702575:"Parameters/ParamCry",
     1882652453:"Parameters/ParamDarkcycles",
     432666763:"Parameters/ParamDoubleForm",
     1863143841:"Parameters/ParamDressSwing",
+    3171936018:"Parameters/ParamEarFuwa",
+    811321787:"Parameters/ParamEarHuwaL1",
+    2840762369:"Parameters/ParamEarHuwaL2",
+    3826972260:"Parameters/ParamEarHuwaR1",
+    2098440158:"Parameters/ParamEarHuwaR2",
+    3731008440:"Parameters/ParamEarL",
+    2894196411:"Parameters/ParamEarLFuwa",
+    1854677020:"Parameters/ParamEarLUpDown",
+    4023736775:"Parameters/ParamEarLswing1",
+    1994131581:"Parameters/ParamEarLswing2",
+    611161819:"Parameters/ParamEarR",
+    1500366735:"Parameters/ParamEarRUpDown",
     2697710:"Parameters/ParamEarRingFuwa",
     3774242525:"Parameters/ParamEarRingHuwa",
     3578773484:"Parameters/ParamEarRingSwing",
+    3627335252:"Parameters/ParamEarRswing1",
+    1094578158:"Parameters/ParamEarRswing2",
     1643718421:"Parameters/ParamEarSwing",
     3015659347:"Parameters/ParamEarY",
+    1104549151:"Parameters/ParamEarsizeL",
+    3151571068:"Parameters/ParamEarsizeR",
+    298392022:"Parameters/ParamEarswingL1",
+    2294302828:"Parameters/ParamEarswingL2",
+    1551988659:"Parameters/ParamEarswingR2",
     1346256061:"Parameters/ParamEnbiFuwa",
+    3617001497:"Parameters/ParamEye",
+    2422726897:"Parameters/ParamEye0",
+    3881881703:"Parameters/ParamEye1",
+    2120843741:"Parameters/ParamEye2",
+    158249291:"Parameters/ParamEye3",
+    2534024424:"Parameters/ParamEye4",
+    3758953598:"Parameters/ParamEye5",
+    439726873:"Parameters/ParamEye5L",
+    3761933946:"Parameters/ParamEye5R",
+    2030323140:"Parameters/ParamEye6",
+    235107666:"Parameters/ParamEye7",
     2171796666:"Parameters/ParamEyeBallX",
     4134915116:"Parameters/ParamEyeBallY",
     2878588271:"Parameters/ParamEyeChange",
     421411201:"Parameters/ParamEyeEyeLid1",
     3248512125:"Parameters/ParamEyeEyelid01",
     3416285413:"Parameters/ParamEyeHi",
+    317062067:"Parameters/ParamEyeHighlight",
     3620524049:"Parameters/ParamEyeHilightonoff",
     832372986:"Parameters/ParamEyeHlForm",
     4097991376:"Parameters/ParamEyeHlOn",
     3989116191:"Parameters/ParamEyeHlOn01",
     1959543973:"Parameters/ParamEyeHlOn02",
+    1581384632:"Parameters/ParamEyeKirakira",
+    690431522:"Parameters/ParamEyeKirakiraOn",
     795883630:"Parameters/ParamEyeLEyelid",
     2199097593:"Parameters/ParamEyeLForm",
     3728205605:"Parameters/ParamEyeLForm2",
     1978396178:"Parameters/ParamEyeLOpen",
     542740187:"Parameters/ParamEyeLSmile",
+    1179028871:"Parameters/ParamEyeLSmileR",
     3641703790:"Parameters/ParamEyeMoth01",
     2714432104:"Parameters/ParamEyeMoth1",
     412213245:"Parameters/ParamEyeREyelid",
     1556330778:"Parameters/ParamEyeRForm",
     3890971854:"Parameters/ParamEyeRForm2",
     2856044529:"Parameters/ParamEyeROpen",
     428207408:"Parameters/ParamEyeRSmile",
     642471233:"Parameters/ParamEyeScale",
     1081240475:"Parameters/ParamEyeSize",
     2867046361:"Parameters/ParamEyeSpecial",
+    2120816101:"Parameters/ParamEyeStar",
     1900066077:"Parameters/ParamEyeTeary",
     2040697441:"Parameters/ParamEyeTeary2",
     245736183:"Parameters/ParamEyeTeary3",
     3778377521:"Parameters/ParamEyeWrinkle01L",
     456804946:"Parameters/ParamEyeWrinkle01R",
     3390579954:"Parameters/ParamEyeWrinkle02L",
     806820241:"Parameters/ParamEyeWrinkle02R",
+    3176763497:"Parameters/ParamEyeWrinkleL",
     2339494597:"Parameters/ParamEyeWrinkleL01",
     1254580187:"Parameters/ParamEyeWrinkleL01_Form",
     3384875282:"Parameters/ParamEyeWrinkleL01_X",
     3200657796:"Parameters/ParamEyeWrinkleL01_Y",
     309889919:"Parameters/ParamEyeWrinkleL02",
     3428003189:"Parameters/ParamEyeWrinkleL02_Form",
     3414665035:"Parameters/ParamEyeWrinkleL02_X",
@@ -624,175 +776,272 @@
     2809806708:"Parameters/ParamFinger4",
     1226323025:"Parameters/ParamFinger4_2",
     3497856994:"Parameters/ParamFinger5",
     1222270566:"Parameters/ParamFinger5_2",
     4188325498:"Parameters/ParamFingerL",
     61602585:"Parameters/ParamFingerR",
     1805095925:"Parameters/ParamFrillFuwa",
+    3613994765:"Parameters/ParamFrillFuwa2",
+    1598146746:"Parameters/ParamFrillSwing",
+    826189143:"Parameters/ParamFrillSwing2",
+    4164060625:"Parameters/ParamFrillSwingA",
+    1631310955:"Parameters/ParamFrillSwingB",
     2986457928:"Parameters/ParamFrontSkirtSwing",
     1784565814:"Parameters/ParamFroshikiHangZ",
     2287383532:"Parameters/ParamFroshikiHuwa",
     2130395650:"Parameters/ParamFroshikiSwing01",
     3891401656:"Parameters/ParamFroshikiSwing02",
+    4252684422:"Parameters/ParamFrownLine",
     1158157453:"Parameters/ParamFumeChange",
     4111916540:"Parameters/ParamGlassOn",
     3095524686:"Parameters/ParamHL1Size",
+    2936508169:"Parameters/ParamHairAccessory",
+    1671823654:"Parameters/ParamHairAccessory2",
+    1415909555:"Parameters/ParamHairAccessorySwing1",
+    3446423817:"Parameters/ParamHairAccessorySwing2",
     3173065058:"Parameters/ParamHairAho",
     3117719384:"Parameters/ParamHairAho2",
     1293934098:"Parameters/ParamHairAhoge",
+    3911307419:"Parameters/ParamHairAhoge2",
     447917413:"Parameters/ParamHairBack",
     2142010931:"Parameters/ParamHairBack01",
     3869585289:"Parameters/ParamHairBack02",
     3189688525:"Parameters/ParamHairBack1",
     655858039:"Parameters/ParamHairBack2",
     1343269345:"Parameters/ParamHairBack3",
+    3994794481:"Parameters/ParamHairBackA",
+    3498141502:"Parameters/ParamHairBackA2",
     1997727819:"Parameters/ParamHairBackB",
+    4222366973:"Parameters/ParamHairBackB2",
+    2360018027:"Parameters/ParamHairBackB3",
     334715107:"Parameters/ParamHairBackLr",
     600178327:"Parameters/ParamHairBackLr2",
     3770647160:"Parameters/ParamHairChoro",
+    1156315265:"Parameters/ParamHairChoro2",
+    303615838:"Parameters/ParamHairControl",
     2078879298:"Parameters/ParamHairFront",
     3520626583:"Parameters/ParamHairFront01",
     1221668397:"Parameters/ParamHairFront02",
     2189195167:"Parameters/ParamHairFront2",
+    1265653529:"Parameters/ParamHairFrontA",
+    3531146915:"Parameters/ParamHairFrontB",
     4203172644:"Parameters/ParamHairFrontFrizz",
+    1018208455:"Parameters/ParamHairFrontHuwa",
     1082396629:"Parameters/ParamHairFuwa",
     2690349286:"Parameters/ParamHairHuwa",
+    1394385464:"Parameters/ParamHairHuwa2",
+    605786798:"Parameters/ParamHairHuwa3",
+    3890600484:"Parameters/ParamHairPartsFuwa",
+    640794374:"Parameters/ParamHairPartsFuwa2",
+    2920896689:"Parameters/ParamHairPartsSwing",
     1032873597:"Parameters/ParamHairRibbon",
     2335421010:"Parameters/ParamHairRibbonHuwa",
     2212593617:"Parameters/ParamHairRibbonL",
     1921772682:"Parameters/ParamHairRibbonL1",
     3951213872:"Parameters/ParamHairRibbonL2",
     2798310229:"Parameters/ParamHairRibbonR1",
     1069777647:"Parameters/ParamHairRibbonR2",
+    1778024379:"Parameters/ParamHairRibbonStringHuwa",
     1425897447:"Parameters/ParamHairSide",
     270528895:"Parameters/ParamHairSide01",
     2299961541:"Parameters/ParamHairSide02",
     3185992987:"Parameters/ParamHairSide1",
     619656353:"Parameters/ParamHairSide2",
     3991082023:"Parameters/ParamHairSideA",
     3207784562:"Parameters/ParamHairSideA2",
+    1961510301:"Parameters/ParamHairSideB",
+    2485107633:"Parameters/ParamHairSideB2",
+    3810036519:"Parameters/ParamHairSideB3",
     4252381227:"Parameters/ParamHairSideFrizz",
     3063165309:"Parameters/ParamHairSideFrizz2",
     185013802:"Parameters/ParamHairSideTail",
     3244650701:"Parameters/ParamHairSideTail2",
+    1678048238:"Parameters/ParamHairSwing",
     4260259553:"Parameters/ParamHairTwin",
     3441787525:"Parameters/ParamHairTwin2",
     3215027315:"Parameters/ParamHairTwintailHuwa1",
     648560073:"Parameters/ParamHairTwintailHuwa2",
     1826430306:"Parameters/ParamHairTwintalHuwa1",
     4124331224:"Parameters/ParamHairTwintalHuwa2",
     968573178:"Parameters/ParamHamdShadow",
+    1199840847:"Parameters/ParamHamdShadow2",
+    813903577:"Parameters/ParamHamdShadow3",
     3789098979:"Parameters/ParamHandLA",
     2026921561:"Parameters/ParamHandLB",
     265776847:"Parameters/ParamHandLC",
     2444491628:"Parameters/ParamHandLD",
     3870608378:"Parameters/ParamHandLE",
     2143132224:"Parameters/ParamHandLF",
     146451158:"Parameters/ParamHandLG",
     2550511431:"Parameters/ParamHandLH",
     4009920465:"Parameters/ParamHandLI",
     1980487275:"Parameters/ParamHandLJ",
     17622781:"Parameters/ParamHandLK",
     2674422622:"Parameters/ParamHandLL",
+    3899605960:"Parameters/ParamHandLM",
+    1902514802:"Parameters/ParamHandLN",
+    107029220:"Parameters/ParamHandLO",
+    2338926353:"Parameters/ParamHandLP",
+    4235075463:"Parameters/ParamHandLQ",
+    1701269053:"Parameters/ParamHandLR",
+    308313771:"Parameters/ParamHandLS",
+    2349132552:"Parameters/ParamHandLT",
     899166268:"Parameters/ParamHandRA",
     2895208838:"Parameters/ParamHandRB",
     3684061456:"Parameters/ParamHandRC",
     1173537971:"Parameters/ParamHandRD",
     854979621:"Parameters/ParamHandRE",
     2885461407:"Parameters/ParamHandRF",
     3707475209:"Parameters/ParamHandRG",
     1279559832:"Parameters/ParamHandRH",
     994293774:"Parameters/ParamHandRI",
     2722818484:"Parameters/ParamHandRJ",
     3578648866:"Parameters/ParamHandRK",
     1260997761:"Parameters/ParamHandRL",
+    1009679383:"Parameters/ParamHandRM",
+    2770808237:"Parameters/ParamHandRN",
+    3525319995:"Parameters/ParamHandRO",
+    1596461262:"Parameters/ParamHandRP",
+    674177112:"Parameters/ParamHandRQ",
+    2972086754:"Parameters/ParamHandRR",
+    3324068212:"Parameters/ParamHandRS",
+    1480971479:"Parameters/ParamHandRT",
     913681141:"Parameters/ParamHandRibbonSwing",
+    3297800182:"Parameters/ParamHatPosition",
     3901298168:"Parameters/ParamHeadHangZ",
     3764026384:"Parameters/ParamHeadShine",
     503887426:"Parameters/ParamHeadSwingA",
     2265049080:"Parameters/ParamHeadSwingB",
     4026980206:"Parameters/ParamHeadSwingC",
     1851933389:"Parameters/ParamHeadSwingD",
     426078811:"Parameters/ParamHeadSwingE",
+    2154570721:"Parameters/ParamHeadSwingF",
     2490204078:"Parameters/ParamHeadSwingZ",
     2784609431:"Parameters/ParamHemFuwa",
     4231243417:"Parameters/ParamHemSwing",
     241073746:"Parameters/ParamHighlight",
     2680082603:"Parameters/ParamHighlight2",
     3904495677:"Parameters/ParamHighlight3",
     240225759:"Parameters/ParamHighlightForm",
     2720324382:"Parameters/ParamHighlightView",
     2037511695:"Parameters/ParamHighlightView1",
     3766003637:"Parameters/ParamHighlightView2",
     152765056:"Parameters/ParamHighlightView4",
     1888112791:"Parameters/ParamHimoFuwa",
     591020629:"Parameters/ParamHoodX",
     1413313219:"Parameters/ParamHoodY",
+    2859155943:"Parameters/ParamHuwaControl",
+    1111428467:"Parameters/ParamInnerSwing",
     4285603815:"Parameters/ParamJacketFuwa",
     3397378595:"Parameters/ParamJacketFuwa02",
     531523796:"Parameters/ParamJacketHuwa",
     1383605806:"Parameters/ParamJacketHuwaA",
+    3413211028:"Parameters/ParamJacketHuwaB",
     2892783486:"Parameters/ParamJacketSwing",
     2915339881:"Parameters/ParamJacketSwing2",
     1690873583:"Parameters/ParamJacketSwingA",
+    2366728306:"Parameters/ParamJacketYure",
+    4031079831:"Parameters/ParamJackettFuwa",
+    4234549816:"Parameters/ParamJackettSwing",
     2790893277:"Parameters/ParamJewelryFuwa",
     1970393414:"Parameters/ParamKira",
+    471235267:"Parameters/ParamKira1",
+    1660276386:"Parameters/ParamKira1Size",
+    2233412473:"Parameters/ParamKira2",
+    626373746:"Parameters/ParamKira2Size",
+    4061666287:"Parameters/ParamKira3",
+    406166978:"Parameters/ParamKira3Size",
+    697577431:"Parameters/ParamKiraKira",
     1191063520:"Parameters/ParamKiraPin",
     2309390569:"Parameters/ParamKirakira",
     2067958139:"Parameters/ParamKneeRibbonL",
     205896173:"Parameters/ParamKneeRibbonM",
     2941204780:"Parameters/ParamKuchi",
     676255654:"Parameters/ParamKumaView",
     1523262320:"Parameters/ParamLTear",
     2202781583:"Parameters/ParamLaceSwing",
+    178000637:"Parameters/ParamLegLR",
     3185367402:"Parameters/ParamLegLRise",
+    3930717155:"Parameters/ParamLegLX",
+    2639186805:"Parameters/ParamLegLY",
     71801551:"Parameters/ParamLegLZ",
+    3739036962:"Parameters/ParamLegRR",
     1645015177:"Parameters/ParamLegRRise",
+    1040761916:"Parameters/ParamLegRX",
+    1225782442:"Parameters/ParamLegRY",
     3490096400:"Parameters/ParamLegRZ",
+    2299297415:"Parameters/ParamLegX",
+    4262153745:"Parameters/ParamLegY",
+    1728192427:"Parameters/ParamLegZ",
     2371033367:"Parameters/ParamLightView",
     2623341031:"Parameters/ParamLioneye01",
     89411677:"Parameters/ParamLioneye02",
     1918066891:"Parameters/ParamLioneye03",
     3963090280:"Parameters/ParamLioneye04",
     2603664894:"Parameters/ParamLioneye05",
     37327940:"Parameters/ParamLioneye06",
     1967039698:"Parameters/ParamLioneye07",
     3181819922:"Parameters/ParamLooseHair01",
     615508392:"Parameters/ParamLooseHair02",
     2563193013:"Parameters/ParamMaskOn",
+    1853511834:"Parameters/ParamMelonPosX",
+    427649036:"Parameters/ParamMelonPosY",
+    2155100598:"Parameters/ParamMelonPosZ",
+    554823962:"Parameters/ParamMelonX",
+    2523974014:"Parameters/ParamMouth",
+    1139864531:"Parameters/ParamMouth0",
+    888652613:"Parameters/ParamMouth1",
     2919142143:"Parameters/ParamMouth2",
+    3673793129:"Parameters/ParamMouth3",
+    1151154122:"Parameters/ParamMouth4",
+    865732444:"Parameters/ParamMouth5",
+    2861782758:"Parameters/ParamMouth6",
+    3717490288:"Parameters/ParamMouth7",
     3514263446:"Parameters/ParamMouthForm",
     57212699:"Parameters/ParamMouthForm2",
     3995501637:"Parameters/ParamMouthOpenY",
+    3165428247:"Parameters/ParamMouthOpenY_old",
     2181955505:"Parameters/ParamMouthPositionX",
     4111126311:"Parameters/ParamMouthPositionY",
     497791140:"Parameters/ParamMouthScaleX",
     1789689906:"Parameters/ParamMouthScaleY",
     894830046:"Parameters/ParamMouthShadow",
     3478896626:"Parameters/ParamMoveFume",
     3201299668:"Parameters/ParamNeckFuwa",
+    2658313561:"Parameters/ParamNeckSwin",
     335380611:"Parameters/ParamNeckSwing",
     4152279213:"Parameters/ParamNeckSwing1",
     1853329687:"Parameters/ParamNeckSwing2",
     2053786751:"Parameters/ParamNecklaceFuwa",
     657730868:"Parameters/ParamNecklaceStringHuwaD",
     2495748948:"Parameters/ParamNecklaceStringSwingD",
     3821349826:"Parameters/ParamNecklaceStringSwingE",
     1379753819:"Parameters/ParamNecklaceSwing",
     3862825774:"Parameters/ParamNecklaceSwing2",
     2975251979:"Parameters/ParamNecklaceSwingF",
     3327233693:"Parameters/ParamNecklaceSwingG",
     334399850:"Parameters/ParamNormalEye",
+    1064906689:"Parameters/ParamNoseRed",
+    3555393053:"Parameters/ParamOrangePosX",
+    2767048331:"Parameters/ParamOrangePosY",
+    1038393137:"Parameters/ParamOrangePosZ",
+    3869781295:"Parameters/ParamOrangeX",
     2251208416:"Parameters/ParamOsageL",
     2082573187:"Parameters/ParamOsageR",
+    1218822606:"Parameters/ParamPantsRibbonSwing",
+    1715598459:"Parameters/ParamPantsRibbonSwing2",
     4037855955:"Parameters/ParamParkerFuwa",
     276020704:"Parameters/ParamParkerHuwa",
     2379707934:"Parameters/ParamParkerSwing",
     3763819544:"Parameters/ParamParkerSwing2",
     1481285104:"Parameters/ParamPiasSwing",
+    1036927352:"Parameters/ParamPiasuSwing",
+    3751362731:"Parameters/ParamPierce",
+    1527668013:"Parameters/ParamPierce2",
+    1461859982:"Parameters/ParamPosition",
     3185949274:"Parameters/ParamPositionX",
     3403844300:"Parameters/ParamPositionY",
     2233141907:"Parameters/ParamRTear",
     3083608617:"Parameters/ParamRedEyeR",
     1728348901:"Parameters/ParamReflectedLight",
     2227145507:"Parameters/ParamRibbon2Swing",
     3090575604:"Parameters/ParamRibbon2Swing2",
@@ -808,14 +1057,16 @@
     203224579:"Parameters/ParamRibbonSwing2",
     1763798882:"Parameters/ParamRibbonX",
     1879883664:"Parameters/ParamRibbonXA",
     3909479978:"Parameters/ParamRibbonXB",
     505831412:"Parameters/ParamRibbonY",
     1763151569:"Parameters/ParamRibbonYA",
     4028555115:"Parameters/ParamRibbonYB",
+    3711684804:"Parameters/ParamRoprHuwaB",
+    263566780:"Parameters/ParamRoprSwingA",
     1424576275:"Parameters/ParamRotationZ",
     3841175661:"Parameters/ParamScale",
     2377047131:"Parameters/ParamScarf1",
     346525153:"Parameters/ParamScarf2",
     2022373968:"Parameters/ParamShimenawaFaceSwing",
     1761407924:"Parameters/ParamShimenawaHuwa",
     1985753683:"Parameters/ParamShimenawaRingSwing",
@@ -824,18 +1075,28 @@
     167184000:"Parameters/ParamShirtFuwa",
     407962998:"Parameters/ParamShirtHuwaB",
     1867920864:"Parameters/ParamShirtHuwaC",
     3004587123:"Parameters/ParamShirtSwingB",
     3289476325:"Parameters/ParamShirtSwingC",
     2437270373:"Parameters/ParamShirtsFuwa",
     2947844518:"Parameters/ParamShirtsSwing",
+    2009336143:"Parameters/ParamShoulder01L",
+    2378904620:"Parameters/ParamShoulder01R",
+    1558796940:"Parameters/ParamShoulder02L",
+    2800117743:"Parameters/ParamShoulder02R",
     151499700:"Parameters/ParamShoulderL",
     4077424343:"Parameters/ParamShoulderR",
     551282230:"Parameters/ParamShyView",
     795402279:"Parameters/ParamSize",
+    3220202374:"Parameters/ParamSize2",
+    3900401720:"Parameters/ParamSkeleton0",
+    2675726510:"Parameters/ParamSkeleton1",
+    108333332:"Parameters/ParamSkeleton2",
+    1903311234:"Parameters/ParamSkeleton3",
+    4011240481:"Parameters/ParamSkeleton4",
     2443564567:"Parameters/ParamSkirt",
     2156391276:"Parameters/ParamSkirt2Swing",
     1219303786:"Parameters/ParamSkirtBertSwing",
     84257039:"Parameters/ParamSkirtFrillHuwa",
     3178758115:"Parameters/ParamSkirtFrillSwing",
     2272788835:"Parameters/ParamSkirtFuwa",
     1474340692:"Parameters/ParamSkirtFuwa1",
@@ -845,14 +1106,16 @@
     1739028048:"Parameters/ParamSkirtHuwa",
     568080819:"Parameters/ParamSkirtHuwaB",
     2766679669:"Parameters/ParamSkirtLaceHuwa",
     218532422:"Parameters/ParamSkirtLaceSwing",
     1075815090:"Parameters/ParamSkirtRibbonFuwa",
     3553727041:"Parameters/ParamSkirtShake",
     1187058009:"Parameters/ParamSkirtSwing",
+    3465061400:"Parameters/ParamSkirtSwing01",
+    1468134818:"Parameters/ParamSkirtSwing02",
     2435696630:"Parameters/ParamSkirtSwing1",
     136615500:"Parameters/ParamSkirtSwing2",
     2133042906:"Parameters/ParamSkirtSwing3",
     3779539833:"Parameters/ParamSkirtSwing4",
     3240670922:"Parameters/ParamSkirtSwingA",
     1478616944:"Parameters/ParamSkirtSwingB",
     791074790:"Parameters/ParamSkirtSwingC",
@@ -862,38 +1125,62 @@
     848414594:"Parameters/ParamSkirtSwingS",
     2901758497:"Parameters/ParamSkirtSwingT",
     2602036815:"Parameters/ParamSleeveFuwa",
     2076744060:"Parameters/ParamSleeveHuwa",
     1946489429:"Parameters/ParamSleeveSwing",
     3055370847:"Parameters/ParamSleeveSwingL",
     1276280636:"Parameters/ParamSleeveSwingR",
+    171939558:"Parameters/ParamSmile",
     2472867533:"Parameters/ParamSpeakerResize",
     213325773:"Parameters/ParamSpecialCheek01",
+    3342417859:"Parameters/ParamSpecialEye",
     2582661823:"Parameters/ParamSpecialEye01",
     16325381:"Parameters/ParamSpecialEye02",
     2013146003:"Parameters/ParamSpecialEye03",
+    410981432:"Parameters/ParamSpecialEye2",
     177352564:"Parameters/ParamSpecialEyeRotate1",
     1715562423:"Parameters/ParamSpecialEyebrow01",
+    3728752230:"Parameters/ParamStar1PositionX",
+    2840006384:"Parameters/ParamStar1PositionY",
+    2610605975:"Parameters/ParamStar1Rotation",
+    800879294:"Parameters/ParamStar1Scaling",
+    897025381:"Parameters/ParamStar2PositionX",
+    1114682867:"Parameters/ParamStar2PositionY",
+    2719454034:"Parameters/ParamStar2Rotation",
+    2704504157:"Parameters/ParamStar2Scaling",
+    3669356123:"Parameters/ParamStar3PositionX",
+    2914180813:"Parameters/ParamStar3PositionY",
+    3043788561:"Parameters/ParamStar3Rotation",
+    1838773699:"Parameters/ParamStar3Scaling",
+    2197501062:"Parameters/ParamStarAllonoff",
+    3216432596:"Parameters/ParamStaronoff",
+    3586705073:"Parameters/ParamStrawberryPosX",
+    2731537959:"Parameters/ParamStrawberryPosY",
+    1002874781:"Parameters/ParamStrawberryPosZ",
+    231510313:"Parameters/ParamStrawberryX",
     2828308470:"Parameters/ParamStringFuwa",
     3331037724:"Parameters/ParamStringSwing",
     971818426:"Parameters/ParamStringSwing01",
     2699400192:"Parameters/ParamStringSwing02",
     2535143522:"Parameters/ParamStringSwing1",
     236087768:"Parameters/ParamStringSwing2",
     141487747:"Parameters/ParamSugaoSwing",
     1852572281:"Parameters/ParamSugaoSwing2",
     2639993062:"Parameters/ParamSuitHuwa",
     1681521550:"Parameters/ParamSuitSwing",
     391498689:"Parameters/ParamSweaMove2",
+    4046985140:"Parameters/ParamSweat1",
     1748059662:"Parameters/ParamSweat2",
     910715833:"Parameters/ParamSweatMove",
+    3872502433:"Parameters/ParamSweatMoveon",
     88717352:"Parameters/ParamSweatOn",
     795172687:"Parameters/ParamSweatOn2",
     663484239:"Parameters/ParamSweatView",
     4237388283:"Parameters/ParamSweatView2",
+    4282366110:"Parameters/ParamSweatonoff",
     2170085279:"Parameters/ParamSwingA",
     407997989:"Parameters/ParamSwingB",
     1867955891:"Parameters/ParamSwingC",
     2732879099:"Parameters/ParamSwingCardigan",
     2819788061:"Parameters/ParamSwingCoat",
     4046596880:"Parameters/ParamSwingD",
     2251627398:"Parameters/ParamSwingE",
@@ -907,50 +1194,63 @@
     378144279:"Parameters/ParamSwingJ",
     1192411332:"Parameters/ParamSwingJacket",
     1636644481:"Parameters/ParamSwingK",
     2142601779:"Parameters/ParamSwingKatyusha",
     2776263321:"Parameters/ParamSwingKatyusha2",
     388770144:"Parameters/ParamTailSwing",
     1467020156:"Parameters/ParamTailSwing2",
+    494375721:"Parameters/ParamTasukiHuwaB",
+    1484411378:"Parameters/ParamTasukiHuwaB2",
+    3519964986:"Parameters/ParamTasukiSwingA",
+    3691555288:"Parameters/ParamTasukiSwingA2",
     2436919207:"Parameters/ParamTear",
     1391904809:"Parameters/ParamTear2",
+    3629100631:"Parameters/ParamTear2on",
     636614847:"Parameters/ParamTear3",
     3147132188:"Parameters/ParamTear4",
     1798597939:"Parameters/ParamTearHighlightL",
     2436583504:"Parameters/ParamTearHighlightR",
     3846935570:"Parameters/ParamTearL",
     3918103761:"Parameters/ParamTearL2",
     2506119870:"Parameters/ParamTearLine",
     524593521:"Parameters/ParamTearR",
     1036565262:"Parameters/ParamTearR2",
+    905834095:"Parameters/ParamTearon",
     2283503513:"Parameters/ParamTeeth",
     2943939027:"Parameters/ParamTeeth01",
     913416297:"Parameters/ParamTeeth02",
     2475593362:"Parameters/ParamTeeth2",
+    3834232324:"Parameters/ParamTeeth3",
+    3126364231:"Parameters/ParamTemp01",
     1110817175:"Parameters/ParamTieFuwa",
     4241779428:"Parameters/ParamTieSwing",
     561217570:"Parameters/ParamTwintail",
     3461348719:"Parameters/ParamTwintails",
     3340143929:"Parameters/ParamTwintails2",
     2953952687:"Parameters/ParamTwintails3",
     1118730002:"Parameters/ParamTwintailsFuwa",
+    3912130866:"Parameters/ParamTwintailsFuwa2",
     2409744776:"Parameters/ParamTwintailsHangZ",
     4146016103:"Parameters/ParamTwintailsLTwist",
     3468905612:"Parameters/ParamTwintailsRTwist",
     1490014742:"Parameters/ParamTwintailsTwistL",
     2730553205:"Parameters/ParamTwintailsTwistR",
     2127276225:"Parameters/ParamUnderBodyHangZ",
     1513497407:"Parameters/ParamUpperBody",
     4018162809:"Parameters/ParamUpperBodyZ",
     2444971114:"Parameters/ParamVestSwing",
     3269570882:"Parameters/ParamWaistcord1Swing01",
     1541988600:"Parameters/ParamWaistcord1Swing02",
     201222549:"Parameters/ParamWaistcord2ySwing",
+    650216962:"Parameters/ParamWhiskerSwingL",
+    3704535905:"Parameters/ParamWhiskerSwingR",
     921748034:"Parameters/ParamWorkRotate",
     39434875:"Parameters/ParamWrinkle",
+    2074752843:"Parameters/ParamZipperFuwa",
+    1938320277:"Parameters/ParamZipperSwing",
     854485227:"Parameters/Param_Angle_Rotation10",
     1172920445:"Parameters/Param_Angle_Rotation11",
     3705670087:"Parameters/Param_Angle_Rotation12",
     2884057425:"Parameters/Param_Angle_Rotation13",
     897821938:"Parameters/Param_Angle_Rotation14",
     1115987044:"Parameters/Param_Angle_Rotation15",
     3683503582:"Parameters/Param_Angle_Rotation16",
@@ -1066,11 +1366,16 @@
     2945058484:"Parameters/Param_Angle_Rotation_8_ArtMesh329",
     3091906503:"Parameters/Param_Angle_Rotation_8_ArtMesh331",
     3282042381:"Parameters/Param_Angle_Rotation_9_ArtMesh181",
     1033438960:"Parameters/Param_Angle_Rotation_9_ArtMesh325",
     3549915100:"Parameters/Param_Angle_Rotation_9_ArtMesh327",
     875514587:"Parameters/Param_Angle_Rotation_9_ArtMesh329",
     602928040:"Parameters/Param_Angle_Rotation_9_ArtMesh331",
+    2745217400:"Parameters/Paramcheek",
+    2360343793:"Parameters/Paramhighlight",
+    513109378:"Parameters/Paramkiraonoff",
     1809445648:"Parameters/ParamshirtHuwa",
     806432332:"Parameters/ParamshirtSwing",
+    2464978475:"Parameters/Paramtears",
     496017766:"Parameters/Paramtongue",
+    100476007:"Parameters/uruuru",
 }
```

### Comparing `sssekai-0.0.6/sssekai.egg-info/PKG-INFO` & `sssekai-0.0.8/sssekai.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sssekai
-Version: 0.0.6
+Version: 0.0.8
 Home-page: https://github.com/mos9527/sssekai
 Author: greats3an
 Author-email: greats3an@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -40,15 +40,16 @@
                             These can be found at /sdcard/Android/data/com.hermes.mk.asia/files/data/
         usmdemux            Demux Sekai USM Video in a AssetBundle
         abcache             Sekai AssetBundle local cache
                             Downloads/Updates *ALL* PJSK JP assets to local devices.
                             NOTE: The assets can take quite a lot of space (est. 42.5GB for app version 3.3.1) so be prepared
                             NOTE: The AssetBundles *cached* are NOT OBFUSCATED. They can be used as is by various Unity ripping tools (and sssekai by extension)
                                   that supports stripped Unity version (should be 2020.3.21f1. the version is ripped).
-        live2dextract       Extract Sekai Live2D Models in a AssetBundle
+        spineextract        Extract Sekai Spine (Esoteric Spine2D) Models in a AssetBundle
+        mvdata              Query Sekai MV data from AssetBundle
         mitm                Run Sekai API MITM proxy (WIP)
 
 # Usage
 Refer to the Wiki!
 https://github.com/mos9527/sssekai/wiki （附带简中）
 
 # See Also
```

### Comparing `sssekai-0.0.6/sssekai.egg-info/SOURCES.txt` & `sssekai-0.0.8/sssekai.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 sssekai/crypto/__init__.py
 sssekai/entrypoint/__init__.py
 sssekai/entrypoint/abcache.py
 sssekai/entrypoint/abdecrypt.py
 sssekai/entrypoint/apidecrypt.py
 sssekai/entrypoint/live2dextract.py
 sssekai/entrypoint/mitm.py
+sssekai/entrypoint/mvdata.py
 sssekai/entrypoint/spineextract.py
 sssekai/entrypoint/usmdemux.py
 sssekai/fmt/__init__.py
 sssekai/fmt/moc3.py
 sssekai/unity/AnimationClip.py
 sssekai/unity/AssetBundle.py
 sssekai/unity/__init__.py
```

