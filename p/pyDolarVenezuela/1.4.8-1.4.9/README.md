# Comparing `tmp/pydolarvenezuela-1.4.8.tar.gz` & `tmp/pydolarvenezuela-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydolarvenezuela-1.4.8.tar", last modified: Fri Apr 26 00:41:28 2024, max compression
+gzip compressed data, was "pydolarvenezuela-1.4.9.tar", last modified: Fri Apr 26 15:30:02 2024, max compression
```

## Comparing `pydolarvenezuela-1.4.8.tar` & `pydolarvenezuela-1.4.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 00:41:28.895638 pydolarvenezuela-1.4.8/
--rw-rw-rw-   0        0        0     1094 2023-10-12 04:26:29.000000 pydolarvenezuela-1.4.8/LICENSE
--rw-rw-rw-   0        0        0     7276 2024-04-26 00:41:28.891677 pydolarvenezuela-1.4.8/PKG-INFO
--rw-rw-rw-   0        0        0     4885 2024-04-25 23:08:28.000000 pydolarvenezuela-1.4.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 00:41:28.739643 pydolarvenezuela-1.4.8/pyDolarVenezuela/
--rw-rw-rw-   0        0        0     2562 2024-04-26 00:40:39.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 00:41:28.780638 pydolarvenezuela-1.4.8/pyDolarVenezuela/assets/
--rw-rw-rw-   0        0        0       20 2023-11-22 01:27:36.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 00:41:28.784637 pydolarvenezuela-1.4.8/pyDolarVenezuela/assets/icons/
--rw-rw-rw-   0        0        0      927 2023-11-22 01:28:58.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela/assets/icons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 00:41:28.807643 pydolarvenezuela-1.4.8/pyDolarVenezuela/data/
--rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela/data/__init__.py
--rw-rw-rw-   0        0        0      612 2024-04-25 22:15:03.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela/data/redis.py
-drwxrwxrwx   0        0        0        0 2024-04-26 00:41:28.824656 pydolarvenezuela-1.4.8/pyDolarVenezuela/models/
--rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela/models/__init__.py
--rw-rw-rw-   0        0        0      159 2024-04-25 21:35:09.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela/models/database.py
--rw-rw-rw-   0        0        0      119 2024-04-25 23:42:45.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela/models/pages.py
--rw-rw-rw-   0        0        0      453 2023-11-23 16:38:28.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela/network.py
--rw-rw-rw-   0        0        0      716 2024-04-25 23:43:03.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela/pages.py
-drwxrwxrwx   0        0        0        0 2024-04-26 00:41:28.862637 pydolarvenezuela-1.4.8/pyDolarVenezuela/provider/
--rw-rw-rw-   0        0        0     3543 2024-04-26 00:39:52.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela/provider/__init__.py
--rw-rw-rw-   0        0        0     2159 2024-04-02 19:39:59.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela/provider/bcv.py
--rw-rw-rw-   0        0        0     2529 2024-04-02 19:27:15.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela/provider/criptodolar.py
--rw-rw-rw-   0        0        0     1842 2024-04-02 19:27:50.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela/provider/dpedidos.py
--rw-rw-rw-   0        0        0     3002 2024-04-02 19:28:10.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela/provider/exchangemonitor.py
--rw-rw-rw-   0        0        0     4136 2024-04-02 19:28:30.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela/provider/ivenezuela.py
-drwxrwxrwx   0        0        0        0 2024-04-26 00:41:28.879645 pydolarvenezuela-1.4.8/pyDolarVenezuela/tools/
--rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela/tools/__init__.py
--rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela/tools/calculator.py
--rw-rw-rw-   0        0        0     2187 2024-04-02 19:26:31.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela/tools/time.py
--rw-rw-rw-   0        0        0     1201 2023-10-17 03:57:15.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-26 00:41:28.884641 pydolarvenezuela-1.4.8/pyDolarVenezuela.egg-info/
--rw-rw-rw-   0        0        0     7276 2024-04-26 00:41:28.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      935 2024-04-26 00:41:28.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 00:41:28.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-26 00:41:28.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-26 00:41:28.000000 pydolarvenezuela-1.4.8/pyDolarVenezuela.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-04-26 00:40:34.000000 pydolarvenezuela-1.4.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-26 00:41:28.896640 pydolarvenezuela-1.4.8/setup.cfg
--rw-rw-rw-   0        0        0     1488 2024-04-26 00:40:30.000000 pydolarvenezuela-1.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:30:02.941635 pydolarvenezuela-1.4.9/
+-rw-rw-rw-   0        0        0     1094 2023-10-12 04:26:29.000000 pydolarvenezuela-1.4.9/LICENSE
+-rw-rw-rw-   0        0        0     7276 2024-04-26 15:30:02.937127 pydolarvenezuela-1.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4885 2024-04-25 23:08:28.000000 pydolarvenezuela-1.4.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 15:30:02.682415 pydolarvenezuela-1.4.9/pyDolarVenezuela/
+-rw-rw-rw-   0        0        0     2723 2024-04-26 15:28:59.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:30:02.723178 pydolarvenezuela-1.4.9/pyDolarVenezuela/assets/
+-rw-rw-rw-   0        0        0       20 2023-11-22 01:27:36.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:30:02.780931 pydolarvenezuela-1.4.9/pyDolarVenezuela/assets/icons/
+-rw-rw-rw-   0        0        0      927 2023-11-22 01:28:58.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela/assets/icons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:30:02.789558 pydolarvenezuela-1.4.9/pyDolarVenezuela/data/
+-rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela/data/__init__.py
+-rw-rw-rw-   0        0        0      684 2024-04-26 15:20:21.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela/data/redis.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:30:02.839823 pydolarvenezuela-1.4.9/pyDolarVenezuela/models/
+-rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela/models/__init__.py
+-rw-rw-rw-   0        0        0      364 2024-04-26 04:56:19.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela/models/database.py
+-rw-rw-rw-   0        0        0      318 2024-04-26 04:57:25.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela/models/pages.py
+-rw-rw-rw-   0        0        0      453 2023-11-23 16:38:28.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela/network.py
+-rw-rw-rw-   0        0        0      716 2024-04-25 23:43:03.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela/pages.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:30:02.906919 pydolarvenezuela-1.4.9/pyDolarVenezuela/provider/
+-rw-rw-rw-   0        0        0     4733 2024-04-26 15:26:49.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela/provider/__init__.py
+-rw-rw-rw-   0        0        0     2159 2024-04-02 19:39:59.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela/provider/bcv.py
+-rw-rw-rw-   0        0        0     2529 2024-04-02 19:27:15.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela/provider/criptodolar.py
+-rw-rw-rw-   0        0        0     1842 2024-04-02 19:27:50.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela/provider/dpedidos.py
+-rw-rw-rw-   0        0        0     3002 2024-04-02 19:28:10.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela/provider/exchangemonitor.py
+-rw-rw-rw-   0        0        0     4136 2024-04-02 19:28:30.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela/provider/ivenezuela.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:30:02.918918 pydolarvenezuela-1.4.9/pyDolarVenezuela/tools/
+-rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela/tools/__init__.py
+-rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela/tools/calculator.py
+-rw-rw-rw-   0        0        0     2187 2024-04-02 19:26:31.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela/tools/time.py
+-rw-rw-rw-   0        0        0     1201 2023-10-17 03:57:15.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:30:02.934127 pydolarvenezuela-1.4.9/pyDolarVenezuela.egg-info/
+-rw-rw-rw-   0        0        0     7276 2024-04-26 15:30:02.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      935 2024-04-26 15:30:02.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 15:30:02.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-26 15:30:02.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-26 15:30:02.000000 pydolarvenezuela-1.4.9/pyDolarVenezuela.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-04-26 15:28:51.000000 pydolarvenezuela-1.4.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-26 15:30:02.942636 pydolarvenezuela-1.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     1488 2024-04-26 15:28:47.000000 pydolarvenezuela-1.4.9/setup.py
```

### Comparing `pydolarvenezuela-1.4.8/LICENSE` & `pydolarvenezuela-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.8/PKG-INFO` & `pydolarvenezuela-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.4.8
+Version: 1.4.9
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
```

### Comparing `pydolarvenezuela-1.4.8/README.md` & `pydolarvenezuela-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.8/pyDolarVenezuela/__init__.py` & `pydolarvenezuela-1.4.9/pyDolarVenezuela/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,26 @@
 
 from . import network
 from .models.pages import Monitor as Page
 from .data.redis import Redis
 from .tools import get_time_zone as getdate, currency_converter
 from .provider import select_monitor
 
-version = '1.4.8'
+version = '1.4.9'
+"""
+Versión actual de la biblioteca    
+"""
 
 class CheckVersion:
+    """
+    Verificar actualización de la biblioteca    
+    ```py
+    check: bool = True
+    ```
+    """
     check = True
 
     @classmethod
     def _check_dependence_version(self):
             response = network.get("https://pypi.org/pypi/pydolarvenezuela/json")
             latest_version = json.loads(response)["info"]["version"]
```

### Comparing `pydolarvenezuela-1.4.8/pyDolarVenezuela/assets/icons/__init__.py` & `pydolarvenezuela-1.4.9/pyDolarVenezuela/assets/icons/__init__.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.8/pyDolarVenezuela/data/redis.py` & `pydolarvenezuela-1.4.9/pyDolarVenezuela/data/redis.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,9 +11,12 @@
     
     def set_data(self, key: str, value: Any, ttl: int = None):
         self.r.set(key, value)
         
         if ttl is not None:
             self.r.expire(key, ttl)
     
+    def delete_data(self, key: str):
+        self.r.delete(key)
+    
     def get_data(self, key: str) -> Any:
         return self.r.get(key)
```

### Comparing `pydolarvenezuela-1.4.8/pyDolarVenezuela/pages.py` & `pydolarvenezuela-1.4.9/pyDolarVenezuela/pages.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.8/pyDolarVenezuela/provider/__init__.py` & `pydolarvenezuela-1.4.9/pyDolarVenezuela/provider/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -39,41 +39,59 @@
         if monitor_class is not None:
             if db is not None:
                 response = monitor_class(provider.provider, currency).get_values()
 
                 key = f'{currency}:{provider.name}'
                 cache = Cache(db)
 
-                if not cache.get_data(key):
+                existing_data = cache.get_data(key)
+
+                if not existing_data:
                     cache.set_data(key, json.dumps(response), db.ttl)
+                else:
+                    existing_data_dict: dict[str, dict] = json.loads(existing_data)
+                    for name in existing_data_dict:
+                        if not name == 'last_update':
+                            if existing_data_dict[name]['price'] != response[name]['price']:
+                                price = existing_data_dict[name]['price']
+                                new_price = response[name]['price']
+                                change  = round(float(new_price - price), 2)
+                                percent = f'{round(float((change / new_price) * 100 if price != 0 else 0), 2)}%'
+                                symbol  = "" if change == 0 else "▲" if change >= 0 else "▼"
+                                color   = "red" if symbol == '▼' else "green" if symbol == '▲' else "neutral"
+                                last_update = None if provider.name == B.name else response[name]['last_update']
+
+                                if not provider.name == B.name:
+                                    existing_data_dict[name].update({
+                                        'price': new_price,
+                                        'change': change,
+                                        'percent': percent,
+                                        'color': color,
+                                        'symbol': symbol,
+                                        'last_update': last_update
+                                    })
+                                else:
+                                    existing_data_dict[name].update({
+                                        'price': new_price,
+                                        'change': change,
+                                        'percent': percent,
+                                        'color': color,
+                                        'symbol': symbol,
+                                    })
                 
-                get_data = dict(json.loads(cache.get_data(key)))
-                for name in get_data:
-                    if not name == 'last_update':
-                        price   = get_data[name]['price']
-                        change  = round(float(response[name]['price'] - price), 2)
-                        percent = f'{round(float((change / price) * 100 if price != 0 else 0), 2)}%'
-                        symbol  = "" if change == 0 else "▲" if change >= 0 else "▼"
-                        color   = "red" if symbol == '▼' else "green" if symbol == '▲' else "neutral"
-                        
-                        get_data[name].update({
-                            'price': price,
-                            'change': change,
-                            'percent': percent,
-                            'color': color,
-                            'symbol': symbol
-                        })
-                        
-                    cache.set_data(key, json.dumps(get_data), db.ttl)
-                
+                cache.set_data(key, json.dumps(existing_data_dict), db.ttl)
+                existing_data_dict: dict[str, dict] = json.loads(
+                    cache.get_data(key)
+                )
+
                 if not monitor_code:
-                    return get_data
+                    return existing_data_dict
                 
                 try:
-                    monitor_data = get_data[monitor_code.lower()]
+                    monitor_data = existing_data_dict[monitor_code.lower()]
                     if name_property:
                         value = monitor_data[name_property]
                         return f'Bs. {value}' if prettify and name_property == 'price' else value
                     return monitor_data
                 except KeyError:
                     raise KeyError("Does not match any of the properties that were provided in the dictionary. Most information: https://github.com/fcoagz/pyDolarVenezuela")
```

### Comparing `pydolarvenezuela-1.4.8/pyDolarVenezuela/provider/bcv.py` & `pydolarvenezuela-1.4.9/pyDolarVenezuela/provider/bcv.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.8/pyDolarVenezuela/provider/criptodolar.py` & `pydolarvenezuela-1.4.9/pyDolarVenezuela/provider/criptodolar.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.8/pyDolarVenezuela/provider/dpedidos.py` & `pydolarvenezuela-1.4.9/pyDolarVenezuela/provider/dpedidos.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.8/pyDolarVenezuela/provider/exchangemonitor.py` & `pydolarvenezuela-1.4.9/pyDolarVenezuela/provider/exchangemonitor.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.8/pyDolarVenezuela/provider/ivenezuela.py` & `pydolarvenezuela-1.4.9/pyDolarVenezuela/provider/ivenezuela.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.8/pyDolarVenezuela/tools/calculator.py` & `pydolarvenezuela-1.4.9/pyDolarVenezuela/tools/calculator.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.8/pyDolarVenezuela/tools/time.py` & `pydolarvenezuela-1.4.9/pyDolarVenezuela/tools/time.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.8/pyDolarVenezuela/utils.py` & `pydolarvenezuela-1.4.9/pyDolarVenezuela/utils.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.8/pyDolarVenezuela.egg-info/PKG-INFO` & `pydolarvenezuela-1.4.9/pyDolarVenezuela.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.4.8
+Version: 1.4.9
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
```

### Comparing `pydolarvenezuela-1.4.8/pyDolarVenezuela.egg-info/SOURCES.txt` & `pydolarvenezuela-1.4.9/pyDolarVenezuela.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.8/pyproject.toml` & `pydolarvenezuela-1.4.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyDolarVenezuela"
-version = "1.4.8"
+version = "1.4.9"
 dependencies = [
   "requests",
   "curl_cffi",
   "beautifulsoup4",
   "babel",
   "pytz",
   "colorama",
```

### Comparing `pydolarvenezuela-1.4.8/setup.py` & `pydolarvenezuela-1.4.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.4.8'
+VERSION = '1.4.9'
 PACKAGE_NAME = 'pyDolarVenezuela' 
 AUTHOR = 'Francisco Griman'
 AUTHOR_EMAIL = 'grihardware@gmail.com'
 URL = 'https://github.com/fcoagz/pydolarvenezuela'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'esta es una librería en python que te permite consultar los precios del dólar en diferentes monitores en Venezuela y el dolar oficial BCV.'
```

