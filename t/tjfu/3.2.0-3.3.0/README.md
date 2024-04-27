# Comparing `tmp/tjfu-3.2.0.tar.gz` & `tmp/tjfu-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tjfu-3.2.0.tar", last modified: Fri Apr 26 18:01:37 2024, max compression
+gzip compressed data, was "tjfu-3.3.0.tar", last modified: Sat Apr 27 18:18:38 2024, max compression
```

## Comparing `tjfu-3.2.0.tar` & `tjfu-3.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 duynguyen  (1000) duynguyen  (1000)        0 2024-04-26 18:01:37.613239 tjfu-3.2.0/
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)     8624 2024-04-26 18:01:37.613239 tjfu-3.2.0/PKG-INFO
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)     8058 2024-04-26 17:58:26.000000 tjfu-3.2.0/README.md
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)       38 2024-04-26 18:01:37.613239 tjfu-3.2.0/setup.cfg
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)     1224 2024-04-25 19:29:35.000000 tjfu-3.2.0/setup.py
-drwxrwxr-x   0 duynguyen  (1000) duynguyen  (1000)        0 2024-04-26 18:01:37.613239 tjfu-3.2.0/tjfu/
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)      114 2024-04-25 19:29:52.000000 tjfu-3.2.0/tjfu/__init__.py
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)     1222 2024-04-25 19:28:34.000000 tjfu-3.2.0/tjfu/route.py
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)      490 2024-04-25 19:28:34.000000 tjfu-3.2.0/tjfu/tj_socket.py
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)      461 2024-04-26 17:22:09.000000 tjfu-3.2.0/tjfu/tj_utils.py
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)     9900 2024-04-26 17:52:20.000000 tjfu-3.2.0/tjfu/tjfu.py
-drwxrwxr-x   0 duynguyen  (1000) duynguyen  (1000)        0 2024-04-26 18:01:37.613239 tjfu-3.2.0/tjfu.egg-info/
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)     8624 2024-04-26 18:01:37.000000 tjfu-3.2.0/tjfu.egg-info/PKG-INFO
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)      236 2024-04-26 18:01:37.000000 tjfu-3.2.0/tjfu.egg-info/SOURCES.txt
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)        1 2024-04-26 18:01:37.000000 tjfu-3.2.0/tjfu.egg-info/dependency_links.txt
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)       65 2024-04-26 18:01:37.000000 tjfu-3.2.0/tjfu.egg-info/requires.txt
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)        5 2024-04-26 18:01:37.000000 tjfu-3.2.0/tjfu.egg-info/top_level.txt
+drwxrwxr-x   0 duynguyen  (1000) duynguyen  (1000)        0 2024-04-27 18:18:38.288163 tjfu-3.3.0/
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)     9219 2024-04-27 18:18:38.284163 tjfu-3.3.0/PKG-INFO
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)     8653 2024-04-27 18:12:52.000000 tjfu-3.3.0/README.md
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)       38 2024-04-27 18:18:38.288163 tjfu-3.3.0/setup.cfg
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)     1224 2024-04-25 19:29:35.000000 tjfu-3.3.0/setup.py
+drwxrwxr-x   0 duynguyen  (1000) duynguyen  (1000)        0 2024-04-27 18:18:38.284163 tjfu-3.3.0/tjfu/
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)      114 2024-04-27 17:58:28.000000 tjfu-3.3.0/tjfu/__init__.py
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)     1222 2024-04-25 19:28:34.000000 tjfu-3.3.0/tjfu/route.py
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)      490 2024-04-25 19:28:34.000000 tjfu-3.3.0/tjfu/tj_socket.py
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)      461 2024-04-26 17:22:09.000000 tjfu-3.3.0/tjfu/tj_utils.py
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)    10462 2024-04-27 17:57:19.000000 tjfu-3.3.0/tjfu/tjfu.py
+drwxrwxr-x   0 duynguyen  (1000) duynguyen  (1000)        0 2024-04-27 18:18:38.284163 tjfu-3.3.0/tjfu.egg-info/
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)     9219 2024-04-27 18:18:38.000000 tjfu-3.3.0/tjfu.egg-info/PKG-INFO
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)      236 2024-04-27 18:18:38.000000 tjfu-3.3.0/tjfu.egg-info/SOURCES.txt
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)        1 2024-04-27 18:18:38.000000 tjfu-3.3.0/tjfu.egg-info/dependency_links.txt
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)       65 2024-04-27 18:18:38.000000 tjfu-3.3.0/tjfu.egg-info/requires.txt
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)        5 2024-04-27 18:18:38.000000 tjfu-3.3.0/tjfu.egg-info/top_level.txt
```

### Comparing `tjfu-3.2.0/PKG-INFO` & `tjfu-3.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tjfu
-Version: 3.2.0
+Version: 3.3.0
 Summary: Python library helps optimize Flask development to be flexible and object-oriented.
 Home-page: https://github.com/duynguyen02/tjfu
 Author: Duy Nguyen
 License: UNKNOWN
 Keywords: Python,Flask
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -66,16 +66,16 @@
     .add_status_code_handler(500, error_500) # optional (>=3.2.0)
     .limiter_storage_uri("memory://") # optinal (default: 'memory://')
     .default_limits(["200 per day", "50 per hour"]) # optinal (default: '[]')
     .log_output(False) # optinal (default: 'True')
     .debug(False) # optinal (default: 'True')
     .use_reloader(False) # optinal (default: 'True')
     .allow_unsafe_werkzeug(False) # optinal (default: 'True')
-    .app_config('MY_SECRET_KEY', 'my_secret_key') # optional (>=3.2.0): use as app['MY_SECRET_KEY'] = 'my_secret_key'
-    .app_config('MY_SECRET_KEY_2', 'my_secret_key') # optional (>=3.2.0): use as app['MY_SECRET_KEY_2'] = 'my_secret_key'
+    .app_config('MY_SECRET_KEY', 'my_secret_key') # optional (>=3.2.0): use as app.config['MY_SECRET_KEY'] = 'my_secret_key'
+    .app_config('MY_SECRET_KEY_2', 'my_secret_key') # optional (>=3.2.0): use as app.config['MY_SECRET_KEY_2'] = 'my_secret_key'
     .build()
 }
 
 from tjfu import Route
 
 app = TJFU.init_app(Route("index", "/"))
 
@@ -198,14 +198,41 @@
 Get Flask App after TJFU.build() (>=3.2.0)
 ```Python
 # Example
 from tjfu import TJFU
 from flask_mail import Mail, Message
 mail = Mail(TJFU.app())
 ```
+Get Extensions (JWT/Limiter/SocketIO) after TJFU.build() (>=3.3.0)
+```Python
+TJFU.jwt()
+TJFU.limiter()
+TJFU.socketio()
+```
+Add custom extensions to TJFU after TJFU.build() (>=3.3.0)
+```Python
+# OTHER CODE...
+
+from flask_mail import Mail, Message
+mail = Mail(TJFU.app())
+
+TJFU.add_extension(
+    'send_mail',
+    mail
+) 
+
+app = TJFU.init_app(index_route)
+
+# OTHER CODE...
+```
+And then you can take it out and use it in contexts (e.g. Route)
+```Python
+mail = TJFU.get_extension('send_mail')
+```
+
 Define a Socket Handle:
 ```Python
 # OTHER CODE...
 
 from tjfu import SocketEvent, SocketHandle
 from flask import request
 class MySocketHandle(SocketHandle):
@@ -284,9 +311,9 @@
 ### Changelog
 - `1.0.0`: First version released. There is a problem in Socket implementation.
 - `2.0.0`: Edit the Socket structure. There is a problem deploying the application to the production environment.
 - `3.0.0`: The version is relatively stable, overcoming the problem of deploying applications in production environments.
 - `3.1.0`: Added the function of registering Routes using Routes Map
 - `3.1.1`: Fixed an issue where additional variables could not be added when inheriting the _index function in Route.
 - `3.2.0`: Assign keys/values to Flask App Config using TJFU.app_config(...,...), add function TJFU.app() to get Flask App after calling TJFU.build(), use the add_status_code_handler function instead of the add_error_handler function.
-
+- `3.3.0`: Build functions that take instances of extensions and add custom extensions.
```

### Comparing `tjfu-3.2.0/README.md` & `tjfu-3.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -49,16 +49,16 @@
     .add_status_code_handler(500, error_500) # optional (>=3.2.0)
     .limiter_storage_uri("memory://") # optinal (default: 'memory://')
     .default_limits(["200 per day", "50 per hour"]) # optinal (default: '[]')
     .log_output(False) # optinal (default: 'True')
     .debug(False) # optinal (default: 'True')
     .use_reloader(False) # optinal (default: 'True')
     .allow_unsafe_werkzeug(False) # optinal (default: 'True')
-    .app_config('MY_SECRET_KEY', 'my_secret_key') # optional (>=3.2.0): use as app['MY_SECRET_KEY'] = 'my_secret_key'
-    .app_config('MY_SECRET_KEY_2', 'my_secret_key') # optional (>=3.2.0): use as app['MY_SECRET_KEY_2'] = 'my_secret_key'
+    .app_config('MY_SECRET_KEY', 'my_secret_key') # optional (>=3.2.0): use as app.config['MY_SECRET_KEY'] = 'my_secret_key'
+    .app_config('MY_SECRET_KEY_2', 'my_secret_key') # optional (>=3.2.0): use as app.config['MY_SECRET_KEY_2'] = 'my_secret_key'
     .build()
 }
 
 from tjfu import Route
 
 app = TJFU.init_app(Route("index", "/"))
 
@@ -181,14 +181,41 @@
 Get Flask App after TJFU.build() (>=3.2.0)
 ```Python
 # Example
 from tjfu import TJFU
 from flask_mail import Mail, Message
 mail = Mail(TJFU.app())
 ```
+Get Extensions (JWT/Limiter/SocketIO) after TJFU.build() (>=3.3.0)
+```Python
+TJFU.jwt()
+TJFU.limiter()
+TJFU.socketio()
+```
+Add custom extensions to TJFU after TJFU.build() (>=3.3.0)
+```Python
+# OTHER CODE...
+
+from flask_mail import Mail, Message
+mail = Mail(TJFU.app())
+
+TJFU.add_extension(
+    'send_mail',
+    mail
+) 
+
+app = TJFU.init_app(index_route)
+
+# OTHER CODE...
+```
+And then you can take it out and use it in contexts (e.g. Route)
+```Python
+mail = TJFU.get_extension('send_mail')
+```
+
 Define a Socket Handle:
 ```Python
 # OTHER CODE...
 
 from tjfu import SocketEvent, SocketHandle
 from flask import request
 class MySocketHandle(SocketHandle):
@@ -267,7 +294,8 @@
 ### Changelog
 - `1.0.0`: First version released. There is a problem in Socket implementation.
 - `2.0.0`: Edit the Socket structure. There is a problem deploying the application to the production environment.
 - `3.0.0`: The version is relatively stable, overcoming the problem of deploying applications in production environments.
 - `3.1.0`: Added the function of registering Routes using Routes Map
 - `3.1.1`: Fixed an issue where additional variables could not be added when inheriting the _index function in Route.
 - `3.2.0`: Assign keys/values to Flask App Config using TJFU.app_config(...,...), add function TJFU.app() to get Flask App after calling TJFU.build(), use the add_status_code_handler function instead of the add_error_handler function.
+- `3.3.0`: Build functions that take instances of extensions and add custom extensions.
```

### Comparing `tjfu-3.2.0/setup.py` & `tjfu-3.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `tjfu-3.2.0/tjfu/route.py` & `tjfu-3.3.0/tjfu/route.py`

 * *Files identical despite different names*

### Comparing `tjfu-3.2.0/tjfu/tjfu.py` & `tjfu-3.3.0/tjfu/tjfu.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,14 +54,16 @@
     
     # error handler
     _ERROR_HANDLER: dict[int, any] = {}
     
     # app config
     _APP_CONFIG = {}
     
+    # extensions
+    _EXTENSIONS = {}
     
     def _after_build_func(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             if TJFU._FLASK_APP is None:
                 raise Exception("TJFU has not been built yet, please call TJFU.build() before using this function.")
             return func(*args, **kwargs)
@@ -82,14 +84,36 @@
     
     @staticmethod
     @_after_build_func
     def app():
         return TJFU._FLASK_APP
     
     @staticmethod
+    @_after_build_func
+    def jwt():
+        return TJFU._JWT
+    
+    @staticmethod
+    @_after_build_func
+    def socketio():
+        return TJFU._SOCKET_IO
+    
+    @staticmethod
+    @_after_build_func
+    def add_extension(key: str, ext):
+        TJFU._EXTENSIONS[key] = ext
+        
+    @staticmethod
+    @_after_build_func
+    def get_extension(key: str):
+        if key in TJFU._EXTENSIONS:
+            return TJFU._EXTENSIONS[key]
+        raise ValueError(f"Not found: {key} extension.")
+        
+    @staticmethod
     @_build_func
     def app_config(key: str, value: str):
         TJFU._APP_CONFIG[key] = value
         return TJFU
     
     @staticmethod
     @_build_func
```

### Comparing `tjfu-3.2.0/tjfu.egg-info/PKG-INFO` & `tjfu-3.3.0/tjfu.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tjfu
-Version: 3.2.0
+Version: 3.3.0
 Summary: Python library helps optimize Flask development to be flexible and object-oriented.
 Home-page: https://github.com/duynguyen02/tjfu
 Author: Duy Nguyen
 License: UNKNOWN
 Keywords: Python,Flask
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -66,16 +66,16 @@
     .add_status_code_handler(500, error_500) # optional (>=3.2.0)
     .limiter_storage_uri("memory://") # optinal (default: 'memory://')
     .default_limits(["200 per day", "50 per hour"]) # optinal (default: '[]')
     .log_output(False) # optinal (default: 'True')
     .debug(False) # optinal (default: 'True')
     .use_reloader(False) # optinal (default: 'True')
     .allow_unsafe_werkzeug(False) # optinal (default: 'True')
-    .app_config('MY_SECRET_KEY', 'my_secret_key') # optional (>=3.2.0): use as app['MY_SECRET_KEY'] = 'my_secret_key'
-    .app_config('MY_SECRET_KEY_2', 'my_secret_key') # optional (>=3.2.0): use as app['MY_SECRET_KEY_2'] = 'my_secret_key'
+    .app_config('MY_SECRET_KEY', 'my_secret_key') # optional (>=3.2.0): use as app.config['MY_SECRET_KEY'] = 'my_secret_key'
+    .app_config('MY_SECRET_KEY_2', 'my_secret_key') # optional (>=3.2.0): use as app.config['MY_SECRET_KEY_2'] = 'my_secret_key'
     .build()
 }
 
 from tjfu import Route
 
 app = TJFU.init_app(Route("index", "/"))
 
@@ -198,14 +198,41 @@
 Get Flask App after TJFU.build() (>=3.2.0)
 ```Python
 # Example
 from tjfu import TJFU
 from flask_mail import Mail, Message
 mail = Mail(TJFU.app())
 ```
+Get Extensions (JWT/Limiter/SocketIO) after TJFU.build() (>=3.3.0)
+```Python
+TJFU.jwt()
+TJFU.limiter()
+TJFU.socketio()
+```
+Add custom extensions to TJFU after TJFU.build() (>=3.3.0)
+```Python
+# OTHER CODE...
+
+from flask_mail import Mail, Message
+mail = Mail(TJFU.app())
+
+TJFU.add_extension(
+    'send_mail',
+    mail
+) 
+
+app = TJFU.init_app(index_route)
+
+# OTHER CODE...
+```
+And then you can take it out and use it in contexts (e.g. Route)
+```Python
+mail = TJFU.get_extension('send_mail')
+```
+
 Define a Socket Handle:
 ```Python
 # OTHER CODE...
 
 from tjfu import SocketEvent, SocketHandle
 from flask import request
 class MySocketHandle(SocketHandle):
@@ -284,9 +311,9 @@
 ### Changelog
 - `1.0.0`: First version released. There is a problem in Socket implementation.
 - `2.0.0`: Edit the Socket structure. There is a problem deploying the application to the production environment.
 - `3.0.0`: The version is relatively stable, overcoming the problem of deploying applications in production environments.
 - `3.1.0`: Added the function of registering Routes using Routes Map
 - `3.1.1`: Fixed an issue where additional variables could not be added when inheriting the _index function in Route.
 - `3.2.0`: Assign keys/values to Flask App Config using TJFU.app_config(...,...), add function TJFU.app() to get Flask App after calling TJFU.build(), use the add_status_code_handler function instead of the add_error_handler function.
-
+- `3.3.0`: Build functions that take instances of extensions and add custom extensions.
```

