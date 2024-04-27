# Comparing `tmp/flask_localtunnel-1.0.6-py3-none-any.whl.zip` & `tmp/flask_localtunnel-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3096 bytes, number of entries: 6
--rw-r--r--  2.0 unx      603 b- defN 23-May-08 02:52 flask_lt.py
--rw-r--r--  2.0 unx      547 b- defN 23-May-08 03:00 flask_localtunnel-1.0.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     2337 b- defN 23-May-08 03:00 flask_localtunnel-1.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-08 03:00 flask_localtunnel-1.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-08 03:00 flask_localtunnel-1.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      501 b- defN 23-May-08 03:00 flask_localtunnel-1.0.6.dist-info/RECORD
-6 files, 4089 bytes uncompressed, 2178 bytes compressed:  46.7%
+Zip file size: 3116 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      646 b- defN 24-Apr-27 15:40 flask_lt.py
+-rw-r--r--  2.0 unx      547 b- defN 24-Apr-27 15:41 flask_localtunnel-1.0.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2336 b- defN 24-Apr-27 15:41 flask_localtunnel-1.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-27 15:41 flask_localtunnel-1.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-27 15:41 flask_localtunnel-1.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      501 b- defN 24-Apr-27 15:41 flask_localtunnel-1.0.7.dist-info/RECORD
+6 files, 4131 bytes uncompressed, 2198 bytes compressed:  46.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: flask_lt.py
 Comment: 
 
-Filename: flask_localtunnel-1.0.6.dist-info/LICENSE
+Filename: flask_localtunnel-1.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: flask_localtunnel-1.0.6.dist-info/METADATA
+Filename: flask_localtunnel-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: flask_localtunnel-1.0.6.dist-info/WHEEL
+Filename: flask_localtunnel-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: flask_localtunnel-1.0.6.dist-info/top_level.txt
+Filename: flask_localtunnel-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: flask_localtunnel-1.0.6.dist-info/RECORD
+Filename: flask_localtunnel-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flask_lt.py

```diff
@@ -1,14 +1,14 @@
 from threading import Timer
 from py_localtunnel.lt import run_localtunnel
 
-__version__ = "1.0.6"
+__version__ = "1.0.7"
 
-def run_lt(port: int, subdomain: str = None):
-    run_localtunnel(port, subdomain)
+def run_lt(port: int, subdomain: str = None, local_host: str = "127.0.0.1"):
+    run_localtunnel(port, subdomain, local_host)
 
 def start_lt(port: int, subdomain: str = None):
     lt_adress = run_lt(port, subdomain)
     print(lt_adress)
 
 def run_with_lt(app, subdomain: str = None):
     old_run = app.run
```

## Comparing `flask_localtunnel-1.0.6.dist-info/LICENSE` & `flask_localtunnel-1.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `flask_localtunnel-1.0.6.dist-info/METADATA` & `flask_localtunnel-1.0.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: flask-localtunnel
-Version: 1.0.6
+Version: 1.0.7
 Summary: A simple way to demo Flask apps from your machine.
 Home-page: https://github.com/redevil1/flask-localtunnel
 Author: Jak Bin
 Keywords: flask,flask-ngrok,ngrok,localtunnel,demo
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Flask (>=0.14.0)
+Requires-Dist: Flask >=0.14.0
 Requires-Dist: py-localtunnel
 
 # flask-localtunnel
 
  [![PyPI version](https://badge.fury.io/py/flask-localtunnel.svg)](https://badge.fury.io/py/flask-localtunnel)
  [![Downloads](https://pepy.tech/badge/flask-localtunnel/month)](https://pepy.tech/project/flask-localtunnel)
  [![Downloads](https://static.pepy.tech/personalized-badge/flask-localtunnel?period=total&units=international_system&left_color=green&right_color=blue&left_text=Total%20Downloads)](https://pepy.tech/project/flask-localtunnel)
@@ -69,13 +69,13 @@
  * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
  * localtunnel is alreadty installed.
  * your url is: https://<random-url>.loca.lt
 ```
 
 ### Support my work :-
 
-BTC - bc1qx2p08qtsxxdzj0yfr2cm7yy3g5ydv3mt2753le
+BTC - bc1qx2p08qtsxxdzj0yfr2cm7yy3g5ydv3mt2753le\
 ETH - 0x40e69DaEC18cD199535b055BDA6582daa5978145
 
 ### Contributer :- 
 - @henk717
 - @NobreHD : subdomain support
```

