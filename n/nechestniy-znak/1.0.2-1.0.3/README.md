# Comparing `tmp/nechestniy_znak-1.0.2.tar.gz` & `tmp/nechestniy_znak-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nechestniy_znak-1.0.2.tar", last modified: Wed Apr 24 14:52:14 2024, max compression
+gzip compressed data, was "nechestniy_znak-1.0.3.tar", last modified: Sat Apr 27 16:25:16 2024, max compression
```

## Comparing `nechestniy_znak-1.0.2.tar` & `nechestniy_znak-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:52:14.570920 nechestniy_znak-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-24 14:52:06.000000 nechestniy_znak-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-24 14:52:14.570920 nechestniy_znak-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-24 14:52:06.000000 nechestniy_znak-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-24 14:52:06.000000 nechestniy_znak-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:52:14.570920 nechestniy_znak-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:52:14.566920 nechestniy_znak-1.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 14:52:06.000000 nechestniy_znak-1.0.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:52:14.566920 nechestniy_znak-1.0.2/src/nechestniy_znak/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-24 14:52:06.000000 nechestniy_znak-1.0.2/src/nechestniy_znak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-24 14:52:06.000000 nechestniy_znak-1.0.2/src/nechestniy_znak/crpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-24 14:52:06.000000 nechestniy_znak-1.0.2/src/nechestniy_znak/egais.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:52:14.570920 nechestniy_znak-1.0.2/src/nechestniy_znak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-24 14:52:14.000000 nechestniy_znak-1.0.2/src/nechestniy_znak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-24 14:52:14.000000 nechestniy_znak-1.0.2/src/nechestniy_znak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:52:14.000000 nechestniy_znak-1.0.2/src/nechestniy_znak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 14:52:14.000000 nechestniy_znak-1.0.2/src/nechestniy_znak.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 14:52:14.000000 nechestniy_znak-1.0.2/src/nechestniy_znak.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:25:16.498327 nechestniy_znak-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-27 16:25:12.000000 nechestniy_znak-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-27 16:25:16.498327 nechestniy_znak-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-27 16:25:12.000000 nechestniy_znak-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-27 16:25:12.000000 nechestniy_znak-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 16:25:16.498327 nechestniy_znak-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:25:16.498327 nechestniy_znak-1.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 16:25:12.000000 nechestniy_znak-1.0.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:25:16.498327 nechestniy_znak-1.0.3/src/nechestniy_znak/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-27 16:25:12.000000 nechestniy_znak-1.0.3/src/nechestniy_znak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-27 16:25:12.000000 nechestniy_znak-1.0.3/src/nechestniy_znak/crpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-27 16:25:12.000000 nechestniy_znak-1.0.3/src/nechestniy_znak/egais.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:25:16.498327 nechestniy_znak-1.0.3/src/nechestniy_znak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-27 16:25:16.000000 nechestniy_znak-1.0.3/src/nechestniy_znak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-27 16:25:16.000000 nechestniy_znak-1.0.3/src/nechestniy_znak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:25:16.000000 nechestniy_znak-1.0.3/src/nechestniy_znak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-27 16:25:16.000000 nechestniy_znak-1.0.3/src/nechestniy_znak.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-27 16:25:16.000000 nechestniy_znak-1.0.3/src/nechestniy_znak.egg-info/top_level.txt
```

### Comparing `nechestniy_znak-1.0.2/LICENSE` & `nechestniy_znak-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nechestniy_znak-1.0.2/PKG-INFO` & `nechestniy_znak-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nechestniy_znak
-Version: 1.0.2
+Version: 1.0.3
 Summary: Библеотека обертка для API ГИС МТ “Честный Знак”
 Author-email: li0ard <li0ard@proton.me>
 Maintainer-email: li0ard <li0ard@proton.me>
 Project-URL: Homepage, https://github.com/li0ard/nechestniy_znak
 Project-URL: Issues, https://github.com/li0ard/nechestniy_znak/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
@@ -34,18 +34,18 @@
 ```
 
 ### Пример
 ```py
 from nechestniy_znak import Crpt, Egais
 
 crpt = Crpt()
-print(crpt.infoFromEAN13(46494139))
+print(crpt.infoFromEAN13("46494139"))
 print(crpt.infoFromDataMatrix("00000046209849Uon<TYfACyAJPHJ"))
 print(crpt.infoFromQr("chek.markirovka.nalog.ru/kc/?kiz=RU-430302-AAA4050108"))
 print(crpt.infoFromReceipt("t=20231203T2319&s=261.80&fn=7281440701309134&i=10027&fp=3516337491&n=1"))
 
 egais = Egais()
-print(egais.getInfoByMarkOld("22N00001543ZQO6QFMW37ZK80215021095854A4P1E4IHMW86GT5RTFHN5XXFABT9TZ9", "104-101355000854071217387105240265"))
-print(egais.getInfoByMarkNew("171200031066131018001EWB6ECS6IGT6L2OH7XP6QFJMTYQMXCZ5WWVPNDLUU7BCE4FWLCBM7QDHQSESJCTOIXMEAHE2EZLXRZXJJT4UJ4OKEFEIO7RE7J7LQK2ISDFXIA34UAYOZ5ZRYFLTXI4TQ"))
-print(egais.getInfoByAlcCode("0150320000003561384"))
+print(egais.infoFromOldMark("22N00001543ZQO6QFMW37ZK80215021095854A4P1E4IHMW86GT5RTFHN5XXFABT9TZ9", "104-101355000854071217387105240265"))
+print(egais.infoFromNewMark("171200031066131018001EWB6ECS6IGT6L2OH7XP6QFJMTYQMXCZ5WWVPNDLUU7BCE4FWLCBM7QDHQSESJCTOIXMEAHE2EZLXRZXJJT4UJ4OKEFEIO7RE7J7LQK2ISDFXIA34UAYOZ5ZRYFLTXI4TQ"))
+print(egais.infoFromAlcCode("0150320000003561384"))
 print(egais.getChains("171200031066131018001EWB6ECS6IGT6L2OH7XP6QFJMTYQMXCZ5WWVPNDLUU7BCE4FWLCBM7QDHQSESJCTOIXMEAHE2EZLXRZXJJT4UJ4OKEFEIO7RE7J7LQK2ISDFXIA34UAYOZ5ZRYFLTXI4TQ"))
 ```
```

### Comparing `nechestniy_znak-1.0.2/README.md` & `nechestniy_znak-1.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 ```
 
 ### Пример
 ```py
 from nechestniy_znak import Crpt, Egais
 
 crpt = Crpt()
-print(crpt.infoFromEAN13(46494139))
+print(crpt.infoFromEAN13("46494139"))
 print(crpt.infoFromDataMatrix("00000046209849Uon<TYfACyAJPHJ"))
 print(crpt.infoFromQr("chek.markirovka.nalog.ru/kc/?kiz=RU-430302-AAA4050108"))
 print(crpt.infoFromReceipt("t=20231203T2319&s=261.80&fn=7281440701309134&i=10027&fp=3516337491&n=1"))
 
 egais = Egais()
-print(egais.getInfoByMarkOld("22N00001543ZQO6QFMW37ZK80215021095854A4P1E4IHMW86GT5RTFHN5XXFABT9TZ9", "104-101355000854071217387105240265"))
-print(egais.getInfoByMarkNew("171200031066131018001EWB6ECS6IGT6L2OH7XP6QFJMTYQMXCZ5WWVPNDLUU7BCE4FWLCBM7QDHQSESJCTOIXMEAHE2EZLXRZXJJT4UJ4OKEFEIO7RE7J7LQK2ISDFXIA34UAYOZ5ZRYFLTXI4TQ"))
-print(egais.getInfoByAlcCode("0150320000003561384"))
+print(egais.infoFromOldMark("22N00001543ZQO6QFMW37ZK80215021095854A4P1E4IHMW86GT5RTFHN5XXFABT9TZ9", "104-101355000854071217387105240265"))
+print(egais.infoFromNewMark("171200031066131018001EWB6ECS6IGT6L2OH7XP6QFJMTYQMXCZ5WWVPNDLUU7BCE4FWLCBM7QDHQSESJCTOIXMEAHE2EZLXRZXJJT4UJ4OKEFEIO7RE7J7LQK2ISDFXIA34UAYOZ5ZRYFLTXI4TQ"))
+print(egais.infoFromAlcCode("0150320000003561384"))
 print(egais.getChains("171200031066131018001EWB6ECS6IGT6L2OH7XP6QFJMTYQMXCZ5WWVPNDLUU7BCE4FWLCBM7QDHQSESJCTOIXMEAHE2EZLXRZXJJT4UJ4OKEFEIO7RE7J7LQK2ISDFXIA34UAYOZ5ZRYFLTXI4TQ"))
 ```
```

### Comparing `nechestniy_znak-1.0.2/pyproject.toml` & `nechestniy_znak-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nechestniy_znak"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
     { name="li0ard", email="li0ard@proton.me" },
 ]
 maintainers = [
     {name = "li0ard", email = "li0ard@proton.me"}
 ]
 description = "Библеотека обертка для API ГИС МТ “Честный Знак”"
```

### Comparing `nechestniy_znak-1.0.2/src/nechestniy_znak/crpt.py` & `nechestniy_znak-1.0.3/src/nechestniy_znak/crpt.py`

 * *Files identical despite different names*

### Comparing `nechestniy_znak-1.0.2/src/nechestniy_znak/egais.py` & `nechestniy_znak-1.0.3/src/nechestniy_znak/egais.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 class Egais:
     def __init__(self):
         pass
     
     def _get(self, url: str, params: str) -> Union[list, dict]:
         return requests.get(f"http://mobapi.fsrar.ru/api3/{url}?{params}", verify=False).json()
     
-    def getInfoByMarkOld(self, pdf417: str, datamatrix: str) -> Union[list, dict]:
+    def infoFromOldMark(self, pdf417: str, datamatrix: str) -> Union[list, dict]:
         return self._get("mark", f"DataMatrix={datamatrix}&Pdf417={pdf417}")
 
-    def getInfoByMarkNew(self, datamatrix: str) -> Union[list, dict]:
+    def infoFromNewMark(self, datamatrix: str) -> Union[list, dict]:
         return self._get("marklong", f"Pdf417={datamatrix}")
 
-    def getInfoByAlcCode(self, alc_code: str) -> Union[list, dict]:
+    def infoFromAlcCode(self, alc_code: str) -> Union[list, dict]:
         return self._get("product_info", f"alc_code={alc_code}")
     
     def getChains(self, datamatrix: str) -> Union[list, dict]:
         return self._get("chain", f"barcode={datamatrix}")
```

### Comparing `nechestniy_znak-1.0.2/src/nechestniy_znak.egg-info/PKG-INFO` & `nechestniy_znak-1.0.3/src/nechestniy_znak.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nechestniy_znak
-Version: 1.0.2
+Version: 1.0.3
 Summary: Библеотека обертка для API ГИС МТ “Честный Знак”
 Author-email: li0ard <li0ard@proton.me>
 Maintainer-email: li0ard <li0ard@proton.me>
 Project-URL: Homepage, https://github.com/li0ard/nechestniy_znak
 Project-URL: Issues, https://github.com/li0ard/nechestniy_znak/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
@@ -34,18 +34,18 @@
 ```
 
 ### Пример
 ```py
 from nechestniy_znak import Crpt, Egais
 
 crpt = Crpt()
-print(crpt.infoFromEAN13(46494139))
+print(crpt.infoFromEAN13("46494139"))
 print(crpt.infoFromDataMatrix("00000046209849Uon<TYfACyAJPHJ"))
 print(crpt.infoFromQr("chek.markirovka.nalog.ru/kc/?kiz=RU-430302-AAA4050108"))
 print(crpt.infoFromReceipt("t=20231203T2319&s=261.80&fn=7281440701309134&i=10027&fp=3516337491&n=1"))
 
 egais = Egais()
-print(egais.getInfoByMarkOld("22N00001543ZQO6QFMW37ZK80215021095854A4P1E4IHMW86GT5RTFHN5XXFABT9TZ9", "104-101355000854071217387105240265"))
-print(egais.getInfoByMarkNew("171200031066131018001EWB6ECS6IGT6L2OH7XP6QFJMTYQMXCZ5WWVPNDLUU7BCE4FWLCBM7QDHQSESJCTOIXMEAHE2EZLXRZXJJT4UJ4OKEFEIO7RE7J7LQK2ISDFXIA34UAYOZ5ZRYFLTXI4TQ"))
-print(egais.getInfoByAlcCode("0150320000003561384"))
+print(egais.infoFromOldMark("22N00001543ZQO6QFMW37ZK80215021095854A4P1E4IHMW86GT5RTFHN5XXFABT9TZ9", "104-101355000854071217387105240265"))
+print(egais.infoFromNewMark("171200031066131018001EWB6ECS6IGT6L2OH7XP6QFJMTYQMXCZ5WWVPNDLUU7BCE4FWLCBM7QDHQSESJCTOIXMEAHE2EZLXRZXJJT4UJ4OKEFEIO7RE7J7LQK2ISDFXIA34UAYOZ5ZRYFLTXI4TQ"))
+print(egais.infoFromAlcCode("0150320000003561384"))
 print(egais.getChains("171200031066131018001EWB6ECS6IGT6L2OH7XP6QFJMTYQMXCZ5WWVPNDLUU7BCE4FWLCBM7QDHQSESJCTOIXMEAHE2EZLXRZXJJT4UJ4OKEFEIO7RE7J7LQK2ISDFXIA34UAYOZ5ZRYFLTXI4TQ"))
 ```
```

