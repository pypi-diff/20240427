# Comparing `tmp/jy_lib-0.6.8.tar.gz` & `tmp/jy_lib-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jy_lib-0.6.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "jy_lib-0.6.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `jy_lib-0.6.8.tar` & `jy_lib-0.6.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     2083 2023-10-19 03:06:08.475402 jy_lib-0.6.8/.gitignore
--rw-r--r--   0        0        0      285 2023-10-23 02:58:33.543130 jy_lib-0.6.8/.pypirc
--rw-r--r--   0        0        0     1073 2023-10-19 06:46:25.394076 jy_lib-0.6.8/LICENSE
--rw-r--r--   0        0        0      573 2024-04-11 01:31:08.426951 jy_lib-0.6.8/Pipfile
--rw-r--r--   0        0        0    40838 2023-02-28 09:06:11.940000 jy_lib-0.6.8/Pipfile.lock
--rw-r--r--   0        0        0       10 2023-10-19 06:54:49.519221 jy_lib-0.6.8/README.md
--rw-r--r--   0        0        0      469 2023-10-19 08:27:51.652921 jy_lib-0.6.8/README_Project.md
--rw-r--r--   0        0        0      518 2024-04-26 07:26:33.355887 jy_lib-0.6.8/jy_lib/__init__.py
--rw-r--r--   0        0        0     7230 2023-10-25 01:56:08.575822 jy_lib-0.6.8/jy_lib/auth_client.py
--rw-r--r--   0        0        0    10531 2023-10-25 08:34:10.093160 jy_lib-0.6.8/jy_lib/bank.py
--rw-r--r--   0        0        0      809 2023-10-23 02:40:21.784597 jy_lib-0.6.8/jy_lib/base.py
--rw-r--r--   0        0        0    11456 2024-04-26 07:26:18.749728 jy_lib-0.6.8/jy_lib/cache.py
--rw-r--r--   0        0        0     3356 2024-04-15 08:39:28.625202 jy_lib-0.6.8/jy_lib/clickhouse.py
--rw-r--r--   0        0        0     4411 2024-04-11 01:28:25.533046 jy_lib-0.6.8/jy_lib/compressor.py
--rw-r--r--   0        0        0    21765 2023-10-25 08:34:10.093378 jy_lib-0.6.8/jy_lib/country.py
--rw-r--r--   0        0        0    10928 2023-10-25 08:34:10.093573 jy_lib-0.6.8/jy_lib/currency.py
--rw-r--r--   0        0        0     2399 2024-01-16 00:58:10.482893 jy_lib-0.6.8/jy_lib/date.py
--rw-r--r--   0        0        0      931 2023-10-27 09:01:08.015737 jy_lib-0.6.8/jy_lib/decorator.py
--rw-r--r--   0        0        0     5916 2024-04-24 02:27:16.042289 jy_lib-0.6.8/jy_lib/exchange.py
--rw-r--r--   0        0        0      602 2024-03-26 02:17:46.967953 jy_lib-0.6.8/jy_lib/interrupt_protect.py
--rw-r--r--   0        0        0     2151 2023-10-25 05:47:55.730076 jy_lib-0.6.8/jy_lib/lock.py
--rw-r--r--   0        0        0      707 2024-01-17 07:58:34.306588 jy_lib-0.6.8/jy_lib/math.py
--rw-r--r--   0        0        0     5926 2023-12-21 06:12:51.186402 jy_lib-0.6.8/jy_lib/nav.py
--rw-r--r--   0        0        0    18478 2024-04-17 00:51:09.235795 jy_lib-0.6.8/jy_lib/smb_client.py
--rw-r--r--   0        0        0    22173 2024-04-26 03:29:55.565762 jy_lib-0.6.8/jy_lib/symbol.py
--rw-r--r--   0        0        0    20726 2024-03-23 07:36:23.764234 jy_lib-0.6.8/jy_lib/symbol_em.py
--rw-r--r--   0        0        0      577 2023-11-03 01:23:44.753118 jy_lib-0.6.8/jy_lib/time.py
--rw-r--r--   0        0        0       67 2023-10-19 06:54:09.145568 jy_lib-0.6.8/publish-jypi.sh
--rw-r--r--   0        0        0       67 2023-10-19 06:53:07.001372 jy_lib-0.6.8/publish-pypi.sh
--rw-r--r--   0        0        0       67 2023-10-19 06:54:14.808768 jy_lib-0.6.8/publish-test.sh
--rw-r--r--   0        0        0      639 2024-04-11 07:52:56.404049 jy_lib-0.6.8/pyproject.toml
--rw-r--r--   0        0        0      117 2024-04-15 07:06:48.431549 jy_lib-0.6.8/requirements.txt
--rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 jy_lib-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0     2083 2024-01-01 02:29:02.554641 jy_lib-0.6.9/.gitignore
+-rw-r--r--   0        0        0      285 2024-01-01 02:29:02.554755 jy_lib-0.6.9/.pypirc
+-rw-r--r--   0        0        0     1073 2024-01-01 02:29:02.555085 jy_lib-0.6.9/LICENSE
+-rw-r--r--   0        0        0      573 2024-04-21 14:22:14.414420 jy_lib-0.6.9/Pipfile
+-rw-r--r--   0        0        0    40838 2024-01-01 02:29:02.555480 jy_lib-0.6.9/Pipfile.lock
+-rw-r--r--   0        0        0       10 2024-01-01 02:29:02.555572 jy_lib-0.6.9/README.md
+-rw-r--r--   0        0        0      469 2024-01-01 02:29:02.555665 jy_lib-0.6.9/README_Project.md
+-rw-r--r--   0        0        0      518 2024-04-26 13:44:52.664545 jy_lib-0.6.9/jy_lib/__init__.py
+-rw-r--r--   0        0        0     7230 2024-01-01 02:29:02.555927 jy_lib-0.6.9/jy_lib/auth_client.py
+-rw-r--r--   0        0        0    10531 2024-01-01 02:29:02.556043 jy_lib-0.6.9/jy_lib/bank.py
+-rw-r--r--   0        0        0      809 2024-01-01 02:29:02.556135 jy_lib-0.6.9/jy_lib/base.py
+-rw-r--r--   0        0        0    11460 2024-04-26 13:44:43.888654 jy_lib-0.6.9/jy_lib/cache.py
+-rw-r--r--   0        0        0     3356 2024-04-21 14:22:14.415034 jy_lib-0.6.9/jy_lib/clickhouse.py
+-rw-r--r--   0        0        0     4411 2024-04-21 14:22:14.415174 jy_lib-0.6.9/jy_lib/compressor.py
+-rw-r--r--   0        0        0    21765 2024-01-01 02:29:02.556414 jy_lib-0.6.9/jy_lib/country.py
+-rw-r--r--   0        0        0    10928 2024-01-01 02:29:02.556554 jy_lib-0.6.9/jy_lib/currency.py
+-rw-r--r--   0        0        0     2399 2024-04-21 14:22:14.416027 jy_lib-0.6.9/jy_lib/date.py
+-rw-r--r--   0        0        0      931 2024-01-01 02:29:02.556726 jy_lib-0.6.9/jy_lib/decorator.py
+-rw-r--r--   0        0        0     5916 2024-04-26 13:44:43.889079 jy_lib-0.6.9/jy_lib/exchange.py
+-rw-r--r--   0        0        0      602 2024-04-21 14:22:14.416177 jy_lib-0.6.9/jy_lib/interrupt_protect.py
+-rw-r--r--   0        0        0     2151 2024-01-01 02:29:02.556936 jy_lib-0.6.9/jy_lib/lock.py
+-rw-r--r--   0        0        0      707 2024-04-21 14:22:14.416596 jy_lib-0.6.9/jy_lib/math.py
+-rw-r--r--   0        0        0     5926 2024-01-01 02:29:02.557127 jy_lib-0.6.9/jy_lib/nav.py
+-rw-r--r--   0        0        0    18478 2024-04-21 14:22:14.416811 jy_lib-0.6.9/jy_lib/smb_client.py
+-rw-r--r--   0        0        0    22173 2024-04-26 13:44:43.889377 jy_lib-0.6.9/jy_lib/symbol.py
+-rw-r--r--   0        0        0    20726 2024-04-21 14:22:14.417332 jy_lib-0.6.9/jy_lib/symbol_em.py
+-rw-r--r--   0        0        0      577 2024-01-01 02:29:02.557631 jy_lib-0.6.9/jy_lib/time.py
+-rw-r--r--   0        0        0       67 2024-01-01 02:29:02.557712 jy_lib-0.6.9/publish-jypi.sh
+-rw-r--r--   0        0        0       67 2024-01-01 02:29:02.557791 jy_lib-0.6.9/publish-pypi.sh
+-rw-r--r--   0        0        0       67 2024-01-01 02:29:02.557873 jy_lib-0.6.9/publish-test.sh
+-rw-r--r--   0        0        0      639 2024-04-21 14:22:14.417488 jy_lib-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0      117 2024-04-21 14:22:14.417721 jy_lib-0.6.9/requirements.txt
+-rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 jy_lib-0.6.9/PKG-INFO
```

### Comparing `jy_lib-0.6.8/.gitignore` & `jy_lib-0.6.9/.gitignore`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.8/LICENSE` & `jy_lib-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.8/Pipfile` & `jy_lib-0.6.9/Pipfile`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.8/Pipfile.lock` & `jy_lib-0.6.9/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.8/jy_lib/__init__.py` & `jy_lib-0.6.9/jy_lib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     SymbolFlag,
     SymbolSubType,
     SymbolType,
     WarrantsType,
 )
 from .symbol_em import EMParser, KLineRecord, TrendRecord
 
-__version__ = "0.6.8"
+__version__ = "0.6.9"
```

### Comparing `jy_lib-0.6.8/jy_lib/auth_client.py` & `jy_lib-0.6.9/jy_lib/auth_client.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.8/jy_lib/bank.py` & `jy_lib-0.6.9/jy_lib/bank.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.8/jy_lib/base.py` & `jy_lib-0.6.9/jy_lib/base.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.8/jy_lib/cache.py` & `jy_lib-0.6.9/jy_lib/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,17 +90,17 @@
             if len(value) <= self.compress_min_size:
                 return value, 0     # 原始数据
             else:
                 return lz4.frame.compress(value), 3     # 仅压缩
         else:
             payload: bytes = pickle.dumps(value)
             if len(payload) <= self.compress_min_size:
-                return value, 4                         # 仅序列化
+                return payload, 4                         # 仅序列化
             else:
-                return lz4.frame.compress(value), 5     # 序列化并压缩
+                return lz4.frame.compress(payload), 5     # 序列化并压缩
 
     @classmethod
     def decode_value(cls, value: Any, encoding: int) -> Any:
         """数据解码"""
         match encoding:
             case 0:
                 return value
```

### Comparing `jy_lib-0.6.8/jy_lib/clickhouse.py` & `jy_lib-0.6.9/jy_lib/clickhouse.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.8/jy_lib/compressor.py` & `jy_lib-0.6.9/jy_lib/compressor.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.8/jy_lib/country.py` & `jy_lib-0.6.9/jy_lib/country.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.8/jy_lib/currency.py` & `jy_lib-0.6.9/jy_lib/currency.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.8/jy_lib/date.py` & `jy_lib-0.6.9/jy_lib/date.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.8/jy_lib/decorator.py` & `jy_lib-0.6.9/jy_lib/decorator.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.8/jy_lib/exchange.py` & `jy_lib-0.6.9/jy_lib/exchange.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.8/jy_lib/interrupt_protect.py` & `jy_lib-0.6.9/jy_lib/interrupt_protect.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.8/jy_lib/lock.py` & `jy_lib-0.6.9/jy_lib/lock.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.8/jy_lib/math.py` & `jy_lib-0.6.9/jy_lib/math.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.8/jy_lib/nav.py` & `jy_lib-0.6.9/jy_lib/nav.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.8/jy_lib/smb_client.py` & `jy_lib-0.6.9/jy_lib/smb_client.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.8/jy_lib/symbol.py` & `jy_lib-0.6.9/jy_lib/symbol.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.8/jy_lib/symbol_em.py` & `jy_lib-0.6.9/jy_lib/symbol_em.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.8/jy_lib/time.py` & `jy_lib-0.6.9/jy_lib/time.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.8/pyproject.toml` & `jy_lib-0.6.9/pyproject.toml`

 * *Files identical despite different names*

