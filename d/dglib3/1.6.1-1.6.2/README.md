# Comparing `tmp/dglib3-1.6.1-py3-none-any.whl.zip` & `tmp/dglib3-1.6.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 21218 bytes, number of entries: 20
--rw-rw-rw-  2.0 fat       67 b- defN 22-Oct-29 19:02 dglib3/__init__.py
+Zip file size: 21306 bytes, number of entries: 20
+-rw-rw-rw-  2.0 fat       67 b- defN 24-Apr-27 14:08 dglib3/__init__.py
 -rw-rw-rw-  2.0 fat     3875 b- defN 22-Jul-17 06:14 dglib3/cache_util.py
 -rw-rw-rw-  2.0 fat      546 b- defN 20-Jun-04 14:22 dglib3/codecs.py
 -rw-rw-rw-  2.0 fat     1945 b- defN 21-Aug-15 13:11 dglib3/db_util.py
 -rw-rw-rw-  2.0 fat      752 b- defN 20-Jun-04 14:22 dglib3/dumper.py
 -rw-rw-rw-  2.0 fat     1838 b- defN 20-Jun-04 14:22 dglib3/logutil.py
 -rw-rw-rw-  2.0 fat     5850 b- defN 21-Sep-14 02:22 dglib3/tracer.py
 -rw-rw-rw-  2.0 fat     7033 b- defN 22-Oct-29 19:00 dglib3/utils.py
 -rw-rw-rw-  2.0 fat     5990 b- defN 20-Jul-12 17:55 dglib3/win_util.py
 -rw-rw-rw-  2.0 fat        0 b- defN 20-Jun-04 14:22 dglib3/basis/__init__.py
 -rw-rw-rw-  2.0 fat      331 b- defN 22-Oct-23 10:21 dglib3/basis/ordered_dict.py
--rw-rw-rw-  2.0 fat    12675 b- defN 15-Nov-27 14:42 dglib3/basis/pydicti.py
+-rw-rw-rw-  2.0 fat    12865 b- defN 24-Apr-27 14:06 dglib3/basis/pydicti.py
 -rw-rw-rw-  2.0 fat     2768 b- defN 20-Jun-04 14:22 dglib3/basis/singleton.py
 -rw-rw-rw-  2.0 fat        0 b- defN 15-Nov-27 14:42 dglib3/config/__init__.py
 -rw-rw-rw-  2.0 fat     5333 b- defN 22-Oct-23 13:39 dglib3/config/inifiles.py
--rw-rw-rw-  2.0 fat     1092 b- defN 22-Oct-29 19:04 dglib3-1.6.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1056 b- defN 22-Oct-29 19:04 dglib3-1.6.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Oct-29 19:04 dglib3-1.6.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 22-Oct-29 19:04 dglib3-1.6.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1528 b- defN 22-Oct-29 19:04 dglib3-1.6.1.dist-info/RECORD
-20 files, 52778 bytes uncompressed, 18762 bytes compressed:  64.5%
+-rw-rw-rw-  2.0 fat     1092 b- defN 24-Apr-27 14:31 dglib3-1.6.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1063 b- defN 24-Apr-27 14:31 dglib3-1.6.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-27 14:31 dglib3-1.6.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 24-Apr-27 14:31 dglib3-1.6.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1528 b- defN 24-Apr-27 14:31 dglib3-1.6.2.dist-info/RECORD
+20 files, 52975 bytes uncompressed, 18850 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: dglib3/config/__init__.py
 Comment: 
 
 Filename: dglib3/config/inifiles.py
 Comment: 
 
-Filename: dglib3-1.6.1.dist-info/LICENSE
+Filename: dglib3-1.6.2.dist-info/LICENSE
 Comment: 
 
-Filename: dglib3-1.6.1.dist-info/METADATA
+Filename: dglib3-1.6.2.dist-info/METADATA
 Comment: 
 
-Filename: dglib3-1.6.1.dist-info/WHEEL
+Filename: dglib3-1.6.2.dist-info/WHEEL
 Comment: 
 
-Filename: dglib3-1.6.1.dist-info/top_level.txt
+Filename: dglib3-1.6.2.dist-info/top_level.txt
 Comment: 
 
-Filename: dglib3-1.6.1.dist-info/RECORD
+Filename: dglib3-1.6.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dglib3/__init__.py

```diff
@@ -1,4 +1,4 @@
 
 __author__ = 'DDGG'
-__version__ = '1.6.1'
+__version__ = '1.6.2'
 __license__ = 'MIT'
```

## dglib3/basis/pydicti.py

```diff
@@ -152,16 +152,23 @@
 
 This program  is free software.  It comes  without any warranty,  to the
 extent permitted by applicable law.
 
 """
 __all__ = ['build_dicti', 'Dicti', 'odicti', 'dicti']
 
+import sys
 import sys as _sys
-from collections import MutableMapping as _MutableMapping
+
+# 2024-04-27 (DDGG): Compatible with Python 3.10 and above versions.
+if sys.version_info >= (3, 10):
+    from collections.abc import MutableMapping as _MutableMapping
+else:
+    from collections import MutableMapping as _MutableMapping
+
 from copy import deepcopy as _deepcopy
 
 try:
     from collections import OrderedDict
 except ImportError:
     try:
         from ordereddict import OrderedDict
```

## Comparing `dglib3-1.6.1.dist-info/LICENSE` & `dglib3-1.6.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dglib3-1.6.1.dist-info/METADATA` & `dglib3-1.6.2.dist-info/METADATA`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,29 @@
-Metadata-Version: 2.1
-Name: dglib3
-Version: 1.6.1
-Summary: Daemon glance lib (for py3)
-Home-page: https://github.com/ddcatgg/dglib3
-Author: DDGG
-Author-email: 990080@qq.com
-License: UNKNOWN
-Keywords: util,tool,ddgg
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Other Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-License-File: LICENSE
-
-Daemon glance lib
------------------
-
-This library provides a number of commonly used functions and classes, but also
-the integration of a number of third-party modules, to facilitate the development.
-
-At present, for the Windows platform, is being ported to linux.
-
-
+Metadata-Version: 2.1
+Name: dglib3
+Version: 1.6.2
+Summary: Daemon glance lib (for py3)
+Home-page: https://github.com/ddcatgg/dglib3
+Download-URL: 
+Author: DDGG
+Author-email: 990080@qq.com
+Keywords: util,tool,ddgg
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Other Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+License-File: LICENSE
+
+Daemon glance lib
+-----------------
+
+This library provides a number of commonly used functions and classes, but also
+the integration of a number of third-party modules, to facilitate the development.
+
+At present, for the Windows platform, is being ported to linux.
```

## Comparing `dglib3-1.6.1.dist-info/RECORD` & `dglib3-1.6.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-dglib3/__init__.py,sha256=QaouiazYK_RoMDLKwdmWou_HJzGMV0Ebprqa51BP6dQ,67
+dglib3/__init__.py,sha256=Ajb9dD0UyQdNj_Zt3SX5Ih4iU1l0f8Cbvigau6TSJ8I,67
 dglib3/cache_util.py,sha256=JYy_nV4LBbjmPZr8ehQApCx8WsDr4oTSkiz2Vhufd78,3875
 dglib3/codecs.py,sha256=ze-CY0QIjB1kOgzHH_t9ECSOPtx5bGAnsPMQd-7kfpg,546
 dglib3/db_util.py,sha256=lzUyRGvgq0aq34bSKgph0R8vHzQMtDD5J2lhItnjzoU,1945
 dglib3/dumper.py,sha256=RRT5yUncyv7LheGV6Qy4UV14LhT_ecp-hWtb_J4tkY0,752
 dglib3/logutil.py,sha256=BTaycEUYAYZtb6YitBCEFYXVEmGvN9I2yQPGoevtN9o,1838
 dglib3/tracer.py,sha256=6vVvl-PnOAgFsLFEpH3B7_YHyiw-wuKxATK8JTiuJdw,5850
 dglib3/utils.py,sha256=UHd3gXiyiQA4Ibc0KLZuonRPZUx1x_mag0ouFuBZvY8,7033
 dglib3/win_util.py,sha256=kdWWqA1G9wiczPRy6J2LIvBcJhTone1ROcx35LUx9bI,5990
 dglib3/basis/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dglib3/basis/ordered_dict.py,sha256=PfILJ0IPGnKIovLlnRmT5hh-gPNOEgOPsE7ocOZNxPc,331
-dglib3/basis/pydicti.py,sha256=yrZuU6b2YUFQfMUt0Fv0BmHA9fK03VdfdETvoFt8fnk,12675
+dglib3/basis/pydicti.py,sha256=pMOA_fpg-xrVUQkft5M7k5o3bH8-Hdkj4Tv9EOz9EYE,12865
 dglib3/basis/singleton.py,sha256=qFqnyPtuWd9dq9qSfyTNq9wibQ7p7sDQg3tXjoD4pNY,2768
 dglib3/config/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dglib3/config/inifiles.py,sha256=CsmShDnGiFlE8c5eOBA_Vu4gS6FZaW01dod_SApxlpA,5333
-dglib3-1.6.1.dist-info/LICENSE,sha256=ULKueyzuY3juudXduTPi2ek-V_oQESUghSJAY9E2OFs,1092
-dglib3-1.6.1.dist-info/METADATA,sha256=mOLthv5WwkwBihIpDLSueUbIpEduTI-OCzqhyrXGGZY,1056
-dglib3-1.6.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dglib3-1.6.1.dist-info/top_level.txt,sha256=MWDKK548gWwsWJtHrc5RXPucVp0vSjtxiyZOJzhAPoY,7
-dglib3-1.6.1.dist-info/RECORD,,
+dglib3-1.6.2.dist-info/LICENSE,sha256=ULKueyzuY3juudXduTPi2ek-V_oQESUghSJAY9E2OFs,1092
+dglib3-1.6.2.dist-info/METADATA,sha256=GpqMoMxA9B9HmHd-ES_h4WGNh4NLzJFrGSYhawrQSh0,1063
+dglib3-1.6.2.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+dglib3-1.6.2.dist-info/top_level.txt,sha256=MWDKK548gWwsWJtHrc5RXPucVp0vSjtxiyZOJzhAPoY,7
+dglib3-1.6.2.dist-info/RECORD,,
```

