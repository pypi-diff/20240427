# Comparing `tmp/stream-inflate-0.0.8.tar.gz` & `tmp/stream-inflate-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stream-inflate-0.0.8.tar", last modified: Tue Oct 19 20:21:55 2021, max compression
+gzip compressed data, was "stream-inflate-0.0.9.tar", last modified: Thu Oct 21 05:59:42 2021, max compression
```

## Comparing `stream-inflate-0.0.8.tar` & `stream-inflate-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-10-19 20:21:55.291136 stream-inflate-0.0.8/
--rw-r--r--   0 dituser    (501) staff       (20)     1072 2021-10-16 13:36:12.000000 stream-inflate-0.0.8/LICENSE
--rw-r--r--   0 dituser    (501) staff       (20)     2064 2021-10-19 20:21:55.290804 stream-inflate-0.0.8/PKG-INFO
--rw-r--r--   0 dituser    (501) staff       (20)     1563 2021-10-19 20:14:37.000000 stream-inflate-0.0.8/README.md
--rw-r--r--   0 dituser    (501) staff       (20)       38 2021-10-19 20:21:55.291242 stream-inflate-0.0.8/setup.cfg
--rw-r--r--   0 dituser    (501) staff       (20)      717 2021-10-19 20:21:13.000000 stream-inflate-0.0.8/setup.py
-drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-10-19 20:21:55.290394 stream-inflate-0.0.8/stream_inflate.egg-info/
--rw-r--r--   0 dituser    (501) staff       (20)     2064 2021-10-19 20:21:55.000000 stream-inflate-0.0.8/stream_inflate.egg-info/PKG-INFO
--rw-r--r--   0 dituser    (501) staff       (20)      196 2021-10-19 20:21:55.000000 stream-inflate-0.0.8/stream_inflate.egg-info/SOURCES.txt
--rw-r--r--   0 dituser    (501) staff       (20)        1 2021-10-19 20:21:55.000000 stream-inflate-0.0.8/stream_inflate.egg-info/dependency_links.txt
--rw-r--r--   0 dituser    (501) staff       (20)       15 2021-10-19 20:21:55.000000 stream-inflate-0.0.8/stream_inflate.egg-info/top_level.txt
--rw-r--r--   0 dituser    (501) staff       (20)    10667 2021-10-19 20:18:19.000000 stream-inflate-0.0.8/stream_inflate.py
+drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-10-21 05:59:42.419802 stream-inflate-0.0.9/
+-rw-r--r--   0 dituser    (501) staff       (20)     1072 2021-10-16 13:36:12.000000 stream-inflate-0.0.9/LICENSE
+-rw-r--r--   0 dituser    (501) staff       (20)     2064 2021-10-21 05:59:42.419468 stream-inflate-0.0.9/PKG-INFO
+-rw-r--r--   0 dituser    (501) staff       (20)     1563 2021-10-19 20:14:37.000000 stream-inflate-0.0.9/README.md
+-rw-r--r--   0 dituser    (501) staff       (20)       38 2021-10-21 05:59:42.419894 stream-inflate-0.0.9/setup.cfg
+-rw-r--r--   0 dituser    (501) staff       (20)      717 2021-10-21 05:59:11.000000 stream-inflate-0.0.9/setup.py
+drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-10-21 05:59:42.419099 stream-inflate-0.0.9/stream_inflate.egg-info/
+-rw-r--r--   0 dituser    (501) staff       (20)     2064 2021-10-21 05:59:42.000000 stream-inflate-0.0.9/stream_inflate.egg-info/PKG-INFO
+-rw-r--r--   0 dituser    (501) staff       (20)      196 2021-10-21 05:59:42.000000 stream-inflate-0.0.9/stream_inflate.egg-info/SOURCES.txt
+-rw-r--r--   0 dituser    (501) staff       (20)        1 2021-10-21 05:59:42.000000 stream-inflate-0.0.9/stream_inflate.egg-info/dependency_links.txt
+-rw-r--r--   0 dituser    (501) staff       (20)       15 2021-10-21 05:59:42.000000 stream-inflate-0.0.9/stream_inflate.egg-info/top_level.txt
+-rw-r--r--   0 dituser    (501) staff       (20)    12038 2021-10-21 05:54:02.000000 stream-inflate-0.0.9/stream_inflate.py
```

### Comparing `stream-inflate-0.0.8/LICENSE` & `stream-inflate-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stream-inflate-0.0.8/PKG-INFO` & `stream-inflate-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stream-inflate
-Version: 0.0.8
+Version: 0.0.9
 Summary: Uncompress DEFLATE streams in pure Python
 Home-page: https://github.com/michalc/stream-inflate
 Author: Michal Charemza
 Author-email: michal@charemza.name
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `stream-inflate-0.0.8/README.md` & `stream-inflate-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `stream-inflate-0.0.8/setup.py` & `stream-inflate-0.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
 
 setuptools.setup(
     name='stream-inflate',
-    version='0.0.8',
+    version='0.0.9',
     author='Michal Charemza',
     author_email='michal@charemza.name',
     description='Uncompress DEFLATE streams in pure Python',
     long_description=long_description(),
     long_description_content_type='text/markdown',
     url='https://github.com/michalc/stream-inflate',
     classifiers=[
```

### Comparing `stream-inflate-0.0.8/stream_inflate.egg-info/PKG-INFO` & `stream-inflate-0.0.9/stream_inflate.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stream-inflate
-Version: 0.0.8
+Version: 0.0.9
 Summary: Uncompress DEFLATE streams in pure Python
 Home-page: https://github.com/michalc/stream-inflate
 Author: Michal Charemza
 Author-email: michal@charemza.name
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `stream-inflate-0.0.8/stream_inflate.py` & `stream-inflate-0.0.9/stream_inflate.py`

 * *Files 16% similar despite different names*

```diff
@@ -115,31 +115,59 @@
 
         def _get_end_index():
             return offset_byte + (1 if offset_bit else 0)
 
         return _get_bits, _get_bytes, _yield_bytes, _get_end_index
 
     def get_backwards_cache(size):
-        cache = b''
+        cache = bytearray(size)
+        cache_start = 0
+        cache_len = 0
 
         def via_cache(bytes_iter):
-            nonlocal cache
+            nonlocal cache, cache_start, cache_len
+
             for chunk in bytes_iter:
-                cache = (cache + chunk)[-size:]
+                chunk_start = max(len(chunk) - size, 0)
+                chunk_end = len(chunk)
+                chunk_len = chunk_end - chunk_start
+                part_1_start = (cache_start + cache_len) % size
+                part_1_end = min(part_1_start + chunk_len, size)
+                part_1_chunk_start = chunk_start
+                part_1_chunk_end = chunk_start + (part_1_end - part_1_start)
+                part_2_start = 0
+                part_2_end = chunk_len - (part_1_end - part_1_start)
+                part_2_chunk_start = part_1_chunk_end
+                part_2_chunk_end = part_1_chunk_end + (part_2_end - part_2_start)
+
+                cache_len_over_size = max((cache_len + chunk_len) - size, 0)
+                cache_len = min(size, cache_len + chunk_len)
+                cache_start = (cache_start + cache_len_over_size) % size
+
+                cache[part_1_start:part_1_end] = chunk[part_1_chunk_start:part_1_chunk_end]
+                cache[part_2_start:part_2_end] = chunk[part_2_chunk_start:part_2_chunk_end]
+
                 yield chunk
 
         def from_cache(dist, length):
-            if dist > len(cache):
+            if dist > cache_len:
                 raise Exception('Searching backwards too far', dist, len(cache))
 
-            start = len(cache) - dist
-            end = max(start + length, len(cache))
-            chunk = cache[start:end]
+            available = dist
+            part_1_start = (cache_start + cache_len - dist) % size
+            part_1_end = min(part_1_start + available, size)
+            part_2_start = 0
+            part_2_end = max(available - (part_1_end - part_1_start), 0)
+
             while length:
-                to_yield = chunk[:length]
+                to_yield = cache[part_1_start:part_1_end][:length]
+                yield to_yield
+                length -= len(to_yield)
+
+                to_yield = cache[part_2_start:part_2_end][:length]
                 yield to_yield
                 length -= len(to_yield)
 
         return via_cache, from_cache
 
     def get_huffman_decoder(get_bits, lengths):
```

