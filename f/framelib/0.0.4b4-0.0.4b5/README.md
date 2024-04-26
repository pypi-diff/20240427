# Comparing `tmp/framelib-0.0.4b4.tar.gz` & `tmp/framelib-0.0.4b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "framelib-0.0.4b4.tar", last modified: Fri Apr 26 13:33:27 2024, max compression
+gzip compressed data, was "framelib-0.0.4b5.tar", last modified: Fri Apr 26 21:54:18 2024, max compression
```

## Comparing `framelib-0.0.4b4.tar` & `framelib-0.0.4b5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 13:33:27.225939 framelib-0.0.4b4/
--rw-r--r--   0 devin     (1000) devin     (1000)     1847 2024-04-26 13:33:27.225939 framelib-0.0.4b4/PKG-INFO
--rw-rw-r--   0 devin     (1000) devin     (1000)     1233 2024-03-20 13:38:58.000000 framelib-0.0.4b4/README.md
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 13:33:27.221938 framelib-0.0.4b4/framelib/
--rw-rw-r--   0 devin     (1000) devin     (1000)      388 2024-04-26 13:27:11.000000 framelib-0.0.4b4/framelib/__init__.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     2038 2024-04-26 13:26:27.000000 framelib-0.0.4b4/framelib/frame.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     3263 2024-04-26 13:33:16.000000 framelib-0.0.4b4/framelib/hub.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     3174 2024-04-26 13:21:35.000000 framelib-0.0.4b4/framelib/models.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     3195 2024-04-26 13:15:55.000000 framelib-0.0.4b4/framelib/neynar.py
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 13:33:27.225939 framelib-0.0.4b4/framelib/templates/
--rw-rw-r--   0 devin     (1000) devin     (1000)     2356 2024-03-13 12:40:19.000000 framelib-0.0.4b4/framelib/templates/frame.html
--rw-rw-r--   0 devin     (1000) devin     (1000)     1578 2024-03-20 13:38:58.000000 framelib-0.0.4b4/framelib/transaction.py
--rw-rw-r--   0 devin     (1000) devin     (1000)      380 2024-02-26 15:07:40.000000 framelib-0.0.4b4/framelib/warpcast.py
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 13:33:27.225939 framelib-0.0.4b4/framelib.egg-info/
--rw-r--r--   0 devin     (1000) devin     (1000)     1847 2024-04-26 13:33:27.000000 framelib-0.0.4b4/framelib.egg-info/PKG-INFO
--rw-rw-r--   0 devin     (1000) devin     (1000)      431 2024-04-26 13:33:27.000000 framelib-0.0.4b4/framelib.egg-info/SOURCES.txt
--rw-rw-r--   0 devin     (1000) devin     (1000)        1 2024-04-26 13:33:27.000000 framelib-0.0.4b4/framelib.egg-info/dependency_links.txt
--rw-rw-r--   0 devin     (1000) devin     (1000)       83 2024-04-26 13:33:27.000000 framelib-0.0.4b4/framelib.egg-info/requires.txt
--rw-rw-r--   0 devin     (1000) devin     (1000)       14 2024-04-26 13:33:27.000000 framelib-0.0.4b4/framelib.egg-info/top_level.txt
--rw-rw-r--   0 devin     (1000) devin     (1000)       38 2024-04-26 13:33:27.225939 framelib-0.0.4b4/setup.cfg
--rw-rw-r--   0 devin     (1000) devin     (1000)      917 2024-04-26 13:27:31.000000 framelib-0.0.4b4/setup.py
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 13:33:27.225939 framelib-0.0.4b4/test/
--rw-rw-r--   0 devin     (1000) devin     (1000)        0 2024-02-26 19:53:14.000000 framelib-0.0.4b4/test/__init__.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     3316 2024-03-20 13:38:58.000000 framelib-0.0.4b4/test/test_render.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     5252 2024-03-20 13:38:58.000000 framelib-0.0.4b4/test/test_transaction.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     2675 2024-04-26 13:15:55.000000 framelib-0.0.4b4/test/test_validation.py
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 21:54:18.289369 framelib-0.0.4b5/
+-rw-r--r--   0 devin     (1000) devin     (1000)     1847 2024-04-26 21:54:18.289369 framelib-0.0.4b5/PKG-INFO
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1233 2024-03-20 13:38:58.000000 framelib-0.0.4b5/README.md
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 21:54:18.289369 framelib-0.0.4b5/framelib/
+-rw-rw-r--   0 devin     (1000) devin     (1000)      388 2024-04-26 13:27:11.000000 framelib-0.0.4b5/framelib/__init__.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2050 2024-04-26 14:46:05.000000 framelib-0.0.4b5/framelib/frame.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3310 2024-04-26 21:44:52.000000 framelib-0.0.4b5/framelib/hub.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3174 2024-04-26 13:21:35.000000 framelib-0.0.4b5/framelib/models.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3293 2024-04-26 21:44:52.000000 framelib-0.0.4b5/framelib/neynar.py
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 21:54:18.289369 framelib-0.0.4b5/framelib/templates/
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2356 2024-03-13 12:40:19.000000 framelib-0.0.4b5/framelib/templates/frame.html
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1578 2024-03-20 13:38:58.000000 framelib-0.0.4b5/framelib/transaction.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)      380 2024-02-26 15:07:40.000000 framelib-0.0.4b5/framelib/warpcast.py
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 21:54:18.289369 framelib-0.0.4b5/framelib.egg-info/
+-rw-r--r--   0 devin     (1000) devin     (1000)     1847 2024-04-26 21:54:18.000000 framelib-0.0.4b5/framelib.egg-info/PKG-INFO
+-rw-rw-r--   0 devin     (1000) devin     (1000)      431 2024-04-26 21:54:18.000000 framelib-0.0.4b5/framelib.egg-info/SOURCES.txt
+-rw-rw-r--   0 devin     (1000) devin     (1000)        1 2024-04-26 21:54:18.000000 framelib-0.0.4b5/framelib.egg-info/dependency_links.txt
+-rw-rw-r--   0 devin     (1000) devin     (1000)       83 2024-04-26 21:54:18.000000 framelib-0.0.4b5/framelib.egg-info/requires.txt
+-rw-rw-r--   0 devin     (1000) devin     (1000)       14 2024-04-26 21:54:18.000000 framelib-0.0.4b5/framelib.egg-info/top_level.txt
+-rw-rw-r--   0 devin     (1000) devin     (1000)       38 2024-04-26 21:54:18.289369 framelib-0.0.4b5/setup.cfg
+-rw-rw-r--   0 devin     (1000) devin     (1000)      917 2024-04-26 21:49:32.000000 framelib-0.0.4b5/setup.py
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 21:54:18.289369 framelib-0.0.4b5/test/
+-rw-rw-r--   0 devin     (1000) devin     (1000)        0 2024-02-26 19:53:14.000000 framelib-0.0.4b5/test/__init__.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3316 2024-03-20 13:38:58.000000 framelib-0.0.4b5/test/test_render.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     5252 2024-03-20 13:38:58.000000 framelib-0.0.4b5/test/test_transaction.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2675 2024-04-26 13:15:55.000000 framelib-0.0.4b5/test/test_validation.py
```

### Comparing `framelib-0.0.4b4/PKG-INFO` & `framelib-0.0.4b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: framelib
-Version: 0.0.4b4
+Version: 0.0.4b5
 Summary: lightweight library for building farcaster frames using python and flask
 Home-page: https://github.com/devinaconley/python-frames
 Author: Devin A. Conley
 Author-email: devinaconley@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `framelib-0.0.4b4/README.md` & `framelib-0.0.4b5/README.md`

 * *Files identical despite different names*

### Comparing `framelib-0.0.4b4/framelib/frame.py` & `framelib-0.0.4b5/framelib/frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,14 @@
 def message() -> FrameMessage:
     # parse action message
     body = json.loads(request.data)
     msg = FrameMessage(**body)
     return msg
 
 
-def error(text: str, status: int = 400):
+def error(text: str, status: int = 400) -> Response:
     if len(text) > 90:
         print('warning: error message exceeds 90 characters')
     e = FrameError(message=text)
     res = jsonify(e.model_dump())
     res.status_code = status
     return res
```

### Comparing `framelib-0.0.4b4/framelib/hub.py` & `framelib-0.0.4b5/framelib/hub.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,21 +20,23 @@
     url = f'{hub}/v1/validateMessage'
     headers = {'content-type': 'application/octet-stream'}
     if api_key:
         headers['api_key'] = api_key
     auth = None
     if username:
         auth = (username, password)
-    print(url)
+
     res = requests.post(url, headers=headers, auth=auth, data=bytes.fromhex(msg))
-    print(res)
-    print(res.text)
+
+    if res.status_code != 200:
+        raise ValueError(f'failed request to hub: {res.text}')
     body = res.json()
     if not body['valid']:
         raise ValueError('frame action message is invalid')
+
     action = ValidatedMessage(**body['message'])
 
     return action
 
 
 def validate_message(
         msg: FrameMessage,
```

### Comparing `framelib-0.0.4b4/framelib/models.py` & `framelib-0.0.4b5/framelib/models.py`

 * *Files identical despite different names*

### Comparing `framelib-0.0.4b4/framelib/neynar.py` & `framelib-0.0.4b5/framelib/neynar.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,16 +22,19 @@
         'message_bytes_in_hex': msg
     }
     headers = {
         'accept': 'application/json',
         'api_key': api_key,
         'content-type': 'application/json'
     }
+
     res = requests.post(url, json=body, headers=headers)
 
+    if res.status_code != 200:
+        raise ValueError(f'failed request to neynar: {res.text}')
     body = res.json()
     if not body['valid']:
         raise ValueError('frame action message is invalid')
 
     action = NeynarValidatedMessage(**body['action'])
 
     return action
```

### Comparing `framelib-0.0.4b4/framelib/templates/frame.html` & `framelib-0.0.4b5/framelib/templates/frame.html`

 * *Files identical despite different names*

### Comparing `framelib-0.0.4b4/framelib/transaction.py` & `framelib-0.0.4b5/framelib/transaction.py`

 * *Files identical despite different names*

### Comparing `framelib-0.0.4b4/framelib.egg-info/PKG-INFO` & `framelib-0.0.4b5/framelib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: framelib
-Version: 0.0.4b4
+Version: 0.0.4b5
 Summary: lightweight library for building farcaster frames using python and flask
 Home-page: https://github.com/devinaconley/python-frames
 Author: Devin A. Conley
 Author-email: devinaconley@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `framelib-0.0.4b4/setup.py` & `framelib-0.0.4b5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='framelib',
-    version='0.0.4b4',
+    version='0.0.4b5',
     author='Devin A. Conley',
     author_email='devinaconley@gmail.com',
     description='lightweight library for building farcaster frames using python and flask',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/devinaconley/python-frames',
     packages=setuptools.find_packages(),
```

### Comparing `framelib-0.0.4b4/test/test_render.py` & `framelib-0.0.4b5/test/test_render.py`

 * *Files identical despite different names*

### Comparing `framelib-0.0.4b4/test/test_transaction.py` & `framelib-0.0.4b5/test/test_transaction.py`

 * *Files identical despite different names*

### Comparing `framelib-0.0.4b4/test/test_validation.py` & `framelib-0.0.4b5/test/test_validation.py`

 * *Files identical despite different names*

