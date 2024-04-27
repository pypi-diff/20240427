# Comparing `tmp/pyxt-0.6.8.tar.gz` & `tmp/pyxt-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxt-0.6.8.tar", last modified: Tue Dec 19 07:30:10 2023, max compression
+gzip compressed data, was "pyxt-0.6.9.tar", last modified: Tue Dec 19 09:34:57 2023, max compression
```

## Comparing `pyxt-0.6.8.tar` & `pyxt-0.6.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 itadmin   (1000) itadmin   (1000)        0 2023-12-19 07:30:10.196181 pyxt-0.6.8/
--rw-rw-r--   0 itadmin   (1000) itadmin   (1000)     1217 2023-12-11 09:54:28.000000 pyxt-0.6.8/LICENSE
--rw-rw-r--   0 itadmin   (1000) itadmin   (1000)     2319 2023-12-19 07:30:10.196181 pyxt-0.6.8/PKG-INFO
--rw-rw-r--   0 itadmin   (1000) itadmin   (1000)     1622 2023-12-12 07:04:10.000000 pyxt-0.6.8/README.md
-drwxrwxr-x   0 itadmin   (1000) itadmin   (1000)        0 2023-12-19 07:30:10.196181 pyxt-0.6.8/pyxt/
--rw-rw-r--   0 itadmin   (1000) itadmin   (1000)    17789 2023-12-19 06:33:21.000000 pyxt-0.6.8/pyxt/perp.py
--rw-rw-r--   0 itadmin   (1000) itadmin   (1000)    25773 2023-12-19 07:30:07.000000 pyxt-0.6.8/pyxt/spot.py
-drwxrwxr-x   0 itadmin   (1000) itadmin   (1000)        0 2023-12-19 07:30:10.196181 pyxt-0.6.8/pyxt/websocket/
--rw-rw-r--   0 itadmin   (1000) itadmin   (1000)     5236 2023-12-13 07:18:04.000000 pyxt-0.6.8/pyxt/websocket/perp.py
--rw-rw-r--   0 itadmin   (1000) itadmin   (1000)     3658 2023-12-13 07:18:04.000000 pyxt-0.6.8/pyxt/websocket/spot.py
--rw-rw-r--   0 itadmin   (1000) itadmin   (1000)     7572 2023-12-13 07:18:04.000000 pyxt-0.6.8/pyxt/websocket/xt_websocket.py
-drwxrwxr-x   0 itadmin   (1000) itadmin   (1000)        0 2023-12-19 07:30:10.196181 pyxt-0.6.8/pyxt.egg-info/
--rw-rw-r--   0 itadmin   (1000) itadmin   (1000)     2319 2023-12-19 07:30:10.000000 pyxt-0.6.8/pyxt.egg-info/PKG-INFO
--rw-rw-r--   0 itadmin   (1000) itadmin   (1000)      305 2023-12-19 07:30:10.000000 pyxt-0.6.8/pyxt.egg-info/SOURCES.txt
--rw-rw-r--   0 itadmin   (1000) itadmin   (1000)        1 2023-12-19 07:30:10.000000 pyxt-0.6.8/pyxt.egg-info/dependency_links.txt
--rw-rw-r--   0 itadmin   (1000) itadmin   (1000)        1 2023-12-19 06:33:42.000000 pyxt-0.6.8/pyxt.egg-info/not-zip-safe
--rw-rw-r--   0 itadmin   (1000) itadmin   (1000)       20 2023-12-19 07:30:10.000000 pyxt-0.6.8/pyxt.egg-info/requires.txt
--rw-rw-r--   0 itadmin   (1000) itadmin   (1000)        5 2023-12-19 07:30:10.000000 pyxt-0.6.8/pyxt.egg-info/top_level.txt
--rw-rw-r--   0 itadmin   (1000) itadmin   (1000)      131 2023-12-19 07:30:10.196181 pyxt-0.6.8/setup.cfg
--rw-rw-r--   0 itadmin   (1000) itadmin   (1000)     1091 2023-12-19 07:30:07.000000 pyxt-0.6.8/setup.py
+drwxrwxr-x   0 itadmin   (1000) itadmin   (1000)        0 2023-12-19 09:34:57.763005 pyxt-0.6.9/
+-rw-rw-r--   0 itadmin   (1000) itadmin   (1000)     1217 2023-12-11 09:54:28.000000 pyxt-0.6.9/LICENSE
+-rw-rw-r--   0 itadmin   (1000) itadmin   (1000)     2319 2023-12-19 09:34:57.763005 pyxt-0.6.9/PKG-INFO
+-rw-rw-r--   0 itadmin   (1000) itadmin   (1000)     1622 2023-12-12 07:04:10.000000 pyxt-0.6.9/README.md
+drwxrwxr-x   0 itadmin   (1000) itadmin   (1000)        0 2023-12-19 09:34:57.763005 pyxt-0.6.9/pyxt/
+-rw-rw-r--   0 itadmin   (1000) itadmin   (1000)    18053 2023-12-19 09:34:54.000000 pyxt-0.6.9/pyxt/perp.py
+-rw-rw-r--   0 itadmin   (1000) itadmin   (1000)    25773 2023-12-19 07:30:07.000000 pyxt-0.6.9/pyxt/spot.py
+drwxrwxr-x   0 itadmin   (1000) itadmin   (1000)        0 2023-12-19 09:34:57.763005 pyxt-0.6.9/pyxt/websocket/
+-rw-rw-r--   0 itadmin   (1000) itadmin   (1000)     5236 2023-12-13 07:18:04.000000 pyxt-0.6.9/pyxt/websocket/perp.py
+-rw-rw-r--   0 itadmin   (1000) itadmin   (1000)     3658 2023-12-13 07:18:04.000000 pyxt-0.6.9/pyxt/websocket/spot.py
+-rw-rw-r--   0 itadmin   (1000) itadmin   (1000)     7572 2023-12-13 07:18:04.000000 pyxt-0.6.9/pyxt/websocket/xt_websocket.py
+drwxrwxr-x   0 itadmin   (1000) itadmin   (1000)        0 2023-12-19 09:34:57.763005 pyxt-0.6.9/pyxt.egg-info/
+-rw-rw-r--   0 itadmin   (1000) itadmin   (1000)     2319 2023-12-19 09:34:57.000000 pyxt-0.6.9/pyxt.egg-info/PKG-INFO
+-rw-rw-r--   0 itadmin   (1000) itadmin   (1000)      305 2023-12-19 09:34:57.000000 pyxt-0.6.9/pyxt.egg-info/SOURCES.txt
+-rw-rw-r--   0 itadmin   (1000) itadmin   (1000)        1 2023-12-19 09:34:57.000000 pyxt-0.6.9/pyxt.egg-info/dependency_links.txt
+-rw-rw-r--   0 itadmin   (1000) itadmin   (1000)        1 2023-12-19 06:33:42.000000 pyxt-0.6.9/pyxt.egg-info/not-zip-safe
+-rw-rw-r--   0 itadmin   (1000) itadmin   (1000)       20 2023-12-19 09:34:57.000000 pyxt-0.6.9/pyxt.egg-info/requires.txt
+-rw-rw-r--   0 itadmin   (1000) itadmin   (1000)        5 2023-12-19 09:34:57.000000 pyxt-0.6.9/pyxt.egg-info/top_level.txt
+-rw-rw-r--   0 itadmin   (1000) itadmin   (1000)      131 2023-12-19 09:34:57.763005 pyxt-0.6.9/setup.cfg
+-rw-rw-r--   0 itadmin   (1000) itadmin   (1000)     1091 2023-12-19 09:34:54.000000 pyxt-0.6.9/setup.py
```

### Comparing `pyxt-0.6.8/LICENSE` & `pyxt-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxt-0.6.8/PKG-INFO` & `pyxt-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyxt
-Version: 0.6.8
+Version: 0.6.9
 Summary: Python3 XT.COM HTTP API Connector
 Home-page: https://github.com/kelvinxue/pyxt
-Download-URL: https://github.com/kelvinxue/pyxt/archive/refs/tags/v0.6.8.tar.gz
+Download-URL: https://github.com/kelvinxue/pyxt/archive/refs/tags/v0.6.9.tar.gz
 Author: xt
 Author-email: xt@xt.com
 License: MIT License
 Keywords: xt api connector
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pyxt-0.6.8/README.md` & `pyxt-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `pyxt-0.6.8/pyxt/perp.py` & `pyxt-0.6.9/pyxt/perp.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,32 +225,34 @@
         url = self.host + path
         params = {}
         header = self._create_sign(self.__access_key, self.__secret_key, path=path, method="get", bodymod=bodymod,
                                    params=params)
         code, success, error = self._fetch(method="GET", url=url, headers=header, params=params, timeout=self.timeout)
         return code, success, error
 
-    def send_order(self, symbol, price, amount, order_side, order_type, position_side):
+    def send_order(self, symbol, amount, order_side, order_type, position_side, price=None):
         """
         :return: send order
         """
         params = {"orderSide": order_side,
                   "orderType": order_type,
                   "origQty": amount,
                   "positionSide": position_side,
-                  "symbol": symbol,
-                  "price": price}
+                  "symbol": symbol
+                  }
+        if price:
+            params["price"] = price
 
         bodymod = "application/x-www-form-urlencoded"
         path = "/future/trade" + '/v1/order/create'
         url = self.host + path
 
         header = self._create_sign(self.__access_key, self.__secret_key, path=path, method="post", bodymod=bodymod,
                                    params=params)
-        code, success, error = self._fetch(method="POST", url=url, headers=header, params=params, timeout=self.timeout)
+        code, success, error = self._fetch(method="POST", url=url, headers=header, body=params, timeout=self.timeout)
         return code, success, error
 
     def get_account_order(self, symbol, state, page, size):
         """
         state:
         NEW
         PARTIALLY_FILLED
@@ -411,11 +413,16 @@
         header = self._create_sign(self.__access_key, self.__secret_key, path=path, method="post", bodymod=bodymod,
                                    params=params)
         code, success, error = self._fetch(method="POST", url=url, headers=header, body=params, timeout=self.timeout)
         return code, success, error
 
 
 if __name__ == '__main__':
+    symbol_xt = 'btc_usdt'
+    quantity = 5
     host = "https://fapi.xt.com"
     access_key = ""
     secret_key = ""
     xt_perp = Perp(host, access_key, secret_key)
+    result = xt_perp.send_order(symbol=symbol_xt, amount=quantity, order_side='BUY', order_type='MARKET',
+                                position_side='LONG')
+    print(result)
```

### Comparing `pyxt-0.6.8/pyxt/spot.py` & `pyxt-0.6.9/pyxt/spot.py`

 * *Files identical despite different names*

### Comparing `pyxt-0.6.8/pyxt/websocket/perp.py` & `pyxt-0.6.9/pyxt/websocket/perp.py`

 * *Files identical despite different names*

### Comparing `pyxt-0.6.8/pyxt/websocket/spot.py` & `pyxt-0.6.9/pyxt/websocket/spot.py`

 * *Files identical despite different names*

### Comparing `pyxt-0.6.8/pyxt/websocket/xt_websocket.py` & `pyxt-0.6.9/pyxt/websocket/xt_websocket.py`

 * *Files identical despite different names*

### Comparing `pyxt-0.6.8/pyxt.egg-info/PKG-INFO` & `pyxt-0.6.9/pyxt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyxt
-Version: 0.6.8
+Version: 0.6.9
 Summary: Python3 XT.COM HTTP API Connector
 Home-page: https://github.com/kelvinxue/pyxt
-Download-URL: https://github.com/kelvinxue/pyxt/archive/refs/tags/v0.6.8.tar.gz
+Download-URL: https://github.com/kelvinxue/pyxt/archive/refs/tags/v0.6.9.tar.gz
 Author: xt
 Author-email: xt@xt.com
 License: MIT License
 Keywords: xt api connector
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pyxt-0.6.8/setup.py` & `pyxt-0.6.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='pyxt',
-    version='0.6.8',
+    version='0.6.9',
     description='Python3 XT.COM HTTP API Connector',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kelvinxue/pyxt",
-    download_url='https://github.com/kelvinxue/pyxt/archive/refs/tags/v0.6.8.tar.gz',
+    download_url='https://github.com/kelvinxue/pyxt/archive/refs/tags/v0.6.9.tar.gz',
     license="MIT License",
     author="xt",
     author_email="xt@xt.com",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

