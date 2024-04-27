# Comparing `tmp/jy_lib-0.6.9.tar.gz` & `tmp/jy_lib-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jy_lib-0.6.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "jy_lib-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `jy_lib-0.6.9.tar` & `jy_lib-0.7.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     2083 2024-01-01 02:29:02.554641 jy_lib-0.6.9/.gitignore
--rw-r--r--   0        0        0      285 2024-01-01 02:29:02.554755 jy_lib-0.6.9/.pypirc
--rw-r--r--   0        0        0     1073 2024-01-01 02:29:02.555085 jy_lib-0.6.9/LICENSE
--rw-r--r--   0        0        0      573 2024-04-21 14:22:14.414420 jy_lib-0.6.9/Pipfile
--rw-r--r--   0        0        0    40838 2024-01-01 02:29:02.555480 jy_lib-0.6.9/Pipfile.lock
--rw-r--r--   0        0        0       10 2024-01-01 02:29:02.555572 jy_lib-0.6.9/README.md
--rw-r--r--   0        0        0      469 2024-01-01 02:29:02.555665 jy_lib-0.6.9/README_Project.md
--rw-r--r--   0        0        0      518 2024-04-26 13:44:52.664545 jy_lib-0.6.9/jy_lib/__init__.py
--rw-r--r--   0        0        0     7230 2024-01-01 02:29:02.555927 jy_lib-0.6.9/jy_lib/auth_client.py
--rw-r--r--   0        0        0    10531 2024-01-01 02:29:02.556043 jy_lib-0.6.9/jy_lib/bank.py
--rw-r--r--   0        0        0      809 2024-01-01 02:29:02.556135 jy_lib-0.6.9/jy_lib/base.py
--rw-r--r--   0        0        0    11460 2024-04-26 13:44:43.888654 jy_lib-0.6.9/jy_lib/cache.py
--rw-r--r--   0        0        0     3356 2024-04-21 14:22:14.415034 jy_lib-0.6.9/jy_lib/clickhouse.py
--rw-r--r--   0        0        0     4411 2024-04-21 14:22:14.415174 jy_lib-0.6.9/jy_lib/compressor.py
--rw-r--r--   0        0        0    21765 2024-01-01 02:29:02.556414 jy_lib-0.6.9/jy_lib/country.py
--rw-r--r--   0        0        0    10928 2024-01-01 02:29:02.556554 jy_lib-0.6.9/jy_lib/currency.py
--rw-r--r--   0        0        0     2399 2024-04-21 14:22:14.416027 jy_lib-0.6.9/jy_lib/date.py
--rw-r--r--   0        0        0      931 2024-01-01 02:29:02.556726 jy_lib-0.6.9/jy_lib/decorator.py
--rw-r--r--   0        0        0     5916 2024-04-26 13:44:43.889079 jy_lib-0.6.9/jy_lib/exchange.py
--rw-r--r--   0        0        0      602 2024-04-21 14:22:14.416177 jy_lib-0.6.9/jy_lib/interrupt_protect.py
--rw-r--r--   0        0        0     2151 2024-01-01 02:29:02.556936 jy_lib-0.6.9/jy_lib/lock.py
--rw-r--r--   0        0        0      707 2024-04-21 14:22:14.416596 jy_lib-0.6.9/jy_lib/math.py
--rw-r--r--   0        0        0     5926 2024-01-01 02:29:02.557127 jy_lib-0.6.9/jy_lib/nav.py
--rw-r--r--   0        0        0    18478 2024-04-21 14:22:14.416811 jy_lib-0.6.9/jy_lib/smb_client.py
--rw-r--r--   0        0        0    22173 2024-04-26 13:44:43.889377 jy_lib-0.6.9/jy_lib/symbol.py
--rw-r--r--   0        0        0    20726 2024-04-21 14:22:14.417332 jy_lib-0.6.9/jy_lib/symbol_em.py
--rw-r--r--   0        0        0      577 2024-01-01 02:29:02.557631 jy_lib-0.6.9/jy_lib/time.py
--rw-r--r--   0        0        0       67 2024-01-01 02:29:02.557712 jy_lib-0.6.9/publish-jypi.sh
--rw-r--r--   0        0        0       67 2024-01-01 02:29:02.557791 jy_lib-0.6.9/publish-pypi.sh
--rw-r--r--   0        0        0       67 2024-01-01 02:29:02.557873 jy_lib-0.6.9/publish-test.sh
--rw-r--r--   0        0        0      639 2024-04-21 14:22:14.417488 jy_lib-0.6.9/pyproject.toml
--rw-r--r--   0        0        0      117 2024-04-21 14:22:14.417721 jy_lib-0.6.9/requirements.txt
--rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 jy_lib-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0     2083 2024-01-01 02:29:02.554641 jy_lib-0.7.0/.gitignore
+-rw-r--r--   0        0        0      285 2024-01-01 02:29:02.554755 jy_lib-0.7.0/.pypirc
+-rw-r--r--   0        0        0     1073 2024-01-01 02:29:02.555085 jy_lib-0.7.0/LICENSE
+-rw-r--r--   0        0        0      573 2024-04-21 14:22:14.414420 jy_lib-0.7.0/Pipfile
+-rw-r--r--   0        0        0    40838 2024-01-01 02:29:02.555480 jy_lib-0.7.0/Pipfile.lock
+-rw-r--r--   0        0        0       10 2024-01-01 02:29:02.555572 jy_lib-0.7.0/README.md
+-rw-r--r--   0        0        0      469 2024-01-01 02:29:02.555665 jy_lib-0.7.0/README_Project.md
+-rw-r--r--   0        0        0      518 2024-04-27 03:29:47.647616 jy_lib-0.7.0/jy_lib/__init__.py
+-rw-r--r--   0        0        0     7230 2024-01-01 02:29:02.555927 jy_lib-0.7.0/jy_lib/auth_client.py
+-rw-r--r--   0        0        0    10531 2024-01-01 02:29:02.556043 jy_lib-0.7.0/jy_lib/bank.py
+-rw-r--r--   0        0        0      809 2024-01-01 02:29:02.556135 jy_lib-0.7.0/jy_lib/base.py
+-rw-r--r--   0        0        0    11460 2024-04-26 13:44:43.888654 jy_lib-0.7.0/jy_lib/cache.py
+-rw-r--r--   0        0        0     4133 2024-04-27 03:29:36.020399 jy_lib-0.7.0/jy_lib/clickhouse.py
+-rw-r--r--   0        0        0     6202 2024-04-27 03:29:36.020586 jy_lib-0.7.0/jy_lib/compressor.py
+-rw-r--r--   0        0        0    21765 2024-01-01 02:29:02.556414 jy_lib-0.7.0/jy_lib/country.py
+-rw-r--r--   0        0        0    10928 2024-01-01 02:29:02.556554 jy_lib-0.7.0/jy_lib/currency.py
+-rw-r--r--   0        0        0     2399 2024-04-21 14:22:14.416027 jy_lib-0.7.0/jy_lib/date.py
+-rw-r--r--   0        0        0      931 2024-01-01 02:29:02.556726 jy_lib-0.7.0/jy_lib/decorator.py
+-rw-r--r--   0        0        0     5916 2024-04-26 13:44:43.889079 jy_lib-0.7.0/jy_lib/exchange.py
+-rw-r--r--   0        0        0      602 2024-04-21 14:22:14.416177 jy_lib-0.7.0/jy_lib/interrupt_protect.py
+-rw-r--r--   0        0        0     2151 2024-01-01 02:29:02.556936 jy_lib-0.7.0/jy_lib/lock.py
+-rw-r--r--   0        0        0      707 2024-04-21 14:22:14.416596 jy_lib-0.7.0/jy_lib/math.py
+-rw-r--r--   0        0        0     5926 2024-01-01 02:29:02.557127 jy_lib-0.7.0/jy_lib/nav.py
+-rw-r--r--   0        0        0    18478 2024-04-21 14:22:14.416811 jy_lib-0.7.0/jy_lib/smb_client.py
+-rw-r--r--   0        0        0    22173 2024-04-26 13:44:43.889377 jy_lib-0.7.0/jy_lib/symbol.py
+-rw-r--r--   0        0        0    20726 2024-04-21 14:22:14.417332 jy_lib-0.7.0/jy_lib/symbol_em.py
+-rw-r--r--   0        0        0      577 2024-01-01 02:29:02.557631 jy_lib-0.7.0/jy_lib/time.py
+-rw-r--r--   0        0        0       67 2024-01-01 02:29:02.557712 jy_lib-0.7.0/publish-jypi.sh
+-rw-r--r--   0        0        0       67 2024-01-01 02:29:02.557791 jy_lib-0.7.0/publish-pypi.sh
+-rw-r--r--   0        0        0       67 2024-01-01 02:29:02.557873 jy_lib-0.7.0/publish-test.sh
+-rw-r--r--   0        0        0      639 2024-04-21 14:22:14.417488 jy_lib-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      117 2024-04-21 14:22:14.417721 jy_lib-0.7.0/requirements.txt
+-rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 jy_lib-0.7.0/PKG-INFO
```

### Comparing `jy_lib-0.6.9/.gitignore` & `jy_lib-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.9/LICENSE` & `jy_lib-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.9/Pipfile` & `jy_lib-0.7.0/Pipfile`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.9/Pipfile.lock` & `jy_lib-0.7.0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.9/jy_lib/__init__.py` & `jy_lib-0.7.0/jy_lib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     SymbolFlag,
     SymbolSubType,
     SymbolType,
     WarrantsType,
 )
 from .symbol_em import EMParser, KLineRecord, TrendRecord
 
-__version__ = "0.6.9"
+__version__ = "0.7.0"
```

### Comparing `jy_lib-0.6.9/jy_lib/auth_client.py` & `jy_lib-0.7.0/jy_lib/auth_client.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.9/jy_lib/bank.py` & `jy_lib-0.7.0/jy_lib/bank.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.9/jy_lib/base.py` & `jy_lib-0.7.0/jy_lib/base.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.9/jy_lib/cache.py` & `jy_lib-0.7.0/jy_lib/cache.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.9/jy_lib/clickhouse.py` & `jy_lib-0.7.0/jy_lib/clickhouse.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,20 +3,43 @@
 import io
 import os
 import polars as pl
 import requests
 import time
 import urllib.parse
 import zstandard
-from typing import Dict
+from dataclasses import dataclass
+from typing import Dict, Type
 from loguru import logger
 from jy_lib.compressor import ZstdStreamCompressor
 from jy_lib.interrupt_protect import KeyboardInterruptProtect
 
 
+@dataclass
+class FieldDetail:
+    name: str = ''  # 字段名
+    note: str = ''  # 注释
+    dtype: Type | pl.Datetime = pl.Float64  # 数据类型
+    read_decimal: bool = None  # 读取该列时是否以decimal类型读取
+    comment: str = ''  # 备注
+    origin: bool = True  # 是否原始字段
+
+    @property
+    def ch_type(self) -> str:
+        """clickhouse中对应的数据类型"""
+        if self.dtype == pl.Datetime(time_unit='ms'):
+            return 'DateTime64(3)'
+        elif self.dtype == pl.Datetime(time_unit='us'):
+            return 'DateTime64(6)'
+        elif self.dtype == pl.Datetime(time_unit='ns'):
+            return 'DateTime64(9)'
+        else:
+            return self.dtype.base_type().__name__
+
+
 class ClickHouse:
 
     def __init__(self, url: str, http_port: int = 8123):
         self.client = clickhouse_driver.Client.from_url(url=url)
         self.http_port: int = http_port
         sp = urllib.parse.urlsplit(url)
         self.database_name: str = os.path.basename(sp.path)
```

### Comparing `jy_lib-0.6.9/jy_lib/compressor.py` & `jy_lib-0.7.0/jy_lib/compressor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 # -*- coding: utf-8 -*-
+import os.path
+import zipfile
+from typing import IO, AnyStr, Iterator
+
 import brotli
 import humanize
 import io
 import lzma
 import zlib
 import zstandard
 from enum import Enum
@@ -125,7 +129,53 @@
             try:
                 self.stream.write(self.compressor.flush())
             except Exception as e:
                 self.stream.close()
                 raise e
         else:
             self.stream.close()
+
+
+class CsvReader:
+    """多行文本分块读取器"""
+
+    @classmethod
+    def iter_zst(cls, f: AnyStr | IO, size: int = 64 * 1024 ** 2) -> Iterator[str | None, str]:
+        path: str | None = None
+        if isinstance(f, str):
+            assert os.path.isfile(f)
+            path: str = f
+            fd: IO = open(f, mode='rb')
+        else:
+            fd: IO = f
+        try:
+            decompressor = zstandard.ZstdDecompressor().stream_reader(f)
+            tail: bytes = b''
+            i: int = 0
+            while segment := decompressor.read(size):       # 每次处理size大小的多行文本
+                i += 1
+                idx: int = segment.rfind(b'\n')
+                text: bytes = tail + segment[:idx + 1]
+                tail: bytes = segment[idx + 1:]
+                text: str = text.decode('utf-8')
+                yield path, text
+        finally:
+            fd.close()
+
+    @classmethod
+    def iter_zip(cls, f: AnyStr | IO, size: int = 64 * 1024 ** 2):
+        if isinstance(f, str):
+            assert os.path.isfile(f)
+        with zipfile.ZipFile(f) as zf:
+            for zi in zf.infolist():
+                if zi.is_dir():
+                    continue
+                with zf.open(zi) as zif:
+                    tail: bytes = b''
+                    i: int = 0
+                    while segment := zif.read(size):        # 每次处理size大小的多行文本
+                        idx: int = segment.rfind(b'\n')
+                        text: bytes = tail + segment[:idx + 1]
+                        tail: bytes = segment[idx + 1:]
+                        text: str = text.decode('utf-8')
+                        yield zi.filename, text
+                        i += 1
```

### Comparing `jy_lib-0.6.9/jy_lib/country.py` & `jy_lib-0.7.0/jy_lib/country.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.9/jy_lib/currency.py` & `jy_lib-0.7.0/jy_lib/currency.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.9/jy_lib/date.py` & `jy_lib-0.7.0/jy_lib/date.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.9/jy_lib/decorator.py` & `jy_lib-0.7.0/jy_lib/decorator.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.9/jy_lib/exchange.py` & `jy_lib-0.7.0/jy_lib/exchange.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.9/jy_lib/interrupt_protect.py` & `jy_lib-0.7.0/jy_lib/interrupt_protect.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.9/jy_lib/lock.py` & `jy_lib-0.7.0/jy_lib/lock.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.9/jy_lib/math.py` & `jy_lib-0.7.0/jy_lib/math.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.9/jy_lib/nav.py` & `jy_lib-0.7.0/jy_lib/nav.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.9/jy_lib/smb_client.py` & `jy_lib-0.7.0/jy_lib/smb_client.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.9/jy_lib/symbol.py` & `jy_lib-0.7.0/jy_lib/symbol.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.9/jy_lib/symbol_em.py` & `jy_lib-0.7.0/jy_lib/symbol_em.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.9/jy_lib/time.py` & `jy_lib-0.7.0/jy_lib/time.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.9/pyproject.toml` & `jy_lib-0.7.0/pyproject.toml`

 * *Files identical despite different names*

