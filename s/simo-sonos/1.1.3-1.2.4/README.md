# Comparing `tmp/simo-sonos-1.1.3.tar.gz` & `tmp/simo_sonos-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simo-sonos-1.1.3.tar", last modified: Thu Jan 25 14:36:36 2024, max compression
+gzip compressed data, was "simo_sonos-1.2.4.tar", last modified: Sat Apr 27 18:08:09 2024, max compression
```

## Comparing `simo-sonos-1.1.3.tar` & `simo_sonos-1.2.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-01-25 14:36:36.200007 simo-sonos-1.1.3/
--rw-rw-r--   0 simanas   (1000) simanas   (1000)    34916 2021-12-07 14:40:19.000000 simo-sonos-1.1.3/LICENSE.md
--rw-rw-r--   0 simanas   (1000) simanas   (1000)       23 2023-12-22 10:09:15.000000 simo-sonos-1.1.3/MANIFEST.in
--rw-r--r--   0 simanas   (1000) simanas   (1000)      562 2024-01-25 14:36:36.200007 simo-sonos-1.1.3/PKG-INFO
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      756 2023-12-20 12:02:18.000000 simo-sonos-1.1.3/README.rst
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      673 2024-01-25 14:35:37.000000 simo-sonos-1.1.3/pyproject.toml
--rw-rw-r--   0 simanas   (1000) simanas   (1000)       25 2023-12-20 12:01:35.000000 simo-sonos-1.1.3/requirements.txt
--rw-rw-r--   0 simanas   (1000) simanas   (1000)       38 2024-01-25 14:36:36.200007 simo-sonos-1.1.3/setup.cfg
-drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-01-25 14:36:36.148008 simo-sonos-1.1.3/src/
-drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-01-25 14:36:36.160008 simo-sonos-1.1.3/src/simo_sonos/
--rw-rw-r--   0 simanas   (1000) simanas   (1000)        0 2023-10-19 08:06:42.000000 simo-sonos-1.1.3/src/simo_sonos/__init__.py
-drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-01-25 14:36:36.180008 simo-sonos-1.1.3/src/simo_sonos/__pycache__/
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      151 2023-10-19 10:40:26.000000 simo-sonos-1.1.3/src/simo_sonos/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     1377 2024-01-05 07:18:25.000000 simo-sonos-1.1.3/src/simo_sonos/__pycache__/admin.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     3394 2024-01-25 09:15:09.000000 simo-sonos-1.1.3/src/simo_sonos/__pycache__/controllers.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      572 2023-10-20 11:05:20.000000 simo-sonos-1.1.3/src/simo_sonos/__pycache__/forms.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     6398 2024-01-24 10:07:46.000000 simo-sonos-1.1.3/src/simo_sonos/__pycache__/gateways.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     2438 2024-01-05 07:18:25.000000 simo-sonos-1.1.3/src/simo_sonos/__pycache__/models.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      352 2023-10-20 06:26:13.000000 simo-sonos-1.1.3/src/simo_sonos/__pycache__/utils.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      802 2024-01-04 07:20:58.000000 simo-sonos-1.1.3/src/simo_sonos/admin.py
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     4012 2024-01-25 14:35:19.000000 simo-sonos-1.1.3/src/simo_sonos/controllers.py
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      260 2023-10-20 11:05:15.000000 simo-sonos-1.1.3/src/simo_sonos/forms.py
--rw-rw-r--   0 simanas   (1000) simanas   (1000)    10088 2024-01-24 10:07:42.000000 simo-sonos-1.1.3/src/simo_sonos/gateways.py
-drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-01-25 14:36:36.188007 simo-sonos-1.1.3/src/simo_sonos/migrations/
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     1585 2023-12-20 11:12:53.000000 simo-sonos-1.1.3/src/simo_sonos/migrations/0001_initial.py
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      362 2023-12-20 11:08:35.000000 simo-sonos-1.1.3/src/simo_sonos/migrations/0002_rename_master_sonosplayer_slave_of.py
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      414 2023-12-20 11:08:55.000000 simo-sonos-1.1.3/src/simo_sonos/migrations/0003_alter_sonosplaylist_item_id.py
--rw-rw-r--   0 simanas   (1000) simanas   (1000)        0 2023-10-20 10:25:49.000000 simo-sonos-1.1.3/src/simo_sonos/migrations/__init__.py
-drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-01-25 14:36:36.196007 simo-sonos-1.1.3/src/simo_sonos/migrations/__pycache__/
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     1319 2023-12-20 11:12:56.000000 simo-sonos-1.1.3/src/simo_sonos/migrations/__pycache__/0001_initial.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      586 2023-12-20 11:08:58.000000 simo-sonos-1.1.3/src/simo_sonos/migrations/__pycache__/0002_rename_master_sonosplayer_slave_of.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      651 2023-12-20 11:08:58.000000 simo-sonos-1.1.3/src/simo_sonos/migrations/__pycache__/0003_alter_sonosplaylist_item_id.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      162 2023-10-20 10:25:49.000000 simo-sonos-1.1.3/src/simo_sonos/migrations/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     1773 2024-01-04 07:41:47.000000 simo-sonos-1.1.3/src/simo_sonos/models.py
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      140 2023-10-19 13:41:27.000000 simo-sonos-1.1.3/src/simo_sonos/utils.py
-drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-01-25 14:36:36.196007 simo-sonos-1.1.3/src/simo_sonos.egg-info/
--rw-r--r--   0 simanas   (1000) simanas   (1000)      562 2024-01-25 14:36:36.000000 simo-sonos-1.1.3/src/simo_sonos.egg-info/PKG-INFO
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     1302 2024-01-25 14:36:36.000000 simo-sonos-1.1.3/src/simo_sonos.egg-info/SOURCES.txt
--rw-rw-r--   0 simanas   (1000) simanas   (1000)        1 2024-01-25 14:36:36.000000 simo-sonos-1.1.3/src/simo_sonos.egg-info/dependency_links.txt
--rw-rw-r--   0 simanas   (1000) simanas   (1000)       25 2024-01-25 14:36:36.000000 simo-sonos-1.1.3/src/simo_sonos.egg-info/requires.txt
--rw-rw-r--   0 simanas   (1000) simanas   (1000)       11 2024-01-25 14:36:36.000000 simo-sonos-1.1.3/src/simo_sonos.egg-info/top_level.txt
+drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-04-27 18:08:09.976063 simo_sonos-1.2.4/
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)    34916 2021-12-07 14:40:19.000000 simo_sonos-1.2.4/LICENSE.md
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)       23 2023-12-22 10:09:15.000000 simo_sonos-1.2.4/MANIFEST.in
+-rw-r--r--   0 simanas   (1000) simanas   (1000)      562 2024-04-27 18:08:09.976063 simo_sonos-1.2.4/PKG-INFO
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      756 2023-12-20 12:02:18.000000 simo_sonos-1.2.4/README.rst
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      673 2024-04-27 18:07:19.000000 simo_sonos-1.2.4/pyproject.toml
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)       25 2023-12-20 12:01:35.000000 simo_sonos-1.2.4/requirements.txt
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)       38 2024-04-27 18:08:09.980063 simo_sonos-1.2.4/setup.cfg
+drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-04-27 18:08:09.956063 simo_sonos-1.2.4/src/
+drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-04-27 18:08:09.968063 simo_sonos-1.2.4/src/simo_sonos/
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)        0 2023-10-19 08:06:42.000000 simo_sonos-1.2.4/src/simo_sonos/__init__.py
+drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-04-27 18:08:09.972063 simo_sonos-1.2.4/src/simo_sonos/__pycache__/
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      151 2023-10-19 10:40:26.000000 simo_sonos-1.2.4/src/simo_sonos/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     1377 2024-01-05 07:18:25.000000 simo_sonos-1.2.4/src/simo_sonos/__pycache__/admin.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     2770 2024-02-09 13:12:49.000000 simo_sonos-1.2.4/src/simo_sonos/__pycache__/controllers.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      572 2023-10-20 11:05:20.000000 simo_sonos-1.2.4/src/simo_sonos/__pycache__/forms.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     6888 2024-02-08 13:19:21.000000 simo_sonos-1.2.4/src/simo_sonos/__pycache__/gateways.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     2438 2024-01-05 07:18:25.000000 simo_sonos-1.2.4/src/simo_sonos/__pycache__/models.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      352 2023-10-20 06:26:13.000000 simo_sonos-1.2.4/src/simo_sonos/__pycache__/utils.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      802 2024-01-04 07:20:58.000000 simo_sonos-1.2.4/src/simo_sonos/admin.py
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     2604 2024-04-27 18:03:14.000000 simo_sonos-1.2.4/src/simo_sonos/controllers.py
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      260 2023-10-20 11:05:15.000000 simo_sonos-1.2.4/src/simo_sonos/forms.py
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)    11254 2024-04-27 18:05:00.000000 simo_sonos-1.2.4/src/simo_sonos/gateways.py
+drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-04-27 18:08:09.976063 simo_sonos-1.2.4/src/simo_sonos/migrations/
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     1585 2023-12-20 11:12:53.000000 simo_sonos-1.2.4/src/simo_sonos/migrations/0001_initial.py
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      362 2023-12-20 11:08:35.000000 simo_sonos-1.2.4/src/simo_sonos/migrations/0002_rename_master_sonosplayer_slave_of.py
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      414 2023-12-20 11:08:55.000000 simo_sonos-1.2.4/src/simo_sonos/migrations/0003_alter_sonosplaylist_item_id.py
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)        0 2023-10-20 10:25:49.000000 simo_sonos-1.2.4/src/simo_sonos/migrations/__init__.py
+drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-04-27 18:08:09.976063 simo_sonos-1.2.4/src/simo_sonos/migrations/__pycache__/
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     1319 2023-12-20 11:12:56.000000 simo_sonos-1.2.4/src/simo_sonos/migrations/__pycache__/0001_initial.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      586 2023-12-20 11:08:58.000000 simo_sonos-1.2.4/src/simo_sonos/migrations/__pycache__/0002_rename_master_sonosplayer_slave_of.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      651 2023-12-20 11:08:58.000000 simo_sonos-1.2.4/src/simo_sonos/migrations/__pycache__/0003_alter_sonosplaylist_item_id.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      162 2023-10-20 10:25:49.000000 simo_sonos-1.2.4/src/simo_sonos/migrations/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     1773 2024-01-04 07:41:47.000000 simo_sonos-1.2.4/src/simo_sonos/models.py
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      140 2023-10-19 13:41:27.000000 simo_sonos-1.2.4/src/simo_sonos/utils.py
+drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-04-27 18:08:09.976063 simo_sonos-1.2.4/src/simo_sonos.egg-info/
+-rw-r--r--   0 simanas   (1000) simanas   (1000)      562 2024-04-27 18:08:09.000000 simo_sonos-1.2.4/src/simo_sonos.egg-info/PKG-INFO
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     1302 2024-04-27 18:08:09.000000 simo_sonos-1.2.4/src/simo_sonos.egg-info/SOURCES.txt
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)        1 2024-04-27 18:08:09.000000 simo_sonos-1.2.4/src/simo_sonos.egg-info/dependency_links.txt
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)       25 2024-04-27 18:08:09.000000 simo_sonos-1.2.4/src/simo_sonos.egg-info/requires.txt
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)       11 2024-04-27 18:08:09.000000 simo_sonos-1.2.4/src/simo_sonos.egg-info/top_level.txt
```

### Comparing `simo-sonos-1.1.3/LICENSE.md` & `simo_sonos-1.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `simo-sonos-1.1.3/PKG-INFO` & `simo_sonos-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simo-sonos
-Version: 1.1.3
+Version: 1.2.4
 Summary: SONOS integration for SIMO.io
 Author-email: Simanas Venčkauskas <simanas@simo.io>
 Project-URL: Homepage, https://github.com/SIMO-io/simo-sonos
 Project-URL: Issues, https://github.com/SIMO-io/simo-sonos/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simo-sonos-1.1.3/README.rst` & `simo_sonos-1.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `simo-sonos-1.1.3/pyproject.toml` & `simo_sonos-1.2.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simo-sonos"
-version = "1.1.3"
+version = "1.2.4"
 authors = [
   { name="Simanas Venčkauskas", email="simanas@simo.io" },
 ]
 description = "SONOS integration for SIMO.io"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `simo-sonos-1.1.3/src/simo_sonos/__pycache__/admin.cpython-38.pyc` & `simo_sonos-1.2.4/src/simo_sonos/__pycache__/admin.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `simo-sonos-1.1.3/src/simo_sonos/__pycache__/controllers.cpython-38.pyc` & `simo_sonos-1.2.4/src/simo_sonos/__pycache__/controllers.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jan 25 08:22:06 2024 UTC, .py size: 4011 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,213 +1,174 @@
-00000000: 550d 0d0a 0000 0000 2e1a b265 ab0f 0000  U..........e....
+00000000: 550d 0d0a 0000 0000 e8d4 c465 5e0a 0000  U..........e^...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
+00000020: 0004 0000 0040 0000 0073 8400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6404 6c07 6d08 5a08 0100 6405 6406 6c09  d.l.m.Z...d.d.l.
-00000070: 6d0a 5a0a 6d0b 5a0b 0100 6405 6407 6c0c  m.Z.m.Z...d.d.l.
-00000080: 6d0d 5a0d 0100 6405 6408 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
-00000090: 0100 4700 6409 640a 8400 640a 6506 8303  ..G.d.d...d.e...
-000000a0: 5a10 6401 5300 290b e900 0000 004e 2901  Z.d.S.)......N).
-000000b0: da09 7469 6d65 6465 6c74 6129 01da 0f42  ..timedelta)...B
-000000c0: 6173 6541 7564 696f 506c 6179 6572 2901  aseAudioPlayer).
-000000d0: da14 4761 7465 7761 794f 626a 6563 7443  ..GatewayObjectC
-000000e0: 6f6d 6d61 6e64 e901 0000 0029 02da 0b53  ommand.....)...S
-000000f0: 6f6e 6f73 506c 6179 6572 da0d 536f 6e6f  onosPlayer..Sono
-00000100: 7350 6c61 796c 6973 7429 01da 1353 4f4e  sPlaylist)...SON
-00000110: 4f53 4761 7465 7761 7948 616e 646c 6572  OSGatewayHandler
-00000120: 2901 da15 534f 4e4f 5350 6c61 7965 7243  )...SONOSPlayerC
-00000130: 6f6e 6669 6746 6f72 6d63 0000 0000 0000  onfigFormc......
-00000140: 0000 0000 0000 0000 0000 0300 0000 0000  ................
-00000150: 0000 735a 0000 0065 005a 0164 005a 0265  ..sZ...e.Z.d.Z.e
-00000160: 035a 0465 055a 0664 015a 0764 015a 0887  .Z.e.Z.d.Z.d.Z..
-00000170: 0066 0164 0264 0384 085a 0964 0464 0584  .f.d.d...Z.d.d..
-00000180: 005a 0a64 0f64 0664 0784 015a 0b64 1064  .Z.d.d.d...Z.d.d
-00000190: 0864 0984 015a 0c64 0a64 0b84 005a 0d64  .d...Z.d.d...Z.d
-000001a0: 1164 0d64 0e84 015a 0e87 0004 005a 0f53  .d.d...Z.....Z.S
-000001b0: 0029 12da 0b53 4f4e 4f53 506c 6179 6572  .)...SONOSPlayer
-000001c0: 4e63 0100 0000 0000 0000 0000 0000 0300  Nc..............
-000001d0: 0000 0300 0000 0f00 0000 7354 0000 0074  ..........sT...t
-000001e0: 0083 006a 017c 017c 028e 0101 0074 026a  ...j.|.|.....t.j
-000001f0: 036a 047c 006a 056a 0664 0119 0064 028d  .j.|.j.j.d...d..
-00000200: 01a0 07a1 007c 005f 087c 006a 0872 507c  .....|._.|.j.rP|
-00000210: 006a 087c 006a 055f 087c 006a 086a 097c  .j.|.j._.|.j.j.|
-00000220: 006a 055f 097c 006a 086a 097c 005f 0964  .j._.|.j.j.|._.d
-00000230: 0053 0029 034e da0c 736f 6e6f 735f 6465  .S.).N..sonos_de
-00000240: 7669 6365 a901 da02 6964 290a da05 7375  vice....id)...su
-00000250: 7065 72da 085f 5f69 6e69 745f 5f72 0600  per..__init__r..
-00000260: 0000 da07 6f62 6a65 6374 73da 0666 696c  ....objects..fil
-00000270: 7465 72da 0963 6f6d 706f 6e65 6e74 da06  ter..component..
-00000280: 636f 6e66 6967 da05 6669 7273 74da 0c73  config..first..s
-00000290: 6f6e 6f73 5f70 6c61 7965 72da 0473 6f63  onos_player..soc
-000002a0: 6f29 03da 0473 656c 66da 0461 7267 73da  o)...self..args.
-000002b0: 066b 7761 7267 73a9 01da 095f 5f63 6c61  .kwargs....__cla
-000002c0: 7373 5f5f a900 fa4d 2f68 6f6d 652f 7369  ss__...M/home/si
-000002d0: 6d61 6e61 732f 5072 6f6a 6563 7473 2f53  manas/Projects/S
-000002e0: 494d 4f2f 7061 636b 6167 6573 2f73 696d  IMO/packages/sim
-000002f0: 6f2d 736f 6e6f 732f 7372 632f 7369 6d6f  o-sonos/src/simo
-00000300: 5f73 6f6e 6f73 2f63 6f6e 7472 6f6c 6c65  _sonos/controlle
-00000310: 7273 2e70 7972 0f00 0000 1300 0000 7310  rs.pyr........s.
-00000320: 0000 0000 010e 0106 010a ff0c 0306 010a  ................
-00000330: 010c 017a 1453 4f4e 4f53 506c 6179 6572  ...z.SONOSPlayer
-00000340: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
-00000350: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
-00000360: 0000 7326 0000 007c 006a 0073 1874 0164  ..s&...|.j.s.t.d
-00000370: 0174 026a 0364 028d 0201 0064 0053 007c  .t.j.d.....d.S.|
-00000380: 006a 00a0 04a1 0001 0064 0053 0029 034e  .j.......d.S.).N
-00000390: fa0f 4e4f 2053 4f43 4f20 706c 6179 6572  ..NO SOCO player
-000003a0: 21a9 01da 0466 696c 6529 0572 1600 0000  !....file).r....
-000003b0: da05 7072 696e 74da 0373 7973 da06 7374  ..print..sys..st
-000003c0: 6465 7272 da06 756e 6a6f 696e 2901 7217  derr..unjoin).r.
-000003d0: 0000 0072 1c00 0000 721c 0000 0072 1d00  ...r....r....r..
-000003e0: 0000 7224 0000 001d 0000 0073 0800 0000  ..r$.......s....
-000003f0: 0001 0601 0e01 0401 7a12 534f 4e4f 5350  ........z.SONOSP
-00000400: 6c61 7965 722e 756e 6a6f 696e 6303 0000  layer.unjoinc...
-00000410: 0000 0000 0000 0000 0003 0000 0005 0000  ................
-00000420: 0043 0000 0073 3200 0000 7c02 721e 6401  .C...s2...|.r.d.
-00000430: 7c02 0400 0300 6b01 7218 6402 6b01 731e  |.....k.r.d.k.s.
-00000440: 6e02 0100 7400 8201 7c00 a001 7c01 7c02  n...t...|...|.|.
-00000450: 6403 9c02 a101 0100 6400 5300 2904 4e72  d.......d.S.).Nr
-00000460: 0100 0000 e964 0000 0029 02da 0870 6c61  .....d...)...pla
-00000470: 795f 7572 69da 0676 6f6c 756d 6529 02da  y_uri..volume)..
-00000480: 0e41 7373 6572 7469 6f6e 4572 726f 72da  .AssertionError.
-00000490: 0473 656e 6429 0372 1700 0000 da03 7572  .send).r......ur
-000004a0: 6972 2700 0000 721c 0000 0072 1c00 0000  ir'...r....r....
-000004b0: 721d 0000 0072 2600 0000 2300 0000 7306  r....r&...#...s.
-000004c0: 0000 0000 0104 011a 017a 1453 4f4e 4f53  .........z.SONOS
-000004d0: 506c 6179 6572 2e70 6c61 795f 7572 6963  Player.play_uric
-000004e0: 0300 0000 0000 0000 0000 0000 0300 0000  ................
-000004f0: 0500 0000 4300 0000 7346 0000 0074 007c  ....C...sF...t.|
-00000500: 0183 0174 0174 0266 026b 0673 1474 0382  ...t.t.f.k.s.t..
-00000510: 017c 0272 3264 017c 0204 0003 006b 0172  .|.r2d.|.....k.r
-00000520: 2c64 026b 0173 326e 0201 0074 0382 017c  ,d.k.s2n...t...|
-00000530: 00a0 047c 017c 0264 039c 02a1 0101 0064  ...|.|.d.......d
-00000540: 0453 0029 057a 1a56 616c 2063 616e 2062  .S.).z.Val can b
-00000550: 6520 736f 756e 6420 6964 206f 7220 7572  e sound id or ur
-00000560: 6972 0100 0000 7225 0000 0029 02da 0561  ir....r%...)...a
-00000570: 6c65 7274 7227 0000 004e 2905 da04 7479  lertr'...N)...ty
-00000580: 7065 da03 696e 74da 0373 7472 7228 0000  pe..int..strr(..
-00000590: 0072 2900 0000 2903 7217 0000 00da 0376  .r)...).r......v
-000005a0: 616c 7227 0000 0072 1c00 0000 721c 0000  alr'...r....r...
-000005b0: 0072 1d00 0000 da0a 706c 6179 5f61 6c65  .r......play_ale
-000005c0: 7274 2800 0000 7308 0000 0000 0214 0104  rt(...s.........
-000005d0: 011a 017a 1653 4f4e 4f53 506c 6179 6572  ...z.SONOSPlayer
-000005e0: 2e70 6c61 795f 616c 6572 7463 0200 0000  .play_alertc....
-000005f0: 0000 0000 0000 0000 0300 0000 0500 0000  ................
-00000600: 4300 0000 7366 0100 007c 006a 0073 1874  C...sf...|.j.s.t
-00000610: 0164 0174 026a 0364 028d 0201 0064 0053  .d.t.j.d.....d.S
-00000620: 007c 0164 036b 0672 3274 047c 006a 007c  .|.d.k.r2t.|.j.|
-00000630: 0183 0283 0001 0090 016e 1874 057c 0174  .........n.t.|.t
-00000640: 0683 0290 0172 4a64 047c 016b 0672 5e7c  .....rJd.|.k.r^|
-00000650: 006a 00a0 0774 087c 0164 0419 0064 058d  .j...t.|.d...d..
-00000660: 01a1 0101 006e ec64 067c 016b 0672 747c  .....n.d.|.k.rt|
-00000670: 0164 0619 007c 006a 005f 096e d664 077c  .d...|.j._.n.d.|
-00000680: 016b 0672 8a7c 0164 0719 007c 006a 005f  .k.r.|.d...|.j._
-00000690: 0a6e c064 087c 016b 0672 a07c 0164 0819  .n.d.|.k.r.|.d..
-000006a0: 007c 006a 005f 0b6e aa64 097c 016b 0672  .|.j._.n.d.|.k.r
-000006b0: f07c 0164 0919 00a0 0c64 0aa1 0164 0b6b  .|.d.....d...d.k
-000006c0: 0372 be64 0053 0074 0d6a 0e6a 0f7c 0164  .r.d.S.t.j.j.|.d
-000006d0: 0919 00a0 0c64 0c64 0da1 0264 0e8d 01a0  .....d.d...d....
-000006e0: 10a1 007d 027c 0273 e464 0053 007c 00a0  ...}.|.s.d.S.|..
-000006f0: 117c 02a1 0101 006e 5a64 0f7c 016b 0690  .|.....nZd.|.k..
-00000700: 0172 287c 01a0 0c64 10a1 0164 006b 0390  .r(|...d...d.k..
-00000710: 0172 167c 0164 1019 007c 006a 005f 097c  .r.|.d...|.j._.|
-00000720: 006a 00a0 127c 0164 0f19 00a1 0101 006e  .j...|.d.......n
-00000730: 2264 117c 016b 0690 0172 4a74 137c 006a  "d.|.k...rJt.|.j
-00000740: 146a 157c 006a 147c 0164 128d 03a0 16a1  .j.|.j.|.d......
-00000750: 0001 0074 137c 006a 146a 157c 006a 1464  ...t.|.j.j.|.j.d
-00000760: 1364 128d 03a0 16a1 0001 0064 0053 0029  .d.........d.S.)
-00000770: 144e 721e 0000 0072 1f00 0000 2905 da04  .Nr....r....)...
-00000780: 706c 6179 da05 7061 7573 65da 0473 746f  play..pause..sto
-00000790: 70da 046e 6578 74da 0870 7265 7669 6f75  p..next..previou
-000007a0: 73da 0473 6565 6b29 01da 0773 6563 6f6e  s..seek)...secon
-000007b0: 6473 da0a 7365 745f 766f 6c75 6d65 da07  ds..set_volume..
-000007c0: 7368 7566 666c 65da 046c 6f6f 70da 1170  shuffle..loop..p
-000007d0: 6c61 795f 6672 6f6d 5f6c 6962 7261 7279  lay_from_library
-000007e0: 722c 0000 00da 0e73 6f6e 6f73 5f70 6c61  r,.....sonos_pla
-000007f0: 796c 6973 7472 0d00 0000 7201 0000 0072  ylistr....r....r
-00000800: 0c00 0000 7226 0000 0072 2700 0000 722b  ....r&...r'...r+
-00000810: 0000 0029 01da 0773 6574 5f76 616c da0b  ...)...set_val..
-00000820: 6368 6563 6b5f 7374 6174 6529 1772 1600  check_state).r..
-00000830: 0000 7221 0000 0072 2200 0000 7223 0000  ..r!...r"...r#..
-00000840: 00da 0767 6574 6174 7472 da0a 6973 696e  ...getattr..isin
-00000850: 7374 616e 6365 da04 6469 6374 7236 0000  stance..dictr6..
-00000860: 0072 0200 0000 7227 0000 0072 3900 0000  .r....r'...r9...
-00000870: da06 7265 7065 6174 da03 6765 7472 0700  ..repeat..getr..
-00000880: 0000 7210 0000 0072 1100 0000 7214 0000  ..r....r....r...
-00000890: 00da 0d70 6c61 795f 706c 6179 6c69 7374  ...play_playlist
-000008a0: 7226 0000 0072 0400 0000 7212 0000 00da  r&...r....r.....
-000008b0: 0767 6174 6577 6179 da07 7075 626c 6973  .gateway..publis
-000008c0: 6829 0372 1700 0000 da05 7661 6c75 65da  h).r......value.
-000008d0: 0870 6c61 796c 6973 7472 1c00 0000 721c  .playlistr....r.
-000008e0: 0000 0072 1d00 0000 da0f 5f73 656e 645f  ...r......_send_
-000008f0: 746f 5f64 6576 6963 652f 0000 0073 4c00  to_device/...sL.
-00000900: 0000 0001 0601 0e01 0401 0803 1201 0c01  ................
-00000910: 0801 1801 0801 0e01 0801 0e01 0801 0e01  ................
-00000920: 0801 1201 0401 0601 0eff 0a03 0401 0401  ................
-00000930: 0c01 0a01 1001 0c01 1201 0a01 0201 0600  ................
-00000940: 0401 02fe 0a05 0201 0600 0400 02ff 7a1b  ..............z.
-00000950: 534f 4e4f 5350 6c61 7965 722e 5f73 656e  SONOSPlayer._sen
-00000960: 645f 746f 5f64 6576 6963 6554 6304 0000  d_to_deviceTc...
-00000970: 0000 0000 0000 0000 0007 0000 0008 0000  ................
-00000980: 0043 0000 0073 c400 0000 7c00 6a00 730a  .C...s....|.j.s.
-00000990: 6400 5300 7c00 6a00 6a01 a002 a100 4400  d.S.|.j.j.....D.
-000009a0: 5da8 7d04 7c04 6a03 7c01 6b02 7216 7a74  ].}.|.j.|.k.r.zt
-000009b0: 7c00 6a01 6a04 7d05 7c05 733a 5700 0100  |.j.j.}.|.s:W...
-000009c0: 6400 5300 7c00 6a01 a005 a100 0100 7c02  d.S.|.j.......|.
-000009d0: 7c00 6a01 5f06 7c03 7c00 6a01 5f07 7c00  |.j._.|.|.j._.|.
-000009e0: 6a01 a008 7c04 a101 0100 6401 7d06 7c02  j...|.....d.}.|.
-000009f0: 7278 7409 a00a 6401 7c05 6402 1800 a102  rxt...d.|.d.....
-00000a00: 7d06 7c00 6a01 a00b 7c06 a101 0100 6403  }.|.j...|.....d.
-00000a10: 7c00 6a0c 5f0d 7c00 6a0c a00e a100 0100  |.j._.|.j.......
-00000a20: 5700 6e1e 0100 0100 0100 740f 7410 a011  W.n.......t.t...
-00000a30: a100 7412 6a13 6404 8d02 0100 5900 6e02  ..t.j.d.....Y.n.
-00000a40: 5800 0100 6400 5300 7116 6400 5300 2905  X...d.S.q.d.S.).
-00000a50: 4e72 0100 0000 7205 0000 00da 0770 6c61  Nr....r......pla
-00000a60: 7969 6e67 721f 0000 0029 1472 1500 0000  yingr....).r....
-00000a70: 7216 0000 00da 1367 6574 5f73 6f6e 6f73  r......get_sonos
-00000a80: 5f70 6c61 796c 6973 7473 da07 6974 656d  _playlists..item
-00000a90: 5f69 64da 0a71 7565 7565 5f73 697a 65da  _id..queue_size.
-00000aa0: 0b63 6c65 6172 5f71 7565 7565 7239 0000  .clear_queuer9..
-00000ab0: 0072 4200 0000 da0c 6164 645f 746f 5f71  .rB.....add_to_q
-00000ac0: 7565 7565 da06 7261 6e64 6f6d da07 7261  ueue..random..ra
-00000ad0: 6e64 696e 74da 0f70 6c61 795f 6672 6f6d  ndint..play_from
-00000ae0: 5f71 7565 7565 7212 0000 0072 4700 0000  _queuer....rG...
-00000af0: da04 7361 7665 7221 0000 00da 0974 7261  ..saver!.....tra
-00000b00: 6365 6261 636b da0a 666f 726d 6174 5f65  ceback..format_e
-00000b10: 7863 7222 0000 0072 2300 0000 2907 7217  xcr"...r#...).r.
-00000b20: 0000 0072 4c00 0000 7239 0000 0072 4200  ...rL...r9...rB.
-00000b30: 0000 5a04 706c 7374 5a08 7175 655f 7369  ..Z.plstZ.que_si
-00000b40: 7a65 da0a 7374 6172 745f 6672 6f6d 721c  ze..start_fromr.
-00000b50: 0000 0072 1c00 0000 721d 0000 0072 4400  ...r....r....rD.
-00000b60: 0000 5700 0000 7330 0000 0000 0106 0104  ..W...s0........
-00000b70: 0110 010a 0102 0108 0104 0108 010a 0108  ................
-00000b80: 0108 010c 0104 0104 0104 0102 0006 ff04  ................
-00000b90: 030c 0108 010e 0106 0118 017a 1953 4f4e  ...........z.SON
-00000ba0: 4f53 506c 6179 6572 2e70 6c61 795f 706c  OSPlayer.play_pl
-00000bb0: 6179 6c69 7374 2901 4e29 014e 2902 5454  aylist).N).N).TT
-00000bc0: 2910 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-00000bd0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00000be0: 6e61 6d65 5f5f 7208 0000 00da 0d67 6174  name__r......gat
-00000bf0: 6577 6179 5f63 6c61 7373 7209 0000 00da  eway_classr.....
-00000c00: 0b63 6f6e 6669 675f 666f 726d 7215 0000  .config_formr...
-00000c10: 0072 1600 0000 720f 0000 0072 2400 0000  .r....r....r$...
-00000c20: 7226 0000 0072 3000 0000 7249 0000 0072  r&...r0...rI...r
-00000c30: 4400 0000 da0d 5f5f 636c 6173 7363 656c  D.....__classcel
-00000c40: 6c5f 5f72 1c00 0000 721c 0000 0072 1a00  l__r....r....r..
-00000c50: 0000 721d 0000 0072 0a00 0000 0c00 0000  ..r....r........
-00000c60: 7314 0000 0008 0104 0104 0204 0104 020c  s...............
-00000c70: 0a08 060a 050a 0708 2872 0a00 0000 2911  ........(r....).
-00000c80: 7254 0000 0072 2200 0000 7250 0000 00da  rT...r"...rP....
-00000c90: 0864 6174 6574 696d 6572 0200 0000 5a1b  .datetimer....Z.
-00000ca0: 7369 6d6f 2e6d 756c 7469 6d65 6469 612e  simo.multimedia.
-00000cb0: 636f 6e74 726f 6c6c 6572 7372 0300 0000  controllersr....
-00000cc0: da10 7369 6d6f 2e63 6f72 652e 6576 656e  ..simo.core.even
-00000cd0: 7473 7204 0000 00da 066d 6f64 656c 7372  tsr......modelsr
-00000ce0: 0600 0000 7207 0000 00da 0867 6174 6577  ....r......gatew
-00000cf0: 6179 7372 0800 0000 da05 666f 726d 7372  aysr......formsr
-00000d00: 0900 0000 720a 0000 0072 1c00 0000 721c  ....r....r....r.
-00000d10: 0000 0072 1c00 0000 721d 0000 00da 083c  ...r....r......<
-00000d20: 6d6f 6475 6c65 3e01 0000 0073 1200 0000  module>....s....
-00000d30: 0801 0801 0801 0c01 0c01 0c01 1001 0c01  ................
-00000d40: 0c03                                     ..
+00000060: 6404 6c07 6d08 5a08 0100 6400 6405 6c09  d.l.m.Z...d.d.l.
+00000070: 6d0a 5a0a 0100 6406 6407 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
+00000080: 6d0d 5a0d 0100 6406 6408 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
+00000090: 0100 6406 6409 6c10 6d11 5a11 0100 4700  ..d.d.l.m.Z...G.
+000000a0: 640a 640b 8400 640b 6508 8303 5a12 6401  d.d...d.e...Z.d.
+000000b0: 5300 290c e900 0000 004e 2901 da09 7469  S.)......N)...ti
+000000c0: 6d65 6465 6c74 6129 01da 0f56 616c 6964  medelta)...Valid
+000000d0: 6174 696f 6e45 7272 6f72 2901 da0f 4261  ationError)...Ba
+000000e0: 7365 4175 6469 6f50 6c61 7965 7229 01da  seAudioPlayer)..
+000000f0: 1447 6174 6577 6179 4f62 6a65 6374 436f  .GatewayObjectCo
+00000100: 6d6d 616e 64e9 0100 0000 2902 da0b 536f  mmand.....)...So
+00000110: 6e6f 7350 6c61 7965 72da 0d53 6f6e 6f73  nosPlayer..Sonos
+00000120: 506c 6179 6c69 7374 2901 da13 534f 4e4f  Playlist)...SONO
+00000130: 5347 6174 6577 6179 4861 6e64 6c65 7229  SGatewayHandler)
+00000140: 01da 1553 4f4e 4f53 506c 6179 6572 436f  ...SONOSPlayerCo
+00000150: 6e66 6967 466f 726d 6300 0000 0000 0000  nfigFormc.......
+00000160: 0000 0000 0000 0000 0004 0000 0000 0000  ................
+00000170: 0073 6000 0000 6500 5a01 6400 5a02 6503  .s`...e.Z.d.Z.e.
+00000180: 5a04 6505 5a06 6401 5a07 6401 5a08 8700  Z.e.Z.d.Z.d.Z...
+00000190: 6601 6402 6403 8408 5a09 6404 6405 8400  f.d.d...Z.d.d...
+000001a0: 5a0a 640f 6406 6407 8401 5a0b 6410 6408  Z.d.d.d...Z.d.d.
+000001b0: 6409 8401 5a0c 6411 8700 6601 640a 640b  d...Z.d...f.d.d.
+000001c0: 8409 5a0d 6412 640d 640e 8401 5a0e 8700  ..Z.d.d.d...Z...
+000001d0: 0400 5a0f 5300 2913 da0b 534f 4e4f 5350  ..Z.S.)...SONOSP
+000001e0: 6c61 7965 724e 6301 0000 0000 0000 0000  layerNc.........
+000001f0: 0000 0003 0000 0003 0000 000f 0000 0073  ...............s
+00000200: 5400 0000 7400 8300 6a01 7c01 7c02 8e01  T...t...j.|.|...
+00000210: 0100 7402 6a03 6a04 7c00 6a05 6a06 6401  ..t.j.j.|.j.j.d.
+00000220: 1900 6402 8d01 a007 a100 7c00 5f08 7c00  ..d.......|._.|.
+00000230: 6a08 7250 7c00 6a08 7c00 6a05 5f08 7c00  j.rP|.j.|.j._.|.
+00000240: 6a08 6a09 7c00 6a05 5f09 7c00 6a08 6a09  j.j.|.j._.|.j.j.
+00000250: 7c00 5f09 6400 5300 2903 4eda 0c73 6f6e  |._.d.S.).N..son
+00000260: 6f73 5f64 6576 6963 6529 01da 0269 6429  os_device)...id)
+00000270: 0ada 0573 7570 6572 da08 5f5f 696e 6974  ...super..__init
+00000280: 5f5f 7207 0000 00da 076f 626a 6563 7473  __r......objects
+00000290: da06 6669 6c74 6572 da09 636f 6d70 6f6e  ..filter..compon
+000002a0: 656e 74da 0663 6f6e 6669 67da 0566 6972  ent..config..fir
+000002b0: 7374 da0c 736f 6e6f 735f 706c 6179 6572  st..sonos_player
+000002c0: da04 736f 636f 2903 da04 7365 6c66 da04  ..soco)...self..
+000002d0: 6172 6773 da06 6b77 6172 6773 a901 da09  args..kwargs....
+000002e0: 5f5f 636c 6173 735f 5fa9 00fa 4d2f 686f  __class__...M/ho
+000002f0: 6d65 2f73 696d 616e 6173 2f50 726f 6a65  me/simanas/Proje
+00000300: 6374 732f 5349 4d4f 2f70 6163 6b61 6765  cts/SIMO/package
+00000310: 732f 7369 6d6f 2d73 6f6e 6f73 2f73 7263  s/simo-sonos/src
+00000320: 2f73 696d 6f5f 736f 6e6f 732f 636f 6e74  /simo_sonos/cont
+00000330: 726f 6c6c 6572 732e 7079 720f 0000 0014  rollers.pyr.....
+00000340: 0000 0073 1000 0000 0001 0e01 0601 0aff  ...s............
+00000350: 0c03 0601 0a01 0c01 7a14 534f 4e4f 5350  ........z.SONOSP
+00000360: 6c61 7965 722e 5f5f 696e 6974 5f5f 6301  layer.__init__c.
+00000370: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+00000380: 0000 0043 0000 0073 2600 0000 7c00 6a00  ...C...s&...|.j.
+00000390: 7318 7401 6401 7402 6a03 6402 8d02 0100  s.t.d.t.j.d.....
+000003a0: 6400 5300 7c00 6a00 a004 a100 0100 6400  d.S.|.j.......d.
+000003b0: 5300 2903 4efa 0f4e 4f20 534f 434f 2070  S.).N..NO SOCO p
+000003c0: 6c61 7965 7221 a901 da04 6669 6c65 2905  layer!....file).
+000003d0: 7216 0000 00da 0570 7269 6e74 da03 7379  r......print..sy
+000003e0: 73da 0673 7464 6572 72da 0675 6e6a 6f69  s..stderr..unjoi
+000003f0: 6e29 0172 1700 0000 721c 0000 0072 1c00  n).r....r....r..
+00000400: 0000 721d 0000 0072 2400 0000 1e00 0000  ..r....r$.......
+00000410: 7308 0000 0000 0106 010e 0104 017a 1253  s............z.S
+00000420: 4f4e 4f53 506c 6179 6572 2e75 6e6a 6f69  ONOSPlayer.unjoi
+00000430: 6e63 0300 0000 0000 0000 0000 0000 0300  nc..............
+00000440: 0000 0500 0000 4300 0000 7332 0000 007c  ......C...s2...|
+00000450: 0272 1e64 017c 0204 0003 006b 0172 1864  .r.d.|.....k.r.d
+00000460: 026b 0173 1e6e 0201 0074 0082 017c 00a0  .k.s.n...t...|..
+00000470: 017c 017c 0264 039c 02a1 0101 0064 0053  .|.|.d.......d.S
+00000480: 0029 044e 7201 0000 00e9 6400 0000 2902  .).Nr.....d...).
+00000490: da08 706c 6179 5f75 7269 da06 766f 6c75  ..play_uri..volu
+000004a0: 6d65 2902 da0e 4173 7365 7274 696f 6e45  me)...AssertionE
+000004b0: 7272 6f72 da04 7365 6e64 2903 7217 0000  rror..send).r...
+000004c0: 00da 0375 7269 7227 0000 0072 1c00 0000  ...urir'...r....
+000004d0: 721c 0000 0072 1d00 0000 7226 0000 0024  r....r....r&...$
+000004e0: 0000 0073 0600 0000 0001 0401 1a01 7a14  ...s..........z.
+000004f0: 534f 4e4f 5350 6c61 7965 722e 706c 6179  SONOSPlayer.play
+00000500: 5f75 7269 6303 0000 0000 0000 0000 0000  _uric...........
+00000510: 0003 0000 0005 0000 0043 0000 0073 4600  .........C...sF.
+00000520: 0000 7400 7c01 8301 7401 7402 6602 6b06  ..t.|...t.t.f.k.
+00000530: 7314 7403 8201 7c02 7232 6401 7c02 0400  s.t...|.r2d.|...
+00000540: 0300 6b01 722c 6402 6b01 7332 6e02 0100  ..k.r,d.k.s2n...
+00000550: 7403 8201 7c00 a004 7c01 7c02 6403 9c02  t...|...|.|.d...
+00000560: a101 0100 6404 5300 2905 7a1a 5661 6c20  ....d.S.).z.Val 
+00000570: 6361 6e20 6265 2073 6f75 6e64 2069 6420  can be sound id 
+00000580: 6f72 2075 7269 7201 0000 0072 2500 0000  or urir....r%...
+00000590: 2902 da05 616c 6572 7472 2700 0000 4e29  )...alertr'...N)
+000005a0: 05da 0474 7970 65da 0369 6e74 da03 7374  ...type..int..st
+000005b0: 7272 2800 0000 7229 0000 0029 0372 1700  rr(...r)...).r..
+000005c0: 0000 da03 7661 6c72 2700 0000 721c 0000  ....valr'...r...
+000005d0: 0072 1c00 0000 721d 0000 00da 0a70 6c61  .r....r......pla
+000005e0: 795f 616c 6572 7429 0000 0073 0800 0000  y_alert)...s....
+000005f0: 0002 1401 0401 1a01 7a16 534f 4e4f 5350  ........z.SONOSP
+00000600: 6c61 7965 722e 706c 6179 5f61 6c65 7274  layer.play_alert
+00000610: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
+00000620: 0004 0000 0003 0000 0073 1c00 0000 7c00  .........s....|.
+00000630: 6a00 730e 7401 6401 8301 8201 7402 8300  j.s.t.d.....t...
+00000640: a003 7c01 7c02 a102 5300 2902 4e72 1e00  ..|.|...S.).Nr..
+00000650: 0000 2904 7216 0000 0072 0300 0000 720e  ..).r....r....r.
+00000660: 0000 00da 0d5f 7661 6c69 6461 7465 5f76  ....._validate_v
+00000670: 616c 2903 7217 0000 0072 2f00 0000 da08  al).r....r/.....
+00000680: 6f63 6361 7369 6f6e 721a 0000 0072 1c00  occasionr....r..
+00000690: 0000 721d 0000 0072 3100 0000 3000 0000  ..r....r1...0...
+000006a0: 7306 0000 0000 0106 0108 017a 1953 4f4e  s..........z.SON
+000006b0: 4f53 506c 6179 6572 2e5f 7661 6c69 6461  OSPlayer._valida
+000006c0: 7465 5f76 616c 5463 0400 0000 0000 0000  te_valTc........
+000006d0: 0000 0000 0700 0000 0800 0000 4300 0000  ............C...
+000006e0: 73c4 0000 007c 006a 0073 0a64 0053 007c  s....|.j.s.d.S.|
+000006f0: 006a 006a 01a0 02a1 0044 005d a87d 047c  .j.j.....D.].}.|
+00000700: 046a 037c 016b 0272 167a 747c 006a 01a0  .j.|.k.r.zt|.j..
+00000710: 04a1 0001 007c 027c 006a 015f 057c 037c  .....|.|.j._.|.|
+00000720: 006a 015f 067c 006a 01a0 077c 04a1 0101  .j._.|.j...|....
+00000730: 007c 006a 016a 087d 057c 0573 6057 0001  .|.j.j.}.|.s`W..
+00000740: 0064 0053 0064 017d 067c 0272 7874 09a0  .d.S.d.}.|.rxt..
+00000750: 0a64 017c 0564 0218 00a1 027d 067c 006a  .d.|.d.....}.|.j
+00000760: 01a0 0b7c 06a1 0101 0064 037c 006a 0c5f  ...|.....d.|.j._
+00000770: 0d7c 006a 0ca0 0ea1 0001 0057 006e 1e01  .|.j.......W.n..
+00000780: 0001 0001 0074 0f74 10a0 11a1 0074 126a  .....t.t.....t.j
+00000790: 1364 048d 0201 0059 006e 0258 0001 0064  .d.....Y.n.X...d
+000007a0: 0053 0071 1664 0053 0029 054e 7201 0000  .S.q.d.S.).Nr...
+000007b0: 0072 0600 0000 da07 706c 6179 696e 6772  .r......playingr
+000007c0: 1f00 0000 2914 7215 0000 0072 1600 0000  ....).r....r....
+000007d0: da13 6765 745f 736f 6e6f 735f 706c 6179  ..get_sonos_play
+000007e0: 6c69 7374 73da 0769 7465 6d5f 6964 da0b  lists..item_id..
+000007f0: 636c 6561 725f 7175 6575 65da 0773 6875  clear_queue..shu
+00000800: 6666 6c65 da06 7265 7065 6174 da0c 6164  ffle..repeat..ad
+00000810: 645f 746f 5f71 7565 7565 da0a 7175 6575  d_to_queue..queu
+00000820: 655f 7369 7a65 da06 7261 6e64 6f6d da07  e_size..random..
+00000830: 7261 6e64 696e 74da 0f70 6c61 795f 6672  randint..play_fr
+00000840: 6f6d 5f71 7565 7565 7212 0000 00da 0576  om_queuer......v
+00000850: 616c 7565 da04 7361 7665 7221 0000 00da  alue..saver!....
+00000860: 0974 7261 6365 6261 636b da0a 666f 726d  .traceback..form
+00000870: 6174 5f65 7863 7222 0000 0072 2300 0000  at_excr"...r#...
+00000880: 2907 7217 0000 0072 3500 0000 7237 0000  ).r....r5...r7..
+00000890: 0072 3800 0000 5a04 706c 7374 5a08 7175  .r8...Z.plstZ.qu
+000008a0: 655f 7369 7a65 da0a 7374 6172 745f 6672  e_size..start_fr
+000008b0: 6f6d 721c 0000 0072 1c00 0000 721d 0000  omr....r....r...
+000008c0: 00da 0d70 6c61 795f 706c 6179 6c69 7374  ...play_playlist
+000008d0: 3500 0000 7330 0000 0000 0106 0104 0110  5...s0..........
+000008e0: 010a 0102 020a 0108 0108 010c 0108 0104  ................
+000008f0: 0108 0104 0104 0104 0102 0006 ff04 030c  ................
+00000900: 0108 010e 0106 0118 017a 1953 4f4e 4f53  .........z.SONOS
+00000910: 506c 6179 6572 2e70 6c61 795f 706c 6179  Player.play_play
+00000920: 6c69 7374 2901 4e29 014e 2901 4e29 0254  list).N).N).N).T
+00000930: 5429 10da 085f 5f6e 616d 655f 5fda 0a5f  T)...__name__.._
+00000940: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000950: 6c6e 616d 655f 5f72 0900 0000 da0d 6761  lname__r......ga
+00000960: 7465 7761 795f 636c 6173 7372 0a00 0000  teway_classr....
+00000970: da0b 636f 6e66 6967 5f66 6f72 6d72 1500  ..config_formr..
+00000980: 0000 7216 0000 0072 0f00 0000 7224 0000  ..r....r....r$..
+00000990: 0072 2600 0000 7230 0000 0072 3100 0000  .r&...r0...r1...
+000009a0: 7243 0000 00da 0d5f 5f63 6c61 7373 6365  rC.....__classce
+000009b0: 6c6c 5f5f 721c 0000 0072 1c00 0000 721a  ll__r....r....r.
+000009c0: 0000 0072 1d00 0000 720b 0000 000d 0000  ...r....r.......
+000009d0: 0073 1400 0000 0801 0401 0402 0401 0402  .s..............
+000009e0: 0c0a 0806 0a05 0a07 0e05 720b 0000 0029  ..........r....)
+000009f0: 1372 4000 0000 7222 0000 0072 3b00 0000  .r@...r"...r;...
+00000a00: da08 6461 7465 7469 6d65 7202 0000 00da  ..datetimer.....
+00000a10: 1664 6a61 6e67 6f2e 636f 7265 2e65 7863  .django.core.exc
+00000a20: 6570 7469 6f6e 7372 0300 0000 5a1b 7369  eptionsr....Z.si
+00000a30: 6d6f 2e6d 756c 7469 6d65 6469 612e 636f  mo.multimedia.co
+00000a40: 6e74 726f 6c6c 6572 7372 0400 0000 da10  ntrollersr......
+00000a50: 7369 6d6f 2e63 6f72 652e 6576 656e 7473  simo.core.events
+00000a60: 7205 0000 00da 066d 6f64 656c 7372 0700  r......modelsr..
+00000a70: 0000 7208 0000 00da 0867 6174 6577 6179  ..r......gateway
+00000a80: 7372 0900 0000 da05 666f 726d 7372 0a00  sr......formsr..
+00000a90: 0000 720b 0000 0072 1c00 0000 721c 0000  ..r....r....r...
+00000aa0: 0072 1c00 0000 721d 0000 00da 083c 6d6f  .r....r......<mo
+00000ab0: 6475 6c65 3e01 0000 0073 1400 0000 0801  dule>....s......
+00000ac0: 0801 0801 0c01 0c01 0c01 0c01 1001 0c01  ................
+00000ad0: 0c03                                     ..
```

### Comparing `simo-sonos-1.1.3/src/simo_sonos/__pycache__/forms.cpython-38.pyc` & `simo_sonos-1.2.4/src/simo_sonos/__pycache__/forms.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `simo-sonos-1.1.3/src/simo_sonos/__pycache__/gateways.cpython-38.pyc` & `simo_sonos-1.2.4/src/simo_sonos/__pycache__/gateways.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Jan 24 10:07:42 2024 UTC, .py size: 10088 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6ee1 b065 6827 0000  U.......n..eh'..
+00000000: 550d 0d0a 0000 0000 d5d4 c465 c82b 0000  U..........e.+..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 0100 6400 6405 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6406 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
@@ -34,367 +34,398 @@
 00000210: 0e64 1053 0029 11da 1353 4f4e 4f53 4761  .d.S.)...SONOSGa
 00000220: 7465 7761 7948 616e 646c 6572 5a05 534f  tewayHandlerZ.SO
 00000230: 4e4f 5329 0229 02da 1a70 6572 696f 6469  NOS).)...periodi
 00000240: 635f 706c 6179 6572 735f 6469 7363 6f76  c_players_discov
 00000250: 6572 7969 5802 0000 2902 da0d 7761 7463  eryiX...)...watc
 00000260: 685f 706c 6179 6572 7372 0c00 0000 7201  h_playersr....r.
 00000270: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
-00000280: 0800 0000 0800 0000 4300 0000 73b2 0000  ........C...s...
+00000280: 0900 0000 0800 0000 4300 0000 73b8 0100  ........C...s...
 00000290: 0074 006a 016a 027c 016a 0364 0119 0064  .t.j.j.|.j.d...d
-000002a0: 028d 017d 037c 0264 036b 0272 287c 00a0  ...}.|.d.k.r(|..
-000002b0: 047c 01a1 0101 006e 8674 057c 0274 0683  .|.....n.t.|.t..
-000002c0: 0272 ae64 047c 026b 0672 ae7a 1074 077c  .r.d.|.k.r.z.t.|
-000002d0: 0264 0419 0083 017d 0457 006e 1801 0001  .d.....}.W.n....
-000002e0: 0001 007c 0264 0419 007d 0564 007d 0659  ...|.d...}.d.}.Y
-000002f0: 006e 2a58 0074 086a 016a 027c 0464 058d  .n*X.t.j.j.|.d..
-00000300: 017d 077c 076a 097d 0664 0674 0a83 009b  .}.|.j.}.d.t....
-00000310: 007c 07a0 0ba1 009b 009d 037d 0574 0c6a  .|.........}.t.j
-00000320: 0d7c 006a 0e7c 037c 057c 067c 02a0 0264  .|.j.|.|.|.|...d
-00000330: 07a1 0166 0464 088d 02a0 0fa1 0001 0064  ...f.d.........d
-00000340: 0053 0029 094e da0c 736f 6e6f 735f 6465  .S.).N..sonos_de
-00000350: 7669 6365 a901 da02 6964 5a0b 6368 6563  vice....idZ.chec
-00000360: 6b5f 7374 6174 65da 0561 6c65 7274 2901  k_state..alert).
-00000370: da02 706b 7a07 6874 7470 3a2f 2fda 0676  ..pkz.http://..v
-00000380: 6f6c 756d 6529 02da 0674 6172 6765 74da  olume)...target.
-00000390: 0461 7267 7329 1072 0d00 0000 da07 6f62  .args).r......ob
-000003a0: 6a65 6374 73da 0367 6574 da06 636f 6e66  jects..get..conf
-000003b0: 6967 da11 636f 6d70 5f73 7461 7465 5f75  ig..comp_state_u
-000003c0: 7064 6174 65da 0a69 7369 6e73 7461 6e63  pdate..isinstanc
-000003d0: 65da 0464 6963 74da 0369 6e74 720b 0000  e..dict..intr...
-000003e0: 00da 066c 656e 6774 6872 0a00 0000 da10  ...lengthr......
-000003f0: 6765 745f 6162 736f 6c75 7465 5f75 726c  get_absolute_url
-00000400: da09 7468 7265 6164 696e 67da 0654 6872  ..threading..Thr
-00000410: 6561 64da 0a70 6c61 795f 616c 6572 74da  ead..play_alert.
-00000420: 0573 7461 7274 2908 da04 7365 6c66 da09  .start)...self..
-00000430: 636f 6d70 6f6e 656e 74da 0576 616c 7565  component..value
-00000440: da0c 736f 6e6f 735f 706c 6179 6572 5a08  ..sonos_playerZ.
-00000450: 736f 756e 645f 6964 da03 7572 6972 2200  sound_id..urir".
-00000460: 0000 da05 736f 756e 64a9 0072 2e00 0000  ....sound..r....
-00000470: fa4a 2f68 6f6d 652f 7369 6d61 6e61 732f  .J/home/simanas/
-00000480: 5072 6f6a 6563 7473 2f53 494d 4f2f 7061  Projects/SIMO/pa
-00000490: 636b 6167 6573 2f73 696d 6f2d 736f 6e6f  ckages/simo-sono
-000004a0: 732f 7372 632f 7369 6d6f 5f73 6f6e 6f73  s/src/simo_sonos
-000004b0: 2f67 6174 6577 6179 732e 7079 da12 7065  /gateways.py..pe
-000004c0: 7266 6f72 6d5f 7661 6c75 655f 7365 6e64  rform_value_send
-000004d0: 1c00 0000 732a 0000 0000 0114 0108 010c  ....s*..........
-000004e0: 020a 0108 0102 0110 0106 0108 010a 020e  ................
-000004f0: 0106 0114 0204 0104 0102 0002 0002 0008  ................
-00000500: ff02 ff7a 2653 4f4e 4f53 4761 7465 7761  ...z&SONOSGatewa
-00000510: 7948 616e 646c 6572 2e70 6572 666f 726d  yHandler.perform
-00000520: 5f76 616c 7565 5f73 656e 6463 0500 0000  _value_sendc....
-00000530: 0000 0000 0000 0000 0a00 0000 0a00 0000  ................
-00000540: 4300 0000 7342 0200 007c 016a 007c 006a  C...sB...|.j.|.j
-00000550: 016b 0772 4074 027c 016a 0383 017c 0274  .k.r@t.|.j...|.t
-00000560: 04a0 04a1 0064 019c 037c 006a 017c 016a  .....d...|.j.|.j
-00000570: 003c 007c 006a 017c 016a 0019 0064 0219  .<.|.j.|.j...d..
-00000580: 00a0 05a1 0001 006e 1c7c 006a 017c 016a  .......n.|.j.|.j
-00000590: 0019 00a0 067c 0274 04a0 04a1 0064 039c  .....|.t.....d..
-000005a0: 02a1 0101 007c 006a 017c 016a 0019 0064  .....|.j.|.j...d
-000005b0: 0419 007d 057c 0464 006b 0372 7c7c 047c  ...}.|.d.k.r||.|
-000005c0: 016a 035f 0774 0864 057c 0283 0201 007c  .j._.t.d.|.....|
-000005d0: 016a 03a0 09a1 0001 0064 067c 016a 035f  .j.......d.|.j._
-000005e0: 0a7c 016a 03a0 0ba1 0001 007c 016a 03a0  .|.j.......|.j..
-000005f0: 0c7c 02a1 0101 007c 0364 006b 0372 ce7c  .|.....|.d.k.r.|
-00000600: 0364 076b 0472 c264 077d 0374 04a0 0d7c  .d.k.r.d.}.t...|
-00000610: 03a1 0101 006e 3874 0e64 0783 0144 005d  .....n8t.d...D.]
-00000620: 2e7d 0674 04a0 0d64 08a1 0101 007c 016a  .}.t...d.....|.j
-00000630: 03a0 0fa1 007d 077c 07a0 1064 0964 0aa1  .....}.|...d.d..
-00000640: 0264 0a6b 0372 d601 0090 0171 0671 d67c  .d.k.r.....q.q.|
-00000650: 006a 01a0 107c 016a 0069 00a1 02a0 1064  .j...|.j.i.....d
-00000660: 0464 0ba1 027c 056b 0390 0172 2864 0053  .d...|.k...r(d.S
-00000670: 007c 006a 01a0 107c 016a 0069 00a1 02a0  .|.j...|.j.i....
-00000680: 1064 0c64 0da1 027c 026b 0390 0172 4a64  .d.d...|.k...rJd
-00000690: 0053 007c 016a 03a0 11a1 007d 087c 08a0  .S.|.j.....}.|..
-000006a0: 1064 0ca1 0190 0172 8c7c 08a0 1064 0ca1  .d.....r.|...d..
-000006b0: 017c 026b 0390 0172 8c7c 016a 007c 006a  .|.k...r.|.j.|.j
-000006c0: 016b 0690 0172 887c 006a 017c 016a 003d  .k...r.|.j.|.j.=
-000006d0: 0064 0053 0074 0864 0e83 0101 007c 006a  .d.S.t.d.....|.j
-000006e0: 017c 016a 0019 0064 0219 007d 097a 147c  .|.j...d...}.z.|
-000006f0: 096a 1890 0172 b67c 09a0 19a1 0001 0057  .j...r.|.......W
-00000700: 0035 007c 096a 127c 096a 135f 127c 096a  .5.|.j.|.j._.|.j
-00000710: 147c 096a 135f 147c 096a 157c 096a 135f  .|.j._.|.j.|.j._
-00000720: 157c 096a 167c 096a 135f 1664 0b7c 096a  .|.j.|.j._.d.|.j
-00000730: 135f 077c 096a 136a 177c 096a 0764 0f64  ._.|.j.j.|.j.d.d
-00000740: 108d 0201 0058 007c 096a 1890 0272 347c  .....X.|.j...r4|
-00000750: 096a 1a64 0a6b 0290 0272 1e7c 096a 13a0  .j.d.k...r.|.j..
-00000760: 1ba1 0001 006e 167c 096a 1a64 116b 0290  .....n.|.j.d.k..
-00000770: 0272 347c 096a 13a0 09a1 0001 007c 006a  .r4|.j.......|.j
-00000780: 017c 016a 003d 0064 0053 0029 124e 2903  .|.j.=.d.S.).N).
-00000790: da04 736e 6170 722c 0000 00da 0974 696d  ..snapr,.....tim
-000007a0: 6573 7461 6d70 7231 0000 0029 0272 2c00  estampr1...).r,.
-000007b0: 0000 7232 0000 0072 3200 0000 7a15 506c  ..r2...r2...z.Pl
-000007c0: 6179 2061 6c65 7274 2066 726f 6d20 5552  ay alert from UR
-000007d0: 493a 2046 e93c 0000 0072 0c00 0000 da17  I: F.<...r......
-000007e0: 6375 7272 656e 745f 7472 616e 7370 6f72  current_transpor
-000007f0: 745f 7374 6174 65da 0750 4c41 5949 4e47  t_state..PLAYING
-00000800: 7201 0000 0072 2c00 0000 da00 7a10 5265  r....r,.....z.Re
-00000810: 7374 6f72 6520 6f72 6967 696e 616c 5a12  store originalZ.
-00000820: 4155 544f 504c 4159 5f52 414d 505f 5459  AUTOPLAY_RAMP_TY
-00000830: 5045 2901 5a09 7261 6d70 5f74 7970 65da  PE).Z.ramp_type.
-00000840: 0753 544f 5050 4544 291c 7215 0000 00da  .STOPPED).r.....
-00000850: 0e70 6c61 7969 6e67 5f61 6c65 7274 7372  .playing_alertsr
-00000860: 0600 0000 da04 736f 636f da04 7469 6d65  ......soco..time
-00000870: 5a08 736e 6170 7368 6f74 da06 7570 6461  Z.snapshot..upda
-00000880: 7465 7218 0000 00da 0570 7269 6e74 da04  ter......print..
-00000890: 7374 6f70 da06 7265 7065 6174 5a0b 636c  stop..repeatZ.cl
-000008a0: 6561 725f 7175 6575 655a 0870 6c61 795f  ear_queueZ.play_
-000008b0: 7572 69da 0573 6c65 6570 da05 7261 6e67  uri..sleep..rang
-000008c0: 65da 1a67 6574 5f63 7572 7265 6e74 5f74  e..get_current_t
-000008d0: 7261 6e73 706f 7274 5f69 6e66 6f72 1c00  ransport_infor..
-000008e0: 0000 da16 6765 745f 6375 7272 656e 745f  ....get_current_
-000008f0: 7472 6163 6b5f 696e 666f da04 6d75 7465  track_info..mute
-00000900: da06 6465 7669 6365 5a04 6261 7373 5a06  ..deviceZ.bassZ.
-00000910: 7472 6562 6c65 5a08 6c6f 7564 6e65 7373  trebleZ.loudness
-00000920: 5a0e 7261 6d70 5f74 6f5f 766f 6c75 6d65  Z.ramp_to_volume
-00000930: 5a0e 6973 5f63 6f6f 7264 696e 6174 6f72  Z.is_coordinator
-00000940: 5a14 5f72 6573 746f 7265 5f63 6f6f 7264  Z._restore_coord
-00000950: 696e 6174 6f72 5a0f 7472 616e 7370 6f72  inatorZ.transpor
-00000960: 745f 7374 6174 65da 0470 6c61 7929 0a72  t_state..play).r
-00000970: 2800 0000 722b 0000 0072 2c00 0000 7222  (...r+...r,...r"
-00000980: 0000 0072 1800 0000 5a0f 7374 6172 745f  ...r....Z.start_
-00000990: 7469 6d65 7374 616d 70da 0169 da06 7374  timestamp..i..st
-000009a0: 6174 7573 5a12 6375 7272 656e 745f 7472  atusZ.current_tr
-000009b0: 6163 6b5f 696e 666f 7231 0000 0072 2e00  ack_infor1...r..
-000009c0: 0000 722e 0000 0072 2f00 0000 7226 0000  ..r....r/...r&..
-000009d0: 0033 0000 0073 8200 0000 0001 0c02 0801  .3...s..........
-000009e0: 0200 06fe 0e04 1602 0c01 0200 06ff 0804  ................
-000009f0: 1002 0801 0802 0a01 0a01 0801 0a01 0c02  ................
-00000a00: 0801 0801 0401 0c02 0c01 0a01 0a01 0401  ................
-00000a10: 0200 02ff 0202 02fe 0403 0803 1601 02ff  ................
-00000a20: 0603 0401 1e02 0402 0a01 0c01 0cff 0403  ................
-00000a30: 0e01 0a01 0402 0801 1001 0201 0801 0c02  ................
-00000a40: 0a01 0a01 0a01 0a01 0801 0601 0400 02ff  ................
-00000a50: 0806 0801 0c01 0c01 0c01 0a02 7a1e 534f  ............z.SO
-00000a60: 4e4f 5347 6174 6577 6179 4861 6e64 6c65  NOSGatewayHandle
-00000a70: 722e 706c 6179 5f61 6c65 7274 6301 0000  r.play_alertc...
-00000a80: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000a90: 0043 0000 0073 3600 0000 7c00 a000 a100  .C...s6...|.....
-00000aa0: 0100 7401 6a02 6a03 7c00 6a04 6401 6402  ..t.j.j.|.j.d.d.
-00000ab0: 8d02 6a05 6403 6404 8d01 4400 5d0e 7d01  ..j.d.d...D.].}.
-00000ac0: 7c00 a006 7c01 a101 0100 7122 6400 5300  |...|.....q"d.S.
-00000ad0: 2905 4efa 0c61 7564 696f 2d70 6c61 7965  ).N..audio-playe
-00000ae0: 72a9 02da 0767 6174 6577 6179 da09 6261  r....gateway..ba
-00000af0: 7365 5f74 7970 65da 0770 6c61 7969 6e67  se_type..playing
-00000b00: a901 722a 0000 0029 07da 1664 6973 636f  ..r*...)...disco
-00000b10: 7665 725f 736f 6e6f 735f 706c 6179 6572  ver_sonos_player
-00000b20: 7372 0900 0000 721b 0000 00da 0666 696c  sr....r......fil
-00000b30: 7465 72da 1067 6174 6577 6179 5f69 6e73  ter..gateway_ins
-00000b40: 7461 6e63 65da 0765 7863 6c75 6465 721e  tance..excluder.
-00000b50: 0000 00a9 0272 2800 0000 da04 636f 6d70  .....r(.....comp
-00000b60: 722e 0000 0072 2e00 0000 722f 0000 0072  r....r....r/...r
-00000b70: 1100 0000 8100 0000 7310 0000 0000 0308  ........s.......
-00000b80: 0106 0104 0002 ff06 0202 fe0a 037a 2e53  .............z.S
-00000b90: 4f4e 4f53 4761 7465 7761 7948 616e 646c  ONOSGatewayHandl
-00000ba0: 6572 2e70 6572 696f 6469 635f 706c 6179  er.periodic_play
-00000bb0: 6572 735f 6469 7363 6f76 6572 7963 0100  ers_discoveryc..
-00000bc0: 0000 0000 0000 0000 0000 0200 0000 0500  ................
-00000bd0: 0000 4300 0000 7372 0000 0074 006a 016a  ..C...sr...t.j.j
-00000be0: 027c 006a 0364 0164 0264 038d 0344 005d  .|.j.d.d.d...D.]
-00000bf0: 0e7d 017c 00a0 047c 01a1 0101 0071 147c  .}.|...|.....q.|
-00000c00: 006a 0564 0416 0073 6064 057c 005f 0574  .j.d...s`d.|._.t
-00000c10: 006a 016a 027c 006a 0364 0164 068d 026a  .j.j.|.j.d.d...j
-00000c20: 0664 0264 078d 0144 005d 0e7d 017c 00a0  .d.d...D.].}.|..
-00000c30: 047c 01a1 0101 0071 4e6e 0e7c 0004 006a  .|.....qNn.|...j
-00000c40: 0564 0837 0002 005f 0564 0053 0029 094e  .d.7..._.d.S.).N
-00000c50: 7248 0000 0072 4c00 0000 2903 724a 0000  rH...rL...).rJ..
-00000c60: 0072 4b00 0000 722a 0000 0072 3300 0000  .rK...r*...r3...
-00000c70: 7201 0000 0072 4900 0000 724d 0000 0072  r....rI...rM...r
-00000c80: 0c00 0000 2907 7209 0000 0072 1b00 0000  ....).r....r....
-00000c90: 724f 0000 0072 5000 0000 721e 0000 00da  rO...rP...r.....
-00000ca0: 0c77 6174 6368 5f73 6563 6f6e 6472 5100  .watch_secondrQ.
-00000cb0: 0000 7252 0000 0072 2e00 0000 722e 0000  ..rR...r....r...
-00000cc0: 0072 2f00 0000 7212 0000 008a 0000 0073  .r/...r........s
-00000cd0: 2000 0000 0001 0601 0400 0201 02fe 0a04   ...............
-00000ce0: 0c03 0a01 0601 0601 0400 02ff 0602 02fe  ................
-00000cf0: 0a03 0e02 7a21 534f 4e4f 5347 6174 6577  ....z!SONOSGatew
-00000d00: 6179 4861 6e64 6c65 722e 7761 7463 685f  ayHandler.watch_
-00000d10: 706c 6179 6572 7363 0100 0000 0000 0000  playersc........
-00000d20: 0000 0000 0c00 0000 0800 0000 4300 0000  ............C...
-00000d30: 7342 0200 0074 0064 0183 0101 0067 007d  sB...t.d.....g.}
-00000d40: 0174 0174 0264 0264 038d 0183 017d 027c  .t.t.d.d.....}.|
-00000d50: 0244 005d 6c7d 037c 036a 036a 046a 057c  .D.]l}.|.j.j.j.|
-00000d60: 036a 056b 0372 3471 1e74 066a 076a 087c  .j.k.r4q.t.j.j.|
-00000d70: 036a 057c 036a 097c 036a 0a74 0ba0 0ca1  .j.|.j.|.j.t....
-00000d80: 0064 0264 049c 0464 058d 025c 027d 047d  .d.d...d...\.}.}
-00000d90: 057c 01a0 0d7c 04a1 0101 007c 0572 7c74  .|...|.....|.r|t
-00000da0: 0064 067c 049b 0064 079d 0383 0101 0071  .d.|...d.......q
-00000db0: 1e74 007c 049b 0064 089d 0283 0101 0071  .t.|...d.......q
-00000dc0: 1e74 066a 076a 0e64 0964 0a84 007c 0144  .t.j.j.d.d...|.D
-00000dd0: 0083 0164 0b8d 017d 067c 0690 0172 5a74  ...d...}.|...rZt
-00000de0: 0064 0c83 0101 007c 0644 005d a27d 077a  .d.....|.D.].}.z
-00000df0: 1674 0f7c 076a 1083 017d 037c 03a0 11a1  .t.|.j...}.|....
-00000e00: 0001 0057 006e 2e01 0001 0001 0074 007c  ...W.n.......t.|
-00000e10: 079b 0064 0d7c 076a 109b 009d 0383 0101  ...d.|.j........
-00000e20: 0064 0e7c 075f 127c 07a0 13a1 0001 0059  .d.|._.|.......Y
-00000e30: 0071 b658 007c 02a0 0d7c 03a1 0101 0074  .q.X.|...|.....t
-00000e40: 066a 076a 087c 036a 057c 036a 097c 036a  .j.j.|.j.|.j.|.j
-00000e50: 0a74 0ba0 0ca1 0064 0264 049c 0464 058d  .t.....d.d...d..
-00000e60: 025c 027d 047d 057c 0590 0172 4a74 0064  .\.}.}.|...rJt.d
-00000e70: 067c 049b 0064 079d 0383 0101 0071 b674  .|...d.......q.t
-00000e80: 007c 049b 0064 089d 0283 0101 0071 b674  .|...d.......q.t
-00000e90: 0064 0f83 0101 007c 0244 005d d67d 0374  .d.....|.D.].}.t
-00000ea0: 066a 076a 147c 036a 0564 108d 017d 047c  .j.j.|.j.d...}.|
-00000eb0: 036a 036a 046a 057c 036a 056b 0290 0172  .j.j.j.|.j.k...r
-00000ec0: 9464 007c 045f 156e 1a74 066a 076a 167c  .d.|._.n.t.j.j.|
-00000ed0: 036a 036a 046a 0564 108d 01a0 17a1 007c  .j.j.j.d.......|
-00000ee0: 045f 157c 04a0 13a1 0001 0067 007d 087c  ._.|.......g.}.|
-00000ef0: 03a0 18a1 0044 005d 3a7d 0974 196a 076a  .....D.]:}.t.j.j
-00000f00: 087c 096a 1a74 066a 076a 147c 036a 0564  .|.j.t.j.j.|.j.d
-00000f10: 108d 0164 117c 096a 1b69 0164 128d 035c  ...d.|.j.i.d...\
-00000f20: 027d 0a7d 057c 08a0 0d7c 0aa1 0101 0090  .}.}.|...|......
-00000f30: 0171 c27c 0890 0172 6674 1c6a 076a 167c  .q.|...rft.j.j.|
-00000f40: 006a 1d64 1364 148d 0244 005d 227d 0b64  .j.d.d...D.]"}.d
-00000f50: 1564 0a84 007c 0844 0083 017c 0b6a 1e64  .d...|.D...|.j.d
-00000f60: 163c 007c 0ba0 13a1 0001 0090 0271 1690  .<.|.........q..
-00000f70: 0171 6664 0053 0029 174e 7a17 4469 7363  .qfd.S.).Nz.Disc
-00000f80: 6f76 6572 2053 4f4e 4f53 2070 6c61 7965  over SONOS playe
-00000f90: 7273 2e54 2901 5a12 616c 6c6f 775f 6e65  rs.T).Z.allow_ne
-00000fa0: 7477 6f72 6b5f 7363 616e 2904 da04 6e61  twork_scan)...na
-00000fb0: 6d65 da02 6970 da09 6c61 7374 5f73 6565  me..ip..last_see
-00000fc0: 6eda 0869 735f 616c 6976 6529 02da 0375  n..is_alive)...u
-00000fd0: 6964 da08 6465 6661 756c 7473 7a0d 4e65  id..defaultsz.Ne
-00000fe0: 7720 706c 6179 6572 202d 207a 0d20 2d20  w player - z. - 
-00000ff0: 7761 7320 666f 756e 6421 7a10 202d 2072  was found!z. - r
-00001000: 6564 6973 636f 7665 7265 642e 6301 0000  ediscovered.c...
-00001010: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00001020: 0053 0000 0073 1200 0000 6700 7c00 5d0a  .S...s....g.|.].
-00001030: 7d01 7c01 6a00 9102 7104 5300 722e 0000  }.|.j...q.S.r...
-00001040: 0072 1400 0000 2902 da02 2e30 da01 7072  .r....)....0..pr
-00001050: 2e00 0000 722e 0000 0072 2f00 0000 da0a  ....r....r/.....
-00001060: 3c6c 6973 7463 6f6d 703e b100 0000 7304  <listcomp>....s.
-00001070: 0000 0006 0002 007a 3e53 4f4e 4f53 4761  .......z>SONOSGa
-00001080: 7465 7761 7948 616e 646c 6572 2e64 6973  tewayHandler.dis
-00001090: 636f 7665 725f 736f 6e6f 735f 706c 6179  cover_sonos_play
-000010a0: 6572 732e 3c6c 6f63 616c 733e 2e3c 6c69  ers.<locals>.<li
-000010b0: 7374 636f 6d70 3e29 01da 0669 645f 5f69  stcomp>)...id__i
-000010c0: 6e7a 264c 6574 2773 206d 616e 7561 6c6c  nz&Let's manuall
-000010d0: 7920 6368 6563 6b20 7468 6520 6d69 7373  y check the miss
-000010e0: 696e 6720 6f6e 6573 217a 1a20 2d20 7374  ing ones!z. - st
-000010f0: 696c 6c20 6e6f 7420 6176 6169 6c61 626c  ill not availabl
-00001100: 6520 6174 2046 7a40 4669 6775 7265 206f  e at Fz@Figure o
-00001110: 7574 2077 686f 2773 2064 6120 626f 7373  ut who's da boss
-00001120: 2061 6e64 2053 4f4e 4f53 2070 6c61 796c   and SONOS playl
-00001130: 6973 7473 2074 6861 7420 6172 6520 6176  ists that are av
-00001140: 6169 6c61 626c 652e 2901 7259 0000 00da  ailable.).rY....
-00001150: 0574 6974 6c65 2903 da07 6974 656d 5f69  .title)...item_i
-00001160: 64da 0670 6c61 7965 7272 5a00 0000 7248  d..playerrZ...rH
-00001170: 0000 0072 4900 0000 6301 0000 0000 0000  ...rI...c.......
-00001180: 0000 0000 0002 0000 0006 0000 0053 0000  .............S..
-00001190: 0073 1c00 0000 6700 7c00 5d14 7d01 6400  .s....g.|.].}.d.
-000011a0: 7c01 6a00 7c01 6a01 6401 9c03 9102 7104  |.j.|.j.d.....q.
-000011b0: 5300 2902 5a0e 736f 6e6f 735f 706c 6179  S.).Z.sonos_play
-000011c0: 6c69 7374 2903 da04 7479 7065 7215 0000  list)...typer...
-000011d0: 0072 5f00 0000 2902 7215 0000 0072 5f00  .r_...).r....r_.
-000011e0: 0000 2902 725b 0000 00da 0370 6c73 722e  ..).r[.....plsr.
-000011f0: 0000 0072 2e00 0000 722f 0000 0072 5d00  ...r....r/...r].
-00001200: 0000 e700 0000 730a 0000 0006 0302 fe02  ......s.........
-00001210: 0104 0004 ffda 076c 6962 7261 7279 291f  .......library).
-00001220: 723c 0000 00da 046c 6973 7472 0400 0000  r<.....listr....
-00001230: da05 6772 6f75 70da 0b63 6f6f 7264 696e  ..group..coordin
-00001240: 6174 6f72 7259 0000 0072 0d00 0000 721b  atorrY...r....r.
-00001250: 0000 00da 1075 7064 6174 655f 6f72 5f63  .....update_or_c
-00001260: 7265 6174 655a 0b70 6c61 7965 725f 6e61  reateZ.player_na
-00001270: 6d65 da0a 6970 5f61 6464 7265 7373 7203  me..ip_addressr.
-00001280: 0000 00da 036e 6f77 da06 6170 7065 6e64  .....now..append
-00001290: 7251 0000 0072 0500 0000 7256 0000 005a  rQ...r....rV...Z
-000012a0: 1067 6574 5f73 7065 616b 6572 5f69 6e66  .get_speaker_inf
-000012b0: 6f72 5800 0000 da04 7361 7665 721c 0000  orX.....saver...
-000012c0: 005a 0873 6c61 7665 5f6f 6672 4f00 0000  .Z.slave_ofrO...
-000012d0: da05 6669 7273 745a 1367 6574 5f73 6f6e  ..firstZ.get_son
-000012e0: 6f73 5f70 6c61 796c 6973 7473 720e 0000  os_playlistsr...
-000012f0: 0072 6000 0000 725f 0000 0072 0900 0000  .r`...r_...r....
-00001300: 7250 0000 00da 046d 6574 6129 0c72 2800  rP.....meta).r(.
-00001310: 0000 5a12 6469 7363 6f76 6572 6564 5f70  ..Z.discovered_p
-00001320: 6c61 7965 7273 5a0d 736f 6e6f 735f 6465  layersZ.sonos_de
-00001330: 7669 6365 735a 0573 6f6e 6f73 7261 0000  vicesZ.sonosra..
-00001340: 00da 036e 6577 5a0f 6d69 7373 696e 675f  ...newZ.missing_
-00001350: 706c 6179 6572 735a 0e6d 6973 7369 6e67  playersZ.missing
-00001360: 5f70 6c61 7965 725a 0970 6c61 796c 6973  _playerZ.playlis
-00001370: 7473 7263 0000 005a 0870 6c61 796c 6973  tsrc...Z.playlis
-00001380: 7472 5300 0000 722e 0000 0072 2e00 0000  trS...r....r....
-00001390: 722f 0000 0072 4e00 0000 9b00 0000 7392  r/...rN.......s.
-000013a0: 0000 0000 0108 0204 010e 0108 0110 0202  ................
-000013b0: 0106 0104 0104 0004 0106 0002 fe04 ff0a  ................
-000013c0: 060a 0104 0112 0210 0206 010c ff06 0306  ................
-000013d0: 0108 0108 0102 010a 010c 0106 0102 010e  ................
-000013e0: ff04 0206 010e 020a 0106 0104 0104 0004  ................
-000013f0: 0106 0002 fe04 ff0a 0606 0112 0210 0202  ................
-00001400: 0102 ff04 0408 0110 0112 0108 0206 0108  ................
-00001410: ff0c 0308 0204 020c 0106 0104 010e 0108  ................
-00001420: fd0a 050e 0206 0106 0104 0002 ff0a 0306  ................
-00001430: 0302 fd0c 057a 2a53 4f4e 4f53 4761 7465  .....z*SONOSGate
-00001440: 7761 7948 616e 646c 6572 2e64 6973 636f  wayHandler.disco
-00001450: 7665 725f 736f 6e6f 735f 706c 6179 6572  ver_sonos_player
-00001460: 7363 0200 0000 0000 0000 0000 0000 0600  sc..............
-00001470: 0000 0900 0000 4300 0000 73e8 0000 0074  ......C...s....t
-00001480: 0064 017c 019b 0064 029d 0383 0101 0074  .d.|...d.......t
-00001490: 016a 026a 037c 016a 0464 0319 0064 048d  .j.j.|.j.d...d..
-000014a0: 017d 027a 0e7c 026a 05a0 06a1 007d 0357  .}.z.|.j.....}.W
-000014b0: 006e 2201 0001 0001 0064 057c 015f 0764  .n"......d.|._.d
-000014c0: 067c 015f 087c 01a0 09a1 0001 0059 0064  .|._.|.......Y.d
-000014d0: 0053 0058 0064 0764 0864 0564 099c 037d  .S.X.d.d.d.d...}
-000014e0: 047c 04a0 037c 03a0 0364 0a64 0ba1 0264  .|...|...d.d...d
-000014f0: 0ba1 027c 015f 077a 0c7c 02a0 0aa1 007d  ...|._.z.|.....}
-00001500: 0557 006e 1c01 0001 0001 0064 067c 015f  .W.n.......d.|._
-00001510: 087c 01a0 09a1 0001 0059 0064 0053 0058  .|.......Y.d.S.X
-00001520: 007c 016a 0ba0 0c7c 0564 0c19 0074 0d7c  .|.j...|.d...t.|
-00001530: 0564 0d19 0083 0174 0d7c 0564 0e19 0083  .d.....t.|.d....
-00001540: 017c 026a 056a 0e7c 026a 056a 0f7c 026a  .|.j.j.|.j.j.|.j
-00001550: 056a 1064 0f9c 06a1 0101 007c 01a0 09a1  .j.d.......|....
-00001560: 0001 0064 0053 0029 104e 7a06 4368 6563  ...d.S.).Nz.Chec
-00001570: 6b20 7a07 2073 7461 7465 2172 1300 0000  k z. state!r....
-00001580: 7214 0000 00da 0773 746f 7070 6564 4672  r......stoppedFr
-00001590: 4c00 0000 da06 7061 7573 6564 2903 7235  L.....paused).r5
-000015a0: 0000 005a 0f50 4155 5345 445f 504c 4159  ...Z.PAUSED_PLAY
-000015b0: 4241 434b 7237 0000 0072 3400 0000 7237  BACKr7...r4...r7
-000015c0: 0000 0072 5f00 0000 da08 6475 7261 7469  ...r_.....durati
-000015d0: 6f6e da08 706f 7369 7469 6f6e 2906 725f  on..position).r_
-000015e0: 0000 0072 7200 0000 7273 0000 0072 1800  ...rr...rs...r..
-000015f0: 0000 da07 7368 7566 666c 65da 046c 6f6f  ....shuffle..loo
-00001600: 7029 1172 3c00 0000 720d 0000 0072 1b00  p).r<...r....r..
-00001610: 0000 721c 0000 0072 1d00 0000 7239 0000  ..r....r....r9..
-00001620: 0072 4100 0000 722a 0000 00da 0561 6c69  .rA...r*.....ali
-00001630: 7665 726c 0000 0072 4200 0000 726e 0000  verl...rB...rn..
-00001640: 0072 3b00 0000 720f 0000 0072 1800 0000  .r;...r....r....
-00001650: 7274 0000 0072 3e00 0000 2906 7228 0000  rt...r>...).r(..
-00001660: 005a 0f73 6f6e 6f73 5f63 6f6d 706f 6e65  .Z.sonos_compone
-00001670: 6e74 722b 0000 0072 4700 0000 5a09 7374  ntr+...rG...Z.st
-00001680: 6174 655f 6d61 70da 0469 6e66 6f72 2e00  ate_map..infor..
-00001690: 0000 722e 0000 0072 2f00 0000 721e 0000  ..r....r/...r...
-000016a0: 00ee 0000 0073 4400 0000 0001 1001 0601  .....sD.........
-000016b0: 08ff 0603 0201 0e01 0601 0601 0601 0801  ................
-000016c0: 0803 0201 0201 02fd 0605 0401 0a01 02fe  ................
-000016d0: 0605 0201 0c01 0601 0601 0801 0802 0601  ................
-000016e0: 0601 0a01 0a01 0601 0601 06fa 0809 7a25  ..............z%
-000016f0: 534f 4e4f 5347 6174 6577 6179 4861 6e64  SONOSGatewayHand
-00001700: 6c65 722e 636f 6d70 5f73 7461 7465 5f75  ler.comp_state_u
-00001710: 7064 6174 654e 290f da08 5f5f 6e61 6d65  pdateN)...__name
-00001720: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00001730: 5f5f 7175 616c 6e61 6d65 5f5f 7255 0000  __qualname__rU..
-00001740: 0072 0800 0000 da0b 636f 6e66 6967 5f66  .r......config_f
-00001750: 6f72 6dda 0e70 6572 696f 6469 635f 7461  orm..periodic_ta
-00001760: 736b 7372 3800 0000 7254 0000 0072 3000  sksr8...rT...r0.
-00001770: 0000 7226 0000 0072 1100 0000 7212 0000  ..r&...r....r...
-00001780: 0072 4e00 0000 721e 0000 0072 2e00 0000  .rN...r....r....
-00001790: 722e 0000 0072 2e00 0000 722f 0000 0072  r....r....r/...r
-000017a0: 1000 0000 1000 0000 7316 0000 0008 0104  ........s.......
-000017b0: 0104 0204 0504 0104 0208 1708 4e08 0908  ............N...
-000017c0: 1108 5372 1000 0000 291b 723a 0000 0072  ..Sr....).r:...r
-000017d0: 2400 0000 da08 6461 7465 7469 6d65 7202  $.....datetimer.
-000017e0: 0000 00da 0c64 6a61 6e67 6f2e 7574 696c  .....django.util
-000017f0: 7372 0300 0000 7239 0000 0072 0400 0000  sr....r9...r....
-00001800: 7205 0000 005a 0d73 6f63 6f2e 736e 6170  r....Z.soco.snap
-00001810: 7368 6f74 7206 0000 005a 1273 696d 6f2e  shotr....Z.simo.
-00001820: 636f 7265 2e67 6174 6577 6179 7372 0700  core.gatewaysr..
-00001830: 0000 5a0f 7369 6d6f 2e63 6f72 652e 666f  ..Z.simo.core.fo
-00001840: 726d 7372 0800 0000 da10 7369 6d6f 2e63  rmsr......simo.c
-00001850: 6f72 652e 6d6f 6465 6c73 7209 0000 00da  ore.modelsr.....
-00001860: 1773 696d 6f2e 636f 7265 2e75 7469 6c73  .simo.core.utils
-00001870: 2e68 656c 7065 7273 720a 0000 005a 1673  .helpersr....Z.s
-00001880: 696d 6f2e 6d75 6c74 696d 6564 6961 2e6d  imo.multimedia.m
-00001890: 6f64 656c 7372 0b00 0000 da06 6d6f 6465  odelsr......mode
-000018a0: 6c73 720d 0000 0072 0e00 0000 da05 7574  lsr....r......ut
-000018b0: 696c 7372 0f00 0000 7210 0000 0072 2e00  ilsr....r....r..
-000018c0: 0000 722e 0000 0072 2e00 0000 722f 0000  ..r....r....r/..
-000018d0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-000018e0: 1a00 0000 0801 0801 0c01 0c01 1001 0c01  ................
-000018f0: 0c01 0c01 0c01 0c01 0c01 1001 0c03       ..............
+000002a0: 028d 017d 037c 0264 036b 0672 2e74 047c  ...}.|.d.k.r.t.|
+000002b0: 036a 057c 0283 0283 0001 0090 016e 7c74  .j.|.........n|t
+000002c0: 067c 0274 0783 0290 0172 aa64 047c 026b  .|.t.....r.d.|.k
+000002d0: 0672 5c7c 036a 05a0 0874 097c 0264 0419  .r\|.j...t.|.d..
+000002e0: 0064 058d 01a1 0101 0090 016e 4e64 067c  .d.........nNd.|
+000002f0: 026b 0672 747c 0264 0619 007c 036a 055f  .k.rt|.d...|.j._
+00000300: 0a90 016e 3664 077c 026b 0672 8c7c 0264  ...n6d.|.k.r.|.d
+00000310: 0719 007c 036a 055f 0b90 016e 1e64 087c  ...|.j._...n.d.|
+00000320: 026b 0672 a47c 0264 0819 007c 036a 055f  .k.r.|.d...|.j._
+00000330: 0c90 016e 0664 097c 026b 0672 f47c 0264  ...n.d.|.k.r.|.d
+00000340: 0919 00a0 0264 0aa1 0164 0b6b 0372 c264  .....d...d.k.r.d
+00000350: 0053 0074 0d6a 016a 0e7c 0264 0919 00a0  .S.t.j.j.|.d....
+00000360: 0264 0c64 0da1 0264 028d 01a0 0fa1 007d  .d.d...d.......}
+00000370: 047c 0473 e864 0053 007c 01a0 107c 04a1  .|.s.d.S.|...|..
+00000380: 0101 006e b664 0e7c 026b 0690 0172 2c7c  ...n.d.|.k...r,|
+00000390: 02a0 0264 0fa1 0164 006b 0390 0172 1a7c  ...d...d.k...r.|
+000003a0: 0264 0f19 007c 036a 055f 0a7c 036a 05a0  .d...|.j._.|.j..
+000003b0: 117c 0264 0e19 00a1 0101 006e 7e64 107c  .|.d.......n~d.|
+000003c0: 026b 0690 0172 aa7a 1074 127c 0264 1019  .k...r.z.t.|.d..
+000003d0: 0083 017d 0557 006e 1801 0001 0001 007c  ...}.W.n.......|
+000003e0: 0264 1019 007d 0664 007d 0759 006e 2a58  .d...}.d.}.Y.n*X
+000003f0: 0074 136a 016a 027c 0564 118d 017d 087c  .t.j.j.|.d...}.|
+00000400: 086a 147d 0764 1274 1583 009b 007c 08a0  .j.}.d.t.....|..
+00000410: 16a1 009b 009d 037d 0674 176a 187c 006a  .......}.t.j.|.j
+00000420: 197c 037c 067c 077c 02a0 0264 0fa1 0166  .|.|.|.|...d...f
+00000430: 0464 138d 02a0 1aa1 0001 007c 00a0 1b7c  .d.........|...|
+00000440: 01a1 0101 0064 0053 0029 144e da0c 736f  .....d.S.).N..so
+00000450: 6e6f 735f 6465 7669 6365 a901 da02 6964  nos_device....id
+00000460: 2905 da04 706c 6179 da05 7061 7573 65da  )...play..pause.
+00000470: 0473 746f 70da 046e 6578 74da 0870 7265  .stop..next..pre
+00000480: 7669 6f75 73da 0473 6565 6b29 01da 0773  vious..seek)...s
+00000490: 6563 6f6e 6473 5a0a 7365 745f 766f 6c75  econdsZ.set_volu
+000004a0: 6d65 da07 7368 7566 666c 65da 046c 6f6f  me..shuffle..loo
+000004b0: 705a 1170 6c61 795f 6672 6f6d 5f6c 6962  pZ.play_from_lib
+000004c0: 7261 7279 da04 7479 7065 da0e 736f 6e6f  rary..type..sono
+000004d0: 735f 706c 6179 6c69 7374 7215 0000 0072  s_playlistr....r
+000004e0: 0100 0000 da08 706c 6179 5f75 7269 da06  ......play_uri..
+000004f0: 766f 6c75 6d65 da05 616c 6572 7429 01da  volume..alert)..
+00000500: 0270 6b7a 0768 7474 703a 2f2f 2902 da06  .pkz.http://)...
+00000510: 7461 7267 6574 da04 6172 6773 291c 720d  target..args).r.
+00000520: 0000 00da 076f 626a 6563 7473 da03 6765  .....objects..ge
+00000530: 74da 0663 6f6e 6669 67da 0767 6574 6174  t..config..getat
+00000540: 7472 da04 736f 636f da0a 6973 696e 7374  tr..soco..isinst
+00000550: 616e 6365 da04 6469 6374 721b 0000 0072  ance..dictr....r
+00000560: 0200 0000 7222 0000 0072 1d00 0000 da06  ....r"...r......
+00000570: 7265 7065 6174 720e 0000 00da 0666 696c  repeatr......fil
+00000580: 7465 72da 0566 6972 7374 5a0d 706c 6179  ter..firstZ.play
+00000590: 5f70 6c61 796c 6973 7472 2100 0000 da03  _playlistr!.....
+000005a0: 696e 7472 0b00 0000 da06 6c65 6e67 7468  intr......length
+000005b0: 720a 0000 00da 1067 6574 5f61 6273 6f6c  r......get_absol
+000005c0: 7574 655f 7572 6cda 0974 6872 6561 6469  ute_url..threadi
+000005d0: 6e67 da06 5468 7265 6164 da0a 706c 6179  ng..Thread..play
+000005e0: 5f61 6c65 7274 da05 7374 6172 74da 1163  _alert..start..c
+000005f0: 6f6d 705f 7374 6174 655f 7570 6461 7465  omp_state_update
+00000600: 2909 da04 7365 6c66 da09 636f 6d70 6f6e  )...self..compon
+00000610: 656e 74da 0576 616c 7565 da0c 736f 6e6f  ent..value..sono
+00000620: 735f 706c 6179 6572 da08 706c 6179 6c69  s_player..playli
+00000630: 7374 5a08 736f 756e 645f 6964 da03 7572  stZ.sound_id..ur
+00000640: 6972 3200 0000 da05 736f 756e 64a9 0072  ir2.....sound..r
+00000650: 4000 0000 fa4a 2f68 6f6d 652f 7369 6d61  @....J/home/sima
+00000660: 6e61 732f 5072 6f6a 6563 7473 2f53 494d  nas/Projects/SIM
+00000670: 4f2f 7061 636b 6167 6573 2f73 696d 6f2d  O/packages/simo-
+00000680: 736f 6e6f 732f 7372 632f 7369 6d6f 5f73  sonos/src/simo_s
+00000690: 6f6e 6f73 2f67 6174 6577 6179 732e 7079  onos/gateways.py
+000006a0: da12 7065 7266 6f72 6d5f 7661 6c75 655f  ..perform_value_
+000006b0: 7365 6e64 1c00 0000 7356 0000 0000 0114  send....sV......
+000006c0: 0208 0312 020c 0108 011a 0108 0110 0108  ................
+000006d0: 0110 0108 0110 0108 0112 0104 0106 010e  ................
+000006e0: ff0a 0304 0104 010c 010a 0110 010c 0112  ................
+000006f0: 020a 0102 0110 0106 0108 010a 020e 0106  ................
+00000700: 0114 0104 0104 0102 0002 0002 0008 ff02  ................
+00000710: ff0a 067a 2653 4f4e 4f53 4761 7465 7761  ...z&SONOSGatewa
+00000720: 7948 616e 646c 6572 2e70 6572 666f 726d  yHandler.perform
+00000730: 5f76 616c 7565 5f73 656e 6463 0500 0000  _value_sendc....
+00000740: 0000 0000 0000 0000 0a00 0000 0a00 0000  ................
+00000750: 4300 0000 7342 0200 007c 016a 007c 006a  C...sB...|.j.|.j
+00000760: 016b 0772 4074 027c 016a 0383 017c 0274  .k.r@t.|.j...|.t
+00000770: 04a0 04a1 0064 019c 037c 006a 017c 016a  .....d...|.j.|.j
+00000780: 003c 007c 006a 017c 016a 0019 0064 0219  .<.|.j.|.j...d..
+00000790: 00a0 05a1 0001 006e 1c7c 006a 017c 016a  .......n.|.j.|.j
+000007a0: 0019 00a0 067c 0274 04a0 04a1 0064 039c  .....|.t.....d..
+000007b0: 02a1 0101 007c 006a 017c 016a 0019 0064  .....|.j.|.j...d
+000007c0: 0419 007d 057c 0464 006b 0372 7c7c 047c  ...}.|.d.k.r||.|
+000007d0: 016a 035f 0774 0864 057c 0283 0201 007c  .j._.t.d.|.....|
+000007e0: 016a 03a0 09a1 0001 0064 067c 016a 035f  .j.......d.|.j._
+000007f0: 0a7c 016a 03a0 0ba1 0001 007c 016a 03a0  .|.j.......|.j..
+00000800: 0c7c 02a1 0101 007c 0364 006b 0372 ce7c  .|.....|.d.k.r.|
+00000810: 0364 076b 0472 c264 077d 0374 04a0 0d7c  .d.k.r.d.}.t...|
+00000820: 03a1 0101 006e 3874 0e64 0783 0144 005d  .....n8t.d...D.]
+00000830: 2e7d 0674 04a0 0d64 08a1 0101 007c 016a  .}.t...d.....|.j
+00000840: 03a0 0fa1 007d 077c 07a0 1064 0964 0aa1  .....}.|...d.d..
+00000850: 0264 0a6b 0372 d601 0090 0171 0671 d67c  .d.k.r.....q.q.|
+00000860: 006a 01a0 107c 016a 0069 00a1 02a0 1064  .j...|.j.i.....d
+00000870: 0464 0ba1 027c 056b 0390 0172 2864 0053  .d...|.k...r(d.S
+00000880: 007c 006a 01a0 107c 016a 0069 00a1 02a0  .|.j...|.j.i....
+00000890: 1064 0c64 0da1 027c 026b 0390 0172 4a64  .d.d...|.k...rJd
+000008a0: 0053 007c 016a 03a0 11a1 007d 087c 08a0  .S.|.j.....}.|..
+000008b0: 1064 0ca1 0190 0172 8c7c 08a0 1064 0ca1  .d.....r.|...d..
+000008c0: 017c 026b 0390 0172 8c7c 016a 007c 006a  .|.k...r.|.j.|.j
+000008d0: 016b 0690 0172 887c 006a 017c 016a 003d  .k...r.|.j.|.j.=
+000008e0: 0064 0053 0074 0864 0e83 0101 007c 006a  .d.S.t.d.....|.j
+000008f0: 017c 016a 0019 0064 0219 007d 097a 147c  .|.j...d...}.z.|
+00000900: 096a 1890 0172 b67c 09a0 19a1 0001 0057  .j...r.|.......W
+00000910: 0035 007c 096a 127c 096a 135f 127c 096a  .5.|.j.|.j._.|.j
+00000920: 147c 096a 135f 147c 096a 157c 096a 135f  .|.j._.|.j.|.j._
+00000930: 157c 096a 167c 096a 135f 1664 0b7c 096a  .|.j.|.j._.d.|.j
+00000940: 135f 077c 096a 136a 177c 096a 0764 0f64  ._.|.j.j.|.j.d.d
+00000950: 108d 0201 0058 007c 096a 1890 0272 347c  .....X.|.j...r4|
+00000960: 096a 1a64 0a6b 0290 0272 1e7c 096a 13a0  .j.d.k...r.|.j..
+00000970: 1ba1 0001 006e 167c 096a 1a64 116b 0290  .....n.|.j.d.k..
+00000980: 0272 347c 096a 13a0 09a1 0001 007c 006a  .r4|.j.......|.j
+00000990: 017c 016a 003d 0064 0053 0029 124e 2903  .|.j.=.d.S.).N).
+000009a0: da04 736e 6170 723e 0000 00da 0974 696d  ..snapr>.....tim
+000009b0: 6573 7461 6d70 7243 0000 0029 0272 3e00  estamprC...).r>.
+000009c0: 0000 7244 0000 0072 4400 0000 7a15 506c  ..rD...rD...z.Pl
+000009d0: 6179 2061 6c65 7274 2066 726f 6d20 5552  ay alert from UR
+000009e0: 493a 2046 e93c 0000 0072 0c00 0000 da17  I: F.<...r......
+000009f0: 6375 7272 656e 745f 7472 616e 7370 6f72  current_transpor
+00000a00: 745f 7374 6174 65da 0750 4c41 5949 4e47  t_state..PLAYING
+00000a10: 7201 0000 0072 3e00 0000 da00 7a10 5265  r....r>.....z.Re
+00000a20: 7374 6f72 6520 6f72 6967 696e 616c 5a12  store originalZ.
+00000a30: 4155 544f 504c 4159 5f52 414d 505f 5459  AUTOPLAY_RAMP_TY
+00000a40: 5045 2901 5a09 7261 6d70 5f74 7970 65da  PE).Z.ramp_type.
+00000a50: 0753 544f 5050 4544 291c 7215 0000 00da  .STOPPED).r.....
+00000a60: 0e70 6c61 7969 6e67 5f61 6c65 7274 7372  .playing_alertsr
+00000a70: 0600 0000 722b 0000 00da 0474 696d 655a  ....r+.....timeZ
+00000a80: 0873 6e61 7073 686f 74da 0675 7064 6174  .snapshot..updat
+00000a90: 6572 2200 0000 da05 7072 696e 7472 1800  er".....printr..
+00000aa0: 0000 722e 0000 005a 0b63 6c65 6172 5f71  ..r....Z.clear_q
+00000ab0: 7565 7565 7221 0000 00da 0573 6c65 6570  ueuer!.....sleep
+00000ac0: da05 7261 6e67 65da 1a67 6574 5f63 7572  ..range..get_cur
+00000ad0: 7265 6e74 5f74 7261 6e73 706f 7274 5f69  rent_transport_i
+00000ae0: 6e66 6f72 2800 0000 da16 6765 745f 6375  nfor(.....get_cu
+00000af0: 7272 656e 745f 7472 6163 6b5f 696e 666f  rrent_track_info
+00000b00: da04 6d75 7465 da06 6465 7669 6365 5a04  ..mute..deviceZ.
+00000b10: 6261 7373 5a06 7472 6562 6c65 5a08 6c6f  bassZ.trebleZ.lo
+00000b20: 7564 6e65 7373 5a0e 7261 6d70 5f74 6f5f  udnessZ.ramp_to_
+00000b30: 766f 6c75 6d65 5a0e 6973 5f63 6f6f 7264  volumeZ.is_coord
+00000b40: 696e 6174 6f72 5a14 5f72 6573 746f 7265  inatorZ._restore
+00000b50: 5f63 6f6f 7264 696e 6174 6f72 5a0f 7472  _coordinatorZ.tr
+00000b60: 616e 7370 6f72 745f 7374 6174 6572 1600  ansport_stater..
+00000b70: 0000 290a 7239 0000 0072 3c00 0000 723e  ..).r9...r<...r>
+00000b80: 0000 0072 3200 0000 7222 0000 005a 0f73  ...r2...r"...Z.s
+00000b90: 7461 7274 5f74 696d 6573 7461 6d70 da01  tart_timestamp..
+00000ba0: 69da 0673 7461 7475 735a 1263 7572 7265  i..statusZ.curre
+00000bb0: 6e74 5f74 7261 636b 5f69 6e66 6f72 4300  nt_track_inforC.
+00000bc0: 0000 7240 0000 0072 4000 0000 7241 0000  ..r@...r@...rA..
+00000bd0: 0072 3600 0000 4d00 0000 7382 0000 0000  .r6...M...s.....
+00000be0: 010c 0208 0102 0006 fe0e 0416 020c 0102  ................
+00000bf0: 0006 ff08 0410 0208 0108 020a 010a 0108  ................
+00000c00: 010a 010c 0208 0108 0104 010c 020c 010a  ................
+00000c10: 010a 0104 0102 0002 ff02 0202 fe04 0308  ................
+00000c20: 0316 0102 ff06 0304 011e 0204 020a 010c  ................
+00000c30: 010c ff04 030e 010a 0104 0208 0110 0102  ................
+00000c40: 0108 010c 020a 010a 010a 010a 0108 0106  ................
+00000c50: 0104 0002 ff08 0608 010c 010c 010c 010a  ................
+00000c60: 027a 1e53 4f4e 4f53 4761 7465 7761 7948  .z.SONOSGatewayH
+00000c70: 616e 646c 6572 2e70 6c61 795f 616c 6572  andler.play_aler
+00000c80: 7463 0100 0000 0000 0000 0000 0000 0200  tc..............
+00000c90: 0000 0400 0000 4300 0000 7336 0000 007c  ......C...s6...|
+00000ca0: 00a0 00a1 0001 0074 016a 026a 037c 006a  .......t.j.j.|.j
+00000cb0: 0464 0164 028d 026a 0564 0364 048d 0144  .d.d...j.d.d...D
+00000cc0: 005d 0e7d 017c 00a0 067c 01a1 0101 0071  .].}.|...|.....q
+00000cd0: 2264 0053 0029 054e fa0c 6175 6469 6f2d  "d.S.).N..audio-
+00000ce0: 706c 6179 6572 a902 da07 6761 7465 7761  player....gatewa
+00000cf0: 79da 0962 6173 655f 7479 7065 da07 706c  y..base_type..pl
+00000d00: 6179 696e 67a9 0172 3b00 0000 2907 da16  aying..r;...)...
+00000d10: 6469 7363 6f76 6572 5f73 6f6e 6f73 5f70  discover_sonos_p
+00000d20: 6c61 7965 7273 7209 0000 0072 2700 0000  layersr....r'...
+00000d30: 722f 0000 00da 1067 6174 6577 6179 5f69  r/.....gateway_i
+00000d40: 6e73 7461 6e63 65da 0765 7863 6c75 6465  nstance..exclude
+00000d50: 7238 0000 00a9 0272 3900 0000 da04 636f  r8.....r9.....co
+00000d60: 6d70 7240 0000 0072 4000 0000 7241 0000  mpr@...r@...rA..
+00000d70: 0072 1100 0000 9b00 0000 7310 0000 0000  .r........s.....
+00000d80: 0308 0106 0104 0002 ff06 0202 fe0a 037a  ...............z
+00000d90: 2e53 4f4e 4f53 4761 7465 7761 7948 616e  .SONOSGatewayHan
+00000da0: 646c 6572 2e70 6572 696f 6469 635f 706c  dler.periodic_pl
+00000db0: 6179 6572 735f 6469 7363 6f76 6572 7963  ayers_discoveryc
+00000dc0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000dd0: 0500 0000 4300 0000 7372 0000 0074 006a  ....C...sr...t.j
+00000de0: 016a 027c 006a 0364 0164 0264 038d 0344  .j.|.j.d.d.d...D
+00000df0: 005d 0e7d 017c 00a0 047c 01a1 0101 0071  .].}.|...|.....q
+00000e00: 147c 006a 0564 0416 0073 6064 057c 005f  .|.j.d...s`d.|._
+00000e10: 0574 006a 016a 027c 006a 0364 0164 068d  .t.j.j.|.j.d.d..
+00000e20: 026a 0664 0264 078d 0144 005d 0e7d 017c  .j.d.d...D.].}.|
+00000e30: 00a0 047c 01a1 0101 0071 4e6e 0e7c 0004  ...|.....qNn.|..
+00000e40: 006a 0564 0837 0002 005f 0564 0053 0029  .j.d.7..._.d.S.)
+00000e50: 094e 7256 0000 0072 5a00 0000 2903 7258  .NrV...rZ...).rX
+00000e60: 0000 0072 5900 0000 723b 0000 0072 4500  ...rY...r;...rE.
+00000e70: 0000 7201 0000 0072 5700 0000 725b 0000  ..r....rW...r[..
+00000e80: 0072 0c00 0000 2907 7209 0000 0072 2700  .r....).r....r'.
+00000e90: 0000 722f 0000 0072 5d00 0000 7238 0000  ..r/...r]...r8..
+00000ea0: 00da 0c77 6174 6368 5f73 6563 6f6e 6472  ...watch_secondr
+00000eb0: 5e00 0000 725f 0000 0072 4000 0000 7240  ^...r_...r@...r@
+00000ec0: 0000 0072 4100 0000 7212 0000 00a4 0000  ...rA...r.......
+00000ed0: 0073 2000 0000 0001 0601 0400 0201 02fe  .s .............
+00000ee0: 0a04 0c03 0a01 0601 0601 0400 02ff 0602  ................
+00000ef0: 02fe 0a03 0e02 7a21 534f 4e4f 5347 6174  ......z!SONOSGat
+00000f00: 6577 6179 4861 6e64 6c65 722e 7761 7463  ewayHandler.watc
+00000f10: 685f 706c 6179 6572 7363 0100 0000 0000  h_playersc......
+00000f20: 0000 0000 0000 0c00 0000 0800 0000 4300  ..............C.
+00000f30: 0000 7342 0200 0074 0064 0183 0101 0067  ..sB...t.d.....g
+00000f40: 007d 0174 0174 0264 0264 038d 0183 017d  .}.t.t.d.d.....}
+00000f50: 027c 0244 005d 6c7d 037c 036a 036a 046a  .|.D.]l}.|.j.j.j
+00000f60: 057c 036a 056b 0372 3471 1e74 066a 076a  .|.j.k.r4q.t.j.j
+00000f70: 087c 036a 057c 036a 097c 036a 0a74 0ba0  .|.j.|.j.|.j.t..
+00000f80: 0ca1 0064 0264 049c 0464 058d 025c 027d  ...d.d...d...\.}
+00000f90: 047d 057c 01a0 0d7c 04a1 0101 007c 0572  .}.|...|.....|.r
+00000fa0: 7c74 0064 067c 049b 0064 079d 0383 0101  |t.d.|...d......
+00000fb0: 0071 1e74 007c 049b 0064 089d 0283 0101  .q.t.|...d......
+00000fc0: 0071 1e74 066a 076a 0e64 0964 0a84 007c  .q.t.j.j.d.d...|
+00000fd0: 0144 0083 0164 0b8d 017d 067c 0690 0172  .D...d...}.|...r
+00000fe0: 5a74 0064 0c83 0101 007c 0644 005d a27d  Zt.d.....|.D.].}
+00000ff0: 077a 1674 0f7c 076a 1083 017d 037c 03a0  .z.t.|.j...}.|..
+00001000: 11a1 0001 0057 006e 2e01 0001 0001 0074  .....W.n.......t
+00001010: 007c 079b 0064 0d7c 076a 109b 009d 0383  .|...d.|.j......
+00001020: 0101 0064 0e7c 075f 127c 07a0 13a1 0001  ...d.|._.|......
+00001030: 0059 0071 b658 007c 02a0 0d7c 03a1 0101  .Y.q.X.|...|....
+00001040: 0074 066a 076a 087c 036a 057c 036a 097c  .t.j.j.|.j.|.j.|
+00001050: 036a 0a74 0ba0 0ca1 0064 0264 049c 0464  .j.t.....d.d...d
+00001060: 058d 025c 027d 047d 057c 0590 0172 4a74  ...\.}.}.|...rJt
+00001070: 0064 067c 049b 0064 079d 0383 0101 0071  .d.|...d.......q
+00001080: b674 007c 049b 0064 089d 0283 0101 0071  .t.|...d.......q
+00001090: b674 0064 0f83 0101 007c 0244 005d d67d  .t.d.....|.D.].}
+000010a0: 0374 066a 076a 147c 036a 0564 108d 017d  .t.j.j.|.j.d...}
+000010b0: 047c 036a 036a 046a 057c 036a 056b 0290  .|.j.j.j.|.j.k..
+000010c0: 0172 9464 007c 045f 156e 1a74 066a 076a  .r.d.|._.n.t.j.j
+000010d0: 167c 036a 036a 046a 0564 108d 01a0 17a1  .|.j.j.j.d......
+000010e0: 007c 045f 157c 04a0 13a1 0001 0067 007d  .|._.|.......g.}
+000010f0: 087c 03a0 18a1 0044 005d 3a7d 0974 196a  .|.....D.]:}.t.j
+00001100: 076a 087c 096a 1a74 066a 076a 147c 036a  .j.|.j.t.j.j.|.j
+00001110: 0564 108d 0164 117c 096a 1b69 0164 128d  .d...d.|.j.i.d..
+00001120: 035c 027d 0a7d 057c 08a0 0d7c 0aa1 0101  .\.}.}.|...|....
+00001130: 0090 0171 c27c 0890 0172 6674 1c6a 076a  ...q.|...rft.j.j
+00001140: 167c 006a 1d64 1364 148d 0244 005d 227d  .|.j.d.d...D.]"}
+00001150: 0b64 1564 0a84 007c 0844 0083 017c 0b6a  .d.d...|.D...|.j
+00001160: 1e64 163c 007c 0ba0 13a1 0001 0090 0271  .d.<.|.........q
+00001170: 1690 0171 6664 0053 0029 174e 7a17 4469  ...qfd.S.).Nz.Di
+00001180: 7363 6f76 6572 2053 4f4e 4f53 2070 6c61  scover SONOS pla
+00001190: 7965 7273 2e54 2901 5a12 616c 6c6f 775f  yers.T).Z.allow_
+000011a0: 6e65 7477 6f72 6b5f 7363 616e 2904 da04  network_scan)...
+000011b0: 6e61 6d65 da02 6970 da09 6c61 7374 5f73  name..ip..last_s
+000011c0: 6565 6eda 0869 735f 616c 6976 6529 02da  een..is_alive)..
+000011d0: 0375 6964 da08 6465 6661 756c 7473 7a0d  .uid..defaultsz.
+000011e0: 4e65 7720 706c 6179 6572 202d 207a 0d20  New player - z. 
+000011f0: 2d20 7761 7320 666f 756e 6421 7a10 202d  - was found!z. -
+00001200: 2072 6564 6973 636f 7665 7265 642e 6301   rediscovered.c.
+00001210: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00001220: 0000 0053 0000 0073 1200 0000 6700 7c00  ...S...s....g.|.
+00001230: 5d0a 7d01 7c01 6a00 9102 7104 5300 7240  ].}.|.j...q.S.r@
+00001240: 0000 0072 1400 0000 2902 da02 2e30 da01  ...r....)....0..
+00001250: 7072 4000 0000 7240 0000 0072 4100 0000  pr@...r@...rA...
+00001260: da0a 3c6c 6973 7463 6f6d 703e cb00 0000  ..<listcomp>....
+00001270: 7304 0000 0006 0002 007a 3e53 4f4e 4f53  s........z>SONOS
+00001280: 4761 7465 7761 7948 616e 646c 6572 2e64  GatewayHandler.d
+00001290: 6973 636f 7665 725f 736f 6e6f 735f 706c  iscover_sonos_pl
+000012a0: 6179 6572 732e 3c6c 6f63 616c 733e 2e3c  ayers.<locals>.<
+000012b0: 6c69 7374 636f 6d70 3e29 01da 0669 645f  listcomp>)...id_
+000012c0: 5f69 6e7a 264c 6574 2773 206d 616e 7561  _inz&Let's manua
+000012d0: 6c6c 7920 6368 6563 6b20 7468 6520 6d69  lly check the mi
+000012e0: 7373 696e 6720 6f6e 6573 217a 1a20 2d20  ssing ones!z. - 
+000012f0: 7374 696c 6c20 6e6f 7420 6176 6169 6c61  still not availa
+00001300: 626c 6520 6174 2046 7a40 4669 6775 7265  ble at Fz@Figure
+00001310: 206f 7574 2077 686f 2773 2064 6120 626f   out who's da bo
+00001320: 7373 2061 6e64 2053 4f4e 4f53 2070 6c61  ss and SONOS pla
+00001330: 796c 6973 7473 2074 6861 7420 6172 6520  ylists that are 
+00001340: 6176 6169 6c61 626c 652e 2901 7266 0000  available.).rf..
+00001350: 00da 0574 6974 6c65 2903 da07 6974 656d  ...title)...item
+00001360: 5f69 64da 0670 6c61 7965 7272 6700 0000  _id..playerrg...
+00001370: 7256 0000 0072 5700 0000 6301 0000 0000  rV...rW...c.....
+00001380: 0000 0000 0000 0002 0000 0006 0000 0053  ...............S
+00001390: 0000 0073 1c00 0000 6700 7c00 5d14 7d01  ...s....g.|.].}.
+000013a0: 6400 7c01 6a00 7c01 6a01 6401 9c03 9102  d.|.j.|.j.d.....
+000013b0: 7104 5300 2902 7220 0000 0029 0372 1f00  q.S.).r ...).r..
+000013c0: 0000 7215 0000 0072 6c00 0000 2902 7215  ..r....rl...).r.
+000013d0: 0000 0072 6c00 0000 2902 7268 0000 00da  ...rl...).rh....
+000013e0: 0370 6c73 7240 0000 0072 4000 0000 7241  .plsr@...r@...rA
+000013f0: 0000 0072 6a00 0000 0101 0000 730a 0000  ...rj.......s...
+00001400: 0006 0302 fe02 0104 0004 ffda 076c 6962  .............lib
+00001410: 7261 7279 291f 724d 0000 00da 046c 6973  rary).rM.....lis
+00001420: 7472 0400 0000 da05 6772 6f75 70da 0b63  tr......group..c
+00001430: 6f6f 7264 696e 6174 6f72 7266 0000 0072  oordinatorrf...r
+00001440: 0d00 0000 7227 0000 00da 1075 7064 6174  ....r'.....updat
+00001450: 655f 6f72 5f63 7265 6174 655a 0b70 6c61  e_or_createZ.pla
+00001460: 7965 725f 6e61 6d65 da0a 6970 5f61 6464  yer_name..ip_add
+00001470: 7265 7373 7203 0000 00da 036e 6f77 da06  ressr......now..
+00001480: 6170 7065 6e64 725e 0000 0072 0500 0000  appendr^...r....
+00001490: 7263 0000 005a 1067 6574 5f73 7065 616b  rc...Z.get_speak
+000014a0: 6572 5f69 6e66 6f72 6500 0000 da04 7361  er_infore.....sa
+000014b0: 7665 7228 0000 005a 0873 6c61 7665 5f6f  ver(...Z.slave_o
+000014c0: 6672 2f00 0000 7230 0000 005a 1367 6574  fr/...r0...Z.get
+000014d0: 5f73 6f6e 6f73 5f70 6c61 796c 6973 7473  _sonos_playlists
+000014e0: 720e 0000 0072 6d00 0000 726c 0000 0072  r....rm...rl...r
+000014f0: 0900 0000 725d 0000 00da 046d 6574 6129  ....r].....meta)
+00001500: 0c72 3900 0000 5a12 6469 7363 6f76 6572  .r9...Z.discover
+00001510: 6564 5f70 6c61 7965 7273 5a0d 736f 6e6f  ed_playersZ.sono
+00001520: 735f 6465 7669 6365 735a 0573 6f6e 6f73  s_devicesZ.sonos
+00001530: 726e 0000 00da 036e 6577 5a0f 6d69 7373  rn.....newZ.miss
+00001540: 696e 675f 706c 6179 6572 735a 0e6d 6973  ing_playersZ.mis
+00001550: 7369 6e67 5f70 6c61 7965 725a 0970 6c61  sing_playerZ.pla
+00001560: 796c 6973 7473 726f 0000 0072 3d00 0000  ylistsro...r=...
+00001570: 7260 0000 0072 4000 0000 7240 0000 0072  r`...r@...r@...r
+00001580: 4100 0000 725c 0000 00b5 0000 0073 9200  A...r\.......s..
+00001590: 0000 0001 0802 0401 0e01 0801 1002 0201  ................
+000015a0: 0601 0401 0400 0401 0600 02fe 04ff 0a06  ................
+000015b0: 0a01 0401 1202 1002 0601 0cff 0603 0601  ................
+000015c0: 0801 0801 0201 0a01 0c01 0601 0201 0eff  ................
+000015d0: 0402 0601 0e02 0a01 0601 0401 0400 0401  ................
+000015e0: 0600 02fe 04ff 0a06 0601 1202 1002 0201  ................
+000015f0: 02ff 0404 0801 1001 1201 0802 0601 08ff  ................
+00001600: 0c03 0802 0402 0c01 0601 0401 0e01 08fd  ................
+00001610: 0a05 0e02 0601 0601 0400 02ff 0a03 0603  ................
+00001620: 02fd 0c05 7a2a 534f 4e4f 5347 6174 6577  ....z*SONOSGatew
+00001630: 6179 4861 6e64 6c65 722e 6469 7363 6f76  ayHandler.discov
+00001640: 6572 5f73 6f6e 6f73 5f70 6c61 7965 7273  er_sonos_players
+00001650: 6302 0000 0000 0000 0000 0000 0006 0000  c...............
+00001660: 0009 0000 0043 0000 0073 e800 0000 7400  .....C...s....t.
+00001670: 6401 7c01 9b00 6402 9d03 8301 0100 7401  d.|...d.......t.
+00001680: 6a02 6a03 7c01 6a04 6403 1900 6404 8d01  j.j.|.j.d...d...
+00001690: 7d02 7a0e 7c02 6a05 a006 a100 7d03 5700  }.z.|.j.....}.W.
+000016a0: 6e22 0100 0100 0100 6405 7c01 5f07 6406  n"......d.|._.d.
+000016b0: 7c01 5f08 7c01 a009 a100 0100 5900 6400  |._.|.......Y.d.
+000016c0: 5300 5800 6407 6408 6405 6409 9c03 7d04  S.X.d.d.d.d...}.
+000016d0: 7c04 a003 7c03 a003 640a 640b a102 640b  |...|...d.d...d.
+000016e0: a102 7c01 5f07 7a0c 7c02 a00a a100 7d05  ..|._.z.|.....}.
+000016f0: 5700 6e1c 0100 0100 0100 6406 7c01 5f08  W.n.......d.|._.
+00001700: 7c01 a009 a100 0100 5900 6400 5300 5800  |.......Y.d.S.X.
+00001710: 7c01 6a0b a00c 7c05 640c 1900 740d 7c05  |.j...|.d...t.|.
+00001720: 640d 1900 8301 740d 7c05 640e 1900 8301  d.....t.|.d.....
+00001730: 7c02 6a05 6a0e 7c02 6a05 6a0f 7c02 6a05  |.j.j.|.j.j.|.j.
+00001740: 6a10 640f 9c06 a101 0100 7c01 a009 a100  j.d.......|.....
+00001750: 0100 6400 5300 2910 4e7a 0643 6865 636b  ..d.S.).Nz.Check
+00001760: 207a 0720 7374 6174 6521 7213 0000 0072   z. state!r....r
+00001770: 1400 0000 da07 7374 6f70 7065 6446 725a  ......stoppedFrZ
+00001780: 0000 00da 0670 6175 7365 6429 0372 4700  .....paused).rG.
+00001790: 0000 5a0f 5041 5553 4544 5f50 4c41 5942  ..Z.PAUSED_PLAYB
+000017a0: 4143 4b72 4900 0000 7246 0000 0072 4900  ACKrI...rF...rI.
+000017b0: 0000 726c 0000 00da 0864 7572 6174 696f  ..rl.....duratio
+000017c0: 6eda 0870 6f73 6974 696f 6e29 0672 6c00  n..position).rl.
+000017d0: 0000 727d 0000 0072 7e00 0000 7222 0000  ..r}...r~...r"..
+000017e0: 0072 1d00 0000 721e 0000 0029 1172 4d00  .r....r....).rM.
+000017f0: 0000 720d 0000 0072 2700 0000 7228 0000  ..r....r'...r(..
+00001800: 0072 2900 0000 722b 0000 0072 5000 0000  .r)...r+...rP...
+00001810: 723b 0000 00da 0561 6c69 7665 7278 0000  r;.....aliverx..
+00001820: 0072 5100 0000 7279 0000 0072 4c00 0000  .rQ...ry...rL...
+00001830: 720f 0000 0072 2200 0000 721d 0000 0072  r....r"...r....r
+00001840: 2e00 0000 2906 7239 0000 005a 0f73 6f6e  ....).r9...Z.son
+00001850: 6f73 5f63 6f6d 706f 6e65 6e74 723c 0000  os_componentr<..
+00001860: 0072 5500 0000 5a09 7374 6174 655f 6d61  .rU...Z.state_ma
+00001870: 70da 0469 6e66 6f72 4000 0000 7240 0000  p..infor@...r@..
+00001880: 0072 4100 0000 7238 0000 0008 0100 0073  .rA...r8.......s
+00001890: 4400 0000 0001 1001 0601 08ff 0603 0201  D...............
+000018a0: 0e01 0601 0601 0601 0801 0803 0201 0201  ................
+000018b0: 02fd 0605 0401 0a01 02fe 0605 0201 0c01  ................
+000018c0: 0601 0601 0801 0802 0601 0601 0a01 0a01  ................
+000018d0: 0601 0601 06fa 0809 7a25 534f 4e4f 5347  ........z%SONOSG
+000018e0: 6174 6577 6179 4861 6e64 6c65 722e 636f  atewayHandler.co
+000018f0: 6d70 5f73 7461 7465 5f75 7064 6174 654e  mp_state_updateN
+00001900: 290f da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00001910: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00001920: 6e61 6d65 5f5f 7262 0000 0072 0800 0000  name__rb...r....
+00001930: da0b 636f 6e66 6967 5f66 6f72 6dda 0e70  ..config_form..p
+00001940: 6572 696f 6469 635f 7461 736b 7372 4a00  eriodic_tasksrJ.
+00001950: 0000 7261 0000 0072 4200 0000 7236 0000  ..ra...rB...r6..
+00001960: 0072 1100 0000 7212 0000 0072 5c00 0000  .r....r....r\...
+00001970: 7238 0000 0072 4000 0000 7240 0000 0072  r8...r@...r@...r
+00001980: 4000 0000 7241 0000 0072 1000 0000 1000  @...rA...r......
+00001990: 0000 7316 0000 0008 0104 0104 0204 0504  ..s.............
+000019a0: 0104 0208 3108 4e08 0908 1108 5372 1000  ....1.N.....Sr..
+000019b0: 0000 291b 724b 0000 0072 3400 0000 da08  ..).rK...r4.....
+000019c0: 6461 7465 7469 6d65 7202 0000 00da 0c64  datetimer......d
+000019d0: 6a61 6e67 6f2e 7574 696c 7372 0300 0000  jango.utilsr....
+000019e0: 722b 0000 0072 0400 0000 7205 0000 005a  r+...r....r....Z
+000019f0: 0d73 6f63 6f2e 736e 6170 7368 6f74 7206  .soco.snapshotr.
+00001a00: 0000 005a 1273 696d 6f2e 636f 7265 2e67  ...Z.simo.core.g
+00001a10: 6174 6577 6179 7372 0700 0000 5a0f 7369  atewaysr....Z.si
+00001a20: 6d6f 2e63 6f72 652e 666f 726d 7372 0800  mo.core.formsr..
+00001a30: 0000 da10 7369 6d6f 2e63 6f72 652e 6d6f  ....simo.core.mo
+00001a40: 6465 6c73 7209 0000 00da 1773 696d 6f2e  delsr......simo.
+00001a50: 636f 7265 2e75 7469 6c73 2e68 656c 7065  core.utils.helpe
+00001a60: 7273 720a 0000 005a 1673 696d 6f2e 6d75  rsr....Z.simo.mu
+00001a70: 6c74 696d 6564 6961 2e6d 6f64 656c 7372  ltimedia.modelsr
+00001a80: 0b00 0000 da06 6d6f 6465 6c73 720d 0000  ......modelsr...
+00001a90: 0072 0e00 0000 da05 7574 696c 7372 0f00  .r......utilsr..
+00001aa0: 0000 7210 0000 0072 4000 0000 7240 0000  ..r....r@...r@..
+00001ab0: 0072 4000 0000 7241 0000 00da 083c 6d6f  .r@...rA.....<mo
+00001ac0: 6475 6c65 3e01 0000 0073 1a00 0000 0801  dule>....s......
+00001ad0: 0801 0c01 0c01 1001 0c01 0c01 0c01 0c01  ................
+00001ae0: 0c01 0c01 1001 0c03                      ........
```

### Comparing `simo-sonos-1.1.3/src/simo_sonos/__pycache__/models.cpython-38.pyc` & `simo_sonos-1.2.4/src/simo_sonos/__pycache__/models.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `simo-sonos-1.1.3/src/simo_sonos/admin.py` & `simo_sonos-1.2.4/src/simo_sonos/admin.py`

 * *Files identical despite different names*

### Comparing `simo-sonos-1.1.3/src/simo_sonos/gateways.py` & `simo_sonos-1.2.4/src/simo_sonos/gateways.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,35 +23,63 @@
     )
 
     playing_alerts = {}
     watch_second = 0
 
     def perform_value_send(self, component, value):
         sonos_player = SonosPlayer.objects.get(id=component.config['sonos_device'])
-        if value == 'check_state':
-            self.comp_state_update(component)
+
+        print(f"{component}: {value}!")
+
+        if value in (
+            'play', 'pause', 'stop', 'next', 'previous',
+        ):
+            getattr(sonos_player.soco, value)()
 
         elif isinstance(value, dict):
-            if 'alert' in value:
+            if 'seek' in value:
+                sonos_player.soco.seek(timedelta(seconds=value['seek']))
+            elif 'set_volume' in value:
+                sonos_player.soco.volume = value['set_volume']
+            elif 'shuffle' in value:
+                sonos_player.soco.shuffle = value['shuffle']
+            elif 'loop' in value:
+                sonos_player.soco.repeat = value['loop']
+            elif 'play_from_library' in value:
+                if value['play_from_library'].get('type') != 'sonos_playlist':
+                    return
+                playlist = SonosPlaylist.objects.filter(
+                    id=value['play_from_library'].get('id', 0)
+                ).first()
+                if not playlist:
+                    return
+                component.play_playlist(playlist)
+            elif 'play_uri' in value:
+                if value.get('volume') != None:
+                    sonos_player.soco.volume = value['volume']
+                sonos_player.soco.play_uri(value['play_uri'])
+
+            elif 'alert' in value:
                 try:
                     sound_id = int(value['alert'])
                 except:
                     uri = value['alert']
                     length = None
                 else:
                     sound = Sound.objects.get(pk=sound_id)
                     length = sound.length
                     uri = f"http://{get_self_ip()}{sound.get_absolute_url()}"
-
                 threading.Thread(
                     target=self.play_alert, args=(
                         sonos_player, uri, length, value.get('volume')
                     )
                 ).start()
 
+        self.comp_state_update(component)
+
     def play_alert(self, sonos_player, uri, length, volume):
         if sonos_player.id not in self.playing_alerts:
             self.playing_alerts[sonos_player.id] = {
                 'snap': Snapshot(sonos_player.soco),
                 'uri': uri, 'timestamp': time.time()
             }
             self.playing_alerts[sonos_player.id]['snap'].snapshot()
@@ -255,15 +283,15 @@
         }
         sonos_component.value = state_map.get(
             status.get('current_transport_state', 'STOPPED'),
             'STOPPED'
         )
 
         try:
-            info = sonos_player.get_current_track_info()
+            info = sonos_player.soco.get_current_track_info()
         except:
             sonos_component.alive = False
             sonos_component.save()
             return
 
         sonos_component.meta.update({
             'title': info['title'],
```

### Comparing `simo-sonos-1.1.3/src/simo_sonos/migrations/0001_initial.py` & `simo_sonos-1.2.4/src/simo_sonos/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `simo-sonos-1.1.3/src/simo_sonos/migrations/__pycache__/0001_initial.cpython-38.pyc` & `simo_sonos-1.2.4/src/simo_sonos/migrations/__pycache__/0001_initial.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `simo-sonos-1.1.3/src/simo_sonos/migrations/__pycache__/0002_rename_master_sonosplayer_slave_of.cpython-38.pyc` & `simo_sonos-1.2.4/src/simo_sonos/migrations/__pycache__/0002_rename_master_sonosplayer_slave_of.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `simo-sonos-1.1.3/src/simo_sonos/migrations/__pycache__/0003_alter_sonosplaylist_item_id.cpython-38.pyc` & `simo_sonos-1.2.4/src/simo_sonos/migrations/__pycache__/0003_alter_sonosplaylist_item_id.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `simo-sonos-1.1.3/src/simo_sonos/models.py` & `simo_sonos-1.2.4/src/simo_sonos/models.py`

 * *Files identical despite different names*

### Comparing `simo-sonos-1.1.3/src/simo_sonos.egg-info/PKG-INFO` & `simo_sonos-1.2.4/src/simo_sonos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simo-sonos
-Version: 1.1.3
+Version: 1.2.4
 Summary: SONOS integration for SIMO.io
 Author-email: Simanas Venčkauskas <simanas@simo.io>
 Project-URL: Homepage, https://github.com/SIMO-io/simo-sonos
 Project-URL: Issues, https://github.com/SIMO-io/simo-sonos/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simo-sonos-1.1.3/src/simo_sonos.egg-info/SOURCES.txt` & `simo_sonos-1.2.4/src/simo_sonos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

